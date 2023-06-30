# Comparing `tmp/logfunc-1.4.0.tar.gz` & `tmp/logfunc-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.4.0.tar", last modified: Fri Jun 30 14:53:54 2023, max compression
+gzip compressed data, was "logfunc-1.4.1.tar", last modified: Fri Jun 30 15:02:21 2023, max compression
```

## Comparing `logfunc-1.4.0.tar` & `logfunc-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 14:53:54.920076 logfunc-1.4.0/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.4.0/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     4091 2023-06-30 14:53:54.919973 logfunc-1.4.0/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     3226 2023-06-30 07:40:13.000000 logfunc-1.4.0/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 14:53:54.919459 logfunc-1.4.0/logfunc/
--rw-r--r--   0 work       (501) staff       (20)     5659 2023-06-30 14:51:50.000000 logfunc-1.4.0/logfunc/__init__.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 14:53:54.919846 logfunc-1.4.0/logfunc.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     4091 2023-06-30 14:53:54.000000 logfunc-1.4.0/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      170 2023-06-30 14:53:54.000000 logfunc-1.4.0/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-06-30 14:53:54.000000 logfunc-1.4.0/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-06-30 14:53:54.000000 logfunc-1.4.0/logfunc.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-06-30 14:53:54.920110 logfunc-1.4.0/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)     1121 2023-06-30 14:52:10.000000 logfunc-1.4.0/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 15:02:21.476024 logfunc-1.4.1/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-06-23 16:56:28.000000 logfunc-1.4.1/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     4191 2023-06-30 15:02:21.475919 logfunc-1.4.1/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     3226 2023-06-30 07:40:13.000000 logfunc-1.4.1/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 15:02:21.475247 logfunc-1.4.1/logfunc/
+-rw-r--r--   0 work       (501) staff       (20)     5659 2023-06-30 14:51:50.000000 logfunc-1.4.1/logfunc/__init__.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-06-30 15:02:21.475758 logfunc-1.4.1/logfunc.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     4191 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      170 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-06-30 15:02:21.000000 logfunc-1.4.1/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-06-30 15:02:21.476057 logfunc-1.4.1/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)     1219 2023-06-30 15:01:49.000000 logfunc-1.4.1/setup.py
```

### Comparing `logfunc-1.4.0/LICENSE` & `logfunc-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.4.0/PKG-INFO` & `logfunc-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.4.0
+Version: 1.4.1
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `logfunc-1.4.0/README.md` & `logfunc-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `logfunc-1.4.0/logfunc/__init__.py` & `logfunc-1.4.1/logfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `logfunc-1.4.0/logfunc.egg-info/PKG-INFO` & `logfunc-1.4.1/logfunc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.4.0
+Version: 1.4.1
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `logfunc-1.4.0/setup.py` & `logfunc-1.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='1.4.0',
+    version='1.4.1',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -17,14 +17,16 @@
     license='MIT',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
```

