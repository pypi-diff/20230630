# Comparing `tmp/multi_start-0.0.2.tar.gz` & `tmp/multi_start-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_start-0.0.2.tar", max compression
+gzip compressed data, was "multi_start-1.0.0.tar", max compression
```

## Comparing `multi_start-0.0.2.tar` & `multi_start-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1494 2023-06-28 14:30:20.736815 multi_start-0.0.2/LICENSE
--rw-r--r--   0        0        0      596 2023-06-28 14:30:20.736815 multi_start-0.0.2/README.md
--rw-r--r--   0        0        0      757 2023-06-28 14:30:20.736815 multi_start-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-28 14:30:20.736815 multi_start-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     2443 2023-06-28 14:30:20.736815 multi_start-0.0.2/src/cli.py
--rw-r--r--   0        0        0     6135 2023-06-28 14:30:20.736815 multi_start-0.0.2/src/starter.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 multi_start-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1494 2023-06-30 12:15:51.976479 multi_start-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2896 2023-06-30 12:15:51.976479 multi_start-1.0.0/README.md
+-rw-r--r--   0        0        0      704 2023-06-30 12:15:51.976479 multi_start-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 12:15:51.976479 multi_start-1.0.0/src/__init__.py
+-rw-r--r--   0        0        0     2857 2023-06-30 12:15:51.976479 multi_start-1.0.0/src/cli.py
+-rw-r--r--   0        0        0      188 2023-06-30 12:15:51.976479 multi_start-1.0.0/src/log.py
+-rw-r--r--   0        0        0     6147 2023-06-30 12:15:51.976479 multi_start-1.0.0/src/starter.py
+-rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 multi_start-1.0.0/PKG-INFO
```

### Comparing `multi_start-0.0.2/LICENSE` & `multi_start-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_start-0.0.2/pyproject.toml` & `multi_start-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [tool.poetry]
 name = "multi-start"
