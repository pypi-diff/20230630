# Comparing `tmp/distans-0.1.3.tar.gz` & `tmp/distans-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distans-0.1.3.tar", max compression
+gzip compressed data, was "distans-0.1.4.tar", max compression
```

## Comparing `distans-0.1.3.tar` & `distans-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-30 14:34:23.009677 distans-0.1.3/LICENSE
--rw-r--r--   0        0        0      359 2023-06-30 17:58:38.555962 distans-0.1.3/README.md
--rw-r--r--   0        0        0      152 2023-06-30 17:56:02.141679 distans-0.1.3/distans/__init__.py
--rw-r--r--   0        0        0     1300 2023-06-30 17:06:57.109496 distans-0.1.3/distans/edit.py
--rw-r--r--   0        0        0      688 2023-06-30 17:06:57.120912 distans-0.1.3/distans/lp_space.py
--rw-r--r--   0        0        0        0 2023-06-30 17:16:03.035768 distans-0.1.3/distans/py.typed
--rw-r--r--   0        0        0      708 2023-06-30 18:05:54.391037 distans-0.1.3/distans/stuff.py
--rw-r--r--   0        0        0      663 2023-06-30 18:14:35.000835 distans-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 distans-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 14:34:23.009677 distans-0.1.4/LICENSE
+-rw-r--r--   0        0        0      359 2023-06-30 21:00:24.269847 distans-0.1.4/README.md
+-rw-r--r--   0        0        0      152 2023-06-30 17:56:02.141679 distans-0.1.4/distans/__init__.py
+-rw-r--r--   0        0        0     1300 2023-06-30 20:54:09.407104 distans-0.1.4/distans/edit.py
+-rw-r--r--   0        0        0      789 2023-06-30 20:55:04.988227 distans-0.1.4/distans/lp_space.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:16:03.035768 distans-0.1.4/distans/py.typed
+-rw-r--r--   0        0        0      690 2023-06-30 20:53:46.922029 distans-0.1.4/distans/stuff.py
+-rw-r--r--   0        0        0      180 2023-06-30 20:58:19.234014 distans-0.1.4/distans/utils.py
+-rw-r--r--   0        0        0      663 2023-06-30 20:59:02.568907 distans-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 distans-0.1.4/PKG-INFO
```

### Comparing `distans-0.1.3/LICENSE` & `distans-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `distans-0.1.3/distans/edit.py` & `distans-0.1.4/distans/edit.py`

 * *Files identical despite different names*

### Comparing `distans-0.1.3/pyproject.toml` & `distans-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "distans"
-version = "0.1.3"
+version = "0.1.4"
 repository = "https://github.com/cospectrum/distans"
 description = "Different distances for Python"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `distans-0.1.3/PKG-INFO` & `distans-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distans
-Version: 0.1.3
+Version: 0.1.4
 Summary: Different distances for Python
 Home-page: https://github.com/cospectrum/distans
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,15 +32,15 @@
 
 ```py
 from distans import lp
 
 a = [1, -2, 3]
 b = [3, 4, -5]
 
-p = 4
+p = 2
 norm = lp(a, p=p)
 dist = lp(a, b, p=p)
 ```
 
 ### Edit similarity
 
 ```py
```

