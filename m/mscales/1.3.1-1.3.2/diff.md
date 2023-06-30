# Comparing `tmp/mscales-1.3.1.tar.gz` & `tmp/mscales-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.3.1.tar", last modified: Wed Jun 14 15:22:08 2023, max compression
+gzip compressed data, was "mscales-1.3.2.tar", last modified: Fri Jun 30 10:38:20 2023, max compression
```

## Comparing `mscales-1.3.1.tar` & `mscales-1.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.3.1/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.3.1/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.3.1/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1244 2023-06-14 15:22:08.787914 mscales-1.3.1/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      790 2023-05-31 17:16:11.000000 mscales-1.3.1/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.783914 mscales-1.3.1/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      673 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      797 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      419 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/pcsets.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1012 2023-06-14 13:57:39.000000 mscales-1.3.1/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.3.1/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      230 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     6596 2023-05-31 17:25:07.000000 mscales-1.3.1/mscales/pcsets.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-05-31 17:16:11.000000 mscales-1.3.1/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-14 15:22:08.787914 mscales-1.3.1/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1244 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      683 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        6 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-06-14 15:22:08.000000 mscales-1.3.1/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      276 2023-05-31 17:16:11.000000 mscales-1.3.1/pyproject.toml
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       58 2023-05-31 17:16:11.000000 mscales-1.3.1/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-06-14 15:22:08.787914 mscales-1.3.1/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-05-31 17:16:11.000000 mscales-1.3.1/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.3.1/versioneer.py
+drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.429272 mscales-1.3.2/
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      170 2023-06-30 05:22:16.000000 mscales-1.3.2/AUTHORS.rst
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-06-30 05:22:16.000000 mscales-1.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-06-30 05:22:16.000000 mscales-1.3.2/LICENSE
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      360 2023-06-30 05:22:16.000000 mscales-1.3.2/MANIFEST.in
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1409 2023-06-30 10:38:20.429272 mscales-1.3.2/PKG-INFO
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      954 2023-06-30 05:22:16.000000 mscales-1.3.2/README.rst
+drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.407605 mscales-1.3.2/docs/
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      673 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/Makefile
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      797 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/make.bat
+drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.418438 mscales-1.3.2/docs/source/
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     7388 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/conf.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      419 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/index.rst
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3578 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/pcsets.rst
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/quickstart.rst
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1100 2023-06-30 10:33:51.000000 mscales-1.3.2/docs/source/release-history.rst
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)       71 2023-06-30 05:22:16.000000 mscales-1.3.2/docs/source/scales.rst
+drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.440105 mscales-1.3.2/mscales/
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      230 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/__init__.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      497 2023-06-30 10:38:20.440105 mscales-1.3.2/mscales/_version.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      529 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/concepts.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     8622 2023-06-30 10:26:06.000000 mscales-1.3.2/mscales/pcsets.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/plots.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/scales.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/sound.py
+drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.429272 mscales-1.3.2/mscales/tests/
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/tests/__init__.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/tests/conftest.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      160 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/tests/test_examples.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     3056 2023-06-30 05:22:16.000000 mscales-1.3.2/mscales/utils.py
+drwxr-xr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-06-30 10:38:20.429272 mscales-1.3.2/mscales.egg-info/
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     1409 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/PKG-INFO
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      683 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/SOURCES.txt
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)        1 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/dependency_links.txt
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)        6 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/requires.txt
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)        8 2023-06-30 10:38:20.000000 mscales-1.3.2/mscales.egg-info/top_level.txt
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      276 2023-06-30 05:22:16.000000 mscales-1.3.2/pyproject.toml
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)       58 2023-06-30 05:22:16.000000 mscales-1.3.2/requirements.txt
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)      178 2023-06-30 10:38:20.429272 mscales-1.3.2/setup.cfg
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-30 05:22:16.000000 mscales-1.3.2/setup.py
+-rw-r--r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-06-30 05:22:16.000000 mscales-1.3.2/versioneer.py
```

### Comparing `mscales-1.3.1/CONTRIBUTING.rst` & `mscales-1.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/LICENSE` & `mscales-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/PKG-INFO` & `mscales-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -30,7 +30,15 @@
         :alt: Documentation Status
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
+
+Notes for development
+---------------------
+
+- `python3 -m pip install -e .``
+- `python3 -m pip install --upgrade -r requirements-dev.txt`
+
+Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.1/docs/Makefile` & `mscales-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/docs/make.bat` & `mscales-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/docs/source/conf.py` & `mscales-1.3.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 release = mscales.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `mscales-1.3.1/docs/source/pcsets.rst` & `mscales-1.3.2/docs/source/pcsets.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/docs/source/quickstart.rst` & `mscales-1.3.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/docs/source/release-history.rst` & `mscales-1.3.2/docs/source/release-history.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release History
 ===============
 
+v1.3.2 (2023-06-30)
+-------------------
+
+- fix prime-form and normal-form calculations
+
 v1.3.1 (2023-06-14)
 -------------------
 
 - update flake8 settings
 
 v1.3.0 (2023-05-31)
 -------------------
```

### Comparing `mscales-1.3.1/mscales/concepts.py` & `mscales-1.3.2/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/mscales/plots.py` & `mscales-1.3.2/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/mscales/scales.py` & `mscales-1.3.2/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/mscales/sound.py` & `mscales-1.3.2/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/mscales/utils.py` & `mscales-1.3.2/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/mscales.egg-info/PKG-INFO` & `mscales-1.3.2/mscales.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
@@ -30,7 +30,15 @@
         :alt: Documentation Status
 
 Python package to generate, visualize, and sonify musical scales.
 
 * Free software: 3-clause BSD license
 * Documentation: https://mscales.readthedocs.io/en/latest/.
 * Package build with a `cookiecutter template <https://nsls-ii.github.io/scientific-python-cookiecutter/index.html>`_
+
+Notes for development
+---------------------
+
+- `python3 -m pip install -e .``
+- `python3 -m pip install --upgrade -r requirements-dev.txt`
+
+Creator: Fabian C. Moss
```

### Comparing `mscales-1.3.1/mscales.egg-info/SOURCES.txt` & `mscales-1.3.2/mscales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/setup.py` & `mscales-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.3.1/versioneer.py` & `mscales-1.3.2/versioneer.py`

 * *Files identical despite different names*

