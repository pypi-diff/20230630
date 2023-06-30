# Comparing `tmp/pycrawlers-0.1.1.tar.gz` & `tmp/pycrawlers-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-0.1.1.tar", last modified: Sun Jun 25 05:57:50 2023, max compression
+gzip compressed data, was "pycrawlers-0.1.2.tar", last modified: Fri Jun 30 07:25:11 2023, max compression
```

## Comparing `pycrawlers-0.1.1.tar` & `pycrawlers-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.429322 pycrawlers-0.1.1/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.1.1/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     1746 2023-06-25 05:57:50.429196 pycrawlers-0.1.1/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     1289 2023-06-25 05:57:32.000000 pycrawlers-0.1.1/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.426503 pycrawlers-0.1.1/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.1.1/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.1.1/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.426708 pycrawlers-0.1.1/pycrawlers/
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.427702 pycrawlers-0.1.1/pycrawlers/Hugging_Face/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.1.1/pycrawlers/Hugging_Face/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.1.1/pycrawlers/Hugging_Face/download.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.428320 pycrawlers-0.1.1/pycrawlers/Web_Site/
--rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-0.1.1/pycrawlers/Web_Site/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-0.1.1/pycrawlers/Web_Site/get_web_page.py
--rw-r--r--   0 bo         (501) staff       (20)     3228 2023-06-25 05:57:32.000000 pycrawlers-0.1.1/pycrawlers/Web_Site/get_web_page_id.py
--rw-r--r--   0 bo         (501) staff       (20)     1006 2023-06-25 03:48:03.000000 pycrawlers-0.1.1/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.428918 pycrawlers-0.1.1/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.1.1/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-0.1.1/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     4962 2023-06-21 09:14:16.000000 pycrawlers-0.1.1/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-25 05:57:50.427374 pycrawlers-0.1.1/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     1746 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      521 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       71 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-06-25 05:57:50.000000 pycrawlers-0.1.1/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-25 05:57:50.429361 pycrawlers-0.1.1/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      907 2023-06-25 04:15:50.000000 pycrawlers-0.1.1/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.388288 pycrawlers-0.1.2/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.1.2/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     2885 2023-06-30 07:25:11.388158 pycrawlers-0.1.2/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     2428 2023-06-30 07:24:12.000000 pycrawlers-0.1.2/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.385222 pycrawlers-0.1.2/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.1.2/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.1.2/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.385415 pycrawlers-0.1.2/pycrawlers/
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.386355 pycrawlers-0.1.2/pycrawlers/Hugging_Face/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.1.2/pycrawlers/Hugging_Face/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.1.2/pycrawlers/Hugging_Face/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.387168 pycrawlers-0.1.2/pycrawlers/Web_Site/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/url_filters.py
+-rw-r--r--   0 bo         (501) staff       (20)     1035 2023-06-30 07:15:34.000000 pycrawlers-0.1.2/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.387821 pycrawlers-0.1.2/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.1.2/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-0.1.2/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     4962 2023-06-21 09:14:16.000000 pycrawlers-0.1.2/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.386003 pycrawlers-0.1.2/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     2885 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      556 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-30 07:25:11.388329 pycrawlers-0.1.2/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-06-30 07:22:01.000000 pycrawlers-0.1.2/setup.py
```

### Comparing `pycrawlers-0.1.1/LICENSE` & `pycrawlers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.1/other/dw_hg.py` & `pycrawlers-0.1.2/other/dw_hg.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.1/pycrawlers/Hugging_Face/download.py` & `pycrawlers-0.1.2/pycrawlers/Hugging_Face/download.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.1/pycrawlers/Web_Site/get_web_page.py` & `pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.1/pycrawlers/Web_Site/get_web_page_id.py` & `pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 
 import time
 from lxml import etree
 from pycrawlers.common.tools import MongoHelper, requests_get
 
 
 def crawl_web_page_id(mongo_host: str, mongo_port: str, db_name: str, id_collection_name: str, collection_name: str,
-                      base_url: str, start_done: int = 0, end_done: int = 1, proxies=None, logger=None):
+                      base_url: str, start_done: int = 0, end_done: int = 1, proxies=None, logger=None,
+                      url_filter=None):
     """
     获取网页url
     :param mongo_host:
     :param mongo_port:
     :param db_name:
     :param id_collection_name: 存储网页url的表名
     :param collection_name: 存储网页的表名
     :param base_url: 网页首页
     :param start_done: 未抓取的url标记
     :param end_done: 已抓取的url标记
     :param proxies: 代理
     :param logger: 日志
+    :param url_filter: url 过滤器, 一个函数，输入url 判断是否需要抓取， 返回值 True 或 Fasle, True表示需要抓取
     :return:
     """
     mg_hp = MongoHelper(mongo_host, mongo_port)
     id_collection = mg_hp.get_collection(id_collection_name, db_name)
     collection = mg_hp.get_collection(collection_name, db_name)
     if not collection.find_one({'_id': base_url}):
         response = requests_get(base_url, is_etree=False, timeout=20, proxies=proxies, logger=logger)
@@ -53,17 +55,21 @@
                                         continue
                                     elif len(href) > 1 and href[1] == '/':
                                         url = 'https:' + href
                                         if base_url not in url:
                                             continue
                                     else:
                                         url = base_url + href
-                                if id_collection.find_one({'_id': url}):
-                                    continue
-                                id_collection.insert_one({'_id': url, 'done': 0})
+                                tag = True
+                                if url_filter:
+                                    tag = url_filter(url)
+                                if tag:
+                                    if id_collection.find_one({'_id': url}):
+                                        continue
+                                    id_collection.insert_one({'_id': url, 'done': 0})
                     except Exception as e:
                         if logger:
                             logger.info(e)
                         else:
                             print(e)
                 else:
                     info_str = 'no html data :' + str(_id)
```

### Comparing `pycrawlers-0.1.1/pycrawlers/__init__.py` & `pycrawlers-0.1.2/pycrawlers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 def huggingface(base_url: str = None):
     from pycrawlers.Hugging_Face.download import HuggingFace
     return HuggingFace(base_url)
 
 
 def website(mongo_host: str, mongo_port: str, db_name: str, id_collection_name: str, collection_name: str,
-            base_url: str, start_done: int = 0, end_done: int = 1, proxies=None, logger=None):
+            base_url: str, start_done: int = 0, end_done: int = 1, proxies=None, logger=None, url_filter=None):
     from concurrent.futures import ThreadPoolExecutor
     from pycrawlers.Web_Site.get_web_page import crawl_web_page
     from pycrawlers.Web_Site.get_web_page_id import crawl_web_page_id
     import time
     pool = ThreadPoolExecutor(max_workers=2)
     pool.submit(crawl_web_page_id, mongo_host, mongo_port, db_name, id_collection_name, collection_name,
-                base_url, start_done, end_done, proxies, logger)
+                base_url, start_done, end_done, proxies, logger, url_filter)
     time.sleep(3)
     pool.submit(crawl_web_page, mongo_host, mongo_port, db_name, id_collection_name, collection_name,
                 start_done, end_done, proxies, logger)
```

### Comparing `pycrawlers-0.1.1/pycrawlers/common/default_data.py` & `pycrawlers-0.1.2/pycrawlers/common/default_data.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.1/pycrawlers/common/tools.py` & `pycrawlers-0.1.2/pycrawlers/common/tools.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.1/setup.py` & `pycrawlers-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='0.1.1',
+    version='0.1.2',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
```

