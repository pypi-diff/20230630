# Comparing `tmp/sspr.python.by.designermadsen-0.0.5.tar.gz` & `tmp/sspr.python.by.designermadsen-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspr.python.by.designermadsen-0.0.5.tar", last modified: Thu Jun 29 00:46:03 2023, max compression
+gzip compressed data, was "sspr.python.by.designermadsen-0.0.6.dev0.tar", last modified: Fri Jun 30 09:02:16 2023, max compression
```

## Comparing `sspr.python.by.designermadsen-0.0.5.tar` & `sspr.python.by.designermadsen-0.0.6.dev0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:46:03.120436 sspr.python.by.designermadsen-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 00:45:51.000000 sspr.python.by.designermadsen-0.0.5/License.md
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-29 00:46:03.120436 sspr.python.by.designermadsen-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-29 00:45:51.000000 sspr.python.by.designermadsen-0.0.5/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:46:03.120436 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:46:03.120436 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-29 00:46:03.000000 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 00:46:03.000000 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:46:03.000000 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 00:46:03.000000 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:46:03.000000 sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-29 00:45:51.000000 sspr.python.by.designermadsen-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 00:46:03.120436 sspr.python.by.designermadsen-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:46:03.120436 sspr.python.by.designermadsen-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 00:45:51.000000 sspr.python.by.designermadsen-0.0.5/tests/test_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:02:16.612727 sspr.python.by.designermadsen-0.0.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 09:02:05.000000 sspr.python.by.designermadsen-0.0.6.dev0/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-30 09:02:16.612727 sspr.python.by.designermadsen-0.0.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-30 09:02:05.000000 sspr.python.by.designermadsen-0.0.6.dev0/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:02:16.612727 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:02:16.612727 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-30 09:02:16.000000 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-30 09:02:16.000000 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:02:16.000000 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 09:02:16.000000 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:02:16.000000 sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 09:02:05.000000 sspr.python.by.designermadsen-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 09:02:16.612727 sspr.python.by.designermadsen-0.0.6.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:02:16.612727 sspr.python.by.designermadsen-0.0.6.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 09:02:05.000000 sspr.python.by.designermadsen-0.0.6.dev0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-30 09:02:05.000000 sspr.python.by.designermadsen-0.0.6.dev0/tests/test_tokens.py
```

### Comparing `sspr.python.by.designermadsen-0.0.5/License.md` & `sspr.python.by.designermadsen-0.0.6.dev0/License.md`

 * *Files identical despite different names*

### Comparing `sspr.python.by.designermadsen-0.0.5/PKG-INFO` & `sspr.python.by.designermadsen-0.0.6.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspr.python.by.designermadsen
-Version: 0.0.5
+Version: 0.0.6.dev0
 Summary: a revised school project that i have programmed in python instead of C#.
 Author-email: Kent vejrup Madsen <Kent.vejrup.Madsen@outlook.com>
 License: # MIT License
         
         Copyright (c) 2023 Kent Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,18 +46,28 @@
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Specialised Study Project - Revised
+## Description
+To install the project:
+
+    pip install sspr.python.by.designermadsen
+
+
 ## Build status
+### Python
 [![Python application](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python.yml)
+[![Python package](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python-matrice.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python-matrice.yml)
+[![Upload Python Package](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/publish.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/publish.yml)
 
-    pip install sspr.python.by.designermadsen
+### Packages
+[![Dependency Review](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/rependencies.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/rependencies.yml)
 
 ## Summary
 Old project that I decided to rewrite in Python. 
 The project was originally written is C# and can be found at a previous account I had on 
 [Github](https://github.com/KentMadsen/Rybners-SpecialisedStudyProject). 
 Which I Since been locked out of.
```

### Comparing `sspr.python.by.designermadsen-0.0.5/Readme.md` & `sspr.python.by.designermadsen-0.0.6.dev0/Readme.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # Specialised Study Project - Revised
+## Description
+To install the project:
+
+    pip install sspr.python.by.designermadsen
+
+
 ## Build status
+### Python
 [![Python application](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python.yml)
+[![Python package](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python-matrice.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python-matrice.yml)
+[![Upload Python Package](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/publish.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/publish.yml)
 
-    pip install sspr.python.by.designermadsen
+### Packages
+[![Dependency Review](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/rependencies.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/rependencies.yml)
 
 ## Summary
 Old project that I decided to rewrite in Python. 
 The project was originally written is C# and can be found at a previous account I had on 
 [Github](https://github.com/KentMadsen/Rybners-SpecialisedStudyProject). 
 Which I Since been locked out of.
```

### Comparing `sspr.python.by.designermadsen-0.0.5/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/PKG-INFO` & `sspr.python.by.designermadsen-0.0.6.dev0/SpecialisedStudyProject/sspr.python.by.designermadsen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspr.python.by.designermadsen
-Version: 0.0.5
+Version: 0.0.6.dev0
 Summary: a revised school project that i have programmed in python instead of C#.
 Author-email: Kent vejrup Madsen <Kent.vejrup.Madsen@outlook.com>
 License: # MIT License
         
         Copyright (c) 2023 Kent Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,18 +46,28 @@
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Specialised Study Project - Revised
+## Description
+To install the project:
+
+    pip install sspr.python.by.designermadsen
+
+
 ## Build status
+### Python
 [![Python application](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python.yml)
+[![Python package](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python-matrice.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/python-matrice.yml)
+[![Upload Python Package](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/publish.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/publish.yml)
 
-    pip install sspr.python.by.designermadsen
+### Packages
+[![Dependency Review](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/rependencies.yml/badge.svg)](https://github.com/KentVejrupMadsen/specialised-study-project.revised.python/actions/workflows/rependencies.yml)
 
 ## Summary
 Old project that I decided to rewrite in Python. 
 The project was originally written is C# and can be found at a previous account I had on 
 [Github](https://github.com/KentMadsen/Rybners-SpecialisedStudyProject). 
 Which I Since been locked out of.
```

### Comparing `sspr.python.by.designermadsen-0.0.5/pyproject.toml` & `sspr.python.by.designermadsen-0.0.6.dev0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sspr.python.by.designermadsen"
-version = "0.0.5"
+version = "0.0.6-dev"
 authors = [
   { name="Kent vejrup Madsen", email="Kent.vejrup.Madsen@outlook.com" },
 ]
 
 readme = { file="Readme.md", content-type="text/markdown" }
 license = { file="License.md", content-type="text/markdown" }
 
@@ -67,8 +67,8 @@
 "Contact" = "https://about.designermadsen.dk"
 "on Github" = "https://github.com/KentVejrupMadsen"
 "On PyPi" = "https://pypi.org/project/sspr.python.by.designermadsen/"
 
 [tool.setuptools.packages.find]
 where = ["SpecialisedStudyProject"]
 include = ["SpecialisedStudyProject.*"]
-exclude = ["tests.*"]
+exclude = ["SpecialisedStudyProject.tests.*"]
```

