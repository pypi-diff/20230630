# Comparing `tmp/collective.recipe.vscode-0.1.8.tar.gz` & `tmp/collective.recipe.vscode-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.recipe.vscode-0.1.8.tar", last modified: Thu Oct 28 14:40:38 2021, max compression
+gzip compressed data, was "collective.recipe.vscode-0.1.9.tar", last modified: Fri Jun 30 20:45:03 2023, max compression
```

## Comparing `collective.recipe.vscode-0.1.8.tar` & `collective.recipe.vscode-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/
--rw-r--r--   0 nazrul     (501) staff       (20)     2333 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/CHANGES.rst
--rw-r--r--   0 nazrul     (501) staff       (20)      105 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/CONTRIBUTORS.rst
--rw-r--r--   0 nazrul     (501) staff       (20)      127 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/MANIFEST.in
--rw-r--r--   0 nazrul     (501) staff       (20)    15836 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/PKG-INFO
--rw-r--r--   0 nazrul     (501) staff       (20)     6575 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/README.rst
--rw-r--r--   0 nazrul     (501) staff       (20)      247 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/setup.cfg
--rw-r--r--   0 nazrul     (501) staff       (20)     2440 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/setup.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/
--rw-r--r--   0 nazrul     (501) staff       (20)       80 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/__init__.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/
--rw-r--r--   0 nazrul     (501) staff       (20)       80 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/__init__.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/
--rw-r--r--   0 nazrul     (501) staff       (20)      170 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)    19434 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/recipes.py
--rw-r--r--   0 nazrul     (501) staff       (20)     2312 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/recipes.rst
--rw-r--r--   0 nazrul     (501) staff       (20)     1257 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/settings_mappings.json
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/Products/
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/Products/VSCodeTestProduct/
--rw-r--r--   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/Products/VSCodeTestProduct/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)        1 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/Products/VSCodeTestProduct/production.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/__init__.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/
--rw-r--r--   0 nazrul     (501) staff       (20)      777 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/.gitignore
--rw-r--r--   0 nazrul     (501) staff       (20)     1075 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/LICENSE
--rw-r--r--   0 nazrul     (501) staff       (20)       34 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/MANIFEST.in
--rw-r--r--   0 nazrul     (501) staff       (20)     1170 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/README.rst
--rw-r--r--   0 nazrul     (501) staff       (20)     1361 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/setup.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/vscodetest_pkg1/
--rw-r--r--   0 nazrul     (501) staff       (20)      119 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/vscodetest_pkg1/__init__.py
--rw-r--r--   0 nazrul     (501) staff       (20)       24 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/vscodetest_pkg1/sublimtexttest_pkg1.py
--rw-r--r--   0 nazrul     (501) staff       (20)     1987 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/test_docs.py
--rw-r--r--   0 nazrul     (501) staff       (20)    16368 2021-10-28 14:40:37.000000 collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/test_recipes.py
-drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/
--rw-r--r--   0 nazrul     (501) staff       (20)    15836 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/PKG-INFO
--rw-r--r--   0 nazrul     (501) staff       (20)     1559 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/SOURCES.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        1 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/dependency_links.txt
--rw-r--r--   0 nazrul     (501) staff       (20)      127 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/entry_points.txt
--rw-r--r--   0 nazrul     (501) staff       (20)       29 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/namespace_packages.txt
--rw-r--r--   0 nazrul     (501) staff       (20)        1 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/not-zip-safe
--rw-r--r--   0 nazrul     (501) staff       (20)       90 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/requires.txt
--rw-r--r--   0 nazrul     (501) staff       (20)       11 2021-10-28 14:40:38.000000 collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/top_level.txt
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.789227 collective.recipe.vscode-0.1.9/
+-rw-r--r--   0 nazrul     (501) staff       (20)     2489 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/CHANGES.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)      105 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/CONTRIBUTORS.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)      127 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/MANIFEST.in
+-rw-r--r--   0 nazrul     (501) staff       (20)    16563 2023-06-30 20:45:03.789323 collective.recipe.vscode-0.1.9/PKG-INFO
+-rw-r--r--   0 nazrul     (501) staff       (20)     6909 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/README.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)      247 2023-06-30 20:45:03.789527 collective.recipe.vscode-0.1.9/setup.cfg
+-rw-r--r--   0 nazrul     (501) staff       (20)     2539 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/setup.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.785254 collective.recipe.vscode-0.1.9/src/
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.786472 collective.recipe.vscode-0.1.9/src/collective/
+-rw-r--r--   0 nazrul     (501) staff       (20)       80 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/__init__.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.787444 collective.recipe.vscode-0.1.9/src/collective/recipe/
+-rw-r--r--   0 nazrul     (501) staff       (20)       80 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/__init__.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.787867 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/
+-rw-r--r--   0 nazrul     (501) staff       (20)      170 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    23065 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/recipes.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     2312 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/recipes.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)     1301 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/settings_mappings.json
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.788164 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.785574 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/Products/
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.788373 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/Products/VSCodeTestProduct/
+-rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/Products/VSCodeTestProduct/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/Products/VSCodeTestProduct/production.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/__init__.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.785693 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.788909 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/
+-rw-r--r--   0 nazrul     (501) staff       (20)      777 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/.gitignore
+-rw-r--r--   0 nazrul     (501) staff       (20)     1075 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/LICENSE
+-rw-r--r--   0 nazrul     (501) staff       (20)       34 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/MANIFEST.in
+-rw-r--r--   0 nazrul     (501) staff       (20)     1170 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/README.rst
+-rw-r--r--   0 nazrul     (501) staff       (20)     1361 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/setup.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.789123 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/vscodetest_pkg1/
+-rw-r--r--   0 nazrul     (501) staff       (20)      119 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/vscodetest_pkg1/__init__.py
+-rw-r--r--   0 nazrul     (501) staff       (20)       24 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/vscodetest_pkg1/sublimtexttest_pkg1.py
+-rw-r--r--   0 nazrul     (501) staff       (20)     1987 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/test_docs.py
+-rw-r--r--   0 nazrul     (501) staff       (20)    16368 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/test_recipes.py
+drwxr-xr-x   0 nazrul     (501) staff       (20)        0 2023-06-30 20:45:03.787335 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/
+-rw-r--r--   0 nazrul     (501) staff       (20)    16563 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/PKG-INFO
+-rw-r--r--   0 nazrul     (501) staff       (20)     1559 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)      127 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/entry_points.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)       29 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/namespace_packages.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)        1 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/not-zip-safe
+-rw-r--r--   0 nazrul     (501) staff       (20)       90 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/requires.txt
+-rw-r--r--   0 nazrul     (501) staff       (20)       11 2023-06-30 20:45:03.000000 collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.recipe.vscode-0.1.8/CHANGES.rst` & `collective.recipe.vscode-0.1.9/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+0.1.9 (2023-06-30)
+------------------
+
+- Add option `robot-enabled` (default *false*) to enable support for Robot Framework Language Server
+  [datakurre]
+
+
 0.1.8 (2021-10-28)
 ------------------
 
 - Change languageserver to Pylance (Microsoft no longer works)
 - Default to generating .env file to aid in debugging
 - Options are removed. ``jedi-path``
 - ``vsintellicode.python.completionsEnabled`` is no longer part of VS code settings.
