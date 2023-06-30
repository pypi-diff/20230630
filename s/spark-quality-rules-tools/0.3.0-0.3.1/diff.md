# Comparing `tmp/spark_quality_rules_tools-0.3.0.tar.gz` & `tmp/spark_quality_rules_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.0.tar", last modified: Sun Jun 18 12:51:49 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.1.tar", last modified: Fri Jun 30 05:05:28 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.0.tar` & `spark_quality_rules_tools-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.523546 spark_quality_rules_tools-0.3.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-06-18 12:51:49.523546 spark_quality_rules_tools-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.0/README.md
--rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-18 12:51:49.524546 spark_quality_rules_tools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-06-18 12:10:00.000000 spark_quality_rules_tools-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.507542 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     1477 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.519545 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    21150 2023-06-18 03:08:52.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.521545 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.523546 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.518544 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.618075 spark_quality_rules_tools-0.3.1/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-30 05:05:28.618075 spark_quality_rules_tools-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.1/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-30 05:05:28.626077 spark_quality_rules_tools-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.577066 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2094 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.609073 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    33429 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.615074 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.617074 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      772 2023-06-30 04:47:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-30 05:05:28.607072 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-30 05:05:28.000000 spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.0/LICENSE` & `spark_quality_rules_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.0/PKG-INFO` & `spark_quality_rules_tools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.0/README.md` & `spark_quality_rules_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.0/pyproject.toml` & `spark_quality_rules_tools-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.0/setup.py` & `spark_quality_rules_tools-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.0',
+    version='0.3.1',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/functions/generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,40 +29,45 @@
     import os
     from pyspark.sql import SparkSession
     from spark_quality_rules_tools import get_color, get_color_b
 
     dir_uuaa_code = os.getenv("pj_dq_dir_uuaa_code")
     dir_sandbox_dq_metrics = os.getenv("pj_dq_dir_sandbox_dq_metrics")
     dir_sandbox_dq_refusals = os.getenv("pj_dq_dir_sandbox_dq_refusals")
+    dir_sandbox_dq_temporaries = os.getenv("pj_dq_dir_sandbox_dq_temporaries")
     if user_sandbox is None:
         user_sandbox = os.getenv('JPY_USER')
         if user_sandbox in ("", None):
             raise Exception(f'required variable user_sandbox')
     if dir_uuaa_code in ("", None):
         raise Exception(f'required environment: pj_dq_dir_uuaa_code')
     if dir_sandbox_dq_metrics in ("", None):
         raise Exception(f'required environment: pj_dq_dir_sandbox_dq_metrics')
     if dir_sandbox_dq_refusals in ("", None):
         raise Exception(f'required environment: pj_dq_dir_sandbox_dq_refusals')
+    if dir_sandbox_dq_temporaries in ("", None):
+        raise Exception(f'required environment: pj_dq_dir_sandbox_dq_temporaries')
 
     os.environ['UUAA_CODE'] = dir_uuaa_code
     os.environ['JPY_USER'] = user_sandbox
     os.environ['SANDBOX_DQ_METRICS'] = dir_sandbox_dq_metrics
     os.environ['SANDBOX_DQ_REFUSALS'] = dir_sandbox_dq_refusals
+    os.environ['SANDBOX_DQ_TEMPORARIES'] = dir_sandbox_dq_temporaries
 
     spark = SparkSession.builder \
         .master("local[*]") \
         .appName("JONAP") \
         .getOrCreate()
     spark.conf.set("spark.sql.execution.arrow.pyspark.enabled", "true")
     sc = spark.sparkContext
     sc._conf.setExecutorEnv("UUAA_CODE", os.getenv("UUAA_CODE"))
     sc._conf.setExecutorEnv("JPY_USER", os.getenv("JPY_USER"))
     sc._conf.setExecutorEnv("SANDBOX_DQ_METRICS", os.getenv("SANDBOX_DQ_METRICS"))
     sc._conf.setExecutorEnv("SANDBOX_DQ_REFUSALS", os.getenv("SANDBOX_DQ_REFUSALS"))
