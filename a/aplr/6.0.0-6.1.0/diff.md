# Comparing `tmp/aplr-6.0.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-6.1.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 345352 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   388608 b- defN 23-Jun-29 17:15 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   410624 b- defN 23-Jun-29 17:20 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-29 17:08 aplr/__init__.py
--rw-rw-rw-  2.0 fat    10532 b- defN 23-Jun-29 17:08 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-Jun-29 17:20 aplr-6.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      655 b- defN 23-Jun-29 17:20 aplr-6.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jun-29 17:20 aplr-6.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-29 17:20 aplr-6.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      691 b- defN 23-Jun-29 17:20 aplr-6.0.0.dist-info/RECORD
-9 files, 812384 bytes uncompressed, 344180 bytes compressed:  57.6%
+Zip file size: 345958 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   390144 b- defN 23-Jun-30 15:26 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   411136 b- defN 23-Jun-30 15:30 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-30 15:21 aplr/__init__.py
+-rw-rw-rw-  2.0 fat    10642 b- defN 23-Jun-30 15:21 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-Jun-30 15:30 aplr-6.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      655 b- defN 23-Jun-30 15:30 aplr-6.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jun-30 15:30 aplr-6.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-30 15:30 aplr-6.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      691 b- defN 23-Jun-30 15:30 aplr-6.1.0.dist-info/RECORD
+9 files, 814542 bytes uncompressed, 344786 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-6.0.0.dist-info/LICENSE
+Filename: aplr-6.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-6.0.0.dist-info/METADATA
+Filename: aplr-6.1.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-6.0.0.dist-info/WHEEL
+Filename: aplr-6.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-6.0.0.dist-info/top_level.txt
+Filename: aplr-6.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-6.0.0.dist-info/RECORD
+Filename: aplr-6.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -81,14 +81,17 @@
 
     def get_feature_importance(self)->npt.ArrayLike:
         return self.APLRRegressor.get_feature_importance()
 
     def get_intercept(self)->float:
         return self.APLRRegressor.get_intercept()
 
+    def get_intercept_steps(self)->npt.ArrayLike:
+        return self.APLRRegressor.get_intercept_steps()
+
     def get_optimal_m(self)->int:
         return self.APLRRegressor.get_optimal_m()
     
     def get_validation_tuning_metric(self)->str:
         return self.APLRRegressor.get_validation_tuning_metric()
  
     def get_validation_indexes(self)->List[int]:
```

## Comparing `aplr-6.0.0.dist-info/LICENSE` & `aplr-6.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-6.0.0.dist-info/METADATA` & `aplr-6.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 6.0.0
+Version: 6.1.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

