# Comparing `tmp/veetility-0.1.92.tar.gz` & `tmp/veetility-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.92.tar", last modified: Fri Jun 23 10:57:32 2023, max compression
+gzip compressed data, was "veetility-0.1.93.tar", last modified: Fri Jun 30 16:47:07 2023, max compression
```

## Comparing `veetility-0.1.92.tar` & `veetility-0.1.93.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.495826 veetility-0.1.92/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-23 10:57:32.495613 veetility-0.1.92/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.92/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-23 10:57:32.495879 veetility-0.1.92/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-23 10:57:23.000000 veetility-0.1.92/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.490158 veetility-0.1.92/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.92/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.92/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.92/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.494067 veetility-0.1.92/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.92/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-12 11:29:12.000000 veetility-0.1.92/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.92/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.92/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    30693 2023-06-23 10:56:40.000000 veetility-0.1.92/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.92/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-12 19:20:06.000000 veetility-0.1.92/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.92/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.92/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.495376 veetility-0.1.92/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.903759 veetility-0.1.93/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-30 16:47:07.903602 veetility-0.1.93/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.93/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-30 16:47:07.903812 veetility-0.1.93/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-30 16:46:59.000000 veetility-0.1.93/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.898795 veetility-0.1.93/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.93/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.93/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.93/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.902376 veetility-0.1.93/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.93/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.93/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.93/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.93/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31084 2023-06-30 16:44:04.000000 veetility-0.1.93/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.93/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-26 09:44:14.000000 veetility-0.1.93/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.93/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.93/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-30 16:47:07.903382 veetility-0.1.93/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-30 16:47:07.000000 veetility-0.1.93/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.92/PKG-INFO` & `veetility-0.1.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.92
+Version: 0.1.93
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.92/README.md` & `veetility-0.1.93/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/setup.py` & `veetility-0.1.93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.92",
+    version="0.1.93",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.92/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.93/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/tests/test_identify_match_multi_cols.py` & `veetility-0.1.93/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/tests/test_prepare_string_matching.py` & `veetility-0.1.93/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/cleaning_functions.py` & `veetility-0.1.93/veetility/cleaning_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/generic_functions.py` & `veetility-0.1.93/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/point_to_point_regressor.py` & `veetility-0.1.93/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/quality_assessments.py` & `veetility-0.1.93/veetility/quality_assessments.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,35 +192,41 @@
                 columns have been added or removed next time, in which case it is deemed an error has occured.
             raise_exceptions (bool): If true, then raise an exception if an error has occured instead of just returning an error message.
 
         Returns:
             error_message (str): String detailing what the error is so that it can be passed to a notification service like slack."""
         
         error_message, error_occured = '', False
+
+        # Create a dictionary of the sums of the columns specified in cols_to_check
         new_dict = {}
-        new_dict['datetime'] = str(datetime.now())
+        new_dict['Date'] = str(datetime.now())
         for col in cols_to_check:
             new_dict[col] = int(df[col].sum())
-
         if check_cols_set == True:
             new_dict['Columns'] = df.columns.tolist()
-
-        if os.path.isdir('Historic df Comparison (Do Not Delete)') == False:
-            os.mkdir('Historic df Comparison (Do Not Delete)')
-        if os.path.exists(f'Historic df Comparison (Do Not Delete)/{name_of_df}_previous_totals.json') ==False:
-            self.util.write_json(new_dict, f'{name_of_df}_previous_totals', file_type='append', folder='Historic df Comparison (Do Not Delete)/')
-            logger.info(f"Creation of {name_of_df}_previous_totals")
-            logger.info(new_dict)
-            return error_message
+        
+        # Check if the historic database already exists, if not create it
+        client_name = self.util.client_name.lower()
+        if self.util.table_exists(f'{client_name}_{name_of_df}_previous_totals'):
+            historic_db = self.util.read_from_postgresql(f'{client_name}_{name_of_df}_previous_totals', clean_date=False)
+            historic_db.drop(columns=['DateWrittenToDB'], inplace=True) # This column is not needed for comparison, it gets created when writing to the db
+            historic_db = historic_db.reset_index()
         else:
-            #old_dict = self.util.unpickle_data(f'{name_of_df}_previous_totals', folder='Historic df Comparison (Do Not Delete)')
-            old_dict_file = self.util.read_json(f'{name_of_df}_previous_totals', folder='Historic df Comparison (Do Not Delete)',
-                                                    file_type='append')
-            old_dict = old_dict_file[-1] # Grab the lastest entry in the json file, descending date order
+            columns = ['Date'].extend(cols_to_check)
+            if check_cols_set == True:
+                columns.append('Columns')
+            historic_db = pd.DataFrame(columns=columns)
+            self.util.write_to_postgresql(historic_db, f'{client_name}_{name_of_df}_previous_totals', if_exists='replace')
+            return error_message
         
+        #Turn the most recent entry in the historic db into a dict
+        old_dict = historic_db.sort_values(by='Date', ascending=False).iloc[0].to_dict()
+
+        # for each key in the old dict, check if it is in the new dict and if it is, check if it has increased or decreased too much
         for key, value in old_dict.items():
             if key == 'Columns':
                 if set(value) != set(new_dict['Columns']):
                     error_occured = True
                     columns_removed = list(set(value) - set(new_dict['Columns']))
                     columns_added = list(set(new_dict['Columns']) - set(value))
                     error_message = error_message + '  ' + f'The columns seems to have changed from last time,\n'\
@@ -239,17 +245,17 @@
                                         f' Prev Value = {old_dict[key]}, New Value = {new_dict[key]}\n'
 
         if error_occured:
             error_message = f'Comparison with historic df {name_of_df}: ' + error_message +'\n'
             logger.info('ERROR' + error_message) # If error messages has been added to then log it
         if raise_exceptions and error_occured:
             raise Exception(error_message)
-        #self.util.pickle_data(new_dict, f'{name_of_df}_previous_totals', folder='Historic df Comparison (Do Not Delete)/')
-        self.util.write_json(new_dict, f'{name_of_df}_previous_totals', file_type='append',
-                             folder='Historic df Comparison (Do Not Delete)/')
+        
+        db_with_new_row = pd.concat([historic_db, pd.DataFrame(new_dict, index=[0])], ignore_index=True)
+        self.util.write_to_postgresql(db_with_new_row, f'{client_name}_{name_of_df}_previous_totals', if_exists='append')
         
         return error_message
     
     def duplicates_qa(self, df: pd.DataFrame, df_name: str, subset= None, drop_duplicates: bool = True):
         """Checks for duplicates and optionally drops duplicates in a dataframe.
         
         Args:
