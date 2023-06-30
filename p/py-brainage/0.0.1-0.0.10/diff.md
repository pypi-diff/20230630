# Comparing `tmp/py_brainage-0.0.1.tar.gz` & `tmp/py_brainage-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_brainage-0.0.1.tar", last modified: Fri Jun 30 16:00:25 2023, max compression
+gzip compressed data, was "py_brainage-0.0.10.tar", last modified: Fri Jun 30 16:06:56 2023, max compression
```

## Comparing `py_brainage-0.0.1.tar` & `py_brainage-0.0.10.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:00:25.277655 py_brainage-0.0.1/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 py_brainage-0.0.1/LICENSE
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      590 2023-06-30 16:00:25.277655 py_brainage-0.0.1/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 py_brainage-0.0.1/README.md
-drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:00:25.277655 py_brainage-0.0.1/py_brainage.egg-info/
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      590 2023-06-30 16:00:25.000000 py_brainage-0.0.1/py_brainage.egg-info/PKG-INFO
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      215 2023-06-30 16:00:25.000000 py_brainage-0.0.1/py_brainage.egg-info/SOURCES.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:00:25.000000 py_brainage-0.0.1/py_brainage.egg-info/dependency_links.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       48 2023-06-30 16:00:25.000000 py_brainage-0.0.1/py_brainage.egg-info/requires.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:00:25.000000 py_brainage-0.0.1/py_brainage.egg-info/top_level.txt
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      648 2023-06-30 15:54:12.000000 py_brainage-0.0.1/pyproject.toml
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 16:00:25.277655 py_brainage-0.0.1/setup.cfg
--rw-r--r--   0 aijishak  (1000) aijishak  (1000)      285 2023-06-30 15:59:57.000000 py_brainage-0.0.1/setup.py
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:06:56.057597 py_brainage-0.0.10/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)     1074 2023-06-30 13:15:46.000000 py_brainage-0.0.10/LICENSE
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      591 2023-06-30 16:06:56.047597 py_brainage-0.0.10/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       92 2023-06-30 13:15:00.000000 py_brainage-0.0.10/README.md
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      649 2023-06-30 16:06:22.000000 py_brainage-0.0.10/pyproject.toml
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       38 2023-06-30 16:06:56.057597 py_brainage-0.0.10/setup.cfg
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:06:56.047597 py_brainage-0.0.10/src/
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:06:56.047597 py_brainage-0.0.10/src/py_brainage/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 12:41:05.000000 py_brainage-0.0.10/src/py_brainage/__init__.py
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)     2943 2023-06-30 15:37:15.000000 py_brainage-0.0.10/src/py_brainage/trees.py
+drwxr-xr-x   0 aijishak  (1000) aijishak  (1000)        0 2023-06-30 16:06:56.047597 py_brainage-0.0.10/src/py_brainage.egg-info/
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      591 2023-06-30 16:06:56.000000 py_brainage-0.0.10/src/py_brainage.egg-info/PKG-INFO
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)      241 2023-06-30 16:06:56.000000 py_brainage-0.0.10/src/py_brainage.egg-info/SOURCES.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)        1 2023-06-30 16:06:56.000000 py_brainage-0.0.10/src/py_brainage.egg-info/dependency_links.txt
+-rw-r--r--   0 aijishak  (1000) aijishak  (1000)       18 2023-06-30 16:06:56.000000 py_brainage-0.0.10/src/py_brainage.egg-info/top_level.txt
```

### Comparing `py_brainage-0.0.1/LICENSE` & `py_brainage-0.0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `py_brainage-0.0.1/PKG-INFO` & `py_brainage-0.0.10/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_brainage
-Version: 0.0.1
+Version: 0.0.10
 Summary: A python package for brain-age prediction on T1w MRI scans using various machine learnig methods.
 Author-email: Ayodeji Ijishakin <ayodeji.ijishakin.21@ucl.ac.uk>, Francesca Biondo <f.biondo@ucl.ac.uk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `py_brainage-0.0.1/py_brainage.egg-info/PKG-INFO` & `py_brainage-0.0.10/src/py_brainage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-brainage
-Version: 0.0.1
+Version: 0.0.10
 Summary: A python package for brain-age prediction on T1w MRI scans using various machine learnig methods.
 Author-email: Ayodeji Ijishakin <ayodeji.ijishakin.21@ucl.ac.uk>, Francesca Biondo <f.biondo@ucl.ac.uk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `py_brainage-0.0.1/pyproject.toml` & `py_brainage-0.0.10/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "pandas==1.5.3", "scikit-learn==1.2.2","numpy==1.24.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_brainage"
-version = "0.0.1"
+version = "0.0.10"
 authors = [
   { name="Ayodeji Ijishakin", email="ayodeji.ijishakin.21@ucl.ac.uk" },
   { name="Francesca Biondo", email="f.biondo@ucl.ac.uk"}
 ]
 description = "A python package for brain-age prediction on T1w MRI scans using various machine learnig methods."
 readme = "README.md"
 requires-python = ">=3.7"
```

