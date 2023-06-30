# Comparing `tmp/ai2_kit-0.3.8.tar.gz` & `tmp/ai2_kit-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.3.8.tar", max compression
+gzip compressed data, was "ai2_kit-0.3.9.tar", max compression
```

## Comparing `ai2_kit-0.3.8.tar` & `ai2_kit-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.8/LICENSE
--rw-r--r--   0        0        0     1627 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.8/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.8/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1854 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5465 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.8/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7939 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1852 2023-06-28 01:16:35.057371 ai2_kit-0.3.8/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9449 2023-06-28 02:30:53.156473 ai2_kit-0.3.8/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-06-28 06:44:38.463386 ai2_kit-0.3.8/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.8/ai2_kit/core/script.py
--rw-r--r--   0        0        0     4195 2023-06-28 08:04:13.892405 ai2_kit-0.3.8/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.8/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      381 2023-06-28 02:30:53.156473 ai2_kit-0.3.8/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     8210 2023-06-28 08:04:13.892405 ai2_kit-0.3.8/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4424 2023-06-28 02:30:53.156473 ai2_kit-0.3.8/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     7169 2023-06-28 02:30:53.156473 ai2_kit-0.3.8/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    16845 2023-06-28 08:04:13.892405 ai2_kit-0.3.8/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3039 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-06-28 03:52:57.155461 ai2_kit-0.3.8/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     9346 2023-06-28 02:30:53.156473 ai2_kit-0.3.8/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1588 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0     1039 2023-06-28 08:16:01.942257 ai2_kit-0.3.8/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.8/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     9230 2023-06-28 03:52:57.155461 ai2_kit-0.3.8/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9117 2023-06-28 01:16:35.067371 ai2_kit-0.3.8/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      843 2023-06-28 08:18:00.732237 ai2_kit-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 ai2_kit-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1962 2023-06-28 08:45:40.481907 ai2_kit-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5465 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7939 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-06-28 09:20:35.201482 ai2_kit-0.3.9/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9449 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-06-28 06:44:38.463386 ai2_kit-0.3.9/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.9/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     4195 2023-06-28 08:04:13.892405 ai2_kit-0.3.9/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      381 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     8210 2023-06-28 08:04:13.892405 ai2_kit-0.3.9/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4424 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     7169 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    16845 2023-06-28 08:04:13.892405 ai2_kit-0.3.9/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3039 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-06-28 03:52:57.155461 ai2_kit-0.3.9/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     9346 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1588 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0     1039 2023-06-28 08:16:01.942257 ai2_kit-0.3.9/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     9230 2023-06-28 03:52:57.155461 ai2_kit-0.3.9/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9117 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      843 2023-06-28 09:21:11.211476 ai2_kit-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 ai2_kit-0.3.9/PKG-INFO
```

### Comparing `ai2_kit-0.3.8/LICENSE` & `ai2_kit-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/README.md` & `ai2_kit-0.3.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -39,9 +39,14 @@
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
 * [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
 * [ASE Toolkit](doc/manual/ase.md)
-* [FAQ](doc/manual/faq.md)
+* [Tips](doc/manual/tips.md)
 
+
+## Acknowledgement
+This project is inspired by and built upon the following projects:
+* [dpgen](https://github.com/deepmodeling/dpgen/tree/master/dpgen): A concurrent learning platform for the generation of reliable deep learning based potential energy models.
+* [ase](https://wiki.fysik.dtu.dk/ase/): Atomic Simulation Environment.
```

### Comparing `ai2_kit-0.3.8/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.3.9/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/artifact.py` & `ai2_kit-0.3.9/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/checkpoint.py` & `ai2_kit-0.3.9/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/connector.py` & `ai2_kit-0.3.9/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/executor.py` & `ai2_kit-0.3.9/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/job.py` & `ai2_kit-0.3.9/ai2_kit/core/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,26 +46,30 @@
     def is_success(self) -> bool:
         ...
 
     @abstractmethod
     def resubmit(self) -> 'JobFuture':
         ...
 
-async def gather_jobs(jobs: List[JobFuture], timeout = float('inf'), max_tries: int = 1) -> List[JobState]:
+async def gather_jobs(jobs: List[JobFuture], timeout = float('inf'), max_tries: int = 1, raise_error=True) -> List[JobState]:
     async def wait_job(job: JobFuture) -> JobState:
         state = JobState.UNKNOWN
         tries = 0
         while True:
             try:
                 state = await job.result_async(timeout)
                 if state is JobState.COMPLETED:
-                    break
+                    return state
             except TimeoutError:
                 state = JobState.TIMEOUT
             tries += 1
 
             if tries >= max_tries:
                 break
             job = job.resubmit()
-        return state
+
+        if raise_error:
+            raise RuntimeError(f'Job {job} failed with state {state}')
+        else:
+            return state
 
     return await asyncio.gather(*[wait_job(job) for job in jobs])
```

### Comparing `ai2_kit-0.3.8/ai2_kit/core/queue_system.py` & `ai2_kit-0.3.9/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/resource_manager.py` & `ai2_kit-0.3.9/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/script.py` & `ai2_kit-0.3.9/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/core/util.py` & `ai2_kit-0.3.9/ai2_kit/core/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/cll.py` & `ai2_kit-0.3.9/ai2_kit/domain/cll.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/cp2k.py` & `ai2_kit-0.3.9/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/data_helper.py` & `ai2_kit-0.3.9/ai2_kit/domain/data_helper.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/deepmd.py` & `ai2_kit-0.3.9/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/lammps.py` & `ai2_kit-0.3.9/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/selector.py` & `ai2_kit-0.3.9/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/domain/vasp.py` & `ai2_kit-0.3.9/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/main.py` & `ai2_kit-0.3.9/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/tool/ase.py` & `ai2_kit-0.3.9/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.3.9/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.3.9/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.8/pyproject.toml` & `ai2_kit-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.3.8/PKG-INFO` & `ai2_kit-0.3.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -67,10 +67,14 @@
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
 * [CLL MLP Training Workflow](doc/manual/cll-workflow.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
 * [ASE Toolkit](doc/manual/ase.md)
-* [FAQ](doc/manual/faq.md)
+* [Tips](doc/manual/tips.md)
 
 
+## Acknowledgement
+This project is inspired by and built upon the following projects:
+* [dpgen](https://github.com/deepmodeling/dpgen/tree/master/dpgen): A concurrent learning platform for the generation of reliable deep learning based potential energy models.
+* [ase](https://wiki.fysik.dtu.dk/ase/): Atomic Simulation Environment.
```

