# Comparing `tmp/dq_module-1.1.2.tar.gz` & `tmp/dq_module-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dq_module-1.1.2.tar", last modified: Fri Jun  2 06:29:47 2023, max compression
+gzip compressed data, was "dist/dq_module-1.1.3.tar", last modified: Fri Jun 30 08:42:58 2023, max compression
```

## Comparing `dq_module-1.1.2.tar` & `dq_module-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-06-02 06:29:47.000000 dq_module-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11346 2023-06-02 06:29:32.000000 dq_module-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/dataqualitycheck/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10482 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/consistencycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    37781 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/dataprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/dataqualitycheck/datasources/
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/azureblobdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5534 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/databricksfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/databrickssqldf.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/datasources/localfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5366 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/enumfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    40659 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckpolars.py
--rw-rw-rw-   0 root         (0) root         (0)    37038 2023-06-02 06:29:32.000000 dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckspark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-02 06:29:47.000000 dq_module-1.1.2/dq_module.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 06:29:47.000000 dq_module-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-02 06:29:32.000000 dq_module-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-06-30 08:42:58.000000 dq_module-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2023-06-30 08:42:41.000000 dq_module-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/dataqualitycheck/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10482 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/consistencycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    37781 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/dataprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/dataqualitycheck/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)     7917 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/azureblobdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5534 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/databricksfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/databrickssqldf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/localfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5366 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/enumfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    42396 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckpolars.py
+-rw-rw-rw-   0 root         (0) root         (0)    38755 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckspark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 08:42:58.000000 dq_module-1.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-30 08:42:41.000000 dq_module-1.1.3/setup.py
```

### Comparing `dq_module-1.1.2/PKG-INFO` & `dq_module-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_module
-Version: 1.1.2
+Version: 1.1.3
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.2/README.md` & `dq_module-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/commonutilities.py` & `dq_module-1.1.3/dataqualitycheck/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/consistencycheck.py` & `dq_module-1.1.3/dataqualitycheck/consistencycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/dataprofile.py` & `dq_module-1.1.3/dataqualitycheck/dataprofile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/datasources/azureblobdf.py` & `dq_module-1.1.3/dataqualitycheck/datasources/azureblobdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/datasources/commonutilities.py` & `dq_module-1.1.3/dataqualitycheck/datasources/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/datasources/databricksfilesystemdf.py` & `dq_module-1.1.3/dataqualitycheck/datasources/databricksfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/datasources/databrickssqldf.py` & `dq_module-1.1.3/dataqualitycheck/datasources/databrickssqldf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         except Exception as e:
             raise Exception(f"Error occured while creating spark dataframe from {source_input['source_name']}.{source_input['filename']} , {e}")
         return df
 
     def read_enforce_schema_spark(self, source_input, schema, no_of_partition = 4):
         try:
             df = self.spark.sql(f"select * from {source_input['source_name']}.{source_input['filename']}").repartition(no_of_partition)
-            df = self.spark.createDataFrame(df.rdd, schema=schema, verifySchema=False)
+            df = self.spark.createDataFrame(df.collect(), schema=schema, verifySchema=False)
         except Exception as e:
             raise Exception(f"Error occured while creating enforce schema data from {source_input['source_name']}.{source_input['filename']}, {e}")
         return df
         
     def read_enforce_schema_polars(self, source_input,schema, no_of_partition = 4):
         try:
             polars_schema=[str(schema_val[1])  for schema_val in schema]
```

### Comparing `dq_module-1.1.2/dataqualitycheck/datasources/localfilesystemdf.py` & `dq_module-1.1.3/dataqualitycheck/datasources/localfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/enumfile.py` & `dq_module-1.1.3/dataqualitycheck/enumfile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheck.py` & `dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheck.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,9 +8,9 @@
             self.is_run_spark = False
             self.dq_ob = SingleDatasetQualityCheckPolars(tables_list, interaction_between_tables, data_read_ob, data_write_ob, data_right_structure, job_id, time_zone, output_db_name, no_of_partition)
         else:
             self.is_run_spark = True
             self.dq_ob = SingleDatasetQualityCheckSpark(tables_list, interaction_between_tables, data_read_ob, data_write_ob, data_right_structure, job_id, time_zone, output_db_name, no_of_partition)
 
 
