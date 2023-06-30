# Comparing `tmp/climy-0.1.0.tar.gz` & `tmp/climy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climy-0.1.0.tar", max compression
+gzip compressed data, was "climy-0.1.1.tar", max compression
```

## Comparing `climy-0.1.0.tar` & `climy-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-31 11:59:05.924021 climy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1236 2023-06-29 12:11:02.677187 climy-0.1.0/README.md
--rw-r--r--   0        0        0      136 2023-06-29 11:45:06.580415 climy-0.1.0/climy/__init__.py
--rw-r--r--   0        0        0     1107 2023-06-29 11:45:06.584415 climy-0.1.0/climy/application.py
--rw-r--r--   0        0        0     5202 2023-06-29 11:57:03.904048 climy-0.1.0/climy/command.py
--rw-r--r--   0        0        0       25 2023-06-16 10:11:53.677630 climy-0.1.0/climy/manager.py
--rw-r--r--   0        0        0      922 2023-06-29 11:45:06.596415 climy-0.1.0/climy/option.py
--rw-r--r--   0        0        0      394 2023-06-29 12:12:35.247273 climy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 climy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 11:59:05.924021 climy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1236 2023-06-29 12:11:02.677187 climy-0.1.1/README.md
+-rw-r--r--   0        0        0      136 2023-06-29 11:45:06.580415 climy-0.1.1/climy/__init__.py
+-rw-r--r--   0        0        0     1107 2023-06-29 11:45:06.584415 climy-0.1.1/climy/application.py
+-rw-r--r--   0        0        0     5217 2023-06-30 12:47:51.074491 climy-0.1.1/climy/command.py
+-rw-r--r--   0        0        0       25 2023-06-16 10:11:53.677630 climy-0.1.1/climy/manager.py
+-rw-r--r--   0        0        0      922 2023-06-29 11:45:06.596415 climy-0.1.1/climy/option.py
+-rw-r--r--   0        0        0      394 2023-06-30 12:49:10.576289 climy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 climy-0.1.1/PKG-INFO
```

### Comparing `climy-0.1.0/LICENSE` & `climy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climy-0.1.0/README.md` & `climy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `climy-0.1.0/climy/application.py` & `climy-0.1.1/climy/application.py`

 * *Files identical despite different names*

### Comparing `climy-0.1.0/climy/command.py` & `climy-0.1.1/climy/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def add_command(
             self,
             command: 'Command',
             *,
             name: str = ''
     ):
         command.parent = self
-        command.app = self.app
+        command.app = command.app or self.app
         self.commands[name or command.name] = command
 
     def add_option(
             self,
             name: str,
             description: str,
             *,
```

### Comparing `climy-0.1.0/climy/option.py` & `climy-0.1.1/climy/option.py`

 * *Files identical despite different names*

### Comparing `climy-0.1.0/PKG-INFO` & `climy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Do CLI applications easily.
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

