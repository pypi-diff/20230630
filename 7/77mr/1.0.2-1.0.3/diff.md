# Comparing `tmp/77mr-1.0.2.tar.gz` & `tmp/77mr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "77mr-1.0.2.tar", last modified: Fri Jun 30 10:13:26 2023, max compression
+gzip compressed data, was "77mr-1.0.3.tar", last modified: Fri Jun 30 10:28:42 2023, max compression
```

## Comparing `77mr-1.0.2.tar` & `77mr-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 10:13:26.809260 77mr-1.0.2/
-drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 10:13:26.808738 77mr-1.0.2/77mr.egg-info/
--rw-r--r--   0 linrol     (501) staff       (20)      615 2023-06-30 10:13:26.000000 77mr-1.0.2/77mr.egg-info/PKG-INFO
--rw-r--r--   0 linrol     (501) staff       (20)      186 2023-06-30 10:13:26.000000 77mr-1.0.2/77mr.egg-info/SOURCES.txt
--rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 10:13:26.000000 77mr-1.0.2/77mr.egg-info/dependency_links.txt
--rw-r--r--   0 linrol     (501) staff       (20)        9 2023-06-30 10:13:26.000000 77mr-1.0.2/77mr.egg-info/requires.txt
--rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 10:13:26.000000 77mr-1.0.2/77mr.egg-info/top_level.txt
--rw-r--r--   0 linrol     (501) staff       (20)     1062 2023-06-30 09:37:07.000000 77mr-1.0.2/LICENSE
--rw-r--r--   0 linrol     (501) staff       (20)      615 2023-06-30 10:13:26.809039 77mr-1.0.2/PKG-INFO
--rw-r--r--   0 linrol     (501) staff       (20)      237 2023-06-30 09:37:07.000000 77mr-1.0.2/README.md
--rw-r--r--   0 linrol     (501) staff       (20)      492 2023-06-30 09:37:07.000000 77mr-1.0.2/mr.py
--rw-r--r--   0 linrol     (501) staff       (20)       84 2023-06-30 09:37:07.000000 77mr-1.0.2/pyproject.toml
--rw-r--r--   0 linrol     (501) staff       (20)       38 2023-06-30 10:13:26.809374 77mr-1.0.2/setup.cfg
--rw-r--r--   0 linrol     (501) staff       (20)      588 2023-06-30 10:11:24.000000 77mr-1.0.2/setup.py
+drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 10:28:42.675179 77mr-1.0.3/
+drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 10:28:42.674617 77mr-1.0.3/77mr.egg-info/
+-rw-r--r--   0 linrol     (501) staff       (20)      615 2023-06-30 10:28:42.000000 77mr-1.0.3/77mr.egg-info/PKG-INFO
+-rw-r--r--   0 linrol     (501) staff       (20)      217 2023-06-30 10:28:42.000000 77mr-1.0.3/77mr.egg-info/SOURCES.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 10:28:42.000000 77mr-1.0.3/77mr.egg-info/dependency_links.txt
+-rw-r--r--   0 linrol     (501) staff       (20)       31 2023-06-30 10:28:42.000000 77mr-1.0.3/77mr.egg-info/entry_points.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        9 2023-06-30 10:28:42.000000 77mr-1.0.3/77mr.egg-info/requires.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 10:28:42.000000 77mr-1.0.3/77mr.egg-info/top_level.txt
+-rw-r--r--   0 linrol     (501) staff       (20)     1062 2023-06-30 09:37:07.000000 77mr-1.0.3/LICENSE
+-rw-r--r--   0 linrol     (501) staff       (20)      615 2023-06-30 10:28:42.674934 77mr-1.0.3/PKG-INFO
+-rw-r--r--   0 linrol     (501) staff       (20)      237 2023-06-30 09:37:07.000000 77mr-1.0.3/README.md
+-rw-r--r--   0 linrol     (501) staff       (20)      492 2023-06-30 09:37:07.000000 77mr-1.0.3/mr.py
+-rw-r--r--   0 linrol     (501) staff       (20)       84 2023-06-30 09:37:07.000000 77mr-1.0.3/pyproject.toml
+-rw-r--r--   0 linrol     (501) staff       (20)       38 2023-06-30 10:28:42.675256 77mr-1.0.3/setup.cfg
+-rw-r--r--   0 linrol     (501) staff       (20)      680 2023-06-30 10:28:26.000000 77mr-1.0.3/setup.py
```

### Comparing `77mr-1.0.2/77mr.egg-info/PKG-INFO` & `77mr-1.0.3/77mr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 77mr
-Version: 1.0.2
+Version: 1.0.3
 Summary: create merge request
 Home-page: https://github.com/linrol/mr
 Author: linrol
 Author-email: linrolmail@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `77mr-1.0.2/LICENSE` & `77mr-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `77mr-1.0.2/PKG-INFO` & `77mr-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 77mr
-Version: 1.0.2
+Version: 1.0.3
 Summary: create merge request
 Home-page: https://github.com/linrol/mr
 Author: linrol
 Author-email: linrolmail@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