-    def apply_validation(self, rule_config_df, write_summary_on_database = True, failed_schema_source_list = [], output_summary_folder_path=''):
-        self.dq_ob.apply_validation(rule_config_df, write_summary_on_database, failed_schema_source_list, output_summary_folder_path)
+    def apply_validation(self, rule_config_df, write_summary_on_database = True, failed_schema_source_list = [], output_summary_folder_path='', write_failed_records_flag=True):
+        self.dq_ob.apply_validation(rule_config_df, write_summary_on_database, failed_schema_source_list, output_summary_folder_path, write_failed_records_flag)
```

### Comparing `dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckpolars.py` & `dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckpolars.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,32 +27,41 @@
         self.run_engine = 'polars'
         self.dataframes = read_dataset(
             self.tables_list, self.data_read_ob, self.no_of_partition, self.run_engine)
         self.output_db_name = output_db_name
         self.job_id = job_id
         self.data_right_structure = data_right_structure
         self.time_zone = time_zone
+        
+
     # ----- Function to define schema and create dataframe of the final result.
 
     def data_check_summarization(self, test_summary):
         schema = get_schema(QualityCheckSummaryStructure.COLUMN_NAME.value, QualityCheckSummaryStructure.COLUMN_DATATYPE.value, self.run_engine)
         df = pl.DataFrame(data=test_summary, schema=schema)
         return df
 
-    def write_failed_records(self, rule, failed_df, add_columns_in_folder_path=True):
-        if self.data_right_structure == 'file':
-            failed_record_folder_path = get_failed_record_folder_path(
-                rule, ModuleName.QUALITYCHECK.value, add_columns_in_folder_path)
-            failed_record_file_name = get_failed_record_file_name(self.time_zone)
-            failed_records_write_location = self.data_write_ob.write_from_polars(
-                failed_df, failed_record_folder_path, failed_record_file_name, rule)
-        else:
-            table_name = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
-            failed_records_write_location = self.data_write_ob.write_from_polars(
-                failed_df, self.output_db_name, table_name)
+    def write_failed_records(self, rule, failed_df, write_failed_records_flag=True, add_columns_in_folder_path=True):
+        if 'write_failed_records' in rule and rule['write_failed_records'] == 'False':
+            failed_records_write_location = 'Failed records are not written.'
+
+        elif write_failed_records_flag == False:
+            failed_records_write_location = 'Failed records are not written.'
+            
+        else:
+            if self.data_right_structure == 'file':
+                failed_record_folder_path = get_failed_record_folder_path(
+                    rule, ModuleName.QUALITYCHECK.value, add_columns_in_folder_path)
+                failed_record_file_name = get_failed_record_file_name(self.time_zone)
+                failed_records_write_location = self.data_write_ob.write_from_polars(
+                    failed_df, failed_record_folder_path, failed_record_file_name, rule)
+            else:
+                table_name = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
+                failed_records_write_location = self.data_write_ob.write_from_polars(
+                    failed_df, self.output_db_name, table_name)
         return failed_records_write_location
 
     def drift_report(self, config_col, dataframe_col):
         # indivisual data drift reports
         drift_df = pl.DataFrame(zip_longest(config_col.split(
             ','), dataframe_col), schema=['config_cols', 'dataframe_cols'])
         return drift_df.with_columns(pl.when((pl.col('config_cols') == pl.col('dataframe_cols')) & (pl.col('config_cols').is_not_null())).then(("No Drift")).otherwise(("Drift")).alias("Drift"))
