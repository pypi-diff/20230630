# Comparing `tmp/rozetka_api-1.1.3.tar.gz` & `tmp/rozetka_api-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rozetka_api-1.1.3.tar", max compression
+gzip compressed data, was "rozetka_api-1.1.4.tar", max compression
```

## Comparing `rozetka_api-1.1.3.tar` & `rozetka_api-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      978 2023-06-30 15:29:40.460135 rozetka_api-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      135 2022-09-03 20:53:08.178729 rozetka_api-1.1.3/README.rst
--rw-r--r--   0        0        0        0 2022-09-02 18:14:26.482651 rozetka_api-1.1.3/rozetka/entities/__init__.py
--rw-r--r--   0        0        0    10637 2023-06-30 13:04:36.394214 rozetka_api-1.1.3/rozetka/entities/category.py
--rw-r--r--   0        0        0    12027 2023-06-30 14:17:20.527737 rozetka_api-1.1.3/rozetka/entities/item.py
--rw-r--r--   0        0        0      555 2022-09-21 11:51:31.500532 rozetka_api-1.1.3/rozetka/entities/point.py
--rw-r--r--   0        0        0     8695 2023-06-30 15:01:21.625968 rozetka_api-1.1.3/rozetka/entities/supercategory.py
--rw-r--r--   0        0        0      821 2022-09-03 11:44:07.607811 rozetka_api-1.1.3/rozetka/examples/example_category.py
--rw-r--r--   0        0        0      108 2022-09-03 10:56:00.803564 rozetka_api-1.1.3/rozetka/examples/example_item.py
--rw-r--r--   0        0        0     3390 2023-06-30 11:40:23.368017 rozetka_api-1.1.3/rozetka/runners/parse_api.py
--rw-r--r--   0        0        0        0 2022-08-30 10:55:06.318671 rozetka_api-1.1.3/rozetka/tools/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-30 13:21:53.957476 rozetka_api-1.1.3/rozetka/tools/constants.py
--rw-r--r--   0        0        0     4717 2023-06-30 13:13:17.667363 rozetka_api-1.1.3/rozetka/tools/db.py
--rw-r--r--   0        0        0     3955 2023-06-30 14:32:19.224443 rozetka_api-1.1.3/rozetka/tools/tools.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 rozetka_api-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      244 2023-06-30 17:07:45.087411 rozetka_api-1.1.4/README.rst
+-rw-r--r--   0        0        0      989 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/entities/__init__.py
+-rw-r--r--   0        0        0    10343 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/entities/category.py
+-rw-r--r--   0        0        0    11705 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/entities/item.py
+-rw-r--r--   0        0        0      535 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/entities/point.py
+-rw-r--r--   0        0        0     8481 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/entities/supercategory.py
+-rw-r--r--   0        0        0      770 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/examples/example_category.py
+-rw-r--r--   0        0        0      103 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/examples/example_item.py
+-rw-r--r--   0        0        0     3298 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/runners/parse_api.py
+-rw-r--r--   0        0        0        0 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/tools/__init__.py
+-rw-r--r--   0        0        0     1755 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/tools/constants.py
+-rw-r--r--   0        0        0     4593 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/tools/db.py
+-rw-r--r--   0        0        0     3801 2023-06-30 17:07:45.091411 rozetka_api-1.1.4/rozetka/tools/tools.py
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 rozetka_api-1.1.4/setup.py
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 rozetka_api-1.1.4/PKG-INFO
```

### Comparing `rozetka_api-1.1.3/pyproject.toml` & `rozetka_api-1.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-[tool.poetry]
-name = "rozetka-api"
-version = "1.1.3"
-description = "Rozetka Python API"
-authors = ["Alexey ALERT Rubasheff <alexey.rubasheff@gmail.com>"]
-readme = "README.rst"
-packages = [{include = "rozetka"}]
-keywords = ["rozetka"]
-classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules"
-]
-
-[tool.poetry.build]
-generate-setup-file = false
-
-[tool.poetry.dependencies]
-python = "^3.10"
-pip = "^22.2.2"
-requests = "^2.28.1"
-pathlib = "^1.0.1"
-pendulum = "^2.1.2"
-influxdb = {extras = ["async"], version = "^5.3.1"}
-aiohttp-retry = "^2.8.3"
-global-logger = "^0.3.30"
-progress = "^1.6"
-ratelimit = "^2.2.1"
-python-worker = "^1.10.1"
-knockknock = "^0.1.8.1"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.1.3"
-
-[tool.poetry-dynamic-versioning]
-enable = true
-vcs = "git"
-style = "semver"
-
-[build-system]
-requires = ["poetry-core", "poetry-dynamic-versioning"]
-build-backend = "poetry_dynamic_versioning.backend"
+[tool.poetry]
+name = "rozetka-api"
+version = "1.1.4"
+description = "Rozetka Python API"
+authors = ["Alexey ALERT Rubasheff <alexey.rubasheff@gmail.com>"]
+readme = "README.rst"
+packages = [{include = "rozetka"}]
+homepage = "https://github.com/ALERTua/rozetka_api"
+keywords = ["rozetka"]
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
+
+[tool.poetry.build]
+generate-setup-file = true
+
+[tool.poetry.dependencies]
+python = "^3.10"
+pip = "^22.2.2"
+requests = "^2.28.1"
+pathlib = "^1.0.1"
+pendulum = "^2.1.2"
+influxdb = {extras = ["async"], version = "^5.3.1"}
+aiohttp-retry = "^2.8.3"
+global-logger = "^0.3.30"
+progress = "^1.6"
+ratelimit = "^2.2.1"
+python-worker = "^1.10.1"
+knockknock = "^0.1.8.1"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.1.3"
+
+[tool.poetry-dynamic-versioning]
+enable = true
+vcs = "git"
+style = "semver"
+
+[build-system]
+requires = ["poetry-core", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `rozetka_api-1.1.3/rozetka/entities/category.py` & `rozetka_api-1.1.4/rozetka/entities/category.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-from rozetka.entities.item import Item
-from typing import List
-
-from global_logger import Log
-
-from rozetka.tools import tools, constants
-
-LOG = Log.get_logger()
-
-
-class Category:
-    _cache: dict[int, object] = dict()
-
-    def __init__(self, id_, title=None, url=None, parent_category=None, parent_category_id=None, direct=True):
-        assert direct is False, f"You cannot use {self.__class__.__name__} directly. Please use get classmethod."
-        self.id_ = id_
-        assert isinstance(self.id_, int), f"{self.__class__.__name__} id must be an int"
-        self._title = title
-        self.url = url
-        self._items_ids = None
-        self._items = None
-        self._parent_category_id = parent_category_id
-        self._parent_category = parent_category
-        self._data: dict | None = None
-        self._subcategories_data: List[dict] | None = None
-        self._subcategories: List[Category] | None = None
-
-    def __str__(self):
-        if self._title:
-            return f"({self.id_}) {self.title}"
-
-        return f"{self.id_}"
-
-    def __repr__(self):
-        return f"[{self.__class__.__name__}]{self.__str__()}"
-
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and self.id_ == other.id_
-
-    def __hash__(self):
-        return int(self.id_)
-
-    def __iter__(self):
-        for subcategory in self.subcategories:
-            LOG.debug(f"category iter: yielding {subcategory}")
-            yield subcategory
-            LOG.debug(f"category iter: yielding from {subcategory}")
-            yield from subcategory.__iter__()
-
-    @property
-    def data(self):
-        if self._data is None:
-            params = {
-                'id': self.id_,
-                'lang': constants.LANGUAGE,
-                'country': constants.COUNTRY,
-            }
-            url = 'https://xl-catalog-api.rozetka.com.ua/v4/categories/get'
-            response = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
-            if response is None:
-                return
-
-            self._data = response.json().get('data', dict()) or dict()
-
-        return self._data
-
-    @data.setter
-    def data(self, value):
-        self._data = value
-
-    @property
-    def title(self):
-        if self._title is None:
-            self._title = self.data.get('title')
-        return self._title
-
-    @title.setter
-    def title(self, value):
-        self._title = value
-
-    @property
-    def parent_category(self):
-        if self._parent_category:
-            return self._parent_category
-
-        if self.parent_category_id:
-            self._parent_category = self.__class__.get(self.parent_category_id)
-        return self._parent_category
-
-    @parent_category.setter
-    def parent_category(self, value):
-        self._parent_category = value
-
-    @property
-    def parent_category_id(self):
-        if self._parent_category_id:
-            return self._parent_category_id
-
-        if self._parent_category:
-            self._parent_category_id = self._parent_category.id_
-
-        return self._parent_category_id
-
-    @parent_category_id.setter
-    def parent_category_id(self, value):
-        self._parent_category_id = value
-
-    @classmethod
-    def get(cls, id_, title=None, url=None, data=None, parent_category_id=None, parent_category=None):
-        if id_ in cls._cache:
-            # noinspection PyTypeChecker
-            output: Category = cls._cache.get(id_)
-            output.title = output._title or title
-            output.url = output.url or url
-            output.parent_category_id = output._parent_category_id or parent_category_id
-            output.parent_category = output._parent_category or parent_category
-            output.data = output._data or data
-        else:
-            from rozetka.entities.supercategory import SuperCategory
-            class_ = Category
-            from rozetka.entities.supercategory import get_super_category_ids
-            if id_ in get_super_category_ids():
-                class_ = SuperCategory
-            output = class_(id_=id_, title=title, url=url, parent_category_id=parent_category_id,
-                            parent_category=parent_category, direct=False)
-            output.data = output._data or data
-            cls._cache[id_] = output
-        return output
-
-    def _get_page(self, page=1):
-        # LOG.debug(f"Getting {self} page {page}")
-        params = {
-            'front-type': 'xl',
-            'country': constants.COUNTRY,
-            'lang': constants.LANGUAGE,
-            'sell_status': 'available,limited',
-            'seller': 'rozetka',
-            'sort': 'cheap',
-            'state': 'new',
-            'category_id': self.id_,
-            'page': page,
-        }
-        response = tools.get('https://xl-catalog-api.rozetka.com.ua/v4/goods/get', params=params,
-                             headers=constants.DEFAULT_HEADERS, retry=True)
-        if response is None or response.status_code != 200:
-            return {}
-
-        return response.json()
-
-    def _get_item_ids(self):
-        LOG.debug(f"Getting all item ids for {self}")
-        initial = self._get_page()
-        if not initial:
-            return []
-
-        data = initial.get('data')
-        output: list = data.get('ids', list())
-        total_pages = data.get('total_pages', 1)
-        pages = [i for i in range(2, total_pages + 1)]
-        results = []
-        # for page in alive_it(pages):
-        for page in pages:
-            result = self._get_page(page)
-            results.append(result)
-
-        for result in results:
-            ids = result.get('data', dict()).get('ids', list())
-            output.extend(ids)
-        output = [i for i in output if i is not None]
-        output = list(set(output))
-        output.sort()
-        LOG.debug(f"Got {len(output)} item ids for {self}")
-        return output
-
-    @property
-    def items_ids(self):
-        if self._items_ids is None:
-            self._items_ids = self._get_item_ids()
-        return self._items_ids
-
-    @property
-    def items(self):
-        if self._items is None:
-            LOG.debug(f"Getting all items for {self}")
-            item_ids = self.items_ids
-            if not item_ids:
-                return []
-
-            from rozetka.entities.item import Item
-            items = [Item.get(i) for i in item_ids]
-            # items.extend([list(i.__iter__()) for i in items])
-            output = []
-            for item in items:
-                item.category = self
-                output.append(item)
-            output = list(set(output))
-            output.sort(key=lambda i: i.id_)
-            LOG.debug(f"Got {len(output)} items for {self}")
-            self._items = output
-        return self._items
-
-    def parse_items(self):
-        _ = Item.parse_multiple(*self.items_ids, parse_subitems=True)
-
-    @property
-    def subcategories_data(self):
-        if self._subcategories_data is None:
-            data = self.data
-            if not data:
-                return []
-
-            id_ = data.get('id')
-            if not id_:
-                data = data.get('category')
-                id_ = data.get('id')
-            assert id_ == self.id_
-
-            title = data.get('title')
-            if title and self._title is None:
-                self.title = title
-
-            url = data.get('href')
-            if url and self.url is None:
-                self.url = url
-
-            parent_category_id = data.get('root_id')
-            if parent_category_id and self._parent_category_id is None:
-                self.parent_category_id = parent_category_id
-
-            self._subcategories_data = data.get('children', list())
-        return self._subcategories_data
-
-    @subcategories_data.setter
-    def subcategories_data(self, value):
-        self._subcategories_data = value
-
-    def _get_subcategories(self, parent_key='parent_id'):
-        if self._subcategories is None:
-            if not (subcategories_data := self.subcategories_data):
-                # LOG.debug(f"No subcategories found for  {self}")
-                self._subcategories = []
-                return self._subcategories
-
-            output = []
-            for subcategory_data in subcategories_data:
-                parent_category_id = subcategory_data.get(parent_key, subcategory_data.get('parent_id'))
-                if not parent_category_id:
-                    LOG.error("THIS SHOULDN'T HAPPEN")
-
-                if parent_category_id != self.id_:
-                    pop = subcategories_data.pop(subcategories_data.index(subcategory_data))
-                    true_cat = Category.get(parent_category_id)
-                    true_cat.subcategories_data = true_cat.subcategories_data or []
-                    true_cat.subcategories_data.append(pop)
-                    true_cat.subcategories_data.sort(key=lambda i: i.get('id', 0))
-                    true_subcategories_data = []
-                    for data in true_cat.subcategories_data:
-                        if data.get('id') not in [i.get('id') for i in true_subcategories_data]:
-                            true_subcategories_data.append(data)
-                    true_cat.subcategories_data = true_subcategories_data
-                    continue
-
-                id_ = subcategory_data.get('id')
-                title = subcategory_data.get('title')
-                url = subcategory_data.get('href')
-                if self.id_ == id_:
-                    LOG.warning(f"Loop subcategory detected @ {id_} {title}")
-                    continue
-
-                children = subcategory_data.get('children', list())
-
-                subcategory = Category.get(id_)
-                subcategory.title = title
-                subcategory.url = url
-                subcategory.parent_category_id = parent_category_id
-                subcategory.parent_category = self
-                subcategory.subcategories_data = children
-                output.append(subcategory)
-
-            output.sort(key=lambda i: i.id_)
-            self._subcategories = output
-            LOG.debug(f"Got {len(output)} subcategories for {self}")
-        return self._subcategories
-
-    @property
-    def subcategories(self):
-        return self._get_subcategories()
-
-
-if __name__ == '__main__':
-    LOG.verbose = True
-    category_ = Category.get(1162030)
-    items_ = category_.items
-    pass
+from rozetka.entities.item import Item
+from typing import List
+
+from global_logger import Log
+
+from rozetka.tools import tools, constants
+
+LOG = Log.get_logger()
+
+
+class Category:
+    _cache: dict[int, object] = dict()
+
+    def __init__(self, id_, title=None, url=None, parent_category=None, parent_category_id=None, direct=True):
+        assert direct is False, f"You cannot use {self.__class__.__name__} directly. Please use get classmethod."
+        self.id_ = id_
+        assert isinstance(self.id_, int), f"{self.__class__.__name__} id must be an int"
+        self._title = title
+        self.url = url
+        self._items_ids = None
+        self._items = None
+        self._parent_category_id = parent_category_id
+        self._parent_category = parent_category
+        self._data: dict | None = None
+        self._subcategories_data: List[dict] | None = None
+        self._subcategories: List[Category] | None = None
+
+    def __str__(self):
+        if self._title:
+            return f"({self.id_}) {self.title}"
+
+        return f"{self.id_}"
+
+    def __repr__(self):
+        return f"[{self.__class__.__name__}]{self.__str__()}"
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.id_ == other.id_
+
+    def __hash__(self):
+        return int(self.id_)
+
+    def __iter__(self):
+        for subcategory in self.subcategories:
+            LOG.debug(f"category iter: yielding {subcategory}")
+            yield subcategory
+            LOG.debug(f"category iter: yielding from {subcategory}")
+            yield from subcategory.__iter__()
+
+    @property
+    def data(self):
+        if self._data is None:
+            params = {
+                'id': self.id_,
+                'lang': constants.LANGUAGE,
+                'country': constants.COUNTRY,
+            }
+            url = 'https://xl-catalog-api.rozetka.com.ua/v4/categories/get'
+            response = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
+            if response is None:
+                return
+
+            self._data = response.json().get('data', dict()) or dict()
+
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        self._data = value
+
+    @property
+    def title(self):
+        if self._title is None:
+            self._title = self.data.get('title')
+        return self._title
+
+    @title.setter
+    def title(self, value):
+        self._title = value
+
+    @property
+    def parent_category(self):
+        if self._parent_category:
+            return self._parent_category
+
+        if self.parent_category_id:
+            self._parent_category = self.__class__.get(self.parent_category_id)
+        return self._parent_category
+
+    @parent_category.setter
+    def parent_category(self, value):
+        self._parent_category = value
+
+    @property
+    def parent_category_id(self):
+        if self._parent_category_id:
+            return self._parent_category_id
+
+        if self._parent_category:
+            self._parent_category_id = self._parent_category.id_
+
+        return self._parent_category_id
+
+    @parent_category_id.setter
+    def parent_category_id(self, value):
+        self._parent_category_id = value
+
+    @classmethod
+    def get(cls, id_, title=None, url=None, data=None, parent_category_id=None, parent_category=None):
+        if id_ in cls._cache:
+            # noinspection PyTypeChecker
+            output: Category = cls._cache.get(id_)
+            output.title = output._title or title
+            output.url = output.url or url
+            output.parent_category_id = output._parent_category_id or parent_category_id
+            output.parent_category = output._parent_category or parent_category
+            output.data = output._data or data
+        else:
+            from rozetka.entities.supercategory import SuperCategory
+            class_ = Category
+            from rozetka.entities.supercategory import get_super_category_ids
+            if id_ in get_super_category_ids():
+                class_ = SuperCategory
+            output = class_(id_=id_, title=title, url=url, parent_category_id=parent_category_id,
+                            parent_category=parent_category, direct=False)
+            output.data = output._data or data
+            cls._cache[id_] = output
+        return output
+
+    def _get_page(self, page=1):
+        # LOG.debug(f"Getting {self} page {page}")
+        params = {
+            'front-type': 'xl',
+            'country': constants.COUNTRY,
+            'lang': constants.LANGUAGE,
+            'sell_status': 'available,limited',
+            'seller': 'rozetka',
+            'sort': 'cheap',
+            'state': 'new',
+            'category_id': self.id_,
+            'page': page,
+        }
+        response = tools.get('https://xl-catalog-api.rozetka.com.ua/v4/goods/get', params=params,
+                             headers=constants.DEFAULT_HEADERS, retry=True)
+        if response is None or response.status_code != 200:
+            return {}
+
+        return response.json()
+
+    def _get_item_ids(self):
+        LOG.debug(f"Getting all item ids for {self}")
+        initial = self._get_page()
+        if not initial:
+            return []
+
+        data = initial.get('data')
+        output: list = data.get('ids', list())
+        total_pages = data.get('total_pages', 1)
+        pages = [i for i in range(2, total_pages + 1)]
+        results = []
+        # for page in alive_it(pages):
+        for page in pages:
+            result = self._get_page(page)
+            results.append(result)
+
+        for result in results:
+            ids = result.get('data', dict()).get('ids', list())
+            output.extend(ids)
+        output = [i for i in output if i is not None]
+        output = list(set(output))
+        output.sort()
+        LOG.debug(f"Got {len(output)} item ids for {self}")
+        return output
+
+    @property
+    def items_ids(self):
+        if self._items_ids is None:
+            self._items_ids = self._get_item_ids()
+        return self._items_ids
+
+    @property
+    def items(self):
+        if self._items is None:
+            LOG.debug(f"Getting all items for {self}")
+            item_ids = self.items_ids
+            if not item_ids:
+                return []
+
+            from rozetka.entities.item import Item
+            items = [Item.get(i) for i in item_ids]
+            # items.extend([list(i.__iter__()) for i in items])
+            output = []
+            for item in items:
+                item.category = self
+                output.append(item)
+            output = list(set(output))
+            output.sort(key=lambda i: i.id_)
+            LOG.debug(f"Got {len(output)} items for {self}")
+            self._items = output
+        return self._items
+
+    def parse_items(self):
+        _ = Item.parse_multiple(*self.items_ids, parse_subitems=True)
+
+    @property
+    def subcategories_data(self):
+        if self._subcategories_data is None:
+            data = self.data
+            if not data:
+                return []
+
+            id_ = data.get('id')
+            if not id_:
+                data = data.get('category')
+                id_ = data.get('id')
+            assert id_ == self.id_
+
+            title = data.get('title')
+            if title and self._title is None:
+                self.title = title
+
+            url = data.get('href')
+            if url and self.url is None:
+                self.url = url
+
+            parent_category_id = data.get('root_id')
+            if parent_category_id and self._parent_category_id is None:
+                self.parent_category_id = parent_category_id
+
+            self._subcategories_data = data.get('children', list())
+        return self._subcategories_data
+
+    @subcategories_data.setter
+    def subcategories_data(self, value):
+        self._subcategories_data = value
+
+    def _get_subcategories(self, parent_key='parent_id'):
+        if self._subcategories is None:
+            if not (subcategories_data := self.subcategories_data):
+                # LOG.debug(f"No subcategories found for  {self}")
+                self._subcategories = []
+                return self._subcategories
+
+            output = []
+            for subcategory_data in subcategories_data:
+                parent_category_id = subcategory_data.get(parent_key, subcategory_data.get('parent_id'))
+                if not parent_category_id:
+                    LOG.error("THIS SHOULDN'T HAPPEN")
+
+                if parent_category_id != self.id_:
+                    pop = subcategories_data.pop(subcategories_data.index(subcategory_data))
+                    true_cat = Category.get(parent_category_id)
+                    true_cat.subcategories_data = true_cat.subcategories_data or []
+                    true_cat.subcategories_data.append(pop)
+                    true_cat.subcategories_data.sort(key=lambda i: i.get('id', 0))
+                    true_subcategories_data = []
+                    for data in true_cat.subcategories_data:
+                        if data.get('id') not in [i.get('id') for i in true_subcategories_data]:
+                            true_subcategories_data.append(data)
+                    true_cat.subcategories_data = true_subcategories_data
+                    continue
+
+                id_ = subcategory_data.get('id')
+                title = subcategory_data.get('title')
+                url = subcategory_data.get('href')
+                if self.id_ == id_:
+                    LOG.warning(f"Loop subcategory detected @ {id_} {title}")
+                    continue
+
+                children = subcategory_data.get('children', list())
+
+                subcategory = Category.get(id_)
+                subcategory.title = title
+                subcategory.url = url
+                subcategory.parent_category_id = parent_category_id
+                subcategory.parent_category = self
+                subcategory.subcategories_data = children
+                output.append(subcategory)
+
+            output.sort(key=lambda i: i.id_)
+            self._subcategories = output
+            LOG.debug(f"Got {len(output)} subcategories for {self}")
+        return self._subcategories
+
+    @property
+    def subcategories(self):
+        return self._get_subcategories()
+
+
+if __name__ == '__main__':
+    LOG.verbose = True
+    category_ = Category.get(1162030)
+    items_ = category_.items
+    pass
```

### Comparing `rozetka_api-1.1.3/rozetka/entities/item.py` & `rozetka_api-1.1.4/rozetka/entities/item.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,322 +1,322 @@
-from functools import cached_property
-from typing import Dict, List, Collection
-
-from global_logger import Log
-
-from rozetka.tools import tools, constants
-
-LOG = Log.get_logger()
-
-
-class Item:
-    _cache = dict()  # type: Dict[int, Item]
-    _data: Dict = dict()
-
-    def __init__(self, id_, direct=True, **kwargs):
-        assert direct is False, f"You cannot use {self.__class__.__name__} directly. Please use get classmethod."
-        self.id_ = id_
-        assert isinstance(self.id_, int), f"{self.__class__.__name__} id must be an int"
-        self.category = None
-        self.data = kwargs
-
-        if (stars := self.__dict__.get('stars', None)) is not None:
-            if '%' in str(stars):
-                self.stars = int(stars.rstrip('%')) / 100
-
-        if (comments_mark := self.__dict__.get('comments_mark', None)) is not None:
-            self.comments_mark = float(comments_mark)
-
-        self._parsed = False
-
-    def __str__(self):
-        if title := self.__dict__.get('title'):
-            return f"({self.id_}) {title}"
-
-        return f"{self.id_}"
-
-    def __repr__(self):
-        return f"[{self.__class__.__name__}]{self.__str__()}"
-
-    def __iter__(self):
-        for subitem in self.subitems:
-            yield subitem
-            # yield from subitem.__iter__()  # prevent sub-subitems
-
-    @staticmethod
-    def _parse_batch(*product_ids, subitems=False, parse_subitems=True):
-        url = 'https://xl-catalog-api.rozetka.com.ua/v4/goods/getDetails'
-        params = {
-            'country': constants.COUNTRY,
-            'lang': constants.LANGUAGE,
-            'with_groups': 1,
-            'with_docket': 1,
-            'goods_group_href': 1,
-            'product_ids': ",".join(product_ids),
-        }
-
-        LOG.debug(f"Parsing batch of {len(product_ids)} products")
-        output = []
-        req = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
-        if req is None:
-            return output
-
-        try:
-            data: List[dict] = req.json().get('data')
-        except Exception as e:
-            pass
-        """
-        {
-            "id": 280528638,
-            "title": "Мобільний телефон Samsung Galaxy A32 4/128 GB Black",
-            "title_suffix": "",
-            "price": 10399,
-            "old_price": 10499,
-            "price_pcs": "281.05",
-            "href": "https://rozetka.com.ua/ua/samsung_galaxy_a32_4_128gb_black/p280528638/",
-            "status": "active",
-            "status_inherited": "active",
-            "sell_status": "available",
-            "category_id": 80003,
-            "seller_id": 5,
-            "merchant_id": 1,
-            "brand": "Samsung",
-            "brand_id": 12,
-            "group_id": 36310773,
-            "group_name": "36310773",
-            "group_title": "Мобільний телефон Samsung Galaxy A32 4/128GB",
-            "pl_bonus_charge_pcs": 0,
-            "pl_use_instant_bonus": 0,
-            "state": "new",
-            "docket": "Екран (6.4\", Super AMOLED, 2400x1080) / Mediatek Helio G80 (2 x 2.0 ГГц + 6 x 1.8 ГГц) / 
-            "mpath": ".4627949.80003.",
-            "is_group_primary": 1,
-            "dispatch": 1,
-            "premium": 0,
-            "preorder": 0,
-            "comments_amount": 109,
-            "comments_mark": 3.9,
-            "gift": null,
-            "tag": {
-                "name": "action",
-                "title": "Акция",
-                "priority": 9,
-                "goods_id": 280528638
-            },
-            "pictograms": [{
-                    "is_auction": true,
-                    "view_position": 1,
-                    "order": 49,
-                    "id": 30277,
-                    "goods_id": 280528638,
-                    "title": "ROZETKA Обмін",
-                    "image_url": "https://content2.rozetka.com.ua/goods_tags/images_ua/original/222408740.png",
-                    "view_type": "in_central_block",
-                    "announce": null,
-                    "has_description": 1,
-                    "description": null,
-                    "url": null,
-                    "url_title": null,
-                    "icon_mobile": ""
-                }
-            ],
-            "title_mode": null,
-            "use_group_links": null,
-            "is_need_street_id": false,
-            "image_main": "https://content1.rozetka.com.ua/goods/images/big_tile/175376690.jpg",
-            "images": {
-                "main": "https://content1.rozetka.com.ua/goods/images/big_tile/175376690.jpg",
-                "preview": "https://content1.rozetka.com.ua/goods/images/preview/175376690.jpg",
-                "hover": "https://content.rozetka.com.ua/goods/images/big_tile/175376700.jpg",
-                "all_images": ["https://content1.rozetka.com.ua/goods/images/original/175376690.jpg", 
-                                "https://content.rozetka.com.ua/goods/images/original/175376700.jpg", 
-                                "https://content2.rozetka.com.ua/goods/images/original/175376709.jpg", 
-                                "https://content1.rozetka.com.ua/goods/images/original/175376715.jpg", 
-                                "https://content1.rozetka.com.ua/goods/images/original/175376721.jpg", 
-                                "https://content1.rozetka.com.ua/goods/images/original/175376697.jpg", 
-                                "https://content1.rozetka.com.ua/goods/images/original/175376698.jpg", 
-                                "https://content.rozetka.com.ua/goods/images/original/175376694.jpg"]
-            },
-            "parent_category_id": 4627949,
-            "is_docket": true,
-            "primary_good_title": "Мобільний телефон Samsung Galaxy A32 4/128 GB Black",
-            "groups": {
-                "color": [{
-                        "value": "Black",
-                        "href": "https://rozetka.com.ua/ua/samsung_galaxy_a32_4_128gb_black/p280528638/",
-                        "rank": "99.9997",
-                        "id": 280528638,
-                        "is_group_primary": 1,
-                        "option_id": 21716,
-                        "option_name": "21716",
-                        "value_id": 6691,
-                        "color": {
-                            "id": 6691,
-                            "hash": "#000",
-                            "url": null
-                        },
-                        "active_option": true
-                    }, {
-                        "value": "Lavenda",
-                        "href": "https://rozetka.com.ua/ua/samsung_galaxy_a32_4_128gb_lavender/p280528633/",
-                        "rank": "99.9997",
-                        "id": 280528633,
-                        "is_group_primary": 0,
-                        "option_id": 21716,
-                        "option_name": "21716",
-                        "value_id": 1360088,
-                        "color": {
-                            "id": 1360088,
-                            "hash": "#000",
-                        "url": "https://content.rozetka.com.ua/goods_details_values/images/original/196717502.jpg"
-                        },
-                        "active_option": false
-                    }
-                ]
-            },
-            "stars": "78%",
-            "discount": 1,
-            "config": {
-                "title": true,
-                "brand": false,
-                "image": true,
-                "price": true,
-                "old_price": true,
-                "promo_price": true,
-                "status": true,
-                "bonus": true,
-                "gift": true,
-                "rating": true,
-                "wishlist_button": true,
-                "compare_button": true,
-                "buy_button": true,
-                "tags": true,
-                "pictograms": true,
-                "description": true,
-                "variables": true,
-                "hide_rating_review": false
-            }
-        }
-        """
-
-        for item_data in data:
-            id_ = item_data.get('id')
-            if not id_:
-                continue
-
-            item_data.pop('id')
-            if subitems:
-                item = SubItem.get(id_, **item_data)
-            else:
-                item = Item.get(id_, **item_data)
-            item._parsed = True
-            output.append(item)
-
-            if parse_subitems:
-                output.extend(item.subitems)
-        LOG.debug(f"Parsing batch of {len(product_ids)} products done. Got {len(output)} Items")
-        return output
-
-    @staticmethod
-    def parse_multiple(*product_ids, subitems=False, parse_subitems=True):
-        if not product_ids:
-            return []
-
-        if isinstance(product_ids[0], Item):
-            product_ids = [i.id_ for i in product_ids]
-        elif isinstance(product_ids[0], Collection):
-            product_ids = product_ids[0]
-
-        product_ids_str = [str(i) for i in product_ids]
-        chunk_size = 900
-        chunked_lists = tools.slice_list(product_ids_str, chunk_size)
-        LOG.debug(f"Parsing {len(product_ids)} products divided into {len(chunked_lists)} batches by {chunk_size} each")
-        outputs = tools.fnc_map(Item._parse_batch, *chunked_lists, subitems=subitems, parse_subitems=parse_subitems)
-        outputs = [i for i in outputs if i]
-        output = []
-        for list_ in outputs:
-            output.extend(list_)
-        return output
-
-    @cached_property
-    def subitem_ids(self):
-        groups = self._data.get('groups', {})
-        if not groups:
-            return []
-
-        for _, block in groups.items():
-            block_iterator = block if isinstance(block, list) else block.values()
-            for group in block_iterator:
-                if isinstance(group, list):
-                    subitem_iterator = group
-                elif isinstance(group, dict):
-                    subitem_iterator = [group]
-                else:
-                    continue
-
-                for subitem in subitem_iterator:
-                    if id_ := subitem.get('id'):
-                        if id_ == self.id_:
-                            continue
-
-                        yield id_
-
-    @cached_property
-    def subitems(self):
-        subitem_ids = list(set(self.subitem_ids))
-        if not subitem_ids:
-            return []
-
-        output = self.__class__.parse_multiple(*subitem_ids, subitems=True)
-        for subitem in output:
-            subitem.parent_item = self
-            subitem.category = self.category
-        return output
-
-    def parse(self, force=False, *args, **kwargs):
-        if not force and self._parsed:
-            return
-
-        self.__class__.parse_multiple(*[self.id_], *args, **kwargs)
-
-    @classmethod
-    def get(cls, id_, **kwargs):
-        if id_ in cls._cache:
-            output = cls._cache[id_]
-            if kwargs and not output.data:
-                output.data = kwargs
-        else:
-            output = cls(id_, direct=False, **kwargs)
-        cls._cache[id_] = output
-        return output
-
-    @property
-    def data(self):
-        return self._data
-
-    @data.setter
-    def data(self, value):
-        self.__dict__.update(value)
-        self._data = value
-
-
-class SubItem(Item):
-    def __init__(self, id_, **kwargs):
-        super().__init__(id_, **kwargs)
-        self.parent_item = None
-
-    @property
-    def subitems(self):
-        return []
-
-    @property
-    def subitem_ids(self):
-        return []
-
-    def parse(self, force=False, *args, **kwargs):
-        return super().parse(force=force, subitems=True, parse_subitems=False)
-
-
-if __name__ == '__main__':
-    item_ = Item.get(177849232)
-    item_.parse()
-    pass
+from functools import cached_property
+from typing import Dict, List, Collection
+
+from global_logger import Log
+
+from rozetka.tools import tools, constants
+
+LOG = Log.get_logger()
+
+
+class Item:
+    _cache = dict()  # type: Dict[int, Item]
+    _data: Dict = dict()
+
+    def __init__(self, id_, direct=True, **kwargs):
+        assert direct is False, f"You cannot use {self.__class__.__name__} directly. Please use get classmethod."
+        self.id_ = id_
+        assert isinstance(self.id_, int), f"{self.__class__.__name__} id must be an int"
+        self.category = None
+        self.data = kwargs
+
+        if (stars := self.__dict__.get('stars', None)) is not None:
+            if '%' in str(stars):
+                self.stars = int(stars.rstrip('%')) / 100
+
+        if (comments_mark := self.__dict__.get('comments_mark', None)) is not None:
+            self.comments_mark = float(comments_mark)
+
+        self._parsed = False
+
+    def __str__(self):
+        if title := self.__dict__.get('title'):
+            return f"({self.id_}) {title}"
+
+        return f"{self.id_}"
+
+    def __repr__(self):
+        return f"[{self.__class__.__name__}]{self.__str__()}"
+
+    def __iter__(self):
+        for subitem in self.subitems:
+            yield subitem
+            # yield from subitem.__iter__()  # prevent sub-subitems
+
+    @staticmethod
+    def _parse_batch(*product_ids, subitems=False, parse_subitems=True):
+        url = 'https://xl-catalog-api.rozetka.com.ua/v4/goods/getDetails'
+        params = {
+            'country': constants.COUNTRY,
+            'lang': constants.LANGUAGE,
+            'with_groups': 1,
+            'with_docket': 1,
+            'goods_group_href': 1,
+            'product_ids': ",".join(product_ids),
+        }
+
+        LOG.debug(f"Parsing batch of {len(product_ids)} products")
+        output = []
+        req = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
+        if req is None:
+            return output
+
+        try:
+            data: List[dict] = req.json().get('data')
+        except Exception as e:
+            pass
+        """
+        {
+            "id": 280528638,
+            "title": "Мобільний телефон Samsung Galaxy A32 4/128 GB Black",
+            "title_suffix": "",
+            "price": 10399,
+            "old_price": 10499,
+            "price_pcs": "281.05",
+            "href": "https://rozetka.com.ua/ua/samsung_galaxy_a32_4_128gb_black/p280528638/",
+            "status": "active",
+            "status_inherited": "active",
+            "sell_status": "available",
+            "category_id": 80003,
+            "seller_id": 5,
+            "merchant_id": 1,
+            "brand": "Samsung",
+            "brand_id": 12,
+            "group_id": 36310773,
+            "group_name": "36310773",
+            "group_title": "Мобільний телефон Samsung Galaxy A32 4/128GB",
+            "pl_bonus_charge_pcs": 0,
+            "pl_use_instant_bonus": 0,
+            "state": "new",
+            "docket": "Екран (6.4\", Super AMOLED, 2400x1080) / Mediatek Helio G80 (2 x 2.0 ГГц + 6 x 1.8 ГГц) / 
+            "mpath": ".4627949.80003.",
+            "is_group_primary": 1,
+            "dispatch": 1,
+            "premium": 0,
+            "preorder": 0,
+            "comments_amount": 109,
+            "comments_mark": 3.9,
+            "gift": null,
+            "tag": {
+                "name": "action",
+                "title": "Акция",
+                "priority": 9,
+                "goods_id": 280528638
+            },
+            "pictograms": [{
+                    "is_auction": true,
+                    "view_position": 1,
+                    "order": 49,
+                    "id": 30277,
+                    "goods_id": 280528638,
+                    "title": "ROZETKA Обмін",
+                    "image_url": "https://content2.rozetka.com.ua/goods_tags/images_ua/original/222408740.png",
+                    "view_type": "in_central_block",
+                    "announce": null,
+                    "has_description": 1,
+                    "description": null,
+                    "url": null,
+                    "url_title": null,
+                    "icon_mobile": ""
+                }
+            ],
+            "title_mode": null,
+            "use_group_links": null,
+            "is_need_street_id": false,
+            "image_main": "https://content1.rozetka.com.ua/goods/images/big_tile/175376690.jpg",
+            "images": {
+                "main": "https://content1.rozetka.com.ua/goods/images/big_tile/175376690.jpg",
+                "preview": "https://content1.rozetka.com.ua/goods/images/preview/175376690.jpg",
+                "hover": "https://content.rozetka.com.ua/goods/images/big_tile/175376700.jpg",
+                "all_images": ["https://content1.rozetka.com.ua/goods/images/original/175376690.jpg", 
+                                "https://content.rozetka.com.ua/goods/images/original/175376700.jpg", 
+                                "https://content2.rozetka.com.ua/goods/images/original/175376709.jpg", 
+                                "https://content1.rozetka.com.ua/goods/images/original/175376715.jpg", 
+                                "https://content1.rozetka.com.ua/goods/images/original/175376721.jpg", 
+                                "https://content1.rozetka.com.ua/goods/images/original/175376697.jpg", 
+                                "https://content1.rozetka.com.ua/goods/images/original/175376698.jpg", 
+                                "https://content.rozetka.com.ua/goods/images/original/175376694.jpg"]
+            },
+            "parent_category_id": 4627949,
+            "is_docket": true,
+            "primary_good_title": "Мобільний телефон Samsung Galaxy A32 4/128 GB Black",
+            "groups": {
+                "color": [{
+                        "value": "Black",
+                        "href": "https://rozetka.com.ua/ua/samsung_galaxy_a32_4_128gb_black/p280528638/",
+                        "rank": "99.9997",
+                        "id": 280528638,
+                        "is_group_primary": 1,
+                        "option_id": 21716,
+                        "option_name": "21716",
+                        "value_id": 6691,
+                        "color": {
+                            "id": 6691,
+                            "hash": "#000",
+                            "url": null
+                        },
+                        "active_option": true
+                    }, {
+                        "value": "Lavenda",
+                        "href": "https://rozetka.com.ua/ua/samsung_galaxy_a32_4_128gb_lavender/p280528633/",
+                        "rank": "99.9997",
+                        "id": 280528633,
+                        "is_group_primary": 0,
+                        "option_id": 21716,
+                        "option_name": "21716",
+                        "value_id": 1360088,
+                        "color": {
+                            "id": 1360088,
+                            "hash": "#000",
+                        "url": "https://content.rozetka.com.ua/goods_details_values/images/original/196717502.jpg"
+                        },
+                        "active_option": false
+                    }
+                ]
+            },
+            "stars": "78%",
+            "discount": 1,
+            "config": {
+                "title": true,
+                "brand": false,
+                "image": true,
+                "price": true,
+                "old_price": true,
+                "promo_price": true,
+                "status": true,
+                "bonus": true,
+                "gift": true,
+                "rating": true,
+                "wishlist_button": true,
+                "compare_button": true,
+                "buy_button": true,
+                "tags": true,
+                "pictograms": true,
+                "description": true,
+                "variables": true,
+                "hide_rating_review": false
+            }
+        }
+        """
+
+        for item_data in data:
+            id_ = item_data.get('id')
+            if not id_:
+                continue
+
+            item_data.pop('id')
+            if subitems:
+                item = SubItem.get(id_, **item_data)
+            else:
+                item = Item.get(id_, **item_data)
+            item._parsed = True
+            output.append(item)
+
+            if parse_subitems:
+                output.extend(item.subitems)
+        LOG.debug(f"Parsing batch of {len(product_ids)} products done. Got {len(output)} Items")
+        return output
+
+    @staticmethod
+    def parse_multiple(*product_ids, subitems=False, parse_subitems=True):
+        if not product_ids:
+            return []
+
+        if isinstance(product_ids[0], Item):
+            product_ids = [i.id_ for i in product_ids]
+        elif isinstance(product_ids[0], Collection):
+            product_ids = product_ids[0]
+
+        product_ids_str = [str(i) for i in product_ids]
+        chunk_size = 900
+        chunked_lists = tools.slice_list(product_ids_str, chunk_size)
+        LOG.debug(f"Parsing {len(product_ids)} products divided into {len(chunked_lists)} batches by {chunk_size} each")
+        outputs = tools.fnc_map(Item._parse_batch, *chunked_lists, subitems=subitems, parse_subitems=parse_subitems)
+        outputs = [i for i in outputs if i]
+        output = []
+        for list_ in outputs:
+            output.extend(list_)
+        return output
+
+    @cached_property
+    def subitem_ids(self):
+        groups = self._data.get('groups', {})
+        if not groups:
+            return []
+
+        for _, block in groups.items():
+            block_iterator = block if isinstance(block, list) else block.values()
+            for group in block_iterator:
+                if isinstance(group, list):
+                    subitem_iterator = group
+                elif isinstance(group, dict):
+                    subitem_iterator = [group]
+                else:
+                    continue
+
+                for subitem in subitem_iterator:
+                    if id_ := subitem.get('id'):
+                        if id_ == self.id_:
+                            continue
+
+                        yield id_
+
+    @cached_property
+    def subitems(self):
+        subitem_ids = list(set(self.subitem_ids))
+        if not subitem_ids:
+            return []
+
+        output = self.__class__.parse_multiple(*subitem_ids, subitems=True)
+        for subitem in output:
+            subitem.parent_item = self
+            subitem.category = self.category
+        return output
+
+    def parse(self, force=False, *args, **kwargs):
+        if not force and self._parsed:
+            return
+
+        self.__class__.parse_multiple(*[self.id_], *args, **kwargs)
+
+    @classmethod
+    def get(cls, id_, **kwargs):
+        if id_ in cls._cache:
+            output = cls._cache[id_]
+            if kwargs and not output.data:
+                output.data = kwargs
+        else:
+            output = cls(id_, direct=False, **kwargs)
+        cls._cache[id_] = output
+        return output
+
+    @property
+    def data(self):
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        self.__dict__.update(value)
+        self._data = value
+
+
+class SubItem(Item):
+    def __init__(self, id_, **kwargs):
+        super().__init__(id_, **kwargs)
+        self.parent_item = None
+
+    @property
+    def subitems(self):
+        return []
+
+    @property
+    def subitem_ids(self):
+        return []
+
+    def parse(self, force=False, *args, **kwargs):
+        return super().parse(force=force, subitems=True, parse_subitems=False)
+
+
+if __name__ == '__main__':
+    item_ = Item.get(177849232)
+    item_.parse()
+    pass
```

### Comparing `rozetka_api-1.1.3/rozetka/entities/supercategory.py` & `rozetka_api-1.1.4/rozetka/entities/supercategory.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-from itertools import chain
-from typing import List
-
-from global_logger import Log
-from requests import Response
-
-from rozetka.entities.category import Category
-from rozetka.entities.item import Item, SubItem
-from rozetka.tools import tools, constants
-
-LOG = Log.get_logger()
-
-
-def get_fat_menu_categories():
-    # noinspection PyProtectedMember
-    if SuperCategory._fat_menu_categories is not None:
-        # noinspection PyProtectedMember
-        return SuperCategory._fat_menu_categories
-
-    params = {
-        'front-type': 'xl',
-        'country': 'UA',
-        'lang': 'ua',
-    }
-    output = []
-    response = tools.get('https://common-api.rozetka.com.ua/v2/fat-menu/full', params=params,
-                         headers=constants.DEFAULT_HEADERS, retry=True)
-    if response is None:
-        return output
-
-    data: dict = response.json().get('data', dict())
-    for div in data.values():
-        children = div.get('children', dict())
-        # noinspection DuplicatedCode
-        if not children:
-            category_id = div.get('category_id')
-            if category_id is not None:
-                category_title = div.get('title')
-                category_url = div.get('manual_url')
-                category = Category.get(id_=category_id, title=category_title, url=category_url)
-                output.append(category)
-
-        for subchild in children.values():
-            for subsubchild in subchild:
-                subchildren = subsubchild.get('children', list())
-                # noinspection DuplicatedCode
-                if not subchildren:
-                    category_id = subsubchild.get('category_id')
-                    if category_id is not None:
-                        category_title = subsubchild.get('title')
-                        category_url = subsubchild.get('manual_url')
-                        category = Category.get(id_=category_id, title=category_title, url=category_url)
-                        output.append(category)
-
-                for subsubsubchild in subchildren:
-                    category_id = subsubsubchild.get('category_id')
-                    if category_id is not None:
-                        category_title = subsubsubchild.get('title')
-                        category_url = subsubsubchild.get('manual_url')
-                        category = Category.get(id_=category_id, title=category_title, url=category_url)
-                        output.append(category)
-
-    SuperCategory._fat_menu_categories = output = list(set(output))
-    return output
-
-
-def get_all_items_recursively() -> List[Item]:
-    categories = list(get_all_categories_recursively())
-    categories.sort(key=lambda _: _.id_)
-    LOG.green("Got ALL categories recursively")
-
-    all_categories = [_ for _ in categories for _ in _]
-    all_categories_len = len(all_categories)
-
-    LOG.green("Getting ALL items recursively")
-    # noinspection PyProtectedMember
-    items_ids = tools.fncs_map((_._get_item_ids for _ in all_categories)) or []
-    items_ids = list(set(chain(*items_ids)))
-    LOG.debug(f"Got {len(items_ids)} item ids from {all_categories_len} categories")
-    items = Item.parse_multiple(*items_ids, parse_subitems=False)
-    LOG.green(f"Got {len(items)} items from {all_categories_len} categories")
-
-    LOG.green("Getting subitem ids")
-    subitems_ids = list(set(list(chain(*[_.subitem_ids for _ in items]))))
-    LOG.debug(f"Got {len(subitems_ids)} subitem ids from {all_categories_len} categories")
-    subitems = Item.parse_multiple(*subitems_ids, subitems=True)
-    LOG.debug(f"Got {len(subitems)} subitems from {all_categories_len} categories")
-
-    # noinspection PyProtectedMember
-    all_items = items + subitems + list(Item._cache.values()) + list(SubItem._cache.values())
-    all_items = list(set(all_items))
-    LOG.green(f"Got {len(all_items)} total items from {all_categories_len} categories")
-    return all_items
-
-
-def get_super_categories():
-    """
-
-    :rtype: List[SuperCategory]
-    """
-    LOG.debug(f"Getting super categories")
-    output = []
-    for super_category_id in get_super_category_ids():
-        super_category = SuperCategory.get(id_=super_category_id)
-        output.append(super_category)
-    output.sort(key=lambda i: i.id_)
-    SuperCategory._super_categories = output
-    LOG.green(f"Got {len(output)} super categories")
-    # noinspection PyProtectedMember
-    return SuperCategory._super_categories
-
-
-def get_super_category_ids():
-    # noinspection PyProtectedMember
-    if SuperCategory._super_category_ids is None:
-        LOG.debug(f"Getting super category ids")
-        url = 'https://xl-catalog-api.rozetka.com.ua/v4/super-portals/getList'
-        response: Response = tools.get(url, headers=constants.DEFAULT_HEADERS, cookies=constants.DEFAULT_COOKIES,
-                                       retry=True)
-        if response is None or not response.ok:
-            msg = f'Error requesting "{url}": {response.status_code if response is not None else None} ' \
-                  f'{response.reason if response is not None else None}'
-            LOG.error(msg)
-            raise Exception(msg)
-
-        SuperCategory._super_category_ids = output = response.json().get('data', list())
-        # noinspection PyProtectedMember
-        SuperCategory._super_category_ids.sort()
-        LOG.debug(f"Got {len(output)} super category ids")
-    # noinspection PyProtectedMember
-    return SuperCategory._super_category_ids
-
-
-def get_all_categories_recursively():
-    LOG.green("Getting ALL categories recursively")
-    supercategories = list(get_super_categories() + get_fat_menu_categories())
-    # noinspection PyProtectedMember
-    cache = list(Category._cache.values())
-    # noinspection PyProtectedMember
-    supers_cache = list(SuperCategory._cache.values())
-    # noinspection PyTypeChecker
-    categories = supercategories + cache + supers_cache
-    categories = list(set(categories))
-    categories.sort(key=lambda i: i.id_)
-    for category in categories:
-        LOG.debug(f"get_all_categories_recursively: yielding {category}")
-        yield category
-        LOG.debug(f"get_all_categories_recursively: yielding from {category}")
-        yield from category.__iter__()
-
-
-class SuperCategory(Category):
-    _super_category_ids: List[int] = None
-    _super_categories = None  # type: List[SuperCategory]
-    _fat_menu_categories = None  # type: List[Category]
-
-    def __init__(self, id_, title=None, url=None, parent_category=None, parent_category_id=None, direct=True):
-        super().__init__(id_=id_, title=title, url=url, parent_category=parent_category,
-                         parent_category_id=parent_category_id, direct=direct)
-
-    @property
-    def data(self):
-        if self._data is None:
-            params = {
-                'category_id': self.id_,
-                'lang': constants.LANGUAGE,
-                'country': constants.COUNTRY,
-            }
-            url = 'https://xl-catalog-api.rozetka.com.ua/v4/super-portals/get'
-            response = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
-            if response is None:
-                return
-
-            self._data = response.json().get('data', dict()) or dict()
-        return self._data
-
-    @data.setter
-    def data(self, value):
-        self._data = value
-
-    @property
-    def subcategories_data(self):
-        if self._subcategories_data is None:
-            if not self.data:
-                return list()
-
-            blocks: list = self.data.get('blocks', list())
-            category_trees = list(filter(lambda i: i.get('type') == 'seo_category_tree', blocks))
-            if not category_trees:
-                return {}
-
-            category_tree: dict = category_trees[0]
-            content: dict = category_tree.get('content', dict())
-            self._subcategories_data = output = content.get('items', list())
-            LOG.debug(f"Got {len(output)} subcategories data for {self}")
-        return self._subcategories_data
-
-    @subcategories_data.setter
-    def subcategories_data(self, value):
-        self._subcategories_data = value
-
-    @property
-    def subcategories(self):
-        return self._get_subcategories('root_id')
-
-
-if __name__ == '__main__':
-    LOG.verbose = True
-    ac = list(get_all_categories_recursively())
-    # supercategory = SuperCategory.get(4627893)
-    # subs = supercategory.subcategories
-    # a = list(supercategory.__iter__())
-    # all_items_ = SuperCategory.get_all_items_recursively()
-    pass
+from itertools import chain
+from typing import List
+
+from global_logger import Log
+from requests import Response
+
+from rozetka.entities.category import Category
+from rozetka.entities.item import Item, SubItem
+from rozetka.tools import tools, constants
+
+LOG = Log.get_logger()
+
+
+def get_fat_menu_categories():
+    # noinspection PyProtectedMember
+    if SuperCategory._fat_menu_categories is not None:
+        # noinspection PyProtectedMember
+        return SuperCategory._fat_menu_categories
+
+    params = {
+        'front-type': 'xl',
+        'country': 'UA',
+        'lang': 'ua',
+    }
+    output = []
+    response = tools.get('https://common-api.rozetka.com.ua/v2/fat-menu/full', params=params,
+                         headers=constants.DEFAULT_HEADERS, retry=True)
+    if response is None:
+        return output
+
+    data: dict = response.json().get('data', dict())
+    for div in data.values():
+        children = div.get('children', dict())
+        # noinspection DuplicatedCode
+        if not children:
+            category_id = div.get('category_id')
+            if category_id is not None:
+                category_title = div.get('title')
+                category_url = div.get('manual_url')
+                category = Category.get(id_=category_id, title=category_title, url=category_url)
+                output.append(category)
+
+        for subchild in children.values():
+            for subsubchild in subchild:
+                subchildren = subsubchild.get('children', list())
+                # noinspection DuplicatedCode
+                if not subchildren:
+                    category_id = subsubchild.get('category_id')
+                    if category_id is not None:
+                        category_title = subsubchild.get('title')
+                        category_url = subsubchild.get('manual_url')
+                        category = Category.get(id_=category_id, title=category_title, url=category_url)
+                        output.append(category)
+
+                for subsubsubchild in subchildren:
+                    category_id = subsubsubchild.get('category_id')
+                    if category_id is not None:
+                        category_title = subsubsubchild.get('title')
+                        category_url = subsubsubchild.get('manual_url')
+                        category = Category.get(id_=category_id, title=category_title, url=category_url)
+                        output.append(category)
+
+    SuperCategory._fat_menu_categories = output = list(set(output))
+    return output
+
+
+def get_all_items_recursively() -> List[Item]:
+    categories = list(get_all_categories_recursively())
+    categories.sort(key=lambda _: _.id_)
+    LOG.green("Got ALL categories recursively")
+
+    all_categories = [_ for _ in categories for _ in _]
+    all_categories_len = len(all_categories)
+
+    LOG.green("Getting ALL items recursively")
+    # noinspection PyProtectedMember
+    items_ids = tools.fncs_map((_._get_item_ids for _ in all_categories)) or []
+    items_ids = list(set(chain(*items_ids)))
+    LOG.debug(f"Got {len(items_ids)} item ids from {all_categories_len} categories")
+    items = Item.parse_multiple(*items_ids, parse_subitems=False)
+    LOG.green(f"Got {len(items)} items from {all_categories_len} categories")
+
+    LOG.green("Getting subitem ids")
+    subitems_ids = list(set(list(chain(*[_.subitem_ids for _ in items]))))
+    LOG.debug(f"Got {len(subitems_ids)} subitem ids from {all_categories_len} categories")
+    subitems = Item.parse_multiple(*subitems_ids, subitems=True)
+    LOG.debug(f"Got {len(subitems)} subitems from {all_categories_len} categories")
+
+    # noinspection PyProtectedMember
+    all_items = items + subitems + list(Item._cache.values()) + list(SubItem._cache.values())
+    all_items = list(set(all_items))
+    LOG.green(f"Got {len(all_items)} total items from {all_categories_len} categories")
+    return all_items
+
+
+def get_super_categories():
+    """
+
+    :rtype: List[SuperCategory]
+    """
+    LOG.debug(f"Getting super categories")
+    output = []
+    for super_category_id in get_super_category_ids():
+        super_category = SuperCategory.get(id_=super_category_id)
+        output.append(super_category)
+    output.sort(key=lambda i: i.id_)
+    SuperCategory._super_categories = output
+    LOG.green(f"Got {len(output)} super categories")
+    # noinspection PyProtectedMember
+    return SuperCategory._super_categories
+
+
+def get_super_category_ids():
+    # noinspection PyProtectedMember
+    if SuperCategory._super_category_ids is None:
+        LOG.debug(f"Getting super category ids")
+        url = 'https://xl-catalog-api.rozetka.com.ua/v4/super-portals/getList'
+        response: Response = tools.get(url, headers=constants.DEFAULT_HEADERS, cookies=constants.DEFAULT_COOKIES,
+                                       retry=True)
+        if response is None or not response.ok:
+            msg = f'Error requesting "{url}": {response.status_code if response is not None else None} ' \
+                  f'{response.reason if response is not None else None}'
+            LOG.error(msg)
+            raise Exception(msg)
+
+        SuperCategory._super_category_ids = output = response.json().get('data', list())
+        # noinspection PyProtectedMember
+        SuperCategory._super_category_ids.sort()
+        LOG.debug(f"Got {len(output)} super category ids")
+    # noinspection PyProtectedMember
+    return SuperCategory._super_category_ids
+
+
+def get_all_categories_recursively():
+    LOG.green("Getting ALL categories recursively")
+    supercategories = list(get_super_categories() + get_fat_menu_categories())
+    # noinspection PyProtectedMember
+    cache = list(Category._cache.values())
+    # noinspection PyProtectedMember
+    supers_cache = list(SuperCategory._cache.values())
+    # noinspection PyTypeChecker
+    categories = supercategories + cache + supers_cache
+    categories = list(set(categories))
+    categories.sort(key=lambda i: i.id_)
+    for category in categories:
+        LOG.debug(f"get_all_categories_recursively: yielding {category}")
+        yield category
+        LOG.debug(f"get_all_categories_recursively: yielding from {category}")
+        yield from category.__iter__()
+
+
+class SuperCategory(Category):
+    _super_category_ids: List[int] = None
+    _super_categories = None  # type: List[SuperCategory]
+    _fat_menu_categories = None  # type: List[Category]
+
+    def __init__(self, id_, title=None, url=None, parent_category=None, parent_category_id=None, direct=True):
+        super().__init__(id_=id_, title=title, url=url, parent_category=parent_category,
+                         parent_category_id=parent_category_id, direct=direct)
+
+    @property
+    def data(self):
+        if self._data is None:
+            params = {
+                'category_id': self.id_,
+                'lang': constants.LANGUAGE,
+                'country': constants.COUNTRY,
+            }
+            url = 'https://xl-catalog-api.rozetka.com.ua/v4/super-portals/get'
+            response = tools.get(url, params=params, headers=constants.DEFAULT_HEADERS, retry=True)
+            if response is None:
+                return
+
+            self._data = response.json().get('data', dict()) or dict()
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        self._data = value
+
+    @property
+    def subcategories_data(self):
+        if self._subcategories_data is None:
+            if not self.data:
+                return list()
+
+            blocks: list = self.data.get('blocks', list())
+            category_trees = list(filter(lambda i: i.get('type') == 'seo_category_tree', blocks))
+            if not category_trees:
+                return {}
+
+            category_tree: dict = category_trees[0]
+            content: dict = category_tree.get('content', dict())
+            self._subcategories_data = output = content.get('items', list())
+            LOG.debug(f"Got {len(output)} subcategories data for {self}")
+        return self._subcategories_data
+
+    @subcategories_data.setter
+    def subcategories_data(self, value):
+        self._subcategories_data = value
+
+    @property
+    def subcategories(self):
+        return self._get_subcategories('root_id')
+
+
+if __name__ == '__main__':
+    LOG.verbose = True
+    ac = list(get_all_categories_recursively())
+    # supercategory = SuperCategory.get(4627893)
+    # subs = supercategory.subcategories
+    # a = list(supercategory.__iter__())
+    # all_items_ = SuperCategory.get_all_items_recursively()
+    pass
```

### Comparing `rozetka_api-1.1.3/rozetka/runners/parse_api.py` & `rozetka_api-1.1.4/rozetka/runners/parse_api.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import asyncio
-
-import pendulum
-import requests
-from global_logger import Log
-from knockknock import telegram_sender, discord_sender, slack_sender, teams_sender
-from progress.bar import Bar
-
-from rozetka.entities.item import Item
-from rozetka.entities.point import Point
-from rozetka.entities.supercategory import get_all_items_recursively
-from rozetka.tools import db, constants, tools
-
-LOG = Log.get_logger()
-
-setters = (
-    constants.Setter(fnc=Point.tag, flds=constants.TAGS),
-    constants.Setter(fnc=Point.field, flds=constants.FIELDS),
-)
-
-
-def build_item_point(item: Item):
-    # item.parse()
-    point = Point(constants.MEASUREMENT)
-    for setter in setters:
-        for fld in setter.flds:
-            if (item_fld := getattr(item, fld, None)) is not None:
-                fnc = getattr(point, setter.fnc.__name__)
-                point = fnc(fld, item_fld)
-    return point
-
-
-def _main():
-    try:
-        requests.get('https://xl-catalog-api.rozetka.com.ua/v4/super-portals/getList')
-    except Exception as e:
-        LOG.exception("Rozetka unavailable", exc_info=e)
-        raise Exception('healthcheck failure')
-
-    healthcheck = asyncio.run(db.health_test())
-    if not healthcheck:
-        LOG.error("InfluxDB inaccessible!")
-        raise Exception('healthcheck failure')
-
-    start = pendulum.now()
-    LOG.verbose = constants.VERBOSE
-
-    all_items = get_all_items_recursively()
-
-    LOG.green(f"Building points for {len(all_items)} items")
-    points = list(map(build_item_point, all_items))
-    LOG.green(f"Dumping {len(points)} points")
-    # https://docs.influxdata.com/influxdb/v2.4/write-data/best-practices/optimize-writes/
-    chunked_points = tools.slice_list(points, 5000)
-    for chunked_points_item in Bar(f"Dumping {len(chunked_points)} point chunks").iter(chunked_points):
-        asyncio.run(db.dump_points_async(record=chunked_points_item))
-
-    duration = pendulum.now().diff_for_humans(start)
-    LOG.green(f"Duration: {duration}")
-    return len(points)
-
-
-def main():
-    assert constants.INFLUXDB_URL and constants.INFLUXDB_TOKEN and constants.INFLUXDB_ORG \
-           and constants.INFLUXDB_BUCKET, "Please fill all INFLUXDB variables"
-
-    assert constants.CALLS_MAX, "Please fill the correct CALLS_MAX variable"
-    assert constants.CALLS_PERIOD, "Please fill the correct CALLS_PERIOD variable"
-
-    fnc = _main  # https://github.com/huggingface/knockknock
-    if (tg_token := constants.TELEGRAM_TOKEN) and (tg_chat := constants.TELEGRAM_CHAT_ID):
-        fnc = telegram_sender(token=tg_token, chat_id=int(tg_chat))(fnc)
-
-    if discord_webhook := constants.DISCORD_WEBHOOK_URL:
-        fnc = discord_sender(discord_webhook)(fnc)
-
-    if (slack_webhook := constants.SLACK_WEBHOOK_URL) and (slack_channel := constants.SLACK_CHANNEL):
-        if slack_user_mentions := constants.SLACK_USER_MENTIONS:
-            slack_user_mentions = slack_user_mentions.split()
-        fnc = slack_sender(slack_webhook, slack_channel, slack_user_mentions)(fnc)
-
-    if teams_webhook := constants.TEAMS_WEBHOOK_URL:
-        if teams_user_mentions := constants.TEAMS_USER_MENTIONS:
-            teams_user_mentions = teams_user_mentions.split()
-        fnc = teams_sender(teams_webhook, teams_user_mentions)(fnc)
-
-    fnc()
-
-
-if __name__ == '__main__':
-    main()
-    pass
+import asyncio
+
+import pendulum
+import requests
+from global_logger import Log
+from knockknock import telegram_sender, discord_sender, slack_sender, teams_sender
+from progress.bar import Bar
+
+from rozetka.entities.item import Item
+from rozetka.entities.point import Point
+from rozetka.entities.supercategory import get_all_items_recursively
+from rozetka.tools import db, constants, tools
+
+LOG = Log.get_logger()
+
+setters = (
+    constants.Setter(fnc=Point.tag, flds=constants.TAGS),
+    constants.Setter(fnc=Point.field, flds=constants.FIELDS),
+)
+
+
+def build_item_point(item: Item):
+    # item.parse()
+    point = Point(constants.MEASUREMENT)
+    for setter in setters:
+        for fld in setter.flds:
+            if (item_fld := getattr(item, fld, None)) is not None:
+                fnc = getattr(point, setter.fnc.__name__)
+                point = fnc(fld, item_fld)
+    return point
+
+
+def _main():
+    try:
+        requests.get('https://xl-catalog-api.rozetka.com.ua/v4/super-portals/getList')
+    except Exception as e:
+        LOG.exception("Rozetka unavailable", exc_info=e)
+        raise Exception('healthcheck failure')
+
+    healthcheck = asyncio.run(db.health_test())
+    if not healthcheck:
+        LOG.error("InfluxDB inaccessible!")
+        raise Exception('healthcheck failure')
+
+    start = pendulum.now()
+    LOG.verbose = constants.VERBOSE
+
+    all_items = get_all_items_recursively()
+
+    LOG.green(f"Building points for {len(all_items)} items")
+    points = list(map(build_item_point, all_items))
+    LOG.green(f"Dumping {len(points)} points")
+    # https://docs.influxdata.com/influxdb/v2.4/write-data/best-practices/optimize-writes/
+    chunked_points = tools.slice_list(points, 5000)
+    for chunked_points_item in Bar(f"Dumping {len(chunked_points)} point chunks").iter(chunked_points):
+        asyncio.run(db.dump_points_async(record=chunked_points_item))
+
+    duration = pendulum.now().diff_for_humans(start)
+    LOG.green(f"Duration: {duration}")
+    return len(points)
+
+
+def main():
+    assert constants.INFLUXDB_URL and constants.INFLUXDB_TOKEN and constants.INFLUXDB_ORG \
+           and constants.INFLUXDB_BUCKET, "Please fill all INFLUXDB variables"
+
+    assert constants.CALLS_MAX, "Please fill the correct CALLS_MAX variable"
+    assert constants.CALLS_PERIOD, "Please fill the correct CALLS_PERIOD variable"
+
+    fnc = _main  # https://github.com/huggingface/knockknock
+    if (tg_token := constants.TELEGRAM_TOKEN) and (tg_chat := constants.TELEGRAM_CHAT_ID):
+        fnc = telegram_sender(token=tg_token, chat_id=int(tg_chat))(fnc)
+
+    if discord_webhook := constants.DISCORD_WEBHOOK_URL:
+        fnc = discord_sender(discord_webhook)(fnc)
+
+    if (slack_webhook := constants.SLACK_WEBHOOK_URL) and (slack_channel := constants.SLACK_CHANNEL):
+        if slack_user_mentions := constants.SLACK_USER_MENTIONS:
+            slack_user_mentions = slack_user_mentions.split()
+        fnc = slack_sender(slack_webhook, slack_channel, slack_user_mentions)(fnc)
+
+    if teams_webhook := constants.TEAMS_WEBHOOK_URL:
+        if teams_user_mentions := constants.TEAMS_USER_MENTIONS:
+            teams_user_mentions = teams_user_mentions.split()
+        fnc = teams_sender(teams_webhook, teams_user_mentions)(fnc)
+
+    fnc()
+
+
+if __name__ == '__main__':
+    main()
+    pass
```

### Comparing `rozetka_api-1.1.3/rozetka/tools/constants.py` & `rozetka_api-1.1.4/rozetka/tools/constants.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import os
-from collections import namedtuple
-
-Setter = namedtuple('Setter', ['fnc', 'flds'])
-
-VERBOSE = os.getenv('VERBOSE') in ('True', '1', 'true')
-
-LANGUAGE = os.getenv('LANGUAGE', 'UA')
-assert LANGUAGE, "Please fill the correct LANGUAGE variable"
-
-COUNTRY = os.getenv('COUNTRY', 'UA')
-assert COUNTRY, "Please fill the correct COUNTRY variable"
-
-DEFAULT_USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:105.0) Gecko/20100101 Firefox/105.0'
-USER_AGENT = os.getenv('USER_AGENT', DEFAULT_USER_AGENT)
-assert USER_AGENT, "Please fill the correct USER_AGENT variable"
-
-DEFAULT_HEADERS = {
-    'User-Agent': USER_AGENT,
-}
-
-DEFAULT_COOKIES = {
-    'visitor_city': "1",
-}
-
-CALLS_MAX = os.getenv('CALLS_MAX', 1000)
-
-CALLS_PERIOD = os.getenv('CALLS_PERIOD', 5)
-
-INFLUXDB_URL = os.getenv('INFLUXDB_URL')
-INFLUXDB_TOKEN = os.getenv('INFLUXDB_TOKEN')
-INFLUXDB_ORG = os.getenv('INFLUXDB_ORG')
-INFLUXDB_BUCKET = os.getenv('INFLUXDB_BUCKET')
-
-TELEGRAM_TOKEN = os.getenv('TELEGRAM_TOKEN')
-TELEGRAM_CHAT_ID = os.getenv('TELEGRAM_CHAT_ID')
-
-DISCORD_WEBHOOK_URL = os.getenv('DISCORD_WEBHOOK_URL')
-
-SLACK_WEBHOOK_URL = os.getenv('SLACK_WEBHOOK_URL')
-SLACK_CHANNEL = os.getenv('SLACK_CHANNEL')
-SLACK_USER_MENTIONS = os.getenv('SLACK_USER_MENTIONS', '')
-
-TEAMS_WEBHOOK_URL = os.getenv('TEAMS_WEBHOOK_URL')
-TEAMS_USER_MENTIONS = os.getenv('TEAMS_USER_MENTIONS', '')
-
-MEASUREMENT = os.getenv('MEASUREMENT', 'goods')
-
-DEFAULT_TAGS = [
-    'id_',
-]
-TAGS = os.getenv('TAGS', DEFAULT_TAGS)
-if isinstance(TAGS, str):
-    TAGS = TAGS.split()
-
-DEFAULT_FIELDS = [
-    'price',
-    'old_price',
-    # 'stars',
-    'discount',
-    # 'comments_amount',
-    # 'comments_mark',
-]
-FIELDS = os.getenv('FIELDS', DEFAULT_FIELDS)
-if isinstance(FIELDS, str):
-    FIELDS = FIELDS.split()
+import os
+from collections import namedtuple
+
+Setter = namedtuple('Setter', ['fnc', 'flds'])
+
+VERBOSE = os.getenv('VERBOSE') in ('True', '1', 'true')
+
+LANGUAGE = os.getenv('LANGUAGE', 'UA')
+assert LANGUAGE, "Please fill the correct LANGUAGE variable"
+
+COUNTRY = os.getenv('COUNTRY', 'UA')
+assert COUNTRY, "Please fill the correct COUNTRY variable"
+
+DEFAULT_USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:105.0) Gecko/20100101 Firefox/105.0'
+USER_AGENT = os.getenv('USER_AGENT', DEFAULT_USER_AGENT)
+assert USER_AGENT, "Please fill the correct USER_AGENT variable"
+
+DEFAULT_HEADERS = {
+    'User-Agent': USER_AGENT,
+}
+
+DEFAULT_COOKIES = {
+    'visitor_city': "1",
+}
+
+CALLS_MAX = os.getenv('CALLS_MAX', 1000)
+
+CALLS_PERIOD = os.getenv('CALLS_PERIOD', 5)
+
+INFLUXDB_URL = os.getenv('INFLUXDB_URL')
+INFLUXDB_TOKEN = os.getenv('INFLUXDB_TOKEN')
+INFLUXDB_ORG = os.getenv('INFLUXDB_ORG')
+INFLUXDB_BUCKET = os.getenv('INFLUXDB_BUCKET')
+
+TELEGRAM_TOKEN = os.getenv('TELEGRAM_TOKEN')
+TELEGRAM_CHAT_ID = os.getenv('TELEGRAM_CHAT_ID')
+
+DISCORD_WEBHOOK_URL = os.getenv('DISCORD_WEBHOOK_URL')
+
+SLACK_WEBHOOK_URL = os.getenv('SLACK_WEBHOOK_URL')
+SLACK_CHANNEL = os.getenv('SLACK_CHANNEL')
+SLACK_USER_MENTIONS = os.getenv('SLACK_USER_MENTIONS', '')
+
+TEAMS_WEBHOOK_URL = os.getenv('TEAMS_WEBHOOK_URL')
+TEAMS_USER_MENTIONS = os.getenv('TEAMS_USER_MENTIONS', '')
+
+MEASUREMENT = os.getenv('MEASUREMENT', 'goods')
+
+DEFAULT_TAGS = [
+    'id_',
+]
+TAGS = os.getenv('TAGS', DEFAULT_TAGS)
+if isinstance(TAGS, str):
+    TAGS = TAGS.split()
+
+DEFAULT_FIELDS = [
+    'price',
+    'old_price',
+    # 'stars',
+    'discount',
+    # 'comments_amount',
+    # 'comments_mark',
+]
+FIELDS = os.getenv('FIELDS', DEFAULT_FIELDS)
+if isinstance(FIELDS, str):
+    FIELDS = FIELDS.split()
```

### Comparing `rozetka_api-1.1.3/rozetka/tools/db.py` & `rozetka_api-1.1.4/rozetka/tools/db.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import asyncio
-from copy import copy
-import datetime
-
-import pendulum
-from aiohttp_retry import ExponentialRetry, RetryClient
-from global_logger import Log
-# https://github.com/influxdata/influxdb-client-python
-from influxdb_client import InfluxDBClient, Bucket, BucketRetentionRules
-from influxdb_client.client.flux_table import FluxRecord
-from influxdb_client.client.influxdb_client_async import InfluxDBClientAsync
-
-from rozetka.entities.point import Point
-from rozetka.tools import constants
-
-log = Log.get_logger()
-
-INFLUXDB_URL = constants.INFLUXDB_URL
-INFLUXDB_TOKEN = constants.INFLUXDB_TOKEN
-INFLUXDB_ORG = constants.INFLUXDB_ORG
-INFLUXDB_BUCKET = constants.INFLUXDB_BUCKET
-
-INFLUX_KWARGS = dict(url=INFLUXDB_URL, token=INFLUXDB_TOKEN, org=INFLUXDB_ORG, timeout=600_000_000, enable_gzip=True)
-INFLUX_KWARGS_ASYNC = copy(INFLUX_KWARGS)
-INFLUX_KWARGS_ASYNC.update(dict(client_session_type=RetryClient,
-                                client_session_kwargs={"retry_options": ExponentialRetry(attempts=3)}))
-
-
-def dump_points(record=None, *args, **kwargs):
-    if not record:
-        return
-
-    with InfluxDBClient(**INFLUX_KWARGS) as client:
-        ready = client.ping()
-        # log.green(f"InfluxDB Ready: {ready}")
-        if not ready:
-            log.error(f"InfluxDB NOT READY")
-            return
-
-        write_api = client.write_api()
-        success = write_api.write(bucket=INFLUXDB_BUCKET, *args, **kwargs)
-        if success is False:
-            log.error(f"Error dumping points")
-        return success
-
-
-async def dump_points_async(*args, **kwargs):
-    async with InfluxDBClientAsync(**INFLUX_KWARGS_ASYNC) as client:
-        ready = await client.ping()
-        if not ready:
-            log.error(f"InfluxDB NOT READY")
-            return
-
-        write_api = client.write_api()
-        success = await write_api.write(bucket=INFLUXDB_BUCKET, *args, **kwargs)
-        if not success:
-            log.error(f"dump_points_async failure")
-            raise Exception('dump_points_async failure')
-
-        # query_api = client.query_api()
-        # records = await query_api.query_stream(f'from(bucket:"{INFLUXDB_BUCKET}") '
-        #                                        '|> range(start: -5s) ')
-        #                                        # f'|> filter(fn: (r) => r["_measurement"] == "{MEASUREMENT}")')
-        # async for record in records:
-        #     log.debug(record)
-
-        # log.debug(f"Dumping points success")
-        return success
-
-
-def empty_bucket(bucket_name=INFLUXDB_BUCKET):
-    with InfluxDBClient(**INFLUX_KWARGS) as client:
-        ready = client.ping()
-        # log.green(f"InfluxDB Ready: {ready}")
-        if not ready:
-            log.error(f"InfluxDB NOT READY")
-            return
-
-        delete_api = client.delete_api()
-        start = "1970-01-01T00:00:00Z"
-        stop = "2052-07-18T09:00:10.000Z"
-        delete_api.delete(start, stop, '', bucket=bucket_name, org=INFLUXDB_ORG)
-
-
-def recreate_bucket(bucket_name=INFLUXDB_BUCKET):
-    with InfluxDBClient(**INFLUX_KWARGS) as client:
-        ready = client.ping()
-        # log.green(f"InfluxDB Ready: {ready}")
-        if not ready:
-            log.error(f"InfluxDB NOT READY")
-            return
-
-        buckets_api = client.buckets_api()
-        bucket: Bucket = buckets_api.find_bucket_by_name(bucket_name=bucket_name)
-        if bucket:
-            seconds = pendulum.duration(hours=1).in_seconds()
-            bucket.retention_rules = [BucketRetentionRules(type="expire", shard_group_duration_seconds=seconds,
-                                                           every_seconds=seconds)]
-            bucket.name = f"{bucket.name}_old_{pendulum.now().timestamp()}"
-            buckets_api.update_bucket(bucket)
-        # result_delete = buckets_api.delete_bucket(bucket)
-        # bucket = Bucket(name=bucket_name, retention_rules=retention_rules)
-        retention_rules = BucketRetentionRules(type="expire", every_seconds=0)
-        result_create = buckets_api.create_bucket(bucket_name=bucket_name, retention_rules=retention_rules,
-                                                  org=INFLUXDB_ORG)
-        pass
-
-
-async def tst_write():
-    points = [Point('goods').tag('id_', '0').field('price', 0)]
-    return await dump_points_async(record=points)
-
-
-async def health_test():
-    async with InfluxDBClientAsync(**INFLUX_KWARGS_ASYNC) as client:
-        ready = await client.ping()
-        return ready
-
-
-if __name__ == "__main__":
-    # asyncio.run(empty_bucket(INFLUXDB_BUCKET))
-    # recreate_bucket(INFLUXDB_BUCKET)
-    # asyncio.run(tst_write())
-    pass
+import asyncio
+from copy import copy
+import datetime
+
+import pendulum
+from aiohttp_retry import ExponentialRetry, RetryClient
+from global_logger import Log
+# https://github.com/influxdata/influxdb-client-python
+from influxdb_client import InfluxDBClient, Bucket, BucketRetentionRules
+from influxdb_client.client.flux_table import FluxRecord
+from influxdb_client.client.influxdb_client_async import InfluxDBClientAsync
+
+from rozetka.entities.point import Point
+from rozetka.tools import constants
+
+log = Log.get_logger()
+
+INFLUXDB_URL = constants.INFLUXDB_URL
+INFLUXDB_TOKEN = constants.INFLUXDB_TOKEN
+INFLUXDB_ORG = constants.INFLUXDB_ORG
+INFLUXDB_BUCKET = constants.INFLUXDB_BUCKET
+
+INFLUX_KWARGS = dict(url=INFLUXDB_URL, token=INFLUXDB_TOKEN, org=INFLUXDB_ORG, timeout=600_000_000, enable_gzip=True)
+INFLUX_KWARGS_ASYNC = copy(INFLUX_KWARGS)
+INFLUX_KWARGS_ASYNC.update(dict(client_session_type=RetryClient,
+                                client_session_kwargs={"retry_options": ExponentialRetry(attempts=3)}))
+
+
+def dump_points(record=None, *args, **kwargs):
+    if not record:
+        return
+
+    with InfluxDBClient(**INFLUX_KWARGS) as client:
+        ready = client.ping()
+        # log.green(f"InfluxDB Ready: {ready}")
+        if not ready:
+            log.error(f"InfluxDB NOT READY")
+            return
+
+        write_api = client.write_api()
+        success = write_api.write(bucket=INFLUXDB_BUCKET, *args, **kwargs)
+        if success is False:
+            log.error(f"Error dumping points")
+        return success
+
+
+async def dump_points_async(*args, **kwargs):
+    async with InfluxDBClientAsync(**INFLUX_KWARGS_ASYNC) as client:
+        ready = await client.ping()
+        if not ready:
+            log.error(f"InfluxDB NOT READY")
+            return
+
+        write_api = client.write_api()
+        success = await write_api.write(bucket=INFLUXDB_BUCKET, *args, **kwargs)
+        if not success:
+            log.error(f"dump_points_async failure")
+            raise Exception('dump_points_async failure')
+
+        # query_api = client.query_api()
+        # records = await query_api.query_stream(f'from(bucket:"{INFLUXDB_BUCKET}") '
+        #                                        '|> range(start: -5s) ')
+        #                                        # f'|> filter(fn: (r) => r["_measurement"] == "{MEASUREMENT}")')
+        # async for record in records:
+        #     log.debug(record)
+
+        # log.debug(f"Dumping points success")
+        return success
+
+
+def empty_bucket(bucket_name=INFLUXDB_BUCKET):
+    with InfluxDBClient(**INFLUX_KWARGS) as client:
+        ready = client.ping()
+        # log.green(f"InfluxDB Ready: {ready}")
+        if not ready:
+            log.error(f"InfluxDB NOT READY")
+            return
+
+        delete_api = client.delete_api()
+        start = "1970-01-01T00:00:00Z"
+        stop = "2052-07-18T09:00:10.000Z"
+        delete_api.delete(start, stop, '', bucket=bucket_name, org=INFLUXDB_ORG)
+
+
+def recreate_bucket(bucket_name=INFLUXDB_BUCKET):
+    with InfluxDBClient(**INFLUX_KWARGS) as client:
+        ready = client.ping()
+        # log.green(f"InfluxDB Ready: {ready}")
+        if not ready:
+            log.error(f"InfluxDB NOT READY")
+            return
+
+        buckets_api = client.buckets_api()
+        bucket: Bucket = buckets_api.find_bucket_by_name(bucket_name=bucket_name)
+        if bucket:
+            seconds = pendulum.duration(hours=1).in_seconds()
+            bucket.retention_rules = [BucketRetentionRules(type="expire", shard_group_duration_seconds=seconds,
+                                                           every_seconds=seconds)]
+            bucket.name = f"{bucket.name}_old_{pendulum.now().timestamp()}"
+            buckets_api.update_bucket(bucket)
+        # result_delete = buckets_api.delete_bucket(bucket)
+        # bucket = Bucket(name=bucket_name, retention_rules=retention_rules)
+        retention_rules = BucketRetentionRules(type="expire", every_seconds=0)
+        result_create = buckets_api.create_bucket(bucket_name=bucket_name, retention_rules=retention_rules,
+                                                  org=INFLUXDB_ORG)
+        pass
+
+
+async def tst_write():
+    points = [Point('goods').tag('id_', '0').field('price', 0)]
+    return await dump_points_async(record=points)
+
+
+async def health_test():
+    async with InfluxDBClientAsync(**INFLUX_KWARGS_ASYNC) as client:
+        ready = await client.ping()
+        return ready
+
+
+if __name__ == "__main__":
+    # asyncio.run(empty_bucket(INFLUXDB_BUCKET))
+    # recreate_bucket(INFLUXDB_BUCKET)
+    # asyncio.run(tst_write())
+    pass
```

### Comparing `rozetka_api-1.1.3/PKG-INFO` & `rozetka_api-1.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: rozetka-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: Rozetka Python API
+Home-page: https://github.com/ALERTua/rozetka_api
 Keywords: rozetka
 Author: Alexey ALERT Rubasheff
 Author-email: alexey.rubasheff@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,7 +30,15 @@
 Examples
 ^^^^^^^^
 
 rozetka/examples/example_item.py
 
 rozetka/examples/example_category.py
 
+Github
+^^^^^^^^
+https://github.com/ALERTua/rozetka_api
+
+PyPi
+^^^^^^^^
+https://pypi.org/project/rozetka-api/
+
```

