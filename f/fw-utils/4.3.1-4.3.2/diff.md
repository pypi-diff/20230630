# Comparing `tmp/fw_utils-4.3.1-py3-none-any.whl.zip` & `tmp/fw_utils-4.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22161 bytes, number of entries: 14
+Zip file size: 22166 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1747 b- defN 80-Jan-01 00:00 fw_utils/__init__.py
 -rw-r--r--  2.0 unx     2914 b- defN 80-Jan-01 00:00 fw_utils/datetime.py
 -rw-r--r--  2.0 unx     3095 b- defN 80-Jan-01 00:00 fw_utils/dicts.py
 -rw-r--r--  2.0 unx     5436 b- defN 80-Jan-01 00:00 fw_utils/files.py
--rw-r--r--  2.0 unx     9221 b- defN 80-Jan-01 00:00 fw_utils/filters.py
+-rw-r--r--  2.0 unx     9228 b- defN 80-Jan-01 00:00 fw_utils/filters.py
 -rw-r--r--  2.0 unx    10502 b- defN 80-Jan-01 00:00 fw_utils/formatters.py
 -rw-r--r--  2.0 unx    15077 b- defN 80-Jan-01 00:00 fw_utils/parsers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_utils/py.typed
 -rw-r--r--  2.0 unx     4382 b- defN 80-Jan-01 00:00 fw_utils/state.py
 -rw-r--r--  2.0 unx     3063 b- defN 80-Jan-01 00:00 fw_utils/testing.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.3.1.dist-info/RECORD
-14 files, 59579 bytes uncompressed, 20449 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.3.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.3.2.dist-info/RECORD
+14 files, 59586 bytes uncompressed, 20454 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: fw_utils/state.py
 Comment: 
 
 Filename: fw_utils/testing.py
 Comment: 
 
-Filename: fw_utils-4.3.1.dist-info/LICENSE
+Filename: fw_utils-4.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: fw_utils-4.3.1.dist-info/METADATA
+Filename: fw_utils-4.3.2.dist-info/METADATA
 Comment: 
 
-Filename: fw_utils-4.3.1.dist-info/WHEEL
+Filename: fw_utils-4.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: fw_utils-4.3.1.dist-info/RECORD
+Filename: fw_utils-4.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_utils/filters.py

```diff
@@ -150,30 +150,30 @@
         return OPERATORS[self.op](value, self.num)
 
 
 class SetFilter(ExpressionFilter):
     """Set filter."""
 
     operators = ["=", "!=", "=~", "!~"]  # ie. in / not in
-    pattern: t.Optional[t.Pattern]
+    pattern: t.Union[str, t.Pattern]
 
     def __init__(self, field: str, op: str, value: str) -> None:
         """Initialize set filter from str value."""
         super().__init__(field, op, value.lower())
         try:
-            self.pattern = re.compile(value) if "~" in op else None
+            self.pattern = re.compile(self.value) if "~" in op else self.value
         except re.error as exc:
             raise ValueError(f"Invalid pattern: {value} - {exc}") from exc
 
     def match(self, value: t.Union[list, set, t.Any]) -> bool:
         """Return that the given item is in the given list/set."""
         values = value if isinstance(value, (list, set)) else self.getval(value) or []
         if not values and self.op.startswith("!"):
             return True
-        return any(OPERATORS[self.op](v, self.pattern or self.value) for v in values)
+        return any(OPERATORS[self.op](v.lower(), self.pattern) for v in values)
 
 
 class StringFilter(ExpressionFilter):
     """String filter."""
 
     operators = STRING_OPS
     string: t.Union[str, t.Pattern]
```

## Comparing `fw_utils-4.3.1.dist-info/LICENSE` & `fw_utils-4.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_utils-4.3.1.dist-info/METADATA` & `fw_utils-4.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-utils
-Version: 4.3.1
+Version: 4.3.2
 Summary: Common Flywheel helper utilities.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-utils
 License: MIT
 Keywords: Flywheel,helper,utility
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

