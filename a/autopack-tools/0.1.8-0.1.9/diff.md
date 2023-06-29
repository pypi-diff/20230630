# Comparing `tmp/autopack_tools-0.1.8.tar.gz` & `tmp/autopack_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.1.8.tar", max compression
+gzip compressed data, was "autopack_tools-0.1.9.tar", max compression
```

## Comparing `autopack_tools-0.1.8.tar` & `autopack_tools-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.8/LICENSE
--rw-r--r--   0        0        0     2925 2023-06-28 18:38:55.268381 autopack_tools-0.1.8/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.8/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.8/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.8/autopack/__main__.py
--rw-r--r--   0        0        0     2331 2023-06-28 18:28:49.076953 autopack_tools-0.1.8/autopack/api.py
--rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.8/autopack/cli.py
--rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.8/autopack/errors.py
--rw-r--r--   0        0        0     4793 2023-06-28 18:27:22.894184 autopack_tools-0.1.8/autopack/get_pack.py
--rw-r--r--   0        0        0     2774 2023-06-28 17:54:45.256305 autopack_tools-0.1.8/autopack/installation.py
--rw-r--r--   0        0        0     1414 2023-06-28 18:27:07.106680 autopack_tools-0.1.8/autopack/pack.py
--rw-r--r--   0        0        0      955 2023-06-28 18:58:09.661286 autopack_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 autopack_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2925 2023-06-28 18:38:55.268381 autopack_tools-0.1.9/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.1.9/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-25 23:21:01.956387 autopack_tools-0.1.9/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.1.9/autopack/__main__.py
+-rw-r--r--   0        0        0     2344 2023-06-28 22:13:39.865795 autopack_tools-0.1.9/autopack/api.py
+-rw-r--r--   0        0        0      864 2023-06-25 23:21:01.957129 autopack_tools-0.1.9/autopack/cli.py
+-rw-r--r--   0        0        0      258 2023-06-25 23:21:01.957337 autopack_tools-0.1.9/autopack/errors.py
+-rw-r--r--   0        0        0     4827 2023-06-28 23:23:28.263867 autopack_tools-0.1.9/autopack/get_pack.py
+-rw-r--r--   0        0        0     2804 2023-06-28 20:52:32.647683 autopack_tools-0.1.9/autopack/installation.py
+-rw-r--r--   0        0        0     2383 2023-06-28 23:21:27.392151 autopack_tools-0.1.9/autopack/pack.py
+-rw-r--r--   0        0        0      955 2023-06-28 22:16:21.117129 autopack_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 autopack_tools-0.1.9/PKG-INFO
```

### Comparing `autopack_tools-0.1.8/LICENSE` & `autopack_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.8/README.md` & `autopack_tools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.8/autopack/api.py` & `autopack_tools-0.1.9/autopack/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import requests
 from dataclasses_json import dataclass_json
 from marshmallow import ValidationError
 
 from autopack.errors import AutoPackFetchError
 
-API_URL = os.environ.get("API_URL", "https://autopack.ai/")
+API_URL = os.environ.get("AUTOPACK_API_URL", "https://autopack.ai/")
 
 
 @dataclass_json
 @dataclass
 class PackResponse:
     """Class to map Pack properties from the API. Internal use only."""
 
@@ -21,15 +21,15 @@
     author: str
     repo: str
     module_path: str
     description: str
     name: str
     dependencies: list[str]
     source: str
-    args: dict[str, Any]
+    run_args: dict[str, Any]
     init_args: dict[str, Any]
 
     def pack_path(self) -> str:
         return f"{self.author}_{self.repo}_{self.name}".replace("-", "_")
 
 
 def get_pack_details(pack_id: str) -> Union[PackResponse, None]:
```

### Comparing `autopack_tools-0.1.8/autopack/cli.py` & `autopack_tools-0.1.9/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.1.8/autopack/get_pack.py` & `autopack_tools-0.1.9/autopack/get_pack.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 import inspect
 import os
 import sys
 from types import ModuleType
 from typing import Type, Union
 
 from autopack.api import PackResponse, get_pack_details
