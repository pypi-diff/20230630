# Comparing `tmp/autodistill-blip-0.1.0.tar.gz` & `tmp/autodistill-blip-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-blip-0.1.0.tar", last modified: Fri Jun 30 09:03:28 2023, max compression
+gzip compressed data, was "autodistill-blip-0.1.1.tar", last modified: Fri Jun 30 09:05:19 2023, max compression
```

## Comparing `autodistill-blip-0.1.0.tar` & `autodistill-blip-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:03:28.883322 autodistill-blip-0.1.0/
--rw-r--r--   0 james      (501) staff       (20)     1501 2023-06-12 11:34:19.000000 autodistill-blip-0.1.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:03:28.883199 autodistill-blip-0.1.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1794 2023-06-30 09:02:51.000000 autodistill-blip-0.1.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:03:28.882235 autodistill-blip-0.1.0/autodistill_blip/
--rw-r--r--   0 james      (501) staff       (20)       62 2023-06-12 11:31:07.000000 autodistill-blip-0.1.0/autodistill_blip/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2808 2023-06-30 09:02:45.000000 autodistill-blip-0.1.0/autodistill_blip/blip.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:03:28.883013 autodistill-blip-0.1.0/autodistill_blip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      279 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      108 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-30 09:03:28.883372 autodistill-blip-0.1.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1134 2023-06-30 09:03:25.000000 autodistill-blip-0.1.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:05:19.613621 autodistill-blip-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)     1501 2023-06-12 11:34:19.000000 autodistill-blip-0.1.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:05:19.613497 autodistill-blip-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1794 2023-06-30 09:02:51.000000 autodistill-blip-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:05:19.612538 autodistill-blip-0.1.1/autodistill_blip/
+-rw-r--r--   0 james      (501) staff       (20)       62 2023-06-30 09:05:14.000000 autodistill-blip-0.1.1/autodistill_blip/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2808 2023-06-30 09:02:45.000000 autodistill-blip-0.1.1/autodistill_blip/blip.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:05:19.613310 autodistill-blip-0.1.1/autodistill_blip.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      279 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      108 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       17 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-30 09:05:19.613667 autodistill-blip-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1134 2023-06-30 09:05:06.000000 autodistill-blip-0.1.1/setup.py
```

### Comparing `autodistill-blip-0.1.0/LICENSE` & `autodistill-blip-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-blip-0.1.0/PKG-INFO` & `autodistill-blip-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autodistill-blip
-Version: 0.1.0
+Version: 0.1.1
 Summary: BLIP module for use with Autodistill
 Home-page: 
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `autodistill-blip-0.1.0/README.md` & `autodistill-blip-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autodistill-blip-0.1.0/autodistill_blip/blip.py` & `autodistill-blip-0.1.1/autodistill_blip/blip.py`

 * *Files identical despite different names*

### Comparing `autodistill-blip-0.1.0/autodistill_blip.egg-info/PKG-INFO` & `autodistill-blip-0.1.1/autodistill_blip.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autodistill-blip
-Version: 0.1.0
+Version: 0.1.1
 Summary: BLIP module for use with Autodistill
 Home-page: 
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `autodistill-blip-0.1.0/setup.py` & `autodistill-blip-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

