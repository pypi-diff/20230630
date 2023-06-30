# Comparing `tmp/asyncio-oss-1.1.0.tar.gz` & `tmp/asyncio-oss-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-oss-1.1.0.tar", last modified: Mon Jun 26 18:04:00 2023, max compression
+gzip compressed data, was "asyncio-oss-1.1.1.tar", last modified: Fri Jun 30 16:08:50 2023, max compression
```

## Comparing `asyncio-oss-1.1.0.tar` & `asyncio-oss-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.209848 asyncio-oss-1.1.0/
--rw-r--r--   0 longyao    (501) staff       (20)     1064 2023-05-24 15:02:54.000000 asyncio-oss-1.1.0/LICENSE
--rw-r--r--   0 longyao    (501) staff       (20)     2944 2023-06-26 18:04:00.209755 asyncio-oss-1.1.0/PKG-INFO
--rw-r--r--   0 longyao    (501) staff       (20)     2598 2023-06-26 18:02:55.000000 asyncio-oss-1.1.0/README.md
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.208317 asyncio-oss-1.1.0/asyncio_oss/
--rw-r--r--   0 longyao    (501) staff       (20)      848 2023-06-26 17:53:43.000000 asyncio-oss-1.1.0/asyncio_oss/__init__.py
--rw-r--r--   0 longyao    (501) staff       (20)   152258 2023-06-26 17:05:09.000000 asyncio-oss-1.1.0/asyncio_oss/api.py
--rw-r--r--   0 longyao    (501) staff       (20)     9451 2023-06-26 14:59:28.000000 asyncio-oss-1.1.0/asyncio_oss/exceptions.py
--rw-r--r--   0 longyao    (501) staff       (20)     6699 2023-06-26 17:30:19.000000 asyncio-oss-1.1.0/asyncio_oss/http.py
--rw-r--r--   0 longyao    (501) staff       (20)    13081 2023-06-26 15:02:39.000000 asyncio-oss-1.1.0/asyncio_oss/iterators.py
--rw-r--r--   0 longyao    (501) staff       (20)     4729 2023-06-26 17:31:59.000000 asyncio-oss-1.1.0/asyncio_oss/models.py
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.209478 asyncio-oss-1.1.0/asyncio_oss/test/
--rw-r--r--   0 longyao    (501) staff       (20)      554 2023-05-29 13:59:36.000000 asyncio-oss-1.1.0/asyncio_oss/test/__init__.py
--rw-r--r--   0 longyao    (501) staff       (20)     2550 2023-06-25 15:44:33.000000 asyncio-oss-1.1.0/asyncio_oss/test/object_test.py
--rw-r--r--   0 longyao    (501) staff       (20)      499 2023-06-23 17:51:40.000000 asyncio-oss-1.1.0/asyncio_oss/test/service_test.py
--rw-r--r--   0 longyao    (501) staff       (20)     5892 2023-06-26 17:30:19.000000 asyncio-oss-1.1.0/asyncio_oss/utils.py
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-26 18:04:00.208945 asyncio-oss-1.1.0/asyncio_oss.egg-info/
--rw-r--r--   0 longyao    (501) staff       (20)     2944 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/PKG-INFO
--rw-r--r--   0 longyao    (501) staff       (20)      451 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/SOURCES.txt
--rw-r--r--   0 longyao    (501) staff       (20)        1 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/dependency_links.txt
--rw-r--r--   0 longyao    (501) staff       (20)       13 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/requires.txt
--rw-r--r--   0 longyao    (501) staff       (20)       12 2023-06-26 18:04:00.000000 asyncio-oss-1.1.0/asyncio_oss.egg-info/top_level.txt
--rw-r--r--   0 longyao    (501) staff       (20)       38 2023-06-26 18:04:00.209881 asyncio-oss-1.1.0/setup.cfg
--rw-r--r--   0 longyao    (501) staff       (20)      679 2023-06-26 18:01:57.000000 asyncio-oss-1.1.0/setup.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-30 16:08:50.775881 asyncio-oss-1.1.1/
+-rw-r--r--   0 longyao    (501) staff       (20)     1064 2023-05-24 15:02:54.000000 asyncio-oss-1.1.1/LICENSE
+-rw-r--r--   0 longyao    (501) staff       (20)     3197 2023-06-30 16:08:50.775775 asyncio-oss-1.1.1/PKG-INFO
+-rw-r--r--   0 longyao    (501) staff       (20)     2851 2023-06-30 16:02:36.000000 asyncio-oss-1.1.1/README.md
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-30 16:08:50.774164 asyncio-oss-1.1.1/asyncio_oss/
+-rw-r--r--   0 longyao    (501) staff       (20)      848 2023-06-26 17:53:43.000000 asyncio-oss-1.1.1/asyncio_oss/__init__.py
+-rw-r--r--   0 longyao    (501) staff       (20)   152258 2023-06-30 14:07:49.000000 asyncio-oss-1.1.1/asyncio_oss/api.py
+-rw-r--r--   0 longyao    (501) staff       (20)     9451 2023-06-26 14:59:28.000000 asyncio-oss-1.1.1/asyncio_oss/exceptions.py
+-rw-r--r--   0 longyao    (501) staff       (20)     6700 2023-06-30 15:48:52.000000 asyncio-oss-1.1.1/asyncio_oss/http.py
+-rw-r--r--   0 longyao    (501) staff       (20)    13081 2023-06-30 14:07:49.000000 asyncio-oss-1.1.1/asyncio_oss/iterators.py
+-rw-r--r--   0 longyao    (501) staff       (20)     4729 2023-06-26 17:31:59.000000 asyncio-oss-1.1.1/asyncio_oss/models.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-30 16:08:50.775482 asyncio-oss-1.1.1/asyncio_oss/test/
+-rw-r--r--   0 longyao    (501) staff       (20)      554 2023-05-29 13:59:36.000000 asyncio-oss-1.1.1/asyncio_oss/test/__init__.py
+-rw-r--r--   0 longyao    (501) staff       (20)     3806 2023-06-30 15:47:14.000000 asyncio-oss-1.1.1/asyncio_oss/test/object_test.py
+-rw-r--r--   0 longyao    (501) staff       (20)      499 2023-06-23 17:51:40.000000 asyncio-oss-1.1.1/asyncio_oss/test/service_test.py
+-rw-r--r--   0 longyao    (501) staff       (20)     5892 2023-06-26 17:30:19.000000 asyncio-oss-1.1.1/asyncio_oss/utils.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-30 16:08:50.774890 asyncio-oss-1.1.1/asyncio_oss.egg-info/
+-rw-r--r--   0 longyao    (501) staff       (20)     3197 2023-06-30 16:08:50.000000 asyncio-oss-1.1.1/asyncio_oss.egg-info/PKG-INFO
+-rw-r--r--   0 longyao    (501) staff       (20)      451 2023-06-30 16:08:50.000000 asyncio-oss-1.1.1/asyncio_oss.egg-info/SOURCES.txt
+-rw-r--r--   0 longyao    (501) staff       (20)        1 2023-06-30 16:08:50.000000 asyncio-oss-1.1.1/asyncio_oss.egg-info/dependency_links.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       13 2023-06-30 16:08:50.000000 asyncio-oss-1.1.1/asyncio_oss.egg-info/requires.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       12 2023-06-30 16:08:50.000000 asyncio-oss-1.1.1/asyncio_oss.egg-info/top_level.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       38 2023-06-30 16:08:50.775918 asyncio-oss-1.1.1/setup.cfg
+-rw-r--r--   0 longyao    (501) staff       (20)      679 2023-06-30 15:55:34.000000 asyncio-oss-1.1.1/setup.py
```

### Comparing `asyncio-oss-1.1.0/LICENSE` & `asyncio-oss-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/PKG-INFO` & `asyncio-oss-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-oss
-Version: 1.1.0
+Version: 1.1.1
 Summary: An asynchronous python client SDK for OSS(Aliyun Object Storage Service).
 Home-page: https://github.com/Yaocool/async-oss
 Author: Ozzy
 Author-email: ozzycharon@gmail.com
 License: MIT
 Keywords: asyncio-oss,async-oss,oss
 Description-Content-Type: text/markdown
