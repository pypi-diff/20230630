# Comparing `tmp/ecopipeline-0.0.8.tar.gz` & `tmp/ecopipeline-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.8.tar", last modified: Mon Apr 17 22:11:58 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.9.tar", last modified: Mon Apr 17 22:44:35 2023, max compression
```

## Comparing `ecopipeline-0.0.8.tar` & `ecopipeline-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:11:58.200955 ecopipeline-0.0.8/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1086 2023-04-17 22:11:58.222247 ecopipeline-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      735 2023-04-17 22:11:58.261081 ecopipeline-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:11:56.592953 ecopipeline-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 22:11:57.604954 ecopipeline-0.0.8/src/ecopipeline/
--rw-rw-rw-   0        0        0     2105 2023-04-17 22:11:31.000000 ecopipeline-0.0.8/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.8/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.8/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    14785 2023-04-17 21:25:54.000000 ecopipeline-0.0.8/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.8/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.8/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    30761 2023-04-17 21:59:13.000000 ecopipeline-0.0.8/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2780 2023-04-14 17:28:33.000000 ecopipeline-0.0.8/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:11:58.116955 ecopipeline-0.0.8/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1086 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-17 22:11:56.000000 ecopipeline-0.0.8/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 22:44:35.644509 ecopipeline-0.0.9/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1086 2023-04-17 22:44:35.661803 ecopipeline-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      735 2023-04-17 22:44:35.705168 ecopipeline-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:44:33.920505 ecopipeline-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 22:44:35.116508 ecopipeline-0.0.9/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2105 2023-04-17 22:11:31.000000 ecopipeline-0.0.9/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.9/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.9/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    14785 2023-04-17 21:25:54.000000 ecopipeline-0.0.9/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.9/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.9/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    30775 2023-04-17 22:44:00.000000 ecopipeline-0.0.9/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2780 2023-04-14 17:28:33.000000 ecopipeline-0.0.9/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:44:35.564509 ecopipeline-0.0.9/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1086 2023-04-17 22:44:33.000000 ecopipeline-0.0.9/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-17 22:44:33.000000 ecopipeline-0.0.9/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:44:33.000000 ecopipeline-0.0.9/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-17 22:44:33.000000 ecopipeline-0.0.9/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 22:44:33.000000 ecopipeline-0.0.9/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.8/PKG-INFO` & `ecopipeline-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ecopipeline-0.0.8/README.md` & `ecopipeline-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/setup.cfg` & `ecopipeline-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 390d  version = 0.0.9.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
```

### Comparing `ecopipeline-0.0.8/src/ecopipeline/__init__.py` & `ecopipeline-0.0.9/src/ecopipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline/bayview.py` & `ecopipeline-0.0.9/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline/config.py` & `ecopipeline-0.0.9/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline/extract.py` & `ecopipeline-0.0.9/src/ecopipeline/extract.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.9/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline/load.py` & `ecopipeline-0.0.9/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline/transform.py` & `ecopipeline-0.0.9/src/ecopipeline/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         col (pd.Series): Pandas series
         ffill_df (pd.DataFrame): Pandas dataframe
     Returns: 
         None (df is modified, not returned)
     """
     if (col.name in ffill_df.index):
         #set initial fill value where needed for first row
-        if previous_fill is not None and len(col) > 0 and col[0] == np.nan:
-            col[0] = previous_fill[col.name][0]
+        if previous_fill is not None and len(col) > 0 and pd.isna(col.iloc[0]):
+            col.iloc[0] = previous_fill[col.name].iloc[0]
         cp = ffill_df.loc[col.name]["changepoint"]
         length = ffill_df.loc[col.name]["ffill_length"]
         if (length != length):  # check for nan, set to 0
             length = 0
         length = int(length)  # casting to int to avoid float errors
         if (cp == 1):  # ffill unconditionally
             col.fillna(method='ffill', inplace=True)
```

### Comparing `ecopipeline-0.0.8/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.9/src/ecopipeline/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.8/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.9/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

