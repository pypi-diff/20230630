# Comparing `tmp/assistant_improve_toolkit-1.3.9.tar.gz` & `tmp/assistant_improve_toolkit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant_improve_toolkit-1.3.9.tar", last modified: Thu Jun 22 21:07:54 2023, max compression
+gzip compressed data, was "assistant_improve_toolkit-1.4.0.tar", last modified: Fri Jun 30 14:33:41 2023, max compression
```

## Comparing `assistant_improve_toolkit-1.3.9.tar` & `assistant_improve_toolkit-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.376123 assistant_improve_toolkit-1.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.380123 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47406 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/computation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/cos_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (123)   109055 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/visualize_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/watson_assistant_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.380123 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.380123 assistant_improve_toolkit-1.3.9/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/src/main/python/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46395 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/computation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/cos_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/export_csv_for_intent_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)   107935 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/visualize_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func_skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.124699 assistant_improve_toolkit-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.128699 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47406 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/computation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/cos_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109055 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/visualize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/watson_assistant_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.128699 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.128699 assistant_improve_toolkit-1.4.0/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/src/main/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46395 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/computation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/cos_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/export_csv_for_intent_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107935 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/visualize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func_skip.py
```

### Comparing `assistant_improve_toolkit-1.3.9/LICENSE` & `assistant_improve_toolkit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/PKG-INFO` & `assistant_improve_toolkit-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant_improve_toolkit
-Version: 1.3.9
+Version: 1.4.0
 Summary: Assistant Improve Toolkit
 Home-page: https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 Maintainer: Zhe Zhang
 Maintainer-email: zhangzhe@us.ibm.com
 License: Apache 2.0
```

### Comparing `assistant_improve_toolkit-1.3.9/README.md` & `assistant_improve_toolkit-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/setup.py` & `assistant_improve_toolkit-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # Learn more about it at: http://github.com/fabiommendes/python-boilerplate/
 #
 
 import setuptools
 from os import path
 
-__version__ = '1.3.8'
+__version__ = '1.3.9'
 
 # read contents of README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as file:
     readme_file = file.read()
 
 setuptools.setup(
@@ -39,20 +39,20 @@
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     # Packages and depencies
     package_dir={'': 'src'},
     packages=setuptools.find_packages('src'),
     install_requires=[
         'pandas==1.2.1',
-        'bokeh==2.0.0',
-        'tqdm==4.43.0',
+        'bokeh==3.2.0',
+        'tqdm==4.65.0',
         'scikit-learn>=0.21.3',
         'matplotlib==3.2.1',
         'XlsxWriter==1.2.8',
-        'ibm-watson==5.1.0',
-        'numpy==1.25.0',
-        'requests==2.26'
+        'ibm-watson==7.0.0',
+        'numpy==1.23.5',
+        'requests==2.29.0'
     ],
 
     zip_safe=False,
     platforms='any',
 )
```

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/__init__.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/computation_func.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/computation_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/cos_op.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/cos_op.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/fetch_logs.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/visualize_func.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/visualize_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/watson_assistant_func.py` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/watson_assistant_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import pandas as pd
 import os
 import csv
 import traceback
 import io
 from string import punctuation
 
+from ibm_watson import AssistantV1, AssistantV2
 
 EN_PUNCTUATION = punctuation + '’'
 
 
 def get_assistant_definition(sdk_object, assistant_info, project=None, overwrite=False, filename='assistant_definition'):
     workspace_id, assistant_id, skill_id = [assistant_info.get(k) for k in ['workspace_id', 'assistant_id', 'skill_id']]
 
@@ -43,28 +44,47 @@
         with open(filename) as data:
             data_json = json.load(data)
         # Read logs into dataframe
         print('Assistant definition is loaded into as a dataframe.')
         df_assistant = pd.json_normalize(data_json)
         return df_assistant
     else:
-        if len(workspace_id) > 0:
-            # Fetch the workspace definition
-            print('Loading workspace definition using workspace id: {}'.format(workspace_id))
-            assistant_definition = sdk_object.get_workspace(workspace_id=workspace_id, export=True,
-                                                            include_audit=True).get_result()
-        elif len(skill_id) > 0:
-            # Fetch the skill definition
-            print('Loading skill definition using skill id: {}'.format(skill_id))
-            assistant_definition = sdk_object.get_workspace(workspace_id=skill_id, export=True,
-                                                            include_audit=True).get_result()
+        if type(sdk_object) == AssistantV1:
+            if len(workspace_id) > 0:
+                # Fetch the workspace definition
+                print('Loading workspace definition using workspace id: {}'.format(workspace_id))
+                assistant_definition = sdk_object.get_workspace(workspace_id=workspace_id, export=True,
+                                                                include_audit=True).get_result()
+            elif len(skill_id) > 0:
+                # Fetch the skill definition
+                print('Loading skill definition using skill id: {}'.format(skill_id))
+                assistant_definition = sdk_object.get_workspace(workspace_id=skill_id, export=True,
+                                                                include_audit=True).get_result()
+            else:
+                print('Please provide a valid Workspace ID or Skill ID!')
+                assistant_definition = None
+        elif type(sdk_object) == AssistantV2:
+            if len(assistant_id) > 0:
+                print('Loading skill definition using assistant id: {}'.format(assistant_id))
+                assistant_definition = None
+                assistants = sdk_object.export_skills(assistant_id=assistant_id, include_audit=True).get_result()
+                for assistant in assistants["assistant_skills"]:
+                    if assistant["type"] == "dialog":
+                        assistant_definition = assistant["workspace"]
+
+                if assistant_definition is None:
+                    print('Your assistant does not support dialog')
+            else:
+                print('Please provide a valid Assistant ID!')
+                assistant_definition = None
         else:
