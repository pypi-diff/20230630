# Comparing `tmp/dataflat-1.0.5.tar.gz` & `tmp/dataflat-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflat-1.0.5.tar", last modified: Thu Jun 29 22:18:06 2023, max compression
+gzip compressed data, was "dataflat-1.0.6.tar", last modified: Thu Jun 29 22:47:35 2023, max compression
```

## Comparing `dataflat-1.0.5.tar` & `dataflat-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-29 22:17:56.000000 dataflat-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:18:06.873386 dataflat-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-29 22:17:56.000000 dataflat-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/dictionary/flattener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/flattener_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/pandas_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/pandas_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/pandas_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/spark_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/spark_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/spark_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:18:06.873386 dataflat-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-29 22:17:56.000000 dataflat-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-29 22:47:25.000000 dataflat-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:47:35.411036 dataflat-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-29 22:47:25.000000 dataflat-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/dictionary/flattener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/flattener_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/pandas_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/pandas_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/pandas_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat/spark_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/spark_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-06-29 22:47:25.000000 dataflat-1.0.6/dataflat/spark_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:47:35.411036 dataflat-1.0.6/dataflat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:47:35.000000 dataflat-1.0.6/dataflat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:47:35.411036 dataflat-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-29 22:47:25.000000 dataflat-1.0.6/setup.py
```

### Comparing `dataflat-1.0.5/LICENSE` & `dataflat-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/PKG-INFO` & `dataflat-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dataflat-1.0.5/README.md` & `dataflat-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/dataflat/commons.py` & `dataflat-1.0.6/dataflat/commons.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/dataflat/dictionary/flattener.py` & `dataflat-1.0.6/dataflat/dictionary/flattener.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/dataflat/exceptions.py` & `dataflat-1.0.6/dataflat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/dataflat/flattener_handler.py` & `dataflat-1.0.6/dataflat/flattener_handler.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/dataflat/pandas_df/flattener.py` & `dataflat-1.0.6/dataflat/pandas_df/flattener.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.5/dataflat/spark_df/flattener.py` & `dataflat-1.0.6/dataflat/spark_df/flattener.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+'''
+spark_df/flattener.py - The processor script for spark dataframes flattening process
+
+Copyright (C) 2023 Juan ROJAS
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+
+Authors:
+    Juan ROJAS <jarojasa97@gmail.com>
+'''
+
 import json
 import re
 from typeguard import typechecked
 from typing import List
 from dataflat.commons import init_logger
 from dataflat.exceptions import FlatteningException
 from pyspark.sql.dataframe import DataFrame
```

### Comparing `dataflat-1.0.5/dataflat.egg-info/PKG-INFO` & `dataflat-1.0.6/dataflat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dataflat-1.0.5/setup.py` & `dataflat-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 PATH = path.abspath(path.dirname(__file__))
 
 with open(path.join(PATH, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
  
 setuptools.setup(
     name="dataflat",
-    version="1.0.5",
+    version="1.0.6",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/JuanARojasA/dataflat',
     author="Juan Rojas",
     author_email="jarojasa97@gmail.com",
     license='Apache License 2.0',
     platforms='any',
```

