# Comparing `tmp/PyBrainAge-0.0.11.tar.gz` & `tmp/PyBrainAge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBrainAge-0.0.11.tar", last modified: Fri Jun 30 15:22:52 2023, max compression
+gzip compressed data, was "PyBrainAge-0.0.2.tar", last modified: Fri Jun 30 14:55:58 2023, max compression
```

## Comparing `PyBrainAge-0.0.11.tar` & `PyBrainAge-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 15:22:52.587997 PyBrainAge-0.0.11/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 PyBrainAge-0.0.11/LICENSE
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      662 2023-06-30 15:22:52.587997 PyBrainAge-0.0.11/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 PyBrainAge-0.0.11/README.md
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      726 2023-06-30 15:21:29.000000 PyBrainAge-0.0.11/pyproject.toml
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 15:22:52.587997 PyBrainAge-0.0.11/setup.cfg
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 15:22:52.587997 PyBrainAge-0.0.11/src/
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 15:22:52.587997 PyBrainAge-0.0.11/src/PyBrainAge/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 12:41:05.000000 PyBrainAge-0.0.11/src/PyBrainAge/__init__.py
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)     2945 2023-06-30 14:04:03.000000 PyBrainAge-0.0.11/src/PyBrainAge/trees.py
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 15:22:52.587997 PyBrainAge-0.0.11/src/PyBrainAge.egg-info/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      662 2023-06-30 15:22:52.000000 PyBrainAge-0.0.11/src/PyBrainAge.egg-info/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      235 2023-06-30 15:22:52.000000 PyBrainAge-0.0.11/src/PyBrainAge.egg-info/SOURCES.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 15:22:52.000000 PyBrainAge-0.0.11/src/PyBrainAge.egg-info/dependency_links.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       17 2023-06-30 15:22:52.000000 PyBrainAge-0.0.11/src/PyBrainAge.egg-info/top_level.txt
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

### Comparing `PyBrainAge-0.0.11/LICENSE` & `PyBrainAge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBrainAge-0.0.11/PKG-INFO` & `PyBrainAge-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBrainAge
-Version: 0.0.11
+Version: 0.0.2
 Summary: PyBrainAge a python package for brain-age prediction on T1w MRI scans using various machine learnig methods.
 Author-email: Ayodeji Ijishakin <ayodeji.ijishakin.21@ucl.ac.uk>, Francesca Biondo <f.biondo@ucl.ac.uk>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `PyBrainAge-0.0.11/pyproject.toml` & `PyBrainAge-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "pandas==1.5.3", "scikit-learn==1.2.2","numpy==1.24.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyBrainAge"
-version = "0.0.11"
+version = "0.0.2"
 authors = [
   { name="Ayodeji Ijishakin", email="ayodeji.ijishakin.21@ucl.ac.uk" },
   { name="Francesca Biondo", email="f.biondo@ucl.ac.uk"}
 ]
 description = "PyBrainAge a python package for brain-age prediction on T1w MRI scans using various machine learnig methods."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `PyBrainAge-0.0.11/src/PyBrainAge.egg-info/PKG-INFO` & `PyBrainAge-0.0.2/PyBrainAge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBrainAge
-Version: 0.0.11
+Version: 0.0.2
 Summary: PyBrainAge a python package for brain-age prediction on T1w MRI scans using various machine learnig methods.
 Author-email: Ayodeji Ijishakin <ayodeji.ijishakin.21@ucl.ac.uk>, Francesca Biondo <f.biondo@ucl.ac.uk>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

