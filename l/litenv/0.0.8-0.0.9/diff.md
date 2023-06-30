# Comparing `tmp/litenv-0.0.8.tar.gz` & `tmp/litenv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litenv-0.0.8.tar", last modified: Sun Jun 18 14:46:44 2023, max compression
+gzip compressed data, was "litenv-0.0.9.tar", last modified: Mon Jun 19 18:53:45 2023, max compression
```

## Comparing `litenv-0.0.8.tar` & `litenv-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 14:46:44.398560 litenv-0.0.8/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.8/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-18 14:46:44.398402 litenv-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 14:46:44.398185 litenv-0.0.8/data/
--rw-r--r--   0 solst      (501) staff       (20)     5264 2023-06-18 14:46:35.000000 litenv-0.0.8/data/litenv.yml
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 14:46:44.396762 litenv-0.0.8/litenv/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.8/litenv/core.py
--rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.8/litenv/defaults.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.8/litenv/tests.py
--rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/themes.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/typer.py
--rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/types.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-18 14:46:40.000000 litenv-0.0.8/litenv/utils.py
--rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.8/litenv/yml.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 14:46:44.398022 litenv-0.0.8/litenv.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-18 14:46:44.000000 litenv-0.0.8/litenv.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-18 14:46:44.000000 litenv-0.0.8/litenv.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-18 14:46:44.000000 litenv-0.0.8/litenv.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-18 14:46:44.000000 litenv-0.0.8/litenv.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.8/litenv.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-18 14:46:44.000000 litenv-0.0.8/litenv.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-18 14:46:44.000000 litenv-0.0.8/litenv.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-18 14:46:40.000000 litenv-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-18 14:46:44.398611 litenv-0.0.8/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-19 18:53:45.431337 litenv-0.0.9/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 litenv-0.0.9/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 litenv-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-19 18:53:45.431192 litenv-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     7305 2023-06-07 17:36:08.000000 litenv-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-19 18:53:45.430995 litenv-0.0.9/data/
+-rw-r--r--   0 solst      (501) staff       (20)     5275 2023-06-19 18:53:11.000000 litenv-0.0.9/data/litenv.yml
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-19 18:53:45.429812 litenv-0.0.9/litenv/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    25532 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3947 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2408 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      142 2023-06-05 12:16:38.000000 litenv-0.0.9/litenv/core.py
+-rw-r--r--   0 solst      (501) staff       (20)    24475 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)    11704 2023-06-05 22:16:07.000000 litenv-0.0.9/litenv/defaults.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      977 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      216 2023-06-05 22:16:07.000000 litenv-0.0.9/litenv/tests.py
+-rw-r--r--   0 solst      (501) staff       (20)     4104 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/themes.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)      269 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/types.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-19 18:53:39.000000 litenv-0.0.9/litenv/utils.py
+-rw-r--r--   0 solst      (501) staff       (20)     5788 2023-06-06 17:57:47.000000 litenv-0.0.9/litenv/yml.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-19 18:53:45.430873 litenv-0.0.9/litenv.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     8081 2023-06-19 18:53:45.000000 litenv-0.0.9/litenv.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      562 2023-06-19 18:53:45.000000 litenv-0.0.9/litenv.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-19 18:53:45.000000 litenv-0.0.9/litenv.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       96 2023-06-19 18:53:45.000000 litenv-0.0.9/litenv.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-05 14:20:25.000000 litenv-0.0.9/litenv.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       37 2023-06-19 18:53:45.000000 litenv-0.0.9/litenv.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-19 18:53:45.000000 litenv-0.0.9/litenv.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      933 2023-06-19 18:53:35.000000 litenv-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-19 18:53:45.431379 litenv-0.0.9/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2671 2023-06-05 19:37:38.000000 litenv-0.0.9/setup.py
```

### Comparing `litenv-0.0.8/LICENSE` & `litenv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/PKG-INFO` & `litenv-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.8
+Version: 0.0.9
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `litenv-0.0.8/README.md` & `litenv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/data/litenv.yml` & `litenv-0.0.9/data/litenv.yml`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     dependencies:
       notebook:
         channel: conda-forge
         always: true
       ipykernel:
         channel: conda-forge
         always: true
-      ipywidget:
+      ipywidgets:
         channel: conda-forge
         always: true
       jupyterlab:
         channel: conda-forge
         always: true
 
   nbdev:
@@ -217,19 +217,19 @@
       sc:
         name: 'Single-Cell'
         dependencies:
           scprep:
             channel: bioconda
           magic-impute:
             pip_only: true
-          meld:
-            pip_only: true
-          degex:
-            pip_only: true
-            note: 'personal collection of utility functions developed with Scott Youlten'
+          # meld:
+          #   pip_only: true
+          # degex:
+          #   pip_only: true
+          #   note: 'personal collection of utility functions developed with Scott Youlten'
 
       ms:
         name: 'Multiscale Analysis'
         dependencies:
           'git+https://github.com/KrishnaswamyLab/Multiscale_PHATE':
             pip_only: true
```

### Comparing `litenv-0.0.8/litenv/_modidx.py` & `litenv-0.0.9/litenv/_modidx.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/commands.py` & `litenv-0.0.9/litenv/commands.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/constants.py` & `litenv-0.0.9/litenv/constants.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/dataclasses.py` & `litenv-0.0.9/litenv/dataclasses.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/defaults.py` & `litenv-0.0.9/litenv/defaults.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/paths.py` & `litenv-0.0.9/litenv/paths.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/rich.py` & `litenv-0.0.9/litenv/rich.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/themes.py` & `litenv-0.0.9/litenv/themes.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv/yml.py` & `litenv-0.0.9/litenv/yml.py`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/litenv.egg-info/PKG-INFO` & `litenv-0.0.9/litenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litenv
-Version: 0.0.8
+Version: 0.0.9
 Summary: quickly make pytorch environments with mamba
 Home-page: https://github.com/dsm-72/litenv
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `litenv-0.0.8/litenv.egg-info/SOURCES.txt` & `litenv-0.0.9/litenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litenv-0.0.8/settings.ini` & `litenv-0.0.9/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = litenv
 lib_name = litenv
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = litenv
 nbs_path = nbs
 recursive = True
```

### Comparing `litenv-0.0.8/setup.py` & `litenv-0.0.9/setup.py`

 * *Files identical despite different names*