```

### Comparing `collective.recipe.vscode-0.1.8/PKG-INFO` & `collective.recipe.vscode-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: collective.recipe.vscode
-Version: 0.1.8
+Version: 0.1.9
 Summary: Visual Studio Code configuration for buildout-based Python projects
 Home-page: https://github.com/nazrulworld/collective.recipe.vscode
 Author: Md Nazrul Islam
 Author-email: email2nazrul@gmail.com
 License: GPL version 2
 Description: .. image:: https://img.shields.io/pypi/status/collective.recipe.vscode.svg
             :target: https://pypi.org/project/collective.recipe.vscode/
             :alt: Package Status
         
-        .. image:: https://travis-ci.org/nazrulworld/collective.recipe.vscode.svg?branch=master
-            :target: https://travis-ci.org/nazrulworld/collective.recipe.vscode
+        .. image:: https://app.travis-ci.com/nazrulworld/collective.recipe.vscode.svg?branch=master
+            :target: https://app.travis-ci.com/nazrulworld/collective.recipe.vscode
             :alt: Travis Build Status
         
         .. image:: https://coveralls.io/repos/github/nazrulworld/collective.recipe.vscode/badge.svg?branch=master
             :target: https://coveralls.io/github/nazrulworld/collective.recipe.vscode?branch=master
             :alt: Test Coverage
         .. image:: https://img.shields.io/pypi/pyversions/collective.recipe.vscode.svg
             :target: https://pypi.org/project/collective.recipe.vscode/
