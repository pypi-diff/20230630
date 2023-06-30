# Comparing `tmp/graphreduce-0.5.tar.gz` & `tmp/graphreduce-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-0.5.tar", last modified: Wed Jun 28 22:08:58 2023, max compression
+gzip compressed data, was "graphreduce-0.6.tar", last modified: Fri Jun 30 01:30:01 2023, max compression
```

## Comparing `graphreduce-0.5.tar` & `graphreduce-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-28 22:08:58.352928 graphreduce-0.5/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7932 2023-06-28 22:08:58.352799 graphreduce-0.5/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6958 2023-06-23 04:33:12.000000 graphreduce-0.5/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-28 22:08:58.351626 graphreduce-0.5/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.5/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-15 15:13:54.000000 graphreduce-0.5/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15607 2023-06-28 22:06:01.000000 graphreduce-0.5/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    11593 2023-06-28 17:47:28.000000 graphreduce-0.5/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-28 22:08:58.352651 graphreduce-0.5/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7932 2023-06-28 22:08:58.000000 graphreduce-0.5/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-28 22:08:58.000000 graphreduce-0.5/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-28 22:08:58.000000 graphreduce-0.5/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.5/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-06-28 22:08:58.000000 graphreduce-0.5/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-28 22:08:58.000000 graphreduce-0.5/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-28 22:08:58.352961 graphreduce-0.5/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-06-28 22:08:40.000000 graphreduce-0.5/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:30:01.932827 graphreduce-0.6/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 01:30:01.932711 graphreduce-0.6/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-0.6/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:30:01.931430 graphreduce-0.6/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.6/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-0.6/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16026 2023-06-30 01:28:08.000000 graphreduce-0.6/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    13223 2023-06-29 22:50:57.000000 graphreduce-0.6/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:30:01.932482 graphreduce-0.6/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.6/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-30 01:30:01.932866 graphreduce-0.6/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-06-30 01:29:56.000000 graphreduce-0.6/setup.py
```

### Comparing `graphreduce-0.5/PKG-INFO` & `graphreduce-0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.5
+Version: 0.6
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # GraphReduce
 
 
 ## Description
 GraphReduce is an abstraction for building machine learning feature
-engineering pipelines in a scalable, extensible, and production-ready way.
+engineering pipelines that involve many tables in a composable way.
 The library is intended to help bridge the gap between research feature
 definitions and production deployment without the overhead of a full 
 feature store.  Underneath the hood, GraphReduce uses graph data
 structures to represent tables/files as nodes and foreign keys
 as edges.
 
 GraphReduce allows for a unified feature engineering interface
```

### Comparing `graphreduce-0.5/README.md` & `graphreduce-0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GraphReduce
 
 
 ## Description
 GraphReduce is an abstraction for building machine learning feature
-engineering pipelines in a scalable, extensible, and production-ready way.
+engineering pipelines that involve many tables in a composable way.
 The library is intended to help bridge the gap between research feature
 definitions and production deployment without the overhead of a full 
 feature store.  Underneath the hood, GraphReduce uses graph data
 structures to represent tables/files as nodes and foreign keys
 as edges.
 
 GraphReduce allows for a unified feature engineering interface
```

### Comparing `graphreduce-0.5/graphreduce/graph_reduce.py` & `graphreduce-0.6/graphreduce/graph_reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -227,15 +227,21 @@
             if "key_0" in joined.columns:
                 joined = joined[[c for c in joined.columns if c != "key_0"]]
                 return joined
             else:
                 return joined
                             
         elif self.compute_layer == ComputeLayerEnum.spark:     
-            if isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame) and isinstance(relation_node.df, pyspark.sql.dataframe.DataFrame):
+            if isinstance(relation_df, pyspark.sql.dataframe.DataFrame) and isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame):
+                joined = parent_node.df.join(
+                        relation_df,
+                        on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"] == relation_df[f"{relation_node.prefix}_{relation_fk}"],
+                        how="left"
+                        )
+            elif isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame) and isinstance(relation_node.df, pyspark.sql.dataframe.DataFrame):
                 joined = parent_node.df.join(
                     relation_node.df,
                     on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"] == relation_node.df[f"{relation_node.prefix}_{relation_fk}"],
                     how="left"
                 ) 
                 return joined
             else:
```

### Comparing `graphreduce-0.5/graphreduce/node.py` & `graphreduce-0.6/graphreduce/node.py`

 * *Files 17% similar despite different names*

```diff
@@ -251,70 +251,110 @@
     @abc.abstractmethod
     def do_labels(self, reduce_key):
         pass
     
         
     def colabbr(self, col: str) -> str:
         return f"{self.prefix}_{col}"
