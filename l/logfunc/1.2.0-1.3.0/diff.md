# Comparing `tmp/logfunc-1.2.0.tar.gz` & `tmp/logfunc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.2.0.tar", last modified: Sun Jun 25 17:49:24 2023, max compression
+gzip compressed data, was "logfunc-1.3.0.tar", last modified: Fri Jun 30 07:40:57 2023, max compression
```

## Comparing `logfunc-1.2.0.tar` & `logfunc-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 17:49:24.485170 logfunc-1.2.0/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.2.0/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     3581 2023-06-25 17:49:24.485051 logfunc-1.2.0/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     2716 2023-06-25 17:48:43.000000 logfunc-1.2.0/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 17:49:24.484419 logfunc-1.2.0/logfunc/
--rw-r--r--   0 work       (501) staff       (20)     4245 2023-06-25 17:34:56.000000 logfunc-1.2.0/logfunc/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-25 17:49:24.484883 logfunc-1.2.0/logfunc.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     3581 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      170 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-06-25 17:49:24.000000 logfunc-1.2.0/logfunc.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-06-25 17:49:24.485208 logfunc-1.2.0/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     1121 2023-06-25 17:46:53.000000 logfunc-1.2.0/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 07:40:57.433203 logfunc-1.3.0/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.3.0/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     4091 2023-06-30 07:40:57.433070 logfunc-1.3.0/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     3226 2023-06-30 07:40:13.000000 logfunc-1.3.0/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 07:40:57.432421 logfunc-1.3.0/logfunc/
+-rw-r--r--   0 work       (501) staff       (20)     5521 2023-06-30 07:36:54.000000 logfunc-1.3.0/logfunc/__init__.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 07:40:57.432894 logfunc-1.3.0/logfunc.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     4091 2023-06-30 07:40:57.000000 logfunc-1.3.0/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      170 2023-06-30 07:40:57.000000 logfunc-1.3.0/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-06-30 07:40:57.000000 logfunc-1.3.0/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-06-30 07:40:57.000000 logfunc-1.3.0/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-06-30 07:40:57.433245 logfunc-1.3.0/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)     1121 2023-06-28 16:54:11.000000 logfunc-1.3.0/setup.py
```

### Comparing `logfunc-1.2.0/LICENSE` & `logfunc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.2.0/PKG-INFO` & `logfunc-1.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,10 @@
-Metadata-Version: 2.1
-Name: logfunc
-Version: 1.2.0
-Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
-Home-page: https://github.com/cc-d/logf/tree/main
-Author: Cary Carter
-Author-email: ccarterdev@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # logf
 
-The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
+`@logf()` is a decorator designed to enable effortless and automatic logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
 
 ## Usage
 
 This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
@@ -76,18 +55,29 @@
     max_str_len=None, log_exec_time=True, single_msg=True)
 def my_function(a, b):
     return a + b
 ```
 
 In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time, and it only uses a single log message as opposed to two on enter/exit.
 
+### Environment Variables
+
+The `logf` function supports overriding some default/passed parameters with environment variables:
+
+| Env Var          | Example Values       |
+|------------------|-------------|
+| LOGF_LEVEL       | DEBUG INFO WARNING ERROR CRITICAL 10 20 30 40 50|
+| LOGF_MAX_STR_LEN | 10 50 10000000 None NONE none |
+| LOGF_SINGLE_MSG  | True False
+
+
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
 
 ```sh
 python tests.py
 ```
 
-The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
+The test suite includes tests for the default behavior of the `logf` decorator as well as its behavior when custom parameters are passed. The tests check whether the function name, arguments, return value, and execution time are correctly logged, and whether the `max_str_len` parameter correctly truncates the logged strings.
```

### Comparing `logfunc-1.2.0/logfunc.egg-info/PKG-INFO` & `logfunc-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.2.0
+Version: 1.3.0
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logf
 
-The `@logf()` decorator, previously a part of the myfuncs pip package, is now a standalone pip package. This repository is dedicated to its development and maintenance.
+`@logf()` is a decorator designed to enable effortless and automatic logging of your Python functions' execution, requiring zero configuration for basic usage. Formerly a part of the myfuncs pip package, it is now a standalone pip package. This repository is dedicated to its continued development and maintenance.
 
 ## Usage
 
 This is a brief guide on how to use the `logfunc` module.
 
 ### Installation
 
@@ -76,14 +76,25 @@
     max_str_len=None, log_exec_time=True, single_msg=True)
 def my_function(a, b):
     return a + b
 ```
 
 In this example, the function logs at the 'INFO' level, it doesn't log the function arguments, it logs the return value, logs the entire return string without any truncation, and it measures and logs the execution time, and it only uses a single log message as opposed to two on enter/exit.
 
+### Environment Variables
+
+The `logf` function supports overriding some default/passed parameters with environment variables:
+
+| Env Var          | Example Values       |
+|------------------|-------------|
+| LOGF_LEVEL       | DEBUG INFO WARNING ERROR CRITICAL 10 20 30 40 50|
+| LOGF_MAX_STR_LEN | 10 50 10000000 None NONE none |
+| LOGF_SINGLE_MSG  | True False
+
+
 ## Testing
 
 This module comes with a test suite which you can run to ensure that `logf` behaves as expected. The tests are implemented using Python's built-in `unittest` module.
 
 To run the tests, navigate to the directory where the `logfunc` package is installed and run:
 
 ```sh
```

### Comparing `logfunc-1.2.0/setup.py` & `logfunc-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='1.2.0',
+    version='1.3.0',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