+    sc._conf.setExecutorEnv("SANDBOX_DQ_TEMPORARIES", os.getenv("SANDBOX_DQ_TEMPORARIES"))
 
     print(f"{get_color('Created Session Spark for user:')} {get_color_b(user_sandbox)}")
     return spark, sc
 
 
 def dq_path_workspace(spark=None,
                       user_sandbox=None,
@@ -77,27 +82,30 @@
         if user_sandbox in ("", None):
             raise Exception(f'required variable user_sandbox')
     is_windows = sys.platform.startswith('win')
     pj_dir_workspace = ""
     pj_dq_dir_uuaa_code = os.path.join(uuaa_code, "data", "projects", project_sda, "data_quality_rules")
     pj_dq_dir_sandbox_dq_metrics = f"/data/sandboxes/{pj_dq_dir_uuaa_code}/data/users/{user_sandbox}/dq/metrics"
     pj_dq_dir_sandbox_dq_refusals = f"/data/sandboxes/{pj_dq_dir_uuaa_code}/data/users/{user_sandbox}/dq/refusals"
+    pj_dq_dir_sandbox_dq_temporaries = f"/data/sandboxes/{pj_dq_dir_uuaa_code}/data/users/{user_sandbox}/dq/temporaries"
+
     pj_dq_dir_name = "data_quality_rules"
     pj_dq_dir_artifacts_python = os.path.join(pj_dir_workspace, "artifacts", "python")
     pj_dq_dir_artifacts_scala = os.path.join(pj_dir_workspace, "artifacts", "scala")
     pj_dq_dir_name = os.path.join(pj_dir_workspace, pj_dq_dir_name)
     pj_dq_dir_confs_name = os.path.join(pj_dir_workspace, pj_dq_dir_name, "data_confs")
     pj_dq_dir_hocons_name = os.path.join(pj_dir_workspace, pj_dq_dir_name, "data_hocons")
     pj_dq_dir_reports_name = os.path.join(pj_dir_workspace, pj_dq_dir_name, "data_reports")
     pj_dq_dir_resolve_name = os.path.join(pj_dir_workspace, pj_dq_dir_name, "data_resolve")
 
     if is_windows:
         pj_dq_dir_uuaa_code = pj_dq_dir_uuaa_code.replace("\\", "/")
         pj_dq_dir_sandbox_dq_metrics = pj_dq_dir_sandbox_dq_metrics.replace("\\", "/")
         pj_dq_dir_sandbox_dq_refusals = pj_dq_dir_sandbox_dq_refusals.replace("\\", "/")
+        pj_dq_dir_sandbox_dq_temporaries = pj_dq_dir_sandbox_dq_temporaries.replace("\\", "/")
         pj_dq_dir_artifacts_python = pj_dq_dir_artifacts_python.replace("\\", "/")
         pj_dq_dir_artifacts_scala = pj_dq_dir_artifacts_scala.replace("\\", "/")
         pj_dq_dir_name = pj_dq_dir_name.replace("\\", "/")
         pj_dq_dir_confs_name = pj_dq_dir_confs_name.replace("\\", "/")
         pj_dq_dir_hocons_name = pj_dq_dir_hocons_name.replace("\\", "/")
         pj_dq_dir_reports_name = pj_dq_dir_reports_name.replace("\\", "/")
         pj_dq_dir_resolve_name = pj_dq_dir_resolve_name.replace("\\", "/")
@@ -107,24 +115,26 @@
     dq_creating_directory_sandbox(path=pj_dq_dir_artifacts_scala)
     dq_creating_directory_sandbox(path=pj_dq_dir_confs_name)
     dq_creating_directory_sandbox(path=pj_dq_dir_hocons_name)
     dq_creating_directory_sandbox(path=pj_dq_dir_reports_name)
     dq_creating_directory_sandbox(path=pj_dq_dir_resolve_name)
     dq_creating_directory_hdfs(spark=spark, path=pj_dq_dir_sandbox_dq_metrics)
     dq_creating_directory_hdfs(spark=spark, path=pj_dq_dir_sandbox_dq_refusals)
+    dq_creating_directory_hdfs(spark=spark, path=pj_dq_dir_sandbox_dq_temporaries)
     os.environ['pj_dq_dir_name'] = pj_dq_dir_name
     os.environ['pj_dq_dir_artifacts_python'] = pj_dq_dir_artifacts_python
     os.environ['pj_dq_dir_artifacts_scala'] = pj_dq_dir_artifacts_scala
     os.environ['pj_dq_dir_confs_name'] = pj_dq_dir_confs_name
     os.environ['pj_dq_dir_hocons_name'] = pj_dq_dir_hocons_name
     os.environ['pj_dq_dir_reports_name'] = pj_dq_dir_reports_name
     os.environ['pj_dir_workspace'] = pj_dir_workspace
     os.environ['pj_dq_dir_uuaa_code'] = pj_dq_dir_uuaa_code
     os.environ['pj_dq_dir_sandbox_dq_metrics'] = pj_dq_dir_sandbox_dq_metrics
     os.environ['pj_dq_dir_sandbox_dq_refusals'] = pj_dq_dir_sandbox_dq_refusals
+    os.environ['pj_dq_dir_sandbox_dq_temporaries'] = pj_dq_dir_sandbox_dq_temporaries
     os.environ['pj_dq_dir_resolve_name'] = pj_dq_dir_resolve_name
 
 
 def dq_download_jar(haas_jar_url=None,
                     haas_version="4.8.0",
                     force=False):
     import requests
@@ -168,25 +178,36 @@
                     f.write(chunk)
         print(f"{get_color('Download Python finished on:')} {get_color_b(dir_artifacts_python_jar_file)}")
         print(f"{get_color('Download Scala finished on:')} {get_color_b(dir_artifacts_scala_jar_file)}")
     else:
         print(f"{get_color('Exist Jar haas Path:')} {get_color_b(dir_artifacts_python_jar_file)}")
 
 
-def dq_validate_conf(url_conf=None):
+def dq_validate_conf_artifactory(url_conf=None):
     import requests
     from spark_quality_rules_tools import get_color_b
 
     if url_conf in ("", None):
         raise Exception(f'required variable url_conf')
     res = requests.get(url_conf)
     print(f"{get_color_b(f'{res.text}')}")
 
 
-def dq_extract_parameters(url_conf=None):
+def dq_validate_conf_file(file_conf=None):
+    from spark_quality_rules_tools import get_color_b
+
+    if file_conf in ("", None):
+        raise Exception(f'required variable file_conf')
+
+    with open(file_conf) as f:
+        res = f.readlines()
+    print(f"{get_color_b(f'{res}')}")
+
+
+def dq_extract_parameters_artifactory(url_conf=None):
     import os
     import sys
     import re
     import json
     import requests
     from spark_quality_rules_tools import get_color, get_color_b
     is_windows = sys.platform.startswith('win')
@@ -248,19 +269,82 @@
     print(f"{get_color('uuaa name :')} {get_color_b(uuaa_name)}")
     print(f"{get_color('table name:')} {get_color_b(url_conf_name)}")
     print(f"{get_color('conf name :')} {get_color_b(url_conf_extension)}")
     print(f"{get_color('parameters:')} {get_color_b(params)}")
     print(f"{get_color('=================================')} ")
 
 
-def dq_run_sandbox(spark=None,
-                   sc=None,
-                   parameter_conf_list=None,
-                   url_conf=None,
-                   is_prod=True):
+def dq_extract_parameters_file(file_conf=None, uuaa=None, table_name=None):
+    import os
+    import sys
+    import re
+    import json
+    from spark_quality_rules_tools import get_color, get_color_b
+    is_windows = sys.platform.startswith('win')
+    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
+
+    if file_conf in ("", None):
+        raise Exception(f'required variable file_conf')
+    if dir_confs_name is None:
+        raise Exception(f'required environment: pj_dq_dir_confs_name')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
+    dir_confs_filename_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS-{url_conf_name}.json")
+
+    if is_windows:
+        dir_confs_filename = dir_confs_filename.replace("\\", "/")
+        dir_confs_filename_parameters = dir_confs_filename_parameters.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
+
+    with open(file_conf) as file:
+        hammurabi_conf = file.read()
+
+    with open(dir_confs_filename, 'w') as file:
+        file.write(hammurabi_conf)
+
+    with open(dir_confs_filename) as f:
+        hammurabi_conf = f.read()
+
+    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_list = list(set(variables_1 + variables_2))
+
+    variables_dict = {variables: "" for variables in variables_list if
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY")}
+
+    parameter_dict = dict()
+    parameter_dict[uuaa_name] = list()
+    parameter_dict[uuaa_name].append({"table": url_conf_name,
+                                      "conf_name": url_conf_extension,
+                                      "parameters": variables_dict})
+
+    with open(f"{dir_confs_filename_parameters}", "w") as f:
+        json.dump(parameter_dict, f, indent=4)
+
+    with open(f"{dir_confs_filename_parameters}") as f:
+        parameter_conf = f.read()
+        parameter_conf = json.loads(parameter_conf)
+
+    params = parameter_conf[uuaa_name][0]["parameters"]
+    params = json.dumps(params, indent=4)
+    print(f"{get_color(f'================================')} ")
+    print(f"{get_color('uuaa name :')} {get_color_b(uuaa_name)}")
+    print(f"{get_color('table name:')} {get_color_b(table_name)}")
+    print(f"{get_color('conf name :')} {get_color_b(url_conf_name)}")
+    print(f"{get_color('parameters:')} {get_color_b(params)}")
+    print(f"{get_color('=================================')} ")
+
+
+def dq_run_sandbox_artifactory(spark=None,
+                               sc=None,
+                               parameter_conf_list=None,
+                               url_conf=None,
+                               is_prod=True):
     import json
     import sys
     import os
     from datetime import datetime
     from tqdm import tqdm
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
@@ -405,15 +489,169 @@
     print(f"{get_color('table name:')} {get_color_b(url_conf_name)}")
     print(f"{get_color('conf name :')} {get_color_b(url_conf_extension)}")
     print(f"{get_color('cutoff date:')} {get_color_b(cutoff_date)}")
     print(f"{get_color('Generating a file csv:')} {get_color_b(dir_reports_name_filename)}")
     print(f"{get_color('=================================')} ")
 
 
-def dq_validate_rules(url_conf=None):
+def dq_run_sandbox_file(spark=None,
+                        sc=None,
+                        uuaa=None,
+                        table_name=None,
+                        parameter_conf_list=None,
+                        file_conf=None,
+                        is_prod=True):
+    import json
+    import sys
+    import os
+    from datetime import datetime
+    from tqdm import tqdm
+    from pyhocon import ConfigFactory
+    from pyhocon.converter import HOCONConverter
+    from pyspark.sql import functions as func
+    from spark_quality_rules_tools import get_color, get_color_b
+    from spark_quality_rules_tools import get_replace_resolve_parameter
+
+    is_windows = sys.platform.startswith('win')
+    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
+    dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
+    dir_reports_name = os.getenv('pj_dq_dir_reports_name')
+    uuaa_code = os.getenv("UUAA_CODE")
+    user_sandbox = os.getenv("JPY_USER")
+    dir_sandbox_dq_metrics = os.getenv("pj_dq_dir_sandbox_dq_metrics")
+    dir_sandbox_dq_refusals = os.getenv("pj_dq_dir_sandbox_dq_refusals")
+
+    if file_conf in ("", None):
+        raise Exception(f'required variable file_conf')
+    if parameter_conf_list in ("", None):
+        raise Exception(f'required variable parameter_conf_list')
+    if dir_confs_name is None:
+        raise Exception(f'required environment: pj_dq_dir_confs_name')
+    if dir_hocons_name is None:
+        raise Exception(f'required environment: pj_dq_dir_hocons_name')
+    if dir_reports_name is None:
+        raise Exception(f'required environment: pj_dq_dir_reports_name')
+    if uuaa_code is None:
+        raise Exception(f'required environment: UUAA_CODE')
+    if user_sandbox is None:
+        raise Exception(f'required environment: JPY_USER')
+    if dir_sandbox_dq_metrics is None:
+        raise Exception(f'required environment: pj_dq_dir_sandbox_dq_metrics')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+
+    now = datetime.now()
+    current_datetime = now.strftime("%Y-%m-%d %H:%M:%S")
+    current_datetime_str = now.strftime("%Y%m%d%H%M")
+
+    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
+    dir_confs_filename_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS-{url_conf_name}.json")
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
+
+    if is_windows:
+        dir_confs_filename = dir_confs_filename.replace("\\", "/")
+        dir_confs_filename_parameters = dir_confs_filename_parameters.replace("\\", "/")
+        dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_hocons_filename), exist_ok=True)
+
+    with open(dir_confs_filename_parameters) as f:
+        parameter_conf = f.read()
+        parameter_conf = json.loads(parameter_conf)
+
+    params_parameter = parameter_conf[uuaa_name][0]["parameters"]
+    validate_parameter_keys = list(set(params_parameter.keys()))
+    validate_parameter_conf_keys = list(set([b for a in parameter_conf_list for b in a.keys()]))
+    validate_compare_parameters = (sorted(validate_parameter_keys) == sorted(validate_parameter_conf_keys))
+    if not validate_compare_parameters:
+        raise Exception(f'Need more variables the parameters: parameter_conf_list')
+
+    cutoff_date = ""
+    with open(dir_confs_filename) as f:
+        txt_conf = f.read()
+
+    txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
+    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}',
+                                "http://artifactory-gdt.central-02.nextgen.igrupobbva")
+    if is_prod:
+        txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-local")
+    else:
+        txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-dev-local")
+
+    for params_parameter_conf in tqdm(parameter_conf_list):
+        for k, v in params_parameter_conf.items():
+            if str(k).upper() in ("ODATE", "ODATE_DATE", "CUTOFF_DATE"):
+                cutoff_date = str(v).replace("-", "").strip()
+            txt_conf = txt_conf.replace(f'${{{k}}}', v)
+            txt_conf = txt_conf.replace(f'${{?{k}}}', v)
+    dir_reports_name_filename = os.path.join(dir_reports_name, uuaa_name,
+                                             f"{url_conf_name}_{current_datetime_str}_{cutoff_date}.csv")
+    if is_windows:
+        dir_reports_name_filename = dir_reports_name_filename.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_reports_name_filename), exist_ok=True)
+
+    conf_file = ConfigFactory.parse_string(txt_conf)
+    hocons_file = HOCONConverter.to_hocon(conf_file)
+    with open(dir_hocons_filename, "w") as f:
+        f.write(hocons_file)
+
+    spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
+
+    conf = sc._jvm.java.io.File(dir_hocons_filename)
+    ConfigFactory2 = sc._jvm.com.typesafe.config.ConfigFactory
+    parsed_conf = ConfigFactory2.parseFile(conf)
+    resolve_path = get_replace_resolve_parameter(sc=sc)
+    resolvedConfig = parsed_conf.withFallback(resolve_path).resolve()
+    Standalone = sc._jvm.com.datio.hammurabi.sandbox
+    result = Standalone.Hammurabi.run(spark._jsparkSession, resolvedConfig)
+
+    if result == 2:
+        print(f"{get_color('Problema para construir la ejecución, posible configuración o regla mal definida')} ")
+    else:
+        if result == 1:
+            print(f"{get_color('La validación de calidad falló, la regla crítica falló')} ")
+        elif result == 0:
+            print(
+                f"{get_color('Ha pasado la validación de calidad. Esto significa que no hay ninguna regla crítica que haya fallado.')} ")
+
+    metrics_df = spark.read.parquet(dir_sandbox_dq_metrics)
+    metrics_filter = metrics_df.filter(
+        func.col("gf_quality_rule_execution_date") >= func.unix_timestamp(func.lit(current_datetime)).cast('timestamp'))
+    df2 = metrics_filter.select(
+        func.col("gf_qr_functional_definition_id"),
+        func.concat(func.col("g_quality_rule_principle_type"),
+                    func.lit("."),
+                    func.col("g_quality_rule_type")).alias("Rule"),
+        func.regexp_replace(func.col("gf_quality_rule_metadata_map.ruleName"),
+                            "com.datio.hammurabi.rules.", ""
+                            ).alias("Rule Name"),
+        func.col("gf_qr_tg_object_physical_name"),
+        func.col("gf_cutoff_date"),
+        func.col("gf_field_physical_name").alias("Field"),
+        func.col("gf_qr_aux_attribute_desc").alias("Format"),
+        func.col("g_qr_critical_type").alias("Is Critical"),
+        func.col("gf_qr_min_acceptance_per").alias("% Acceptation"),
+        func.col("g_quality_rule_status_type").alias("Status"),
+        func.col("gf_quality_rule_compliance_per").alias("Por"))
+    df3 = df2.distinct().sort("gf_qr_functional_definition_id")
+    df3.show(500, False, True)
+
+    metrics_filter_pandas = df3.toPandas()
+    metrics_filter_pandas.to_csv(dir_reports_name_filename, index=False)
+
+    print(f"{get_color(f'================================')} ")
+    print(f"{get_color('uuaa name :')} {get_color_b(uuaa_name)}")
+    print(f"{get_color('table name:')} {get_color_b(table_name)}")
+    print(f"{get_color('conf name :')} {get_color_b(url_conf_name)}")
+    print(f"{get_color('cutoff date:')} {get_color_b(cutoff_date)}")
+    print(f"{get_color('Generating a file csv:')} {get_color_b(dir_reports_name_filename)}")
+    print(f"{get_color('=================================')} ")
+
+
+def dq_validate_rules_artifactory(url_conf=None):
     import sys
     import os
     from spark_quality_rules_tools import get_validate_rules
 
     is_windows = sys.platform.startswith('win')
     dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
 