@@ -89,15 +98,15 @@
                 infer_df, 'row_nr,'+column_names, 'int,'+",".join(['str']*len(column_names.split(',')))))
             total_records_df = total_records_df.unique(subset=total_records_df.columns)
         except Exception as e:
             raise Exception(e)
         return total_records_df
     # ----- Function to check if column have any null value.
 
-    def null_check(self, df, rule):
+    def null_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         result = df.filter(pl.col(rule["column_to_be_checked"]).is_null())
         #result = df.filter(~pl.all(pl.col(rule["column_to_be_checked"]).is_not_null()))
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -113,19 +122,19 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df,  write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
-    def schema_check(self, df, rule):
+    def schema_check(self, df, rule,  write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         date_col_config = eval(
             rule["date_column_config"]) if rule["date_column_config"] and rule["date_column_config"] != 'null' else {}
         total_row_count = df.height
         failed_records_count = 0
         failed_records_write_location = 'N/A'
@@ -202,15 +211,15 @@
                         pl.lit("All columns").alias("Column_Tested"),
                         pl.lit(1 if rule["ruletype"] ==
                                'Mandatory' else 0).alias("Mandatory"),
                         pl.lit(self.job_id).alias("job_id")
                     ]
                 )
                 failed_records_write_location = self.write_failed_records(
-                    rule, failed_df, False)
+                    rule, failed_df, write_failed_records_flag, False)
 
         except Exception as e:
             test_status = "FAIL"
             failed_records_count = total_row_count
             reason = f', {e}'
             failed_df = df.with_columns(
                 [
@@ -219,21 +228,21 @@
                     pl.lit("All columns").alias("Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status + reason, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if values not be less than the given value
 
-    def range_min_check(self, df, rule):
+    def range_min_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
 #         df = df.filter(~pl.all(pl.col(rule["column_to_be_checked"]).is_null()))
         result = df.filter(pl.col(rule["column_to_be_checked"]).cast(
             pl.Float64, strict=False) < float(rule["value"]))
         failed_records_count = result.height
@@ -250,19 +259,19 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if values should not be less than or equal to the required value
-#    def range_min_inclusive_check(self, df, rule):
+#    def range_min_inclusive_check(self, df, rule, write_failed_records_flag):
 #       start = time.time()
 #        run_date = date.today().strftime("%Y/%m/%d")
 #        total_row_count = df.height
 #         df = df.filter(~pl.all(pl.col(rule["column_to_be_checked"]).is_null()))
 #        result = df.filter(
 #            pl.col(rule["column_to_be_checked"]).cast(pl.Float64, strict=False) <= float(rule["value"]))
 #        failed_records_count = result.height
@@ -279,20 +288,20 @@
 #                        "Column_Tested"),
 #                    pl.lit(1 if rule["ruletype"] ==
 #                           'Mandatory' else 0).alias("Mandatory"),
 #                    pl.lit(self.job_id).alias("job_id")
 #                ]
 #            )
 #            failed_records_write_location = self.write_failed_records(
-#                rule, failed_df)
+#                rule, failed_df, write_failed_records_flag)
 #
 #        return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if values should not be greater then the given value
-    def range_max_check(self, df, rule):
+    def range_max_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
 #         df = df.filter(~pl.all(pl.col(rule["column_to_be_checked"]).is_null()))
         result = df.filter(
             pl.col(rule["column_to_be_checked"]).cast(pl.Float64, strict=False) > float(rule["value"]))
         failed_records_count = result.height
@@ -309,20 +318,20 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the values in the column have given length or not.
-    def length_check(self, df, rule):
+    def length_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         result = df.filter(
             pl.col(rule["column_to_be_checked"]).cast(pl.Utf8,strict=False).str.lengths() > int(rule["value"]))
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -338,20 +347,20 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if all the records are unique or not in the table.
-    def unique_records_check(self, df, rule):
+    def unique_records_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         columnList = df.columns
         d = df.select(columnList)
         result = df.filter(pl.lit(d.is_duplicated()))
         failed_records_count = result.height
@@ -369,20 +378,20 @@
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
 
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date, False, ",".join(df.columns))
 
     # ----- Function to check if all the records are unique for all given input columns.It takes a list of columns as an arguement
 
-    def unique_keys_check(self, df, rule):
+    def unique_keys_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         d = df.select(list(rule["column_to_be_checked"].split(",")))
         result = df.filter(pl.lit(d.is_duplicated()))
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -398,20 +407,20 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function takes a list of allowed values for a particular column and check if the values of the column belongs to that list or not.
-    def allowed_values_check(self, df, rule):
+    def allowed_values_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         result = df.filter(
             pl.col(rule["column_to_be_checked"]).is_in(rule["value"].strip().split(',')).is_not())
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -427,20 +436,20 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check that if the values in the column has the required minimum length or not.
-    def min_length_check(self, df, rule):
+    def min_length_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         result = df.filter(
             pl.col(rule["column_to_be_checked"]).cast(pl.Utf8,strict=False).str.lengths() < int(rule["value"]))
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -456,19 +465,19 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check that the table has required column count or not.
-    def column_count_check(self, df, rule):
+    def column_count_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         total_col_count = len(df.columns)
         failed_records_count = total_col_count - int(rule["value"])
         failed_records_write_location = 'N/A'
         if total_col_count == int(rule["value"]):
@@ -485,20 +494,20 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function takes a list of not allowed values for a particular column and check if the column has not allowed values or not.
-    def not_allowed_values_check(self, df, rule):
+    def not_allowed_values_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         result = df.filter(
             pl.col(rule["column_to_be_checked"]).is_in(rule["value"].strip().split(',')))
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -514,20 +523,20 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the date lies in the given range or not.
-    def date_range_check(self, df, rule):
+    def date_range_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         value = eval(rule["value"])
         
         min_value= parse( value["min_value"] )
         max_value= parse( value["max_value"] )
@@ -559,22 +568,22 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
         except :
           raise Exception("Wrong date format in date column config")
             
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the given column matches the given regex pattern or not.
-    def regex_check(self, df, rule):
+    def regex_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         result = df.filter(
             pl.col(rule["column_to_be_checked"]).str.contains(rule["value"]).is_not())
         failed_records_count = result.height
         failed_records_write_location = 'N/A'
@@ -589,19 +598,19 @@
                         "Column_Tested"),
                     pl.lit(1 if rule["ruletype"] ==
                            'Mandatory' else 0).alias("Mandatory"),
                     pl.lit(self.job_id).alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
-    def row_count_check(self, df, rule):
+    def row_count_check(self, df, rule, write_failed_records_flag):
         start = time.time()
         run_date = date.today().strftime("%Y/%m/%d")
         total_row_count = df.height
         failed_records_write_location = 'N/A'
         failed_records_count = total_row_count - int(rule["value"])
         if total_row_count == int(rule["value"]):
             test_status = "PASS"
@@ -614,15 +623,15 @@
                     pl.lit("All columns").alias("Column_Tested"),
                     pl.lit(1 if rule["ruletype"] == 'Mandatory' else 0).alias(
                         "Mandatory"),
                     pl.lit("NA").alias("job_id")
                 ]
             )
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
     # ----- Function takes the filepath of ruleset as an input and apply validations defined in the ruleset.
 
     def read_csv_input_and_apply_validation(self, rules_csv_file_path, result_summery_file_path, file_path=None):
         input_df = pl.read_csv(rules_csv_file_path)
         rule_set = input_df.rows(named=True)