-version = "0.0.2"
+version = "1.0.0"
 description = "Run multiple services inside a docker container"
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/multi-start"
 authors = ["IOXIO Ltd"]
 packages = [
     {include="src", from="."}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "^0.9.0"
 httpx = "^0.24.1"
-pydantic = "^1.10.9"
-
-[tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 flake8-pyproject = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multi_start-0.0.2/src/cli.py` & `multi_start-1.0.0/src/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import asyncio
 import shlex
 from typing import Optional
 
 import typer
 from typer import Typer
 
-from .starter import RunConfig, Runner, Service
+from .log import logger
+from .starter import Runner, Service
 
 cli = Typer()
 
 
-@cli.command()
+@cli.command(
+    help=(
+        "Run multiple services at once. "
+        "Set DEBUG environment variable to 1 for more verbose output when running."
+    )
+)
 def main(
     backend: bool = typer.Option(
         default=False,
         help="Enable backend service",
     ),
     backend_cmd: str = typer.Option(
         default="poetry run invoke serve",
         help="Command to start backend service",
     ),
     backend_dir: str = typer.Option(
-        default=".",
-        help="Working directory for a backend",
+        default="backend",
+        help="Working directory for the backend",
     ),
     backend_port: Optional[int] = typer.Option(
         default=None,
         help="Port number that backend is running at if port is used",
     ),
     backend_socket: str = typer.Option(
         default="/run/nginx/uvicorn.sock",
@@ -41,52 +47,61 @@
         help="Port number that frontend is running at",
     ),
     frontend_cmd: str = typer.Option(
         default="pnpm run start",
         help="Command to start frontend service",
     ),
     frontend_dir: str = typer.Option(
-        default="../frontend",
-        help="Working directory for a frontend",
+        default="frontend",
+        help="Working directory for the frontend",
     ),
     nginx: bool = typer.Option(
         default=False,
         help="Enable nginx",
     ),
     nginx_cmd: str = typer.Option(
         default='nginx -g "daemon off;"',
         help="Command to start Nginx",
     ),
-    service_wait_time: int = typer.Option(
-        default=3,
+    service_wait_time: float = typer.Option(
+        default=3.0,
         help="How long to wait for a service to be up an running (sec)",
     ),
 ):
     if not any([backend, frontend, nginx]):
-        raise RuntimeError("At least one service must be enabled")
+        logger.error("At least one service must be enabled")
+        raise typer.Exit(1)
 
-    cfg = RunConfig(
-        backend=Service(
+    backend_service = None
+    if backend:
+        backend_service = Service(
             cmd=shlex.split(backend_cmd),
             cwd=backend_dir,
             port=backend_port,
             socket=backend_socket,
+            timeout=service_wait_time,
         )
-        if backend
-        else None,
-        frontend=Service(
+
+    frontend_service = None
+    if frontend:
+        frontend_service = Service(
             cmd=shlex.split(frontend_cmd),
             cwd=frontend_dir,
             port=frontend_port,
+            timeout=service_wait_time,
         )
-        if frontend
-        else None,
-        nginx=Service(
+
+    nginx_service = None
+    if nginx:
+        nginx_service = Service(
             cmd=shlex.split(nginx_cmd),
             cwd=".",
+            timeout=service_wait_time,
         )
-        if nginx
-        else None,
-        svc_wait_time=service_wait_time,
-    )
 
-    asyncio.run(Runner(cfg).start())
+    asyncio.run(
+        Runner().start(
+            backend=backend_service,
+            frontend=frontend_service,
+            nginx=nginx_service,
+        )
+    )
```

### Comparing `multi_start-0.0.2/src/starter.py` & `multi_start-1.0.0/src/starter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,83 @@
 import asyncio
 import os
 import signal
 import sys
 from asyncio.subprocess import Process
+from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
 import httpx
-from pydantic import BaseModel
 
+from .log import logger
 
-class Service(BaseModel):
+
+@dataclass
+class Service:
     cmd: List[str]
     cwd: str
-    socket: Optional[str]
-    port: Optional[int]
-
-
-class RunConfig(BaseModel):
-    backend: Optional[Service]
-    frontend: Optional[Service]
-    nginx: Optional[Service]
-    svc_wait_time: int
+    timeout: float
+    socket: Optional[str] = None
+    port: Optional[int] = None
 
 
-async def run(cmd, cwd=None, pipe_output=False, extra_env=None) -> Process:
+async def run(
+    cmd: List[str],
+    cwd: Optional[str] = None,
+    pipe_output=False,
+    extra_env: Optional[dict] = None,
+) -> Process:
     """
     Run a process
     :param cmd: Command to run
     :param cwd: Working directory
     :param pipe_output: Whether to pipe the output or print it on screen instead
     :param extra_env: Extra environment variables
     :return: Process
     """
     env = os.environ.copy()
     if extra_env:
         env.update(extra_env)
 
     proc = await asyncio.create_subprocess_exec(
-        cmd[0],
-        *cmd[1:],
+        *cmd,
         stdout=asyncio.subprocess.PIPE if pipe_output else sys.stdout,
         stderr=asyncio.subprocess.PIPE if pipe_output else sys.stderr,
         cwd=cwd,
         env=env,
     )
 
     return proc
 
 
-def debug_msg(msg: str) -> None:
-    """
-    Print message only when DEBUG environment variable is set
-    :param msg: Message to print
-    """
-    if os.environ.get("DEBUG"):
-        print(msg)
-
-
-async def run_and_wait(cmd, cwd=None):
-    proc = await run(cmd, cwd)
+async def run_and_wait(
+    cmd: List[str], cwd: Optional[str] = None, extra_env: Optional[dict] = None
+):
+    proc = await run(cmd, cwd, extra_env=extra_env)
     code = await proc.wait()
     if code != 0:
         raise RuntimeError(f"{cmd} failed with code {code}")
 
 
-async def get_output(cmd, cwd=None) -> bytes:
+async def get_output(cmd: List[str], cwd: Optional[str] = None) -> bytes:
     """
     Run command and get its stdout if completed successfully
     :param cmd: Command to run
     :param cwd: Working directory
     :return: Bytes from stdout
     """
     proc = await run(cmd, cwd, pipe_output=True)
     out, err = await proc.communicate()
     if proc.returncode != 0:
         raise RuntimeError(f"{cmd} failed with code {proc.returncode}")
     return out
 
 
-async def stop_process(proc: Process, timeout=3.0) -> None:
+async def stop_process(proc: Process, timeout: float = 3.0) -> None:
     """
     Try to stop the process gracefully, otherwise killing it
     :param proc: Process to stop
     :param timeout: How long to wait for a graceful stop
     """
     if proc.returncode is not None:
         return
@@ -104,103 +98,107 @@
     if user := os.environ.get("HTTP_BASIC_AUTH_USER"):
         pwd = os.environ["HTTP_BASIC_AUTH_PASSWORD"]
         await run_and_wait(["htpasswd", "-b", "-c", "/run/nginx/.htpasswd", user, pwd])
         if not os.environ.get("HTTP_BASIC_AUTH_REALM"):
             os.environ["HTTP_BASIC_AUTH_REALM"] = "Private area"
 
     for f in ["/etc/nginx/conf.d/default.conf", "/etc/nginx/dataspace-headers.conf"]:
+        path = Path(f)
         final_config = await get_output(["parse-template", f])
-        Path(f).write_bytes(final_config)
-        print(f"{f} is generated")
+        path.write_bytes(final_config)
+        logger.info(f"{f} is generated")
 
         if os.environ.get("NGINX_DEBUG"):
-            print(f"=== {f} ===")
-            print(Path(f).read_text("utf8") + "\n")
+            logger.info(f"=== {f} ===")
+            logger.info(path.read_text("utf8") + "\n")
 
 
 async def start_service(svc: Service, extra_env: Optional[dict] = None) -> Process:
     """
     Start a service.
     :param svc: Service to run
     :param extra_env: Extra environment variables
     :return: Process
     """
-    debug_msg(f"Starting service: {svc.cmd}")
+    logger.debug(f"Starting service: {svc.cmd}")
     return await run(svc.cmd, cwd=svc.cwd, extra_env=extra_env)
 
 
-async def wait_for_service(svc: Service, timeout: int):
+async def wait_for_service(svc: Service, timeout: float):
     """
     Wait until a service and up and listening for either a port or socket.
     Port takes precedence over a socket if both defined.
     :param svc: Service to wait for
     :param timeout: How long to wait in seconds
     """
     if not svc.socket and not svc.port:
         raise RuntimeError("Either socket or port should be defined")
 
-    url = "http://localhost"
-    transport = httpx.AsyncHTTPTransport(uds=svc.socket)
-
     if svc.port:
+        url = f"http://localhost:{svc.port}"
         transport = httpx.AsyncHTTPTransport()
-        url += f":{svc.port}"
+    else:
+        url = "http://localhost"
+        transport = httpx.AsyncHTTPTransport(uds=svc.socket)
 
     async with httpx.AsyncClient(transport=transport) as client:
         wait_step = 0.3
         max_attempts = int(timeout / wait_step)
         for _ in range(max_attempts):
             try:
-                await client.get(url)
+                await client.get(url, timeout=timeout)
             except httpx.ConnectError:
                 await asyncio.sleep(wait_step)
             else:
-                debug_msg(f"Connection established: {url}")
+                logger.debug(f"Connection established: {url}")
                 break
         else:
-            print("Service is not responding", svc)
+            logger.error("Service is not responding", svc)
             raise TimeoutError("Service is not responding")
 
 
 class Runner:
-    def __init__(self, cfg: RunConfig):
-        self.cfg = cfg
+    def __init__(self):
         self._stop = asyncio.Event()
 
     def stop(self, *args):
         self._stop.set()
 
-    async def start(self):
+    async def start(
+        self,
+        backend: Optional[Service],
+        frontend: Optional[Service],
+        nginx: Optional[Service],
+    ):
         # Handle Ctrl+C gracefully by stopping all running services
         loop = asyncio.get_running_loop()
         loop.add_signal_handler(signal.SIGINT, self.stop)
         loop.add_signal_handler(signal.SIGTERM, self.stop)
-        cfg = self.cfg
 
         prerequisites = []
         procs = []
 
-        if cfg.backend:
-            procs.append(await start_service(cfg.backend))
-            prerequisites.append(wait_for_service(cfg.backend, cfg.svc_wait_time))
+        if backend:
+            procs.append(await start_service(backend))
+            prerequisites.append(wait_for_service(backend, backend.timeout))
 
-        if cfg.frontend:
+        if frontend:
             frontend_svc = await start_service(
-                cfg.frontend, extra_env={"PORT": str(cfg.frontend.port)}
+                frontend, extra_env={"PORT": str(frontend.port)}
             )
             procs.append(frontend_svc)
-            prerequisites.append(wait_for_service(cfg.frontend, cfg.svc_wait_time))
+            prerequisites.append(wait_for_service(frontend, frontend.timeout))
 
-        if cfg.nginx:
+        if nginx:
             prerequisites.append(setup_nginx())
 
         await asyncio.gather(*prerequisites)
 
-        if cfg.nginx:
-            procs.append(await start_service(cfg.nginx))
+        if nginx:
+            procs.append(await start_service(nginx))
 
         tasks = [p.wait() for p in procs]
         tasks.append(self._stop.wait())
         await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
 
-        print("Shutting down all processes")
+        logger.info("Shutting down all processes")
         await asyncio.gather(*[stop_process(proc) for proc in procs])
```

