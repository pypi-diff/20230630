# Comparing `tmp/cheetah_orm-2.0.0b6-py3-none-any.whl.zip` & `tmp/cheetah_orm-2.0.0b7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13798 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      211 b- defN 23-Jun-27 20:58 cheetah_orm/__init__.py
+Zip file size: 13800 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      211 b- defN 23-Jun-30 21:40 cheetah_orm/__init__.py
 -rw-rw-rw-  2.0 fat      849 b- defN 23-Jun-08 21:21 cheetah_orm/constants.py
 -rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-08 20:36 cheetah_orm/error.py
 -rw-rw-rw-  2.0 fat     7695 b- defN 23-Jun-25 04:32 cheetah_orm/fields.py
 -rw-rw-rw-  2.0 fat     2526 b- defN 23-Jun-25 17:24 cheetah_orm/indexes.py
--rw-rw-rw-  2.0 fat    28717 b- defN 23-Jun-27 20:57 cheetah_orm/mappers.py
+-rw-rw-rw-  2.0 fat    28701 b- defN 23-Jun-30 21:39 cheetah_orm/mappers.py
 -rw-rw-rw-  2.0 fat    14130 b- defN 23-Jun-26 21:08 cheetah_orm/migrators.py
 -rw-rw-rw-  2.0 fat     1898 b- defN 23-Jun-20 03:51 cheetah_orm/model.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-27 20:59 cheetah_orm-2.0.0b6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6765 b- defN 23-Jun-27 20:59 cheetah_orm-2.0.0b6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 20:59 cheetah_orm-2.0.0b6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-27 20:59 cheetah_orm-2.0.0b6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-27 20:59 cheetah_orm-2.0.0b6.dist-info/RECORD
-13 files, 65517 bytes uncompressed, 12058 bytes compressed:  81.6%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-30 21:41 cheetah_orm-2.0.0b7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6765 b- defN 23-Jun-30 21:41 cheetah_orm-2.0.0b7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 21:41 cheetah_orm-2.0.0b7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-30 21:41 cheetah_orm-2.0.0b7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-30 21:41 cheetah_orm-2.0.0b7.dist-info/RECORD
+13 files, 65501 bytes uncompressed, 12060 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: cheetah_orm/migrators.py
 Comment: 
 
 Filename: cheetah_orm/model.py
 Comment: 
 
-Filename: cheetah_orm-2.0.0b6.dist-info/LICENSE
+Filename: cheetah_orm-2.0.0b7.dist-info/LICENSE
 Comment: 
 
-Filename: cheetah_orm-2.0.0b6.dist-info/METADATA
+Filename: cheetah_orm-2.0.0b7.dist-info/METADATA
 Comment: 
 
-Filename: cheetah_orm-2.0.0b6.dist-info/WHEEL
+Filename: cheetah_orm-2.0.0b7.dist-info/WHEEL
 Comment: 
 
-Filename: cheetah_orm-2.0.0b6.dist-info/top_level.txt
+Filename: cheetah_orm-2.0.0b7.dist-info/top_level.txt
 Comment: 
 
-Filename: cheetah_orm-2.0.0b6.dist-info/RECORD
+Filename: cheetah_orm-2.0.0b7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cheetah_orm/__init__.py

```diff
@@ -1,6 +1,6 @@
 """A lightweight and high-performance object-relational mapper for Python."""
 
 __author__    = "Cybermals"
 __copyright__ = "Copyright (c) 2023 by Cybermals"
 __license__   = "MIT"
-__version__   = "2.0.0b6"
+__version__   = "2.0.0b7"
```

## cheetah_orm/mappers.py

```diff
@@ -557,16 +557,16 @@
         """Delete the given model from the database."""
         self._cur.execute(self._cache[model.__class__]["delete"], (model.id,))
 
     def filter(self, model, condition="", *args, **kwargs):
         """Filter data in the database."""
         sql = self._cache[model]["select"]
 
-        # Replace "=?" placeholders with "=%s" placeholders in the condition format string
-        condition = condition.replace("=?", "=%s")
+        # Replace "?" placeholders with "%s" placeholders in the condition format string
+        condition = condition.replace("?", "%s")
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         # Are there columns to order by?
         if "order_by" in kwargs:
@@ -589,16 +589,16 @@
         results = [model(**dict(row)) for row in self._cur.fetchall()]
         return results
     
     def count(self, model, condition="", *args, **kwargs):
         """Count data in the database."""
         sql = self._cache[model]["count"]
 
-        # Replace "=?" placeholders with "=%s" placeholders in the condition format string
-        condition = condition.replace("=?", "=%s")
+        # Replace "?" placeholders with "%s" placeholders in the condition format string
+        condition = condition.replace("?", "%s")
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         sql += ";"
 
@@ -825,17 +825,17 @@
         """Delete the given model from the database."""
         self._cur.execute(self._cache[model.__class__]["delete"], (model.id,))
 
     def filter(self, model, condition="", *args, **kwargs):
         """Filter data in the database."""
         sql = self._cache[model]["select"]
 
-        # Replace "=?" placeholders with "=%s" placeholders and replace backticks with double quotes in the 
+        # Replace "?" placeholders with "%s" placeholders and replace backticks with double quotes in the 
         # condition format string
-        condition = condition.replace("=?", "=%s").replace("`", '"')
+        condition = condition.replace("?", "%s").replace("`", '"')
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         # Are there columns to order by?
         if "order_by" in kwargs:
