# Comparing `tmp/Signal8-4.3.tar.gz` & `tmp/Signal8-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.3.tar", last modified: Fri Jun 30 19:04:15 2023, max compression
+gzip compressed data, was "Signal8-4.4.tar", last modified: Fri Jun 30 19:05:09 2023, max compression
```

## Comparing `Signal8-4.3.tar` & `Signal8-4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:04:15.792094 Signal8-4.3/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.3/LICENSE
--rw-rw-rw-   0        0        0     4769 2023-06-30 19:04:15.789096 Signal8-4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4271 2023-06-22 19:39:26.000000 Signal8-4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 19:04:15.704113 Signal8-4.3/Signal8/
--rw-rw-rw-   0        0        0    12400 2023-06-30 19:02:52.000000 Signal8-4.3/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.3/Signal8/__init__.py
--rw-rw-rw-   0        0        0      208 2023-06-30 18:57:45.000000 Signal8-4.3/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:04:15.784093 Signal8-4.3/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.3/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.3/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-29 18:47:43.000000 Signal8-4.3/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.3/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11954 2023-06-30 18:56:28.000000 Signal8-4.3/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.3/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:04:15.762091 Signal8-4.3/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4769 2023-06-30 19:04:15.000000 Signal8-4.3/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-30 19:04:15.000000 Signal8-4.3/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:04:15.000000 Signal8-4.3/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 19:04:15.000000 Signal8-4.3/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 19:04:15.793094 Signal8-4.3/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-30 19:03:01.000000 Signal8-4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:05:09.471614 Signal8-4.4/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.4/LICENSE
+-rw-rw-rw-   0        0        0     4769 2023-06-30 19:05:09.468612 Signal8-4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4271 2023-06-22 19:39:26.000000 Signal8-4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 19:05:09.397091 Signal8-4.4/Signal8/
+-rw-rw-rw-   0        0        0    12400 2023-06-30 19:02:52.000000 Signal8-4.4/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.4/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      208 2023-06-30 18:57:45.000000 Signal8-4.4/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:05:09.463612 Signal8-4.4/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.4/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.4/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2322 2023-06-29 18:47:43.000000 Signal8-4.4/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.4/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11954 2023-06-30 18:56:28.000000 Signal8-4.4/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.4/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:05:09.433091 Signal8-4.4/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4769 2023-06-30 19:05:09.000000 Signal8-4.4/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-30 19:05:09.000000 Signal8-4.4/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:05:09.000000 Signal8-4.4/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 19:05:09.000000 Signal8-4.4/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 19:05:09.472612 Signal8-4.4/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-30 19:04:47.000000 Signal8-4.4/setup.py
```

### Comparing `Signal8-4.3/LICENSE` & `Signal8-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/PKG-INFO` & `Signal8-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.3
+Version: 4.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.3/README.md` & `Signal8-4.4/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/Signal8/Signal8.py` & `Signal8-4.4/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/Signal8/utils/core.py` & `Signal8-4.4/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/Signal8/utils/problems.py` & `Signal8-4.4/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/Signal8/utils/simple_env.py` & `Signal8-4.4/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.4/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.3/Signal8.egg-info/PKG-INFO` & `Signal8-4.4/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.3
+Version: 4.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.3/setup.py` & `Signal8-4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.3",
+    version="4.4",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

