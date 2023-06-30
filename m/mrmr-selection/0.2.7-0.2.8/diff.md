# Comparing `tmp/mrmr_selection-0.2.7-py3-none-any.whl.zip` & `tmp/mrmr_selection-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15089 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      185 b- defN 23-May-29 21:01 mrmr/__init__.py
+Zip file size: 15149 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      185 b- defN 23-Jun-30 19:29 mrmr/__init__.py
 -rw-rw-rw-  2.0 fat    12053 b- defN 22-Feb-18 21:49 mrmr/bigquery.py
 -rw-rw-rw-  2.0 fat     5755 b- defN 22-Feb-18 21:29 mrmr/main.py
 -rw-rw-rw-  2.0 fat    11095 b- defN 22-Apr-23 18:25 mrmr/pandas.py
 -rw-rw-rw-  2.0 fat     8613 b- defN 23-May-28 22:00 mrmr/polars.py
 -rw-rw-rw-  2.0 fat     8402 b- defN 22-Feb-19 16:57 mrmr/spark.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6024 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      848 b- defN 23-May-29 21:12 mrmr_selection-0.2.7.dist-info/RECORD
-11 files, 54159 bytes uncompressed, 13673 bytes compressed:  74.8%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-30 19:32 mrmr_selection-0.2.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6633 b- defN 23-Jun-30 19:32 mrmr_selection-0.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 19:32 mrmr_selection-0.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jun-30 19:32 mrmr_selection-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      848 b- defN 23-Jun-30 19:32 mrmr_selection-0.2.8.dist-info/RECORD
+11 files, 54768 bytes uncompressed, 13733 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mrmr/polars.py
 Comment: 
 
 Filename: mrmr/spark.py
 Comment: 
 
-Filename: mrmr_selection-0.2.7.dist-info/LICENSE
+Filename: mrmr_selection-0.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: mrmr_selection-0.2.7.dist-info/METADATA
+Filename: mrmr_selection-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: mrmr_selection-0.2.7.dist-info/WHEEL
+Filename: mrmr_selection-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: mrmr_selection-0.2.7.dist-info/top_level.txt
+Filename: mrmr_selection-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mrmr_selection-0.2.7.dist-info/RECORD
+Filename: mrmr_selection-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mrmr/__init__.py

```diff
@@ -1,8 +1,8 @@
 from . import bigquery
 from . import pandas
 from . import polars
 from . import spark
 from .pandas import mrmr_classif, mrmr_regression
 from .main import mrmr_base
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

## Comparing `mrmr_selection-0.2.7.dist-info/LICENSE` & `mrmr_selection-0.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mrmr_selection-0.2.7.dist-info/METADATA` & `mrmr_selection-0.2.8.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrmr-selection
-Version: 0.2.7
+Version: 0.2.8
 Summary: minimum-Redundancy-Maximum-Relevance algorithm for feature selection
 Home-page: https://github.com/smazzanti/mrmr
 Author: Samuele Mazzanti
 Author-email: mazzanti.sam@gmail.com
 License: GNU General Public License v3.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: jinja2
 Requires-Dist: tqdm
 Requires-Dist: joblib
 Requires-Dist: pandas (>=1.0.3)
 Requires-Dist: numpy (>=1.18.1)
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
+Requires-Dist: polars (>=0.12.5)
 
 <p align="center">
 <img src="./docs/img/mrmr_logo_white_bck.png" alt="drawing" width="450"/>
 </p>
 
 ## What is mRMR
 
@@ -66,15 +67,16 @@
 </pre>
 
 ## How to use this package
 
 This package is designed to do *mRMR* selection through different tools, depending on your needs and constraints.
 
 Currently, the following tools are supported (others will be added):
-- **Pandas** (in-memory)
+- **Pandas**
+- **Polars**
 - **Spark**
 - **Google BigQuery**
 
 The package has a module for each supported tool. Each module has *at least* these 2 functions:
 - `mrmr_classif`, for feature selection when the target variable is categorical (binary or multiclass).
 - `mrmr_regression`, for feature selection when the target variable is numeric.
 
@@ -95,15 +97,33 @@
 # select top 10 features using mRMR
 from mrmr import mrmr_classif
 selected_features = mrmr_classif(X=X, y=y, K=10)
 ```
 
 Note: the output of mrmr_classif is a list containing K selected features. This is a **ranking**, therefore, if you want to make a further selection, take the first elements of this list.
 
-#### 2. Spark example
+#### 2. Polars example
+
+```python
+# create some polars data
+import polars
+data = [(1.0, 1.0, 1.0, 7.0, 1.5, -2.3), 
+        (2.0, None, 2.0, 7.0, 8.5, 6.7), 
+        (2.0, None, 3.0, 7.0, -2.3, 4.4),
+        (3.0, 4.0, 3.0, 7.0, 0.0, 0.0),
+        (4.0, 5.0, 4.0, 7.0, 12.1, -5.2)]
+columns = ["target", "some_null", "feature", "constant", "other_feature", "another_feature"]
+df_polars = polars.DataFrame(data=data, schema=columns)
+
+# select top 2 features using mRMR
+import mrmr
+selected_features = mrmr.polars.mrmr_regression(df=df_polars, target_column="target", K=2)
+```
+
+#### 3. Spark example
 
 ```python
 # create some spark data
 import pyspark
 session = pyspark.sql.SparkSession(pyspark.context.SparkContext())
 data = [(1.0, 1.0, 1.0, 7.0, 1.5, -2.3), 
         (2.0, float('NaN'), 2.0, 7.0, 8.5, 6.7), 
@@ -114,15 +134,15 @@
 df_spark = session.createDataFrame(data=data, schema=columns)
 
 # select top 2 features using mRMR
 import mrmr
 selected_features = mrmr.spark.mrmr_regression(df=df_spark, target_column="target", K=2)
 ```
 
-#### 3. Google BigQuery example
+#### 4. Google BigQuery example
 
 ```python
 # initialize BigQuery client
 from google.cloud.bigquery import Client
 bq_client = Client(credentials=your_credentials)
 
 # select top 20 features using mRMR
```