@@ -630,31 +639,31 @@
         self.tables_list = {**self.tables_list, **new_tables}
         new_dataframes = read_dataset(
             new_tables, self.data_read_ob, self.no_of_partition, self.run_engine)
         if new_dataframes:
             self.dataframes = {**self.dataframes, **new_dataframes}
         self.df_rules_validation(rule_set, result_summery_file_path)
 
-    def apply_validation(self, rule_config_df, write_summary_on_database=False, failed_schema_source_list=[], output_summary_folder_path=''):
+    def apply_validation(self, rule_config_df, write_summary_on_database=False, failed_schema_source_list=[], output_summary_folder_path='', write_failed_records_flag=True):
         try:
             rule_set = rule_config_df.rows(named=True)
         except:
             rule_set = rule_config_df.collect()
         new_tables = get_missing_tables(self.tables_list, rule_set)
         self.tables_list = {**self.tables_list, **new_tables}
         new_dataframes = read_dataset(
             new_tables, self.data_read_ob, self.no_of_partition, self.run_engine)
         if new_dataframes:
             self.dataframes = {**self.dataframes, **new_dataframes}
         self.df_rules_validation(rule_set, write_summary_on_database,
-                                 failed_schema_source_list, output_summary_folder_path)
+                                 failed_schema_source_list, output_summary_folder_path, write_failed_records_flag)
 
     # ----- Function include all the above functions and apply rule set at once and gives a consolidated result.
 
