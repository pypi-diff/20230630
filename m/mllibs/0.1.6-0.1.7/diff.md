# Comparing `tmp/mllibs-0.1.6-py3-none-any.whl.zip` & `tmp/mllibs-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 160598 bytes, number of entries: 36
+Zip file size: 160595 bytes, number of entries: 36
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-23 14:43 mllibs/__init__.py
 -rw-rw-rw-  2.0 fat     5640 b- defN 23-Jun-29 16:54 mllibs/common_corpus.py
 -rw-rw-rw-  2.0 fat    15722 b- defN 23-Jun-28 18:43 mllibs/common_eval.py
 -rw-rw-rw-  2.0 fat     4821 b- defN 23-Jun-28 18:53 mllibs/interface.py
 -rw-rw-rw-  2.0 fat    10770 b- defN 23-Jun-27 14:31 mllibs/mdsplit.py
 -rw-rw-rw-  2.0 fat     9912 b- defN 23-Jun-24 06:11 mllibs/meda_scplot.py
 -rw-rw-rw-  2.0 fat    22347 b- defN 23-Jun-25 14:45 mllibs/meda_splot.py
@@ -14,25 +14,25 @@
 -rw-rw-rw-  2.0 fat     6940 b- defN 23-Jun-25 10:54 mllibs/mseda.py
 -rw-rw-rw-  2.0 fat    10512 b- defN 23-Jun-28 19:16 mllibs/mslcatboost.py
 -rw-rw-rw-  2.0 fat    28139 b- defN 23-Jun-28 12:54 mllibs/mslensemble.py
 -rw-rw-rw-  2.0 fat    19284 b- defN 23-Jun-28 11:05 mllibs/msllinear.py
 -rw-rw-rw-  2.0 fat    11831 b- defN 23-Jun-28 20:25 mllibs/msltree.py
 -rw-rw-rw-  2.0 fat    16763 b- defN 23-Jun-23 14:44 mllibs/mtextnorm.py
 -rw-rw-rw-  2.0 fat    19605 b- defN 23-Jun-24 17:56 mllibs/musldimred.py
--rw-rw-rw-  2.0 fat    39112 b- defN 23-Jun-30 17:24 mllibs/nlpi.py
+-rw-rw-rw-  2.0 fat    39117 b- defN 23-Jun-30 17:55 mllibs/nlpi.py
 -rw-rw-rw-  2.0 fat    17737 b- defN 23-Jun-30 15:22 mllibs/nlpm.py
 -rw-rw-rw-  2.0 fat    75880 b- defN 23-Jun-23 08:27 mllibs/corpus/wordlist.10000.txt
 -rw-rw-rw-  2.0 fat   126077 b- defN 23-Jun-24 17:03 mllibs/models/cv_ner_tagger.pickle
 -rw-rw-rw-  2.0 fat     2745 b- defN 23-Jun-24 17:03 mllibs/models/dtc_ner_tagger.pickle
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-23 08:27 mlmodels/__init__.py
 -rw-rw-rw-  2.0 fat     2994 b- defN 23-Jun-23 08:27 mlmodels/bl_regressor.py
 -rw-rw-rw-  2.0 fat     4402 b- defN 23-Jun-23 08:27 mlmodels/gmm.py
 -rw-rw-rw-  2.0 fat     5761 b- defN 23-Jun-23 08:27 mlmodels/gp_bclassifier.py
 -rw-rw-rw-  2.0 fat     4627 b- defN 23-Jun-23 08:27 mlmodels/gp_regressor.py
 -rw-rw-rw-  2.0 fat     6350 b- defN 23-Jun-23 08:27 mlmodels/gpr_bclassifier.py
 -rw-rw-rw-  2.0 fat     5170 b- defN 23-Jun-23 08:27 mlmodels/kriging_regressor.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-30 17:33 mllibs-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8968 b- defN 23-Jun-30 17:33 mllibs-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 17:33 mllibs-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-30 17:33 mllibs-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2814 b- defN 23-Jun-30 17:33 mllibs-0.1.6.dist-info/RECORD
-36 files, 557861 bytes uncompressed, 156222 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-30 17:56 mllibs-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     8968 b- defN 23-Jun-30 17:56 mllibs-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 17:56 mllibs-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-30 17:56 mllibs-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2814 b- defN 23-Jun-30 17:56 mllibs-0.1.7.dist-info/RECORD
+36 files, 557866 bytes uncompressed, 156219 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: mlmodels/gpr_bclassifier.py
 Comment: 
 
 Filename: mlmodels/kriging_regressor.py
 Comment: 
 
-Filename: mllibs-0.1.6.dist-info/LICENSE
+Filename: mllibs-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: mllibs-0.1.6.dist-info/METADATA
+Filename: mllibs-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: mllibs-0.1.6.dist-info/WHEEL
+Filename: mllibs-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: mllibs-0.1.6.dist-info/top_level.txt
+Filename: mllibs-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mllibs-0.1.6.dist-info/RECORD
+Filename: mllibs-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mllibs/nlpi.py

