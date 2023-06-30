# Comparing `tmp/rozetka_api-1.1.2.tar.gz` & `tmp/rozetka_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rozetka_api-1.1.2.tar", max compression
+gzip compressed data, was "rozetka_api-1.1.3.tar", max compression
```

## Comparing `rozetka_api-1.1.2.tar` & `rozetka_api-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      978 2023-06-30 13:22:27.305656 rozetka_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      135 2022-09-03 20:53:08.178729 rozetka_api-1.1.2/README.rst
--rw-r--r--   0        0        0        0 2022-09-02 18:14:26.482651 rozetka_api-1.1.2/rozetka/entities/__init__.py
--rw-r--r--   0        0        0    10637 2023-06-30 13:04:36.394214 rozetka_api-1.1.2/rozetka/entities/category.py
--rw-r--r--   0        0        0    11959 2023-06-30 13:11:48.616706 rozetka_api-1.1.2/rozetka/entities/item.py
--rw-r--r--   0        0        0      555 2022-09-21 11:51:31.500532 rozetka_api-1.1.2/rozetka/entities/point.py
--rw-r--r--   0        0        0     8709 2023-06-30 13:05:29.369115 rozetka_api-1.1.2/rozetka/entities/supercategory.py
--rw-r--r--   0        0        0      821 2022-09-03 11:44:07.607811 rozetka_api-1.1.2/rozetka/examples/example_category.py
--rw-r--r--   0        0        0      108 2022-09-03 10:56:00.803564 rozetka_api-1.1.2/rozetka/examples/example_item.py
--rw-r--r--   0        0        0     3390 2023-06-30 11:40:23.368017 rozetka_api-1.1.2/rozetka/runners/parse_api.py
--rw-r--r--   0        0        0        0 2022-08-30 10:55:06.318671 rozetka_api-1.1.2/rozetka/tools/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-30 13:21:53.957476 rozetka_api-1.1.2/rozetka/tools/constants.py
--rw-r--r--   0        0        0     4717 2023-06-30 13:13:17.667363 rozetka_api-1.1.2/rozetka/tools/db.py
--rw-r--r--   0        0        0     3949 2023-06-30 13:09:17.549730 rozetka_api-1.1.2/rozetka/tools/tools.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 rozetka_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      978 2023-06-30 15:29:40.460135 rozetka_api-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      135 2022-09-03 20:53:08.178729 rozetka_api-1.1.3/README.rst
+-rw-r--r--   0        0        0        0 2022-09-02 18:14:26.482651 rozetka_api-1.1.3/rozetka/entities/__init__.py
+-rw-r--r--   0        0        0    10637 2023-06-30 13:04:36.394214 rozetka_api-1.1.3/rozetka/entities/category.py
+-rw-r--r--   0        0        0    12027 2023-06-30 14:17:20.527737 rozetka_api-1.1.3/rozetka/entities/item.py
+-rw-r--r--   0        0        0      555 2022-09-21 11:51:31.500532 rozetka_api-1.1.3/rozetka/entities/point.py
+-rw-r--r--   0        0        0     8695 2023-06-30 15:01:21.625968 rozetka_api-1.1.3/rozetka/entities/supercategory.py
+-rw-r--r--   0        0        0      821 2022-09-03 11:44:07.607811 rozetka_api-1.1.3/rozetka/examples/example_category.py
+-rw-r--r--   0        0        0      108 2022-09-03 10:56:00.803564 rozetka_api-1.1.3/rozetka/examples/example_item.py
+-rw-r--r--   0        0        0     3390 2023-06-30 11:40:23.368017 rozetka_api-1.1.3/rozetka/runners/parse_api.py
+-rw-r--r--   0        0        0        0 2022-08-30 10:55:06.318671 rozetka_api-1.1.3/rozetka/tools/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-30 13:21:53.957476 rozetka_api-1.1.3/rozetka/tools/constants.py
+-rw-r--r--   0        0        0     4717 2023-06-30 13:13:17.667363 rozetka_api-1.1.3/rozetka/tools/db.py
+-rw-r--r--   0        0        0     3955 2023-06-30 14:32:19.224443 rozetka_api-1.1.3/rozetka/tools/tools.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 rozetka_api-1.1.3/PKG-INFO
```

### Comparing `rozetka_api-1.1.2/pyproject.toml` & `rozetka_api-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rozetka-api"
-version = "1.1.2"
+version = "1.1.3"
 description = "Rozetka Python API"
 authors = ["Alexey ALERT Rubasheff <alexey.rubasheff@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "rozetka"}]
 keywords = ["rozetka"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `rozetka_api-1.1.2/rozetka/entities/category.py` & `rozetka_api-1.1.3/rozetka/entities/category.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.2/rozetka/entities/item.py` & `rozetka_api-1.1.3/rozetka/entities/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
         LOG.debug(f"Parsing batch of {len(product_ids)} products")
         output = []
         req = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
         if req is None:
             return output
 
-        data: List[dict] = req.json().get('data')
+        try:
+            data: List[dict] = req.json().get('data')
+        except Exception as e:
+            pass
         """
         {
             "id": 280528638,
             "title": "Мобільний телефон Samsung Galaxy A32 4/128 GB Black",
             "title_suffix": "",
             "price": 10399,
             "old_price": 10499,
```

### Comparing `rozetka_api-1.1.2/rozetka/entities/point.py` & `rozetka_api-1.1.3/rozetka/entities/point.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.2/rozetka/entities/supercategory.py` & `rozetka_api-1.1.3/rozetka/entities/supercategory.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,34 +62,38 @@
 
     SuperCategory._fat_menu_categories = output = list(set(output))
     return output
 
 
 def get_all_items_recursively() -> List[Item]:
     categories = list(get_all_categories_recursively())
+    categories.sort(key=lambda _: _.id_)
     LOG.green("Got ALL categories recursively")
 
+    all_categories = [_ for _ in categories for _ in _]
+    all_categories_len = len(all_categories)
+
     LOG.green("Getting ALL items recursively")
     # noinspection PyProtectedMember
-    items_ids = tools.fncs_map((cat._get_item_ids for cat in categories)) or []
+    items_ids = tools.fncs_map((_._get_item_ids for _ in all_categories)) or []
     items_ids = list(set(chain(*items_ids)))
-    LOG.debug(f"Got {len(items_ids)} item ids from {len(categories)} categories")
+    LOG.debug(f"Got {len(items_ids)} item ids from {all_categories_len} categories")
     items = Item.parse_multiple(*items_ids, parse_subitems=False)
-    LOG.green(f"Got {len(items)} items from {len(categories)} categories")
+    LOG.green(f"Got {len(items)} items from {all_categories_len} categories")
 
     LOG.green("Getting subitem ids")
-    subitems_ids = list(set(list(chain(*[i.subitem_ids for i in items]))))
-    LOG.debug(f"Got {len(subitems_ids)} subitem ids from {len(categories)} categories")
+    subitems_ids = list(set(list(chain(*[_.subitem_ids for _ in items]))))
+    LOG.debug(f"Got {len(subitems_ids)} subitem ids from {all_categories_len} categories")
     subitems = Item.parse_multiple(*subitems_ids, subitems=True)
-    LOG.debug(f"Got {len(subitems)} subitems from {len(categories)} categories")
+    LOG.debug(f"Got {len(subitems)} subitems from {all_categories_len} categories")
 
     # noinspection PyProtectedMember
     all_items = items + subitems + list(Item._cache.values()) + list(SubItem._cache.values())
     all_items = list(set(all_items))
-    LOG.green(f"Got {len(all_items)} total items from {len(categories)} categories")
+    LOG.green(f"Got {len(all_items)} total items from {all_categories_len} categories")
     return all_items
 
 
 def get_super_categories():
     """
 
     :rtype: List[SuperCategory]
@@ -198,15 +202,13 @@
     @property
     def subcategories(self):
         return self._get_subcategories('root_id')
 
 
 if __name__ == '__main__':
     LOG.verbose = True
-    supercategory = SuperCategory.get(1162030)
-    subs = supercategory.subcategories
-    a = list(supercategory.__iter__())
-    # get_super_category_ids = SuperCategory.get_super_category_ids()
-    # get_super_categories = SuperCategory.get_super_categories()
-    # get_all_categories_recursively = list(SuperCategory.get_all_categories_recursively())
+    ac = list(get_all_categories_recursively())
+    # supercategory = SuperCategory.get(4627893)
+    # subs = supercategory.subcategories
+    # a = list(supercategory.__iter__())
     # all_items_ = SuperCategory.get_all_items_recursively()
     pass
```

### Comparing `rozetka_api-1.1.2/rozetka/examples/example_category.py` & `rozetka_api-1.1.3/rozetka/examples/example_category.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.2/rozetka/runners/parse_api.py` & `rozetka_api-1.1.3/rozetka/runners/parse_api.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.2/rozetka/tools/constants.py` & `rozetka_api-1.1.3/rozetka/tools/constants.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.2/rozetka/tools/db.py` & `rozetka_api-1.1.3/rozetka/tools/db.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.2/rozetka/tools/tools.py` & `rozetka_api-1.1.3/rozetka/tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,23 +89,23 @@
     floats = floats_from_str(reviews_str)
     if floats:
         return int(floats[0])
 
 
 # @sleep_and_retry
 @limits(calls=constants.CALLS_MAX, period=constants.CALLS_PERIOD, raise_on_limit=False)
-def get(*args, retry=False, max_tries=3, delay=30, **kwargs) -> Response:
+def get(*args, retry=False, max_tries=10, delay=30, **kwargs) -> Response:
     try:
         response = requests.get(*args, timeout=120, **kwargs)
     except Exception as e:
         response = None
 
     if retry:
         i = 0
-        while response is None or not response.ok and response.status_code in (502, ) and (i := i + 1) < max_tries:
+        while response is None or not response.ok and response.status_code in (502, 524, ) and (i := i + 1) < max_tries:
             if response:
                 LOG.error(f"ERROR Requesting {response.request.url} : {response.status_code}. Retrying in {delay}")
             else:
                 LOG.error(f"ERROR Requesting {args}. Retrying in {delay}")
 
             time.sleep(delay)
             try:
```

### Comparing `rozetka_api-1.1.2/PKG-INFO` & `rozetka_api-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozetka-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Rozetka Python API
 Keywords: rozetka
 Author: Alexey ALERT Rubasheff
 Author-email: alexey.rubasheff@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

