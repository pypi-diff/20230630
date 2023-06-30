# Comparing `tmp/77tool-1.0.6.tar.gz` & `tmp/77tool-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "77tool-1.0.6.tar", last modified: Fri Jun 30 15:01:08 2023, max compression
+gzip compressed data, was "77tool-1.0.7.tar", last modified: Fri Jun 30 15:06:46 2023, max compression
```

## Comparing `77tool-1.0.6.tar` & `77tool-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:01:08.456689 77tool-1.0.6/
-drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:01:08.455935 77tool-1.0.6/77tool.egg-info/
--rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:01:08.000000 77tool-1.0.6/77tool.egg-info/PKG-INFO
--rw-r--r--   0 linrol     (501) staff       (20)      231 2023-06-30 15:01:08.000000 77tool-1.0.6/77tool.egg-info/SOURCES.txt
--rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:01:08.000000 77tool-1.0.6/77tool.egg-info/dependency_links.txt
--rw-r--r--   0 linrol     (501) staff       (20)       37 2023-06-30 15:01:08.000000 77tool-1.0.6/77tool.egg-info/entry_points.txt
--rw-r--r--   0 linrol     (501) staff       (20)       17 2023-06-30 15:01:08.000000 77tool-1.0.6/77tool.egg-info/requires.txt
--rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:01:08.000000 77tool-1.0.6/77tool.egg-info/top_level.txt
--rw-r--r--   0 linrol     (501) staff       (20)     1062 2023-06-30 12:54:33.000000 77tool-1.0.6/LICENSE
--rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:01:08.456340 77tool-1.0.6/PKG-INFO
--rw-r--r--   0 linrol     (501) staff       (20)      244 2023-06-30 13:04:21.000000 77tool-1.0.6/README.md
--rw-r--r--   0 linrol     (501) staff       (20)       84 2023-06-30 12:54:33.000000 77tool-1.0.6/pyproject.toml
--rw-r--r--   0 linrol     (501) staff       (20)       38 2023-06-30 15:01:08.456765 77tool-1.0.6/setup.cfg
--rw-r--r--   0 linrol     (501) staff       (20)      699 2023-06-30 15:00:38.000000 77tool-1.0.6/setup.py
--rw-r--r--   0 linrol     (501) staff       (20)      808 2023-06-30 13:55:20.000000 77tool-1.0.6/tool.py
+drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:06:46.527065 77tool-1.0.7/
+drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:06:46.526306 77tool-1.0.7/77tool.egg-info/
+-rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:06:46.000000 77tool-1.0.7/77tool.egg-info/PKG-INFO
+-rw-r--r--   0 linrol     (501) staff       (20)      239 2023-06-30 15:06:46.000000 77tool-1.0.7/77tool.egg-info/SOURCES.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:06:46.000000 77tool-1.0.7/77tool.egg-info/dependency_links.txt
+-rw-r--r--   0 linrol     (501) staff       (20)       37 2023-06-30 15:06:46.000000 77tool-1.0.7/77tool.egg-info/entry_points.txt
+-rw-r--r--   0 linrol     (501) staff       (20)       17 2023-06-30 15:06:46.000000 77tool-1.0.7/77tool.egg-info/requires.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:06:46.000000 77tool-1.0.7/77tool.egg-info/top_level.txt
+-rw-r--r--   0 linrol     (501) staff       (20)     1062 2023-06-30 12:54:33.000000 77tool-1.0.7/LICENSE
+-rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:06:46.526650 77tool-1.0.7/PKG-INFO
+-rw-r--r--   0 linrol     (501) staff       (20)      244 2023-06-30 13:04:21.000000 77tool-1.0.7/README.md
+-rw-r--r--   0 linrol     (501) staff       (20)       84 2023-06-30 12:54:33.000000 77tool-1.0.7/pyproject.toml
+-rw-r--r--   0 linrol     (501) staff       (20)       38 2023-06-30 15:06:46.527144 77tool-1.0.7/setup.cfg
+-rw-r--r--   0 linrol     (501) staff       (20)      699 2023-06-30 15:06:19.000000 77tool-1.0.7/setup.py
+-rw-r--r--   0 linrol     (501) staff       (20)       47 2023-06-30 15:05:48.000000 77tool-1.0.7/test.py
+-rw-r--r--   0 linrol     (501) staff       (20)      808 2023-06-30 13:55:20.000000 77tool-1.0.7/tool.py
```

### Comparing `77tool-1.0.6/77tool.egg-info/PKG-INFO` & `77tool-1.0.7/77tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 77tool
-Version: 1.0.6
+Version: 1.0.7
 Summary: 77 branch tool
 Home-page: https://github.com/linrol/77tool
 Author: linrol
 Author-email: linrolmail@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `77tool-1.0.6/LICENSE` & `77tool-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `77tool-1.0.6/PKG-INFO` & `77tool-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 77tool
-Version: 1.0.6
+Version: 1.0.7
 Summary: 77 branch tool
 Home-page: https://github.com/linrol/77tool
 Author: linrol
 Author-email: linrolmail@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `77tool-1.0.6/tool.py` & `77tool-1.0.7/tool.py`

 * *Files identical despite different names*

