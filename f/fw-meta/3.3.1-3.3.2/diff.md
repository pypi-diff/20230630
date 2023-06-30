# Comparing `tmp/fw_meta-3.3.1-py3-none-any.whl.zip` & `tmp/fw_meta-3.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14277 bytes, number of entries: 9
+Zip file size: 14270 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 fw_meta/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 80-Jan-01 00:00 fw_meta/aliases.py
--rw-r--r--  2.0 unx     7728 b- defN 80-Jan-01 00:00 fw_meta/exports.py
+-rw-r--r--  2.0 unx     7720 b- defN 80-Jan-01 00:00 fw_meta/exports.py
 -rw-r--r--  2.0 unx    20553 b- defN 80-Jan-01 00:00 fw_meta/imports.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_meta/py.typed
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.3.1.dist-info/RECORD
-9 files, 41157 bytes uncompressed, 13149 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.3.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.3.2.dist-info/RECORD
+9 files, 41149 bytes uncompressed, 13142 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: fw_meta/imports.py
 Comment: 
 
 Filename: fw_meta/py.typed
 Comment: 
 
-Filename: fw_meta-3.3.1.dist-info/LICENSE
+Filename: fw_meta-3.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: fw_meta-3.3.1.dist-info/METADATA
+Filename: fw_meta-3.3.2.dist-info/METADATA
 Comment: 
 
-Filename: fw_meta-3.3.1.dist-info/WHEEL
+Filename: fw_meta-3.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: fw_meta-3.3.1.dist-info/RECORD
+Filename: fw_meta-3.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_meta/exports.py

```diff
@@ -14,15 +14,15 @@
 class ClassificationFilter(fw_utils.SetFilter):
     """File classification filter."""
 
     def match(self, value) -> bool:
         """Return True if the given value is among the classifications."""
         classification = fw_utils.get_field(value, "file.classification")
         if not classification:
-            return False  # pragma: no cover
+            return super().match([])
         key = self.field.replace("file.classification", "").strip(".").lower()
         if key:
             # filtering on a specific (given) classification key
             values = {k.lower(): v for k, v in classification.items()}.get(key, [])
         else:
             # filtering on any classification value regardless of key
             values = [v for vs in classification.values() for v in vs]
```

## Comparing `fw_meta-3.3.1.dist-info/LICENSE` & `fw_meta-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_meta-3.3.1.dist-info/METADATA` & `fw_meta-3.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-meta
-Version: 3.3.1
+Version: 3.3.2
 Summary: Flywheel metadata extraction.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-meta
 License: MIT
 Keywords: Flywheel,DICOM,metadata,extract
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

