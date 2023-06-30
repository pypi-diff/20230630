# Comparing `tmp/angola-0.14.3.tar.gz` & `tmp/angola-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.14.3.tar", last modified: Wed Jun 28 00:53:32 2023, max compression
+gzip compressed data, was "angola-0.14.4.tar", last modified: Fri Jun 30 07:41:44 2023, max compression
```

## Comparing `angola-0.14.3.tar` & `angola-0.14.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-28 00:53:32.025714 angola-0.14.3/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.3/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.3/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-28 00:53:32.025789 angola-0.14.3/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.3/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-28 00:53:32.026056 angola-0.14.3/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      776 2023-06-28 00:53:19.000000 angola-0.14.3/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-28 00:53:32.018880 angola-0.14.3/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-28 00:53:32.022782 angola-0.14.3/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.3/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    50979 2023-06-23 08:06:55.000000 angola-0.14.3/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.3/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.3/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    18669 2023-06-28 00:51:03.000000 angola-0.14.3/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.3/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-28 00:53:32.024237 angola-0.14.3/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-28 00:53:32.000000 angola-0.14.3/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-28 00:53:32.000000 angola-0.14.3/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-28 00:53:32.000000 angola-0.14.3/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       47 2023-06-28 00:53:32.000000 angola-0.14.3/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-28 00:53:32.000000 angola-0.14.3/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-28 00:53:32.025586 angola-0.14.3/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.3/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.3/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.3/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     4792 2023-06-23 14:59:38.000000 angola-0.14.3/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.3/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.228037 angola-0.14.4/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.14.4/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.14.4/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-30 07:41:44.228109 angola-0.14.4/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.14.4/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-30 07:41:44.228364 angola-0.14.4/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      776 2023-06-30 07:41:36.000000 angola-0.14.4/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.222094 angola-0.14.4/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.225587 angola-0.14.4/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.14.4/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    51001 2023-06-28 16:10:18.000000 angola-0.14.4/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.14.4/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.14.4/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18673 2023-06-30 07:41:24.000000 angola-0.14.4/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20084 2023-06-23 04:30:25.000000 angola-0.14.4/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.226748 angola-0.14.4/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       47 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-30 07:41:44.000000 angola-0.14.4/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-30 07:41:44.227937 angola-0.14.4/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.14.4/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.14.4/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.14.4/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     4810 2023-06-30 07:41:06.000000 angola-0.14.4/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.14.4/tests/test_query.py
```

### Comparing `angola-0.14.3/LICENSE` & `angola-0.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/PKG-INFO` & `angola-0.14.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.3
+Version: 0.14.4
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.3/README.md` & `angola-0.14.4/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/setup.py` & `angola-0.14.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.14.3"
+VERSION = "0.14.4"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.14.3/src/angola/database.py` & `angola-0.14.4/src/angola/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1500,15 +1500,15 @@
         Update by filter
 
         Params:
             filter:dict - filter document criteria
             mutations:dict - changes on the found documents
         """
         _data = self._normalize_data()
-        res = self.find(filters)
+        res = self.find(filters=filters, limit=1000)
         if res:
             for item in res:
                 ts = lib.get_timestamp()
                 _key = item.get("_key")
                 _default = {  # ensuring we do some data can't be overwritten
                     "_key": _key,
                     # "_created_at": ts
@@ -1550,15 +1550,15 @@
         Return:
             dict
         """
         if res := self.find(filters=filters, limit=1):
             return list(res)[0]
         return None 
 
-    def find(self, filters: dict = {}, sort: dict = {}, limit: int = 10,  offset:int=0, page=None) -> dict_query.Cursor:
+    def find(self, filters: dict = {}, sort: dict = {}, limit: int = 1000,  offset:int=0, page=None) -> dict_query.Cursor:
         """
         Perform a query
 
         Params:
             filters:
             sort:
             limit:
```

### Comparing `angola-0.14.3/src/angola/dict_mutator.py` & `angola-0.14.4/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/src/angola/dict_query.py` & `angola-0.14.4/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/src/angola/lib.py` & `angola-0.14.4/src/angola/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     Params:
         name:str
     Returns:
         bool
     """
     if not name or not isinstance(name, str):
         return False
-    pattern = re.compile(r"^[a-zA-Z\_][a-zA-Z0-9\_\-]*$")
+    pattern = re.compile(r"^[a-zA-Z\_\$][a-zA-Z0-9\_\-\$]*$")
     return bool(pattern.match(name)) 
 
 
 
 def gen_xid() -> str:
     """
     XID - To be used as id.
```

### Comparing `angola-0.14.3/src/angola/lib_xql.py` & `angola-0.14.4/src/angola/lib_xql.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/src/angola.egg-info/PKG-INFO` & `angola-0.14.4/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.14.3
+Version: 0.14.4
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.14.3/tests/test_database.py` & `angola-0.14.4/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/tests/test_dict_mutator.py` & `angola-0.14.4/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.14.3/tests/test_lib.py` & `angola-0.14.4/tests/test_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     assert len(c[len(c) - 1]) == 2
 
 
 def test_keyname_valid():
     n = [
         ("a", True), ("ab", True), ("abC", True), ("hello", True), ("World", True), 
         ("WORDL", True), ("WORLD1", True), ("woRld7_", True), ("somethin_g", True), 
-        ("_under", True), ("__double", True),
+        ("_under", True), ("__double", True), ("$_some", True),
         ("", False), ("0", False), ("0Boom", False),("-something", False), ("somet-hing", True),
         (0, False), (None, False), (True, False), (False, False)
     ]
     for k in n: 
         assert lib.keyname_valid(k[0]) is k[1]
 
 def test_dict_inspect_valid_keyname():
```

