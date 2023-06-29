# Comparing `tmp/niemads-1.0.8.tar.gz` & `tmp/niemads-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/niemads-1.0.8.tar", last modified: Wed Jan 23 01:34:49 2019, max compression
+gzip compressed data, was "dist/niemads-1.0.9.tar", last modified: Wed Jan 23 17:46:44 2019, max compression
```

## Comparing `niemads-1.0.8.tar` & `niemads-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 niema      (501) staff       (20)        0 2019-01-23 01:34:49.000000 niemads-1.0.8/
--rw-r--r--   0 niema      (501) staff       (20)     1090 2019-01-23 01:34:49.000000 niemads-1.0.8/PKG-INFO
--rw-r--r--   0 niema      (501) staff       (20)    35149 2019-01-22 23:34:10.000000 niemads-1.0.8/LICENSE
-drwxr-xr-x   0 niema      (501) staff       (20)        0 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads/
--rw-r--r--   0 niema      (501) staff       (20)       70 2019-01-22 23:40:19.000000 niemads-1.0.8/niemads/__init__.py
--rwxr-xr-x   0 niema      (501) staff       (20)     4208 2019-01-23 01:32:58.000000 niemads-1.0.8/niemads/DisjointSet.py
--rw-r--r--   0 niema      (501) staff       (20)      130 2019-01-22 23:34:45.000000 niemads-1.0.8/MANIFEST.in
--rw-r--r--   0 niema      (501) staff       (20)       71 2019-01-22 23:34:10.000000 niemads-1.0.8/README.md
--rwxr-xr-x   0 niema      (501) staff       (20)     2157 2019-01-23 01:34:48.000000 niemads-1.0.8/setup.py
-drwxr-xr-x   0 niema      (501) staff       (20)        0 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads.egg-info/
--rw-r--r--   0 niema      (501) staff       (20)     1090 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads.egg-info/PKG-INFO
--rw-r--r--   0 niema      (501) staff       (20)      245 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads.egg-info/SOURCES.txt
--rw-r--r--   0 niema      (501) staff       (20)       22 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads.egg-info/requires.txt
--rw-r--r--   0 niema      (501) staff       (20)        8 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads.egg-info/top_level.txt
--rw-r--r--   0 niema      (501) staff       (20)        1 2019-01-23 01:34:49.000000 niemads-1.0.8/niemads.egg-info/dependency_links.txt
--rwxr-xr-x   0 niema      (501) staff       (20)      102 2019-01-23 01:34:49.000000 niemads-1.0.8/setup.cfg
+drwxr-xr-x   0 niema      (501) staff       (20)        0 2019-01-23 17:46:44.000000 niemads-1.0.9/
+-rw-r--r--   0 niema      (501) staff       (20)     1090 2019-01-23 17:46:44.000000 niemads-1.0.9/PKG-INFO
+-rw-r--r--   0 niema      (501) staff       (20)    35149 2019-01-22 23:34:10.000000 niemads-1.0.9/LICENSE
+drwxr-xr-x   0 niema      (501) staff       (20)        0 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads/
+-rw-r--r--   0 niema      (501) staff       (20)       70 2019-01-22 23:40:19.000000 niemads-1.0.9/niemads/__init__.py
+-rwxr-xr-x   0 niema      (501) staff       (20)     4210 2019-01-23 16:52:49.000000 niemads-1.0.9/niemads/DisjointSet.py
+-rwxr-xr-x   0 niema      (501) staff       (20)     3988 2019-01-23 17:43:32.000000 niemads-1.0.9/niemads/MultiwayTrie.py
+-rw-r--r--   0 niema      (501) staff       (20)      130 2019-01-22 23:34:45.000000 niemads-1.0.9/MANIFEST.in
+-rw-r--r--   0 niema      (501) staff       (20)       71 2019-01-22 23:34:10.000000 niemads-1.0.9/README.md
+-rwxr-xr-x   0 niema      (501) staff       (20)     2157 2019-01-23 17:46:42.000000 niemads-1.0.9/setup.py
+drwxr-xr-x   0 niema      (501) staff       (20)        0 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads.egg-info/
+-rw-r--r--   0 niema      (501) staff       (20)     1090 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads.egg-info/PKG-INFO
+-rw-r--r--   0 niema      (501) staff       (20)      269 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads.egg-info/SOURCES.txt
+-rw-r--r--   0 niema      (501) staff       (20)       22 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads.egg-info/requires.txt
+-rw-r--r--   0 niema      (501) staff       (20)        8 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads.egg-info/top_level.txt
+-rw-r--r--   0 niema      (501) staff       (20)        1 2019-01-23 17:46:44.000000 niemads-1.0.9/niemads.egg-info/dependency_links.txt
+-rwxr-xr-x   0 niema      (501) staff       (20)      102 2019-01-23 17:46:44.000000 niemads-1.0.9/setup.cfg
```

### Comparing `niemads-1.0.8/PKG-INFO` & `niemads-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niemads
-Version: 1.0.8
+Version: 1.0.9
 Summary: NiemaDS: Non-standard data structures for Python 2 and 3
 Home-page: https://github.com/niemasd/TreeDS
 Author: Niema Moshiri
 Author-email: niemamoshiri@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/niemasd/NiemaDS
 Project-URL: Bug Reports, https://github.com/niemasd/NiemaDS/issues
```

### Comparing `niemads-1.0.8/LICENSE` & `niemads-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `niemads-1.0.8/niemads/DisjointSet.py` & `niemads-1.0.9/niemads/DisjointSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 try:
     from Queue import Queue
 except ImportError:
     from queue import Queue
 class DisjointSet:
     '''``DisjointSet`` class, implemented using the Up-Tree data structure for amortized O(1) find and union operations'''
     def __init__(self, initial=None):
-        '''`DisjointSet` constructor
+        '''``DisjointSet`` constructor
         
         Args:
             ``initial`` (iterable): Elements with which to initialize the ``DisjointSet`` (each element will be in its own set)
         '''
         self.parent = dict() # parent[u] = parent of node u
         self.num_below = dict() # num_below[u] = number of nodes below u (including u) (only current for sentinels)
         if initial is not None:
```

### Comparing `niemads-1.0.8/setup.py` & `niemads-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 setup(
     name='niemads',  # Required
-    version='1.0.8',  # Required
+    version='1.0.9',  # Required
     description='NiemaDS: Non-standard data structures for Python 2 and 3',  # Required
     long_description='NiemaDS is a Python library that implements useful non-standard data structures.',  # Optional
     long_description_content_type='text/plain',  # Optional (see note above)
     url='https://github.com/niemasd/TreeDS',  # Optional
     author='Niema Moshiri',  # Optional
     author_email='niemamoshiri@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `niemads-1.0.8/niemads.egg-info/PKG-INFO` & `niemads-1.0.9/niemads.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niemads
-Version: 1.0.8
+Version: 1.0.9
 Summary: NiemaDS: Non-standard data structures for Python 2 and 3
 Home-page: https://github.com/niemasd/TreeDS
 Author: Niema Moshiri
 Author-email: niemamoshiri@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/niemasd/NiemaDS
 Project-URL: Bug Reports, https://github.com/niemasd/NiemaDS/issues
```

