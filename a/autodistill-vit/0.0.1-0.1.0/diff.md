# Comparing `tmp/autodistill-vit-0.0.1.tar.gz` & `tmp/autodistill-vit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-vit-0.0.1.tar", last modified: Wed Jun  7 12:13:03 2023, max compression
+gzip compressed data, was "autodistill-vit-0.1.0.tar", last modified: Fri Jun 30 08:38:04 2023, max compression
```

## Comparing `autodistill-vit-0.0.1.tar` & `autodistill-vit-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:13:03.180762 autodistill-vit-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      883 2023-06-07 12:13:03.180633 autodistill-vit-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      541 2023-06-07 12:13:01.000000 autodistill-vit-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:13:03.179707 autodistill-vit-0.0.1/autodistill_vit/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 12:13:01.000000 autodistill-vit-0.0.1/autodistill_vit/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 12:13:03.180431 autodistill-vit-0.0.1/autodistill_vit.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      883 2023-06-07 12:13:03.000000 autodistill-vit-0.0.1/autodistill_vit.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      240 2023-06-07 12:13:03.000000 autodistill-vit-0.0.1/autodistill_vit.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 12:13:03.000000 autodistill-vit-0.0.1/autodistill_vit.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 12:13:03.000000 autodistill-vit-0.0.1/autodistill_vit.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       16 2023-06-07 12:13:03.000000 autodistill-vit-0.0.1/autodistill_vit.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 12:13:03.180801 autodistill-vit-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      975 2023-06-07 12:13:01.000000 autodistill-vit-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 08:38:04.859768 autodistill-vit-0.1.0/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-08 06:49:21.000000 autodistill-vit-0.1.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2027 2023-06-30 08:38:04.859629 autodistill-vit-0.1.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1560 2023-06-08 06:48:28.000000 autodistill-vit-0.1.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 08:38:04.858690 autodistill-vit-0.1.0/autodistill_vit/
+-rw-r--r--   0 james      (501) staff       (20)       59 2023-06-30 08:37:58.000000 autodistill-vit-0.1.0/autodistill_vit/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4147 2023-06-30 08:37:00.000000 autodistill-vit-0.1.0/autodistill_vit/vit.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 08:38:04.859434 autodistill-vit-0.1.0/autodistill_vit.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2027 2023-06-30 08:38:04.000000 autodistill-vit-0.1.0/autodistill_vit.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      271 2023-06-30 08:38:04.000000 autodistill-vit-0.1.0/autodistill_vit.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-30 08:38:04.000000 autodistill-vit-0.1.0/autodistill_vit.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      124 2023-06-30 08:38:04.000000 autodistill-vit-0.1.0/autodistill_vit.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       16 2023-06-30 08:38:04.000000 autodistill-vit-0.1.0/autodistill_vit.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-30 08:38:04.859820 autodistill-vit-0.1.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1205 2023-06-08 06:43:24.000000 autodistill-vit-0.1.0/setup.py
```

### Comparing `autodistill-vit-0.0.1/setup.py` & `autodistill-vit-0.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+import re
 
 import setuptools
 from setuptools import find_packages
-import re
 
-with open("./autodistill_vit/__init__.py", 'r') as f:
+with open("./autodistill_vit/__init__.py", "r") as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
-    
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autodistill-vit",
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="ViT module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/autodistill/autodistill-vit",
+    install_requires=[
+        "supervision==0.9.0",
+        "numpy",
+        "autodistill",
+        "torch",
+        "transformers" "datasets",
+        "Pillow",
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

