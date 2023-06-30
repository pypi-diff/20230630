# Comparing `tmp/poe_shell-0.1.2.tar.gz` & `tmp/poe_shell-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_shell-0.1.2.tar", max compression
+gzip compressed data, was "poe_shell-0.1.3.tar", max compression
```

## Comparing `poe_shell-0.1.2.tar` & `poe_shell-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.2/README.md
--rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.2/poe_shell/__init__.py
--rw-r--r--   0        0        0     1441 2023-06-30 08:04:11.719404 poe_shell-0.1.2/poe_shell/__main__.py
--rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.2/poe_shell/handlers/__init__.py
--rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.2/poe_shell/handlers/chat_handler.py
--rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.2/poe_shell/handlers/handler.py
--rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.2/poe_shell/handlers/one_off_handler.py
--rw-r--r--   0        0        0     1632 2023-06-30 03:28:52.616388 poe_shell-0.1.2/poe_shell/handlers/shell_handler.py
--rw-r--r--   0        0        0      840 2023-06-30 03:02:37.315763 poe_shell-0.1.2/poe_shell/poe_client.py
--rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.2/poe_shell/roles.py
--rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.2/poe_shell/utils.py
--rw-r--r--   0        0        0      424 2023-06-30 08:06:00.190411 poe_shell-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      760 2023-06-30 04:11:45.326714 poe_shell-0.1.3/README.md
+-rw-r--r--   0        0        0       35 2023-06-30 07:35:34.125904 poe_shell-0.1.3/poe_shell/__init__.py
+-rw-r--r--   0        0        0     1441 2023-06-30 08:08:24.427152 poe_shell-0.1.3/poe_shell/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:02:37.315128 poe_shell-0.1.3/poe_shell/handlers/__init__.py
+-rw-r--r--   0        0        0      942 2023-06-30 03:28:19.430015 poe_shell-0.1.3/poe_shell/handlers/chat_handler.py
+-rw-r--r--   0        0        0      291 2023-06-30 03:22:17.474038 poe_shell-0.1.3/poe_shell/handlers/handler.py
+-rw-r--r--   0        0        0      375 2023-06-30 03:22:44.232937 poe_shell-0.1.3/poe_shell/handlers/one_off_handler.py
+-rw-r--r--   0        0        0     1632 2023-06-30 03:28:52.616388 poe_shell-0.1.3/poe_shell/handlers/shell_handler.py
+-rw-r--r--   0        0        0      840 2023-06-30 03:02:37.315763 poe_shell-0.1.3/poe_shell/poe_client.py
+-rw-r--r--   0        0        0     1245 2023-06-30 03:02:37.315873 poe_shell-0.1.3/poe_shell/roles.py
+-rw-r--r--   0        0        0      646 2023-06-30 03:02:37.315982 poe_shell-0.1.3/poe_shell/utils.py
+-rw-r--r--   0        0        0      424 2023-06-30 08:11:12.754955 poe_shell-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 poe_shell-0.1.3/PKG-INFO
```

### Comparing `poe_shell-0.1.2/README.md` & `poe_shell-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/poe_shell/__main__.py` & `poe_shell-0.1.3/poe_shell/__main__.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/poe_shell/handlers/chat_handler.py` & `poe_shell-0.1.3/poe_shell/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/poe_shell/handlers/shell_handler.py` & `poe_shell-0.1.3/poe_shell/handlers/shell_handler.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/poe_shell/poe_client.py` & `poe_shell-0.1.3/poe_shell/poe_client.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/poe_shell/roles.py` & `poe_shell-0.1.3/poe_shell/roles.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/poe_shell/utils.py` & `poe_shell-0.1.3/poe_shell/utils.py`

 * *Files identical despite different names*

### Comparing `poe_shell-0.1.2/PKG-INFO` & `poe_shell-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-shell
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Samson Hui
 Author-email: hui.kawang@yahoo.com.hk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poe-api (>=0.4.6,<0.5.0)
```

