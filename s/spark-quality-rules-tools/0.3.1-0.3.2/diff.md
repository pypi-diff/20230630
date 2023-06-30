# Comparing `tmp/spark_quality_rules_tools-0.3.1.tar.gz` & `tmp/spark_quality_rules_tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.1.tar", last modified: Fri Jun 30 05:05:28 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.2.tar", last modified: Fri Jun 30 05:16:39 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.1.tar` & `spark_quality_rules_tools-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.618075 spark_quality_rules_tools-0.3.1/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-06-30 05:05:28.618075 spark_quality_rules_tools-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.1/README.md
--rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-30 05:05:28.626077 spark_quality_rules_tools-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.577066 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2094 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.609073 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    33429 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.615074 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.617074 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      772 2023-06-30 04:47:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.607072 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.655862 spark_quality_rules_tools-0.3.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-30 05:16:39.655862 spark_quality_rules_tools-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.2/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-30 05:16:39.656862 spark_quality_rules_tools-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-30 05:16:23.000000 spark_quality_rules_tools-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.638858 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2094 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.651861 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    33416 2023-06-30 05:16:23.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.653861 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.655862 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      772 2023-06-30 04:47:28.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.649860 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.1/LICENSE` & `spark_quality_rules_tools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/PKG-INFO` & `spark_quality_rules_tools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.1/README.md` & `spark_quality_rules_tools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/pyproject.toml` & `spark_quality_rules_tools-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/setup.py` & `spark_quality_rules_tools-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.1',
+    version='0.3.2',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 def dq_validate_conf_file(file_conf=None):
     from spark_quality_rules_tools import get_color_b
 
     if file_conf in ("", None):
         raise Exception(f'required variable file_conf')
 
     with open(file_conf) as f:
-        res = f.readlines()
+        res = f.read()
     print(f"{get_color_b(f'{res}')}")
 
 
 def dq_extract_parameters_artifactory(url_conf=None):
     import os
     import sys
     import re
@@ -311,16 +311,16 @@
     variables_list = list(set(variables_1 + variables_2))
 
     variables_dict = {variables: "" for variables in variables_list if
                       variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY")}
 
     parameter_dict = dict()
     parameter_dict[uuaa_name] = list()
-    parameter_dict[uuaa_name].append({"table": url_conf_name,
-                                      "conf_name": url_conf_extension,
+    parameter_dict[uuaa_name].append({"table": table_name,
+                                      "conf_name": url_conf_name,
                                       "parameters": variables_dict})
 
     with open(f"{dir_confs_filename_parameters}", "w") as f:
         json.dump(parameter_dict, f, indent=4)
 
     with open(f"{dir_confs_filename_parameters}") as f:
         parameter_conf = f.read()
```

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

