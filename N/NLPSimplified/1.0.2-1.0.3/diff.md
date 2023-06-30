# Comparing `tmp/NLPSimplified-1.0.2.tar.gz` & `tmp/NLPSimplified-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NLPSimplified-1.0.2.tar", last modified: Fri Jun 30 01:52:40 2023, max compression
+gzip compressed data, was "NLPSimplified-1.0.3.tar", last modified: Fri Jun 30 02:00:20 2023, max compression
```

## Comparing `NLPSimplified-1.0.2.tar` & `NLPSimplified-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:52:40.501903 NLPSimplified-1.0.2/
--rw-rw-rw-   0        0        0     1034 2023-06-30 01:39:25.000000 NLPSimplified-1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-30 01:52:40.495395 NLPSimplified-1.0.2/NLPSimplified/
--rw-rw-rw-   0        0        0       82 2023-06-30 01:49:45.000000 NLPSimplified-1.0.2/NLPSimplified/__init__.py
--rw-rw-rw-   0        0        0      861 2023-06-30 01:49:59.000000 NLPSimplified-1.0.2/NLPSimplified/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:52:40.500902 NLPSimplified-1.0.2/NLPSimplified.egg-info/
--rw-rw-rw-   0        0        0      354 2023-06-30 01:52:40.000000 NLPSimplified-1.0.2/NLPSimplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-30 01:52:40.000000 NLPSimplified-1.0.2/NLPSimplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:52:40.000000 NLPSimplified-1.0.2/NLPSimplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-30 01:52:40.000000 NLPSimplified-1.0.2/NLPSimplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 01:52:40.000000 NLPSimplified-1.0.2/NLPSimplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      354 2023-06-30 01:52:40.501903 NLPSimplified-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2471 2023-06-30 01:50:01.000000 NLPSimplified-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 01:52:40.502904 NLPSimplified-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-30 01:52:36.000000 NLPSimplified-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:00:20.666190 NLPSimplified-1.0.3/
+-rw-rw-rw-   0        0        0     1034 2023-06-30 01:58:51.000000 NLPSimplified-1.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-30 02:00:20.660181 NLPSimplified-1.0.3/NLPSimplified/
+-rw-rw-rw-   0        0        0       82 2023-06-30 01:55:08.000000 NLPSimplified-1.0.3/NLPSimplified/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-06-30 01:58:53.000000 NLPSimplified-1.0.3/NLPSimplified/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:00:20.664687 NLPSimplified-1.0.3/NLPSimplified.egg-info/
+-rw-rw-rw-   0        0        0     2762 2023-06-30 02:00:20.000000 NLPSimplified-1.0.3/NLPSimplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-30 02:00:20.000000 NLPSimplified-1.0.3/NLPSimplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:00:20.000000 NLPSimplified-1.0.3/NLPSimplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-30 02:00:20.000000 NLPSimplified-1.0.3/NLPSimplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 02:00:20.000000 NLPSimplified-1.0.3/NLPSimplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2762 2023-06-30 02:00:20.665687 NLPSimplified-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2419 2023-06-30 01:58:50.000000 NLPSimplified-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:00:20.666190 NLPSimplified-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      433 2023-06-30 02:00:03.000000 NLPSimplified-1.0.3/setup.py
```

### Comparing `NLPSimplified-1.0.2/LICENSE` & `NLPSimplified-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NLPSimplified-1.0.2/NLPSimplified/pipeline.py` & `NLPSimplified-1.0.3/NLPSimplified/pipeline.py`

 * *Files identical despite different names*

### Comparing `NLPSimplified-1.0.2/README.md` & `NLPSimplified-1.0.3/NLPSimplified.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: NLPSimplified
+Version: 1.0.3
+Summary: A simple NLP pipeline using spaCy
+Home-page: UNKNOWN
+Author: Avneh Singh Bhatia
+Author-email: avnehb@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MyPackage
 
 ## MyPackage is a Python package that provides a simple NLP pipeline using spaCy.
 
 # Installation
 
 ## Clone the repository and navigate to the root directory. Then run the following command:
@@ -46,8 +58,9 @@
 ## Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 ## The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 ## **THE SOFTWARE IS PROVIDED “AS IS”, _WITHOUT WARRANTY_ OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.**
 
 # Contact
-## Contact me at avnehb@gmail.com
+## Contact me at avnehb@gmail.com
+
```

