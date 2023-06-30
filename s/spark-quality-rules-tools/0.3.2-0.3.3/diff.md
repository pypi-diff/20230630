# Comparing `tmp/spark_quality_rules_tools-0.3.2.tar.gz` & `tmp/spark_quality_rules_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.2.tar", last modified: Fri Jun 30 05:16:39 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.3.tar", last modified: Fri Jun 30 19:06:36 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.2.tar` & `spark_quality_rules_tools-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.655862 spark_quality_rules_tools-0.3.2/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-06-30 05:16:39.655862 spark_quality_rules_tools-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.2/README.md
--rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-30 05:16:39.656862 spark_quality_rules_tools-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-06-30 05:16:23.000000 spark_quality_rules_tools-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.638858 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2094 2023-06-30 05:01:41.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.651861 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    33416 2023-06-30 05:16:23.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.653861 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.655862 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      772 2023-06-30 04:47:28.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-06-30 05:16:39.649860 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-30 05:16:39.000000 spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/
+-rw-rw-rw-   0        0        0     1092 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-29 15:13:53.000000 spark_quality_rules_tools-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-30 19:04:10.000000 spark_quality_rules_tools-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.045713 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2094 2023-06-30 13:36:52.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.061335 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    33747 2023-06-30 16:22:49.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.076962 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-11 22:08:20.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 16:22:49.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.092585 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 14:07:09.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 13:58:14.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-11 17:19:50.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 18:59:43.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:36.061335 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-30 19:06:35.000000 spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.2/LICENSE` & `spark_quality_rules_tools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.2/PKG-INFO` & `spark_quality_rules_tools-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.2/README.md` & `spark_quality_rules_tools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.2/pyproject.toml` & `spark_quality_rules_tools-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.2/setup.py` & `spark_quality_rules_tools-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.2',
+    version='0.3.3',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/functions/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,16 @@
     print(f"{get_color('=================================')} ")
 
 
 def dq_run_sandbox_artifactory(spark=None,
                                sc=None,
                                parameter_conf_list=None,
                                url_conf=None,
-                               is_prod=True):
+                               is_prod=True,
+                               resolve_name="resolve_sandbox.conf"):
     import json
     import sys
     import os
     from datetime import datetime
     from tqdm import tqdm
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
@@ -373,14 +374,16 @@
         raise Exception(f'required environment: pj_dq_dir_reports_name')
     if uuaa_code is None:
         raise Exception(f'required environment: UUAA_CODE')
     if user_sandbox is None:
         raise Exception(f'required environment: JPY_USER')
     if dir_sandbox_dq_metrics is None:
         raise Exception(f'required environment: pj_dq_dir_sandbox_dq_metrics')
+    if resolve_name is None:
+        raise Exception(f'required environment: resolve_name')
 
     url = url_conf
     url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
     url_conf_name = str(str(url_conf_extension).split(".")[0])
     uuaa_name = str(str(url).split("/")[-2]).upper()
     if not len(uuaa_name) == 4:
         uuaa_name = str(str(url).split("/")[-5]).upper()
@@ -435,21 +438,20 @@
     os.makedirs(os.path.dirname(dir_reports_name_filename), exist_ok=True)
 
     conf_file = ConfigFactory.parse_string(txt_conf)
     hocons_file = HOCONConverter.to_hocon(conf_file)
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file)
 
-    spark._jvm.org.apache.hadoop.fs.Path
     spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
 
     conf = sc._jvm.java.io.File(dir_hocons_filename)
     ConfigFactory2 = sc._jvm.com.typesafe.config.ConfigFactory
     parsed_conf = ConfigFactory2.parseFile(conf)
-    resolve_path = get_replace_resolve_parameter(sc=sc)
+    resolve_path = get_replace_resolve_parameter(sc=sc, resolve_name=resolve_name)
     resolvedConfig = parsed_conf.withFallback(resolve_path).resolve()
     Standalone = sc._jvm.com.datio.hammurabi.sandbox
     result = Standalone.Hammurabi.run(spark._jsparkSession, resolvedConfig)
 
     if result == 2:
         print(f"{get_color('Problema para construir la ejecución, posible configuración o regla mal definida')} ")
     else:
@@ -495,15 +497,16 @@
 
 def dq_run_sandbox_file(spark=None,
                         sc=None,
                         uuaa=None,
                         table_name=None,
                         parameter_conf_list=None,
                         file_conf=None,
-                        is_prod=True):
+                        is_prod=True,
+                        resolve_name="resolve_sandbox.conf"):
     import json
     import sys
     import os
     from datetime import datetime
     from tqdm import tqdm
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
@@ -532,14 +535,16 @@
         raise Exception(f'required environment: pj_dq_dir_reports_name')
     if uuaa_code is None:
         raise Exception(f'required environment: UUAA_CODE')
     if user_sandbox is None:
         raise Exception(f'required environment: JPY_USER')
     if dir_sandbox_dq_metrics is None:
         raise Exception(f'required environment: pj_dq_dir_sandbox_dq_metrics')
