# Comparing `tmp/pywaiwera-1.3.1.tar.gz` & `tmp/pywaiwera-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaiwera-1.3.1.tar", last modified: Tue Jun 28 23:29:14 2022, max compression
+gzip compressed data, was "pywaiwera-1.4.0.tar", last modified: Fri Jun 30 02:56:26 2023, max compression
```

## Comparing `pywaiwera-1.3.1.tar` & `pywaiwera-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:29:14.382610 pywaiwera-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-06-28 23:29:14.382610 pywaiwera-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:29:14.382610 pywaiwera-1.3.1/pywaiwera/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/pywaiwera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/pywaiwera/common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    33623 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/pywaiwera/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:29:14.382610 pywaiwera-1.3.1/pywaiwera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-06-28 23:29:14.000000 pywaiwera-1.3.1/pywaiwera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-06-28 23:29:14.000000 pywaiwera-1.3.1/pywaiwera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 23:29:14.000000 pywaiwera-1.3.1/pywaiwera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 23:29:14.000000 pywaiwera-1.3.1/pywaiwera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-28 23:29:14.000000 pywaiwera-1.3.1/pywaiwera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-28 23:29:14.382610 pywaiwera-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 23:29:14.382610 pywaiwera-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/test/test_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     5159 2022-06-28 23:29:03.000000 pywaiwera-1.3.1/test/test_waiwera_dkr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:56:26.987083 pywaiwera-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-30 02:56:26.987083 pywaiwera-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:56:26.987083 pywaiwera-1.4.0/pywaiwera/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/pywaiwera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/pywaiwera/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33623 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/pywaiwera/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:56:26.987083 pywaiwera-1.4.0/pywaiwera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-30 02:56:26.000000 pywaiwera-1.4.0/pywaiwera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-30 02:56:26.000000 pywaiwera-1.4.0/pywaiwera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 02:56:26.000000 pywaiwera-1.4.0/pywaiwera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-30 02:56:26.000000 pywaiwera-1.4.0/pywaiwera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 02:56:26.000000 pywaiwera-1.4.0/pywaiwera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 02:56:26.987083 pywaiwera-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:56:26.987083 pywaiwera-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/test/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-30 02:56:17.000000 pywaiwera-1.4.0/test/test_waiwera_dkr.py
```

### Comparing `pywaiwera-1.3.1/PKG-INFO` & `pywaiwera-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pywaiwera
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python package for the Waiwera simulator
 Home-page: https://waiwera.github.io
 Author: Waiwera Project
 Author-email: waiwera.project@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 
@@ -59,9 +57,7 @@
 
 It is also possible to use the PyWaiwera package from within Python scripts. For example, the following script imports PyWaiwera, creates a Docker environment and uses it to run Waiwera on the model input file `input.json`:
 
     import pywaiwera
     print(pywaiwera.__version__)
     env = pywaiwera.docker.DockerEnv()
     env.run_waiwera('input.json')
-
-
```

### Comparing `pywaiwera-1.3.1/README.md` & `pywaiwera-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pywaiwera-1.3.1/pywaiwera/docker.py` & `pywaiwera-1.4.0/pywaiwera/docker.py`

 * *Files identical despite different names*

### Comparing `pywaiwera-1.3.1/pywaiwera.egg-info/PKG-INFO` & `pywaiwera-1.4.0/pywaiwera.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pywaiwera
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python package for the Waiwera simulator
 Home-page: https://waiwera.github.io
 Author: Waiwera Project
 Author-email: waiwera.project@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 
@@ -59,9 +57,7 @@
 
 It is also possible to use the PyWaiwera package from within Python scripts. For example, the following script imports PyWaiwera, creates a Docker environment and uses it to run Waiwera on the model input file `input.json`:
 
     import pywaiwera
     print(pywaiwera.__version__)
     env = pywaiwera.docker.DockerEnv()
     env.run_waiwera('input.json')
-
-
```

### Comparing `pywaiwera-1.3.1/setup.py` & `pywaiwera-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pywaiwera",
-    version="1.3.1",
+    version="1.4.0",
     author="Waiwera Project",
     author_email="waiwera.project@gmail.com",
     description="Python package for the Waiwera simulator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://waiwera.github.io",
     packages=setuptools.find_packages(),
```

### Comparing `pywaiwera-1.3.1/test/test_package.py` & `pywaiwera-1.4.0/test/test_package.py`

 * *Files identical despite different names*

### Comparing `pywaiwera-1.3.1/test/test_waiwera_dkr.py` & `pywaiwera-1.4.0/test/test_waiwera_dkr.py`

 * *Files identical despite different names*

