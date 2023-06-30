# Comparing `tmp/ncs-uml-1.0.0.tar.gz` & `tmp/ncs-uml-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncs-uml-1.0.0.tar", last modified: Fri Jun 30 20:25:06 2023, max compression
+gzip compressed data, was "ncs-uml-1.0.1.tar", last modified: Fri Jun 30 21:49:16 2023, max compression
```

## Comparing `ncs-uml-1.0.0.tar` & `ncs-uml-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:25:06.832288 ncs-uml-1.0.0/
--rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.0.0/LICENSE
--rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-1.0.0/MANIFEST.in
--rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 20:25:06.832105 ncs-uml-1.0.0/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)        9 2023-06-23 13:12:35.000000 ncs-uml-1.0.0/README.md
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:25:06.830788 ncs-uml-1.0.0/ncs_uml/
--rw-r--r--   0 kkotari    (501) staff       (20)      248 2023-06-30 20:23:43.000000 ncs-uml-1.0.0/ncs_uml/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5528 2023-06-30 20:12:43.000000 ncs-uml-1.0.0/ncs_uml/main.py
--rw-r--r--   0 kkotari    (501) staff       (20)      639 2023-06-24 00:35:50.000000 ncs-uml-1.0.0/ncs_uml/run.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5981 2023-06-30 20:08:47.000000 ncs-uml-1.0.0/ncs_uml/utils.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 20:25:06.831870 ncs-uml-1.0.0/ncs_uml.egg-info/
--rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)      311 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/SOURCES.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/dependency_links.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       71 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/entry_points.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/requires.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-06-30 20:25:06.000000 ncs-uml-1.0.0/ncs_uml.egg-info/top_level.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.0.0/requirements.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-06-30 20:25:06.832346 ncs-uml-1.0.0/setup.cfg
--rw-r--r--   0 kkotari    (501) staff       (20)     1683 2023-06-30 20:23:16.000000 ncs-uml-1.0.0/setup.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 21:49:16.440384 ncs-uml-1.0.1/
+-rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.0.1/LICENSE
+-rw-r--r--   0 kkotari    (501) staff       (20)       75 2023-06-23 13:29:14.000000 ncs-uml-1.0.1/MANIFEST.in
+-rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 21:49:16.440209 ncs-uml-1.0.1/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)        9 2023-06-23 13:12:35.000000 ncs-uml-1.0.1/README.md
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 21:49:16.438707 ncs-uml-1.0.1/ncs_uml/
+-rw-r--r--   0 kkotari    (501) staff       (20)      248 2023-06-30 21:33:18.000000 ncs-uml-1.0.1/ncs_uml/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5545 2023-06-30 21:41:35.000000 ncs-uml-1.0.1/ncs_uml/main.py
+-rw-r--r--   0 kkotari    (501) staff       (20)      960 2023-06-30 21:48:39.000000 ncs-uml-1.0.1/ncs_uml/run.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5981 2023-06-30 20:08:47.000000 ncs-uml-1.0.1/ncs_uml/utils.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-06-30 21:49:16.439977 ncs-uml-1.0.1/ncs_uml.egg-info/
+-rw-r--r--   0 kkotari    (501) staff       (20)      999 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)      311 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       71 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/entry_points.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/requires.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-06-30 21:49:16.000000 ncs-uml-1.0.1/ncs_uml.egg-info/top_level.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.0.1/requirements.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-06-30 21:49:16.440439 ncs-uml-1.0.1/setup.cfg
+-rw-r--r--   0 kkotari    (501) staff       (20)     1683 2023-06-30 20:23:16.000000 ncs-uml-1.0.1/setup.py
```

### Comparing `ncs-uml-1.0.0/LICENSE` & `ncs-uml-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.0.0/PKG-INFO` & `ncs-uml-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.0.0
+Version: 1.0.1
 Summary: ncs-uml is the smartway to generate the plantuml code from yang file
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
```

### Comparing `ncs-uml-1.0.0/ncs_uml/main.py` & `ncs-uml-1.0.1/ncs_uml/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         """
 
     @property
     def options(self):
         self._help = ['-h', '--help']
         self._version = ['-v', '--version']
         self._verbose = ['-vv', '--verbose']
-        return self.util.flatset([self._help, self._version, self._verbose])
+        return self.util.flatset([['--skip-uses'], self._help, self._version, self._verbose])
 
     def get_ncs_path(self):
         ncs_path = None
         try:
             ncs_path = self.util.cmd.run(['which', 'ncsc'])
         except Exception as e:
             msg = f"source <NCS-DIR>/ncsrc\n\n{e.message}"
```

### Comparing `ncs-uml-1.0.0/ncs_uml/utils.py` & `ncs-uml-1.0.1/ncs_uml/utils.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.0.0/ncs_uml.egg-info/PKG-INFO` & `ncs-uml-1.0.1/ncs_uml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.0.0
+Version: 1.0.1
 Summary: ncs-uml is the smartway to generate the plantuml code from yang file
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
```

### Comparing `ncs-uml-1.0.0/setup.py` & `ncs-uml-1.0.1/setup.py`

 * *Files identical despite different names*

