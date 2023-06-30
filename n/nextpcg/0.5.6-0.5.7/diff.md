# Comparing `tmp/nextpcg-0.5.6.tar.gz` & `tmp/nextpcg-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.6.tar", last modified: Fri Jun 30 02:56:06 2023, max compression
+gzip compressed data, was "nextpcg-0.5.7.tar", last modified: Fri Jun 30 03:01:37 2023, max compression
```

## Comparing `nextpcg-0.5.6.tar` & `nextpcg-0.5.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:56:06.338725 nextpcg-0.5.6/
--rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-06-30 02:56:06.337724 nextpcg-0.5.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 02:56:06.293683 nextpcg-0.5.6/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-06-30 02:56:06.000000 nextpcg-0.5.6/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-06-30 02:56:06.000000 nextpcg-0.5.6/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:56:06.000000 nextpcg-0.5.6/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-30 02:56:06.000000 nextpcg-0.5.6/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-06-30 02:56:06.000000 nextpcg-0.5.6/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 02:56:06.000000 nextpcg-0.5.6/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.6/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-30 02:56:06.330718 nextpcg-0.5.6/pypapi/
--rw-rw-rw-   0        0        0       87 2023-06-30 02:55:09.000000 nextpcg-0.5.6/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.6/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.6/pypapi/const.py
--rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.6/pypapi/dson.py
--rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.6/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.6/pypapi/field.py
--rw-rw-rw-   0        0        0     1430 2023-06-30 01:56:30.000000 nextpcg-0.5.6/pypapi/field_heightfield.py
--rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.6/pypapi/field_instanced_staticmesh.py
--rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.6/pypapi/field_texture.py
--rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.6/pypapi/geo.py
--rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.6/pypapi/geo_heightfield.py
--rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.6/pypapi/geo_instanced_staticmesh.py
--rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.6/pypapi/geo_texture.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.6/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.6/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:56:06.335722 nextpcg-0.5.6/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.6/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.6/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.6/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-06-30 02:56:06.339726 nextpcg-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-06-30 02:55:51.000000 nextpcg-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.170993 nextpcg-0.5.7/
+-rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-06-30 03:01:37.169992 nextpcg-0.5.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.138964 nextpcg-0.5.7/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.7/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.164988 nextpcg-0.5.7/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-06-30 03:01:10.000000 nextpcg-0.5.7/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.7/pypapi/const.py
+-rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/dson.py
+-rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.7/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/field.py
+-rw-rw-rw-   0        0        0     1430 2023-06-30 01:56:30.000000 nextpcg-0.5.7/pypapi/field_heightfield.py
+-rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/field_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/field_texture.py
+-rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.7/pypapi/geo.py
+-rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.7/pypapi/geo_heightfield.py
+-rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/geo_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.7/pypapi/geo_texture.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.7/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.7/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.167990 nextpcg-0.5.7/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 03:01:37.170993 nextpcg-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-06-30 03:01:16.000000 nextpcg-0.5.7/setup.py
```

### Comparing `nextpcg-0.5.6/PKG-INFO` & `nextpcg-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.6
+Version: 0.5.7
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.6/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.5.7/nextpcg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.6
+Version: 0.5.7
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.6/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.5.7/nextpcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/__main__.py` & `nextpcg-0.5.7/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/dson.py` & `nextpcg-0.5.7/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/dson_create.py` & `nextpcg-0.5.7/pypapi/dson_create.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/field.py` & `nextpcg-0.5.7/pypapi/field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/field_heightfield.py` & `nextpcg-0.5.7/pypapi/field_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/field_instanced_staticmesh.py` & `nextpcg-0.5.7/pypapi/field_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/field_texture.py` & `nextpcg-0.5.7/pypapi/field_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/geo.py` & `nextpcg-0.5.7/pypapi/geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/geo_heightfield.py` & `nextpcg-0.5.7/pypapi/geo_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/geo_instanced_staticmesh.py` & `nextpcg-0.5.7/pypapi/geo_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/geo_texture.py` & `nextpcg-0.5.7/pypapi/geo_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/meta_helper.py` & `nextpcg-0.5.7/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/pantry/dson_generator.py` & `nextpcg-0.5.7/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/pypapi/plugin_protocol.py` & `nextpcg-0.5.7/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.6/setup.py` & `nextpcg-0.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.5.6',
+    version='0.5.7',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```

