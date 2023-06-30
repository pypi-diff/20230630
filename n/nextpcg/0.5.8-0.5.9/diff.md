# Comparing `tmp/nextpcg-0.5.8.tar.gz` & `tmp/nextpcg-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.8.tar", last modified: Fri Jun 30 06:04:40 2023, max compression
+gzip compressed data, was "nextpcg-0.5.9.tar", last modified: Fri Jun 30 07:05:33 2023, max compression
```

## Comparing `nextpcg-0.5.8.tar` & `nextpcg-0.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.543034 nextpcg-0.5.8/
--rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-06-30 06:04:40.543034 nextpcg-0.5.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.522014 nextpcg-0.5.8/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 06:04:40.000000 nextpcg-0.5.8/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.8/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.538030 nextpcg-0.5.8/pypapi/
--rw-rw-rw-   0        0        0       15 2023-06-30 03:01:10.000000 nextpcg-0.5.8/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.8/pypapi/const.py
--rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/dson.py
--rw-rw-rw-   0        0        0    10191 2023-06-30 03:23:16.000000 nextpcg-0.5.8/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    17451 2023-06-30 03:18:15.000000 nextpcg-0.5.8/pypapi/dson_field.py
--rw-rw-rw-   0        0        0    38443 2023-06-30 03:10:42.000000 nextpcg-0.5.8/pypapi/dson_geo.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.8/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.8/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:04:40.541032 nextpcg-0.5.8/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.8/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-06-30 06:04:40.544034 nextpcg-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-06-30 06:04:36.000000 nextpcg-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.769843 nextpcg-0.5.9/
+-rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-06-30 07:05:33.768842 nextpcg-0.5.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.741819 nextpcg-0.5.9/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 07:05:33.000000 nextpcg-0.5.9/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.9/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.762837 nextpcg-0.5.9/pypapi/
+-rw-rw-rw-   0        0        0       15 2023-06-30 03:01:10.000000 nextpcg-0.5.9/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     1995 2023-06-30 06:47:27.000000 nextpcg-0.5.9/pypapi/__main__.py
+-rw-rw-rw-   0        0        0     2129 2023-06-30 06:48:26.000000 nextpcg-0.5.9/pypapi/dson.py
+-rw-rw-rw-   0        0        0      470 2023-06-30 06:47:02.000000 nextpcg-0.5.9/pypapi/dson_const.py
+-rw-rw-rw-   0        0        0     8624 2023-06-30 06:48:46.000000 nextpcg-0.5.9/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    17451 2023-06-30 03:18:15.000000 nextpcg-0.5.9/pypapi/dson_field.py
+-rw-rw-rw-   0        0        0    38443 2023-06-30 03:10:42.000000 nextpcg-0.5.9/pypapi/dson_geo.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.9/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.9/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:05:33.766841 nextpcg-0.5.9/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.9/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.9/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.9/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:05:33.770844 nextpcg-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-06-30 07:05:20.000000 nextpcg-0.5.9/setup.py
```

### Comparing `nextpcg-0.5.8/PKG-INFO` & `nextpcg-0.5.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.8
+Version: 0.5.9
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.8/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.5.9/nextpcg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.8
+Version: 0.5.9
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.8/pypapi/__main__.py` & `nextpcg-0.5.9/pypapi/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import argparse
 import os
 import yaml
 import shutil
 from importlib_resources import files, as_file
 
+
 def entry():
     parser = argparse.ArgumentParser(prog = 'nextpcg')
     subparsers = parser.add_subparsers(
         title='These are common NextPCG Dson commands used in various situations',
         metavar='command'
     )
 
@@ -56,12 +57,10 @@
         yaml.safe_dump(dson_config, f, sort_keys=False)
         f.close()
     
     source = files('pypapi').joinpath('pantry').joinpath('dson_generator.py')
     with as_file(source) as source_path:
         shutil.copyfile(source_path,os.path.join(plugin_path, 'dson_generator.py'))
 
-    
-
 
 if __name__ == '__main__':
     entry()
