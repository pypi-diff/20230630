# Comparing `tmp/drekar_launch-0.1.2-py3-none-any.whl.zip` & `tmp/drekar_launch-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 14945 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    31054 b- defN 23-Jun-13 01:48 drekar_launch.py
--rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-13 02:01 drekar_launch-0.1.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5450 b- defN 23-Jun-13 02:01 drekar_launch-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 02:01 drekar_launch-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 23-Jun-13 02:01 drekar_launch-0.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-13 02:01 drekar_launch-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      596 b- defN 23-Jun-13 02:01 drekar_launch-0.1.2.dist-info/RECORD
-7 files, 48813 bytes uncompressed, 13881 bytes compressed:  71.6%
+Zip file size: 16476 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    39182 b- defN 23-Jun-17 06:45 drekar_launch.py
+-rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-30 07:23 drekar_launch-0.1.3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5450 b- defN 23-Jun-30 07:23 drekar_launch-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 07:23 drekar_launch-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Jun-30 07:23 drekar_launch-0.1.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-30 07:23 drekar_launch-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      596 b- defN 23-Jun-30 07:23 drekar_launch-0.1.3.dist-info/RECORD
+7 files, 56941 bytes uncompressed, 15412 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: drekar_launch.py
 Comment: 
 
-Filename: drekar_launch-0.1.2.dist-info/LICENSE.txt
+Filename: drekar_launch-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: drekar_launch-0.1.2.dist-info/METADATA
+Filename: drekar_launch-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: drekar_launch-0.1.2.dist-info/WHEEL
+Filename: drekar_launch-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: drekar_launch-0.1.2.dist-info/entry_points.txt
+Filename: drekar_launch-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: drekar_launch-0.1.2.dist-info/top_level.txt
+Filename: drekar_launch-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: drekar_launch-0.1.2.dist-info/RECORD
+Filename: drekar_launch-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drekar_launch.py