-    def df_rules_validation(self, rule_set,  write_summary_on_database, failed_schema_source_list, result_summary_folder_path=''):
+    def df_rules_validation(self, rule_set,  write_summary_on_database, failed_schema_source_list, result_summary_folder_path='', write_failed_records_flag=True):
         test_summary = []
         try:
             for rule in rule_set:
                 try:
                     source = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
 
                     if "failed_schema_source_list" in rule and rule['failed_schema_source_list'] in failed_schema_source_list:
@@ -667,71 +676,71 @@
                         run_date = date.today().strftime("%Y/%m/%d")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "", "", "", "", 0, run_date))
                         continue
 
                     if rule["rule_name"] == "null_check":
                         result_df = self.null_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "schema_check":
                         result_df = self.schema_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "range_min_check":
                         result_df = self.range_min_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                    # elif rule["rule_name"] == "range_min_inclusive_check":
                    #     result_df = self.range_min_inclusive_check(
-                   #         self.dataframes[source], rule)
+                   #         self.dataframes[source], rule, write_failed_records_flag)
                    #     test_summary.append(result_df)
                     elif rule["rule_name"] == "range_max_check":
                         result_df = self.range_max_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "length_check":
                         result_df = self.length_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "unique_keys_check":
                         result_df = self.unique_keys_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "unique_records_check":
                         result_df = self.unique_records_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "allowed_values_check":
                         result_df = self.allowed_values_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "min_length_check":
                         result_df = self.min_length_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "column_count_check":
                         result_df = self.column_count_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "not_allowed_values_check":
                         result_df = self.not_allowed_values_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "date_range_check":
                         result_df = self.date_range_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "regex_check":
                         result_df = self.regex_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "row_count_check":
                         result_df = self.row_count_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     else:
                         run_date = date.today().strftime("%Y/%m/%d")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "invalid rule name", "", "", "", 0, run_date))
                         continue
                 except Exception as e:
```

### Comparing `dq_module-1.1.2/dataqualitycheck/singledatasetqualitycheckspark.py` & `dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckspark.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,25 +29,33 @@
         self.run_engine = 'pyspark'
         self.dataframes = read_dataset(
             self.tables_list, self.data_read_ob, self.no_of_partition)
         self.output_db_name = output_db_name
         self.job_id = job_id
         self.time_zone = time_zone
 