@@ -19,18 +19,19 @@
 $ pip install asyncio-oss
 ```
 
 ## Local compilation
 ```shell script
 $ git clone git@github.com:Yaocool/async-oss.git
 $ python setup.py bdist_wheel
-$ pip install ./dist/asyncio_oss-1.0.0-py3-none-any.whl
+$ pip install ./dist/asyncio_oss-1.1.1-py3-none-any.whl
 ```
 
-# Example
+# Examples
+For more examples, please refer to the [test](./asyncio_oss/test) directory.
 ```python
 import logging
 
 import asyncio_oss
 import asyncio
 import oss2
 
@@ -70,24 +71,37 @@
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
 * [Jul 29, 2022 - 1.0.0]
   * fix `http.py/do_request` method stream read bug
+
+
 * [May 29, 2023]
   * add test cases and supported `asyncio-oss` package in PyPI
+
+
 * [May 30, 2023 - 1.0.1]
   * bump version to 1.0.1 for PyPI package description updating
+
+
 * [June 24, 2023 - 1.0.2]
   * remove unused fields add params in `asyncio_oss/http.py api.py` files
   * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
   * add `list_buckets` test case in `tests/service_test.py` for `Service` class
   * bump version to 1.0.2
+
+
 * [June 27, 2023 - 1.1.0]
   * remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package
   * support oss2==2.18.0 newest apis
   * support global log
   * bump version to 1.1.0
 
