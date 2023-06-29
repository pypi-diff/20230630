# Comparing `tmp/lollms-2.1.6.tar.gz` & `tmp/lollms-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.1.6.tar", last modified: Thu Jun 29 21:53:57 2023, max compression
+gzip compressed data, was "lollms-2.1.7.tar", last modified: Thu Jun 29 21:59:27 2023, max compression
```

## Comparing `lollms-2.1.6.tar` & `lollms-2.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:53:57.548527 lollms-2.1.6/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.6/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:53:57.548527 lollms-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 21:53:57.529638 lollms-2.1.6/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.6/lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:53:57.544638 lollms-2.1.6/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.6/lollms/assets/logo.png
--rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.6/lollms/binding.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.6/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:53:57.546636 lollms-2.1.6/lollms/configs/
--rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.6/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0    30469 2023-06-29 21:53:18.000000 lollms-2.1.6/lollms/console.py
--rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.6/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.6/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.6/lollms/main_config.py
--rw-rw-rw-   0        0        0    13160 2023-06-29 21:38:33.000000 lollms-2.1.6/lollms/paths.py
--rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.6/lollms/personality.py
--rw-rw-rw-   0        0        0    32676 2023-06-29 21:53:18.000000 lollms-2.1.6/lollms/server.py
--rw-rw-rw-   0        0        0    11084 2023-06-29 21:53:44.000000 lollms-2.1.6/lollms/settings.py
--rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.6/lollms/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:53:57.543639 lollms-2.1.6/lollms.egg-info/
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:53:57.000000 lollms-2.1.6/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-29 21:53:57.000000 lollms-2.1.6/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:53:57.000000 lollms-2.1.6/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-06-29 21:53:57.000000 lollms-2.1.6/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-06-29 21:53:57.000000 lollms-2.1.6/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 21:53:57.000000 lollms-2.1.6/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 21:53:57.548527 lollms-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1792 2023-06-29 21:53:53.000000 lollms-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.334417 lollms-2.1.7/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    11117 2023-06-29 21:59:27.334417 lollms-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.312787 lollms-2.1.7/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.7/lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.329721 lollms-2.1.7/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.7/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.7/lollms/binding.py
+-rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.7/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.332406 lollms-2.1.7/lollms/configs/
+-rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.7/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0    30469 2023-06-29 21:53:18.000000 lollms-2.1.7/lollms/console.py
+-rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.7/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.7/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.7/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13221 2023-06-29 21:59:06.000000 lollms-2.1.7/lollms/paths.py
+-rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.7/lollms/personality.py
+-rw-rw-rw-   0        0        0    32676 2023-06-29 21:53:18.000000 lollms-2.1.7/lollms/server.py
+-rw-rw-rw-   0        0        0    11084 2023-06-29 21:53:44.000000 lollms-2.1.7/lollms/settings.py
+-rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.7/lollms/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.328721 lollms-2.1.7/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11117 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      184 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:59:27.334417 lollms-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2023-06-29 21:59:24.000000 lollms-2.1.7/setup.py
```

### Comparing `lollms-2.1.6/LICENSE` & `lollms-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/PKG-INFO` & `lollms-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.6
+Version: 2.1.7
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.6/README.md` & `lollms-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/assets/logo.png` & `lollms-2.1.7/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/binding.py` & `lollms-2.1.7/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/config.py` & `lollms-2.1.7/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/configs/config.yaml` & `lollms-2.1.7/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/console.py` & `lollms-2.1.7/lollms/console.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/helpers.py` & `lollms-2.1.7/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/langchain_integration.py` & `lollms-2.1.7/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/main_config.py` & `lollms-2.1.7/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/paths.py` & `lollms-2.1.7/lollms/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                     pp.mkdir(parents=True)
                 except:
                     print(f"{ASCIIColors.color_red}It seams there is an error in the path you rovided{ASCIIColors.color_reset}")
                     continue
             if force_local:
                 global_paths_cfg_path = Path(f"./{self.tool_prefix}global_paths_cfg.yaml")
             else:
-                global_paths_cfg_path = Path.home()/"global_paths_cfg.yaml"
+                global_paths_cfg_path = Path.home()/f"{self.tool_prefix}global_paths_cfg.yaml"
             cfg.save_config(global_paths_cfg_path)
             found = True
         
         return LollmsPaths(global_paths_cfg_path, cfg.lollms_path, cfg.lollms_personal_path, custom_default_cfg_path=custom_default_cfg_path)        
 
     @staticmethod
     def find_paths(force_local=False, custom_default_cfg_path=None, tool_prefix=""):
@@ -160,15 +160,15 @@
                     cfg.lollms_personal_path=lollms_personal_path
                 cfg.save_config(global_paths_cfg_path)
                 lollms_path = cfg.lollms_path
                 lollms_personal_path = cfg.lollms_personal_path
                 return LollmsPaths(global_paths_cfg_path, lollms_path, lollms_personal_path, custom_default_cfg_path=custom_default_cfg_path, tool_prefix=tool_prefix)
         else:
             # if the app is not forcing a specific path, then try to find out if the default installed library has specified a default path
-            global_paths_cfg_path = Path.home()/"global_paths_cfg.yaml"
+            global_paths_cfg_path = Path.home()/f"{tool_prefix}global_paths_cfg.yaml"
             if global_paths_cfg_path.exists():
                 cfg = BaseConfig()
                 cfg.load_config(global_paths_cfg_path)
                 try:
                     lollms_path = cfg.lollms_path
                     lollms_personal_path = cfg.lollms_personal_path
                     return LollmsPaths(global_paths_cfg_path, lollms_path, lollms_personal_path, custom_default_cfg_path=custom_default_cfg_path, tool_prefix=tool_prefix)
@@ -204,28 +204,28 @@
                             pp.mkdir(parents=True)
                         except:
                             print(f"{ASCIIColors.color_red}It seams there is an error in the path you rovided{ASCIIColors.color_reset}")
                             continue
                     if force_local:
                         global_paths_cfg_path = Path(f"./{tool_prefix}global_paths_cfg.yaml")
                     else:
-                        global_paths_cfg_path = Path.home()/"global_paths_cfg.yaml"
+                        global_paths_cfg_path = Path.home()/f"{tool_prefix}global_paths_cfg.yaml"
                     cfg.save_config(global_paths_cfg_path)
                     found = True
                 
                 return LollmsPaths(global_paths_cfg_path, cfg.lollms_path, cfg.lollms_personal_path, custom_default_cfg_path=custom_default_cfg_path, tool_prefix=tool_prefix)
             
             
     @staticmethod     
     def reset_configs(tool_prefix=""):
         lollms_path = Path(__file__).parent
         global_paths_cfg_path = Path(f"./{tool_prefix}global_paths_cfg.yaml")
         if global_paths_cfg_path.exists():
             ASCIIColors.error("Resetting local settings")
             global_paths_cfg_path.unlink()
             return
-        global_paths_cfg_path = Path.home()/"global_paths_cfg.yaml"
+        global_paths_cfg_path = Path.home()/f"{tool_prefix}global_paths_cfg.yaml"
         if global_paths_cfg_path.exists():
             ASCIIColors.error("Resetting global settings")
             global_paths_cfg_path.unlink()
```

### Comparing `lollms-2.1.6/lollms/personality.py` & `lollms-2.1.7/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/server.py` & `lollms-2.1.7/lollms/server.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/settings.py` & `lollms-2.1.7/lollms/settings.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms/types.py` & `lollms-2.1.7/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.6/lollms.egg-info/PKG-INFO` & `lollms-2.1.7/lollms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.6
+Version: 2.1.7
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.6/setup.py` & `lollms-2.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.1.6",
+    version="2.1.7",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

