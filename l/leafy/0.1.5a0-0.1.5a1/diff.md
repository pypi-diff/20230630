# Comparing `tmp/leafy-0.1.5a0-cp39-cp39-win_amd64.whl.zip` & `tmp/leafy-0.1.5a1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 151476 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       24 b- defN 23-Jun-30 09:10 leafy/__init__.py
--rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-30 09:11 leafy/data_structure.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    66048 b- defN 23-Jun-30 09:11 leafy/digraph.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    72704 b- defN 23-Jun-30 09:11 leafy/graph.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-30 09:11 leafy/search.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    51712 b- defN 23-Jun-30 09:11 leafy/shortest_path.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-30 09:11 leafy-0.1.5a0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3113 b- defN 23-Jun-30 09:11 leafy-0.1.5a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-30 09:11 leafy-0.1.5a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-30 09:11 leafy-0.1.5a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      918 b- defN 23-Jun-30 09:11 leafy-0.1.5a0.dist-info/RECORD
-11 files, 358016 bytes uncompressed, 149926 bytes compressed:  58.1%
+Zip file size: 151486 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Jun-30 09:26 leafy/__init__.py
+-rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-30 09:26 leafy/data_structure.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    66048 b- defN 23-Jun-30 09:26 leafy/digraph.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    72704 b- defN 23-Jun-30 09:26 leafy/graph.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-30 09:26 leafy/search.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    51712 b- defN 23-Jun-30 09:26 leafy/shortest_path.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-30 09:26 leafy-0.1.5a1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3217 b- defN 23-Jun-30 09:26 leafy-0.1.5a1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-30 09:26 leafy-0.1.5a1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-30 09:26 leafy-0.1.5a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      918 b- defN 23-Jun-30 09:26 leafy-0.1.5a1.dist-info/RECORD
+11 files, 358120 bytes uncompressed, 149936 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: leafy/search.cp39-win_amd64.pyd
 Comment: 
 
 Filename: leafy/shortest_path.cp39-win_amd64.pyd
 Comment: 
 
-Filename: leafy-0.1.5a0.dist-info/LICENSE
+Filename: leafy-0.1.5a1.dist-info/LICENSE
 Comment: 
 
-Filename: leafy-0.1.5a0.dist-info/METADATA
+Filename: leafy-0.1.5a1.dist-info/METADATA
 Comment: 
 
-Filename: leafy-0.1.5a0.dist-info/WHEEL
+Filename: leafy-0.1.5a1.dist-info/WHEEL
 Comment: 
 
-Filename: leafy-0.1.5a0.dist-info/top_level.txt
+Filename: leafy-0.1.5a1.dist-info/top_level.txt
 Comment: 
 
-Filename: leafy-0.1.5a0.dist-info/RECORD
+Filename: leafy-0.1.5a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `leafy-0.1.5a0.dist-info/LICENSE` & `leafy-0.1.5a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `leafy-0.1.5a0.dist-info/METADATA` & `leafy-0.1.5a1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leafy
-Version: 0.1.5a0
+Version: 0.1.5a1
 Summary: Another fast graph algorithms library
 Home-page: https://github.com/ajaaliconsulting/leafy
 Author: Ahmed Ali
 Author-email: ahmed@ajaali.com
 License: MIT
 Keywords: graph dag algorithm library
 Platform: UNKNOWN
@@ -12,14 +12,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Leafy Graph Library
```