+
+* [June 28, 2023 - 1.1.1]
+  * fix the bug of wrong signature of `put_object_tagging` interface caused by default `Content-Type` of aiohttp
+  * bump version to 1.1.1
+
 # Discussions Or Issues
 Any questions can be raised in `Discussions` or `Issues`, I will answer them from time to time.
```

### Comparing `asyncio-oss-1.1.0/README.md` & `asyncio-oss-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 $ pip install asyncio-oss
 ```
 
 ## Local compilation
 ```shell script
 $ git clone git@github.com:Yaocool/async-oss.git
 $ python setup.py bdist_wheel
-$ pip install ./dist/asyncio_oss-1.0.0-py3-none-any.whl
+$ pip install ./dist/asyncio_oss-1.1.1-py3-none-any.whl
 ```
 
-# Example
+# Examples
+For more examples, please refer to the [test](./asyncio_oss/test) directory.
 ```python
 import logging
 
 import asyncio_oss
 import asyncio
 import oss2
 
@@ -58,24 +59,37 @@
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
 * [Jul 29, 2022 - 1.0.0]
   * fix `http.py/do_request` method stream read bug
+
+
 * [May 29, 2023]
   * add test cases and supported `asyncio-oss` package in PyPI
+
+
 * [May 30, 2023 - 1.0.1]
   * bump version to 1.0.1 for PyPI package description updating
+
+
 * [June 24, 2023 - 1.0.2]
   * remove unused fields add params in `asyncio_oss/http.py api.py` files
   * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
   * add `list_buckets` test case in `tests/service_test.py` for `Service` class
   * bump version to 1.0.2
+
+
 * [June 27, 2023 - 1.1.0]
   * remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package
   * support oss2==2.18.0 newest apis
   * support global log
   * bump version to 1.1.0
 
+
+* [June 28, 2023 - 1.1.1]
+  * fix the bug of wrong signature of `put_object_tagging` interface caused by default `Content-Type` of aiohttp
+  * bump version to 1.1.1
+
 # Discussions Or Issues
 Any questions can be raised in `Discussions` or `Issues`, I will answer them from time to time.
```

### Comparing `asyncio-oss-1.1.0/asyncio_oss/__init__.py` & `asyncio-oss-1.1.1/asyncio_oss/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss/api.py` & `asyncio-oss-1.1.1/asyncio_oss/api.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss/exceptions.py` & `asyncio-oss-1.1.1/asyncio_oss/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss/http.py` & `asyncio-oss-1.1.1/asyncio_oss/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,17 +99,17 @@
         self.cloudbox_id = cloudbox_id
 
         if not isinstance(headers, CaseInsensitiveDict):
             self.headers = CaseInsensitiveDict(headers)
         else:
             self.headers = headers
 
-        # tell requests not to add 'Accept-Encoding: gzip, deflate' by default
-        if 'Accept-Encoding' not in self.headers:
-            self.headers['Accept-Encoding'] = ''
+        # tell aiohttp not to add 'Content-Type: application/octet-stream' by default
+        if 'Content-Type' not in self.headers:
+            self.headers['Content-Type'] = ''
 
         if 'User-Agent' not in self.headers:
             if app_name:
                 self.headers['User-Agent'] = USER_AGENT + '/' + app_name
             else:
                 self.headers['User-Agent'] = USER_AGENT
```

### Comparing `asyncio-oss-1.1.0/asyncio_oss/iterators.py` & `asyncio-oss-1.1.1/asyncio_oss/iterators.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss/models.py` & `asyncio-oss-1.1.1/asyncio_oss/models.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss/test/__init__.py` & `asyncio-oss-1.1.1/asyncio_oss/test/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss/test/object_test.py` & `asyncio-oss-1.1.1/asyncio_oss/test/object_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,34 @@
         # Act
         result = await api.put_object(OBJECT_KEY, data)
 
         # Assert
         assert result.status == 200
 
     @pytest.mark.asyncio
