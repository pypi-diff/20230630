# Comparing `tmp/pypdtools-0.0.1.tar.gz` & `tmp/pypdtools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdtools-0.0.1.tar", last modified: Fri Jun 30 15:45:57 2023, max compression
+gzip compressed data, was "pypdtools-0.0.2.tar", last modified: Fri Jun 30 18:20:35 2023, max compression
```

## Comparing `pypdtools-0.0.1.tar` & `pypdtools-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:45:57.973132 pypdtools-0.0.1/
--rw-rw-rw-   0        0        0     1511 2023-06-28 17:19:48.000000 pypdtools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2518 2023-06-30 15:45:57.973132 pypdtools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1850 2023-06-30 15:40:55.000000 pypdtools-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 15:45:57.931609 pypdtools-0.0.1/pypdtools/
-drwxrwxrwx   0        0        0        0 2023-06-30 15:45:57.941610 pypdtools-0.0.1/pypdtools/abc/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.1/pypdtools/abc/__init__.py
--rw-rw-rw-   0        0        0      677 2023-06-28 21:28:40.000000 pypdtools-0.0.1/pypdtools/abc/dataframe.py
--rw-rw-rw-   0        0        0      709 2023-06-30 15:31:22.000000 pypdtools-0.0.1/pypdtools/abc/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:45:57.946614 pypdtools-0.0.1/pypdtools/core/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.1/pypdtools/core/__init__.py
--rw-rw-rw-   0        0        0     6568 2023-06-30 15:31:22.000000 pypdtools-0.0.1/pypdtools/core/dataframe.py
--rw-rw-rw-   0        0        0     2627 2023-06-30 15:31:22.000000 pypdtools-0.0.1/pypdtools/core/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:45:57.970130 pypdtools-0.0.1/pypdtools/pypdtools.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-06-30 15:45:57.000000 pypdtools-0.0.1/pypdtools/pypdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-06-30 15:45:57.000000 pypdtools-0.0.1/pypdtools/pypdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:45:57.000000 pypdtools-0.0.1/pypdtools/pypdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2023-06-30 15:45:57.000000 pypdtools-0.0.1/pypdtools/pypdtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-30 15:45:57.000000 pypdtools-0.0.1/pypdtools/pypdtools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 15:45:57.972132 pypdtools-0.0.1/pypdtools/utils/
--rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.1/pypdtools/utils/__init__.py
--rw-rw-rw-   0        0        0     2207 2023-06-30 14:41:49.000000 pypdtools-0.0.1/pypdtools/utils/asyncs.py
--rw-rw-rw-   0        0        0     1772 2023-06-30 15:37:27.000000 pypdtools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-06-30 15:45:57.978133 pypdtools-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 18:20:35.401129 pypdtools-0.0.2/
+-rw-rw-rw-   0        0        0     1511 2023-06-28 17:19:48.000000 pypdtools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2518 2023-06-30 18:20:35.400128 pypdtools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1850 2023-06-30 15:40:55.000000 pypdtools-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 18:20:35.366121 pypdtools-0.0.2/pypdtools/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.2/pypdtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:20:35.392127 pypdtools-0.0.2/pypdtools/abc/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.2/pypdtools/abc/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-06-28 21:28:40.000000 pypdtools-0.0.2/pypdtools/abc/dataframe.py
+-rw-rw-rw-   0        0        0      709 2023-06-30 15:31:22.000000 pypdtools-0.0.2/pypdtools/abc/scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:20:35.396128 pypdtools-0.0.2/pypdtools/core/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.2/pypdtools/core/__init__.py
+-rw-rw-rw-   0        0        0     6568 2023-06-30 15:31:22.000000 pypdtools-0.0.2/pypdtools/core/dataframe.py
+-rw-rw-rw-   0        0        0     2627 2023-06-30 15:31:22.000000 pypdtools-0.0.2/pypdtools/core/scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:20:35.398129 pypdtools-0.0.2/pypdtools/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-28 17:19:48.000000 pypdtools-0.0.2/pypdtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2207 2023-06-30 14:41:49.000000 pypdtools-0.0.2/pypdtools/utils/asyncs.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:20:35.388127 pypdtools-0.0.2/pypdtools.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-06-30 18:20:35.000000 pypdtools-0.0.2/pypdtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-30 18:20:35.000000 pypdtools-0.0.2/pypdtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 18:20:35.000000 pypdtools-0.0.2/pypdtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      230 2023-06-30 18:20:35.000000 pypdtools-0.0.2/pypdtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 18:20:35.000000 pypdtools-0.0.2/pypdtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1917 2023-06-30 18:15:14.000000 pypdtools-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 18:20:35.401129 pypdtools-0.0.2/setup.cfg
```

### Comparing `pypdtools-0.0.1/LICENSE` & `pypdtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/PKG-INFO` & `pypdtools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package with tools for pandas
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>
 Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/
 Project-URL: Bug Tracker, https://github.com/msbar/pypdtools/issues
 Keywords: pandas,tools,asyncio
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypdtools Version: 0.0.1 Summary: Package with
+Metadata-Version: 2.1 Name: pypdtools Version: 0.0.2 Summary: Package with
 tools for pandas Author-email: Marciel Barcellos
 barcellos@tcmrio.tc.br> Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/ Project-URL: Bug
 Tracker, https://github.com/msbar/pypdtools/issues Keywords:
 pandas,tools,asyncio Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `pypdtools-0.0.1/README.md` & `pypdtools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/pypdtools/abc/dataframe.py` & `pypdtools-0.0.2/pypdtools/abc/dataframe.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/pypdtools/abc/scripts.py` & `pypdtools-0.0.2/pypdtools/abc/scripts.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/pypdtools/core/dataframe.py` & `pypdtools-0.0.2/pypdtools/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/pypdtools/core/scripts.py` & `pypdtools-0.0.2/pypdtools/core/scripts.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/pypdtools/pypdtools.egg-info/PKG-INFO` & `pypdtools-0.0.2/pypdtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package with tools for pandas
 Author-email: Marciel Barcellos <marciel.barcellos@tcmrio.tc.br>
 Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/
 Project-URL: Bug Tracker, https://github.com/msbar/pypdtools/issues
 Keywords: pandas,tools,asyncio
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypdtools Version: 0.0.1 Summary: Package with
+Metadata-Version: 2.1 Name: pypdtools Version: 0.0.2 Summary: Package with
 tools for pandas Author-email: Marciel Barcellos
 barcellos@tcmrio.tc.br> Project-URL: source, https://github.com/msbar/pypdtools
 Project-URL: Documentation, https://msbar.github.io/pypdtools/ Project-URL: Bug
 Tracker, https://github.com/msbar/pypdtools/issues Keywords:
 pandas,tools,asyncio Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `pypdtools-0.0.1/pypdtools/utils/asyncs.py` & `pypdtools-0.0.2/pypdtools/utils/asyncs.py`

 * *Files identical despite different names*

### Comparing `pypdtools-0.0.1/pyproject.toml` & `pypdtools-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0" , "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = true
+
+[tool.setuptools.packages.find]
+include = ["pypdtools", "pypdtools.*"]
+namespaces = false
+
 [project]
 name = "pypdtools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Marciel Barcellos", email="marciel.barcellos@tcmrio.tc.br" }
 ]
 description = "Package with tools for pandas"
 
 readme = "README.md"
 requires-python = ">=3.7"
```