```

### Comparing `nextpcg-0.5.8/pypapi/dson.py` & `nextpcg-0.5.9/pypapi/dson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Author  : NextPCG
 """
 
 from .meta_helper import Singleton
-from .const import *
+from .dson_const import *
 
 
 class nextpcgmethod(staticmethod):
     def __init__(self, function):
         super(nextpcgmethod, self).__init__(function)
```

### Comparing `nextpcg-0.5.8/pypapi/dson_create.py` & `nextpcg-0.5.9/pypapi/dson_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import os
 import json
 import logging
 
 from inspect import signature, Signature
 from functools import wraps
 from typing import *
-from .const import *
 from .dson import DsonMetaInfo, DsonManager, nextpcgmethod
+from .dson_const import *
 from .dson_field import Field, FieldCategory
 
 
 def create_dson_from_pda(func: Callable, tag, dson_meta_info: DsonMetaInfo) -> Dict:
     cda_json = {}
     try:
         func_sig = signature(func)
@@ -78,22 +78,22 @@
     with open(os.path.join(nextpcg_path, script_name), 'w', encoding='utf-8') as f:
         f.write(script_string)
 
 
 def generate_dson_main(base_path, dson_plugin_name, dson_config):
     # import info
     dsonmain_string1 = """
-                        from pypapi import Dispatcher
-                        from pypapi.plugin_protocol import module_send_done
-                        import sys
-                        import os
-                        import json
-                        import logging
+from pypapi.dispatch import Dispatcher
+from pypapi.plugin_protocol import module_send_done
+import sys
+import os
+import json
+import logging
 
-                        """
+"""
     # dsonmain_import contains code used to load necessary modules or classes
     dsonmain_import = ''
     for module in dson_config['modules']:
         if isinstance(module, str):
             # only module name
             try:
                 dsonmain_import += 'import ' + module + '\n'
