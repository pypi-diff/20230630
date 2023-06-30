# Comparing `tmp/nextpcg-0.5.7.tar.gz` & `tmp/nextpcg-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.7.tar", last modified: Fri Jun 30 03:01:37 2023, max compression
+gzip compressed data, was "nextpcg-0.5.8.tar", last modified: Fri Jun 30 06:04:40 2023, max compression
```

## Comparing `nextpcg-0.5.7.tar` & `nextpcg-0.5.8.tar`

### file list

```diff
@@ -1,33 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.170993 nextpcg-0.5.7/
--rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-06-30 03:01:37.169992 nextpcg-0.5.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.138964 nextpcg-0.5.7/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 03:01:37.000000 nextpcg-0.5.7/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.7/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.164988 nextpcg-0.5.7/pypapi/
--rw-rw-rw-   0        0        0       15 2023-06-30 03:01:10.000000 nextpcg-0.5.7/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.7/pypapi/const.py
--rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/dson.py
--rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.7/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/field.py
--rw-rw-rw-   0        0        0     1430 2023-06-30 01:56:30.000000 nextpcg-0.5.7/pypapi/field_heightfield.py
--rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/field_instanced_staticmesh.py
--rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/field_texture.py
--rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.7/pypapi/geo.py
--rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.7/pypapi/geo_heightfield.py
--rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.7/pypapi/geo_instanced_staticmesh.py
--rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.7/pypapi/geo_texture.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.7/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.7/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:01:37.167990 nextpcg-0.5.7/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.7/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-06-30 03:01:37.170993 nextpcg-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-06-30 03:01:16.000000 nextpcg-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.543034 nextpcg-0.5.8/
+-rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-06-30 06:04:40.543034 nextpcg-0.5.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.522014 nextpcg-0.5.8/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.8/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.538030 nextpcg-0.5.8/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-06-30 03:01:10.000000 nextpcg-0.5.8/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.8/pypapi/const.py
+-rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/dson.py
+-rw-rw-rw-   0        0        0    10191 2023-06-30 03:23:16.000000 nextpcg-0.5.8/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    17451 2023-06-30 03:18:15.000000 nextpcg-0.5.8/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-06-30 03:10:42.000000 nextpcg-0.5.8/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.8/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.8/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.541032 nextpcg-0.5.8/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 06:04:40.544034 nextpcg-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-06-30 06:04:36.000000 nextpcg-0.5.8/setup.py
```

### Comparing `nextpcg-0.5.7/PKG-INFO` & `nextpcg-0.5.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.7
+Version: 0.5.8
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.7/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.5.8/nextpcg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.7
+Version: 0.5.8
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.7/pypapi/__main__.py` & `nextpcg-0.5.8/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.7/pypapi/dson.py` & `nextpcg-0.5.8/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.7/pypapi/dson_create.py` & `nextpcg-0.5.8/pypapi/dson_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import os
 import json
 import logging
 
 from inspect import signature, Signature
 from functools import wraps
 from typing import *
-from .field import Field, FieldCategory
 from .const import *
 from .dson import DsonMetaInfo, DsonManager, nextpcgmethod
+from .dson_field import Field, FieldCategory
 
 
 def create_dson_from_pda(func: Callable, tag, dson_meta_info: DsonMetaInfo) -> Dict:
     cda_json = {}
     try:
         func_sig = signature(func)
         func_name = func.__name__
```

### Comparing `nextpcg-0.5.7/pypapi/field.py` & `nextpcg-0.5.8/pypapi/dson_field.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 """
 Author  : NextPCG
 """
 
 import json
 import os
 import time
-from typing import Dict, List, Tuple, Any
-from inspect import signature, Signature, Parameter
-import logging
-from abc import ABCMeta, abstractmethod
+from typing import Dict, List
 from enum import Enum
