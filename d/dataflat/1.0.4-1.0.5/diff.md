# Comparing `tmp/dataflat-1.0.4.tar.gz` & `tmp/dataflat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflat-1.0.4.tar", last modified: Fri Jun  9 19:15:34 2023, max compression
+gzip compressed data, was "dataflat-1.0.5.tar", last modified: Thu Jun 29 22:18:06 2023, max compression
```

## Comparing `dataflat-1.0.4.tar` & `dataflat-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:34.454042 dataflat-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 19:15:24.000000 dataflat-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 19:15:34.454042 dataflat-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 19:15:24.000000 dataflat-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:34.454042 dataflat-1.0.4/dataflat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:34.454042 dataflat-1.0.4/dataflat/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/dictionary/flattener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/flattener_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:34.454042 dataflat-1.0.4/dataflat/pandas_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/pandas_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/pandas_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:34.454042 dataflat-1.0.4/dataflat/spark_df/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/spark_df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-09 19:15:24.000000 dataflat-1.0.4/dataflat/spark_df/flattener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:15:34.454042 dataflat-1.0.4/dataflat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-09 19:15:34.000000 dataflat-1.0.4/dataflat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 19:15:34.000000 dataflat-1.0.4/dataflat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:15:34.000000 dataflat-1.0.4/dataflat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 19:15:34.000000 dataflat-1.0.4/dataflat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 19:15:34.000000 dataflat-1.0.4/dataflat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:15:34.454042 dataflat-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-09 19:15:24.000000 dataflat-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-29 22:17:56.000000 dataflat-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:18:06.873386 dataflat-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-29 22:17:56.000000 dataflat-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/dictionary/flattener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/flattener_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/pandas_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/pandas_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/pandas_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat/spark_df/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/spark_df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-29 22:17:56.000000 dataflat-1.0.5/dataflat/spark_df/flattener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:18:06.873386 dataflat-1.0.5/dataflat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 22:18:06.000000 dataflat-1.0.5/dataflat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 22:18:06.873386 dataflat-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-29 22:17:56.000000 dataflat-1.0.5/setup.py
```

### Comparing `dataflat-1.0.4/LICENSE` & `dataflat-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/PKG-INFO` & `dataflat-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dataflat-1.0.4/README.md` & `dataflat-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/dataflat/commons.py` & `dataflat-1.0.5/dataflat/commons.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/dataflat/dictionary/flattener.py` & `dataflat-1.0.5/dataflat/dictionary/flattener.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/dataflat/exceptions.py` & `dataflat-1.0.5/dataflat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/dataflat/flattener_handler.py` & `dataflat-1.0.5/dataflat/flattener_handler.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/dataflat/pandas_df/flattener.py` & `dataflat-1.0.5/dataflat/pandas_df/flattener.py`

 * *Files identical despite different names*

### Comparing `dataflat-1.0.4/dataflat/spark_df/flattener.py` & `dataflat-1.0.5/dataflat/spark_df/flattener.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-'''
-spark_df/flattener.py- The processor script for pyspark dataframes flattening process
-
-Copyright (C) 2023 Juan ROJAS
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-
-Authors:
-    Juan ROJAS <jarojasa97@gmail.com>
-'''
-
 import json
 import re
 from typeguard import typechecked
 from typing import List
 from dataflat.commons import init_logger
 from dataflat.exceptions import FlatteningException
 from pyspark.sql.dataframe import DataFrame
@@ -44,131 +25,133 @@
             return col_name.replace(".", "_")
         return col_name
 
     def _process_column_name(self, dataframe:DataFrame, to_snake_case:bool, replace_dots:bool):
         """Receive a Spark Dataframe and return a snake_case columns like dataframe.
         If replace_dots is True, then all the subcolumns like "Column.SubColumn" will be
         renamed as "Column_SubColumn".
-
         Parameters
         ----------
         dataframe: pyspark.Dataframe
             The Spark Dataframe to rename each column to snake_case and replace dots with underscores.
         to_snake_case: bool
             If True rename the column to Snake Case column name like.
         replace_dots: bool
             If True replace the column name dots with underscores.
-
         Returns
         -------
         dataframe: pyspark.Dataframe
         """
         for col in dataframe.columns:
