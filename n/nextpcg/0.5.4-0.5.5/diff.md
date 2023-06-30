# Comparing `tmp/nextpcg-0.5.4.tar.gz` & `tmp/nextpcg-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.4.tar", last modified: Thu Jun 29 08:50:36 2023, max compression
+gzip compressed data, was "nextpcg-0.5.5.tar", last modified: Fri Jun 30 02:51:08 2023, max compression
```

## Comparing `nextpcg-0.5.4.tar` & `nextpcg-0.5.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.990858 nextpcg-0.5.4/
--rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-06-29 08:50:36.989857 nextpcg-0.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.957828 nextpcg-0.5.4/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.4/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.983851 nextpcg-0.5.4/pypapi/
--rw-rw-rw-   0        0        0      713 2023-06-29 08:49:32.000000 nextpcg-0.5.4/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.4/pypapi/const.py
--rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/dson.py
--rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.4/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field.py
--rw-rw-rw-   0        0        0     1835 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field_heightfield.py
--rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field_instanced_staticmesh.py
--rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field_texture.py
--rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.4/pypapi/geo.py
--rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.4/pypapi/geo_heightfield.py
--rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/geo_instanced_staticmesh.py
--rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.4/pypapi/geo_texture.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.4/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.4/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.987855 nextpcg-0.5.4/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-06-29 08:50:36.990858 nextpcg-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-06-29 08:50:18.000000 nextpcg-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:51:08.807051 nextpcg-0.5.5/
+-rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-06-30 02:51:08.806050 nextpcg-0.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 02:51:08.776023 nextpcg-0.5.5/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-06-30 02:51:08.000000 nextpcg-0.5.5/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-06-30 02:51:08.000000 nextpcg-0.5.5/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:51:08.000000 nextpcg-0.5.5/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-30 02:51:08.000000 nextpcg-0.5.5/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 02:51:08.000000 nextpcg-0.5.5/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 02:51:08.000000 nextpcg-0.5.5/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.5/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-30 02:51:08.801047 nextpcg-0.5.5/pypapi/
+-rw-rw-rw-   0        0        0       17 2023-06-30 02:26:01.000000 nextpcg-0.5.5/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.5/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.5/pypapi/const.py
+-rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.5/pypapi/dson.py
+-rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.5/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.5/pypapi/field.py
+-rw-rw-rw-   0        0        0     1430 2023-06-30 01:56:30.000000 nextpcg-0.5.5/pypapi/field_heightfield.py
+-rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.5/pypapi/field_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.5/pypapi/field_texture.py
+-rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.5/pypapi/geo.py
+-rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.5/pypapi/geo_heightfield.py
+-rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.5/pypapi/geo_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.5/pypapi/geo_texture.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.5/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.5/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:51:08.804049 nextpcg-0.5.5/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.5/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.5/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.5/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:51:08.807051 nextpcg-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-06-30 01:52:29.000000 nextpcg-0.5.5/setup.py
```

### Comparing `nextpcg-0.5.4/PKG-INFO` & `nextpcg-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.4
+Version: 0.5.5
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.4/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.5.5/nextpcg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.4
+Version: 0.5.5
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.4/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.5.5/nextpcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/__main__.py` & `nextpcg-0.5.5/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/dson.py` & `nextpcg-0.5.5/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/dson_create.py` & `nextpcg-0.5.5/pypapi/dson_create.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/field.py` & `nextpcg-0.5.5/pypapi/field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/field_heightfield.py` & `nextpcg-0.5.5/pypapi/field_heightfield.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,14 @@
 class HeightFieldField(Field):
     """
     _value is list of HeightField
     """
     field_type_name = "paramType.HeightField"
     support_param = False
 
-    # @classmethod
-    # def create_json_field(cls, field_category=FieldCategory.Input, name: str = None):
-    #     """ create a json object
-    #     """
-    #     """get json format field"""
-    #     field = {'Type': cls.field_type_name, 'If List': cls.if_list, 'FieldCategory': field_category.name}
-    #     if name is not None:
-    #         field["Label"] = name
-    #     return field
-
     def __init__(self, value=None):
         self._value: List[HeightField] = value
 
     @classmethod
     def from_json(cls, json_object, input_name, field_desc):
         if field_desc.work_path is None:
             raise Exception("HeightFieldField from_json failed:work path need to be set, not allowed")
```

### Comparing `nextpcg-0.5.4/pypapi/field_instanced_staticmesh.py` & `nextpcg-0.5.5/pypapi/field_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/field_texture.py` & `nextpcg-0.5.5/pypapi/field_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/geo.py` & `nextpcg-0.5.5/pypapi/geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/geo_heightfield.py` & `nextpcg-0.5.5/pypapi/geo_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/geo_instanced_staticmesh.py` & `nextpcg-0.5.5/pypapi/geo_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/geo_texture.py` & `nextpcg-0.5.5/pypapi/geo_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/meta_helper.py` & `nextpcg-0.5.5/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/pantry/dson_generator.py` & `nextpcg-0.5.5/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/pypapi/plugin_protocol.py` & `nextpcg-0.5.5/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.4/setup.py` & `nextpcg-0.5.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.5.4',
+    version='0.5.5',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```

