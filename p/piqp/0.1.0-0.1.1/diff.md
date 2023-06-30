# Comparing `tmp/piqp-0.1.0.tar.gz` & `tmp/piqp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqp-0.1.0.tar", last modified: Wed Jun 28 15:01:25 2023, max compression
+gzip compressed data, was "piqp-0.1.1.tar", last modified: Fri Jun 30 15:05:22 2023, max compression
```

## Comparing `piqp-0.1.0.tar` & `piqp-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:01:25.004776 piqp-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-28 15:01:11.000000 piqp-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-28 15:01:25.004776 piqp-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-28 15:01:11.000000 piqp-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:01:25.000776 piqp-0.1.0/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:01:25.000776 piqp-0.1.0/interfaces/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:01:25.004776 piqp-0.1.0/interfaces/python/piqp/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-28 15:01:11.000000 piqp-0.1.0/interfaces/python/piqp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:01:25.004776 piqp-0.1.0/piqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-28 15:01:24.000000 piqp-0.1.0/piqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-28 15:01:25.000000 piqp-0.1.0/piqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:01:24.000000 piqp-0.1.0/piqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:01:24.000000 piqp-0.1.0/piqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 15:01:24.000000 piqp-0.1.0/piqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-28 15:01:24.000000 piqp-0.1.0/piqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-28 15:01:11.000000 piqp-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:01:25.004776 piqp-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-06-28 15:01:11.000000 piqp-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:22.277158 piqp-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-30 15:05:08.000000 piqp-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-30 15:05:22.277158 piqp-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-30 15:05:08.000000 piqp-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:22.277158 piqp-0.1.1/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:22.277158 piqp-0.1.1/interfaces/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:22.277158 piqp-0.1.1/interfaces/python/piqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-30 15:05:08.000000 piqp-0.1.1/interfaces/python/piqp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:05:22.277158 piqp-0.1.1/piqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-30 15:05:22.000000 piqp-0.1.1/piqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 15:05:22.000000 piqp-0.1.1/piqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:05:22.000000 piqp-0.1.1/piqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:05:22.000000 piqp-0.1.1/piqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 15:05:22.000000 piqp-0.1.1/piqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-30 15:05:22.000000 piqp-0.1.1/piqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-30 15:05:08.000000 piqp-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:05:22.277158 piqp-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-06-30 15:05:08.000000 piqp-0.1.1/setup.py
```

### Comparing `piqp-0.1.0/LICENSE` & `piqp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `piqp-0.1.0/PKG-INFO` & `piqp-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.1.0
+Version: 0.1.1
 Summary: An embedded Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `piqp-0.1.0/README.md` & `piqp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `piqp-0.1.0/interfaces/python/piqp/__init__.py` & `piqp-0.1.1/interfaces/python/piqp/__init__.py`

 * *Files identical despite different names*

### Comparing `piqp-0.1.0/piqp.egg-info/PKG-INFO` & `piqp-0.1.1/piqp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.1.0
+Version: 0.1.1
 Summary: An embedded Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `piqp-0.1.0/pyproject.toml` & `piqp-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piqp-0.1.0/setup.py` & `piqp-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="piqp",
-    version="0.1.0",
+    version="0.1.1",
     url='https://github.com/PREDICT-EPFL/piqp',
     author="Roland Schwan",
     author_email="roland.schwan@epfl.ch",
     license='BSD-2-Clause',
     description="An embedded Proximal Interior Point Quadratic Programming solver",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