-            sc_col = self._to_snake_case(to_snake_case, col)
-            sc_col = self._replace_dots(replace_dots, sc_col)
+            renamed_col = self._to_snake_case(to_snake_case, col)
+            renamed_col = self._replace_dots(replace_dots, renamed_col)
             if to_snake_case | replace_dots:
-                dataframe = dataframe.withColumnRenamed(col, sc_col)
+                dataframe = dataframe.withColumnRenamed(col, renamed_col)
         return dataframe
 
     def _get_schema_struct(self, dataframe_schema:dict, id_key:str, black_list:List[str], dataframe_name:str, _ref:str = "", named_struct:dict = {}):
         """Receive Spark Dataframe Schema in dictionary format, and return 
         a dictionary[str, str] with the all required named_struct expressions
         to flatten de Dataframe.
-
         Parameters
         ----------
         dataframe_schema: dict
             A dictionary with the Dataframe schema.
         id_key: str
             The id key to be used as reference to the parent dataframe.
         black_list: List[str]
             A list of columns to ignore and not to add to the resulting flattened dictionary.
         dataframe_name: str
             A reference name for the dataframe, used to difference each
             resulting dataframe in the named_struct return.
         named_struct : dict, default is {}
-
         Returns
         -------
         named_struct: dict[str, str]
             A dictionary with all the named_struct expressions to flatten the
             provided Dataframe schema.
         """
         for field in dataframe_schema['fields']:
             if field['name'] not in black_list:
-                field_name = _ref + field['name']
+                field_ref = _ref + f"`{field['name']}`"
+                field_name = field_ref.replace("`","").replace(f"{dataframe_name.split('.')[-1]}.","")
                 if type(field['type']) is dict:
                     if field['type']['type'] == "array":
                         try:
-                            named_struct[f"{dataframe_name}.{field_name}"] += f"'{id_key}', {id_key},'{field_name}', {field_name},"
+                            named_struct[f"{dataframe_name}.{field_name}"] += f"'{dataframe_name}_id',{id_key},'{field_name}',{field_ref},"
                         except:
-                            named_struct[f"{dataframe_name}.{field_name}"] = f"'{id_key}', {id_key},'{field_name}', {field_name},"
+                            named_struct[f"{dataframe_name}.{field_name}"] = f"'{dataframe_name}_id',{id_key},'{field_name}',{field_ref},"
                     else:
-                        named_struct = self._get_schema_struct(field['type'], id_key, black_list, dataframe_name, f"{field_name}.", named_struct)
+                        named_struct = self._get_schema_struct(field['type'], id_key, black_list, dataframe_name, f"{field_ref}.", named_struct)
                 elif field['type'] == "map":
-                    print(f"MapType is not supported with pyflat processing, skipping column: {field_name}")
+                    print(f"MapType is not supported, skipping column: {field_name}")
                 else:
                     try:
-                        named_struct[dataframe_name] += f"'{field_name}', {field_name},"
+                        named_struct[dataframe_name] += f"'{field_name}',{field_ref},"
                     except:
-                        named_struct[dataframe_name] = f"'{field_name}', {field_name},"
+                        named_struct[dataframe_name] = f"'{field_name}',{field_ref},"
         return named_struct
 
     def _processor(self, dataframe:DataFrame, id_key:str, black_list:List[str], dataframe_name:str):
         """Receive a pyspark.Dataframe and returns a Dictionary[str, pyspark.DataFrame]
         with all the processed dataframes.
-
         Parameters
         ----------
         dataframe: pyspark.DataFrame
             A Dataframe to be flattened
         id_key: str
             The id key to be used as reference to the parent dataframe.
         black_list: List[str]
             A list of columns to ignore and not to add to the resulting flattened dictionary.
         dataframe_name: str
             A reference name for the dataframe, used to difference each
             resulting dataframe in the named_struct return.
-
         Returns
         -------
         processed_data : dict[str, pyspark.DataFrame]
             A dictionary with all the resulting Dataframes from the flattening process.
             Each ArrayType column will be flattened and added as a Dataframe inside the
             processed_data return.
         """
         processed_data = {}
         schema = json.loads(dataframe.schema.json())
         ns = self._get_schema_struct(schema, id_key, black_list, dataframe_name, _ref="", named_struct={})
