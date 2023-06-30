# Comparing `tmp/77tool-1.0.9.tar.gz` & `tmp/77tool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "77tool-1.0.9.tar", last modified: Fri Jun 30 15:21:38 2023, max compression
+gzip compressed data, was "77tool-1.1.0.tar", last modified: Fri Jun 30 15:28:21 2023, max compression
```

## Comparing `77tool-1.0.9.tar` & `77tool-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:21:38.638996 77tool-1.0.9/
-drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:21:38.638425 77tool-1.0.9/77tool.egg-info/
--rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:21:38.000000 77tool-1.0.9/77tool.egg-info/PKG-INFO
--rw-r--r--   0 linrol     (501) staff       (20)      231 2023-06-30 15:21:38.000000 77tool-1.0.9/77tool.egg-info/SOURCES.txt
--rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:21:38.000000 77tool-1.0.9/77tool.egg-info/dependency_links.txt
--rw-r--r--   0 linrol     (501) staff       (20)       37 2023-06-30 15:21:38.000000 77tool-1.0.9/77tool.egg-info/entry_points.txt
--rw-r--r--   0 linrol     (501) staff       (20)       17 2023-06-30 15:21:38.000000 77tool-1.0.9/77tool.egg-info/requires.txt
--rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:21:38.000000 77tool-1.0.9/77tool.egg-info/top_level.txt
--rw-r--r--   0 linrol     (501) staff       (20)     1062 2023-06-30 12:54:33.000000 77tool-1.0.9/LICENSE
--rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:21:38.638750 77tool-1.0.9/PKG-INFO
--rw-r--r--   0 linrol     (501) staff       (20)      244 2023-06-30 13:04:21.000000 77tool-1.0.9/README.md
--rw-r--r--   0 linrol     (501) staff       (20)       84 2023-06-30 12:54:33.000000 77tool-1.0.9/pyproject.toml
--rw-r--r--   0 linrol     (501) staff       (20)       38 2023-06-30 15:21:38.639063 77tool-1.0.9/setup.cfg
--rw-r--r--   0 linrol     (501) staff       (20)      709 2023-06-30 15:21:22.000000 77tool-1.0.9/setup.py
--rw-r--r--   0 linrol     (501) staff       (20)       47 2023-06-30 15:05:48.000000 77tool-1.0.9/test.py
+drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:28:21.127952 77tool-1.1.0/
+drwxr-xr-x   0 linrol     (501) staff       (20)        0 2023-06-30 15:28:21.127372 77tool-1.1.0/77tool.egg-info/
+-rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:28:21.000000 77tool-1.1.0/77tool.egg-info/PKG-INFO
+-rw-r--r--   0 linrol     (501) staff       (20)      231 2023-06-30 15:28:21.000000 77tool-1.1.0/77tool.egg-info/SOURCES.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:28:21.000000 77tool-1.1.0/77tool.egg-info/dependency_links.txt
+-rw-r--r--   0 linrol     (501) staff       (20)       36 2023-06-30 15:28:21.000000 77tool-1.1.0/77tool.egg-info/entry_points.txt
+-rw-r--r--   0 linrol     (501) staff       (20)       17 2023-06-30 15:28:21.000000 77tool-1.1.0/77tool.egg-info/requires.txt
+-rw-r--r--   0 linrol     (501) staff       (20)        1 2023-06-30 15:28:21.000000 77tool-1.1.0/77tool.egg-info/top_level.txt
+-rw-r--r--   0 linrol     (501) staff       (20)     1062 2023-06-30 12:54:33.000000 77tool-1.1.0/LICENSE
+-rw-r--r--   0 linrol     (501) staff       (20)      622 2023-06-30 15:28:21.127697 77tool-1.1.0/PKG-INFO
+-rw-r--r--   0 linrol     (501) staff       (20)      244 2023-06-30 13:04:21.000000 77tool-1.1.0/README.md
+-rw-r--r--   0 linrol     (501) staff       (20)       84 2023-06-30 12:54:33.000000 77tool-1.1.0/pyproject.toml
+-rw-r--r--   0 linrol     (501) staff       (20)       38 2023-06-30 15:28:21.128026 77tool-1.1.0/setup.cfg
+-rw-r--r--   0 linrol     (501) staff       (20)      708 2023-06-30 15:28:06.000000 77tool-1.1.0/setup.py
+-rw-r--r--   0 linrol     (501) staff       (20)      833 2023-06-30 15:27:02.000000 77tool-1.1.0/tool.py
```

### Comparing `77tool-1.0.9/77tool.egg-info/PKG-INFO` & `77tool-1.1.0/77tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 77tool
-Version: 1.0.9
+Version: 1.1.0
 Summary: 77 branch tool
 Home-page: https://github.com/linrol/77tool
 Author: linrol
 Author-email: linrolmail@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `77tool-1.0.9/LICENSE` & `77tool-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `77tool-1.0.9/PKG-INFO` & `77tool-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 77tool
-Version: 1.0.9
+Version: 1.1.0
 Summary: 77 branch tool
 Home-page: https://github.com/linrol/77tool
 Author: linrol
 Author-email: linrolmail@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