@@ -455,16 +461,20 @@
                     return "Correct"
                 else:
                     return 'Incorrect Value'
 
         
         for level in conv_level_tuple:
             checking_cols = []
+            if 'video_views' in df.columns:
+                cols_to_sum = [spend_col, 'video_views']
+            else:
+                cols_to_sum = spend_col
             #For each level of the naming convention, i.e. campaign, adgroup, adname
-            output_df = round(df.groupby(level[1])[spend_col].sum().reset_index(),1)
+            output_df = round(df.groupby(level[1])[cols_to_sum].sum().reset_index(),1)
             if level[0] == None: continue #no convention dict provided therefore ignore
             for label,tag in level[0].items():
                 #For each label and tag in the required set 
                 if label in key_values_conv_cols:
                     acceptable_values= remove_empties_from_list(naming_convention[label+' Key'].str.upper().unique().tolist())
                     output_df[f'{label} ("{tag}")'] = output_df[level[1]].apply(lambda x: return_value(x, tag, acceptable_values))
                     checking_cols.append(f'{label} ("{tag}")')
```

### Comparing `veetility-0.1.92/veetility/snowflake.py` & `veetility-0.1.93/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/utility_functions.py` & `veetility-0.1.93/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/v_lift.py` & `veetility-0.1.93/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility/view_through_rate.py` & `veetility-0.1.93/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.92/veetility.egg-info/PKG-INFO` & `veetility-0.1.93/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.92
+Version: 0.1.93
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.92/veetility.egg-info/SOURCES.txt` & `veetility-0.1.93/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