+        parent_pos = f",'{dataframe_name}_pos',`pos`" if "'pos',`pos`" in ns[dataframe_name] else ""
         for df_name, struct in ns.items():
-            selectExpr = f"named_struct( {struct[:-1]} ) as Item"
-            aux_df = dataframe.selectExpr( selectExpr ).select("Item.*")
             if df_name != dataframe_name:
+                selectExpr = f"named_struct( {struct[:-1]}{parent_pos} ) as Item"
+                aux_df = dataframe.selectExpr( selectExpr ).select("Item.*")
+                child_id_key = aux_df.columns[0] if "." not in aux_df.columns[0] else f"`{aux_df.columns[0]}`"
                 expld_col = aux_df.columns[1]
                 expld_expr = expld_col if "." not in expld_col else f"`{expld_col}`"
-                aux_df = aux_df.select(id_key, posexplode(expld_expr).alias('pos', expld_col))
+                selected_cols = [child_id_key, posexplode(expld_expr).alias('pos', expld_col)]
+                if parent_pos:
+                    selected_cols.append(f'`{dataframe_name}_pos`')
+                aux_df = aux_df.select(selected_cols) \
+                    .withColumnRenamed(expld_col, expld_col.split(".")[-1])
                 processed_data[df_name] = aux_df
                 for types in aux_df.dtypes:
                     if "struct<" in types[1]:
-                        nested_dfs = self._processor(aux_df, id_key, black_list, df_name)
+                        nested_dfs = self._processor(aux_df, child_id_key, black_list, df_name)
                         processed_data.update(nested_dfs)
             else:
+                selectExpr = f"named_struct( {struct[:-1]} ) as Item"
+                aux_df = dataframe.selectExpr( selectExpr ).select("Item.*")
                 processed_data[df_name] = aux_df
         return processed_data
 
     def transform(self, dataframe:DataFrame, id_key:str, black_list:List[str] = [], dataframe_name:str = "df", to_snake_case:bool = False, replace_dots:bool = False):
         """Receive a pyspark.Dataframe and returns a Dictionary[str, pyspark.DataFrame]
         with all the processed dataframes.
         The ammount of dataframes on returned dictionary will depends on the number
         of ArrayType columns present on the input dataframe.
         If to_snake_case is set True, the column names on every processed Dataframe
         will be casted to snake_case.
         If replace_docts is set to True, all the dots present on a column name will
         be replaces such as follow example, "Column.SubColumn" -> "Column_SubColumn".
-
         Parameters
         ----------
         dataframe: pyspark.DataFrame
             A Dataframe to be flattened
         id_key: str
             The id key to be used as reference to the parent dataframe.
         black_list: List[str]
@@ -176,15 +159,14 @@
         dataframe_name: str
             A reference name for the dataframe, used to difference each
             resulting dataframe in the named_struct return.
         to_snake_case: bool
             If True rename the column to Snake Case column name like.
         replace_dots: bool
             If True replace the column name dots with underscores.
-
         Returns
         -------
         processed_data : dict[str, pyspark.DataFrame]
             A dictionary with all the resulting Dataframes from the flattening process.
             Each ArrayType column will be flattened and added as a Dataframe inside the
             processed_data return.
         """
```

### Comparing `dataflat-1.0.4/dataflat.egg-info/PKG-INFO` & `dataflat-1.0.5/dataflat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflat
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/JuanARojasA/dataflat
 Author: Juan Rojas
 Author-email: jarojasa97@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dataflat-1.0.4/setup.py` & `dataflat-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 PATH = path.abspath(path.dirname(__file__))
 
 with open(path.join(PATH, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
  
 setuptools.setup(
     name="dataflat",
-    version="1.0.4",
+    version="1.0.5",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/JuanARojasA/dataflat',
     author="Juan Rojas",
     author_email="jarojasa97@gmail.com",
     license='Apache License 2.0',
     platforms='any',
```

