# Comparing `tmp/poe_shell-0.1.4.tar.gz` & `tmp/poe_shell-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_shell-0.1.4.tar", max compression
+gzip compressed data, was "poe_shell-0.1.5.tar", max compression
```

## Comparing `poe_shell-0.1.4.tar` & `poe_shell-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.4/README.md
--rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.4/poe_shell/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-30 08:29:11.644029 poe_shell-0.1.4/poe_shell/__main__.py
--rw-r--r--   0        0        0       67 2023-06-30 08:28:39.799053 poe_shell-0.1.4/poe_shell/config.py
--rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.4/poe_shell/handlers/__init__.py
--rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.4/poe_shell/handlers/chat_handler.py
--rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.4/poe_shell/handlers/handler.py
--rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.4/poe_shell/handlers/one_off_handler.py
--rw-r--r--   0        0        0     1632 2023-06-30 03:28:52.616388 poe_shell-0.1.4/poe_shell/handlers/shell_handler.py
--rw-r--r--   0        0        0      889 2023-06-30 08:30:30.576523 poe_shell-0.1.4/poe_shell/poe_client.py
--rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.4/poe_shell/roles.py
--rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.4/poe_shell/utils.py
--rw-r--r--   0        0        0      424 2023-06-30 08:30:59.050256 poe_shell-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.5/README.md
+-rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.5/poe_shell/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-30 08:29:11.644029 poe_shell-0.1.5/poe_shell/__main__.py
+-rw-r--r--   0        0        0       67 2023-06-30 08:28:39.799053 poe_shell-0.1.5/poe_shell/config.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.5/poe_shell/handlers/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-30 03:04:19.592632 poe_shell-0.1.5/poe_shell/handlers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2015 2023-06-30 03:59:17.025656 poe_shell-0.1.5/poe_shell/handlers/__pycache__/chat_handler.cpython-311.pyc
+-rw-r--r--   0        0        0     1063 2023-06-30 03:26:22.131426 poe_shell-0.1.5/poe_shell/handlers/__pycache__/handler.cpython-311.pyc
+-rw-r--r--   0        0        0     1187 2023-06-30 03:27:40.596752 poe_shell-0.1.5/poe_shell/handlers/__pycache__/one_off_handler.cpython-311.pyc
+-rw-r--r--   0        0        0     2761 2023-06-30 03:29:26.961034 poe_shell-0.1.5/poe_shell/handlers/__pycache__/shell_handler.cpython-311.pyc
+-rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.5/poe_shell/handlers/chat_handler.py
+-rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.5/poe_shell/handlers/handler.py
+-rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.5/poe_shell/handlers/one_off_handler.py
+-rw-r--r--   0        0        0     1634 2023-06-30 08:37:45.068549 poe_shell-0.1.5/poe_shell/handlers/shell_handler.py
+-rw-r--r--   0        0        0      889 2023-06-30 08:30:30.576523 poe_shell-0.1.5/poe_shell/poe_client.py
+-rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.5/poe_shell/roles.py
+-rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.5/poe_shell/utils.py
+-rw-r--r--   0        0        0      424 2023-06-30 08:38:46.974239 poe_shell-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.5/PKG-INFO
```

### Comparing `poe_shell-0.1.4/README.md` & `poe_shell-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.4/poe_shell/__main__.py` & `poe_shell-0.1.5/poe_shell/__main__.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.4/poe_shell/handlers/chat_handler.py` & `poe_shell-0.1.5/poe_shell/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.4/poe_shell/handlers/shell_handler.py` & `poe_shell-0.1.5/poe_shell/handlers/shell_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils import run_command
+from ..utils import run_command
 from .handler import Handler
 
 
 class ShellHandler(Handler):
     chat_bot = "shellbotsss"
 
     def handle(self):
```

### Comparing `poe_shell-0.1.4/poe_shell/poe_client.py` & `poe_shell-0.1.5/poe_shell/poe_client.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.4/poe_shell/roles.py` & `poe_shell-0.1.5/poe_shell/roles.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.4/poe_shell/utils.py` & `poe_shell-0.1.5/poe_shell/utils.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.4/PKG-INFO` & `poe_shell-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-shell
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Samson Hui
 Author-email: hui.kawang@yahoo.com.hk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poe-api (>=0.4.6,<0.5.0)
```

