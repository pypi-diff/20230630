# Comparing `tmp/pytket_qir-0.2.0rc8-py3-none-any.whl.zip` & `tmp/pytket_qir-0.2.0rc9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 18119 bytes, number of entries: 12
--rw-r--r--  2.0 unx      858 b- defN 23-May-26 14:26 pytket/qir/__init__.py
--rw-r--r--  2.0 unx       69 b- defN 23-May-26 14:27 pytket/qir/_metadata.py
--rw-r--r--  2.0 unx      711 b- defN 23-May-26 14:26 pytket/qir/conversion/__init__.py
--rw-r--r--  2.0 unx     3352 b- defN 23-May-26 14:26 pytket/qir/conversion/api.py
--rw-r--r--  2.0 unx    30282 b- defN 23-May-26 14:26 pytket/qir/conversion/conversion.py
--rw-r--r--  2.0 unx     4082 b- defN 23-May-26 14:26 pytket/qir/conversion/gatesets.py
--rw-r--r--  2.0 unx     1481 b- defN 23-May-26 14:26 pytket/qir/conversion/module.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4183 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1017 b- defN 23-May-26 14:27 pytket_qir-0.2.0rc8.dist-info/RECORD
-12 files, 57491 bytes uncompressed, 16397 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx      858 b- defN 23-May-26 14:57 pytket/qir/__init__.py
+-rw-r--r--  2.0 unx       69 b- defN 23-May-26 14:58 pytket/qir/_metadata.py
+-rw-r--r--  2.0 unx      711 b- defN 23-May-26 14:57 pytket/qir/conversion/__init__.py
+-rw-r--r--  2.0 unx     3357 b- defN 23-May-26 14:57 pytket/qir/conversion/api.py
+-rw-r--r--  2.0 unx    30282 b- defN 23-May-26 14:57 pytket/qir/conversion/conversion.py
+-rw-r--r--  2.0 unx     4082 b- defN 23-May-26 14:57 pytket/qir/conversion/gatesets.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-May-26 14:57 pytket/qir/conversion/module.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-26 14:58 pytket_qir-0.2.0rc9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4183 b- defN 23-May-26 14:58 pytket_qir-0.2.0rc9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:58 pytket_qir-0.2.0rc9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-26 14:58 pytket_qir-0.2.0rc9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1017 b- defN 23-May-26 14:58 pytket_qir-0.2.0rc9.dist-info/RECORD
+12 files, 57496 bytes uncompressed, 16397 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pytket/qir/conversion/gatesets.py
 Comment: 
 
 Filename: pytket/qir/conversion/module.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc8.dist-info/LICENSE
+Filename: pytket_qir-0.2.0rc9.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qir-0.2.0rc8.dist-info/METADATA
+Filename: pytket_qir-0.2.0rc9.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qir-0.2.0rc8.dist-info/WHEEL
+Filename: pytket_qir-0.2.0rc9.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_qir-0.2.0rc8.dist-info/top_level.txt
+Filename: pytket_qir-0.2.0rc9.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_qir-0.2.0rc8.dist-info/RECORD
+Filename: pytket_qir-0.2.0rc9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/qir/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.2.0rc8"
+__extension_version__ = "0.2.0rc9"
 __extension_name__ = "pytket-qir"
```

## pytket/qir/conversion/api.py

```diff
@@ -39,22 +39,23 @@
 def pytket_to_qir(
     circ: Circuit,
     name: str = "Generated from input pytket circuit",
     qir_format: QIRFormat = QIRFormat.BINARY,
     pyqir_0_7_compatibility: bool = False,
 ) -> Union[str, bytes, None]:
     """converts given pytket circuit to qir
+
     :param circ: given circuit
     :type circ: pytket circuit
     :param name: name for the qir module created
     :type name: str
     :param qir_format: format of the generated qir, default value is binary
     :type qir_format: QIRFormat
     :param pyqir_0_7_compatibility: converts the output to be compatible with
-    pyqir 0.7, default value false
+        pyqir 0.7, default value false
     :type pyqir_0_7_compatibility: bool
     """
 
     if len(circ.q_registers) > 1 or circ.q_registers[0].name != "q":
         raise ValueError(
             """The circuit that should be converted should only have the default
             quantum register. You can convert it using the pytket
```

## Comparing `pytket_qir-0.2.0rc8.dist-info/LICENSE` & `pytket_qir-0.2.0rc9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_qir-0.2.0rc8.dist-info/METADATA` & `pytket_qir-0.2.0rc9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qir
-Version: 0.2.0rc8
+Version: 0.2.0rc9
 Summary: Extension for pytket, providing functions for conversion into to qir
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-qir/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-qir
 Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
```

## Comparing `pytket_qir-0.2.0rc8.dist-info/RECORD` & `pytket_qir-0.2.0rc9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pytket/qir/__init__.py,sha256=3AXz2dN6Yg20zM3YYtMAPf6ZCidAG-opHomVhmU93w4,858
-pytket/qir/_metadata.py,sha256=_eC4ecZVUur4-IjCTiB0CUgH_SvFq5CM9ICJsUbdxDg,69
+pytket/qir/_metadata.py,sha256=NhIYfPH5zUyHiQkIowEHy1GGzKGCwvtgkzBvsKXtZ9A,69
 pytket/qir/conversion/__init__.py,sha256=kKuV2wCn6cMf_iVQhlsu28cH8K4dDCUqwUXlHF_FpUg,711
-pytket/qir/conversion/api.py,sha256=FznzHIsaAJCAbhQxc3iudc173sWYI9bz1i8dJJtl9L0,3352
+pytket/qir/conversion/api.py,sha256=kYD42oBguCbNSt_4auBV8YTzH9RoM_UY0bSGGwMwQ5s,3357
 pytket/qir/conversion/conversion.py,sha256=c8xtnC7zNntqiiPuEE1EjO9ApxS7IaXnesjJVL6YL60,30282
 pytket/qir/conversion/gatesets.py,sha256=Ix1KkLlFoyE1LkoUs0J7wFikZXT9w5jYs8mnTQnZURM,4082
 pytket/qir/conversion/module.py,sha256=fj8iHNh27_-wbjKkO9JdnKkExiRAhMWXTzjVP9kCwtA,1481
-pytket_qir-0.2.0rc8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytket_qir-0.2.0rc8.dist-info/METADATA,sha256=3nyE2s3mXKqknbnOLBUL0Uj9EtZw_SwZDrefD0iKJr4,4183
-pytket_qir-0.2.0rc8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytket_qir-0.2.0rc8.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_qir-0.2.0rc8.dist-info/RECORD,,
+pytket_qir-0.2.0rc9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_qir-0.2.0rc9.dist-info/METADATA,sha256=yislGfeU2FE11Yu-n7sTuGjnw8zGwEbagjn6ZngmcnY,4183
+pytket_qir-0.2.0rc9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytket_qir-0.2.0rc9.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_qir-0.2.0rc9.dist-info/RECORD,,
```

