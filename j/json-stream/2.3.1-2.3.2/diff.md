# Comparing `tmp/json-stream-2.3.1.tar.gz` & `tmp/json-stream-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-stream-2.3.1.tar", last modified: Wed Jun 14 22:50:05 2023, max compression
+gzip compressed data, was "json-stream-2.3.2.tar", last modified: Fri Jun 30 09:43:07 2023, max compression
```

## Comparing `json-stream-2.3.1.tar` & `json-stream-2.3.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.467652 json-stream-2.3.1/
--rw-r--r--   0 jamie      (501) staff       (20)     1058 2022-08-06 08:09:13.000000 json-stream-2.3.1/LICENSE.txt
--rw-r--r--   0 jamie      (501) staff       (20)    23960 2023-06-14 22:50:05.467490 json-stream-2.3.1/PKG-INFO
--rw-r--r--   0 jamie      (501) staff       (20)    21632 2023-06-13 15:55:51.000000 json-stream-2.3.1/README.md
--rw-r--r--   0 jamie      (501) staff       (20)     1452 2023-06-13 16:26:36.000000 json-stream-2.3.1/pyproject.toml
--rw-r--r--   0 jamie      (501) staff       (20)       38 2023-06-14 22:50:05.467689 json-stream-2.3.1/setup.cfg
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.460083 json-stream-2.3.1/src/
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.463400 json-stream-2.3.1/src/json_stream/
--rw-r--r--   0 jamie      (501) staff       (20)      227 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     8908 2023-06-13 16:29:22.000000 json-stream-2.3.1/src/json_stream/base.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464447 json-stream-2.3.1/src/json_stream/dump/
--rw-r--r--   0 jamie      (501) staff       (20)      569 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/dump/__init__.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464774 json-stream-2.3.1/src/json_stream/dump/tests/
--rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/dump/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     1533 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/dump/tests/test_dump.py
--rw-r--r--   0 jamie      (501) staff       (20)     1476 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/dump/threading.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464950 json-stream-2.3.1/src/json_stream/httpx/
--rw-r--r--   0 jamie      (501) staff       (20)      602 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/httpx/__init__.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.465306 json-stream-2.3.1/src/json_stream/httpx/tests/
--rw-r--r--   0 jamie      (501) staff       (20)        0 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/httpx/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     1876 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/httpx/tests/test_httpx.py
--rw-r--r--   0 jamie      (501) staff       (20)      728 2023-06-07 13:57:08.000000 json-stream-2.3.1/src/json_stream/iterators.py
--rw-r--r--   0 jamie      (501) staff       (20)      483 2023-06-13 16:29:22.000000 json-stream-2.3.1/src/json_stream/loader.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.465560 json-stream-2.3.1/src/json_stream/requests/
--rw-r--r--   0 jamie      (501) staff       (20)      604 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/requests/__init__.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.465803 json-stream-2.3.1/src/json_stream/requests/tests/
--rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/requests/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)     1940 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/requests/tests/test_requests.py
--rw-r--r--   0 jamie      (501) staff       (20)      387 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/select_tokenizer.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.467275 json-stream-2.3.1/src/json_stream/tests/
--rw-r--r--   0 jamie      (501) staff       (20)     3053 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/tests/__init__.py
--rw-r--r--   0 jamie      (501) staff       (20)      500 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/tests/test_iterators.py
--rw-r--r--   0 jamie      (501) staff       (20)    10284 2023-06-13 15:56:01.000000 json-stream-2.3.1/src/json_stream/tests/test_loader.py
--rw-r--r--   0 jamie      (501) staff       (20)    10353 2023-06-14 22:48:01.000000 json-stream-2.3.1/src/json_stream/tests/test_tokenizer.py
--rw-r--r--   0 jamie      (501) staff       (20)     1454 2023-03-17 22:41:52.000000 json-stream-2.3.1/src/json_stream/tests/test_tokenizer_integration.py
--rw-r--r--   0 jamie      (501) staff       (20)      440 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/tests/test_util.py
--rw-r--r--   0 jamie      (501) staff       (20)      884 2022-08-06 08:09:13.000000 json-stream-2.3.1/src/json_stream/tests/test_visitor.py
--rw-r--r--   0 jamie      (501) staff       (20)     1132 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/tests/test_writer.py
--rw-r--r--   0 jamie      (501) staff       (20)    14198 2023-06-14 22:48:01.000000 json-stream-2.3.1/src/json_stream/tokenizer.py
--rw-r--r--   0 jamie      (501) staff       (20)     2071 2023-02-21 10:49:10.000000 json-stream-2.3.1/src/json_stream/util.py
--rw-r--r--   0 jamie      (501) staff       (20)      902 2023-06-13 16:29:22.000000 json-stream-2.3.1/src/json_stream/visitor.py
--rw-r--r--   0 jamie      (501) staff       (20)     1775 2023-02-11 10:45:16.000000 json-stream-2.3.1/src/json_stream/writer.py
-drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-14 22:50:05.464154 json-stream-2.3.1/src/json_stream.egg-info/
--rw-r--r--   0 jamie      (501) staff       (20)    23960 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/PKG-INFO
--rw-r--r--   0 jamie      (501) staff       (20)     1182 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/SOURCES.txt
--rw-r--r--   0 jamie      (501) staff       (20)        1 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/dependency_links.txt
--rw-r--r--   0 jamie      (501) staff       (20)       69 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/requires.txt
--rw-r--r--   0 jamie      (501) staff       (20)       12 2023-06-14 22:50:05.000000 json-stream-2.3.1/src/json_stream.egg-info/top_level.txt
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.023471 json-stream-2.3.2/
+-rw-r--r--   0 jamie      (501) staff       (20)     1058 2022-08-06 08:09:13.000000 json-stream-2.3.2/LICENSE.txt
+-rw-r--r--   0 jamie      (501) staff       (20)    23960 2023-06-30 09:43:07.023310 json-stream-2.3.2/PKG-INFO
+-rw-r--r--   0 jamie      (501) staff       (20)    21632 2023-06-13 15:55:51.000000 json-stream-2.3.2/README.md
+-rw-r--r--   0 jamie      (501) staff       (20)     1452 2023-06-30 09:41:12.000000 json-stream-2.3.2/pyproject.toml
+-rw-r--r--   0 jamie      (501) staff       (20)       38 2023-06-30 09:43:07.023511 json-stream-2.3.2/setup.cfg
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.015534 json-stream-2.3.2/src/
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.018933 json-stream-2.3.2/src/json_stream/
+-rw-r--r--   0 jamie      (501) staff       (20)      227 2023-02-21 10:49:10.000000 json-stream-2.3.2/src/json_stream/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     8908 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/base.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.020018 json-stream-2.3.2/src/json_stream/dump/
+-rw-r--r--   0 jamie      (501) staff       (20)      569 2023-02-21 10:49:10.000000 json-stream-2.3.2/src/json_stream/dump/__init__.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.020366 json-stream-2.3.2/src/json_stream/dump/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.2/src/json_stream/dump/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1533 2023-02-21 10:49:10.000000 json-stream-2.3.2/src/json_stream/dump/tests/test_dump.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1476 2022-08-06 08:09:13.000000 json-stream-2.3.2/src/json_stream/dump/threading.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.020564 json-stream-2.3.2/src/json_stream/httpx/
+-rw-r--r--   0 jamie      (501) staff       (20)      602 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/httpx/__init__.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.020912 json-stream-2.3.2/src/json_stream/httpx/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)        0 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/httpx/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1876 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/httpx/tests/test_httpx.py
+-rw-r--r--   0 jamie      (501) staff       (20)      709 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/iterators.py
+-rw-r--r--   0 jamie      (501) staff       (20)      483 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/loader.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.021100 json-stream-2.3.2/src/json_stream/requests/
+-rw-r--r--   0 jamie      (501) staff       (20)      604 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/requests/__init__.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.021341 json-stream-2.3.2/src/json_stream/requests/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)        0 2022-08-06 08:09:13.000000 json-stream-2.3.2/src/json_stream/requests/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1940 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/requests/tests/test_requests.py
+-rw-r--r--   0 jamie      (501) staff       (20)      387 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/select_tokenizer.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.023104 json-stream-2.3.2/src/json_stream/tests/
+-rw-r--r--   0 jamie      (501) staff       (20)     3053 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/tests/__init__.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1479 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/tests/test_buffering.py
+-rw-r--r--   0 jamie      (501) staff       (20)      500 2023-06-29 14:51:56.000000 json-stream-2.3.2/src/json_stream/tests/test_iterators.py
+-rw-r--r--   0 jamie      (501) staff       (20)    10284 2023-06-13 15:56:01.000000 json-stream-2.3.2/src/json_stream/tests/test_loader.py
+-rw-r--r--   0 jamie      (501) staff       (20)    10353 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/tests/test_tokenizer.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1454 2023-03-17 22:41:52.000000 json-stream-2.3.2/src/json_stream/tests/test_tokenizer_integration.py
+-rw-r--r--   0 jamie      (501) staff       (20)      440 2023-02-21 10:49:10.000000 json-stream-2.3.2/src/json_stream/tests/test_util.py
+-rw-r--r--   0 jamie      (501) staff       (20)      884 2022-08-06 08:09:13.000000 json-stream-2.3.2/src/json_stream/tests/test_visitor.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1132 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/tests/test_writer.py
+-rw-r--r--   0 jamie      (501) staff       (20)    14198 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/tokenizer.py
+-rw-r--r--   0 jamie      (501) staff       (20)     2071 2023-02-21 10:49:10.000000 json-stream-2.3.2/src/json_stream/util.py
+-rw-r--r--   0 jamie      (501) staff       (20)      902 2023-06-30 09:41:12.000000 json-stream-2.3.2/src/json_stream/visitor.py
+-rw-r--r--   0 jamie      (501) staff       (20)     1775 2023-02-11 10:45:16.000000 json-stream-2.3.2/src/json_stream/writer.py
+drwxr-xr-x   0 jamie      (501) staff       (20)        0 2023-06-30 09:43:07.019731 json-stream-2.3.2/src/json_stream.egg-info/
+-rw-r--r--   0 jamie      (501) staff       (20)    23960 2023-06-30 09:43:07.000000 json-stream-2.3.2/src/json_stream.egg-info/PKG-INFO
+-rw-r--r--   0 jamie      (501) staff       (20)     1222 2023-06-30 09:43:07.000000 json-stream-2.3.2/src/json_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 jamie      (501) staff       (20)        1 2023-06-30 09:43:07.000000 json-stream-2.3.2/src/json_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 jamie      (501) staff       (20)       69 2023-06-30 09:43:07.000000 json-stream-2.3.2/src/json_stream.egg-info/requires.txt
+-rw-r--r--   0 jamie      (501) staff       (20)       12 2023-06-30 09:43:07.000000 json-stream-2.3.2/src/json_stream.egg-info/top_level.txt
```

### Comparing `json-stream-2.3.1/LICENSE.txt` & `json-stream-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/PKG-INFO` & `json-stream-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream
-Version: 2.3.1
+Version: 2.3.2
 Summary: Streaming JSON encoder and decoder
 Author-email: Jamie Cockburn <jamie_cockburn@hotmail.co.uk>
 License: Copyright (c) 2020 Jamie Cockburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `json-stream-2.3.1/README.md` & `json-stream-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/pyproject.toml` & `json-stream-2.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "json-stream"
-version = "2.3.1"
+version = "2.3.2"
 authors = [
     {name = "Jamie Cockburn", email="jamie_cockburn@hotmail.co.uk"},
 ]
 license = {file = "LICENSE.txt"}
 description = "Streaming JSON encoder and decoder"
 keywords = ["json", "stream", "decoder", "encoder", "parsing"]
 classifiers = [
```

