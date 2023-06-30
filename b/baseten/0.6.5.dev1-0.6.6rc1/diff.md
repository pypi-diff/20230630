# Comparing `tmp/baseten-0.6.5.dev1.tar.gz` & `tmp/baseten-0.6.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.6.5.dev1.tar", max compression
+gzip compressed data, was "baseten-0.6.6rc1.tar", max compression
```

## Comparing `baseten-0.6.5.dev1.tar` & `baseten-0.6.6rc1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     5041 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/__init__.py
--rw-r--r--   0        0        0    29519 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/lib_support.py
--rw-r--r--   0        0        0    18701 2023-06-29 14:46:14.726091 baseten-0.6.5.dev1/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2847 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/settings.py
--rw-r--r--   0        0        0     1787 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     5130 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/training/datasets.py
--rw-r--r--   0        0        0    33964 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/training/logs.py
--rw-r--r--   0        0        0      479 2023-06-22 17:25:17.902135 baseten-0.6.5.dev1/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-06-22 17:25:17.906135 baseten-0.6.5.dev1/pypi_readme.md
--rw-r--r--   0        0        0     1969 2023-06-29 14:57:14.218114 baseten-0.6.5.dev1/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 baseten-0.6.5.dev1/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-06-30 18:08:26.650019 baseten-0.6.6rc1/baseten/__init__.py
+-rw-r--r--   0        0        0    12867 2023-06-30 18:08:26.650164 baseten-0.6.6rc1/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-02-28 15:48:08.032836 baseten-0.6.6rc1/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-02-28 15:48:08.033195 baseten-0.6.6rc1/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-06-30 18:08:26.650269 baseten-0.6.6rc1/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-02-28 15:48:08.033504 baseten-0.6.6rc1/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-02-28 15:48:08.033647 baseten-0.6.6rc1/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-02-28 15:48:08.033791 baseten-0.6.6rc1/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2022-09-07 01:02:04.877401 baseten-0.6.6rc1/baseten/common/__init__.py
+-rw-r--r--   0        0        0    29519 2023-06-30 18:08:26.650430 baseten-0.6.6rc1/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-06-30 18:08:26.650556 baseten-0.6.6rc1/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-02-28 15:48:08.034880 baseten-0.6.6rc1/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-06-30 18:08:26.650670 baseten-0.6.6rc1/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-02-28 15:48:08.035269 baseten-0.6.6rc1/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    18701 2023-06-30 18:08:26.650827 baseten-0.6.6rc1/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2288 2023-06-30 18:10:46.800516 baseten-0.6.6rc1/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-06-30 18:08:26.651045 baseten-0.6.6rc1/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-02-28 15:48:08.035833 baseten-0.6.6rc1/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-06-30 18:08:26.651165 baseten-0.6.6rc1/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-06-30 18:08:26.651869 baseten-0.6.6rc1/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-06-30 18:08:26.652036 baseten-0.6.6rc1/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-06-30 18:08:26.652139 baseten-0.6.6rc1/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-06-30 18:08:26.652207 baseten-0.6.6rc1/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-06-30 18:08:26.652347 baseten-0.6.6rc1/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-02-28 15:48:08.036730 baseten-0.6.6rc1/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-06-30 18:08:26.652468 baseten-0.6.6rc1/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-06-30 18:08:26.652587 baseten-0.6.6rc1/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-30 18:08:26.652688 baseten-0.6.6rc1/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-06-30 18:08:26.652899 baseten-0.6.6rc1/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-02-28 15:48:08.037504 baseten-0.6.6rc1/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-02-28 15:48:08.037598 baseten-0.6.6rc1/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-02-28 15:48:08.044032 baseten-0.6.6rc1/pypi_readme.md
+-rw-r--r--   0        0        0     1963 2023-06-30 18:12:14.385356 baseten-0.6.6rc1/pyproject.toml
+-rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 baseten-0.6.6rc1/setup.py
+-rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 baseten-0.6.6rc1/PKG-INFO
```

### Comparing `baseten-0.6.5.dev1/baseten/__init__.py` & `baseten-0.6.6rc1/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/baseten_deployed_model.py` & `baseten-0.6.6rc1/baseten/baseten_deployed_model.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/cli.py` & `baseten-0.6.6rc1/baseten/cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/client_commands/baseten_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/client_commands/dataset_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/client_commands/finetuning_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/client_commands/models_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/client_commands/pretrained_cli.py` & `baseten-0.6.6rc1/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/api.py` & `baseten-0.6.6rc1/baseten/common/api.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/core.py` & `baseten-0.6.6rc1/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/error_handler.py` & `baseten-0.6.6rc1/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/files.py` & `baseten-0.6.6rc1/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/lib_support.py` & `baseten-0.6.6rc1/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/model_deployer.py` & `baseten-0.6.6rc1/baseten/common/model_deployer.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/settings.py` & `baseten-0.6.6rc1/baseten/common/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import configparser
 import os
