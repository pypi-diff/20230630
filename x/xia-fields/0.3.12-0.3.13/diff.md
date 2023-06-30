# Comparing `tmp/xia_fields-0.3.12-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields-0.3.13-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11493 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1177 b- defN 23-Jun-29 20:50 xia_fields/__init__.py
--rw-r--r--  2.0 unx    13346 b- defN 23-Jun-29 20:50 xia_fields/base.py
--rw-r--r--  2.0 unx    13317 b- defN 23-Jun-29 20:50 xia_fields/fields.py
--rw-r--r--  2.0 unx     9575 b- defN 23-Jun-29 20:50 xia_fields/fields_ext.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3310 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      723 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/RECORD
-9 files, 41709 bytes uncompressed, 10253 bytes compressed:  75.4%
+Zip file size: 10280 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1177 b- defN 23-Jun-30 11:24 xia_fields/__init__.py
+-rw-r--r--  2.0 unx    13346 b- defN 23-Jun-30 10:30 xia_fields/base.py
+-rw-r--r--  2.0 unx    13317 b- defN 23-Jun-30 10:30 xia_fields/fields.py
+-rw-r--r--  2.0 unx     9575 b- defN 23-Jun-30 10:30 xia_fields/fields_ext.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      388 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      722 b- defN 23-Jun-30 11:29 xia_fields-0.3.13.dist-info/RECORD
+9 files, 38786 bytes uncompressed, 9040 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_fields/fields.py
 Comment: 
 
 Filename: xia_fields/fields_ext.py
 Comment: 
 
-Filename: xia_fields-0.3.12.dist-info/LICENSE.txt
+Filename: xia_fields-0.3.13.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields-0.3.12.dist-info/METADATA
+Filename: xia_fields-0.3.13.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields-0.3.12.dist-info/WHEEL
+Filename: xia_fields-0.3.13.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields-0.3.12.dist-info/top_level.txt
+Filename: xia_fields-0.3.13.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields-0.3.12.dist-info/RECORD
+Filename: xia_fields-0.3.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields/__init__.py

```diff
@@ -14,8 +14,8 @@
     "JsonField", "DictField", "CompressedStringField",
     "Int64Field", "Int32Field", "SFixed64Field", "SFixed32Field",
     "UInt64Field", "UInt32Field", "Fixed64Field", "Fixed32Field",
     "DoubleField", "DateField", "TimestampField", "TimeField", "DateTimeField",
     "OsEnvironField"
 ]
 
-__version__ = "0.3.12"
+__version__ = "0.3.13"
```

## Comparing `xia_fields-0.3.12.dist-info/RECORD` & `xia_fields-0.3.13.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_fields/__init__.py,sha256=kM_JP_Nn37UOlGgxfdkCZyH3UHmCCamusv8wwoUFUrQ,1177
+xia_fields/__init__.py,sha256=d7GNVnB-cquXWdyclnSN1-Q6T8Es5i6sKjf0V6Aqn6I,1177
 xia_fields/base.py,sha256=gJD8TMRl6LFdSzVh0p4wHMgK19eU-1hGxXYMm7PbtAQ,13346
 xia_fields/fields.py,sha256=AW2ef1L3kSsNAABArIXV2xdp8KEXjoDR7dVP9Kehvrs,13317
 xia_fields/fields_ext.py,sha256=G5nDz8NrZeSMnmKwK_iY4_tzJieTzQQIGgq1Npa5x_o,9575
-xia_fields-0.3.12.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_fields-0.3.12.dist-info/METADATA,sha256=mJD5vGgAvIlAOyZqsvHLYbFDmt4VueIvYn_jSddwLyc,3310
-xia_fields-0.3.12.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_fields-0.3.12.dist-info/top_level.txt,sha256=pXvwXCVXR-n1PTScNVgqx5GAlG0H2tIpu7XuuswUrng,11
-xia_fields-0.3.12.dist-info/RECORD,,
+xia_fields-0.3.13.dist-info/LICENSE.txt,sha256=mpr6mJwzeixxwdsBolN0mQUjF2BIXPyL8zvZgqTk7PI,151
+xia_fields-0.3.13.dist-info/METADATA,sha256=pkzg-17u7Te093vMiB-RauKazs3L05sripEc_YLqmKA,388
+xia_fields-0.3.13.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_fields-0.3.13.dist-info/top_level.txt,sha256=pXvwXCVXR-n1PTScNVgqx5GAlG0H2tIpu7XuuswUrng,11
+xia_fields-0.3.13.dist-info/RECORD,,
```