-from autopack.errors import AutoPackError, AutoPackLoadError, AutoPackNotFoundError, AutoPackNotInstalledError
+from autopack.errors import (
+    AutoPackError,
+    AutoPackLoadError,
+    AutoPackNotFoundError,
+    AutoPackNotInstalledError,
+)
 from autopack.pack import Pack
 
 
 def try_get_pack(pack_id: str, quiet=False) -> Union[Pack, None]:
     """
     Get a pack based on its ID, in `author/repo_name/pack_name` format. Same as `get_pack` but does not raise an
     Exception. If there is a problem finding or loading a pack it will return None.
@@ -68,15 +73,17 @@
             return importlib.import_module(pack_data.pack_path() + "." + module_path)
         finally:
             sys.path.remove(autopack_dir)
 
 
 def find_or_create_autopack_dir(depth=0) -> str:
     """Search in current and parent directories looking for .autopack"""
-    autopack_dir = os.path.abspath(os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack"))
+    autopack_dir = os.path.abspath(
+        os.path.join(os.getcwd(), *[os.pardir] * depth, ".autopack")
+    )
 
     if not os.path.exists(autopack_dir) or not os.path.isdir(autopack_dir):
         if depth > 3:
             raise ModuleNotFoundError(".autopack directory could not be found")
         return find_or_create_autopack_dir(depth=depth + 1)
 
     return autopack_dir
@@ -90,22 +97,20 @@
                 f"Pack {pack_data.pack_id} could not be found. Either it is misconfigured or .autopack directory not "
                 f"found"
             )
             raise AutoPackNotFoundError(message)
 
         for _, obj in inspect.getmembers(module):
             if is_valid_pack(obj, pack_data.name):
-                return Pack(tool=obj, **pack_data.__dict__)
+                return Pack(**{"tool": obj, **pack_data.__dict__})
 
         message = f"Pack {pack_data.pack_id} found, but {pack_data.name} is not found in its module"
         raise AutoPackNotFoundError(message)
     except ModuleNotFoundError:
-        message = (
-            f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
-        )
+        message = f"Pack {pack_data.pack_id} is available but not installed. To install: autopack install {pack_data.pack_id}"
         if not quiet:
             print(message)
         raise AutoPackNotInstalledError(message)
     except (ImportError, AttributeError) as e:
         message = f"Error loading {pack_data.pack_id}: {e}"
         if not quiet:
             print(message)
@@ -113,15 +118,17 @@
 
 
 def is_valid_pack(klass: Type, name: str):
     if not inspect.isclass(klass):
         return False
 
     base_class_names = [k.__name__ for k in klass.__bases__]
-    roughly_adheres_to_interface = hasattr(klass, "run") or "BaseTool" in base_class_names
+    roughly_adheres_to_interface = (
+        hasattr(klass, "run") or "BaseTool" in base_class_names
+    )
     if not roughly_adheres_to_interface:
         return False
 
     # Pack name is the class name
     if name == klass.__name__:
         return True
```

### Comparing `autopack_tools-0.1.8/autopack/installation.py` & `autopack_tools-0.1.9/autopack/installation.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     for dependency in dependencies:
         if is_dependency_installed(dependency):
             continue
 
         if force:
             install_dependency(dependency)
         else:
-            print(f"This pack requires the dependency {dependency} to be installed. Continue?")
+            print(
+                f"This pack requires the dependency {dependency} to be installed. Continue?"
+            )
             agree = input("[Yn]")
             if agree.lower() == "y" or agree == "":
                 install_dependency(dependency)
             else:
                 print(f"Skipping install of {dependency}")
```

### Comparing `autopack_tools-0.1.8/pyproject.toml` & `autopack_tools-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.1.8"
+version = "0.1.9"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
@@ -14,28 +14,28 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
 urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
+langchain = "^0.0.218"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
 pytest = "^7.3.2"
 pytest-mock = "^3.11.1"
 types-requests = "^2.31.0.1"
 psycopg2 = "^2.9.6"
 docopt = "^0.6.2"
 autoflake = "^2.2.0"
 types-psycopg2 = "^2.9.21.10"
 types-docopt = "^0.6.11.3"
-langchain = "^0.0.215"
 pipreqs = "^0.4.13"
 gitpython = "^3.1.31"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autopack_tools-0.1.8/PKG-INFO` & `autopack_tools-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: langchain (>=0.0.218,<0.0.219)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/AutoPackAI/autopack
 Description-Content-Type: text/markdown
 
 # AutoPack Tools
```

