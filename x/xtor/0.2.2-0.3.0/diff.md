# Comparing `tmp/xtor-0.2.2.tar.gz` & `tmp/xtor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtor-0.2.2.tar", max compression
+gzip compressed data, was "xtor-0.3.0.tar", max compression
```

## Comparing `xtor-0.2.2.tar` & `xtor-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-06-28 18:39:30.877596 xtor-0.2.2/README.md
--rw-r--r--   0        0        0      623 2023-06-30 12:28:01.120564 xtor-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       67 2023-06-30 12:27:39.544282 xtor-0.2.2/xtor/__init__.py
--rw-r--r--   0        0        0     5090 2023-06-30 12:25:53.430569 xtor-0.2.2/xtor/tor.py
--rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.2.2/xtor/utils.py
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 xtor-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-30 12:29:01.033240 xtor-0.3.0/README.md
+-rw-r--r--   0        0        0      685 2023-06-30 12:50:22.533886 xtor-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-06-30 12:50:16.105940 xtor-0.3.0/xtor/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-30 12:47:55.419073 xtor-0.3.0/xtor/cli.py
+-rw-r--r--   0        0        0     5090 2023-06-30 12:25:53.430569 xtor-0.3.0/xtor/tor.py
+-rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.3.0/xtor/utils.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 xtor-0.3.0/PKG-INFO
```

### Comparing `xtor-0.2.2/README.md` & `xtor-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 xtor
 ===============================
 
-Torx is a simple tool for managing Tor instances.
+xtor is a simple tool for managing Tor instances.
 
 ## Installation
 
 - Linux
   - `sudo apt-get install tor`
   - `sudo apt-get install obfs4proxy`
```

### Comparing `xtor-0.2.2/xtor/tor.py` & `xtor-0.3.0/xtor/tor.py`

 * *Files identical despite different names*

### Comparing `xtor-0.2.2/xtor/utils.py` & `xtor-0.3.0/xtor/utils.py`

 * *Files identical despite different names*

### Comparing `xtor-0.2.2/PKG-INFO` & `xtor-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtor
-Version: 0.2.2
+Version: 0.3.0
 Summary: Manage Tor instances
 Home-page: https://github.com/khalidelborai/xtor
 License: GNU Version 3
 Keywords: tor,torrc,torrc manager,tor manager,tor instance,proxy
 Author: khalidelborai
 Author-email: elboraikhalid@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -13,22 +13,23 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx[socks] (>=0.24.1,<0.25.0)
 Requires-Dist: stem (>=1.8.2,<2.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: where (>=1.0.2,<2.0.0)
 Project-URL: Repository, https://github.com/khalidelborai/xtor
 Description-Content-Type: text/markdown
 
 xtor
 ===============================
 
-Torx is a simple tool for managing Tor instances.
+xtor is a simple tool for managing Tor instances.
 
 ## Installation
 
 - Linux
   - `sudo apt-get install tor`
   - `sudo apt-get install obfs4proxy`
```

