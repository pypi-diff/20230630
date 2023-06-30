# Comparing `tmp/robert-0.0.1.tar.gz` & `tmp/robert-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robert-0.0.1.tar", last modified: Wed Feb 15 11:52:39 2023, max compression
+gzip compressed data, was "robert-1.0.0.tar", last modified: Fri Jun 30 17:37:09 2023, max compression
```

## Comparing `robert-0.0.1.tar` & `robert-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 11:52:39.902098 robert-0.0.1/
--rw-rw-rw-   0        0        0     1099 2022-01-26 18:07:48.000000 robert-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     8377 2023-02-15 11:52:39.902098 robert-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7447 2022-01-26 18:07:48.000000 robert-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 11:52:39.892596 robert-0.0.1/robert/
--rw-rw-rw-   0        0        0        0 2022-09-14 16:11:15.000000 robert-0.0.1/robert/__init__.py
--rw-rw-rw-   0        0        0      583 2023-02-13 16:54:43.000000 robert-0.0.1/robert/__main__.py
--rw-rw-rw-   0        0        0     1376 2023-02-14 19:20:06.000000 robert-0.0.1/robert/argument_parser.py
--rw-rw-rw-   0        0        0     8955 2023-02-15 11:31:59.000000 robert-0.0.1/robert/curate.py
--rw-rw-rw-   0        0        0     2519 2023-02-15 11:40:38.000000 robert-0.0.1/robert/robert.py
--rw-rw-rw-   0        0        0     7995 2023-02-15 11:20:02.000000 robert-0.0.1/robert/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-15 11:52:39.902098 robert-0.0.1/robert.egg-info/
--rw-rw-rw-   0        0        0     8377 2023-02-15 11:52:39.000000 robert-0.0.1/robert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-02-15 11:52:39.000000 robert-0.0.1/robert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 11:52:39.000000 robert-0.0.1/robert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-02-15 11:52:39.000000 robert-0.0.1/robert.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-15 11:52:39.000000 robert-0.0.1/robert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-02-15 11:52:39.902098 robert-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1916 2023-02-15 11:50:51.000000 robert-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.083404 robert-1.0.0/
+-rw-rw-rw-   0        0        0     1099 2023-05-23 09:25:43.000000 robert-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      992 2023-06-30 17:37:09.085836 robert-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2023-06-18 10:39:36.000000 robert-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.038152 robert-1.0.0/robert/
+-rw-rw-rw-   0        0        0        0 2023-05-23 09:25:43.000000 robert-1.0.0/robert/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-05-23 09:25:43.000000 robert-1.0.0/robert/__main__.py
+-rw-rw-rw-   0        0        0     5020 2023-06-17 18:18:26.000000 robert-1.0.0/robert/aqme.py
+-rw-rw-rw-   0        0        0     2017 2023-06-20 18:14:41.000000 robert-1.0.0/robert/argument_parser.py
+-rw-rw-rw-   0        0        0    15344 2023-06-30 11:54:20.000000 robert-1.0.0/robert/curate.py
+-rw-rw-rw-   0        0        0     7529 2023-06-20 18:11:53.000000 robert-1.0.0/robert/generate.py
+-rw-rw-rw-   0        0        0    29733 2023-06-30 16:53:53.000000 robert-1.0.0/robert/generate_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.064396 robert-1.0.0/robert/model_params/
+-rw-rw-rw-   0        0        0      211 2023-05-23 09:25:43.000000 robert-1.0.0/robert/model_params/ADAB_params.yaml
+-rw-rw-rw-   0        0        0      775 2023-06-30 17:01:38.000000 robert-1.0.0/robert/model_params/GB_params.yaml
+-rw-rw-rw-   0        0        0       91 2023-06-19 12:21:08.000000 robert-1.0.0/robert/model_params/GP_params.yaml
+-rw-rw-rw-   0        0        0       88 2023-06-07 12:49:19.000000 robert-1.0.0/robert/model_params/MVL_params.yaml
+-rw-rw-rw-   0        0        0      808 2023-06-07 12:43:39.000000 robert-1.0.0/robert/model_params/NN_params.yaml
+-rw-rw-rw-   0        0        0      576 2023-06-30 17:01:41.000000 robert-1.0.0/robert/model_params/RF_params.yaml
+-rw-rw-rw-   0        0        0      732 2023-06-30 17:01:45.000000 robert-1.0.0/robert/model_params/VR_params.yaml
+-rw-rw-rw-   0        0        0     4374 2023-06-20 17:35:36.000000 robert-1.0.0/robert/predict.py
+-rw-rw-rw-   0        0        0    26483 2023-06-21 06:22:51.000000 robert-1.0.0/robert/predict_utils.py
+-rw-rw-rw-   0        0        0     5745 2023-05-23 09:25:43.000000 robert-1.0.0/robert/report.py
+-rw-rw-rw-   0        0        0     5875 2023-06-20 15:37:54.000000 robert-1.0.0/robert/robert.py
+-rw-rw-rw-   0        0        0    37329 2023-06-30 16:54:00.000000 robert-1.0.0/robert/utils.py
+-rw-rw-rw-   0        0        0    19418 2023-06-20 15:37:54.000000 robert-1.0.0/robert/verify.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.048620 robert-1.0.0/robert.egg-info/
+-rw-rw-rw-   0        0        0      992 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 17:37:08.000000 robert-1.0.0/robert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-06-30 17:37:09.085836 robert-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2035 2023-06-30 17:01:03.000000 robert-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:37:09.083404 robert-1.0.0/tests/
+-rw-rw-rw-   0        0        0     6529 2023-06-19 15:13:27.000000 robert-1.0.0/tests/test_1curate.py
+-rw-rw-rw-   0        0        0     6379 2023-06-20 18:16:46.000000 robert-1.0.0/tests/test_2generate.py
+-rw-rw-rw-   0        0        0     4289 2023-06-20 19:38:53.000000 robert-1.0.0/tests/test_3verify.py
+-rw-rw-rw-   0        0        0     5019 2023-06-20 19:47:48.000000 robert-1.0.0/tests/test_4predict.py
+-rw-rw-rw-   0        0        0     4142 2023-06-20 18:05:57.000000 robert-1.0.0/tests/test_5aqme_n_full.py
```

### Comparing `robert-0.0.1/LICENSE` & `robert-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robert-0.0.1/robert/__main__.py` & `robert-1.0.0/robert/__main__.py`

 * *Files identical despite different names*

### Comparing `robert-0.0.1/setup.py` & `robert-1.0.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 from setuptools import setup, find_packages
-import io
-
-# read the contents of your README file
-from os import path
-
-this_directory = path.abspath(path.dirname(__file__))
-with io.open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
-
+version="1.0.0"
 setup(
     name="robert",
     packages=find_packages(exclude=["tests"]),
-    version="0.0.1",
+    package_data={"robert": ["model_params/*"]},
+    version=version,
     license="MIT",
     description="Refiner and Optimizer of a Bunch of Existing Regression Tools",
-    long_description=long_description,
+    long_description="Documentation in Read The Docs: https://robert.readthedocs.io",
     long_description_content_type="text/markdown",
     author="Juan V. Alegre Requena, David Dalmau",
     author_email="jv.alegre@csic.es",
     keywords=[
         "workflows",
         "machine learning",
         "cheminformatics",
         "data curation",
         "prediction",
         "automated",
     ],
     url="https://github.com/jvalegre/robert",
-    download_url="https://github.com/jvalegre/robert/archive/refs/tags/0.0.1.tar.gz",
+    download_url=f"https://github.com/jvalegre/robert/archive/refs/tags/{version}.tar.gz",
     classifiers=[
-        "Development Status :: 3 - Alpha",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+        "Development Status :: 4 - Beta",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         "Intended Audience :: Developers",  # Define that your audience are developers
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",  # Specify which python versions you want to support
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     install_requires=[
         "PyYAML",
-        "pandas",
+        "pandas>=2.0",
         "progress",
-        "numpy",
-        "matplotlib",
+        "numpy>=1.23,<1.24",
+        "matplotlib>=3.7.1",
         "seaborn",
-        "cffi",
         "scipy",
-        "sklearn",
+        "scikit-learn>=1.2,<1.3",
         "hyperopt",
+        "numba",
         "shap",
+        "glib",
+        "weasyprint",
+        "scikit-learn-intelex",
+        # requires also "conda install -c conda-forge gtk3" in Windows
+        # requires also "conda install -c conda-forge shap"
     ],
     python_requires=">=3.0",
     include_package_data=True,
 )
```

