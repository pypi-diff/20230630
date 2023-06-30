# Comparing `tmp/JsonDecoder-0.0.8.tar.gz` & `tmp/JsonDecoder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonDecoder-0.0.8.tar", last modified: Thu Nov 17 13:36:07 2022, max compression
+gzip compressed data, was "JsonDecoder-0.0.9.tar", last modified: Mon Jan  2 15:52:30 2023, max compression
```

## Comparing `JsonDecoder-0.0.8.tar` & `JsonDecoder-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 philips    (503) staff       (20)        0 2022-11-17 13:36:07.528498 JsonDecoder-0.0.8/
-drwxr-xr-x   0 philips    (503) staff       (20)        0 2022-11-17 13:36:07.522980 JsonDecoder-0.0.8/JsonDecoder.egg-info/
--rw-r--r--   0 philips    (503) staff       (20)      918 2022-11-17 13:36:07.000000 JsonDecoder-0.0.8/JsonDecoder.egg-info/PKG-INFO
--rw-r--r--   0 philips    (503) staff       (20)      367 2022-11-17 13:36:07.000000 JsonDecoder-0.0.8/JsonDecoder.egg-info/SOURCES.txt
--rw-r--r--   0 philips    (503) staff       (20)        1 2022-11-17 13:36:07.000000 JsonDecoder-0.0.8/JsonDecoder.egg-info/dependency_links.txt
--rw-r--r--   0 philips    (503) staff       (20)       13 2022-11-17 13:36:07.000000 JsonDecoder-0.0.8/JsonDecoder.egg-info/top_level.txt
--rw-r--r--   0 philips    (503) staff       (20)     1069 2022-07-19 09:08:14.000000 JsonDecoder-0.0.8/LICENSE
--rw-r--r--   0 philips    (503) staff       (20)      918 2022-11-17 13:36:07.528200 JsonDecoder-0.0.8/PKG-INFO
--rw-r--r--   0 philips    (503) staff       (20)      171 2022-09-14 16:17:57.000000 JsonDecoder-0.0.8/README.md
-drwxr-xr-x   0 philips    (503) staff       (20)        0 2022-11-17 13:36:07.524476 JsonDecoder-0.0.8/json_decoder/
--rw-r--r--   0 philips    (503) staff       (20)      102 2022-09-14 17:51:23.000000 JsonDecoder-0.0.8/json_decoder/__init__.py
-drwxr-xr-x   0 philips    (503) staff       (20)        0 2022-11-17 13:36:07.525692 JsonDecoder-0.0.8/json_decoder/classes/
--rw-r--r--   0 philips    (503) staff       (20)      107 2022-09-14 17:18:42.000000 JsonDecoder-0.0.8/json_decoder/classes/__init__.py
--rw-r--r--   0 philips    (503) staff       (20)     3081 2022-11-17 13:35:19.000000 JsonDecoder-0.0.8/json_decoder/classes/jsondecoder.py
--rw-r--r--   0 philips    (503) staff       (20)      103 2022-07-19 11:38:28.000000 JsonDecoder-0.0.8/json_decoder/exceptions.py
-drwxr-xr-x   0 philips    (503) staff       (20)        0 2022-11-17 13:36:07.526934 JsonDecoder-0.0.8/json_decoder/tests/
--rw-r--r--   0 philips    (503) staff       (20)        0 2022-07-19 11:39:32.000000 JsonDecoder-0.0.8/json_decoder/tests/__init__.py
-drwxr-xr-x   0 philips    (503) staff       (20)        0 2022-11-17 13:36:07.527728 JsonDecoder-0.0.8/json_decoder/tests/test_json_decoder/
--rw-r--r--   0 philips    (503) staff       (20)        0 2022-07-19 11:39:32.000000 JsonDecoder-0.0.8/json_decoder/tests/test_json_decoder/__init__.py
--rw-r--r--   0 philips    (503) staff       (20)       38 2022-11-17 13:36:07.528610 JsonDecoder-0.0.8/setup.cfg
--rw-r--r--   0 philips    (503) staff       (20)     1387 2022-11-17 13:35:29.000000 JsonDecoder-0.0.8/setup.py
+drwxr-xr-x   0 philips    (503) staff       (20)        0 2023-01-02 15:52:30.555780 JsonDecoder-0.0.9/
+drwxr-xr-x   0 philips    (503) staff       (20)        0 2023-01-02 15:52:30.544799 JsonDecoder-0.0.9/JsonDecoder.egg-info/
+-rw-r--r--   0 philips    (503) staff       (20)      918 2023-01-02 15:52:30.000000 JsonDecoder-0.0.9/JsonDecoder.egg-info/PKG-INFO
+-rw-r--r--   0 philips    (503) staff       (20)      423 2023-01-02 15:52:30.000000 JsonDecoder-0.0.9/JsonDecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 philips    (503) staff       (20)        1 2023-01-02 15:52:30.000000 JsonDecoder-0.0.9/JsonDecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 philips    (503) staff       (20)       13 2023-01-02 15:52:30.000000 JsonDecoder-0.0.9/JsonDecoder.egg-info/top_level.txt
+-rw-r--r--   0 philips    (503) staff       (20)     1069 2022-07-19 09:08:14.000000 JsonDecoder-0.0.9/LICENSE
+-rw-r--r--   0 philips    (503) staff       (20)      918 2023-01-02 15:52:30.555377 JsonDecoder-0.0.9/PKG-INFO
+-rw-r--r--   0 philips    (503) staff       (20)      171 2022-09-14 16:17:57.000000 JsonDecoder-0.0.9/README.md
+drwxr-xr-x   0 philips    (503) staff       (20)        0 2023-01-02 15:52:30.546989 JsonDecoder-0.0.9/json_decoder/
+-rw-r--r--   0 philips    (503) staff       (20)      102 2022-09-14 17:51:23.000000 JsonDecoder-0.0.9/json_decoder/__init__.py
+drwxr-xr-x   0 philips    (503) staff       (20)        0 2023-01-02 15:52:30.550739 JsonDecoder-0.0.9/json_decoder/classes/
+-rw-r--r--   0 philips    (503) staff       (20)      107 2022-09-14 17:18:42.000000 JsonDecoder-0.0.9/json_decoder/classes/__init__.py
+-rw-r--r--   0 philips    (503) staff       (20)     3993 2023-01-02 15:48:23.000000 JsonDecoder-0.0.9/json_decoder/classes/jsondecoder.py
+-rw-r--r--   0 philips    (503) staff       (20)      103 2022-07-19 11:38:28.000000 JsonDecoder-0.0.9/json_decoder/exceptions.py
+drwxr-xr-x   0 philips    (503) staff       (20)        0 2023-01-02 15:52:30.552039 JsonDecoder-0.0.9/json_decoder/tests/
+-rw-r--r--   0 philips    (503) staff       (20)        0 2022-07-19 11:39:32.000000 JsonDecoder-0.0.9/json_decoder/tests/__init__.py
+drwxr-xr-x   0 philips    (503) staff       (20)        0 2023-01-02 15:52:30.554023 JsonDecoder-0.0.9/json_decoder/tests/test_json_decoder/
+-rw-r--r--   0 philips    (503) staff       (20)        0 2022-07-19 11:39:32.000000 JsonDecoder-0.0.9/json_decoder/tests/test_json_decoder/__init__.py
+-rw-r--r--   0 philips    (503) staff       (20)      276 2023-01-02 12:52:03.000000 JsonDecoder-0.0.9/json_decoder/tests/test_json_decoder/test_jsonParser.py
+-rw-r--r--   0 philips    (503) staff       (20)       38 2023-01-02 15:52:30.555934 JsonDecoder-0.0.9/setup.cfg
+-rw-r--r--   0 philips    (503) staff       (20)     1387 2023-01-02 15:50:36.000000 JsonDecoder-0.0.9/setup.py
```

### Comparing `JsonDecoder-0.0.8/JsonDecoder.egg-info/PKG-INFO` & `JsonDecoder-0.0.9/JsonDecoder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonDecoder
-Version: 0.0.8
+Version: 0.0.9
 Summary: json parser framework for Python
 Home-page: https://github.com/sheikhjebran/jsonparser
 Author: Sheikh Jebran
 Author-email: sheikhjebran@gmail.com
 License: MIT License
 Keywords: json python json parser json parser parser json python decover
 Platform: UNKNOWN
