# Comparing `tmp/mpc_obscodes-2023.6.4.tar.gz` & `tmp/mpc_obscodes-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.6.4.tar", last modified: Sun Jun  4 02:51:16 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.6.8.tar", last modified: Thu Jun  8 02:42:13 2023, max compression
```

## Comparing `mpc_obscodes-2023.6.4.tar` & `mpc_obscodes-2023.6.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.248063 mpc_obscodes-2023.6.4/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245714 2023-06-04 02:51:05.000000 mpc_obscodes-2023.6.4/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 02:51:05.000000 mpc_obscodes-2023.6.4/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.248063 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-04 02:51:05.000000 mpc_obscodes-2023.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:42:13.434773 mpc_obscodes-2023.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-08 02:42:13.434773 mpc_obscodes-2023.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:42:13.430773 mpc_obscodes-2023.6.8/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246039 2023-06-08 02:42:02.000000 mpc_obscodes-2023.6.8/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 02:42:02.000000 mpc_obscodes-2023.6.8/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:42:13.434773 mpc_obscodes-2023.6.8/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 02:41:59.000000 mpc_obscodes-2023.6.8/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:42:13.430773 mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-08 02:42:13.000000 mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 02:42:13.000000 mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:42:13.000000 mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 02:42:13.000000 mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 02:42:13.000000 mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 02:42:02.000000 mpc_obscodes-2023.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:42:13.434773 mpc_obscodes-2023.6.8/setup.cfg
```

### Comparing `mpc_obscodes-2023.6.4/PKG-INFO` & `mpc_obscodes-2023.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2023.6.4
+Version: 2023.6.8
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.6.4/README.md` & `mpc_obscodes-2023.6.8/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes/compare.py` & `mpc_obscodes-2023.6.8/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.6.8/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.6.8/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987689782519491%*

 * *Differences: {"'M05'": "OrderedDict([('Longitude', 1.33161), ('cos', 0.729979), ('sin', 0.681267), ('Name', "*

 * *          "'Observatoire de la Nine, Canens')])",*

 * * "'X11'": "OrderedDict([('Longitude', 289.59604), ('cos', 0.909953), ('sin', -0.414324), ('Name', "*

 * *          "'VLT Survey Telescope, Paranal')])",*

 * * "'X60'": "OrderedDict([('Longitude', 306.42556), ('cos', 0.895232), ('sin', -0.444317), ('Name', "*

 * *          "'Guaraciaba Observatory')])"}*

```diff
@@ -11821,14 +11821,20 @@
     },
     "M04": {
         "Longitude": 1.4256,
         "Name": "Pujalt Observatory, Barcelona",
         "cos": 0.74764,
         "sin": 0.66207
     },
+    "M05": {
+        "Longitude": 1.33161,
+        "Name": "Observatoire de la Nine, Canens",
+        "cos": 0.729979,
+        "sin": 0.681267
+    },
     "M09": {
         "Longitude": 5.60094,
         "Name": "Observatory Gromme - Oudsbergen",
         "cos": 0.630164,
         "sin": 0.773882
     },
     "M10": {
@@ -13759,14 +13765,20 @@
     },
     "X10": {
         "Longitude": 291.8204,
         "Name": "OVTLN, San Pedro de Atacama",
         "cos": 0.921644,
         "sin": -0.387717
     },
+    "X11": {
+        "Longitude": 289.59604,
+        "Name": "VLT Survey Telescope, Paranal",
+        "cos": 0.909953,
+        "sin": -0.414324
+    },
     "X12": {
         "Longitude": 295.712,
         "Name": "Observatorio Los Cabezones",
         "cos": 0.80343,
         "sin": -0.593455
     },
     "X13": {
@@ -13819,14 +13831,20 @@
     },
     "X57": {
         "Longitude": 305.40626,
         "Name": "Polo Astronomico CMF,Foz do Iguacu",
         "cos": 0.903659,
         "sin": -0.426885
     },
+    "X60": {
+        "Longitude": 306.42556,
+        "Name": "Guaraciaba Observatory",
+        "cos": 0.895232,
+        "sin": -0.444317
+    },
     "X70": {
         "Longitude": 308.43322,
         "Name": "Observatorio OATU, Tupi Paulista",
         "cos": 0.931623,
         "sin": -0.362375
     },
     "X74": {
```

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.6.8/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.6.8/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.6.8/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.6.8/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-obscodes
-Version: 2023.6.4
+Version: 2023.6.8
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.6.4/pyproject.toml` & `mpc_obscodes-2023.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.06.04"
+version = "2023.06.08"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

