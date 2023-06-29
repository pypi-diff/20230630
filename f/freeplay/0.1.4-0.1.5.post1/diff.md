# Comparing `tmp/freeplay-0.1.4.tar.gz` & `tmp/freeplay-0.1.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.4.tar", max compression
+gzip compressed data, was "freeplay-0.1.5.post1.tar", max compression
```

## Comparing `freeplay-0.1.4.tar` & `freeplay-0.1.5.post1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.1.4/README.md
--rw-r--r--   0        0        0       62 2023-05-30 19:38:09.617870 freeplay-0.1.4/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.1.4/freeplay/api_support.py
--rw-r--r--   0        0        0      188 2023-06-15 15:26:56.089064 freeplay-0.1.4/freeplay/errors.py
--rw-r--r--   0        0        0     3107 2023-06-21 16:31:59.846196 freeplay-0.1.4/freeplay/freeplay.py
--rw-r--r--   0        0        0    19252 2023-06-22 20:50:42.558516 freeplay-0.1.4/freeplay/freeplay_encapsulated.py
--rw-r--r--   0        0        0      391 2023-06-22 20:46:25.284996 freeplay-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.1.5.post1/README.md
+-rw-r--r--   0        0        0       61 2023-06-28 22:11:30.981007 freeplay-0.1.5.post1/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.1.5.post1/freeplay/api_support.py
+-rw-r--r--   0        0        0      553 2023-06-29 23:02:37.695249 freeplay-0.1.5.post1/freeplay/completions.py
+-rw-r--r--   0        0        0      188 2023-06-15 15:26:56.089064 freeplay-0.1.5.post1/freeplay/errors.py
+-rw-r--r--   0        0        0     8414 2023-06-29 23:02:37.695694 freeplay-0.1.5.post1/freeplay/flavors.py
+-rw-r--r--   0        0        0    17759 2023-06-29 23:02:37.696236 freeplay-0.1.5.post1/freeplay/freeplay.py
+-rw-r--r--   0        0        0      828 2023-06-27 23:41:00.518463 freeplay-0.1.5.post1/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      393 2023-06-29 23:06:34.925049 freeplay-0.1.5.post1/pyproject.toml
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 freeplay-0.1.5.post1/PKG-INFO
```

### Comparing `freeplay-0.1.4/freeplay/api_support.py` & `freeplay-0.1.5.post1/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.4/PKG-INFO` & `freeplay-0.1.5.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.4
+Version: 0.1.5.post1
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

