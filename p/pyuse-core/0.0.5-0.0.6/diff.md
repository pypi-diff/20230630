# Comparing `tmp/pyuse-core-0.0.5.tar.gz` & `tmp/pyuse-core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuse-core-0.0.5.tar", last modified: Wed Sep 21 02:52:56 2022, max compression
+gzip compressed data, was "pyuse-core-0.0.6.tar", last modified: Fri Jun 30 03:32:39 2023, max compression
```

## Comparing `pyuse-core-0.0.5.tar` & `pyuse-core-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2022-09-21 02:52:56.644435 pyuse-core-0.0.5/
--rw-r--r--   0 yangqing   (501) staff       (20)     1111 2022-09-21 02:52:56.644114 pyuse-core-0.0.5/PKG-INFO
--rw-r--r--   0 yangqing   (501) staff       (20)      577 2022-05-03 02:38:00.000000 pyuse-core-0.0.5/README.md
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2022-09-21 02:52:56.640360 pyuse-core-0.0.5/pyuse/
--rw-r--r--   0 yangqing   (501) staff       (20)      330 2022-04-25 02:51:06.000000 pyuse-core-0.0.5/pyuse/__init__.py
--rw-r--r--   0 yangqing   (501) staff       (20)     3976 2022-04-27 07:23:42.000000 pyuse-core-0.0.5/pyuse/dingtalk.py
--rw-r--r--   0 yangqing   (501) staff       (20)     4703 2022-08-19 08:34:43.000000 pyuse-core-0.0.5/pyuse/generator.py
--rw-r--r--   0 yangqing   (501) staff       (20)     2409 2022-04-25 08:15:01.000000 pyuse-core-0.0.5/pyuse/path.py
--rw-r--r--   0 yangqing   (501) staff       (20)     4955 2022-04-26 08:54:06.000000 pyuse-core-0.0.5/pyuse/time.py
-drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2022-09-21 02:52:56.643499 pyuse-core-0.0.5/pyuse_core.egg-info/
--rw-r--r--   0 yangqing   (501) staff       (20)     1111 2022-09-21 02:52:56.000000 pyuse-core-0.0.5/pyuse_core.egg-info/PKG-INFO
--rw-r--r--   0 yangqing   (501) staff       (20)      237 2022-09-21 02:52:56.000000 pyuse-core-0.0.5/pyuse_core.egg-info/SOURCES.txt
--rw-r--r--   0 yangqing   (501) staff       (20)        1 2022-09-21 02:52:56.000000 pyuse-core-0.0.5/pyuse_core.egg-info/dependency_links.txt
--rw-r--r--   0 yangqing   (501) staff       (20)        6 2022-09-21 02:52:56.000000 pyuse-core-0.0.5/pyuse_core.egg-info/top_level.txt
--rw-r--r--   0 yangqing   (501) staff       (20)       38 2022-09-21 02:52:56.644516 pyuse-core-0.0.5/setup.cfg
--rw-r--r--   0 yangqing   (501) staff       (20)      906 2022-09-21 02:52:04.000000 pyuse-core-0.0.5/setup.py
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-30 03:32:39.009293 pyuse-core-0.0.6/
+-rw-r--r--   0 yangqing   (501) staff       (20)     1111 2023-06-30 03:32:39.008847 pyuse-core-0.0.6/PKG-INFO
+-rw-r--r--   0 yangqing   (501) staff       (20)      577 2022-05-03 02:38:00.000000 pyuse-core-0.0.6/README.md
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-30 03:32:39.004318 pyuse-core-0.0.6/pyuse/
+-rw-r--r--   0 yangqing   (501) staff       (20)      330 2022-04-25 02:51:06.000000 pyuse-core-0.0.6/pyuse/__init__.py
+-rw-r--r--   0 yangqing   (501) staff       (20)     3976 2022-04-27 07:23:42.000000 pyuse-core-0.0.6/pyuse/dingtalk.py
+-rw-r--r--   0 yangqing   (501) staff       (20)     4703 2022-08-19 08:34:43.000000 pyuse-core-0.0.6/pyuse/generator.py
+-rw-r--r--   0 yangqing   (501) staff       (20)     2409 2022-04-25 08:15:01.000000 pyuse-core-0.0.6/pyuse/path.py
+-rw-r--r--   0 yangqing   (501) staff       (20)     4955 2022-04-26 08:54:06.000000 pyuse-core-0.0.6/pyuse/time.py
+drwxr-xr-x   0 yangqing   (501) staff       (20)        0 2023-06-30 03:32:39.008266 pyuse-core-0.0.6/pyuse_core.egg-info/
+-rw-r--r--   0 yangqing   (501) staff       (20)     1111 2023-06-30 03:32:38.000000 pyuse-core-0.0.6/pyuse_core.egg-info/PKG-INFO
+-rw-r--r--   0 yangqing   (501) staff       (20)      237 2023-06-30 03:32:38.000000 pyuse-core-0.0.6/pyuse_core.egg-info/SOURCES.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)        1 2023-06-30 03:32:38.000000 pyuse-core-0.0.6/pyuse_core.egg-info/dependency_links.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)        6 2023-06-30 03:32:38.000000 pyuse-core-0.0.6/pyuse_core.egg-info/top_level.txt
+-rw-r--r--   0 yangqing   (501) staff       (20)       38 2023-06-30 03:32:39.009568 pyuse-core-0.0.6/setup.cfg
+-rw-r--r--   0 yangqing   (501) staff       (20)      906 2023-06-30 03:31:32.000000 pyuse-core-0.0.6/setup.py
```

### Comparing `pyuse-core-0.0.5/PKG-INFO` & `pyuse-core-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuse-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pkg of wheels. Hope it helps you to write less code.
 Home-page: https://github.com/yongchin0821/pyuse
 Author: Yongchin
 Author-email: yongchin39@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/yongchin0821/pyuse/issues
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyuse-core Version: 0.0.5 Summary: A pkg of wheels.
+Metadata-Version: 2.1 Name: pyuse-core Version: 0.0.6 Summary: A pkg of wheels.
 Hope it helps you to write less code. Home-page: https://github.com/
 yongchin0821/pyuse Author: Yongchin Author-email: yongchin39@qq.com License:
 UNKNOWN Project-URL: Bug Tracker, https://github.com/yongchin0821/pyuse/issues
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `pyuse-core-0.0.5/README.md` & `pyuse-core-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyuse-core-0.0.5/pyuse/dingtalk.py` & `pyuse-core-0.0.6/pyuse/dingtalk.py`

 * *Files identical despite different names*

