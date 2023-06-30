# Comparing `tmp/rozetka_api-1.1.1.tar.gz` & `tmp/rozetka_api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rozetka_api-1.1.1.tar", max compression
+gzip compressed data, was "rozetka_api-1.1.2.tar", max compression
```

## Comparing `rozetka_api-1.1.1.tar` & `rozetka_api-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      978 2023-06-30 11:53:18.736184 rozetka_api-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      135 2022-09-03 20:53:08.178729 rozetka_api-1.1.1/README.rst
--rw-r--r--   0        0        0        0 2022-09-02 18:14:26.482651 rozetka_api-1.1.1/rozetka/entities/__init__.py
--rw-r--r--   0        0        0    10557 2022-09-11 14:55:35.661756 rozetka_api-1.1.1/rozetka/entities/category.py
--rw-r--r--   0        0        0    11903 2022-09-21 11:51:31.522568 rozetka_api-1.1.1/rozetka/entities/item.py
--rw-r--r--   0        0        0      555 2022-09-21 11:51:31.500532 rozetka_api-1.1.1/rozetka/entities/point.py
--rw-r--r--   0        0        0     8485 2022-10-09 10:10:02.078055 rozetka_api-1.1.1/rozetka/entities/supercategory.py
--rw-r--r--   0        0        0      821 2022-09-03 11:44:07.607811 rozetka_api-1.1.1/rozetka/examples/example_category.py
--rw-r--r--   0        0        0      108 2022-09-03 10:56:00.803564 rozetka_api-1.1.1/rozetka/examples/example_item.py
--rw-r--r--   0        0        0     3390 2023-06-30 11:40:23.368017 rozetka_api-1.1.1/rozetka/runners/parse_api.py
--rw-r--r--   0        0        0        0 2022-08-30 10:55:06.318671 rozetka_api-1.1.1/rozetka/tools/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-30 11:00:39.652176 rozetka_api-1.1.1/rozetka/tools/constants.py
--rw-r--r--   0        0        0     6494 2023-06-30 11:16:50.860136 rozetka_api-1.1.1/rozetka/tools/db.py
--rw-r--r--   0        0        0     3582 2022-09-21 11:51:31.483488 rozetka_api-1.1.1/rozetka/tools/tools.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 rozetka_api-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      978 2023-06-30 13:22:27.305656 rozetka_api-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      135 2022-09-03 20:53:08.178729 rozetka_api-1.1.2/README.rst
+-rw-r--r--   0        0        0        0 2022-09-02 18:14:26.482651 rozetka_api-1.1.2/rozetka/entities/__init__.py
+-rw-r--r--   0        0        0    10637 2023-06-30 13:04:36.394214 rozetka_api-1.1.2/rozetka/entities/category.py
+-rw-r--r--   0        0        0    11959 2023-06-30 13:11:48.616706 rozetka_api-1.1.2/rozetka/entities/item.py
+-rw-r--r--   0        0        0      555 2022-09-21 11:51:31.500532 rozetka_api-1.1.2/rozetka/entities/point.py
+-rw-r--r--   0        0        0     8709 2023-06-30 13:05:29.369115 rozetka_api-1.1.2/rozetka/entities/supercategory.py
+-rw-r--r--   0        0        0      821 2022-09-03 11:44:07.607811 rozetka_api-1.1.2/rozetka/examples/example_category.py
+-rw-r--r--   0        0        0      108 2022-09-03 10:56:00.803564 rozetka_api-1.1.2/rozetka/examples/example_item.py
+-rw-r--r--   0        0        0     3390 2023-06-30 11:40:23.368017 rozetka_api-1.1.2/rozetka/runners/parse_api.py
+-rw-r--r--   0        0        0        0 2022-08-30 10:55:06.318671 rozetka_api-1.1.2/rozetka/tools/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-30 13:21:53.957476 rozetka_api-1.1.2/rozetka/tools/constants.py
+-rw-r--r--   0        0        0     4717 2023-06-30 13:13:17.667363 rozetka_api-1.1.2/rozetka/tools/db.py
+-rw-r--r--   0        0        0     3949 2023-06-30 13:09:17.549730 rozetka_api-1.1.2/rozetka/tools/tools.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 rozetka_api-1.1.2/PKG-INFO
```

### Comparing `rozetka_api-1.1.1/pyproject.toml` & `rozetka_api-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rozetka-api"
-version = "1.1.1"
+version = "1.1.2"
 description = "Rozetka Python API"
 authors = ["Alexey ALERT Rubasheff <alexey.rubasheff@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "rozetka"}]
 keywords = ["rozetka"]
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `rozetka_api-1.1.1/rozetka/entities/category.py` & `rozetka_api-1.1.2/rozetka/entities/category.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,19 @@
             params = {
                 'id': self.id_,
                 'lang': constants.LANGUAGE,
                 'country': constants.COUNTRY,
             }
             url = 'https://xl-catalog-api.rozetka.com.ua/v4/categories/get'
             response = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
+            if response is None:
+                return
+
             self._data = response.json().get('data', dict()) or dict()
+
         return self._data
 
     @data.setter
     def data(self, value):
         self._data = value
 
     @property
@@ -134,15 +138,15 @@
             'sort': 'cheap',
             'state': 'new',
             'category_id': self.id_,
             'page': page,
         }
         response = tools.get('https://xl-catalog-api.rozetka.com.ua/v4/goods/get', params=params,
                              headers=constants.DEFAULT_HEADERS, retry=True)
-        if response.status_code != 200:
+        if response is None or response.status_code != 200:
             return {}
 
         return response.json()
 
     def _get_item_ids(self):
         LOG.debug(f"Getting all item ids for {self}")
         initial = self._get_page()
@@ -284,8 +288,7 @@
 
 
 if __name__ == '__main__':
     LOG.verbose = True
     category_ = Category.get(1162030)
     items_ = category_.items
     pass
-
```

### Comparing `rozetka_api-1.1.1/rozetka/entities/item.py` & `rozetka_api-1.1.2/rozetka/entities/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,19 @@
             'with_groups': 1,
             'with_docket': 1,
             'goods_group_href': 1,
             'product_ids': ",".join(product_ids),
         }
 
         LOG.debug(f"Parsing batch of {len(product_ids)} products")