```diff
@@ -95,15 +95,15 @@
 
     # Load Dataset from Seaborn Repository
     
     def load_dataset(self,name:str,info:str=None):
         
         # load data from seaborn repository             
         data = load_dataset(name)
-        self.store(data,name,info)
+        self.store_data(data,name,info)
 
     # Store Data Function
         
     def store_data(self,data,name:str,info:str=None):
         
 		# dictionary to store data information
         datainfo = {'data':None,'subset':None,'splits':None,
```

## Comparing `mllibs-0.1.6.dist-info/LICENSE` & `mllibs-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mllibs-0.1.6.dist-info/METADATA` & `mllibs-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllibs
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simplifying Machine Learning
 Home-page: https://github.com/shtrausslearning/mllibs
 Author: Andrey Shtrauss
 Author-email: shtraussart@gmail.com
 Project-URL: Bug Tracker, https://github.com/shtrausslearning/mllibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `mllibs-0.1.6.dist-info/RECORD` & `mllibs-0.1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 mllibs/mseda.py,sha256=Qv4G1iBdmjUtqiYsYwRZq3uLAEmyxMDd3FMYLpK2WAc,6940
 mllibs/mslcatboost.py,sha256=yyFFwdywxrh9_DAZE1k9S8lMMft5urQ_6gtVHU69VB4,10512
 mllibs/mslensemble.py,sha256=w6ZuXH1ycx_GR7qAIL1ipDxYgtHR5xByk3oPAt4b3c0,28139
 mllibs/msllinear.py,sha256=IP_CVg0Fthss_WOgwsvzBK0iaD-Kj_TT3cu0NXs9NTU,19284
 mllibs/msltree.py,sha256=85osfqJJt2SNVN17xqWVLfgAnoUYq9VD9PlHU3GTY_Q,11831
 mllibs/mtextnorm.py,sha256=UzULYUE0sC05YgYvLxdcbTglKFiQS_7R-5_KItGiiDk,16763
 mllibs/musldimred.py,sha256=zm1yfU4LClEiCZE7gku-Vd-MyeND10HWsbstm7VyBVc,19605
-mllibs/nlpi.py,sha256=s-0b6-PXOIXHwdxcw8yZklrPUdKhccTbZ1538bkw04k,39112
+mllibs/nlpi.py,sha256=-eLhHl3X5vB67nEEsbRG_z5Nt3pGIuCN_YxvgE65EpA,39117
 mllibs/nlpm.py,sha256=qjLwCy6NEbwSNGN9aRYnlfBtzMMxWQry22kWzn6_U4M,17737
 mllibs/corpus/wordlist.10000.txt,sha256=r2Zt6NAnUYF3WgVpXwWfcb49f0YwOzMIcnHNChSaYbw,75880
 mllibs/models/cv_ner_tagger.pickle,sha256=AyQjmX6WjO1Ubw5K55KDaxQ7vnAS6oQ3v15l_QHlTxs,126077
 mllibs/models/dtc_ner_tagger.pickle,sha256=1QXY45gqUaoOzU4zYik6DQoD-DB2hwsOliESF8iVE-Q,2745
 mlmodels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlmodels/bl_regressor.py,sha256=XxpL3yeQPe_46SnkoRxpTt_4AM6q4PWAT8GD9dorVY0,2994
 mlmodels/gmm.py,sha256=y_HtXZvFJJ3gPbCHn_AAM7SMsF-6hPJpW9NVjIY38_s,4402
 mlmodels/gp_bclassifier.py,sha256=rDgCJhSchYx45iE-e7WuWdzax4bIoJgGQW_ZFKb8_kQ,5761
 mlmodels/gp_regressor.py,sha256=l43eI4a_4URUr6iz1ZHWi4U5NEWb5kvWewS_Sag0nAM,4627
 mlmodels/gpr_bclassifier.py,sha256=1c3Fr5f98F1MfLIiuAzB3Owdhn92dRqtZGNMECId_IY,6350
 mlmodels/kriging_regressor.py,sha256=sEyYE4U53N6iT7W38RH6Cj-QCQ-sEEkQHo2udqZzhtk,5170
-mllibs-0.1.6.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-mllibs-0.1.6.dist-info/METADATA,sha256=GvmDKH3fDDFEhW2EWJc3xOhYVEzjnXnnUijvkUgOpM4,8968
-mllibs-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mllibs-0.1.6.dist-info/top_level.txt,sha256=pOn_KI6Jw7pep1KTFkqiQHucEYgV3Mxor9LucXj_LY4,16
-mllibs-0.1.6.dist-info/RECORD,,
+mllibs-0.1.7.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+mllibs-0.1.7.dist-info/METADATA,sha256=vguQ7ZAsN60bzoSpBY3fDjVRgmXXKTPR1odjRUAYh-s,8968
+mllibs-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mllibs-0.1.7.dist-info/top_level.txt,sha256=pOn_KI6Jw7pep1KTFkqiQHucEYgV3Mxor9LucXj_LY4,16
+mllibs-0.1.7.dist-info/RECORD,,
```

