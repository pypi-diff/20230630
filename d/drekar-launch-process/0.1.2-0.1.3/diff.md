# Comparing `tmp/drekar_launch_process-0.1.2-py3-none-any.whl.zip` & `tmp/drekar_launch_process-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8345 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     5462 b- defN 23-Jun-13 01:41 drekar_launch_process.py
--rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-13 02:02 drekar_launch_process-0.1.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3208 b- defN 23-Jun-13 02:02 drekar_launch_process-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 02:02 drekar_launch_process-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-13 02:02 drekar_launch_process-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      542 b- defN 23-Jun-13 02:02 drekar_launch_process-0.1.2.dist-info/RECORD
-6 files, 20880 bytes uncompressed, 7353 bytes compressed:  64.8%
+Zip file size: 8405 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     5462 b- defN 23-Jun-13 02:03 drekar_launch_process.py
+-rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-30 07:32 drekar_launch_process-0.1.3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3348 b- defN 23-Jun-30 07:32 drekar_launch_process-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 07:32 drekar_launch_process-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-30 07:32 drekar_launch_process-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      542 b- defN 23-Jun-30 07:32 drekar_launch_process-0.1.3.dist-info/RECORD
+6 files, 21020 bytes uncompressed, 7413 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: drekar_launch_process.py
 Comment: 
 
-Filename: drekar_launch_process-0.1.2.dist-info/LICENSE.txt
+Filename: drekar_launch_process-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: drekar_launch_process-0.1.2.dist-info/METADATA
+Filename: drekar_launch_process-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: drekar_launch_process-0.1.2.dist-info/WHEEL
+Filename: drekar_launch_process-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: drekar_launch_process-0.1.2.dist-info/top_level.txt
+Filename: drekar_launch_process-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: drekar_launch_process-0.1.2.dist-info/RECORD
+Filename: drekar_launch_process-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `drekar_launch_process-0.1.2.dist-info/LICENSE.txt` & `drekar_launch_process-0.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `drekar_launch_process-0.1.2.dist-info/METADATA` & `drekar_launch_process-0.1.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: drekar-launch-process
-Version: 0.1.2
+Version: 0.1.3
 Summary: Client library for drekar-launch
 Author-email: John Wason <wason@wasontech.com>
 License: Apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Provides-Extra: test
+Requires-Dist: pytest ; extra == 'test'
+Requires-Dist: pywin32 ; (platform_system == "Windows") and extra == 'test'
 
 # Drekar Launch Process
 
 This library contains client utility functions for processes launched using `drekar-launch`, although they may also be used without `drekar-launch`. Currently this package provides a reliable way for processes to receive shutdown signals from a process manager or the user using `ctrl-c`.
 
 See `drekar-launch`: https://github.com/johnwason/drekar-launch
```

