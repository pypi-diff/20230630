# Comparing `tmp/rozetka-api-1.0.1.tar.gz` & `tmp/rozetka_api-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rozetka-api-1.0.1.tar", max compression
+gzip compressed data, was "rozetka_api-1.1.tar", max compression
```

## Comparing `rozetka-api-1.0.1.tar` & `rozetka_api-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      135 2022-09-21 12:38:31.895645 rozetka-api-1.0.1/README.rst
--rw-r--r--   0        0        0      938 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/entities/__init__.py
--rw-r--r--   0        0        0    10266 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/entities/category.py
--rw-r--r--   0        0        0    11588 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/entities/item.py
--rw-r--r--   0        0        0      535 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/entities/point.py
--rw-r--r--   0        0        0     8274 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/entities/supercategory.py
--rw-r--r--   0        0        0      770 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/examples/example_category.py
--rw-r--r--   0        0        0      103 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/examples/example_item.py
--rw-r--r--   0        0        0     3447 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/runners/parse_api.py
--rw-r--r--   0        0        0        0 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/tools/__init__.py
--rw-r--r--   0        0        0     1906 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/tools/constants.py
--rw-r--r--   0        0        0     4719 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/tools/db.py
--rw-r--r--   0        0        0     3440 2022-09-21 12:38:31.899645 rozetka-api-1.0.1/rozetka/tools/tools.py
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rozetka-api-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-06-30 11:23:33.743234 rozetka_api-1.1/pyproject.toml
+-rw-r--r--   0        0        0      135 2022-09-03 20:53:08.178729 rozetka_api-1.1/README.rst
+-rw-r--r--   0        0        0        0 2022-09-02 18:14:26.482651 rozetka_api-1.1/rozetka/entities/__init__.py
+-rw-r--r--   0        0        0    10557 2022-09-11 14:55:35.661756 rozetka_api-1.1/rozetka/entities/category.py
+-rw-r--r--   0        0        0    11903 2022-09-21 11:51:31.522568 rozetka_api-1.1/rozetka/entities/item.py
+-rw-r--r--   0        0        0      555 2022-09-21 11:51:31.500532 rozetka_api-1.1/rozetka/entities/point.py
+-rw-r--r--   0        0        0     8485 2022-10-09 10:10:02.078055 rozetka_api-1.1/rozetka/entities/supercategory.py
+-rw-r--r--   0        0        0      821 2022-09-03 11:44:07.607811 rozetka_api-1.1/rozetka/examples/example_category.py
+-rw-r--r--   0        0        0      108 2022-09-03 10:56:00.803564 rozetka_api-1.1/rozetka/examples/example_item.py
+-rw-r--r--   0        0        0     3390 2023-06-30 11:40:23.368017 rozetka_api-1.1/rozetka/runners/parse_api.py
+-rw-r--r--   0        0        0        0 2022-08-30 10:55:06.318671 rozetka_api-1.1/rozetka/tools/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-30 11:00:39.652176 rozetka_api-1.1/rozetka/tools/constants.py
+-rw-r--r--   0        0        0     6494 2023-06-30 11:16:50.860136 rozetka_api-1.1/rozetka/tools/db.py
+-rw-r--r--   0        0        0     3582 2022-09-21 11:51:31.483488 rozetka_api-1.1/rozetka/tools/tools.py
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 rozetka_api-1.1/PKG-INFO
```

### Comparing `rozetka-api-1.0.1/pyproject.toml` & `rozetka_api-1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-[tool.poetry]
-name = "rozetka-api"
-version = "1.0.1"
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
+version = "1.1"
+description = "Rozetka Python API"
+authors = ["Alexey ALERT Rubasheff <alexey.rubasheff@gmail.com>"]
+readme = "README.rst"
+packages = [{include = "rozetka"}]
+keywords = ["rozetka"]
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
+
+[tool.poetry.build]
+generate-setup-file = false
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

