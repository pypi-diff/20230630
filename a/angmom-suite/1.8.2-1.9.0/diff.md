# Comparing `tmp/angmom_suite-1.8.2.tar.gz` & `tmp/angmom_suite-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angmom_suite-1.8.2.tar", last modified: Thu Jun  9 10:34:33 2022, max compression
+gzip compressed data, was "angmom_suite-1.9.0.tar", last modified: Mon Jun 13 09:58:28 2022, max compression
```

## Comparing `angmom_suite-1.8.2.tar` & `angmom_suite-1.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 10:34:33.959519 angmom_suite-1.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     2790 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     5081 2022-06-09 10:34:30.000000 angmom_suite-1.8.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    35072 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3689 2022-06-09 10:34:33.959519 angmom_suite-1.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2970 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 10:34:33.956519 angmom_suite-1.8.2/angmom_suite/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2022-06-09 10:34:30.000000 angmom_suite-1.8.2/angmom_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     9496 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)    22997 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/basis.py
--rw-rw-rw-   0 root         (0) root         (0)     4050 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    31970 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/crystal.py
--rw-rw-rw-   0 root         (0) root         (0)    14051 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/multi_electron.py
--rw-rw-rw-   0 root         (0) root         (0)     3414 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/angmom_suite/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 10:34:33.958519 angmom_suite-1.8.2/angmom_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3689 2022-06-09 10:34:33.000000 angmom_suite-1.8.2/angmom_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      680 2022-06-09 10:34:33.000000 angmom_suite-1.8.2/angmom_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-09 10:34:33.000000 angmom_suite-1.8.2/angmom_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-06-09 10:34:33.000000 angmom_suite-1.8.2/angmom_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-06-09 10:34:33.000000 angmom_suite-1.8.2/angmom_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      175 2022-06-09 10:33:45.000000 angmom_suite-1.8.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-09 10:34:33.959519 angmom_suite-1.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1230 2022-06-09 10:34:30.000000 angmom_suite-1.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 09:58:28.271882 angmom_suite-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5106 2022-06-13 09:58:19.000000 angmom_suite-1.9.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3689 2022-06-13 09:58:28.268882 angmom_suite-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 09:58:28.263881 angmom_suite-1.9.0/angmom_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2022-06-13 09:58:19.000000 angmom_suite-1.9.0/angmom_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9496 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)    22997 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/basis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3830 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    31970 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/crystal.py
+-rw-rw-rw-   0 root         (0) root         (0)    14051 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/multi_electron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/angmom_suite/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 09:58:28.268882 angmom_suite-1.9.0/angmom_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3689 2022-06-13 09:58:25.000000 angmom_suite-1.9.0/angmom_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      680 2022-06-13 09:58:28.000000 angmom_suite-1.9.0/angmom_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 09:58:26.000000 angmom_suite-1.9.0/angmom_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2022-06-13 09:58:27.000000 angmom_suite-1.9.0/angmom_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-06-13 09:58:27.000000 angmom_suite-1.9.0/angmom_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      175 2022-06-13 09:57:57.000000 angmom_suite-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-13 09:58:28.271882 angmom_suite-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2022-06-13 09:58:19.000000 angmom_suite-1.9.0/setup.py
```

### Comparing `angmom_suite-1.8.2/.gitlab-ci.yml` & `angmom_suite-1.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/CHANGELOG.md` & `angmom_suite-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.9.0 (2022-06-13)
+
+
 ## v1.8.2 (2022-06-09)
 
 
 ## v1.8.1 (2022-05-19)
 ### Fix
 * Ion parser ([`4ca435c`](https://gitlab.com/chilton-group/angmom_suite/-/commit/4ca435c34b3ea41864db0ba233284ce532710f6d))
```

### Comparing `angmom_suite-1.8.2/LICENSE` & `angmom_suite-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/PKG-INFO` & `angmom_suite-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angmom_suite
-Version: 1.8.2
+Version: 1.9.0
 Summary: A package for working with phenomenological spin and angular momentum operators
 Home-page: https://github.com/chilton-group/angmom_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/chilton-group/angmom_suite/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/angmom_suite
```

### Comparing `angmom_suite-1.8.2/README.md` & `angmom_suite-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/angmom_suite/barrier.py` & `angmom_suite-1.9.0/angmom_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/angmom_suite/basis.py` & `angmom_suite-1.9.0/angmom_suite/basis.py`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/angmom_suite/cli.py` & `angmom_suite-1.9.0/angmom_suite/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from argparse import ArgumentParser, ArgumentTypeError, Action, \
-        RawDescriptionHelpFormatter
+from argparse import ArgumentParser, Action, RawDescriptionHelpFormatter
 import h5py
 import hpc_suite as hpc
 from .multi_electron import Ion, parse_termsymbol
-from molcas_suite.extractor import make_extractor
 
 
 # Action for secondary help message
 class SecondaryHelp(hpc.SecondaryHelp):
     def __init__(self, option_strings, dest=None, const=None, default=None,
                  help=None):
         super().__init__(option_strings, dest=dest, const=const,
@@ -28,18 +26,16 @@
         )
 
     def __call__(self, parser, namespace, value, option_string=None):
 
         if hpc.store.is_hdf5(value[0]):  # import from HDF5 database
             with h5py.File(value[0], 'r') as h:
                 quax = h["quax"][...]
-        else:  # extract from Molcas calculation
-            if namespace.basis is None:
-                raise ValueError("Specify --basis before --quax")
-            quax = make_extractor(value[0], ("quax", namespace.basis))[1]
+        else:
+            raise ValueError("Invalid file type for QUAX specification.")
 
         setattr(namespace, self.dest, quax)
 
 
 cfp_parser = ArgumentParser(
         formatter_class=RawDescriptionHelpFormatter,
         add_help=False
```

### Comparing `angmom_suite-1.8.2/angmom_suite/crystal.py` & `angmom_suite-1.9.0/angmom_suite/crystal.py`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/angmom_suite/multi_electron.py` & `angmom_suite-1.9.0/angmom_suite/multi_electron.py`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/angmom_suite/utils.py` & `angmom_suite-1.9.0/angmom_suite/utils.py`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/angmom_suite.egg-info/PKG-INFO` & `angmom_suite-1.9.0/angmom_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angmom-suite
-Version: 1.8.2
+Version: 1.9.0
 Summary: A package for working with phenomenological spin and angular momentum operators
 Home-page: https://github.com/chilton-group/angmom_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/chilton-group/angmom_suite/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/angmom_suite
```

### Comparing `angmom_suite-1.8.2/angmom_suite.egg-info/SOURCES.txt` & `angmom_suite-1.9.0/angmom_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angmom_suite-1.8.2/setup.py` & `angmom_suite-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.8.2"
+__version__ = "1.9.0"
 
 setuptools.setup(
     name="angmom_suite",
     version=__version__,
     author="Chilton Group",
     author_email="nicholas.chilton@manchester.ac.uk",
     description="A package for working with phenomenological spin and angular momentum operators", # noqa
```