@@ -224,14 +224,24 @@
         generate-envfile
             Required: No
         
             Default: True
         
             Generate .env file to add eggs to PYTHONPATH
         
+        robot-enabled
+            Required: No
+        
+            Default: False
+        
+            Generate setting `robot.python.env` with buildout eggs for Robot Framework Language Server.
+            Generate task **Start Plone Test Server** into `tasks.json`.
+            Generate task **Robot Framework: Launch Template** into `launch.json` for Robot Framework Language Server.
+        
+        
         Links
         =====
         
         Code repository:
         
             https://github.com/nazrulworld/collective.recipe.vscode
         
@@ -336,14 +346,21 @@
         - Md Nazrul Islam<email2nazrul@gmail.com>, Original Author.
         - Matteo Parrucci
         
         
         Changelog
         =========
         
+        0.1.9 (2023-06-30)
+        ------------------
+        
+        - Add option `robot-enabled` (default *false*) to enable support for Robot Framework Language Server
+          [datakurre]
+        
+        
         0.1.8 (2021-10-28)
         ------------------
         
         - Change languageserver to Pylance (Microsoft no longer works)
         - Default to generating .env file to aid in debugging
         - Options are removed. ``jedi-path``
         - ``vsintellicode.python.completionsEnabled`` is no longer part of VS code settings.
@@ -429,11 +446,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
```

### Comparing `collective.recipe.vscode-0.1.8/README.rst` & `collective.recipe.vscode-0.1.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. image:: https://img.shields.io/pypi/status/collective.recipe.vscode.svg
     :target: https://pypi.org/project/collective.recipe.vscode/
     :alt: Package Status
 
-.. image:: https://travis-ci.org/nazrulworld/collective.recipe.vscode.svg?branch=master
-    :target: https://travis-ci.org/nazrulworld/collective.recipe.vscode
+.. image:: https://app.travis-ci.com/nazrulworld/collective.recipe.vscode.svg?branch=master
+    :target: https://app.travis-ci.com/nazrulworld/collective.recipe.vscode
     :alt: Travis Build Status
 
 .. image:: https://coveralls.io/repos/github/nazrulworld/collective.recipe.vscode/badge.svg?branch=master
     :target: https://coveralls.io/github/nazrulworld/collective.recipe.vscode?branch=master
     :alt: Test Coverage
 .. image:: https://img.shields.io/pypi/pyversions/collective.recipe.vscode.svg
     :target: https://pypi.org/project/collective.recipe.vscode/
@@ -216,14 +216,24 @@
 generate-envfile
     Required: No
 
     Default: True
 
     Generate .env file to add eggs to PYTHONPATH
 
+robot-enabled
+    Required: No
+
+    Default: False
+
+    Generate setting `robot.python.env` with buildout eggs for Robot Framework Language Server.
+    Generate task **Start Plone Test Server** into `tasks.json`.
+    Generate task **Robot Framework: Launch Template** into `launch.json` for Robot Framework Language Server.
+
+
 Links
 =====
 
 Code repository:
 
     https://github.com/nazrulworld/collective.recipe.vscode