### Comparing `rozetka-api-1.0.1/rozetka/entities/category.py` & `rozetka_api-1.1/rozetka/entities/category.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,291 +1,291 @@
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
-            self._data = response.json().get('data', dict()) or dict()
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
-        if response.status_code != 200:
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
-
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
+            self._data = response.json().get('data', dict()) or dict()
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
+        if response.status_code != 200:
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
+
```

### Comparing `rozetka-api-1.0.1/rozetka/entities/supercategory.py` & `rozetka_api-1.1/rozetka/entities/supercategory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,205 +1,205 @@
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
-    response = tools.get('https://common-api.rozetka.com.ua/v2/fat-menu/full', params=params,
-                         headers=constants.DEFAULT_HEADERS, retry=True)
-    output = []
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
-    LOG.green("Got ALL categories recursively")
-
-    LOG.green("Getting ALL items recursively")
-    # noinspection PyProtectedMember
-    items_ids = tools.fncs_map((cat._get_item_ids for cat in categories))
-    items_ids = list(set(chain(*items_ids)))
-    LOG.debug(f"Got {len(items_ids)} item ids from {len(categories)} categories")
-    items = Item.parse_multiple(*items_ids, parse_subitems=False)
-    LOG.green(f"Got {len(items)} items from {len(categories)} categories")
-
-    LOG.green("Getting subitem ids")
-    subitems_ids = list(set(list(chain(*[i.subitem_ids for i in items]))))
-    LOG.debug(f"Got {len(subitems_ids)} subitem ids from {len(categories)} categories")
-    subitems = Item.parse_multiple(*subitems_ids, subitems=True)
-    LOG.debug(f"Got {len(subitems)} subitems from {len(categories)} categories")
-
-    # noinspection PyProtectedMember
-    all_items = items + subitems + list(Item._cache.values()) + list(SubItem._cache.values())
-    all_items = list(set(all_items))
-    LOG.green(f"Got {len(all_items)} total items from {len(categories)} categories")
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
-        if not response.ok:
-            msg = f'Error requesting "{url}": {response.status_code} {response.reason}'
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
-    supercategory = SuperCategory.get(1162030)
-    subs = supercategory.subcategories
-    a = list(supercategory.__iter__())
-    # get_super_category_ids = SuperCategory.get_super_category_ids()
-    # get_super_categories = SuperCategory.get_super_categories()
-    # get_all_categories_recursively = list(SuperCategory.get_all_categories_recursively())
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
+    response = tools.get('https://common-api.rozetka.com.ua/v2/fat-menu/full', params=params,
+                         headers=constants.DEFAULT_HEADERS, retry=True)
+    output = []
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
+    LOG.green("Got ALL categories recursively")
+
+    LOG.green("Getting ALL items recursively")
+    # noinspection PyProtectedMember
+    items_ids = tools.fncs_map((cat._get_item_ids for cat in categories)) or []
+    items_ids = list(set(chain(*items_ids)))
+    LOG.debug(f"Got {len(items_ids)} item ids from {len(categories)} categories")
+    items = Item.parse_multiple(*items_ids, parse_subitems=False)
+    LOG.green(f"Got {len(items)} items from {len(categories)} categories")
+
+    LOG.green("Getting subitem ids")
+    subitems_ids = list(set(list(chain(*[i.subitem_ids for i in items]))))
+    LOG.debug(f"Got {len(subitems_ids)} subitem ids from {len(categories)} categories")
+    subitems = Item.parse_multiple(*subitems_ids, subitems=True)
+    LOG.debug(f"Got {len(subitems)} subitems from {len(categories)} categories")
+
+    # noinspection PyProtectedMember
+    all_items = items + subitems + list(Item._cache.values()) + list(SubItem._cache.values())
+    all_items = list(set(all_items))
+    LOG.green(f"Got {len(all_items)} total items from {len(categories)} categories")
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
+        if not response.ok:
+            msg = f'Error requesting "{url}": {response.status_code} {response.reason}'
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
+    supercategory = SuperCategory.get(1162030)
+    subs = supercategory.subcategories
+    a = list(supercategory.__iter__())
+    # get_super_category_ids = SuperCategory.get_super_category_ids()
+    # get_super_categories = SuperCategory.get_super_categories()
+    # get_all_categories_recursively = list(SuperCategory.get_all_categories_recursively())
+    # all_items_ = SuperCategory.get_all_items_recursively()
+    pass
```

### Comparing `rozetka-api-1.0.1/rozetka/tools/tools.py` & `rozetka_api-1.1/rozetka/tools/tools.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import re
-import time
-from itertools import zip_longest
-
-import requests
-from global_logger import Log
-from ratelimit import limits, sleep_and_retry
-from requests import Response
-# noinspection PyPackageRequirements
-from worker import worker
-
-from rozetka.tools import constants
-
-LOG = Log.get_logger()
-
-
-def title_clean(title):
-    """
-    Cleans
-    Ноутбуки - ROZETKA | Купити ноутбук в Києві: ціна, відгуки, продаж, вибір ноутбуків в Україні'
-    to
-    Ноутбуки
-    """
-    if not title:
-        return ''
-
-    tails = [
-        ' - ROZETKA',
-        ' – в інтернет-магазині ROZETKA',
-    ]
-    output = title
-    for tail in tails:
-        split = re.split(tail, output)
-        # noinspection PyUnresolvedReferences
-        output = split[0].strip()
-    return output
-
-
-def ints_from_str(str_):
-    blocks = str_.split()
-    output = []
-    for block in blocks:
-        # noinspection PyBroadException
-        try:
-            output.append(int(block))
-        except:  # noqa: E722
-            pass
-
-    return output
-
-
-def floats_from_str(str_):
-    blocks = str_.split()
-    floats = []
-    for block in blocks:
-        # noinspection PyBroadException
-        try:
-            floats.append(float(block))
-        except:  # noqa: E722
-            pass
-
-    return floats
-
-
-def str_to_price(price_str):
-    if not price_str:
-        return
-
-    price_str = price_str.replace("₴", "")
-    price_str = price_str.split()
-    price_str = "".join(price_str)
-    return int(price_str)
-
-
-def parse_rating(rating_str):
-    if not rating_str:
-        return
-
-    floats = floats_from_str(rating_str)
-    if len(floats) == 2:
-        rating_value, rating_max = floats
-        return rating_value / rating_max
-
-
-def parse_reviews(reviews_str):
-    if not reviews_str:
-        return
-
-    floats = floats_from_str(reviews_str)
-    if floats:
-        return int(floats[0])
-
-
-@sleep_and_retry
-@limits(calls=constants.CALLS_MAX, period=constants.CALLS_PERIOD)
-def get(*args, retry=False, max_tries=3, delay=30, **kwargs) -> Response:
-    response = requests.get(*args, timeout=60, **kwargs)
-    if retry:
-        i = 0
-        while not response.ok and response.status_code in (502, ) and (i := i + 1) < max_tries:
-            LOG.error(f"ERROR Requesting {response.request.url} : {response.status_code}. Retrying in {delay}")
-            time.sleep(delay)
-            response = requests.get(*args, **kwargs)
-    return response
-
-
-def fnc_map(fnc, *tuple_of_args, **kwargs):
-    @worker
-    def _worker(*worker_args, **worker_kwargs):
-        return fnc(*worker_args, **worker_kwargs)
-
-    workers = []
-    for tuple_ in tuple_of_args:
-        workers.append(_worker(*tuple_, **kwargs))
-
-    outputs = []
-    for worker_ in workers:
-        worker_.wait()
-        outputs.append(worker_.ret)
-    return outputs
-
-
-def fncs_map(tuple_of_fncs, *tuple_of_args):
-    workers = []
-    for fnc, fnc_args in zip_longest(tuple_of_fncs, tuple_of_args):
-        @worker
-        def _worker(*worker_args):
-            return fnc(*worker_args)
-
-        fnc_args = fnc_args or []
-        workers.append(_worker(*fnc_args))
-
-    outputs = []
-    for worker_ in workers:
-        worker_.wait()
-        outputs.append(worker_.ret)
-    return outputs
-
-
-def slice_list(list_, chunk_size):
-    return [list_[i:i + chunk_size] for i in range(0, len(list_), chunk_size)]
-
+import re
+import time
+from itertools import zip_longest
+
+import requests
+from global_logger import Log
+from ratelimit import limits, sleep_and_retry
+from requests import Response
+# noinspection PyPackageRequirements
+from worker import worker
+
+from rozetka.tools import constants
+
+LOG = Log.get_logger()
+
+
+def title_clean(title):
+    """
+    Cleans
+    Ноутбуки - ROZETKA | Купити ноутбук в Києві: ціна, відгуки, продаж, вибір ноутбуків в Україні'
+    to
+    Ноутбуки
+    """
+    if not title:
+        return ''
+
+    tails = [
+        ' - ROZETKA',
+        ' – в інтернет-магазині ROZETKA',
+    ]
+    output = title
+    for tail in tails:
+        split = re.split(tail, output)
+        # noinspection PyUnresolvedReferences
+        output = split[0].strip()
+    return output
+
+
+def ints_from_str(str_):
+    blocks = str_.split()
+    output = []
+    for block in blocks:
+        # noinspection PyBroadException
+        try:
+            output.append(int(block))
+        except:  # noqa: E722
+            pass
+
+    return output
+
+
+def floats_from_str(str_):
+    blocks = str_.split()
+    floats = []
+    for block in blocks:
+        # noinspection PyBroadException
+        try:
+            floats.append(float(block))
+        except:  # noqa: E722
+            pass
+
+    return floats
+
+
+def str_to_price(price_str):
+    if not price_str:
+        return
+
+    price_str = price_str.replace("₴", "")
+    price_str = price_str.split()
+    price_str = "".join(price_str)
+    return int(price_str)
+
+
+def parse_rating(rating_str):
+    if not rating_str:
+        return
+
+    floats = floats_from_str(rating_str)
+    if len(floats) == 2:
+        rating_value, rating_max = floats
+        return rating_value / rating_max
+
+
+def parse_reviews(reviews_str):
+    if not reviews_str:
+        return
+
+    floats = floats_from_str(reviews_str)
+    if floats:
+        return int(floats[0])
+
+
+@sleep_and_retry
+@limits(calls=constants.CALLS_MAX, period=constants.CALLS_PERIOD)
+def get(*args, retry=False, max_tries=3, delay=30, **kwargs) -> Response:
+    response = requests.get(*args, timeout=60, **kwargs)
+    if retry:
+        i = 0
+        while not response.ok and response.status_code in (502, ) and (i := i + 1) < max_tries:
+            LOG.error(f"ERROR Requesting {response.request.url} : {response.status_code}. Retrying in {delay}")
+            time.sleep(delay)
+            response = requests.get(*args, **kwargs)
+    return response
+
+
+def fnc_map(fnc, *tuple_of_args, **kwargs):
+    @worker
+    def _worker(*worker_args, **worker_kwargs):
+        return fnc(*worker_args, **worker_kwargs)
+
+    workers = []
+    for tuple_ in tuple_of_args:
+        workers.append(_worker(*tuple_, **kwargs))
+
+    outputs = []
+    for worker_ in workers:
+        worker_.wait()
+        outputs.append(worker_.ret)
+    return outputs
+
+
+def fncs_map(tuple_of_fncs, *tuple_of_args):
+    workers = []
+    for fnc, fnc_args in zip_longest(tuple_of_fncs, tuple_of_args):
+        @worker
+        def _worker(*worker_args):
+            return fnc(*worker_args)
+
+        fnc_args = fnc_args or []
+        workers.append(_worker(*fnc_args))
+
+    outputs = []
+    for worker_ in workers:
+        worker_.wait()
+        outputs.append(worker_.ret)
+    return outputs
+
+
+def slice_list(list_, chunk_size):
+    return [list_[i:i + chunk_size] for i in range(0, len(list_), chunk_size)]
+
```

### Comparing `rozetka-api-1.0.1/PKG-INFO` & `rozetka_api-1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: rozetka-api
-Version: 1.0.1
+Version: 1.1
 Summary: Rozetka Python API
 Keywords: rozetka
 Author: Alexey ALERT Rubasheff
 Author-email: alexey.rubasheff@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp-retry (>=2.8.3,<3.0.0)
 Requires-Dist: global-logger (>=0.3.30,<0.4.0)
 Requires-Dist: influxdb[async] (>=5.3.1,<6.0.0)
 Requires-Dist: knockknock (>=0.1.8.1,<0.2.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
```