-            print('Please provide a valid Workspace ID or Skill ID!')
+            print("Please provide a valid watson sdk object")
             assistant_definition = None
 
+
         if assistant_definition:
             # Store the workspace details in a dataframe
             df_assistant = pd.json_normalize(assistant_definition)
 
             # Set `overwrite` to True for exporting assistant definition to json file
             if not os.path.isfile(filename) or overwrite:
                 if project is not None:
@@ -114,21 +134,21 @@
     except Exception as ex:
         traceback.print_tb(ex.__traceback__)
         raise RuntimeError("Error getting logs using API.  Please check if URL/credentials are correct.")
 
     return log_list
 
 
-def _get_logs_from_v2_api(sdk_object, assistant_id, log_filter, num_logs):
+def _get_logs_from_v2_api(sdk_object, environment_id, log_filter, num_logs):
     log_list = list()
     try:
         current_cursor = None
         while num_logs > 0:
             logs_response = sdk_object.list_logs(
-                    assistant_id=assistant_id,
+                    assistant_id=environment_id,
                     page_limit=500,
                     cursor=current_cursor,
                     filter=log_filter
                 ).get_result()
             min_num = min(num_logs, len(logs_response['logs']))
             log_list.extend(logs_response['logs'][:min_num])
             print('\r{} logs retrieved'.format(len(log_list)), end='')
@@ -163,15 +183,15 @@
        Returns
        ----------
        log_df : DataFrame of fetched logs
     """
     if filters is None:
         filters = []
 
-    workspace_id, assistant_id, skill_id = [assistant_info.get(k) for k in ['workspace_id', 'assistant_id', 'skill_id']]
+    workspace_id, assistant_id, skill_id, environment_id = [assistant_info.get(k) for k in ['workspace_id', 'assistant_id', 'skill_id', 'environment_id']]
 
     if (workspace_id is None or len(workspace_id) == 0) \
             and (assistant_id is None or len(assistant_id) == 0) \
             and (skill_id is None or len(skill_id) == 0):
         print('Please provide a valid Workspace ID, Assistant ID, or Skill ID!')
         return None
 
@@ -206,15 +226,15 @@
     if version == 1:
         logs = _get_logs_from_v1_api(sdk_object=sdk_v1_object,
                                      workspace_id=workspace_id,
                                      log_filter=','.join(filters),
                                      num_logs=num_logs)
     elif version == 2:
         logs = _get_logs_from_v2_api(sdk_object=sdk_v2_object,
-                                     assistant_id=assistant_id,
+                                     environment_id=environment_id,
                                      log_filter=','.join(filters),
                                      num_logs=num_logs)
     print('\nLoaded {} logs'.format(len(logs)))
 
     if not file_exist or overwrite:
         print('Saving {} logs into {}... '.format(len(logs), filename))
         if project:
```

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/PKG-INFO` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant-improve-toolkit
-Version: 1.3.9
+Version: 1.4.0
 Summary: Assistant Improve Toolkit
 Home-page: https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 Maintainer: Zhe Zhang
 Maintainer-email: zhangzhe@us.ibm.com
 License: Apache 2.0
```

### Comparing `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/SOURCES.txt` & `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/__init__.py` & `assistant_improve_toolkit-1.4.0/src/main/python/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/computation_func.py` & `assistant_improve_toolkit-1.4.0/src/main/python/computation_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/cos_op.py` & `assistant_improve_toolkit-1.4.0/src/main/python/cos_op.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/export_csv_for_intent_recommendation.py` & `assistant_improve_toolkit-1.4.0/src/main/python/export_csv_for_intent_recommendation.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/fetch_logs.py` & `assistant_improve_toolkit-1.4.0/src/main/python/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/visualize_func.py` & `assistant_improve_toolkit-1.4.0/src/main/python/visualize_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func.py` & `assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func_skip.py` & `assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func_skip.py`

 * *Files identical despite different names*