```

### Comparing `collective.recipe.vscode-0.1.8/setup.py` & `collective.recipe.vscode-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 entry_points = {
     "zc.buildout": ["default = {0}".format(entry_point)],
     "zc.buildout.uninstall": ["default = {0}".format(uninstall_entry_point)],
 }
 
 setup(
     name="collective.recipe.vscode",
-    version="0.1.8",
+    version="0.1.9",
     description="Visual Studio Code configuration for buildout-based Python projects",
     long_description=long_description,
     # Get more from https://pypi.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 4 - Beta",
         "Framework :: Plone",
@@ -45,14 +45,16 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="python buildout plone vscode jedi sublimelinter buildout-recipe anaconda",
     author="Md Nazrul Islam",
     author_email="email2nazrul@gmail.com",
```

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/recipes.py` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/recipes.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,54 @@
 json_load_params = {}
 
 python_file_defaults = {
     "files.associations": {"*.zcml": "xml"},
     "files.exclude": {"**/*.py[co]": True, "**/*.so": True, "**/__pycache__": True},
 }
 
+ROBOT_LSP_LAUNCH_TEMPLATE = lambda pythonpath: {  # noqa: E731
+    "type": "robotframework-lsp",
+    "name": "Robot Framework: Launch Template",
+    "request": "launch",
+    "cwd": "^\"\\${workspaceFolder}\"",
+    "target": "^\"\\${file}\"",
+    "terminal": "integrated",
+    "env": {
+        "LISTENER_HOST": "localhost",
+        "LISTENER_PORT": 49999,
+        "PYTHONPATH": pythonpath,
+    },
+    "args": [
+        "--variable",
+        "ZOPE_HOST:localhost",
+        "--variable",
+        "ZOPE_port:55001",
+        "--listener",
+        "plone.app.robotframework.server.RobotListener",
+    ]
+}
+
+ROBOT_SERVER_TASK_TEMPLATE = {
+    "label": "Start Plone Test Server",
+    "type": "shell",
+    "command": "ZSERVER_PORT=55001 bin/robot-server ${input:ploneTestingLayer} --no-reload -vv",  # noqa: E501
+    "presentation": {
+      "reveal": "always",
+      "panel": "shared",
+    },
+    "problemMatcher": [],
+}
+
+ROBOT_SERVER_INPUT_TEMPLATE = {
+    "id": "ploneTestingLayer",
+    "type": "promptString",
+    "description": "Enter Plone Testing Fixture",
+    "default": "Products.CMFPlone.testing.PRODUCTS_CMFPLONE_ROBOT_TESTING"
+}
+
 
 def ensure_unicode(string):
     """" """
     u_string = string
     if isinstance(u_string, bytes):
         u_string = u_string.decode("utf-8", "strict")
 
@@ -91,15 +131,15 @@
 
         # Make all other recipes dependent on us so they run first to
         # ensure all implctly
         # referenced parts are loaded
         for part in self.buildout["buildout"].get("parts", "").split():
             self.buildout.get(part)
 
-    def install(self):
+    def install(self):  # noqa: C901
         """Let's build vscode settings file:
         This is the method will be called by buildout it-self and this recipe
         will generate or/update vscode setting file (.vscode/settings.json) based
         on provided options.
         """
 
         if self.options.get("eggs"):
@@ -168,14 +208,61 @@
         vs_generated_file = os.path.join(
             self.settings_dir, "vs-recipe-generated-settings.json"
         )
         with io.open(vs_generated_file, "w", encoding="utf-8") as fp:
             json_text = json.dumps(vscode_settings, indent=2, sort_keys=True)
             fp.write(ensure_unicode(json_text))
 
+        # Update .vscode/launch.js and .vscode/tasks.js for Robot testing
+        if vscode_settings.get("robot.python.env"):
+            vs_launch_file = os.path.join(self.settings_dir, "launch.json")
+            if os.path.exists(vs_launch_file):
+                with io.open(vs_launch_file, "r", encoding="utf-8") as fp:
+                    launch_json = json.loads(fp.read())
+            else:
+                launch_json = dict(version="0.2.0")
+            launch_json.setdefault("configurations", [])
+            launch_json["configurations"] = [
+                c for c in launch_json["configurations"]
+                if c["type"] != "robotframwork-lsp" and
+                c["name"] != "Robot Framework: Launch Template"
+            ] + [
+                ROBOT_LSP_LAUNCH_TEMPLATE(
+                    vscode_settings["robot.python.env"]["PYTHONPATH"].replace(
+                        '${PYTHONPATH}', '${env:PYTHONPATH}'
+                    )
+                )
+            ]
+            with io.open(vs_launch_file, "w", encoding="utf-8") as fp:
+                fp.write(json.dumps(launch_json, indent=4))
+
+            vs_tasks_file = os.path.join(self.settings_dir, "tasks.json")
+            if os.path.exists(vs_tasks_file):
+                with io.open(vs_tasks_file, "r", encoding="utf-8") as fp:
+                    tasks_json = json.loads(fp.read())
+            else:
+                tasks_json = dict(version="2.0.0")
+            tasks_json.setdefault("tasks", [])
+            tasks_json.setdefault("inputs", [])
+            tasks_json["tasks"] = [
+                t for t in tasks_json["tasks"]
+                if t["type"] != "shell" and
+                t["name"] != "Plone: Start Test Server"
+            ] + [
+                ROBOT_SERVER_TASK_TEMPLATE
+            ]
+            tasks_json["inputs"] = [
+                i for i in tasks_json["inputs"]
+                if i["id"] != "ploneTestingLayer"
+            ] + [
+                ROBOT_SERVER_INPUT_TEMPLATE
+            ]
+            with io.open(vs_tasks_file, "w", encoding="utf-8") as fp:
+                fp.write(json.dumps(tasks_json, indent=4))
+
         return vs_generated_file
 
     update = install
 
     def normalize_options(self):
         """This method is simply doing tranformation of cfg string to python datatype.
         For example: yes(cfg) = True(python), 2(cfg) = 2(python)"""
@@ -202,14 +289,17 @@
 
         # pep8 check: Issue#1
         self._normalize_boolean("pep8-enabled", options)
 
         # generate .env file
         self._normalize_boolean("generate-envfile", options)
 
+        # robotframework lsp pythonpath
+        self._normalize_boolean("robot-enabled", options)
+
         # autocomplete
         options["autocomplete-use-omelette"] = self.options[
             "autocomplete-use-omelette"
         ].lower() in ("yes", "y", "true", "t", "on", "1", "sure")
 
         # Parse linter arguments
         if "pylint-args" in options:
@@ -296,14 +386,15 @@
         self.options.setdefault("black-args", "")
         self.options.setdefault("formatting-provider", "")
         self.options.setdefault("autocomplete-use-omelette", "False")
         self.options.setdefault("ignore-develop", "False")
         self.options.setdefault("ignores", "")
         self.options.setdefault("packages", "")
         self.options.setdefault("generate-envfile", "True")
+        self.options.setdefault("robot-enabled", "False")
 
     def _prepare_settings(
         self, eggs_locations, develop_eggs_locations, existing_settings
     ):
         """ """
         options = self.normalize_options()
         settings = dict()
@@ -336,14 +427,18 @@
             ] + develop_eggs_locations
 
         # Needed for pylance
         settings[mappings["analysis-extrapaths"]] = settings[
             mappings["autocomplete-extrapaths"]
         ]
 
