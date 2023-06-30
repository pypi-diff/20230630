# Comparing `tmp/btimer-1.0.7.tar.gz` & `tmp/btimer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btimer-1.0.7.tar", last modified: Fri Jun 30 03:33:40 2023, max compression
+gzip compressed data, was "btimer-1.0.8.tar", last modified: Fri Jun 30 06:12:17 2023, max compression
```

## Comparing `btimer-1.0.7.tar` & `btimer-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 03:33:40.904377 btimer-1.0.7/
--rw-r--r--   0 dylan      (502) staff       (20)     1075 2023-06-30 02:58:44.000000 btimer-1.0.7/LICENSE.txt
--rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 03:33:40.904242 btimer-1.0.7/PKG-INFO
--rw-r--r--   0 dylan      (502) staff       (20)      730 2023-06-30 02:58:44.000000 btimer-1.0.7/README.md
-drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 03:33:40.904062 btimer-1.0.7/btimer.egg-info/
--rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (502) staff       (20)      227 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (502) staff       (20)        1 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/entry_points.txt
--rw-r--r--   0 dylan      (502) staff       (20)       13 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/requires.txt
--rw-r--r--   0 dylan      (502) staff       (20)        6 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/top_level.txt
--rw-r--r--   0 dylan      (502) staff       (20)      641 2023-06-30 03:31:11.000000 btimer-1.0.7/pyproject.toml
--rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 03:33:40.904417 btimer-1.0.7/setup.cfg
--rw-r--r--   0 dylan      (502) staff       (20)     1274 2023-06-30 03:25:13.000000 btimer-1.0.7/timer.py
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 06:12:17.427322 btimer-1.0.8/
+-rw-r--r--   0 dylan      (502) staff       (20)     1075 2023-06-30 02:58:44.000000 btimer-1.0.8/LICENSE.txt
+-rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 06:12:17.427173 btimer-1.0.8/PKG-INFO
+-rw-r--r--   0 dylan      (502) staff       (20)      730 2023-06-30 02:58:44.000000 btimer-1.0.8/README.md
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 06:12:17.426961 btimer-1.0.8/btimer.egg-info/
+-rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (502) staff       (20)      227 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (502) staff       (20)        1 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/entry_points.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       13 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/requires.txt
+-rw-r--r--   0 dylan      (502) staff       (20)        6 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (502) staff       (20)      688 2023-06-30 06:11:40.000000 btimer-1.0.8/pyproject.toml
+-rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 06:12:17.427363 btimer-1.0.8/setup.cfg
+-rw-r--r--   0 dylan      (502) staff       (20)     1274 2023-06-30 03:25:13.000000 btimer-1.0.8/timer.py
```

### Comparing `btimer-1.0.7/LICENSE.txt` & `btimer-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btimer-1.0.7/PKG-INFO` & `btimer-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.7
+Version: 1.0.8
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.7/README.md` & `btimer-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `btimer-1.0.7/btimer.egg-info/PKG-INFO` & `btimer-1.0.8/btimer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.7
+Version: 1.0.8
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.7/pyproject.toml` & `btimer-1.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btimer"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Dylan Ngo", email="it.tinhngo@gmail.com" },
 ]
 description = "Help people get away from the computer"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -18,10 +18,13 @@
 
 [project.scripts]
 btimer = "timer:main"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
+[tool.setuptools]
+include-package-data = true
+
 [project.urls]
 "Homepage" = "https://github.com/dylanngo95/timer"
 "Bug Tracker" = "https://github.com/dylanngo95/timer/issues"
```

### Comparing `btimer-1.0.7/timer.py` & `btimer-1.0.8/timer.py`

 * *Files identical despite different names*