-import shutil
-import tempfile
 from pathlib import Path
 from threading import local
 from urllib.parse import urlparse
 
 SKLEARN = "sklearn"
 KERAS = "keras"
 TENSORFLOW = "tensorflow"
@@ -14,26 +12,14 @@
 
 DEBUG = False
 CONFIG_FILE_PATH = f"{Path.home()}/.baseten_config"
 
 thread_data = local()
 
 
-def _write_file(config: configparser.ConfigParser, file_path: str):
-    """
-    We use a tempfile to write the contents to prevent race conditions around
-    writing this file, in cases where `baseten.login` is used programmatically.
-    This ensures that writes to the config file are atomic.
-    """
-    with tempfile.NamedTemporaryFile(delete=False, mode="w") as tmp_file:
-        with open(tmp_file.name, "w") as tmp_file_handler:
-            config.write(tmp_file_handler)
-        shutil.move(tmp_file.name, file_path)
-
-
 def is_config_file_valid() -> bool:
     try:
         config = configparser.ConfigParser()
         config.read(CONFIG_FILE_PATH)
         # read() doesn't raise an exception if the file doesn't exist
         return os.path.exists(CONFIG_FILE_PATH)
     except configparser.ParsingError:
@@ -43,15 +29,16 @@
 def set_config_defaults():
     config = configparser.ConfigParser()
     if is_config_file_valid():
         config.read(CONFIG_FILE_PATH)
     if not config.has_section("api"):
         config.add_section("api")
     config.set("api", "url_base", "https://app.baseten.co")
-    _write_file(config, CONFIG_FILE_PATH)
+    with open(CONFIG_FILE_PATH, "w") as configfile:
+        config.write(configfile)
 
     return config
 
 
 def read_config():
     if not is_config_file_valid():
         set_config_defaults()
@@ -61,19 +48,16 @@
 
 
 def set_config_value(section: str, key: str, value: str):
     config = read_config()
     if section not in config.sections():
         config.add_section(section)
     config.set(section, key, value)
-    _write_file(config, CONFIG_FILE_PATH)
-
-
-#    with open(CONFIG_FILE_PATH, "w") as configfile:
-#        config.write(configfile)
+    with open(CONFIG_FILE_PATH, "w") as configfile:
+        config.write(configfile)
 
 
 def get_server_url() -> str:
     config = read_config()
     try:
         return config.get("api", "url_base")
     except (configparser.NoSectionError, configparser.NoOptionError):
```

### Comparing `baseten-0.6.5.dev1/baseten/common/tar.py` & `baseten-0.6.6rc1/baseten/common/tar.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/types.py` & `baseten-0.6.6rc1/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/common/util.py` & `baseten-0.6.6rc1/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/models/flan_t5.py` & `baseten-0.6.6rc1/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/models/llama.py` & `baseten-0.6.6rc1/baseten/models/llama.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/models/stable_diffusion.py` & `baseten-0.6.6rc1/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/models/util.py` & `baseten-0.6.6rc1/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/models/whisper.py` & `baseten-0.6.6rc1/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/training/datasets.py` & `baseten-0.6.6rc1/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/training/finetuning.py` & `baseten-0.6.6rc1/baseten/training/finetuning.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/baseten/training/logs.py` & `baseten-0.6.6rc1/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/pypi_readme.md` & `baseten-0.6.6rc1/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.6.5.dev1/pyproject.toml` & `baseten-0.6.6rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.6.5dev1"
+version = "0.6.6rc1"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
@@ -25,15 +25,15 @@
 coolname = ">=1.1.0"
 pyyaml = ">=5.1"
 tqdm = "^4.62.1"
 requests-toolbelt = "^0.9.1"
 tenacity = "^8.0.1"
 single-source = "^0.3.0"
 semantic-version = "^2.10.0"
-truss = "0.4.9dev33"
+truss = "0.4.9"
 Pillow = "^9.3.0"
 types-requests = "^2.28.11.7"
 types-setuptools = "^65.6.0.2"
 types-pillow = "^9.3.0.4"
 types-pyyaml = "^6.0.12.2"
 halo = "^0.0.31"
 types-pytz = "^2022.7.1.0"
```

### Comparing `baseten-0.6.5.dev1/PKG-INFO` & `baseten-0.6.6rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.6.5.dev1
+Version: 0.6.6rc1
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: requests (>=2.22)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tqdm (>=4.62.1,<5.0.0)
-Requires-Dist: truss (==0.4.9dev33)
+Requires-Dist: truss (==0.4.9)
 Requires-Dist: types-pillow (>=9.3.0.4,<10.0.0.0)
 Requires-Dist: types-pytz (>=2022.7.1.0,<2023.0.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.2,<7.0.0.0)
 Requires-Dist: types-requests (>=2.28.11.7,<3.0.0.0)
 Requires-Dist: types-setuptools (>=65.6.0.2,<66.0.0.0)
 Project-URL: Documentation, https://docs.baseten.co
 Project-URL: Homepage, https://baseten.co
```