+        output = []
         req = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
+        if req is None:
+            return output
+
         data: List[dict] = req.json().get('data')
         """
         {
             "id": 280528638,
             "title": "Мобільний телефон Samsung Galaxy A32 4/128 GB Black",
             "title_suffix": "",
             "price": 10399,
@@ -186,15 +190,15 @@
                 "pictograms": true,
                 "description": true,
                 "variables": true,
                 "hide_rating_review": false
             }
         }
         """
-        output = []
+
         for item_data in data:
             id_ = item_data.get('id')
             if not id_:
                 continue
 
             item_data.pop('id')
             if subitems:
```

### Comparing `rozetka_api-1.1.1/rozetka/entities/point.py` & `rozetka_api-1.1.2/rozetka/entities/point.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.1/rozetka/entities/supercategory.py` & `rozetka_api-1.1.2/rozetka/entities/supercategory.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,20 @@
         return SuperCategory._fat_menu_categories
 
     params = {
         'front-type': 'xl',
         'country': 'UA',
         'lang': 'ua',
     }
+    output = []
     response = tools.get('https://common-api.rozetka.com.ua/v2/fat-menu/full', params=params,
                          headers=constants.DEFAULT_HEADERS, retry=True)
-    output = []
+    if response is None:
+        return output
+
     data: dict = response.json().get('data', dict())
     for div in data.values():
         children = div.get('children', dict())
         # noinspection DuplicatedCode
         if not children:
             category_id = div.get('category_id')
             if category_id is not None:
@@ -106,16 +109,17 @@
 def get_super_category_ids():
     # noinspection PyProtectedMember
     if SuperCategory._super_category_ids is None:
         LOG.debug(f"Getting super category ids")
         url = 'https://xl-catalog-api.rozetka.com.ua/v4/super-portals/getList'
         response: Response = tools.get(url, headers=constants.DEFAULT_HEADERS, cookies=constants.DEFAULT_COOKIES,
                                        retry=True)
-        if not response.ok:
-            msg = f'Error requesting "{url}": {response.status_code} {response.reason}'
+        if response is None or not response.ok:
+            msg = f'Error requesting "{url}": {response.status_code if response is not None else None} ' \
+                  f'{response.reason if response is not None else None}'
             LOG.error(msg)
             raise Exception(msg)
 
         SuperCategory._super_category_ids = output = response.json().get('data', list())
         # noinspection PyProtectedMember
         SuperCategory._super_category_ids.sort()
         LOG.debug(f"Got {len(output)} super category ids")
@@ -156,14 +160,17 @@
             params = {
                 'category_id': self.id_,
                 'lang': constants.LANGUAGE,
                 'country': constants.COUNTRY,
             }
             url = 'https://xl-catalog-api.rozetka.com.ua/v4/super-portals/get'
             response = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
+            if response is None:
+                return
+
             self._data = response.json().get('data', dict()) or dict()
         return self._data
 
     @data.setter
     def data(self, value):
         self._data = value
```

### Comparing `rozetka_api-1.1.1/rozetka/examples/example_category.py` & `rozetka_api-1.1.2/rozetka/examples/example_category.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.1/rozetka/runners/parse_api.py` & `rozetka_api-1.1.2/rozetka/runners/parse_api.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.1/rozetka/tools/constants.py` & `rozetka_api-1.1.2/rozetka/tools/constants.py`

 * *Files identical despite different names*

### Comparing `rozetka_api-1.1.1/rozetka/tools/tools.py` & `rozetka_api-1.1.2/rozetka/tools/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,24 +87,37 @@
         return
 
     floats = floats_from_str(reviews_str)
     if floats:
         return int(floats[0])
 
 
-@sleep_and_retry
-@limits(calls=constants.CALLS_MAX, period=constants.CALLS_PERIOD)
+# @sleep_and_retry
+@limits(calls=constants.CALLS_MAX, period=constants.CALLS_PERIOD, raise_on_limit=False)
 def get(*args, retry=False, max_tries=3, delay=30, **kwargs) -> Response:
-    response = requests.get(*args, timeout=60, **kwargs)
+    try:
+        response = requests.get(*args, timeout=120, **kwargs)
+    except Exception as e:
+        response = None
+
     if retry:
         i = 0
-        while not response.ok and response.status_code in (502, ) and (i := i + 1) < max_tries:
-            LOG.error(f"ERROR Requesting {response.request.url} : {response.status_code}. Retrying in {delay}")
+        while response is None or not response.ok and response.status_code in (502, ) and (i := i + 1) < max_tries:
+            if response:
+                LOG.error(f"ERROR Requesting {response.request.url} : {response.status_code}. Retrying in {delay}")
+            else:
+                LOG.error(f"ERROR Requesting {args}. Retrying in {delay}")
+
             time.sleep(delay)
-            response = requests.get(*args, **kwargs)
+            try:
+                response = requests.get(*args, timeout=120, **kwargs)
+            except Exception as e:
+                response = None
+                pass
+
     return response
 
 
 def fnc_map(fnc, *tuple_of_args, **kwargs):
     @worker
     def _worker(*worker_args, **worker_kwargs):
         return fnc(*worker_args, **worker_kwargs)
@@ -135,8 +148,7 @@
         worker_.wait()
         outputs.append(worker_.ret)
     return outputs
 
 
 def slice_list(list_, chunk_size):
     return [list_[i:i + chunk_size] for i in range(0, len(list_), chunk_size)]
-
```

### Comparing `rozetka_api-1.1.1/PKG-INFO` & `rozetka_api-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozetka-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Rozetka Python API
 Keywords: rozetka
 Author: Alexey ALERT Rubasheff
 Author-email: alexey.rubasheff@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

