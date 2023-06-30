# Comparing `tmp/SydneyGPT-0.11.6.tar.gz` & `tmp/SydneyGPT-0.11.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SydneyGPT-0.11.6.tar", last modified: Sat Jun 24 09:54:53 2023, max compression
+gzip compressed data, was "SydneyGPT-0.11.8.tar", last modified: Fri Jun 30 07:27:09 2023, max compression
```

## Comparing `SydneyGPT-0.11.6.tar` & `SydneyGPT-0.11.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:54:53.935740 SydneyGPT-0.11.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-24 09:54:53.935740 SydneyGPT-0.11.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 09:54:53.935740 SydneyGPT-0.11.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:54:53.927740 SydneyGPT-0.11.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:54:53.931740 SydneyGPT-0.11.6/src/SydneyGPT/
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/src/SydneyGPT/SydneyGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/src/SydneyGPT/SydneyGPTUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/src/SydneyGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/src/SydneyGPT/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 09:54:20.000000 SydneyGPT-0.11.6/src/SydneyGPT/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:54:53.935740 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-24 09:54:53.000000 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-24 09:54:53.000000 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:54:53.000000 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-24 09:54:53.000000 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-24 09:54:53.000000 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 09:54:53.000000 SydneyGPT-0.11.6/src/SydneyGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:27:09.838809 SydneyGPT-0.11.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-30 07:27:09.838809 SydneyGPT-0.11.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 07:27:09.838809 SydneyGPT-0.11.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:27:09.834808 SydneyGPT-0.11.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:27:09.834808 SydneyGPT-0.11.8/src/SydneyGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/src/SydneyGPT/SydneyGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/src/SydneyGPT/SydneyGPTUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/src/SydneyGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/src/SydneyGPT/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 07:26:39.000000 SydneyGPT-0.11.8/src/SydneyGPT/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:27:09.838809 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-30 07:27:09.000000 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 07:27:09.000000 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:27:09.000000 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 07:27:09.000000 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 07:27:09.000000 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 07:27:09.000000 SydneyGPT-0.11.8/src/SydneyGPT.egg-info/top_level.txt
```

### Comparing `SydneyGPT-0.11.6/LICENSE` & `SydneyGPT-0.11.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.11.6/PKG-INFO` & `SydneyGPT-0.11.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SydneyGPT
-Version: 0.11.6
+Version: 0.11.8
 Summary: Reverse engineered Sydney Bing Chat API
 Home-page: https://github.com/rafaelcalleja/SydneyGPT
 Author: Rafael Calleja
 Author-email: rafaelcalleja@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/rafaelcalleja/SydneyGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `SydneyGPT-0.11.6/README.md` & `SydneyGPT-0.11.8/README.md`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.11.6/setup.py` & `SydneyGPT-0.11.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="SydneyGPT",
-    version="0.11.6",
+    version="0.11.8",
     license="GNU General Public License v2.0",
     author="Rafael Calleja",
     author_email="rafaelcalleja@gmail.com",
     description="Reverse engineered Sydney Bing Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/rafaelcalleja/SydneyGPT",
```

### Comparing `SydneyGPT-0.11.6/src/SydneyGPT/SydneyGPT.py` & `SydneyGPT-0.11.8/src/SydneyGPT/SydneyGPT.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.11.6/src/SydneyGPT/SydneyGPTUtils.py` & `SydneyGPT-0.11.8/src/SydneyGPT/SydneyGPTUtils.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.11.6/src/SydneyGPT/conversation_style.py` & `SydneyGPT-0.11.8/src/SydneyGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.11.6/src/SydneyGPT.egg-info/PKG-INFO` & `SydneyGPT-0.11.8/src/SydneyGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SydneyGPT
-Version: 0.11.6
+Version: 0.11.8
 Summary: Reverse engineered Sydney Bing Chat API
 Home-page: https://github.com/rafaelcalleja/SydneyGPT
 Author: Rafael Calleja
 Author-email: rafaelcalleja@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/rafaelcalleja/SydneyGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