@@ -858,17 +858,17 @@
         results = [model(**dict(row)) for row in self._cur.fetchall()]
         return results
     
     def count(self, model, condition="", *args, **kwargs):
         """Count data in the database."""
         sql = self._cache[model]["count"]
 
-        # Replace "=?" placeholders with "=%s" placeholders and replace backticks with double quotes in the 
+        # Replace "?" placeholders with "%s" placeholders and replace backticks with double quotes in the 
         # condition format string
-        condition = condition.replace("=?", "=%s").replace("`", '"')
+        condition = condition.replace("?", "%s").replace("`", '"')
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         sql += ";"
```

## Comparing `cheetah_orm-2.0.0b6.dist-info/LICENSE` & `cheetah_orm-2.0.0b7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cheetah_orm-2.0.0b6.dist-info/METADATA` & `cheetah_orm-2.0.0b7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheetah-orm
-Version: 2.0.0b6
+Version: 2.0.0b7
 Summary: A lightweight and high-performance object-relational mapper for Python.
 Author-email: Cybermals <cybermals@googlegroups.com>
 License: MIT
 Keywords: object-relational mapper
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `cheetah_orm-2.0.0b6.dist-info/RECORD` & `cheetah_orm-2.0.0b7.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-cheetah_orm/__init__.py,sha256=YjaCRVq0VB4F04DDMJmAl7LNrpwFpyeIrf8inNCVoXM,211
+cheetah_orm/__init__.py,sha256=-UkQPYaLGX4liBPNWd_wYQhbmL7WXfeLNGYLcQEfqVw,211
 cheetah_orm/constants.py,sha256=fojdJdDRVwQolDdDm6j1aJFGdjkxSK3mmgwLGT9Ra9U,849
 cheetah_orm/error.py,sha256=Pe7nQ8lq07n5hpoqJru5bCOl6I-6CZ8PiXIovZFcOKQ,483
 cheetah_orm/fields.py,sha256=zSxcTobqlfmjqVj6aCCVLizRRwxGbSqyHYR72i-CdlQ,7695
 cheetah_orm/indexes.py,sha256=tqpXYIq07wtYXS2jhKbLT8VCCdNxTchGkluGuJ64Im4,2526
-cheetah_orm/mappers.py,sha256=AKXDzUpx0hl6xBOemiPJoomNdGqXxwjWJqr7h7Ep5no,28717
+cheetah_orm/mappers.py,sha256=ufPMs928qO9o-Lolv2bxJjBWE1-I49Ew1J0wyNT-HPg,28701
 cheetah_orm/migrators.py,sha256=76pEegCBNU21mX8RtCmVxinEh8VtB2JOkKdWaJm2Mb8,14130
 cheetah_orm/model.py,sha256=5lTnPXhpbkTfeOUJLl95NqIUpEpTnzOJr9o5S6t0faE,1898
-cheetah_orm-2.0.0b6.dist-info/LICENSE,sha256=8jBr0dsKeC3z7oRXG4rt7swwMNm1sQVL_67_T71Fq0k,1092
-cheetah_orm-2.0.0b6.dist-info/METADATA,sha256=d1_QvqOQusDMmZGvwtI7Pm0HluFtEyjAtoWOoBWlv4s,6765
-cheetah_orm-2.0.0b6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cheetah_orm-2.0.0b6.dist-info/top_level.txt,sha256=V3lo5iuVk8dwLfgSrIXFlsSogMqqSyfODL5rHI8fxpM,12
-cheetah_orm-2.0.0b6.dist-info/RECORD,,
+cheetah_orm-2.0.0b7.dist-info/LICENSE,sha256=8jBr0dsKeC3z7oRXG4rt7swwMNm1sQVL_67_T71Fq0k,1092
+cheetah_orm-2.0.0b7.dist-info/METADATA,sha256=ylOSC-y8R2foqHHDTipGmXL6DAjv9XUiqOX9f5-nVz8,6765
+cheetah_orm-2.0.0b7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cheetah_orm-2.0.0b7.dist-info/top_level.txt,sha256=V3lo5iuVk8dwLfgSrIXFlsSogMqqSyfODL5rHI8fxpM,12
+cheetah_orm-2.0.0b7.dist-info/RECORD,,
```