-    def write_failed_records(self, rule, failed_df, add_columns_in_folder_path=True):
-        if self.data_right_structure == 'file':
-            failed_record_folder_path = get_failed_record_folder_path(
-                rule, ModuleName.QUALITYCHECK.value, add_columns_in_folder_path)
-            failed_record_file_name = get_failed_record_file_name(self.time_zone)
-            failed_records_write_location = self.data_write_ob.write(
-                failed_df, failed_record_folder_path, failed_record_file_name, rule)
-        else:
-            table_name = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
-            failed_records_write_location = self.data_write_ob.write(
-                failed_df, self.output_db_name, table_name)
+    def write_failed_records(self, rule, failed_df, write_failed_records_flag=True, add_columns_in_folder_path=True):
+        if 'write_failed_records' in rule and rule['write_failed_records'] == 'False':
+            failed_records_write_location = 'Failed records are not written.'
+
+        elif write_failed_records_flag == False:
+            failed_records_write_location = 'Failed records are not written.'
+
+        else:
+        
+            if self.data_right_structure == 'file':
+                failed_record_folder_path = get_failed_record_folder_path(
+                    rule, ModuleName.QUALITYCHECK.value, add_columns_in_folder_path)
+                failed_record_file_name = get_failed_record_file_name(self.time_zone)
+                failed_records_write_location = self.data_write_ob.write(
+                    failed_df, failed_record_folder_path, failed_record_file_name, rule)
+            else:
+                table_name = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
+                failed_records_write_location = self.data_write_ob.write(
+                    failed_df, self.output_db_name, table_name)
         return failed_records_write_location
 
     def drift_report(self, config_col, dataframe_col):
         # indivisual data drift reports
         drift_df = self.spark.createDataFrame(zip_longest(config_col.split(','), dataframe_col), schema=['config_cols', 'dataframe_cols']).\
             withColumn('Drift', when((col('config_cols') == col('dataframe_cols')) & (col('config_cols').isNotNull()),
                                      "No Drift").otherwise('Drift'))
@@ -80,35 +88,35 @@
                 schema_enforce_structure(column_names, ",".join(['str']*len(column_names.split(','))))))
             total_records_df = total_records_df.dropDuplicates(total_records_df.columns)
         except Exception as e:
             raise Exception(e)
         return total_records_df
 
     # ----- Function to check if column have any null value.
