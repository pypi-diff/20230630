# Comparing `tmp/nonebot_plugin_userinfo-0.0.1.tar.gz` & `tmp/nonebot_plugin_userinfo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_userinfo-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_userinfo-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_userinfo-0.0.1.tar` & `nonebot_plugin_userinfo-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/LICENSE
--rw-r--r--   0        0        0     2680 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/README.md
--rw-r--r--   0        0        0      699 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/__init__.py
--rw-r--r--   0        0        0       75 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/__init__.py
--rw-r--r--   0        0        0     1008 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/console.py
--rw-r--r--   0        0        0     1850 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/kaiheila.py
--rw-r--r--   0        0        0     1723 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3940 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1968 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/qqguild.py
--rw-r--r--   0        0        0     3472 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/telegram.py
--rw-r--r--   0        0        0       40 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/exception.py
--rw-r--r--   0        0        0     2447 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/getter.py
--rw-r--r--   0        0        0     1921 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/image_source.py
--rw-r--r--   0        0        0      324 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/user_info.py
--rw-r--r--   0        0        0      565 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/utils.py
--rw-r--r--   0        0        0     1620 2023-06-27 05:04:41.247684 nonebot_plugin_userinfo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 nonebot_plugin_userinfo-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2680 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/README.md
+-rw-r--r--   0        0        0      699 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/__init__.py
+-rw-r--r--   0        0        0     1008 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/console.py
+-rw-r--r--   0        0        0     1850 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/kaiheila.py
+-rw-r--r--   0        0        0     1723 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3940 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1968 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/qqguild.py
+-rw-r--r--   0        0        0     3472 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/telegram.py
+-rw-r--r--   0        0        0       40 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/exception.py
+-rw-r--r--   0        0        0     2447 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/getter.py
+-rw-r--r--   0        0        0     2066 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/image_source.py
+-rw-r--r--   0        0        0      324 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/user_info.py
+-rw-r--r--   0        0        0      565 2023-06-30 03:35:48.777446 nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/utils.py
+-rw-r--r--   0        0        0     1620 2023-06-30 03:35:48.781446 nonebot_plugin_userinfo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 nonebot_plugin_userinfo-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_userinfo-0.0.1/LICENSE` & `nonebot_plugin_userinfo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/README.md` & `nonebot_plugin_userinfo-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/__init__.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/console.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/kaiheila.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/onebot_v11.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/onebot_v12.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/qqguild.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/adapters/telegram.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/getter.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/getter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/image_source.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/image_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import hashlib
+from pathlib import Path
 
+import anyio
 import emoji
 from pydantic import BaseModel, validator
 from strenum import StrEnum
 
 from .utils import download_url
 
 
@@ -69,8 +71,10 @@
     file_path: str
     api_server: str = "https://api.telegram.org/"
 
     def get_url(self) -> str:
         return f"{self.api_server}file/bot{self.token}/{self.file_path}"
 
     async def get_image(self) -> bytes:
+        if Path(self.file_path).exists():
+            return await anyio.Path(self.file_path).read_bytes()
         return await download_url(self.get_url())
```

### Comparing `nonebot_plugin_userinfo-0.0.1/nonebot_plugin_userinfo/utils.py` & `nonebot_plugin_userinfo-0.0.2/nonebot_plugin_userinfo/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_userinfo-0.0.1/pyproject.toml` & `nonebot_plugin_userinfo-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_userinfo"
-version = "0.0.1"
+version = "0.0.2"
 description = "Nonebot2 用户信息获取插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-userinfo"
 repository = "https://github.com/noneplugin/nonebot-plugin-userinfo"
```

### Comparing `nonebot_plugin_userinfo-0.0.1/PKG-INFO` & `nonebot_plugin_userinfo-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-userinfo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Nonebot2 用户信息获取插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-userinfo
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-userinfo Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-userinfo Version: 0.0.2 Summary:
 Nonebot2 ç¨æ·ä¿¡æ¯è·åæä»¶ Home-page: https://github.com/noneplugin/
 nonebot-plugin-userinfo License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: cachetools
```