### Comparing `pyuse-core-0.0.5/pyuse/generator.py` & `pyuse-core-0.0.6/pyuse/generator.py`

 * *Files identical despite different names*

### Comparing `pyuse-core-0.0.5/pyuse/path.py` & `pyuse-core-0.0.6/pyuse/path.py`

 * *Files identical despite different names*

### Comparing `pyuse-core-0.0.5/pyuse/time.py` & `pyuse-core-0.0.6/pyuse/time.py`

 * *Files identical despite different names*

### Comparing `pyuse-core-0.0.5/pyuse_core.egg-info/PKG-INFO` & `pyuse-core-0.0.6/pyuse_core.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuse-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pkg of wheels. Hope it helps you to write less code.
 Home-page: https://github.com/yongchin0821/pyuse
 Author: Yongchin
 Author-email: yongchin39@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/yongchin0821/pyuse/issues
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyuse-core Version: 0.0.5 Summary: A pkg of wheels.
+Metadata-Version: 2.1 Name: pyuse-core Version: 0.0.6 Summary: A pkg of wheels.
 Hope it helps you to write less code. Home-page: https://github.com/
 yongchin0821/pyuse Author: Yongchin Author-email: yongchin39@qq.com License:
 UNKNOWN Project-URL: Bug Tracker, https://github.com/yongchin0821/pyuse/issues
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `pyuse-core-0.0.5/setup.py` & `pyuse-core-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyuse-core",
-    version="0.0.5",
+    version="0.0.6",
     author="Yongchin",
     author_email="yongchin39@qq.com",
     description="A pkg of wheels. Hope it helps you to write less code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yongchin0821/pyuse",
     project_urls={
```