```

### Comparing `JsonDecoder-0.0.8/LICENSE` & `JsonDecoder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonDecoder-0.0.8/PKG-INFO` & `JsonDecoder-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JsonDecoder
-Version: 0.0.8
+Version: 0.0.9
 Summary: json parser framework for Python
 Home-page: https://github.com/sheikhjebran/jsonparser
 Author: Sheikh Jebran
 Author-email: sheikhjebran@gmail.com
 License: MIT License
 Keywords: json python json parser json parser parser json python decover
 Platform: UNKNOWN
```

### Comparing `JsonDecoder-0.0.8/json_decoder/classes/jsondecoder.py` & `JsonDecoder-0.0.9/json_decoder/classes/jsondecoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,14 +54,16 @@
             setattr(self, f"{data}", data)
 
     def get_data(self):
         f = open(self.json_path, 'r')
         data = json.load(f)
         if isinstance(data, dict):
             self.my_dict(data)
+        if isinstance(data, list) or isinstance(data,tuple):
+            self.my_list(data)
         if isinstance(data, str)or isinstance(data, int) or isinstance(data, float) or isinstance(data,bool):
             setattr(self, f"{data}", data)
 
     def my_dict(self, data):
 
         for k, v in data.items():
             if isinstance(v, str)or isinstance(v, int) or isinstance(v, float) or isinstance(v,bool):
@@ -71,21 +73,39 @@
                 my_dict.set_attribute(v)
                 setattr(self, f"{k}", my_dict)
             elif isinstance(v, list):
                 my_list = List()
                 my_list_data = my_list.set_attribute(data=v, parent=k)
                 setattr(self, f"{k}", my_list_data)
 
+    def my_list(self, data,parent=None):
+        self.temp_list = []
+        for iteam in data:
+            if isinstance(iteam, str) or isinstance(iteam, int) or isinstance(iteam, float) or isinstance(iteam, bool):
+                self.temp_list.append(iteam)
+            elif isinstance(iteam, dict):
+                my_dict = Dict()
+                my_dict.set_attribute(iteam)
+                self.temp_list.append(my_dict)
+            elif isinstance(iteam, list):
+                my_list = List()
+                self.temp_list.append(my_list.set_attribute(data=iteam, parent=f"{parent}+counter"))
+
+        if len(self.temp_list) > 0:
+            if parent is None:
+                setattr(self, f"{0}", self.temp_list)
+            else:
+                setattr(self, f"{parent}", self.temp_list)
 
 class JsonParser:
 
     @staticmethod
-    def parserJson(json_object, filepath=False):
+    def parserJson(json_object):
         json_decoder = JsonDecoder()
         try:
-            if not filepath:
+            if json_object[len(json_object) - 5:] != ".json":
                 json_decoder.read_string(json_object)
             else:
                 json_decoder.read_json_file(json_object)
             return json_decoder
         except Exception:
             raise TypeError("Object type is not supported")
```

### Comparing `JsonDecoder-0.0.8/setup.py` & `JsonDecoder-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name='JsonDecoder',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[],
     license='MIT License',
     description='json parser framework for Python',
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
```