### Comparing `json-stream-2.3.1/src/json_stream/base.py` & `json-stream-2.3.2/src/json_stream/base.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/dump/__init__.py` & `json-stream-2.3.2/src/json_stream/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/dump/tests/test_dump.py` & `json-stream-2.3.2/src/json_stream/dump/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/dump/threading.py` & `json-stream-2.3.2/src/json_stream/dump/threading.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/httpx/__init__.py` & `json-stream-2.3.2/src/json_stream/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/httpx/tests/test_httpx.py` & `json-stream-2.3.2/src/json_stream/httpx/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/requests/__init__.py` & `json-stream-2.3.2/src/json_stream/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/requests/tests/test_requests.py` & `json-stream-2.3.2/src/json_stream/requests/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tests/__init__.py` & `json-stream-2.3.2/src/json_stream/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tests/test_loader.py` & `json-stream-2.3.2/src/json_stream/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tests/test_tokenizer.py` & `json-stream-2.3.2/src/json_stream/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tests/test_tokenizer_integration.py` & `json-stream-2.3.2/src/json_stream/tests/test_tokenizer_integration.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tests/test_visitor.py` & `json-stream-2.3.2/src/json_stream/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tests/test_writer.py` & `json-stream-2.3.2/src/json_stream/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/tokenizer.py` & `json-stream-2.3.2/src/json_stream/tokenizer.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/util.py` & `json-stream-2.3.2/src/json_stream/util.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/visitor.py` & `json-stream-2.3.2/src/json_stream/visitor.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream/writer.py` & `json-stream-2.3.2/src/json_stream/writer.py`

 * *Files identical despite different names*

### Comparing `json-stream-2.3.1/src/json_stream.egg-info/PKG-INFO` & `json-stream-2.3.2/src/json_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-stream
-Version: 2.3.1
+Version: 2.3.2
 Summary: Streaming JSON encoder and decoder
 Author-email: Jamie Cockburn <jamie_cockburn@hotmail.co.uk>
 License: Copyright (c) 2020 Jamie Cockburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `json-stream-2.3.1/src/json_stream.egg-info/SOURCES.txt` & `json-stream-2.3.2/src/json_stream.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/json_stream/httpx/__init__.py
 src/json_stream/httpx/tests/__init__.py
 src/json_stream/httpx/tests/test_httpx.py
 src/json_stream/requests/__init__.py
 src/json_stream/requests/tests/__init__.py
 src/json_stream/requests/tests/test_requests.py
 src/json_stream/tests/__init__.py
+src/json_stream/tests/test_buffering.py
 src/json_stream/tests/test_iterators.py
 src/json_stream/tests/test_loader.py
 src/json_stream/tests/test_tokenizer.py
 src/json_stream/tests/test_tokenizer_integration.py
 src/json_stream/tests/test_util.py
 src/json_stream/tests/test_visitor.py
 src/json_stream/tests/test_writer.py
```

