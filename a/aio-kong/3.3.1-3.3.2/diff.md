# Comparing `tmp/aio_kong-3.3.1.tar.gz` & `tmp/aio_kong-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_kong-3.3.1.tar", max compression
+gzip compressed data, was "aio_kong-3.3.2.tar", max compression
```

## Comparing `aio_kong-3.3.1.tar` & `aio_kong-3.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1461 2023-06-21 09:38:30.518849 aio_kong-3.3.1/LICENSE
--rw-r--r--   0        0        0       54 2023-06-21 09:38:30.518849 aio_kong-3.3.1/kong/__init__.py
--rw-r--r--   0        0        0     2314 2023-06-21 09:38:30.518849 aio_kong-3.3.1/kong/auths.py
--rw-r--r--   0        0        0      278 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/certificates.py
--rw-r--r--   0        0        0     1986 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/cli.py
--rw-r--r--   0        0        0     3783 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/client.py
--rw-r--r--   0        0        0     5342 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/components.py
--rw-r--r--   0        0        0     2720 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/consumers.py
--rw-r--r--   0        0        0     2685 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/plugins.py
--rw-r--r--   0        0        0        0 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/py.typed
--rw-r--r--   0        0        0     1482 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/routes.py
--rw-r--r--   0        0        0     2514 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/services.py
--rw-r--r--   0        0        0      665 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/snis.py
--rw-r--r--   0        0        0      931 2023-06-21 09:38:30.522849 aio_kong-3.3.1/kong/utils.py
--rw-r--r--   0        0        0     1778 2023-06-21 09:38:30.522849 aio_kong-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     2192 2023-06-21 09:38:30.522849 aio_kong-3.3.1/readme.md
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 aio_kong-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-06-30 12:04:41.907900 aio_kong-3.3.2/LICENSE
+-rw-r--r--   0        0        0       54 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/__init__.py
+-rw-r--r--   0        0        0     2314 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/auths.py
+-rw-r--r--   0        0        0      278 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/certificates.py
+-rw-r--r--   0        0        0     1932 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/cli.py
+-rw-r--r--   0        0        0     3782 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/client.py
+-rw-r--r--   0        0        0     5342 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/components.py
+-rw-r--r--   0        0        0     2720 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/consumers.py
+-rw-r--r--   0        0        0     2685 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/py.typed
+-rw-r--r--   0        0        0     1482 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/routes.py
+-rw-r--r--   0        0        0     2514 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/services.py
+-rw-r--r--   0        0        0      665 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/snis.py
+-rw-r--r--   0        0        0      931 2023-06-30 12:04:41.907900 aio_kong-3.3.2/kong/utils.py
+-rw-r--r--   0        0        0     1827 2023-06-30 12:04:41.907900 aio_kong-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2192 2023-06-30 12:04:41.907900 aio_kong-3.3.2/readme.md
+-rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 aio_kong-3.3.2/PKG-INFO
```

### Comparing `aio_kong-3.3.1/LICENSE` & `aio_kong-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/auths.py` & `aio_kong-3.3.2/kong/auths.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/cli.py` & `aio_kong-3.3.2/kong/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,11 +62,7 @@
             if keys:
                 key = keys[0]
             else:
                 key = await c.keyauths.create()
             click.echo(json.dumps(key.data, indent=4))
         except KongError as exc:
             raise click.ClickException(str(exc))
-
-
-def main() -> None:  # pragma    nocover
-    kong()
```

### Comparing `aio_kong-3.3.1/kong/client.py` & `aio_kong-3.3.2/kong/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 import os
 import sys
-from aiohttp import ClientResponse, ClientSession
 from typing import Any, Callable, Dict, Optional
 
+from aiohttp import ClientResponse, ClientSession
+
 from . import __version__
 from .certificates import Certificates
 from .components import CrudComponent, KongError, KongResponseError
 from .consumers import Consumers
 from .plugins import Plugins
 from .routes import Routes
 from .services import Services
 from .snis import Snis
 
 __all__ = ["Kong", "KongError", "KongResponseError"]
 
 DEFAULT_USER_AGENT = (
-    f"Python/${'.'.join(map(str, sys.version_info[:2]))} aio-kong/${__version__}"
+    f"Python/{'.'.join(map(str, sys.version_info[:2]))} aio-kong/{__version__}"
 )
 
 
 class Kong:
     """Kong client"""
 
     url: str = os.getenv(
```

### Comparing `aio_kong-3.3.1/kong/components.py` & `aio_kong-3.3.2/kong/components.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/consumers.py` & `aio_kong-3.3.2/kong/consumers.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/plugins.py` & `aio_kong-3.3.2/kong/plugins.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/routes.py` & `aio_kong-3.3.2/kong/routes.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/services.py` & `aio_kong-3.3.2/kong/services.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/snis.py` & `aio_kong-3.3.2/kong/snis.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/kong/utils.py` & `aio_kong-3.3.2/kong/utils.py`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/pyproject.toml` & `aio_kong-3.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-kong"
-version = "3.3.1"
+version = "3.3.2"
 description = "Asynchronous Kong Client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD-3-Clause"
 readme = "readme.md"
 packages = [
     {include = "kong"}
 ]
@@ -48,14 +48,17 @@
 types-PyYAML = "^6.0.11"
 ruff = "^0.0.274"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.poetry.scripts]
+kongfig = "kong.cli:kong"
+
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
```

### Comparing `aio_kong-3.3.1/readme.md` & `aio_kong-3.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `aio_kong-3.3.1/PKG-INFO` & `aio_kong-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-kong
-Version: 3.3.1
+Version: 3.3.2
 Summary: Asynchronous Kong Client
 License: BSD-3-Clause
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