+        # Needed for robotframework-slp
+        if "robot-enabled" in self.user_options and options["robot-enabled"]:
+            settings[mappings["robot-python-env"]] = dict(PYTHONPATH=pythonpath)
+
         # Look on Jedi
         if "jedi-enabled" in self.user_options and options["jedi-enabled"]:
             # TODO: not even sure jediEnabled setting is supported anymore
             # settings[mappings["jedi-enabled"]] = options["jedi-enabled"]
             settings[mappings["languageserver"]] = "Jedi"
             # VS code no longer supports this settings
             # settings[mappings["completionsenabled"]] = False
```

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/recipes.rst` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/recipes.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/settings_mappings.json` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/settings_mappings.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'robot-python-env'": "'robot.python.env'"}*

```diff
@@ -17,11 +17,12 @@
     "pep8-args": "python.linting.pep8Args",
     "pep8-enabled": "python.linting.pep8Enabled",
     "pep8-path": "python.linting.pep8Path",
     "pylint-args": "python.linting.pylintArgs",
     "pylint-enabled": "python.linting.pylintEnabled",
     "pylint-path": "python.linting.pylintPath",
     "python-path": "python.pythonPath",
+    "robot-python-env": "robot.python.env",
     "rst-linter-args": "restructuredtext.linter.extraArgs",
     "rst-linter-enabled": "restructuredtext.linter.run",
     "rst-linter-path": "restructuredtext.linter.executablePath"
 }