+    if resolve_name is None:
+        raise Exception(f'required environment: resolve_name')
 
     url_conf_name = str(str(file_conf).split(".")[0])
     uuaa_name = str(uuaa).upper()
 
     now = datetime.now()
     current_datetime = now.strftime("%Y-%m-%d %H:%M:%S")
     current_datetime_str = now.strftime("%Y%m%d%H%M")
@@ -595,15 +600,15 @@
         f.write(hocons_file)
 
     spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
 
     conf = sc._jvm.java.io.File(dir_hocons_filename)
     ConfigFactory2 = sc._jvm.com.typesafe.config.ConfigFactory
     parsed_conf = ConfigFactory2.parseFile(conf)
-    resolve_path = get_replace_resolve_parameter(sc=sc)
+    resolve_path = get_replace_resolve_parameter(sc=sc, resolve_name=resolve_name)
     resolvedConfig = parsed_conf.withFallback(resolve_path).resolve()
     Standalone = sc._jvm.com.datio.hammurabi.sandbox
     result = Standalone.Hammurabi.run(spark._jsparkSession, resolvedConfig)
 
     if result == 2:
         print(f"{get_color('Problema para construir la ejecución, posible configuración o regla mal definida')} ")
     else:
```

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resolve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import warnings
 
 warnings.filterwarnings('always')
 warnings.filterwarnings('ignore')
 
 
-def get_replace_resolve_parameter(sc=None):
+def get_replace_resolve_parameter(sc=None, resolve_name=None):
     import os
     import sys
     from spark_quality_rules_tools.utils import BASE_DIR
     from spark_quality_rules_tools.utils.color import get_color, get_color_b
     from pyhocon.converter import HOCONConverter
     from pyhocon import ConfigFactory
 
     is_windows = sys.platform.startswith('win')
     user_sandbox = os.getenv('JPY_USER')
     dir_uuaa_code = os.getenv("pj_dq_dir_uuaa_code")
     dir_resolve_name = os.getenv("pj_dq_dir_resolve_name")
-    dir_resource_resolve = os.path.join(BASE_DIR, "utils", "resource", "resolve.conf")
-    dir_resolve_filename = os.path.join(dir_resolve_name, "resolve.conf")
+    dir_resource_resolve = os.path.join(BASE_DIR, "utils", "resource", resolve_name)
+    dir_resolve_filename = os.path.join(dir_resolve_name, "resolve_sandbox.conf")
 
     if user_sandbox in ("", None):
         raise Exception(f'required environment JPY_USER')
     if dir_uuaa_code in ("", None):
         raise Exception(f'required environment pj_dq_dir_uuaa_code')
     if dir_resolve_name in ("", None):
         raise Exception(f'required environment pj_dq_dir_resolve_name')
```

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools/utils/rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,26 @@
         rules_columns_all = {**rules_columns, **rules_default_properties}
         rules_columns_required = [key for key, val in rules_columns_all.items() if val[1] == "true"]
 
         t = PrettyTable()
         print(f"type   => {get_color_g(haas_rules_type)}")
         print(f"class  => {get_color_g(haas_rules_class)}")
         print(f"version=> {get_color_g(rules_version)}")
+        if "id" in haas_columns.keys():
+            print(f"id=> {get_color_g(haas_columns.get('id'))}")
+        else:
+            print(f"id=> {get_color_g('No existe parametro ID')}")
 
         t.field_names = [f"Variable", "Value", "Dtype Actual", "Dtype Esperado", "Es Obligatorio"]
         for col in rules_columns_required:
+            if "id" in haas_columns.keys():
+                print(f"id=> {get_color_g(rules_columns_all[col])}")
+            else:
+                print(f"id=> {get_color_g('No existe parametro ID')}")
+
             if str(col) not in haas_columns.keys():
                 t.add_row([get_color_r(col),
                            get_color_r("variable requerida"),
                            get_color_r("variable requerida"),
                            get_color_r(rules_columns_all[col][0]),
                            get_color_r(rules_columns_all[col][1])
                            ])
```

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.2/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.3/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 spark_quality_rules_tools.egg-info/top_level.txt
 spark_quality_rules_tools/functions/__init__.py
 spark_quality_rules_tools/functions/generator.py
 spark_quality_rules_tools/utils/__init__.py
 spark_quality_rules_tools/utils/color.py
 spark_quality_rules_tools/utils/resolve.py
 spark_quality_rules_tools/utils/rules.py
-spark_quality_rules_tools/utils/resource/resolve.conf
+spark_quality_rules_tools/utils/resource/resolve_edge.conf
+spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
 spark_quality_rules_tools/utils/resource/rules.json
```

