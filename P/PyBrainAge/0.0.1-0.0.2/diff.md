# Comparing `tmp/pybrainage-0.0.1.tar.gz` & `tmp/PyBrainAge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "PyBrainAge-0.0.2.tar", last modified: Fri Jun 30 14:55:58 2023, max compression
```

## Comparing `pybrainage-0.0.1.tar` & `PyBrainAge-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 pybrainage-0.0.1/setup.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pybrainage-0.0.1/src/PyBrainAge/__init__.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pybrainage-0.0.1/src/PyBrainAge/trees.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pybrainage-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pybrainage-0.0.1/LICENSE
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybrainage-0.0.1/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pybrainage-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pybrainage-0.0.1/PKG-INFO
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 14:55:58.528242 PyBrainAge-0.0.2/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 PyBrainAge-0.0.2/LICENSE
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      661 2023-06-30 14:55:58.528242 PyBrainAge-0.0.2/PKG-INFO
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 14:55:58.528242 PyBrainAge-0.0.2/PyBrainAge.egg-info/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      661 2023-06-30 14:55:58.000000 PyBrainAge-0.0.2/PyBrainAge.egg-info/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      210 2023-06-30 14:55:58.000000 PyBrainAge-0.0.2/PyBrainAge.egg-info/SOURCES.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 14:55:58.000000 PyBrainAge-0.0.2/PyBrainAge.egg-info/dependency_links.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       48 2023-06-30 14:55:58.000000 PyBrainAge-0.0.2/PyBrainAge.egg-info/requires.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 14:55:58.000000 PyBrainAge-0.0.2/PyBrainAge.egg-info/top_level.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 PyBrainAge-0.0.2/README.md
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      725 2023-06-30 14:55:31.000000 PyBrainAge-0.0.2/pyproject.toml
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 14:55:58.528242 PyBrainAge-0.0.2/setup.cfg
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      298 2023-06-30 14:55:35.000000 PyBrainAge-0.0.2/setup.py
```

### Comparing `pybrainage-0.0.1/LICENSE` & `PyBrainAge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybrainage-0.0.1/pyproject.toml` & `PyBrainAge-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0", "pandas==1.5.3", "scikit-learn==1.2.2","numpy==1.24.2"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyBrainAge"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ayodeji Ijishakin", email="ayodeji.ijishakin.21@ucl.ac.uk" },
   { name="Francesca Biondo", email="f.biondo@ucl.ac.uk"}
 ]
 description = "PyBrainAge a python package for brain-age prediction on T1w MRI scans using various machine learnig methods."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pybrainage-0.0.1/PKG-INFO` & `PyBrainAge-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyBrainAge
-Version: 0.0.1
+Version: 0.0.2
 Summary: PyBrainAge a python package for brain-age prediction on T1w MRI scans using various machine learnig methods.
-Project-URL: Homepage, https://github.com/pypa/sampleproject
 Author-email: Ayodeji Ijishakin <ayodeji.ijishakin.21@ucl.ac.uk>, Francesca Biondo <f.biondo@ucl.ac.uk>
-License-File: LICENSE
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 This Package Features a suite of brain age prediction models, which work on T1w MRI Scans.
```