+
+from .dson_geo import HeightField, InstancedStaticMesh, Texture
 from .meta_helper import Singleton
 
 """note:
 io_mode:
 0: server_text (like houdini_text)
 1: houdini_text (support)
 2: houdini_binary (support)
@@ -432,7 +431,88 @@
 
     def get_output(self, json_field, field_desc: FieldDesc, data_field='Value Data', output_index=0):
         def helper(value):
             return self.inner_field_type.list_to_json_value(value, work_path=field_desc.work_path)
 
         values = list(map(helper, self._value))
         json_field[data_field] = values
+
+
+class HeightFieldField(Field):
+    """
+    _value is list of HeightField
+    """
+    field_type_name = "paramType.HeightField"
+    support_param = False
+
+    def __init__(self, value=None):
+        self._value: List[HeightField] = value
+
+    @classmethod
+    def from_json(cls, json_object, input_name, field_desc):
+        if field_desc.work_path is None:
+            raise Exception("HeightFieldField from_json failed:work path need to be set, not allowed")
+        value = []
+        for editing_layer_key, editing_layer_val in json_object.items():
+            if 'EditingLayer_' in editing_layer_key:
+                heightfield = HeightField.create_from_json(json_object, editing_layer_val, field_desc.work_path, field_desc.io_mode, field_desc.raw_compress)
+                value.append(heightfield)
+        return cls(value)
+
+    def get_input(self):
+        return self._value
+
+    def get_output(self, json_field, field_desc: FieldDesc, data_field='Value Data', output_index=0):
+        geo_index = 0
+        for heightfield in self._value:
+            num = heightfield.to_json(geo_index, output_index, json_field, field_desc.io_mode, field_desc.work_path, field_desc.raw_compress)
+            geo_index += num
+
+
+class InstancedStaticMeshField(Field):
+    """
+    _value is a InstanceStaticMesh
+    """
+    field_type_name = "paramType.InstancedStaticMesh"
+    support_param = False
+
+    def __init__(self, value):
+        self._value = value
+
+    @classmethod
+    def from_json(cls, json_object, input_name, field_desc:FieldDesc):
+        if field_desc.work_path is None:
+            raise Exception("HeightFieldField from_json failed:work path need to be set, not allowed")
+        value = InstancedStaticMesh.create_from_json(json_object, field_desc.work_path, field_desc.io_mode, input_name)
+        return InstancedStaticMeshField(value)
+
+    def get_input(self):
+        return self._value
+
+    def get_output(self, json_field, field_desc, data_field='Value Data', output_index=0):
+        geo_index = 0
+        self._value.to_json(geo_index, output_index, json_field, field_desc.io_mode, field_desc.work_path)
+
+
+class TextureField(Field):
+    """
+    _value is a Texture
+    """
+    field_type_name = "paramType.Texture"
+    support_param = False
+
+    def __init__(self, value=None):
+        self._value: Texture = value
+
+    @classmethod
+    def from_json(cls, json_object, input_name, field_desc: FieldDesc):
+        if field_desc.work_path is None:
+            raise Exception("TextureField from_json failed:work path need to be set, not allowed")
+        value = Texture.create_from_json(json_object, field_desc.work_path, field_desc.io_mode, field_desc.raw_compress, input_name)
+        return cls(value)
+
+    def get_input(self):
+        return self._value
+
+    def get_output(self, json_field, field_desc: FieldDesc, data_field='Value Data', output_index=0):
+        geo_index = 0
+        self._value.to_json(geo_index, output_index, json_field, field_desc.io_mode, field_desc.work_path, field_desc.raw_compress)
```

### Comparing `nextpcg-0.5.7/pypapi/meta_helper.py` & `nextpcg-0.5.8/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.7/pypapi/pantry/dson_generator.py` & `nextpcg-0.5.8/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.7/pypapi/plugin_protocol.py` & `nextpcg-0.5.8/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.7/setup.py` & `nextpcg-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.5.7',
+    version='0.5.8',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```