```diff
@@ -14,14 +14,15 @@
 from pathlib import Path
 import sys
 from datetime import datetime
 import os
 import time
 import signal
 import subprocess
+import uuid
 import jinja2
 import drekar_launch_process
 
 
 class DrekarTask(NamedTuple):
     name: str
     program: str
@@ -68,15 +69,15 @@
                 if not self._keep_going:
                     return
             while self._keep_going:
                 try:
                     self.parent.process_state_changed(s.name,ProcessState.START_PENDING)
                     stderr_log.write(f"Starting process {s.name}...\n")
                     python_exe = sys.executable
-                    self._process = await create_subprocess_exec(s.program, s.args, s.environment, s.cwd)
+                    self._process = await create_subprocess_exec(s.program, s.args, s.environment, s.cwd, self.parent.cgroup)
                     # print(f"process pid: {self._process.pid}")
                     stderr_log.write(f"Process {s.name} started\n\n")                   
                     self.parent.process_state_changed(s.name,ProcessState.RUNNING)
                     stdout_read_task = asyncio.ensure_future(self._process.stdout.readline())
                     stderr_read_task = asyncio.ensure_future(self._process.stderr.readline())
                     while True: #self._keep_going:
                         wait_tasks = list(filter(lambda x: x is not None, [stdout_read_task, stderr_read_task]))
@@ -160,14 +161,20 @@
         self.log_dir = log_dir
         self.loop = loop
         self.screen=screen
 
         self._subprocesses = dict()
         self._lock = threading.RLock()
         self.exit_event = exit_event
+        self.cgroup = None
+
+        if sys.platform == "linux":
+            self.cgroup = _linux_cgroupv2_launch_scope()
+            self.cgroup.create_launcher_cgroup()
+
 
     def _do_start(self,s):
         p = DrekarProcess(self, s, self.log_dir, self.loop)
         self._subprocesses[s.name] = p
         self.loop.create_task(p.run())
 
     def start_all(self):
@@ -194,28 +201,28 @@
                 with self._lock:
                     if process_name in self._subprocesses:
                         del self._subprocesses[process_name]
 
     def check_deps_status(self, deps):
         return True
 
-    def close(self):
+    def stop_all(self):
         with self._lock:
             if self._closed:
                 return
             self._closed = True
 
             for p in self._subprocesses.values():
                 try:
                     p.close()
                 except Exception:
                     traceback.print_exc()
                     pass
 
-    async def wait_all_closed(self):
+    async def wait_all_stopped(self):
         try:
             t1 = time.time()
             t_last_sent_close = 0
             while True:
                 t_diff = time.time() - t1
                 if t_diff > 15:
                     break
@@ -259,17 +266,21 @@
     def get_exit_status(self):
         exit_status = 0
         with self._lock:
             for p in self._subprocesses.values():
                 if p.exit_status != 0:
                     exit_status = p.exit_status
         return exit_status
+    
+    def close(self):
+        if sys.platform == "linux":
+            self.cgroup.close()
 
 
-async def create_subprocess_exec(process, args, env, cwd):
+async def create_subprocess_exec(process, args, env, cwd, launcher_cgroup=None):
     if sys.platform == "win32":
         job_handle = subprocess_impl_win32.win32_create_job_object()
 
         process = await asyncio.create_subprocess_exec(process,*args, \
             stdout=asyncio.subprocess.PIPE,stderr=asyncio.subprocess.PIPE,\
             env=env, cwd=cwd, creationflags=subprocess_impl_win32.CREATE_SUSPENDED \
             | subprocess.CREATE_NEW_PROCESS_GROUP 
@@ -280,21 +291,25 @@
         return DrekarSubprocessImpl(process,job_handle)
 
     else:
         #TODO: Use "start_new_session=True" arg for new process
         process = await asyncio.create_subprocess_exec(process,*args, \
             stdout=asyncio.subprocess.PIPE,stderr=asyncio.subprocess.PIPE,\
             env=env, cwd=cwd, close_fds=True, start_new_session=True )
+        if sys.platform == "linux" and launcher_cgroup is not None:
+            task_cgroup = launcher_cgroup.create_task_cgroup(process.pid)
+            return DrekarSubprocessImpl(process, task_cgroup = task_cgroup)
         return DrekarSubprocessImpl(process)
 
 
 class DrekarSubprocessImpl:
-    def __init__(self, asyncio_subprocess, job_handle = None):
+    def __init__(self, asyncio_subprocess, job_handle = None, task_cgroup = None):
         self._process = asyncio_subprocess
         self._job_handle = job_handle
+        self._task_cgroup = task_cgroup
         # TODO: Linux
 
     @property
     def process(self):
         return self._process
 
     @property
@@ -326,19 +341,19 @@
             pid = self._process.pid
             pgid = os.getpgid(pid)
             os.killpg(pgid, signal.SIGINT)
 
     def close(self):
         if sys.platform == "win32":            
             subprocess_impl_win32.win32_close_job_object(self._job_handle)
+        elif sys.platform == "linux" and self._task_cgroup:            
+            self._task_cgroup.close()
         else:
-            try:
+            with suppress(Exception):
                 self._process.kill()
-            except Exception:
-                pass
 
     def get_exit_status(self):
         return self._process.returncode
 
 
 if sys.platform == "win32":
     import ctypes.wintypes
@@ -536,14 +551,204 @@
         def _win32_send_ctrl_c_event(pid):
             if isinstance(pid, list):
                 for p in pid:
                     subprocess_impl_win32._win32_send_ctrl_c_event(p)
                 return
             ctypes.windll.kernel32.GenerateConsoleCtrlEvent(0,pid)
 
+if sys.platform == "linux":
+
+    class _linux_cgroupv2_launch_scope:
+
+        @staticmethod
+        def cgroupv2_supported():
+            if Path("/sys/fs/cgroup/cgroup.controllers").exists():
+                return True
+            return False
+
+        def __init__(self):
+            self._pid = os.getpid()
+            self.cgroup_parent_path = None
+            self.cgroup_path = None
+
+            if not self.cgroupv2_supported():
+                return
+            
+            self.cgroup_parent_path = _linux_cgroupv2_launch_scope.read_proc_cgroup(self._pid)
+
+            self.sentinel_process = None
+
+        @staticmethod
+        def read_proc_cgroup(pid):
+            cgroup_path = None
+            try:
+                # read cgroup path from /proc/{pid}/cgroup
+                with open(f"/proc/{pid}/cgroup","r") as f:
+                    for line in f:
+                        if line.startswith("0::/"):
+                            path1 = line.split(":")[2]
+                            if path1.strip() == "/":
+                                # Not currently assigned to a cgroup
+                                break
+                            cgroup_path = Path("/sys/fs/cgroup") / Path(path1.strip().strip("/"))
+                            break
+            except:
+                # TODO: log error
+                traceback.print_exc()
+                pass
+
+            return cgroup_path
+        
+        def create_launcher_cgroup(self):
+            if not self.cgroupv2_supported():
+                return
+            
+            # create a new cgroup scope for this launcher with the name drekar-launch-{random_uuid}.scope
+            try:
+                cgroup_name = f"drekar-launch-{uuid.uuid4().hex}.scope"
+                cgroup_path = self.cgroup_parent_path / cgroup_name
+                # TODO: log
+                # print(f"Creating cgroup {cgroup_path}")
+                cgroup_path.mkdir()
+                self.cgroup_path = cgroup_path
+
+                enable_sentinel_environ = os.environ.get("DREKAR_LAUNCH_ENABLE_SENTINEL", "1").strip().lower()
+                if enable_sentinel_environ == "1" or enable_sentinel_environ == "true":
+                    self.start_sentinel()
+            except:
+                traceback.print_exc()
+                pass
+
+        def create_task_cgroup(self, task_pid):
+            task_name = f"task-{task_pid}"
+            if self.cgroup_path is None:
+                return _linux_cgroupv2_task_scope(None, task_name, task_pid)
+            
+            task_cgroup = _linux_cgroupv2_task_scope(self.cgroup_path, task_name, task_pid)
+            task_cgroup.create_task_cgroup()
+            return task_cgroup
+        
+        @staticmethod
+        def close_cgroup_path(cgroup_path):
+            try:
+                #Iterate through all subdirectories and recursively close them
+                for subpath in cgroup_path.iterdir():
+                    if subpath.is_dir():
+                        _linux_cgroupv2_launch_scope.close_cgroup_path(subpath)
+                cgroup_kill_path = cgroup_path / "cgroup.kill"
+                if cgroup_kill_path.exists():
+                    with open(cgroup_kill_path,"w") as f:
+                        f.write("1")
+                    pass
+                    time.sleep(0.1)
+                cgroup_path.rmdir()
+            except:
+                traceback.print_exc()
+                pass
+
+        def close(self):
+            if self.cgroup_path is not None:
+                # Iterate through all subdirectories depth first
+
+                self.close_cgroup_path(self.cgroup_path)
+
+                self.cgroup_path = None
+
+                if self.sentinel_process is not None:
+                    self.stop_sentinel()
+
+        def start_sentinel(self):
+            if self.sentinel_process is not None:
+                return
+            
+            sentinel_environ = os.environ.copy()
+            sentinel_environ["DREKAR_LAUNCH_ENABLE_SENTINEL"] = "0"
+            self.sentinel_process=subprocess.Popen([sys.executable, "-m", "drekar_launch", "--sentinel", str(os.getpid()), str(self.cgroup_path)], 
+                                                    env=sentinel_environ, close_fds=True, start_new_session=True)
+            
+        def stop_sentinel(self):
+            if self.sentinel_process is None:
+                return
+            try:                
+                os.killpg(self.sentinel_process.pid, signal.SIGTERM)
+            except:
+                pass
+
+        def __enter__(self):
+            self.create_launcher_cgroup()
+            return self
+        
+        def __exit__(self, exc_type, exc_value, traceback):
+            self.close()
+
+
+    class _linux_cgroupv2_task_scope:
+        def __init__(self, cgroup_path, task_name, task_pid):
+            self.cgroup_path = cgroup_path
+            self.task_name = task_name
+            self.task_pid = task_pid
+            self.task_cgroup_path = None
+
+        def create_task_cgroup(self):
+            if self.cgroup_path is None:
+                return
+            
+            self.task_cgroup_path = self.cgroup_path / f"{self.task_name}.scope"
+            self.task_cgroup_path.mkdir()
+            # Move task to new cgroup
+            with open(self.task_cgroup_path / "cgroup.procs","w") as f:
+                f.write(str(self.task_pid))
+            
+        def close(self):
+            if self.task_cgroup_path is not None:
+                task_cgroup_kill_path = self.task_cgroup_path / "cgroup.kill"
+                if task_cgroup_kill_path.exists():
+                    with open(task_cgroup_kill_path,"w") as f:
+                        f.write("1")
+                    pass
+                self.task_cgroup_path.rmdir()
+                self.task_cgroup_path = None
+
+        def __enter__(self):
+            self.create_task_cgroup()
+            return self
+        
+        def __exit__(self, exc_type, exc_value, traceback):
+            self.close()
+
+    def _sentinel_main():
+        if not _linux_cgroupv2_launch_scope.cgroupv2_supported():
+            return
+        assert len(sys.argv) >= 4
+        assert sys.argv[1] == "--sentinel"
+        parent_pid = int(sys.argv[2])
+        parent_cgroup_path = Path(sys.argv[3])
+        parent_pid_proc_path = Path(f"/proc/{parent_pid}")
+        evt = threading.Event()
+        drekar_launch_process.wait_exit_callback(lambda: evt.set())
+        while True:
+            evt.wait(15)
+            if evt.is_set():
+                break
+            if not parent_cgroup_path.exists():
+                return
+            
+            # Check if parent process is still alive
+            if not parent_pid_proc_path.exists():
+                break            
+            
+        # Parent process is dead, close cgroup
+        if not parent_cgroup_path.exists():
+            return
+        time.sleep(10)
+        if not parent_cgroup_path.exists():
+            return
+        _linux_cgroupv2_launch_scope.close_cgroup_path(Path(parent_cgroup_path))
+
+
 def parse_task_launch_from_yaml(yaml_dict, cwd):
     # parse yaml_dict into DrekarTask tuple
     name = yaml_dict["name"]
     program = yaml_dict["program"]
     cwd = yaml_dict.get("cwd", cwd)
     args = yaml_dict.get("args", None)
     if args is None:
@@ -708,14 +913,21 @@
     config_text = jinja2_env.from_string(config_text).render(**extra_args)
     yaml_dict = yaml.safe_load(config_text)
     name, task_launches = parse_task_launches_from_yaml_dict(yaml_dict, cwd)
 
     return name, task_launches
 
 def main():
+
+    # Run the sentinel if requsted on linux
+    if sys.platform == "linux" and "--sentinel" in sys.argv:
+        _sentinel_main()
+        return
+
+    core = None
     try:
         parser = argparse.ArgumentParser("PyRI Core Launcher")
         parser.add_argument("--config", type=str, default=None, help="Configuration file")
         parser.add_argument("--config-j2", type=str, default=None, help="Configuration file (jinja2 template)")
         parser.add_argument("--cwd", type=str, default=".", help="Working directory")
         parser.add_argument("--name", type=str, default=None, help="Name of the launch")
         parser.add_argument("--quiet", action="store_true", help="Echo output to screen")
@@ -742,44 +954,48 @@
 
         name = parser_results.name if parser_results.name is not None else name
         if name is None:
             name = "drekar-launch"
 
         timestamp = datetime.now().strftime("-%Y-%m-%d--%H-%M-%S")
         log_dir = Path(appdirs.user_log_dir(appname="drekar-launch")).joinpath(name).joinpath(name + timestamp)
-        log_dir.mkdir(parents=True, exist_ok=True)        
-        loop = asyncio.get_event_loop()
+        log_dir.mkdir(parents=True, exist_ok=True)
+        
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)        
                         
         exit_event = asyncio.Event()
         core = DrekarCore(parser_results.name, task_launch, exit_event, log_dir, not parser_results.quiet, loop)
         gui = None
         if parser_results.gui:
             gui = DrekarGui(name, core, exit_event)
             gui.start()
         loop.call_soon(lambda: core.start_all())
         def ctrl_c_pressed():
             loop.call_soon_threadsafe(lambda: exit_event.set())
-            loop.call_soon_threadsafe(lambda: core.close())
         drekar_launch_process.wait_exit_callback(ctrl_c_pressed)
         print("Press Ctrl-C to exit")        
         loop.run_until_complete(exit_event.wait())
         print("Exit received, closing")
-        core.close()
-        loop.run_until_complete(core.wait_all_closed())
+        core.stop_all()
+        loop.run_until_complete(core.wait_all_stopped())
         #pending = asyncio.all_tasks(loop)
         # pending = asyncio.all_tasks()
         #loop.run_until_complete(asyncio.gather(*pending))
         if gui is not None:
             gui.close()
         print("Exiting!")
         exit_status = core.get_exit_status()
         if exit_status != 0:
             print(f"Exit status: {exit_status}")
         sys.exit(exit_status)
     except Exception:
         traceback.print_exc()
         raise
+    finally:
+        if core is not None:
+            core.close()
     
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `drekar_launch-0.1.2.dist-info/LICENSE.txt` & `drekar_launch-0.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `drekar_launch-0.1.2.dist-info/METADATA` & `drekar_launch-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drekar-launch
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple launcher for Robotics applications
 Author-email: John Wason <wason@wasontech.com>
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml
```

