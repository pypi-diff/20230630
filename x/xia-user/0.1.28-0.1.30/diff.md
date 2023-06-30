# Comparing `tmp/xia_user-0.1.28-cp39-none-win_amd64.whl.zip` & `tmp/xia_user-0.1.30-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 441407 bytes, number of entries: 9
--rw-r--r--  2.0 unx      364 b- defN 23-Jun-26 06:11 xia_user/__init__.py
--rw-r--r--  2.0 unx   274944 b- defN 23-Jun-26 06:16 xia_user/messages.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   389120 b- defN 23-Jun-26 06:15 xia_user/role_matrix.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   509952 b- defN 23-Jun-26 06:14 xia_user/user.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 06:16 xia_user-0.1.28.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-26 06:16 xia_user-0.1.28.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 06:16 xia_user-0.1.28.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-26 06:16 xia_user-0.1.28.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      757 b- defN 23-Jun-26 06:16 xia_user-0.1.28.dist-info/RECORD
-9 files, 1176111 bytes uncompressed, 440101 bytes compressed:  62.6%
+Zip file size: 9644 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      363 b- defN 23-Jun-29 21:00 xia_user/__init__.py
+-rw-r--r--  2.0 unx      887 b- defN 23-Jun-29 20:17 xia_user/messages.py
+-rw-r--r--  2.0 unx     9660 b- defN 23-Jun-29 20:17 xia_user/role_matrix.py
+-rw-r--r--  2.0 unx    19323 b- defN 23-Jun-29 20:17 xia_user/user.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:04 xia_user-0.1.30.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-29 21:04 xia_user-0.1.30.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:04 xia_user-0.1.30.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-29 21:04 xia_user-0.1.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      703 b- defN 23-Jun-29 21:04 xia_user-0.1.30.dist-info/RECORD
+9 files, 31910 bytes uncompressed, 8434 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_user/__init__.py
 Comment: 
 
-Filename: xia_user/messages.cp39-win_amd64.pyd
+Filename: xia_user/messages.py
 Comment: 
 
-Filename: xia_user/role_matrix.cp39-win_amd64.pyd
+Filename: xia_user/role_matrix.py
 Comment: 
 
-Filename: xia_user/user.cp39-win_amd64.pyd
+Filename: xia_user/user.py
 Comment: 
 
-Filename: xia_user-0.1.28.dist-info/LICENSE.txt
+Filename: xia_user-0.1.30.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_user-0.1.28.dist-info/METADATA
+Filename: xia_user-0.1.30.dist-info/METADATA
 Comment: 
 
-Filename: xia_user-0.1.28.dist-info/WHEEL
+Filename: xia_user-0.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: xia_user-0.1.28.dist-info/top_level.txt
+Filename: xia_user-0.1.30.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_user-0.1.28.dist-info/RECORD
+Filename: xia_user-0.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_user/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "UserBasicInfo", "AppNameField",
     "User", "UserRoles", "ApiInfo", "ApiKey",
     "RoleMatrix", "RoleContent", "Policy", "Group"
 ]
 
 
-__version__ = "0.1.28"
+__version__ = "0.1.30"
```

## Comparing `xia_user-0.1.28.dist-info/METADATA` & `xia_user-0.1.30.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-user
-Version: 0.1.28
+Version: 0.1.30
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-user/0.1.28/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-user/0.1.30/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

