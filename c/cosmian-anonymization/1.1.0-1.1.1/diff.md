# Comparing `tmp/cosmian_anonymization-1.1.0-py3-none-any.whl.zip` & `tmp/cosmian_anonymization-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20328 bytes, number of entries: 11
+Zip file size: 20345 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      169 b- defN 80-Jan-01 00:00 cosmian_anonymization/__init__.py
--rw-r--r--  2.0 unx     8012 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
+-rw-r--r--  2.0 unx     8030 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
 -rw-r--r--  2.0 unx     1954 b- defN 80-Jan-01 00:00 cosmian_anonymization/conversion_helper.py
 -rw-r--r--  2.0 unx     3628 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
 -rw-r--r--  2.0 unx     3784 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
 -rw-r--r--  2.0 unx     3887 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
--rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/RECORD
-11 files, 56400 bytes uncompressed, 18548 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/RECORD
+11 files, 56418 bytes uncompressed, 18565 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: cosmian_anonymization/noise_correlation.py
 Comment: 
 
 Filename: cosmian_anonymization/noise_parser.py
 Comment: 
 
-Filename: cosmian_anonymization-1.1.0.dist-info/LICENSE.md
+Filename: cosmian_anonymization-1.1.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: cosmian_anonymization-1.1.0.dist-info/METADATA
+Filename: cosmian_anonymization-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_anonymization-1.1.0.dist-info/WHEEL
+Filename: cosmian_anonymization-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: cosmian_anonymization-1.1.0.dist-info/entry_points.txt
+Filename: cosmian_anonymization-1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: cosmian_anonymization-1.1.0.dist-info/RECORD
+Filename: cosmian_anonymization-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cosmian_anonymization/anonymize.py

```diff
@@ -143,16 +143,16 @@
 
     # Iterate over each column to anonymize.
     for column_metadata in config["metadata"]:
         col_name: str = column_metadata["name"]
         # Anonymize the column
         output_df[col_name] = apply_anonymization_column(
             output_df[col_name],
-            column_metadata["method"],
-            column_metadata["method_options"],
+            column_metadata.get("method", None),
+            column_metadata.get("method_options", {}),
         )
 
     # -- Noise correlation --
     # Read through the config to find all correlation tasks
     noise_corr_tasks = parse_noise_correlation_config(config)
     # Apply correlation on each groups
     for task in noise_corr_tasks.values():
```

## Comparing `cosmian_anonymization-1.1.0.dist-info/LICENSE.md` & `cosmian_anonymization-1.1.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cosmian_anonymization-1.1.0.dist-info/METADATA` & `cosmian_anonymization-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-anonymization
-Version: 1.1.0
+Version: 1.1.1
 Summary: Cosmian Anonymization library in Python
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `cosmian_anonymization-1.1.0.dist-info/RECORD` & `cosmian_anonymization-1.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cosmian_anonymization/__init__.py,sha256=G62TkbdQTsCYntoi-21PwY8tBtEYGea6OoW9EeGLR70,169
-cosmian_anonymization/anonymize.py,sha256=Gu3tULLKkrHgzJ_GH97U9VEMoX_XKXuIzkQQUkN84DU,8012
+cosmian_anonymization/anonymize.py,sha256=w03T1Tt_SJn8_mExdluOzhClPCvul44EGpcLjuImMqg,8030
 cosmian_anonymization/conversion_helper.py,sha256=WiT2AVz9_eR0KdR1hHx79U8wS_rDPy9_8hXolvWB-gg,1954
 cosmian_anonymization/method_parser.py,sha256=JoDKER4MZVYbOcRzsNcXZTe7DADZzWA9H4oHaBeJXbA,3628
 cosmian_anonymization/noise_correlation.py,sha256=GCmDJKpmB3p1DxeaQA_y6BcVLuB_tXxtCfBVJauwQmE,3784
 cosmian_anonymization/noise_parser.py,sha256=l6G9qjwPXNf43Rb9PvawFriF1AcDzSz0_nBNAqBz1Q4,3887
-cosmian_anonymization-1.1.0.dist-info/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
-cosmian_anonymization-1.1.0.dist-info/METADATA,sha256=qlWPgBQJFfCfzp4zjVOYcag1a-YjdnfX8WSOeqjzCIw,1500
-cosmian_anonymization-1.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-cosmian_anonymization-1.1.0.dist-info/entry_points.txt,sha256=8zwjT9vbjKsVxtbgIOOw9YY0zzI7PE9y06fEsILeAyA,73
-cosmian_anonymization-1.1.0.dist-info/RECORD,,
+cosmian_anonymization-1.1.1.dist-info/LICENSE.md,sha256=_zfsPgqYDWuqWECzE0w-LQfkkgg28_DMNj87xgn6OUI,32275
+cosmian_anonymization-1.1.1.dist-info/METADATA,sha256=DQIu1CbSP6mTVOc6UBipUvDDv01wsIXm8ZeqyLlQbA0,1500
+cosmian_anonymization-1.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+cosmian_anonymization-1.1.1.dist-info/entry_points.txt,sha256=8zwjT9vbjKsVxtbgIOOw9YY0zzI7PE9y06fEsILeAyA,73
+cosmian_anonymization-1.1.1.dist-info/RECORD,,
```