+
+
+    def compute_period_minutes (
+            self,
+            ) -> int:
+        """
+Convert the compute period to minutes
+        """
+        if self.compute_period_unit == PeriodUnit.second:
+            return self.compute_period_val / 60
+        elif self.compute_period_unit == PeriodUnit.minute:
+            return self.compute_period_val
+        elif self.compute_period_unit == PeriodUnit.hour:
+            return self.compute_period_val * 60
+        elif self.compute_period_unit == PeriodUnit.day:
+            return self.compute_period_val * 1440
+        elif self.compute_period_unit == PeriodUnit.week:
+            return (self.compute_period_val * 7)*1440
+        elif self.compute_period_unit == PeriodUnit.month:
+            return (self.compute_period_val * 30.417)*1440
+
+
+    def label_period_minutes (
+            self,
+            ) -> int:
+        """
+Convert the label period to minutes
+        """
+        if self.label_period_unit == PeriodUnit.second:
+            return self.label_period_val / 60
+        elif self.label_period_unit == PeriodUnit.minute:
+            return self.label_period_val
+        elif self.label_period_unit == PeriodUnit.hour:
+            return self.label_period_val * 60
+        elif self.label_period_unit == PeriodUnit.day:
+            return self.label_period_val * 1440
+        elif self.label_period_unit == PeriodUnit.week:
+            return (self.label_period_val * 7)*1440
+        elif self.label_period_unit == PeriodUnit.month:
+            return (self.label_period_val * 30.417)*1440
     
     
     def prep_for_features(self):
         """
 Prepare the dataset for feature aggregations / reduce
         """
-        if self.date_key:
+        if self.date_key:           
             if self.cut_date and isinstance(self.cut_date, str) or isinstance(self.cut_date, datetime.datetime):
                 if isinstance(self.df, pd.DataFrame) or isinstance(self.df, dd.DataFrame):
                     return self.df[
                         (self.df[self.colabbr(self.date_key)] < self.cut_date)
                         &
-                        (self.df[self.colabbr(self.date_key)] > (self.cut_date - datetime.timedelta(days=self.compute_period_val)))
+                        (self.df[self.colabbr(self.date_key)] > (self.cut_date - datetime.timedelta(minutes=self.compute_period_minutes())))
                     ]
                 elif isinstance(self.df, pyspark.sql.dataframe.DataFrame):
                     return self.df.filter(
                         (self.df[self.colabbr(self.date_key)] < self.cut_date)
                         &
-                        (self.df[self.colabbr(self.date_key)] > (self.cut_date - datetime.timedelta(days=self.compute_period_val)))
+                        (self.df[self.colabbr(self.date_key)] > (self.cut_date - datetime.timedelta(minutes=self.compute_period_minutes())))
                     )
             else:
                 if isinstance(self.df, pd.DataFrame) or isinstance(self.df, dd.DataFrame):
                     return self.df[
                         (self.df[self.colabbr(self.date_key)] < datetime.datetime.now())
                         &
-                        (self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(days=self.compute_period_val)))
+                        (self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.compute_period_minutes())))
                     ]
                 elif isinstance(self.df, pyspark.sql.dataframe.DataFrame):
                     return self.df.filter(
-                        self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(days=self.compute_period_val))
+                        self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.compute_period_minutes()))
                 )
         # no-op
         return self.df
     
     
     def prep_for_labels(self):
         """
 Prepare the dataset for labels
         """
         if self.date_key:
             if self.cut_date and isinstance(self.cut_date, str) or isinstance(self.cut_date, datetime.datetime):
                 if isinstance(self.df, pd.DataFrame):
                     return self.df[
-                        (self.df[self.colabbr(self.date_key)] > (self.cut_date))
+                        (self.df[self.colabbr(self.date_key)] > self.cut_date)
                         &
-                        (self.df[self.colabbr(self.date_key)] < (self.cut_date + datetime.timedelta(days=self.label_period_val)))
+                        (self.df[self.colabbr(self.date_key)] < (self.cut_date + datetime.timedelta(minutes=self.label_period_minutes())))
                     ]
                 elif isinstance(self.df, pyspark.sql.dataframe.DataFrame):
                     return self.df.filter(
-                        (self.df[self.colabbr(self.date_key)] > (self.cut_date))
+                        (self.df[self.colabbr(self.date_key)] > self.cut_date)
                         &
-                        (self.df[self.colabbr(self.date_key)] < (self.cutDate + datetime.timedelta(days=self.label_period_val)))
+                        (self.df[self.colabbr(self.date_key)] < (self.cut_date + datetime.timedelta(minutes=self.label_period_minutes())))
                     )
             else:
                 if isinstance(self.df, pd.DataFrame):
                     return self.df[
-                        self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(days=self.label_period_val))
+                        self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.label_period_minutes()))
                     ]
                 elif isinstance(self.df, pyspark.sql.dataframe.DataFrame):
                     return self.df.filter(
-                    self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(days=self.label_period_val))
+                    self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.label_period_minutes()))
                 )
         return self.df
```

### Comparing `graphreduce-0.5/graphreduce.egg-info/PKG-INFO` & `graphreduce-0.6/graphreduce.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.5
+Version: 0.6
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # GraphReduce
 
 
 ## Description
 GraphReduce is an abstraction for building machine learning feature
-engineering pipelines in a scalable, extensible, and production-ready way.
+engineering pipelines that involve many tables in a composable way.
 The library is intended to help bridge the gap between research feature
 definitions and production deployment without the overhead of a full 
 feature store.  Underneath the hood, GraphReduce uses graph data
 structures to represent tables/files as nodes and foreign keys
 as edges.
 
 GraphReduce allows for a unified feature engineering interface
```

### Comparing `graphreduce-0.5/setup.py` & `graphreduce-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 0.5,
+        version = 0.6,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

