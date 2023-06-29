# Comparing `tmp/lollms-2.1.8.tar.gz` & `tmp/lollms-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.1.8.tar", last modified: Thu Jun 29 22:05:13 2023, max compression
+gzip compressed data, was "lollms-2.1.9.tar", last modified: Thu Jun 29 22:22:46 2023, max compression
```

## Comparing `lollms-2.1.8.tar` & `lollms-2.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.573388 lollms-2.1.8/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.8/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    11117 2023-06-29 22:05:13.573388 lollms-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.553093 lollms-2.1.8/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.8/lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.570387 lollms-2.1.8/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.8/lollms/assets/logo.png
--rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.8/lollms/binding.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.8/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.572384 lollms-2.1.8/lollms/configs/
--rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.8/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0    30470 2023-06-29 22:04:08.000000 lollms-2.1.8/lollms/console.py
--rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.8/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.8/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.8/lollms/main_config.py
--rw-rw-rw-   0        0        0    13221 2023-06-29 21:59:06.000000 lollms-2.1.8/lollms/paths.py
--rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.8/lollms/personality.py
--rw-rw-rw-   0        0        0    32680 2023-06-29 22:04:29.000000 lollms-2.1.8/lollms/server.py
--rw-rw-rw-   0        0        0    11120 2023-06-29 22:05:02.000000 lollms-2.1.8/lollms/settings.py
--rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.8/lollms/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.569390 lollms-2.1.8/lollms.egg-info/
--rw-rw-rw-   0        0        0    11117 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 22:05:13.574384 lollms-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1792 2023-06-29 22:05:11.000000 lollms-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.756621 lollms-2.1.9/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-06-29 22:22:46.756621 lollms-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.727621 lollms-2.1.9/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.9/lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.751620 lollms-2.1.9/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.9/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.9/lollms/binding.py
+-rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.9/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.754619 lollms-2.1.9/lollms/configs/
+-rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.9/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0    30470 2023-06-29 22:04:08.000000 lollms-2.1.9/lollms/console.py
+-rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.9/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.9/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.9/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13221 2023-06-29 21:59:06.000000 lollms-2.1.9/lollms/paths.py
+-rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.9/lollms/personality.py
+-rw-rw-rw-   0        0        0    32664 2023-06-29 22:21:42.000000 lollms-2.1.9/lollms/server.py
+-rw-rw-rw-   0        0        0    11120 2023-06-29 22:05:02.000000 lollms-2.1.9/lollms/settings.py
+-rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.9/lollms/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:22:46.750618 lollms-2.1.9/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      184 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 22:22:46.000000 lollms-2.1.9/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:22:46.756621 lollms-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2023-06-29 22:22:34.000000 lollms-2.1.9/setup.py
```

### Comparing `lollms-2.1.8/LICENSE` & `lollms-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/PKG-INFO` & `lollms-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.8
+Version: 2.1.9
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -288,9 +286,7 @@
 ## License
 
 LoLLMs Server is licensed under the Apache 2.0 License. See the [LICENSE](https://github.com/ParisNeo/lollms/blob/main/LICENSE) file for more information.
 
 ## Repository
 
 The source code for LoLLMs Server can be found on GitHub
-
-
```

### Comparing `lollms-2.1.8/README.md` & `lollms-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/assets/logo.png` & `lollms-2.1.9/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/binding.py` & `lollms-2.1.9/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/config.py` & `lollms-2.1.9/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/configs/config.yaml` & `lollms-2.1.9/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/console.py` & `lollms-2.1.9/lollms/console.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/helpers.py` & `lollms-2.1.9/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/langchain_integration.py` & `lollms-2.1.9/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/main_config.py` & `lollms-2.1.9/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/paths.py` & `lollms-2.1.9/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/personality.py` & `lollms-2.1.9/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/server.py` & `lollms-2.1.9/lollms/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                             help='The path to the Bindings folder')
         parser.add_argument('--personalities_path', '-pp',
                             default=str(self.lollms_paths.personalities_zoo_path),
                             help='The path to the personalities folder')
         parser.add_argument('--models_path', '-mp', default=str(self.lollms_paths.personal_models_path),
                             help='The path to the models folder')
 
-        parser.add_argument('--binding_name', '-b', default="llama_cpp_official",
+        parser.add_argument('--binding_name', '-b', default=None,
                             help='Binding to be used by default')
         parser.add_argument('--model_name', '-m', default=None,
                             help='Model name')
         parser.add_argument('--personality_full_name', '-p', default="personality",
                             help='Personality path relative to the personalities folder (language/category/name)')
         
         parser.add_argument('--reset_personal_path', action='store_true', help='Reset the personal path')
```

### Comparing `lollms-2.1.8/lollms/settings.py` & `lollms-2.1.9/lollms/settings.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms/types.py` & `lollms-2.1.9/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.8/lollms.egg-info/PKG-INFO` & `lollms-2.1.9/lollms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.8
+Version: 2.1.9
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -288,9 +286,7 @@
 ## License
 
 LoLLMs Server is licensed under the Apache 2.0 License. See the [LICENSE](https://github.com/ParisNeo/lollms/blob/main/LICENSE) file for more information.
 
 ## Repository
 
 The source code for LoLLMs Server can be found on GitHub
-
-
```

### Comparing `lollms-2.1.8/setup.py` & `lollms-2.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.1.8",
+    version="2.1.9",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