## Comparing `drekar_launch-0.1.2.dist-info/RECORD` & `drekar_launch-0.1.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-drekar_launch.py,sha256=JrvyCd5geZVJ082Lnt1QwmQTwFnmaI1HD4UC9bw9cjg,31054
-drekar_launch-0.1.2.dist-info/LICENSE.txt,sha256=Tl1tRxWGtrUEp-8aQr9k8kNBVeVc0FnOcSY8m7eKPfc,11554
-drekar_launch-0.1.2.dist-info/METADATA,sha256=j5H51YeoJD3GvLpSbXSctPUaL-1BrqE8dr25AtTG3xw,5450
-drekar_launch-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drekar_launch-0.1.2.dist-info/entry_points.txt,sha256=6tYJlxAt1he_nlcz1XIWGuG25TY3CHKXlLz3IdOMG6I,53
-drekar_launch-0.1.2.dist-info/top_level.txt,sha256=RgrbC56bqzVppX9z-Js4DoCjJWX2O9yw1dDjzoqILfY,14
-drekar_launch-0.1.2.dist-info/RECORD,,
+drekar_launch.py,sha256=CtIKFk5ZDtD9uLvA4sqtV3pjQy0Q9CxI4DOe-F9Q1TA,39182
+drekar_launch-0.1.3.dist-info/LICENSE.txt,sha256=Tl1tRxWGtrUEp-8aQr9k8kNBVeVc0FnOcSY8m7eKPfc,11554
+drekar_launch-0.1.3.dist-info/METADATA,sha256=P6YnYRTD5PNnd4gM4anl5ZyY0kiQMDSqqPMKs3bn2Jg,5450
+drekar_launch-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drekar_launch-0.1.3.dist-info/entry_points.txt,sha256=6tYJlxAt1he_nlcz1XIWGuG25TY3CHKXlLz3IdOMG6I,53
+drekar_launch-0.1.3.dist-info/top_level.txt,sha256=RgrbC56bqzVppX9z-Js4DoCjJWX2O9yw1dDjzoqILfY,14
+drekar_launch-0.1.3.dist-info/RECORD,,
```