@@ -427,7 +665,27 @@
     if url_conf in ("", None):
         raise Exception(f'required variable url_conf')
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
+
+
+def dq_validate_rules_file(file_conf=None, uuaa=None):
+    import sys
+    import os
+    from spark_quality_rules_tools import get_validate_rules
+
+    is_windows = sys.platform.startswith('win')
+    dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+
+    if file_conf in ("", None):
+        raise Exception(f'required variable file_conf')
+
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
+    if is_windows:
+        dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
+    get_validate_rules(hocons_dir=dir_hocons_filename)
```

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files 21% similar despite different names*

```diff
@@ -6,13 +6,13 @@
         {"class": "com.datio.hammurabi.writers.LogsWriter",
          "config": {"uuaa": ${UUAA_CODE}, "user": ${JPY_USER} }},
         {"class": "com.datio.hammurabi.sandbox.writers.SandboxMetricsWriter",
          "config": {"uuaa": ${UUAA_CODE}, "user": ${JPY_USER} }},
         {"class": "com.datio.hammurabi.sandbox.writers.SandboxRefusalsWriter",
          "config": {"uuaa": ${UUAA_CODE}, "user": ${JPY_USER} }}
       ],
-      "temporaryWriter":
+      "temporaryWriter":[
         {"class": "com.datio.hammurabi.sandbox.writers.SandboxTemporalObjectsWriter",
-         "config": {"uuaa": ${UUAA_CODE}, "user": ${JPY_USER} }}
+         "config": {"uuaa": ${UUAA_CODE}, "user": /data/sandboxes/${UUAA_CODE}/data/users/${JPY_USER}/dq/temporaries}}]
     }
   }
 }
```

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.1/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

