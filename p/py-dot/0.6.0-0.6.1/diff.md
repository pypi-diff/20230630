# Comparing `tmp/py_dot-0.6.0.tar.gz` & `tmp/py_dot-0.6.1.tar.gz`

## Comparing `py_dot-0.6.0.tar` & `py_dot-0.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 py_dot-0.6.0/BUILD.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 py_dot-0.6.0/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/__init__.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/dicts.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/jsons.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/lists.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/objects.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/operator.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/paths.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/strings.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/syntax.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/timer.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/date/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/date/modify.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/regex/__init__.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/route/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/route/route.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_core.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_dicts.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_lists.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_route.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_strings.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/__init__.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/frame.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/summary_time_unit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/tests/test_data.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/tests/test_frame.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/prompt/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/prompt/tests/prompt_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/__init__.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/arrange.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/sqlalchemies/__init__.py
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_query_string.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_string.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/tests/__init__.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/tests/test_arrange.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 py_dot-0.6.0/.gitignore
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 py_dot-0.6.0/README.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 py_dot-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 py_dot-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 py_dot-0.6.1/BUILD.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 py_dot-0.6.1/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/__init__.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/dicts.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/jsons.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/lists.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/objects.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/operator.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/paths.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/strings.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/syntax.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/timer.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/date/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/date/modify.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/regex/__init__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/route/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/route/route.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/tests/__init__.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/tests/test_core.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/tests/test_dicts.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/tests/test_lists.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/tests/test_route.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/core/tests/test_strings.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/data/__init__.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/data/frame.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/data/summary_time_unit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/data/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/data/tests/test_data.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/data/tests/test_frame.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/prompt/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/prompt/tests/prompt_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/__init__.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/arrange.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/sqlalchemies/__init__.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/sqlalchemies/filter_from_query_string.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/sqlalchemies/filter_from_string.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/tests/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 py_dot-0.6.1/py_dot/store/tests/test_arrange.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 py_dot-0.6.1/.gitignore
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 py_dot-0.6.1/README.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 py_dot-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 py_dot-0.6.1/PKG-INFO
```

### Comparing `py_dot-0.6.0/setup.py` & `py_dot-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/__init__.py` & `py_dot-0.6.1/py_dot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/dicts.py` & `py_dot-0.6.1/py_dot/core/dicts.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/jsons.py` & `py_dot-0.6.1/py_dot/core/jsons.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/lists.py` & `py_dot-0.6.1/py_dot/core/lists.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     :param separator     : items join with this character
     :param first_starts  : most-left additional character
     :param last_ends     : most-right additional character
     """
     if first_starts + starts + separator + ends + last_ends == '':
         raise ValueError('Required one argument at least')
 
+    wrapped_string = wrapped_string.strip() if wrapped_string else None
+
     if not wrapped_string:
         return []
 
     if ends == '':
         ends = starts
 
     start_strings = first_starts + starts
```

### Comparing `py_dot-0.6.0/py_dot/core/objects.py` & `py_dot-0.6.1/py_dot/core/objects.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/strings.py` & `py_dot-0.6.1/py_dot/core/strings.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/syntax.py` & `py_dot-0.6.1/py_dot/core/syntax.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/timer.py` & `py_dot-0.6.1/py_dot/core/timer.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/date/__init__.py` & `py_dot-0.6.1/py_dot/core/date/__init__.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/route/__init__.py` & `py_dot-0.6.1/py_dot/core/route/__init__.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/route/route.py` & `py_dot-0.6.1/py_dot/core/route/route.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/tests/test_core.py` & `py_dot-0.6.1/py_dot/core/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/tests/test_dicts.py` & `py_dot-0.6.1/py_dot/core/tests/test_dicts.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/core/tests/test_lists.py` & `py_dot-0.6.1/py_dot/core/tests/test_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,7 +52,15 @@
                 '{a, b, c}',
                 first_starts='{',
                 separator=', ',
                 last_ends='}'
             ),
             ['a', 'b', 'c']
         )
+
+        self.assertListEqual(
+            from_wrap_string(
+                ' ',
+                '|'
+            ),
+            []
+        )
```

### Comparing `py_dot-0.6.0/py_dot/core/tests/test_route.py` & `py_dot-0.6.1/py_dot/core/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/data/__init__.py` & `py_dot-0.6.1/py_dot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/data/frame.py` & `py_dot-0.6.1/py_dot/data/frame.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/data/tests/test_data.py` & `py_dot-0.6.1/py_dot/data/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/data/tests/test_frame.py` & `py_dot-0.6.1/py_dot/data/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/prompt/__init__.py` & `py_dot-0.6.1/py_dot/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/prompt/tests/prompt_test.py` & `py_dot-0.6.1/py_dot/prompt/tests/prompt_test.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/store/arrange.py` & `py_dot-0.6.1/py_dot/store/arrange.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/store/sqlalchemies/__init__.py` & `py_dot-0.6.1/py_dot/store/sqlalchemies/__init__.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_query_string.py` & `py_dot-0.6.1/py_dot/store/sqlalchemies/filter_from_query_string.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_string.py` & `py_dot-0.6.1/py_dot/store/sqlalchemies/filter_from_string.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/py_dot/store/tests/test_arrange.py` & `py_dot-0.6.1/py_dot/store/tests/test_arrange.py`

 * *Files identical despite different names*

### Comparing `py_dot-0.6.0/pyproject.toml` & `py_dot-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_dot"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="protyliss", email="protyliss@gmail.com" },
 ]
 description = "Python Development Utility Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

