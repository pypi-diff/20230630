# Comparing `tmp/lollms-2.1.7.tar.gz` & `tmp/lollms-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.1.7.tar", last modified: Thu Jun 29 21:59:27 2023, max compression
+gzip compressed data, was "lollms-2.1.8.tar", last modified: Thu Jun 29 22:05:13 2023, max compression
```

## Comparing `lollms-2.1.7.tar` & `lollms-2.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.334417 lollms-2.1.7/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.7/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:59:27.334417 lollms-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.312787 lollms-2.1.7/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.7/lollms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.329721 lollms-2.1.7/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.7/lollms/assets/logo.png
--rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.7/lollms/binding.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.7/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.332406 lollms-2.1.7/lollms/configs/
--rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.7/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0    30469 2023-06-29 21:53:18.000000 lollms-2.1.7/lollms/console.py
--rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.7/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.7/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.7/lollms/main_config.py
--rw-rw-rw-   0        0        0    13221 2023-06-29 21:59:06.000000 lollms-2.1.7/lollms/paths.py
--rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.7/lollms/personality.py
--rw-rw-rw-   0        0        0    32676 2023-06-29 21:53:18.000000 lollms-2.1.7/lollms/server.py
--rw-rw-rw-   0        0        0    11084 2023-06-29 21:53:44.000000 lollms-2.1.7/lollms/settings.py
--rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.7/lollms/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 21:59:27.328721 lollms-2.1.7/lollms.egg-info/
--rw-rw-rw-   0        0        0    11117 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      184 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 21:59:27.000000 lollms-2.1.7/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 21:59:27.334417 lollms-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1792 2023-06-29 21:59:24.000000 lollms-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.573388 lollms-2.1.8/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-29 21:31:56.000000 lollms-2.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    11117 2023-06-29 22:05:13.573388 lollms-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.553093 lollms-2.1.8/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.1.8/lollms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.570387 lollms-2.1.8/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.1.8/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0     9914 2023-06-25 17:30:21.000000 lollms-2.1.8/lollms/binding.py
+-rw-rw-rw-   0        0        0    21424 2023-06-22 15:34:05.000000 lollms-2.1.8/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.572384 lollms-2.1.8/lollms/configs/
+-rw-rw-rw-   0        0        0      651 2023-06-25 11:51:47.000000 lollms-2.1.8/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0    30470 2023-06-29 22:04:08.000000 lollms-2.1.8/lollms/console.py
+-rw-rw-rw-   0        0        0     2613 2023-06-20 17:34:25.000000 lollms-2.1.8/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.1.8/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-06-29 21:40:56.000000 lollms-2.1.8/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13221 2023-06-29 21:59:06.000000 lollms-2.1.8/lollms/paths.py
+-rw-rw-rw-   0        0        0    38528 2023-06-28 21:28:43.000000 lollms-2.1.8/lollms/personality.py
+-rw-rw-rw-   0        0        0    32680 2023-06-29 22:04:29.000000 lollms-2.1.8/lollms/server.py
+-rw-rw-rw-   0        0        0    11120 2023-06-29 22:05:02.000000 lollms-2.1.8/lollms/settings.py
+-rw-rw-rw-   0        0        0     1127 2023-06-28 21:31:20.000000 lollms-2.1.8/lollms/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 22:05:13.569390 lollms-2.1.8/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11117 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      184 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 22:05:13.000000 lollms-2.1.8/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:05:13.574384 lollms-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2023-06-29 22:05:11.000000 lollms-2.1.8/setup.py
```

### Comparing `lollms-2.1.7/LICENSE` & `lollms-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/PKG-INFO` & `lollms-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.7
+Version: 2.1.8
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.7/README.md` & `lollms-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/assets/logo.png` & `lollms-2.1.8/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/binding.py` & `lollms-2.1.8/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/config.py` & `lollms-2.1.8/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/configs/config.yaml` & `lollms-2.1.8/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/console.py` & `lollms-2.1.8/lollms/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def reset_paths(lollms_paths:LollmsPaths):
     lollms_paths.resetPaths()
 
 def reset_all_installs(lollms_paths:LollmsPaths):
     ASCIIColors.info("Removeing all configuration files to force reinstall")
     ASCIIColors.info(f"Searching files from {lollms_paths.personal_configuration_path}")
     for file_path in lollms_paths.personal_configuration_path.iterdir():
-        if file_path.name!=lollms_paths.tool_prefix+"local_config.yaml" and file_path.suffix.lower()==".yaml":
+        if file_path.name!=f"{lollms_paths.tool_prefix}local_config.yaml" and file_path.suffix.lower()==".yaml":
             file_path.unlink()
             ASCIIColors.info(f"Deleted file: {file_path}")
 
 class MainMenu:
     def __init__(self, lollms_app:LollmsApplication):
         self.binding_infs = []
         self.lollms_app = lollms_app
@@ -607,16 +607,16 @@
     if args.reset_installs:
         reset_all_installs()
 
     if args.reset_personal_path:
         LollmsPaths.reset_configs()
     
     if args.reset_config:
-        lollms_pathds = LollmsPaths.find_paths(tool_prefix="lollms_server_")
-        cfg_path = lollms_pathds.personal_configuration_path / lollms_pathds.tool_prefix+"local_config.yaml"
+        lollms_paths = LollmsPaths.find_paths(tool_prefix="lollms_server_")
+        cfg_path = lollms_paths.personal_configuration_path / f"{lollms_paths.tool_prefix}local_config.yaml"
         try:
             cfg_path.unlink()
             ASCIIColors.success("LOLLMS configuration reset successfully")
         except:
             ASCIIColors.success("Couldn't reset LOLLMS configuration")
```

### Comparing `lollms-2.1.7/lollms/helpers.py` & `lollms-2.1.8/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/langchain_integration.py` & `lollms-2.1.8/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/main_config.py` & `lollms-2.1.8/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/paths.py` & `lollms-2.1.8/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/personality.py` & `lollms-2.1.8/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms/server.py` & `lollms-2.1.8/lollms/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import yaml
 import copy
 
 def reset_all_installs(lollms_paths:LollmsPaths):
     ASCIIColors.info("Removeing all configuration files to force reinstall")
     ASCIIColors.info(f"Searching files from {lollms_paths.personal_configuration_path}")
     for file_path in lollms_paths.personal_configuration_path.iterdir():
-        if file_path.name!=lollms_paths.tool_prefix+"local_config.yaml" and file_path.suffix.lower()==".yaml":
+        if file_path.name!=f"{lollms_paths.tool_prefix}local_config.yaml" and file_path.suffix.lower()==".yaml":
             file_path.unlink()
             ASCIIColors.info(f"Deleted file: {file_path}")
 
 
 class LoLLMsServer:
     def __init__(self):
         host = "localhost"
@@ -73,15 +73,15 @@
             reset_all_installs()
 
         if args.reset_personal_path:
             LollmsPaths.reset_configs()
 
         if args.reset_config:
             lollms_paths = LollmsPaths.find_paths(tool_prefix="lollms_server_")
-            cfg_path = lollms_paths.personal_configuration_path / lollms_paths.tool_prefix+"local_config.yaml"
+            cfg_path = lollms_paths.personal_configuration_path / f"{lollms_paths.tool_prefix}local_config.yaml"
             try:
                 cfg_path.unlink()
                 ASCIIColors.success("LOLLMS configuration reset successfully")
             except:
                 ASCIIColors.success("Couldn't reset LOLLMS configuration")
 
         # Configuration loading part
```

### Comparing `lollms-2.1.7/lollms/settings.py` & `lollms-2.1.8/lollms/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from lollms.personality import PersonalityBuilder
 from lollms.console import MainMenu
 
 def reset_all_installs(lollms_paths:LollmsPaths):
     ASCIIColors.info("Removeing all configuration files to force reinstall")
     ASCIIColors.info(f"Searching files from {lollms_paths.personal_configuration_path}")
     for file_path in lollms_paths.personal_configuration_path.iterdir():
-        if file_path.name!=lollms_paths.tool_prefix+"local_config.yaml" and file_path.suffix.lower()==".yaml":
+        if file_path.name!=f"{lollms_paths.tool_prefix}local_config.yaml" and file_path.suffix.lower()==".yaml":
             file_path.unlink()
             ASCIIColors.info(f"Deleted file: {file_path}")
 
 
 class Settings:
     def __init__(
                     self, 
@@ -43,15 +43,15 @@
 
         # Build menu
         self.menu = MainMenu(self)
         
         # Change configuration
         original = self.lollms_paths.default_cfg_path
         if configuration_path is None:
-            local = self.lollms_paths.personal_configuration_path / "local_config.yaml"        
+            local = self.lollms_paths.personal_configuration_path / f"{self.lollms_paths.tool_prefix}local_config.yaml"        
         else:
             local = Path(configuration_path)
             
         if not local.exists():
             shutil.copy(original, local)
         self.cfg_path = local
 
@@ -251,15 +251,15 @@
         reset_all_installs()
 
     if args.reset_personal_path:
         LollmsPaths.reset_configs()
     
     if args.reset_config:
         lollms_paths = LollmsPaths.find_paths(tool_prefix="lollms_server_")
-        cfg_path = lollms_paths.personal_configuration_path / lollms_paths.tool_prefix+"local_config.yaml"
+        cfg_path = lollms_paths.personal_configuration_path / f"{lollms_paths.tool_prefix}local_config.yaml"
         try:
             cfg_path.unlink()
             ASCIIColors.success("LOLLMS configuration reset successfully")
         except:
             ASCIIColors.success("Couldn't reset LOLLMS configuration")
 
     configuration_path = args.configuration_path
```

### Comparing `lollms-2.1.7/lollms/types.py` & `lollms-2.1.8/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.1.7/lollms.egg-info/PKG-INFO` & `lollms-2.1.8/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.1.7
+Version: 2.1.8
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lollms-2.1.7/setup.py` & `lollms-2.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.1.7",
+    version="2.1.8",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

