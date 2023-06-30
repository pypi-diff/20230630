# Comparing `tmp/Digital_Farming_Solution-0.1.2.tar.gz` & `tmp/Digital_Farming_Solution-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Farming_Solution-0.1.2.tar", last modified: Tue Jun 27 10:31:50 2023, max compression
+gzip compressed data, was "Digital_Farming_Solution-0.1.3.tar", last modified: Fri Jun 30 09:08:47 2023, max compression
```

## Comparing `Digital_Farming_Solution-0.1.2.tar` & `Digital_Farming_Solution-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 10:31:50.838976 Digital_Farming_Solution-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-27 10:31:50.696801 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/
--rw-rw-rw-   0        0        0     6912 2023-06-27 10:30:05.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/Select_options.py
--rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 10:31:50.791151 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/
--rw-rw-rw-   0        0        0      609 2023-06-27 10:31:49.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-27 10:31:50.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 10:31:49.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-27 10:31:49.000000 Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-06-27 10:31:50.806305 Digital_Farming_Solution-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-27 10:31:50.840947 Digital_Farming_Solution-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      771 2023-06-27 10:31:05.000000 Digital_Farming_Solution-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:08:47.393730 Digital_Farming_Solution-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-30 09:08:47.207816 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/
+-rw-rw-rw-   0        0        0     7800 2023-06-30 09:08:01.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/Select_options.py
+-rw-rw-rw-   0        0        0        2 2023-06-25 10:57:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:08:47.383755 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      609 2023-06-30 09:08:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-30 09:08:46.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:08:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-30 09:08:45.000000 Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-06-30 09:08:47.391739 Digital_Farming_Solution-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:08:47.394727 Digital_Farming_Solution-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-06-27 12:08:01.000000 Digital_Farming_Solution-0.1.3/setup.py
```

### Comparing `Digital_Farming_Solution-0.1.2/Digital_Farming_Solution/Select_options.py` & `Digital_Farming_Solution-0.1.3/Digital_Farming_Solution/Select_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
+import boto3
 
+# Get the Data From the AWS S3 buket
+
+def Get_Data_from_S3_Bucket(aws_access_key_id, aws_secret_access_key, bucket_name, file_path):
+    s3 = boto3.client("s3", 
+                      aws_access_key_id = aws_access_key_id,
+                      aws_secret_access_key=aws_secret_access_key)
+    
+    obj = s3.get_object(Bucket=bucket_name, Key=file_path)
+ 
+    try:
+        df = pd.read_csv(obj["Body"])
+        
+        return df
+    
+    except:
+        
+        df = pd.read_excel(obj["Body"])
+   
+        return df
+
+
+# Binning the Yield
 def Yield_Binning(datframe,column):
     
     # Filling the Missing Values   
     datframe[column] = datframe[column].fillna(datframe[column].mean())
     
     # Calculating the yield quantiles
     col_values = list(datframe[column])
@@ -26,15 +49,15 @@
             datframe.at[index,'Category'] = 'Medium High'
             
         else:
             datframe.at[index,'Category'] = 'High'
 
     return datframe
 
-#######################################################################################################
+#################################################################
 
 # Creating the function for Yield binning Ranges Values
 def Yield_Binning_Ranges_Values(data,Yield_column_name):
     
     df_new = data[[Yield_column_name]]
     
     #Removing the null values
@@ -71,16 +94,17 @@
             df_new.at[index,'% of Yield Range'] = '>76'
     
     df_final = df_new.groupby(['% of Yield Range','Yeild Category']).agg(min=(Yield_column_name, 'min'),max=(Yield_column_name, 'max'), mean=(Yield_column_name, 'mean'),
                                                                          median=(Yield_column_name, 'median')).sort_values('mean')
     
     return df_final
 
-##################################################################################################
+#############################################################################################################################################################################
 
+# Getting the delta change for palnting and Harvest dates
 def Delta_Change(data, Yield_cloumn, by, return_dataframe = True):
 
     # Storing the column Name
     column_name = by
     # Converting the string data type  into datetime format
 
     data[column_name] = pd.to_datetime(data[column_name])
@@ -118,16 +142,17 @@
     
     else:
         
         fig = px.scatter(data, x= 'Month_Date', y="Avg_yield", size='Avg_yield',color = 'Month',title= 'Delta Change by ' + column_name +' .')
         
         fig.show()
 
-################################################################################################
+#################################################################################################################################################
 
+# Getting the Best planting and Harvest Dates
 def Best_Dates(data,Yield_cloumn,by,Season = False,return_dataframe = True):
     
     # Storing the name 
     column_name = by
     
     if Season == True:
     
@@ -182,8 +207,11 @@
             return data
         
         else:
             
             fig = px.bar(data, x= 'Month_Date', y='Avg_yield')
             fig.update_layout(title = 'Best ' + column_name +' in the Season', yaxis_title = 'Average Yield') 
             fig.show()
-        
+        
+
+################################################################################################################
+
```

### Comparing `Digital_Farming_Solution-0.1.2/Digital_Farming_Solution.egg-info/PKG-INFO` & `Digital_Farming_Solution-0.1.3/Digital_Farming_Solution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital-Farming-Solution
-Version: 0.1.2
+Version: 0.1.3
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.2/PKG-INFO` & `Digital_Farming_Solution-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digital_Farming_Solution
-Version: 0.1.2
+Version: 0.1.3
 Summary:  The packages are helps to the DFS Teams to perform some of the task easily.
 Author: Bharatesha N S
 Author-email: bharatesha.ns.ext@bayer.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Digital_Farming_Solution-0.1.2/setup.py` & `Digital_Farming_Solution-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Digital_Farming_Solution",
-    version="0.1.2",
+    version="0.1.3",
     author="Bharatesha N S",
     author_email="bharatesha.ns.ext@bayer.com",
     description=" The packages are helps to the DFS Teams to perform some of the task easily.",
     long_description= 'By importing this packages we can work on easily and  get some meaningfull information.It is more siutable for the dataframe works and it will returnns the Dataframe.',
     long_description_content_type="text/markdown",
     packages=["Digital_Farming_Solution"],
     classifiers=[
```