-    def null_check(self, df, rule):
+    def null_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(col(rule["column_to_be_checked"]).isNull())
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(
                 rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
        # ----- Function to check if all the required columns exist.
 
-    def schema_check(self, df, rule):
+    def schema_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         date_col_config = eval(
             rule["date_column_config"]) if rule["date_column_config"] and rule["date_column_config"] != 'null' else {}
         total_row_count = df.count()
         failed_records_count = 0
         failed_records_write_location = 'N/A'
@@ -185,29 +193,29 @@
                 else:
                     failed_df = failed_enforce_records
                     reason = ', wrong data type'
 
                 failed_df = failed_df.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                     .withColumn("Column_Tested", lit("All columns")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
                 failed_records_write_location = self.write_failed_records(
-                    rule, failed_df, False)
+                    rule, failed_df, write_failed_records_flag, False)
 
         except Exception as e:
             test_status = "FAIL"
             failed_records_count = total_row_count
             reason = f', {e}'
             failed_df = df.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit("All columns")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
         return data_quality_test_summary_tuple(self.job_id, rule, test_status + reason, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if values not be less than the given value
 
-    def range_min_check(self, df, rule):
+    def range_min_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
         result = df.filter(
             col(rule["column_to_be_checked"]) < float(rule["value"]))
         failed_records_count = result.count()
@@ -215,20 +223,20 @@
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
   #  # ----- Function to check if values should not be less than or equal to the required value
-  #  def range_min_inclusive_check(self, df, rule):
+  #  def range_min_inclusive_check(self, df, rule, write_failed_records_flag):
   #     run_date = date.today().strftime("%Y/%m/%d")
   #      start = time.time()
   #     total_row_count = df.count()
   #     df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
   #     result = df.filter(
   #          col(rule["column_to_be_checked"]) <= float(rule["value"]))
   #      failed_records_count = result.count()
@@ -236,20 +244,20 @@
   #     if failed_records_count == 0:
   #         test_status = "PASS"
   #     else:
   #          test_status = "FAIL"
   #          failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
   #             .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
   #         failed_records_write_location = self.write_failed_records(
-  #             rule, failed_df)
+  #             rule, failed_df, write_failed_records_flag)
   #
   #      return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if values should not be greater then the given value
-    def range_max_check(self, df, rule):
+    def range_max_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
         result = df.filter(
             col(rule["column_to_be_checked"]) > float(rule["value"]))
         failed_records_count = result.count()
@@ -257,40 +265,40 @@
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the values in the column have given length or not.
-    def length_check(self, df, rule):
+    def length_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             length(col(rule["column_to_be_checked"])) > int(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if all the records are unique or not in the table.
-    def unique_records_check(self, df, rule):
+    def unique_records_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         columnList = df.columns
         d = df.groupBy(columnList).count().filter(
             col("count") == 1).drop("count")
         result = df.exceptAll(d)
@@ -299,20 +307,20 @@
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit("All columns")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date, False, ",".join(df.columns))
 
     # ----- Function to check if all the records are unique for all given input columns.It takes a list of columns as an arguement
-    def unique_keys_check(self, df, rule):
+    def unique_keys_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
         d = df.groupBy(columnList).count().filter(col("count") > 1).drop("count")
         d= d.withColumn("concat_col", concat_ws("//", *columnList))
         df1 = df.withColumn("concat_col", concat_ws("//", *columnList))
@@ -322,60 +330,60 @@
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function takes a list of allowed values for a particular column and check if the values of the column belongs to that list or not.
-    def allowed_values_check(self, df, rule):
+    def allowed_values_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(~col(rule["column_to_be_checked"]).isin(
             rule["value"].strip().split(',')) | col(rule["column_to_be_checked"]).isNull())
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check that if the values in the column has the required minimum length or not.
-    def min_length_check(self, df, rule):
+    def min_length_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             length(col(rule["column_to_be_checked"])) < int(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check that the table has required column count or not.
-    def column_count_check(self, df, rule):
+    def column_count_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         total_col_count = len(df.columns)
         failed_records_count = total_col_count - int(rule["value"])
         failed_records_write_location = 'N/A'
         if total_col_count == int(rule["value"]):
@@ -383,40 +391,40 @@
         else:
             test_status = "FAIL"
             result = self.spark.createDataFrame(
                 data=[tuple([None for x in df.columns])], schema=df.schema)
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(f"{rule['rule_name']}:{rule['value']}"))\
                 .withColumn("Column_Tested", lit(f"All_Columns:{total_col_count}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function takes a list of not allowed values for a particular column and check if the column has not allowed values or not.
-    def not_allowed_values_check(self, df, rule):
+    def not_allowed_values_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             col(rule["column_to_be_checked"]).isin(rule["value"].strip().split(',')))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the date lies in the given range or not.
-    def date_range_check(self, df, rule):
+    def date_range_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         value = eval(rule["value"]) 
         date_column_config = eval(rule["date_column_config"])
         
         min_value= parse( value["min_value"] )
@@ -441,51 +449,51 @@
         if failed_records_count == 0:
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{value['min_value']},{value['max_value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the given column matches the given regex pattern or not.
-    def regex_check(self, df, rule):
+    def regex_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             ~col(rule["column_to_be_checked"]).rlike(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         test_status = "PASS" if failed_records_count == 0 else "FAIL"
 
         if failed_records_count > 0:
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(
                 f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df)
+                rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
-    def row_count_check(self, df, rule):
+    def row_count_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         failed_records_write_location = 'N/A'
         failed_records_count = total_row_count - int(rule["value"])
         if total_row_count == int(rule["value"]):
             test_status = "PASS"
         else:
             test_status = "FAIL"
             failed_df = self.spark.createDataFrame([], schema=df.schema).withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit("All columns")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
-                rule, failed_df, False)
+                rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
 # ----- Function takes the filepath of ruleset as an input and apply validations defined in the ruleset.
     def read_csv_input_and_apply_validation(self, rules_csv_file_path, result_summery_file_path, file_path=None):
         input_df = self.spark.read.option(
             "header", True).csv(rules_csv_file_path)
@@ -494,28 +502,28 @@
         self.tables_list = {**self.tables_list, **new_tables}
         new_dataframes = read_dataset(
             new_tables, self.data_read_ob, self.no_of_partition)
         if new_dataframes:
             self.dataframes = {**self.dataframes, **new_dataframes}
         self.df_rules_validation(rule_set, result_summery_file_path)
 
-    def apply_validation(self, rule_config_df, write_summary_on_database=True, failed_schema_source_list=[], output_summary_folder_path=''):
+    def apply_validation(self, rule_config_df, write_summary_on_database=True, failed_schema_source_list=[], output_summary_folder_path='', write_failed_records_flag=True):
         rule_set = rule_config_df.collect()
         new_tables = get_missing_tables(self.tables_list, rule_set)
         self.tables_list = {**self.tables_list, **new_tables}
         new_dataframes = read_dataset(
             new_tables, self.data_read_ob, self.no_of_partition)
         if new_dataframes:
             self.dataframes = {**self.dataframes, **new_dataframes}
         self.df_rules_validation(rule_set, write_summary_on_database,
-                                 failed_schema_source_list, output_summary_folder_path)
+                                 failed_schema_source_list, output_summary_folder_path, write_failed_records_flag)
 
     # ----- Function include all the above functions and apply rule set at once and gives a consolidated result.
 
-    def df_rules_validation(self, rule_set, write_summary_on_database, failed_schema_source_list, result_summary_folder_path):
+    def df_rules_validation(self, rule_set, write_summary_on_database, failed_schema_source_list, result_summary_folder_path, write_failed_records_flag):
         test_summary = []
         try:
             for rule in rule_set:
                 try:
                     source = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
                     if "failed_schema_source_list" in rule and rule['failed_schema_source_list'] in failed_schema_source_list:
                         run_date = date.today().strftime("%Y/%m/%d")
@@ -527,71 +535,71 @@
                         run_date = date.today().strftime("%Y/%m/%d")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "", "", "", "", 0, run_date))
                         continue
 
                     if rule["rule_name"] == "null_check":
                         result_df = self.null_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "schema_check":
                         result_df = self.schema_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "range_min_check":
                         result_df = self.range_min_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     #elif rule["rule_name"] == "range_min_inclusive_check":
                     #    result_df = self.range_min_inclusive_check(
-                    #       self.dataframes[source], rule)
+                    #       self.dataframes[source], rule, write_failed_records_flag)
                     #    test_summary.append(result_df)
                     elif rule["rule_name"] == "range_max_check":
                         result_df = self.range_max_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "length_check":
                         result_df = self.length_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "unique_keys_check":
                         result_df = self.unique_keys_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "unique_records_check":
                         result_df = self.unique_records_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "allowed_values_check":
                         result_df = self.allowed_values_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "min_length_check":
                         result_df = self.min_length_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "column_count_check":
                         result_df = self.column_count_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "not_allowed_values_check":
                         result_df = self.not_allowed_values_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "date_range_check":
                         result_df = self.date_range_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "regex_check":
                         result_df = self.regex_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "row_count_check":
                         result_df = self.row_count_check(
-                            self.dataframes[source], rule)
+                            self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
 
                     else:
                         run_date = date.today().strftime("%Y/%m/%d")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "invalid rule name", "", "", "", 0, run_date))
                         continue
```

### Comparing `dq_module-1.1.2/dq_module.egg-info/PKG-INFO` & `dq_module-1.1.3/dq_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq-module
-Version: 1.1.2
+Version: 1.1.3
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.2/dq_module.egg-info/SOURCES.txt` & `dq_module-1.1.3/dq_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.2/setup.py` & `dq_module-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COMMAND ----------
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
     
 setuptools.setup(
     name="dq_module",
-    version="1.1.2",
+    version="1.1.3",
     author="Sweta",
     author_email="sweta.swami@decisionpoint.in",
     description="data profiling and basic data quality rules check",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=setuptools.find_packages(include=['*']),
     packages=['dataqualitycheck', 'dataqualitycheck.datasources'],
```