@@ -106,83 +106,83 @@
                 dsonmain_import += 'from ' + module_name + ' import  '
                 for class_name in module[module_name]:
                     dsonmain_import += class_name + ','
                 dsonmain_import = dsonmain_import[:-1]
     # code
     dsonmain_string2 = f"""
 
-                        dson_plugin_name = '{dson_plugin_name}'
-                        dispatcher = Dispatcher()
-                        logger = logging.getLogger('pypapi_'+dson_plugin_name)
-                        current_path = os.path.split(os.path.realpath(__file__))[0] # path to dosn_path.py
-                        dot_nextpcg_path = os.path.join(current_path, '.nextpcg')
-
-                        def set_up_logger():
-                            logFormatter = logging.Formatter('%(levelname)s:%(name)s:[%(asctime)s]: %(message)s')
-
-                            if not os.path.exists(dot_nextpcg_path):
-                                os.makedirs(dot_nextpcg_path)
-
-                            logfile_path = os.path.join(current_path, '.nextpcg', 'nextpcgpython.log')
-                            # delete old log file
-                            try:
-                                os.remove(logfile_path)
-                            except OSError:
-                                pass
-
-                            fileHandler = logging.FileHandler(logfile_path)
-                            fileHandler.setFormatter(logFormatter)
-
-                            consoleHandler = logging.StreamHandler()
-                            consoleHandler.setFormatter(logFormatter)
-
-                            logger.addHandler(fileHandler)
-                            logger.addHandler(consoleHandler)
-
-                        class Tee:
-                            def __init__(self, *files):
-                                self.files = files
-
-                            def write(self, obj):
-                                for f in self.files:
-                                    f.write(obj)
-                                    f.flush()
-
-                            def flush(self):
-                                for f in self.files:
-                                    f.flush()
-
-                        if __name__ == '__main__':
-                            set_up_logger()
-                            ferr = open(os.path.join(dot_nextpcg_path, 'err.txt'), 'w')
-                            sys.stderr = Tee(sys.stderr,ferr)
-                            module_send_done()
-                            while(True):
-                                json_file_name, work_path = input().split()
-                                json_error_data = {{}}
-                                try:
-                                    with open(json_file_name, 'r') as f:
-                                        json_data = json.load(f)
-                                    if not json_data:
-                                        print("didn't get dson data")
-                                        module_send_done()
-                                    dispatcher.run_func(json_data, logger, work_path, json_error_data)
-                                    json_data_error_file_name = os.path.join(work_path, 'error.json').replace("\\\\",'/')
-                                    # write back json_data
-                                    with open(json_file_name, 'w') as f:
-                                        json.dump(json_data, f)
-                                except Exception as e:
-                                    json_error_data['Error_Tag'] = 'plugin {dson_plugin_name} error in main loop'
-                                    json_error_data['Error_Info'] = str(e)
-                                    logger.exception(e)
-                                finally:
-                                    with open(json_data_error_file_name, 'w') as f:
-                                        json_error_data = json.dump(json_error_data, f)
-                                module_send_done()
-                        """
+dson_plugin_name = '{dson_plugin_name}'
+dispatcher = Dispatcher()
+logger = logging.getLogger('pypapi_'+dson_plugin_name)
+current_path = os.path.split(os.path.realpath(__file__))[0] # path to dosn_path.py
+dot_nextpcg_path = os.path.join(current_path, '.nextpcg')
+
+def set_up_logger():
+    logFormatter = logging.Formatter('%(levelname)s:%(name)s:[%(asctime)s]: %(message)s')
+
+    if not os.path.exists(dot_nextpcg_path):
+        os.makedirs(dot_nextpcg_path)
+
+    logfile_path = os.path.join(current_path, '.nextpcg', 'nextpcgpython.log')
+    # delete old log file
+    try:
+        os.remove(logfile_path)
+    except OSError:
+        pass
+
+    fileHandler = logging.FileHandler(logfile_path)
+    fileHandler.setFormatter(logFormatter)
+
+    consoleHandler = logging.StreamHandler()
+    consoleHandler.setFormatter(logFormatter)
+
+    logger.addHandler(fileHandler)
+    logger.addHandler(consoleHandler)
+
+class Tee:
+    def __init__(self, *files):
+        self.files = files
+
+    def write(self, obj):
+        for f in self.files:
+            f.write(obj)
+            f.flush()
+
+    def flush(self):
+        for f in self.files:
+            f.flush()
+
+if __name__ == '__main__':
+    set_up_logger()
+    ferr = open(os.path.join(dot_nextpcg_path, 'err.txt'), 'w')
+    sys.stderr = Tee(sys.stderr,ferr)
+    module_send_done()
+    while(True):
+        json_file_name, work_path = input().split()
+        json_error_data = {{}}
+        try:
+            with open(json_file_name, 'r') as f:
+                json_data = json.load(f)
+            if not json_data:
+                print("didn't get dson data")
+                module_send_done()
+            dispatcher.run_func(json_data, logger, work_path, json_error_data)
+            json_data_error_file_name = os.path.join(work_path, 'error.json').replace("\\\\",'/')
+            # write back json_data
+            with open(json_file_name, 'w') as f:
+                json.dump(json_data, f)
+        except Exception as e:
+            json_error_data['Error_Tag'] = 'plugin {dson_plugin_name} error in main loop'
+            json_error_data['Error_Info'] = str(e)
+            logger.exception(e)
+        finally:
+            with open(json_data_error_file_name, 'w') as f:
+                json_error_data = json.dump(json_error_data, f)
+        module_send_done()
+"""
     dsonmain_string = dsonmain_string1 + dsonmain_import + dsonmain_string2
     with open(os.path.join(base_path, 'dson_main.py'), 'w', encoding='utf-8') as f:
         f.write(dsonmain_string)
 
 
 def get_inputs(sig: Signature):
     inputs = {}
@@ -227,16 +227,15 @@
 
 def get_doc(sig: Callable):
     return sig.__doc__
 
 
 # for test
 if __name__ == "__main__":
-    from field import Int, Int2, String, ListField
-
+    from dson_field import Int, Int2, String, ListField
 
     def foo(a: Int, b: ListField[Int2] = [1, 2], c: Int2 = (1, 2)) -> String:
         pass
 
 
     jj = create_dson_from_pda(foo)
     file_path = "test.json"
```

### Comparing `nextpcg-0.5.8/pypapi/dson_field.py` & `nextpcg-0.5.9/pypapi/dson_field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.8/pypapi/dson_geo.py` & `nextpcg-0.5.9/pypapi/dson_geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.8/pypapi/meta_helper.py` & `nextpcg-0.5.9/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.8/pypapi/pantry/dson_generator.py` & `nextpcg-0.5.9/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.8/pypapi/plugin_protocol.py` & `nextpcg-0.5.9/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.8/setup.py` & `nextpcg-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.5.8',
+    version='0.5.9',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```

