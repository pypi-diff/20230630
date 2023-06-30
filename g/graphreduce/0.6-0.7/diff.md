# Comparing `tmp/graphreduce-0.6.tar.gz` & `tmp/graphreduce-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-0.6.tar", last modified: Fri Jun 30 01:30:01 2023, max compression
+gzip compressed data, was "graphreduce-0.7.tar", last modified: Fri Jun 30 01:44:49 2023, max compression
```

## Comparing `graphreduce-0.6.tar` & `graphreduce-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:30:01.932827 graphreduce-0.6/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 01:30:01.932711 graphreduce-0.6/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-0.6/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:30:01.931430 graphreduce-0.6/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.6/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-0.6/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16026 2023-06-30 01:28:08.000000 graphreduce-0.6/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    13223 2023-06-29 22:50:57.000000 graphreduce-0.6/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:30:01.932482 graphreduce-0.6/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.6/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-30 01:30:01.000000 graphreduce-0.6/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-30 01:30:01.932866 graphreduce-0.6/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-06-30 01:29:56.000000 graphreduce-0.6/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:44:49.723506 graphreduce-0.7/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 01:44:49.723387 graphreduce-0.7/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-0.7/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:44:49.722276 graphreduce-0.7/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.7/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-0.7/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16056 2023-06-30 01:37:39.000000 graphreduce-0.7/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    13223 2023-06-29 22:50:57.000000 graphreduce-0.7/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-30 01:44:49.723243 graphreduce-0.7/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-06-30 01:44:49.000000 graphreduce-0.7/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-30 01:44:49.000000 graphreduce-0.7/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-30 01:44:49.000000 graphreduce-0.7/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.7/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-06-30 01:44:49.000000 graphreduce-0.7/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-30 01:44:49.000000 graphreduce-0.7/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-30 01:44:49.723541 graphreduce-0.7/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-06-30 01:37:52.000000 graphreduce-0.7/setup.py
```

### Comparing `graphreduce-0.6/PKG-INFO` & `graphreduce-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.6
+Version: 0.7
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-0.6/README.md` & `graphreduce-0.7/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-0.6/graphreduce/graph_reduce.py` & `graphreduce-0.7/graphreduce/graph_reduce.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
         elif self.compute_layer == ComputeLayerEnum.spark:     
             if isinstance(relation_df, pyspark.sql.dataframe.DataFrame) and isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame):
                 joined = parent_node.df.join(
                         relation_df,
                         on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"] == relation_df[f"{relation_node.prefix}_{relation_fk}"],
                         how="left"
                         )
+                return joined
             elif isinstance(parent_node.df, pyspark.sql.dataframe.DataFrame) and isinstance(relation_node.df, pyspark.sql.dataframe.DataFrame):
                 joined = parent_node.df.join(
                     relation_node.df,
                     on=parent_node.df[f"{parent_node.prefix}_{parent_pk}"] == relation_node.df[f"{relation_node.prefix}_{relation_fk}"],
                     how="left"
                 ) 
                 return joined
```

### Comparing `graphreduce-0.6/graphreduce/node.py` & `graphreduce-0.7/graphreduce/node.py`

 * *Files identical despite different names*

### Comparing `graphreduce-0.6/graphreduce.egg-info/PKG-INFO` & `graphreduce-0.7/graphreduce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.6
+Version: 0.7
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-0.6/setup.py` & `graphreduce-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 0.6,
+        version = 0.7,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

