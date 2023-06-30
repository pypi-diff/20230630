# Comparing `tmp/autodistill-blip-0.0.1.tar.gz` & `tmp/autodistill-blip-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-blip-0.0.1.tar", last modified: Wed Jun  7 12:10:30 2023, max compression
+gzip compressed data, was "autodistill-blip-0.1.0.tar", last modified: Fri Jun 30 09:03:28 2023, max compression
```

## Comparing `autodistill-blip-0.0.1.tar` & `autodistill-blip-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:10:30.611950 autodistill-blip-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      887 2023-06-07 12:10:30.611785 autodistill-blip-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      544 2023-06-07 12:10:28.000000 autodistill-blip-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:10:30.610355 autodistill-blip-0.0.1/autodistill_blip/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 12:10:28.000000 autodistill-blip-0.0.1/autodistill_blip/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:10:30.611396 autodistill-blip-0.0.1/autodistill_blip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      887 2023-06-07 12:10:30.000000 autodistill-blip-0.0.1/autodistill_blip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      246 2023-06-07 12:10:30.000000 autodistill-blip-0.0.1/autodistill_blip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 12:10:30.000000 autodistill-blip-0.0.1/autodistill_blip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 12:10:30.000000 autodistill-blip-0.0.1/autodistill_blip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-07 12:10:30.000000 autodistill-blip-0.0.1/autodistill_blip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 12:10:30.611998 autodistill-blip-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      977 2023-06-07 12:10:28.000000 autodistill-blip-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:03:28.883322 autodistill-blip-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)     1501 2023-06-12 11:34:19.000000 autodistill-blip-0.1.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:03:28.883199 autodistill-blip-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1794 2023-06-30 09:02:51.000000 autodistill-blip-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:03:28.882235 autodistill-blip-0.1.0/autodistill_blip/
+-rw-r--r--   0 james      (501) staff       (20)       62 2023-06-12 11:31:07.000000 autodistill-blip-0.1.0/autodistill_blip/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2808 2023-06-30 09:02:45.000000 autodistill-blip-0.1.0/autodistill_blip/blip.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:03:28.883013 autodistill-blip-0.1.0/autodistill_blip.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      279 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      108 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       17 2023-06-30 09:03:28.000000 autodistill-blip-0.1.0/autodistill_blip.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-30 09:03:28.883372 autodistill-blip-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1134 2023-06-30 09:03:25.000000 autodistill-blip-0.1.0/setup.py
```

### Comparing `autodistill-blip-0.0.1/setup.py` & `autodistill-blip-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./autodistill_blip/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
@@ -12,23 +11,29 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="autodistill-blip",
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="BLIP module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="",
+    install_requires=[
+        "transformers==4.25",
+        "torch",
+        "numpy",
+        "autodistill",
+        "supervision"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
-
```

