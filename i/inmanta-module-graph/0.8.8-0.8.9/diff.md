# Comparing `tmp/inmanta_module_graph-0.8.8-py3-none-any.whl.zip` & `tmp/inmanta_module_graph-0.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8119 bytes, number of entries: 7
--rw-rw-r--  2.0 unx    23534 b- defN 22-Aug-05 09:42 inmanta_plugins/graph/__init__.py
--rw-rw-r--  2.0 unx      667 b- defN 22-Aug-05 09:42 inmanta_plugins/graph/setup.cfg
--rw-rw-r--  2.0 unx      955 b- defN 22-Aug-05 09:42 inmanta_plugins/graph/model/_init.cf
--rw-rw-r--  2.0 unx      118 b- defN 22-Aug-05 09:42 inmanta_module_graph-0.8.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-05 09:42 inmanta_module_graph-0.8.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 22-Aug-05 09:42 inmanta_module_graph-0.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      619 b- defN 22-Aug-05 09:42 inmanta_module_graph-0.8.8.dist-info/RECORD
-7 files, 26001 bytes uncompressed, 7005 bytes compressed:  73.1%
+Zip file size: 8120 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx    23534 b- defN 22-Sep-28 08:45 inmanta_plugins/graph/__init__.py
+-rw-rw-r--  2.0 unx      667 b- defN 22-Sep-28 08:46 inmanta_plugins/graph/setup.cfg
+-rw-rw-r--  2.0 unx      955 b- defN 22-Sep-28 08:45 inmanta_plugins/graph/model/_init.cf
+-rw-rw-r--  2.0 unx      118 b- defN 22-Sep-28 08:46 inmanta_module_graph-0.8.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Sep-28 08:46 inmanta_module_graph-0.8.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-Sep-28 08:46 inmanta_module_graph-0.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      619 b- defN 22-Sep-28 08:46 inmanta_module_graph-0.8.9.dist-info/RECORD
+7 files, 26001 bytes uncompressed, 7006 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: inmanta_plugins/graph/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/graph/model/_init.cf
 Comment: 
 
-Filename: inmanta_module_graph-0.8.8.dist-info/METADATA
+Filename: inmanta_module_graph-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_graph-0.8.8.dist-info/WHEEL
+Filename: inmanta_module_graph-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_graph-0.8.8.dist-info/top_level.txt
+Filename: inmanta_module_graph-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_graph-0.8.8.dist-info/RECORD
+Filename: inmanta_module_graph-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/graph/setup.cfg

```diff
@@ -15,15 +15,15 @@
 line_length = 128
 known_first_party = inmanta
 
 [metadata]
 name = inmanta-module-graph
 freeze_recursive = False
 freeze_operator = ~=
-version = 0.8.8
+version = 0.8.9
 license = Apache V2
 
 [options]
 install_requires = inmanta-module-std
 zip_safe = False
 include_package_data = True
 packages = find_namespace:
```

## Comparing `inmanta_module_graph-0.8.8.dist-info/RECORD` & `inmanta_module_graph-0.8.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 inmanta_plugins/graph/__init__.py,sha256=xO6QzIEMcpqgvG5VxCzJxqFYqDG_iR8ndO7R2CSnzjU,23534
-inmanta_plugins/graph/setup.cfg,sha256=LhAUsabIze8lf1FHWeexC668xaDZEHMzj08ZsrTASNU,667
+inmanta_plugins/graph/setup.cfg,sha256=ZxBRjinqhaGuYpr3N2uiQNiJFapsSZp445ZgZ8AeMeo,667
 inmanta_plugins/graph/model/_init.cf,sha256=9_Qk2eZF6V5u8kzCz7lJxKIzPN-wxMW6BCelEksLefU,955
-inmanta_module_graph-0.8.8.dist-info/METADATA,sha256=9LaLk307Ps-tC3mLnBNy5TtK1g0eW1j8UzqFLv7aC7A,118
-inmanta_module_graph-0.8.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inmanta_module_graph-0.8.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_graph-0.8.8.dist-info/RECORD,,
+inmanta_module_graph-0.8.9.dist-info/METADATA,sha256=Bmg-W9vhRYUiarmvqe4MvwOiIagmtvNUM70hmMrVeVw,118
+inmanta_module_graph-0.8.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inmanta_module_graph-0.8.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_graph-0.8.9.dist-info/RECORD,,
```