+    async def test_put_object_with_tagging(self, api):
+        from oss2.headers import OSS_OBJECT_TAGGING
+
+        # Arrange
+        with open(LOCAL_TEST_FILE, 'rb') as f:
+            data = f.read()
+
+        # Act
+        tagging = "k1=v1"
+        headers = {OSS_OBJECT_TAGGING: tagging}
+
+        result = await api.put_object(OBJECT_KEY, data, headers=headers)
+
+        # Assert
+        assert result.status == 200
+        res = await api.get_object_tagging(OBJECT_KEY)
+        assert res.status == 200
+        assert res.tag_set.tagging_rule.get('k1', '') == 'v1'
+
+    @pytest.mark.asyncio
     async def test_put_object_from_file(self, api):
         # Act
         result = await api.put_object_from_file(OBJECT_KEY, LOCAL_TEST_FILE)
 
         # Assert
         assert result.status == 200
 
@@ -65,14 +85,39 @@
         # Assert
         assert result.status == 200
         with open(LOCAL_TEST_FILE, 'rb') as f:
             data_length = len(f.read())
         assert result.content_length == data_length
 
     @pytest.mark.asyncio
+    async def test_put_object_tagging(self, api):
+        from oss2.models import TaggingRule, Tagging
+
+        # Act
+        rule = TaggingRule()
+        rule.add('key1', 'value1')
+
+        # 创建标签。
+        tagging = Tagging(rule)
+
+        result = await api.put_object_tagging(OBJECT_KEY, tagging)
+
+        # Assert
+        assert result.status == 200
+
+    @pytest.mark.asyncio
+    async def test_get_object_tagging(self, api):
+        # Act
+        result = await api.get_object_tagging(OBJECT_KEY)
+
+        # Assert
+        assert result.status == 200
+        assert result.tag_set.tagging_rule.get('key1', '') == 'value1'
+
+    @pytest.mark.asyncio
     async def test_sign_url(self, api):
         # Act
         result = await api.sign_url('GET', OBJECT_KEY, 5 * 60)
         assert result is not None
         assert result != ""
 
     @pytest.mark.asyncio
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asyncio-oss-1.1.0/asyncio_oss/utils.py` & `asyncio-oss-1.1.1/asyncio_oss/utils.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.1.0/asyncio_oss.egg-info/PKG-INFO` & `asyncio-oss-1.1.1/asyncio_oss.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-oss
-Version: 1.1.0
+Version: 1.1.1
 Summary: An asynchronous python client SDK for OSS(Aliyun Object Storage Service).
 Home-page: https://github.com/Yaocool/async-oss
 Author: Ozzy
 Author-email: ozzycharon@gmail.com
 License: MIT
 Keywords: asyncio-oss,async-oss,oss
 Description-Content-Type: text/markdown
@@ -19,18 +19,19 @@
 $ pip install asyncio-oss
 ```
 
 ## Local compilation
 ```shell script
 $ git clone git@github.com:Yaocool/async-oss.git
 $ python setup.py bdist_wheel
-$ pip install ./dist/asyncio_oss-1.0.0-py3-none-any.whl
+$ pip install ./dist/asyncio_oss-1.1.1-py3-none-any.whl
 ```
 
-# Example
+# Examples
+For more examples, please refer to the [test](./asyncio_oss/test) directory.
 ```python
 import logging
 
 import asyncio_oss
 import asyncio
 import oss2
 
@@ -70,24 +71,37 @@
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
 * [Jul 29, 2022 - 1.0.0]
   * fix `http.py/do_request` method stream read bug
+
+
 * [May 29, 2023]
   * add test cases and supported `asyncio-oss` package in PyPI
+
+
 * [May 30, 2023 - 1.0.1]
   * bump version to 1.0.1 for PyPI package description updating
+
+
 * [June 24, 2023 - 1.0.2]
   * remove unused fields add params in `asyncio_oss/http.py api.py` files
   * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
   * add `list_buckets` test case in `tests/service_test.py` for `Service` class
   * bump version to 1.0.2
+
+
 * [June 27, 2023 - 1.1.0]
   * remove unused objects and methods in `asyncio_oss/models.py` and `asyncio_oss/utils.py` to streamline sdk package
   * support oss2==2.18.0 newest apis
   * support global log
   * bump version to 1.1.0
 
+
+* [June 28, 2023 - 1.1.1]
+  * fix the bug of wrong signature of `put_object_tagging` interface caused by default `Content-Type` of aiohttp
+  * bump version to 1.1.1
+
 # Discussions Or Issues
 Any questions can be raised in `Discussions` or `Issues`, I will answer them from time to time.
```

### Comparing `asyncio-oss-1.1.0/setup.py` & `asyncio-oss-1.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='asyncio-oss',
-    version='1.1.0',
+    version='1.1.1',
     description='An asynchronous python client SDK for OSS(Aliyun Object Storage Service).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yaocool/async-oss",
     keywords="asyncio-oss, async-oss, oss",
     author='Ozzy',
     author_email='ozzycharon@gmail.com',
```