```

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/.gitignore` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/.gitignore`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/LICENSE` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/LICENSE`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/README.rst` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/setup.py` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/develop/vscodetest_pkg1/setup.py`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/test_docs.py` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective/recipe/vscode/tests/test_recipes.py` & `collective.recipe.vscode-0.1.9/src/collective/recipe/vscode/tests/test_recipes.py`

 * *Files identical despite different names*

### Comparing `collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/PKG-INFO` & `collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: collective.recipe.vscode
-Version: 0.1.8
+Version: 0.1.9
 Summary: Visual Studio Code configuration for buildout-based Python projects
 Home-page: https://github.com/nazrulworld/collective.recipe.vscode
 Author: Md Nazrul Islam
 Author-email: email2nazrul@gmail.com
 License: GPL version 2
 Description: .. image:: https://img.shields.io/pypi/status/collective.recipe.vscode.svg
             :target: https://pypi.org/project/collective.recipe.vscode/
             :alt: Package Status
         
-        .. image:: https://travis-ci.org/nazrulworld/collective.recipe.vscode.svg?branch=master
-            :target: https://travis-ci.org/nazrulworld/collective.recipe.vscode
+        .. image:: https://app.travis-ci.com/nazrulworld/collective.recipe.vscode.svg?branch=master
+            :target: https://app.travis-ci.com/nazrulworld/collective.recipe.vscode
             :alt: Travis Build Status
         
         .. image:: https://coveralls.io/repos/github/nazrulworld/collective.recipe.vscode/badge.svg?branch=master
             :target: https://coveralls.io/github/nazrulworld/collective.recipe.vscode?branch=master
             :alt: Test Coverage
         .. image:: https://img.shields.io/pypi/pyversions/collective.recipe.vscode.svg
             :target: https://pypi.org/project/collective.recipe.vscode/
@@ -224,14 +224,24 @@
         generate-envfile
             Required: No
         
             Default: True
         
             Generate .env file to add eggs to PYTHONPATH
         
+        robot-enabled
+            Required: No
+        
+            Default: False
+        
+            Generate setting `robot.python.env` with buildout eggs for Robot Framework Language Server.
+            Generate task **Start Plone Test Server** into `tasks.json`.
+            Generate task **Robot Framework: Launch Template** into `launch.json` for Robot Framework Language Server.
+        
+        
         Links
         =====
         
         Code repository:
         
             https://github.com/nazrulworld/collective.recipe.vscode
         
@@ -336,14 +346,21 @@
         - Md Nazrul Islam<email2nazrul@gmail.com>, Original Author.
         - Matteo Parrucci
         
         
         Changelog
         =========
         
+        0.1.9 (2023-06-30)
+        ------------------
+        
+        - Add option `robot-enabled` (default *false*) to enable support for Robot Framework Language Server
+          [datakurre]
+        
+        
         0.1.8 (2021-10-28)
         ------------------
         
         - Change languageserver to Pylance (Microsoft no longer works)
         - Default to generating .env file to aid in debugging
         - Options are removed. ``jedi-path``
         - ``vsintellicode.python.completionsEnabled`` is no longer part of VS code settings.
@@ -429,11 +446,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
```

### Comparing `collective.recipe.vscode-0.1.8/src/collective.recipe.vscode.egg-info/SOURCES.txt` & `collective.recipe.vscode-0.1.9/src/collective.recipe.vscode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

