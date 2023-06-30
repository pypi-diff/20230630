# Comparing `tmp/up_enhsp-0.0.8.tar.gz` & `tmp/up_enhsp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_enhsp-0.0.8.tar", last modified: Mon Dec  5 14:15:22 2022, max compression
+gzip compressed data, was "up_enhsp-0.0.9.tar", last modified: Thu Dec 22 09:43:36 2022, max compression
```

## Comparing `up_enhsp-0.0.8.tar` & `up_enhsp-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 14:15:22.109609 up_enhsp-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-05 14:15:13.000000 up_enhsp-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-05 14:15:22.109609 up_enhsp-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2022-12-05 14:15:13.000000 up_enhsp-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 14:15:22.109609 up_enhsp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2022-12-05 14:15:13.000000 up_enhsp-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 14:15:22.109609 up_enhsp-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2022-12-05 14:15:13.000000 up_enhsp-0.0.8/test/test_up_enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 14:15:22.109609 up_enhsp-0.0.8/up_enhsp/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-05 14:15:13.000000 up_enhsp-0.0.8/up_enhsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2022-12-05 14:15:13.000000 up_enhsp-0.0.8/up_enhsp/enhsp_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 14:15:22.109609 up_enhsp-0.0.8/up_enhsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-05 14:15:22.000000 up_enhsp-0.0.8/up_enhsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-05 14:15:22.000000 up_enhsp-0.0.8/up_enhsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 14:15:22.000000 up_enhsp-0.0.8/up_enhsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-05 14:15:22.000000 up_enhsp-0.0.8/up_enhsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 09:43:36.923326 up_enhsp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-22 09:43:24.000000 up_enhsp-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-22 09:43:36.923326 up_enhsp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2022-12-22 09:43:24.000000 up_enhsp-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 09:43:36.923326 up_enhsp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2022-12-22 09:43:24.000000 up_enhsp-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 09:43:36.919326 up_enhsp-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2022-12-22 09:43:24.000000 up_enhsp-0.0.9/test/test_up_enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 09:43:36.919326 up_enhsp-0.0.9/up_enhsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-22 09:43:24.000000 up_enhsp-0.0.9/up_enhsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2022-12-22 09:43:24.000000 up_enhsp-0.0.9/up_enhsp/enhsp_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 09:43:36.923326 up_enhsp-0.0.9/up_enhsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-22 09:43:36.000000 up_enhsp-0.0.9/up_enhsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-22 09:43:36.000000 up_enhsp-0.0.9/up_enhsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 09:43:36.000000 up_enhsp-0.0.9/up_enhsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-22 09:43:36.000000 up_enhsp-0.0.9/up_enhsp.egg-info/top_level.txt
```

### Comparing `up_enhsp-0.0.8/LICENSE` & `up_enhsp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `up_enhsp-0.0.8/README.md` & `up_enhsp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `up_enhsp-0.0.8/setup.py` & `up_enhsp-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import urllib
 import shutil
 
 
 ENHSP_dst = './up_enhsp/ENHSP'
 ENHSP_PUBLIC = 'ENHSP-Public'
 COMPILE_CMD = './compile'
-ENHSP_TAG = 'enhsp20-0.9.4'
+ENHSP_TAG = 'enhsp20-0.9.5'
 ENHSP_REPO = 'https://gitlab.com/enricos83/ENHSP-Public'
 JDK_REQUIRE = 17
 
 long_description = \
     """============================================================
     UP_ENHSP
  ============================================================
@@ -58,15 +58,15 @@
 
     def run(self):
         install_ENHSP()
         develop.run(self)
 
 
 setup(name='up_enhsp',
-      version='0.0.8',
+      version='0.0.9',
       description='up_enhsp',
       author='UNIBS Team',
       author_email='enrico.scala@unibs.it',
       packages=['up_enhsp'],
       package_data={
           "": ["ENHSP/enhsp.jar","ENHSP/libs/*"],
       },
```

### Comparing `up_enhsp-0.0.8/test/test_up_enhsp.py` & `up_enhsp-0.0.9/test/test_up_enhsp.py`

 * *Files identical despite different names*

### Comparing `up_enhsp-0.0.8/up_enhsp/enhsp_planner.py` & `up_enhsp-0.0.9/up_enhsp/enhsp_planner.py`

 * *Files identical despite different names*

