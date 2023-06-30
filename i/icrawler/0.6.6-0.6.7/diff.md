# Comparing `tmp/icrawler-0.6.6.tar.gz` & `tmp/icrawler-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/v-zhichen/icrawler/dist/tmp96abvoku/icrawler-0.6.6.tar", last modified: Sat Aug 14 11:21:13 2021, max compression
+gzip compressed data, was "icrawler-0.6.7.tar", last modified: Fri Jun 30 16:00:44 2023, max compression
```

## Comparing `icrawler-0.6.6.tar` & `icrawler-0.6.7.tar`

### file list

```diff
@@ -1,42 +1,66 @@
-drwxr-xr-x   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        0 2021-08-14 11:21:13.342877 icrawler-0.6.6/
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1075 2021-08-14 11:04:52.000000 icrawler-0.6.6/LICENSE
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)       18 2021-08-14 11:04:52.000000 icrawler-0.6.6/MANIFEST.in
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     4318 2021-08-14 11:21:13.342877 icrawler-0.6.6/PKG-INFO
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     3453 2021-08-14 11:19:51.000000 icrawler-0.6.6/README.rst
-drwxr-xr-x   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        0 2021-08-14 11:21:13.338877 icrawler-0.6.6/icrawler/
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)      321 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/__init__.py
-drwxr-xr-x   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        0 2021-08-14 11:21:13.338877 icrawler-0.6.6/icrawler/builtin/
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)      426 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/__init__.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     5966 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/baidu.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     6166 2021-08-14 11:19:51.000000 icrawler-0.6.6/icrawler/builtin/bing.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1373 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/filter.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     5623 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/flickr.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     7737 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/google.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     3987 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/greedy.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     2189 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/builtin/urllist.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     7639 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/crawler.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)    10411 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/downloader.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     3311 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/feeder.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     5347 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/parser.py
-drwxr-xr-x   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        0 2021-08-14 11:21:13.338877 icrawler-0.6.6/icrawler/storage/
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)      165 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/storage/__init__.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)      843 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/storage/base.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1120 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/storage/filesystem.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1304 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/storage/google_storage.py
-drwxr-xr-x   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        0 2021-08-14 11:21:13.342877 icrawler-0.6.6/icrawler/utils/
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)      295 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/utils/__init__.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     2232 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/utils/cached_queue.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)    20757 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/utils/proxy_pool.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1521 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/utils/session.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1366 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/utils/signal.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     3663 2021-08-14 11:04:52.000000 icrawler-0.6.6/icrawler/utils/thread_pool.py
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)       22 2021-08-14 11:20:21.000000 icrawler-0.6.6/icrawler/version.py
-drwxr-xr-x   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        0 2021-08-14 11:21:13.338877 icrawler-0.6.6/icrawler.egg-info/
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     4318 2021-08-14 11:21:13.000000 icrawler-0.6.6/icrawler.egg-info/PKG-INFO
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)      865 2021-08-14 11:21:13.000000 icrawler-0.6.6/icrawler.egg-info/SOURCES.txt
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        1 2021-08-14 11:21:13.000000 icrawler-0.6.6/icrawler.egg-info/dependency_links.txt
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        1 2021-08-14 11:08:06.000000 icrawler-0.6.6/icrawler.egg-info/not-zip-safe
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)       62 2021-08-14 11:21:13.000000 icrawler-0.6.6/icrawler.egg-info/requires.txt
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)        9 2021-08-14 11:21:13.000000 icrawler-0.6.6/icrawler.egg-info/top_level.txt
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)       67 2021-08-14 11:21:13.342877 icrawler-0.6.6/setup.cfg
--rw-r--r--   0 FAREAST.v-zhichen (202706864) FAREAST.domain users (200000513)     1544 2021-08-14 11:04:52.000000 icrawler-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.173752 icrawler-0.6.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 16:00:39.000000 icrawler-0.6.7/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.173752 icrawler-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-30 16:00:39.000000 icrawler-0.6.7/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-30 16:00:39.000000 icrawler-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-30 16:00:39.000000 icrawler-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-30 16:00:39.000000 icrawler-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 16:00:39.000000 icrawler-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-30 16:00:44.177752 icrawler-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-30 16:00:39.000000 icrawler-0.6.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/builtin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/extend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-30 16:00:39.000000 icrawler-0.6.7/docs/release_notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-30 16:00:39.000000 icrawler-0.6.7/examples/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 16:00:39.000000 icrawler-0.6.7/examples/filelist_demo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/flickr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/builtin/urllist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/storage/google_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/cached_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/proxy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 16:00:39.000000 icrawler-0.6.7/icrawler/utils/thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 16:00:43.000000 icrawler-0.6.7/icrawler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/icrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 16:00:44.000000 icrawler-0.6.7/icrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 16:00:39.000000 icrawler-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 16:00:39.000000 icrawler-0.6.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:00:44.177752 icrawler-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:00:39.000000 icrawler-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:00:44.177752 icrawler-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-30 16:00:39.000000 icrawler-0.6.7/tests/test_todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 16:00:39.000000 icrawler-0.6.7/tox.ini
```

### Comparing `icrawler-0.6.6/LICENSE` & `icrawler-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `icrawler-0.6.6/README.rst` & `icrawler-0.6.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ------------
 
 A crawler consists of 3 main components (Feeder, Parser and Downloader),
 they are connected with each other with FIFO queues. The workflow is shown in
 the following figure.
 
 .. figure:: http://7xopqn.com1.z0.glb.clouddn.com/workflow.png
-   :alt: 
+   :alt:
 
 -  ``url_queue`` stores the url of pages which may contain images
 -  ``task_queue`` stores the image url as well as any meta data you
    like, each element in the queue is a dictionary and must contain the
    field ``img_url``
 -  Feeder puts page urls to ``url_queue``
 -  Parser requests and parses the page, then extracts the image urls and
```

### Comparing `icrawler-0.6.6/icrawler/builtin/baidu.py` & `icrawler-0.6.7/icrawler/builtin/baidu.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,173 +1,179 @@
-# -*- coding: utf-8 -*-
-
 import json
 
-from icrawler import Crawler, Feeder, Parser, ImageDownloader
-from icrawler.builtin.filter import Filter
+from .. import Crawler, Feeder, ImageDownloader, Parser
+from .filter import Filter
 
 
 class BaiduFeeder(Feeder):
-
     def get_filter(self):
         search_filter = Filter()
 
         # type filter
         type_code = {
-            'portrait': 's=3&lm=0&st=-1&face=0',
-            'face': 's=0&lm=0&st=-1&face=1',
-            'clipart': 's=0&lm=0&st=1&face=0',
-            'linedrawing': 's=0&lm=0&st=2&face=0',
-            'animated': 's=0&lm=6&st=-1&face=0',
-            'static': 's=0&lm=7&st=-1&face=0'
+            "portrait": "s=3&lm=0&st=-1&face=0",
+            "face": "s=0&lm=0&st=-1&face=1",
+            "clipart": "s=0&lm=0&st=1&face=0",
+            "linedrawing": "s=0&lm=0&st=2&face=0",
+            "animated": "s=0&lm=6&st=-1&face=0",
+            "static": "s=0&lm=7&st=-1&face=0",
         }
 
         def format_type(img_type):
             return type_code[img_type]
 
         type_choices = list(type_code.keys())
-        search_filter.add_rule('type', format_type, type_choices)
+        search_filter.add_rule("type", format_type, type_choices)
 
         # color filter
         color_code = {
-            'red': 1,
-            'orange': 256,
-            'yellow': 2,
-            'green': 4,
-            'purple': 32,
-            'pink': 64,
-            'teal': 8,
-            'blue': 16,
-            'brown': 12,
-            'white': 1024,
-            'black': 512,
-            'blackandwhite': 2048
+            "red": 1,
+            "orange": 256,
+            "yellow": 2,
+            "green": 4,
+            "purple": 32,
+            "pink": 64,
+            "teal": 8,
+            "blue": 16,
+            "brown": 12,
+            "white": 1024,
+            "black": 512,
+            "blackandwhite": 2048,
         }
 
         def format_color(color):
-            return 'ic={}'.format(color_code[color])
+            return f"ic={color_code[color]}"
 
         color_choices = list(color_code.keys())
-        search_filter.add_rule('color', format_color, color_choices)
+        search_filter.add_rule("color", format_color, color_choices)
 
         # size filter
         def format_size(size):
-            if size in ['extralarge', 'large', 'medium', 'small']:
-                size_code = {
-                    'extralarge': 9,
-                    'large': 3,
-                    'medium': 2,
-                    'small': 1
-                }
-                return 'z={}'.format(size_code[size])
-            elif size.startswith('='):
-                wh = size[1:].split('x')
+            if size in ["extralarge", "large", "medium", "small"]:
+                size_code = {"extralarge": 9, "large": 3, "medium": 2, "small": 1}
+                return f"z={size_code[size]}"
+            elif size.startswith("="):
+                wh = size[1:].split("x")
                 assert len(wh) == 2
-                return 'width={}&height={}'.format(*wh)
+                return "width={}&height={}".format(*wh)
             else:
                 raise ValueError(
                     'filter option "size" must be one of the following: '
-                    'extralarge, large, medium, small, >[]x[] '
-                    '([] is an integer)')
+                    "extralarge, large, medium, small, >[]x[] "
+                    "([] is an integer)"
+                )
 
-        search_filter.add_rule('size', format_size)
+        search_filter.add_rule("size", format_size)
 
         return search_filter
 
     def feed(self, keyword, offset, max_num, filters=None):
-        base_url = ('http://image.baidu.com/search/acjson?tn=resultjson_com'
-                    '&ipn=rj&word={}&pn={}&rn=30')
+        base_url = "http://image.baidu.com/search/acjson?tn=resultjson_com" "&ipn=rj&word={}&pn={}&rn=30"
         self.filter = self.get_filter()
-        filter_str = self.filter.apply(filters, sep='&')
+        filter_str = self.filter.apply(filters, sep="&")
         for i in range(offset, offset + max_num, 30):
             url = base_url.format(keyword, i)
             if filter_str:
-                url += '&' + filter_str
+                url += "&" + filter_str
             self.out_queue.put(url)
-            self.logger.debug('put url to url_queue: {}'.format(url))
+            self.logger.debug(f"put url to url_queue: {url}")
 
 
 class BaiduParser(Parser):
-
     def _decode_url(self, encrypted_url):
         url = encrypted_url
-        map1 = {'_z2C$q': ':', '_z&e3B': '.', 'AzdH3F': '/'}
+        map1 = {"_z2C$q": ":", "_z&e3B": ".", "AzdH3F": "/"}
         map2 = {
-            'w': 'a', 'k': 'b', 'v': 'c', '1': 'd', 'j': 'e',
-            'u': 'f', '2': 'g', 'i': 'h', 't': 'i', '3': 'j',
-            'h': 'k', 's': 'l', '4': 'm', 'g': 'n', '5': 'o',
-            'r': 'p', 'q': 'q', '6': 'r', 'f': 's', 'p': 't',
-            '7': 'u', 'e': 'v', 'o': 'w', '8': '1', 'd': '2',
-            'n': '3', '9': '4', 'c': '5', 'm': '6', '0': '7',
-            'b': '8', 'l': '9', 'a': '0'
+            "w": "a",
+            "k": "b",
+            "v": "c",
+            "1": "d",
+            "j": "e",
+            "u": "f",
+            "2": "g",
+            "i": "h",
+            "t": "i",
+            "3": "j",
+            "h": "k",
+            "s": "l",
+            "4": "m",
+            "g": "n",
+            "5": "o",
+            "r": "p",
+            "q": "q",
+            "6": "r",
+            "f": "s",
+            "p": "t",
+            "7": "u",
+            "e": "v",
+            "o": "w",
+            "8": "1",
+            "d": "2",
+            "n": "3",
+            "9": "4",
+            "c": "5",
+            "m": "6",
+            "0": "7",
+            "b": "8",
+            "l": "9",
+            "a": "0",
         }  # yapf: disable
-        for (ciphertext, plaintext) in map1.items():
+        for ciphertext, plaintext in map1.items():
             url = url.replace(ciphertext, plaintext)
         char_list = [char for char in url]
         for i in range(len(char_list)):
             if char_list[i] in map2:
                 char_list[i] = map2[char_list[i]]
-        url = ''.join(char_list)
+        url = "".join(char_list)
         return url
 
     def parse(self, response):
         try:
-            content = response.content.decode('utf-8',
-                                              'ignore').replace("\\'", "'")
+            content = response.content.decode("utf-8", "ignore").replace("\\'", "'")
             content = json.loads(content, strict=False)
         except:
-            self.logger.error('Fail to parse the response in json format')
+            self.logger.error("Fail to parse the response in json format")
             return
-        for item in content['data']:
-            if 'objURL' in item:
-                img_url = self._decode_url(item['objURL'])
-            elif 'hoverURL' in item:
-                img_url = item['hoverURL']
+        for item in content["data"]:
+            if "objURL" in item:
+                img_url = self._decode_url(item["objURL"])
+            elif "hoverURL" in item:
+                img_url = item["hoverURL"]
             else:
                 continue
             yield dict(file_url=img_url)
 
 
 class BaiduImageCrawler(Crawler):
+    def __init__(self, feeder_cls=BaiduFeeder, parser_cls=BaiduParser, downloader_cls=ImageDownloader, *args, **kwargs):
+        super().__init__(feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
 
-    def __init__(self,
-                 feeder_cls=BaiduFeeder,
-                 parser_cls=BaiduParser,
-                 downloader_cls=ImageDownloader,
-                 *args,
-                 **kwargs):
-        super(BaiduImageCrawler,
-              self).__init__(feeder_cls, parser_cls, downloader_cls, *args,
-                             **kwargs)
-
-    def crawl(self,
-              keyword,
-              filters=None,
-              offset=0,
-              max_num=1000,
-              min_size=None,
-              max_size=None,
-              file_idx_offset=0,
-              overwrite=False):
+    def crawl(
+        self,
+        keyword,
+        filters=None,
+        offset=0,
+        max_num=1000,
+        min_size=None,
+        max_size=None,
+        file_idx_offset=0,
+        overwrite=False,
+    ):
         if offset + max_num > 1000:
             if offset > 1000:
-                self.logger.error('Offset cannot exceed 1000, otherwise you '
-                                  'will get duplicated searching results.')
+                self.logger.error("Offset cannot exceed 1000, otherwise you " "will get duplicated searching results.")
                 return
             elif max_num > 1000:
                 max_num = 1000 - offset
                 self.logger.warning(
-                    'Due to Baidu\'s limitation, you can only '
+                    "Due to Baidu's limitation, you can only "
                     'get the first 1000 result. "max_num" has '
-                    'been automatically set to %d', 1000 - offset)
+                    "been automatically set to %d",
+                    1000 - offset,
+                )
         else:
             pass
-        feeder_kwargs = dict(
-            keyword=keyword, offset=offset, max_num=max_num, filters=filters)
+        feeder_kwargs = dict(keyword=keyword, offset=offset, max_num=max_num, filters=filters)
         downloader_kwargs = dict(
-            max_num=max_num,
-            min_size=min_size,
-            max_size=max_size,
-            file_idx_offset=file_idx_offset,
-            overwrite=overwrite)
-        super(BaiduImageCrawler, self).crawl(
-            feeder_kwargs=feeder_kwargs, downloader_kwargs=downloader_kwargs)
+            max_num=max_num, min_size=min_size, max_size=max_size, file_idx_offset=file_idx_offset, overwrite=overwrite
+        )
+        super().crawl(feeder_kwargs=feeder_kwargs, downloader_kwargs=downloader_kwargs)
```

### Comparing `icrawler-0.6.6/icrawler/builtin/bing.py` & `icrawler-0.6.7/icrawler/builtin/bing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,174 +1,165 @@
-# -*- coding: utf-8 -*-
-
+import html
 import re
 
 import six
 from bs4 import BeautifulSoup
-import html
 
-from icrawler import Crawler, Parser, Feeder, ImageDownloader
-from icrawler.builtin.filter import Filter
+from .. import Crawler, Feeder, ImageDownloader, Parser
+from .filter import Filter
 
 
 class BingFeeder(Feeder):
-
     def get_filter(self):
         search_filter = Filter()
 
         # type filter
         def format_type(img_type):
-            prefix = '+filterui:photo-'
-            return (prefix + 'animatedgif'
-                    if img_type == 'animated' else prefix + img_type)
+            prefix = "+filterui:photo-"
+            return prefix + "animatedgif" if img_type == "animated" else prefix + img_type
 
-        type_choices = [
-            'photo', 'clipart', 'linedrawing', 'transparent', 'animated'
-        ]
-        search_filter.add_rule('type', format_type, type_choices)
+        type_choices = ["photo", "clipart", "linedrawing", "transparent", "animated"]
+        search_filter.add_rule("type", format_type, type_choices)
 
         # color filter
         def format_color(color):
-            prefix = '+filterui:color2-'
-            if color == 'color':
-                return prefix + 'color'
-            elif color == 'blackandwhite':
-                return prefix + 'bw'
+            prefix = "+filterui:color2-"
+            if color == "color":
+                return prefix + "color"
+            elif color == "blackandwhite":
+                return prefix + "bw"
             else:
-                return prefix + 'FGcls_' + color.upper()
+                return prefix + "FGcls_" + color.upper()
 
         color_choices = [
-            'color', 'blackandwhite', 'red', 'orange', 'yellow', 'green',
-            'teal', 'blue', 'purple', 'pink', 'white', 'gray', 'black', 'brown'
+            "color",
+            "blackandwhite",
+            "red",
+            "orange",
+            "yellow",
+            "green",
+            "teal",
+            "blue",
+            "purple",
+            "pink",
+            "white",
+            "gray",
+            "black",
+            "brown",
         ]
-        search_filter.add_rule('color', format_color, color_choices)
+        search_filter.add_rule("color", format_color, color_choices)
 
         # size filter
         def format_size(size):
-            if size in ['large', 'medium', 'small']:
-                return '+filterui:imagesize-' + size
-            elif size == 'extralarge':
-                return '+filterui:imagesize-wallpaper'
-            elif size.startswith('>'):
-                wh = size[1:].split('x')
+            if size in ["large", "medium", "small"]:
+                return "+filterui:imagesize-" + size
+            elif size == "extralarge":
+                return "+filterui:imagesize-wallpaper"
+            elif size.startswith(">"):
+                wh = size[1:].split("x")
                 assert len(wh) == 2
-                return '+filterui:imagesize-custom_{}_{}'.format(*wh)
+                return "+filterui:imagesize-custom_{}_{}".format(*wh)
             else:
                 raise ValueError(
                     'filter option "size" must be one of the following: '
-                    'extralarge, large, medium, small, >[]x[] '
-                    '([] is an integer)')
+                    "extralarge, large, medium, small, >[]x[] "
+                    "([] is an integer)"
+                )
 
-        search_filter.add_rule('size', format_size)
+        search_filter.add_rule("size", format_size)
 
         # licence filter
         license_code = {
-            'creativecommons': 'licenseType-Any',
-            'publicdomain': 'license-L1',
-            'noncommercial': 'license-L2_L3_L4_L5_L6_L7',
-            'commercial': 'license-L2_L3_L4',
-            'noncommercial,modify': 'license-L2_L3_L5_L6',
-            'commercial,modify': 'license-L2_L3'
+            "creativecommons": "licenseType-Any",
+            "publicdomain": "license-L1",
+            "noncommercial": "license-L2_L3_L4_L5_L6_L7",
+            "commercial": "license-L2_L3_L4",
+            "noncommercial,modify": "license-L2_L3_L5_L6",
+            "commercial,modify": "license-L2_L3",
         }
 
         def format_license(license):
-            return '+filterui:' + license_code[license]
+            return "+filterui:" + license_code[license]
 
         license_choices = list(license_code.keys())
-        search_filter.add_rule('license', format_license, license_choices)
+        search_filter.add_rule("license", format_license, license_choices)
 
         # layout filter
-        layout_choices = ['square', 'wide', 'tall']
-        search_filter.add_rule('layout', lambda x: '+filterui:aspect-' + x,
-                               layout_choices)
+        layout_choices = ["square", "wide", "tall"]
+        search_filter.add_rule("layout", lambda x: "+filterui:aspect-" + x, layout_choices)
 
         # people filter
-        people_choices = ['face', 'portrait']
-        search_filter.add_rule('people', lambda x: '+filterui:face-' + x,
-                               people_choices)
+        people_choices = ["face", "portrait"]
+        search_filter.add_rule("people", lambda x: "+filterui:face-" + x, people_choices)
 
         # date filter
-        date_minutes = {
-            'pastday': 1440,
-            'pastweek': 10080,
-            'pastmonth': 43200,
-            'pastyear': 525600
-        }
+        date_minutes = {"pastday": 1440, "pastweek": 10080, "pastmonth": 43200, "pastyear": 525600}
 
         def format_date(date):
-            return '+filterui:age-lt' + str(date_minutes[date])
+            return "+filterui:age-lt" + str(date_minutes[date])
 
         date_choices = list(date_minutes.keys())
-        search_filter.add_rule('date', format_date, date_choices)
+        search_filter.add_rule("date", format_date, date_choices)
 
         return search_filter
 
     def feed(self, keyword, offset, max_num, filters=None):
-        base_url = 'https://www.bing.com/images/async?q={}&first={}'
+        base_url = "https://www.bing.com/images/async?q={}&first={}"
         self.filter = self.get_filter()
         filter_str = self.filter.apply(filters)
-        filter_str = '&qft=' + filter_str if filter_str else ''
+        filter_str = "&qft=" + filter_str if filter_str else ""
 
         for i in range(offset, offset + max_num, 20):
             url = base_url.format(keyword, i) + filter_str
             self.out_queue.put(url)
-            self.logger.debug('put url to url_queue: {}'.format(url))
+            self.logger.debug(f"put url to url_queue: {url}")
 
 
 class BingParser(Parser):
-
     def parse(self, response):
-        soup = BeautifulSoup(
-            response.content.decode('utf-8', 'ignore'), 'lxml')
-        image_divs = soup.find_all('div', class_='imgpt')
-        pattern = re.compile(r'murl\":\"(.*?)\.jpg')
+        soup = BeautifulSoup(response.content.decode("utf-8", "ignore"), "lxml")
+        image_divs = soup.find_all("div", class_="imgpt")
+        pattern = re.compile(r"murl\":\"(.*?)\.jpg")
         for div in image_divs:
-            href_str = html.unescape(div.a['m'])
+            try:
+                href_str = html.unescape(div.a["m"])
+            except KeyError:
+                continue
             match = pattern.search(href_str)
             if match:
-                name = (match.group(1)
-                        if six.PY3 else match.group(1).encode('utf-8'))
-                img_url = '{}.jpg'.format(name)
+                name = match.group(1) if six.PY3 else match.group(1).encode("utf-8")
+                img_url = f"{name}.jpg"
                 yield dict(file_url=img_url)
 
 
 class BingImageCrawler(Crawler):
+    def __init__(self, feeder_cls=BingFeeder, parser_cls=BingParser, downloader_cls=ImageDownloader, *args, **kwargs):
+        super().__init__(feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
 
-    def __init__(self,
-                 feeder_cls=BingFeeder,
-                 parser_cls=BingParser,
-                 downloader_cls=ImageDownloader,
-                 *args,
-                 **kwargs):
-        super(BingImageCrawler, self).__init__(feeder_cls, parser_cls,
-                                               downloader_cls, *args, **kwargs)
-
-    def crawl(self,
-              keyword,
-              filters=None,
-              offset=0,
-              max_num=1000,
-              min_size=None,
-              max_size=None,
-              file_idx_offset=0,
-              overwrite=False):
+    def crawl(
+        self,
+        keyword,
+        filters=None,
+        offset=0,
+        max_num=1000,
+        min_size=None,
+        max_size=None,
+        file_idx_offset=0,
+        overwrite=False,
+    ):
         if offset + max_num > 1000:
             if offset > 1000:
-                self.logger.error('Offset cannot exceed 1000, otherwise you '
-                                  'will get duplicated searching results.')
+                self.logger.error("Offset cannot exceed 1000, otherwise you " "will get duplicated searching results.")
                 return
             elif max_num > 1000:
                 max_num = 1000 - offset
-                self.logger.warning('Due to Bing\'s limitation, you can only '
-                                    'get the first 1000 result. "max_num" has '
-                                    'been automatically set to %d',
-                                    1000 - offset)
-        feeder_kwargs = dict(
-            keyword=keyword, offset=offset, max_num=max_num, filters=filters)
+                self.logger.warning(
+                    "Due to Bing's limitation, you can only "
+                    'get the first 1000 result. "max_num" has '
+                    "been automatically set to %d",
+                    1000 - offset,
+                )
+        feeder_kwargs = dict(keyword=keyword, offset=offset, max_num=max_num, filters=filters)
         downloader_kwargs = dict(
-            max_num=max_num,
-            min_size=min_size,
-            max_size=max_size,
-            file_idx_offset=file_idx_offset,
-            overwrite=overwrite)
-        super(BingImageCrawler, self).crawl(
-            feeder_kwargs=feeder_kwargs, downloader_kwargs=downloader_kwargs)
+            max_num=max_num, min_size=min_size, max_size=max_size, file_idx_offset=file_idx_offset, overwrite=overwrite
+        )
+        super().crawl(feeder_kwargs=feeder_kwargs, downloader_kwargs=downloader_kwargs)
```

### Comparing `icrawler-0.6.6/icrawler/builtin/filter.py` & `icrawler-0.6.7/icrawler/builtin/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-# -*- coding: utf-8 -*-
-
-
-class Filter():
-
+class Filter:
     def __init__(self):
         self.rules = {}
 
     def add_rule(self, name, format_fn, choices=None):
         assert callable(format_fn)
         assert choices is None or isinstance(choices, list)
         self.rules[name] = (format_fn, choices)
 
-    def apply(self, options, sep=''):
+    def apply(self, options, sep=""):
         if options is None:
-            return ''
+            return ""
         assert isinstance(options, dict)
         formatted = []
         for name, val in options.items():
             if name not in self.rules:
                 raise KeyError(
-                    'unsupported filter "{}"， supported filter options are {}'.
-                    format(name), ', '.join(self.rules.keys()))
+                    f"unsupported filter '{name}'， supported filter options are {', '.join(self.rules.keys())}",
+                )
             format_fn, choices = self.rules[name]
             # validate the option value
             if isinstance(choices, type) and not isinstance(val, choices):
-                raise TypeError(
-                    'filter option "{}" must be a {}, not {}'.format(
-                        name, choices.__name__,
-                        type(val).__name__))
+                raise TypeError(f'filter option "{name}" must be a {choices.__name__}, not {type(val).__name__}')
             elif isinstance(choices, list) and val not in choices:
-                raise ValueError(
-                    'filter option "{}" must be one of the following: {}'.
-                    format(name, ', '.join(choices)))
+                raise ValueError('filter option "{}" must be one of the following: {}'.format(name, ", ".join(choices)))
             formatted.append(format_fn(val))
         return sep.join(formatted)
```

### Comparing `icrawler-0.6.6/icrawler/builtin/flickr.py` & `icrawler-0.6.7/icrawler/builtin/flickr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,152 +1,174 @@
-# -*- coding: utf-8 -*-
-
 import datetime
 import json
 import math
 import os
+from urllib.parse import urlencode
 
-from six.moves.urllib.parse import urlencode
-
-from icrawler import Crawler, Feeder, Parser, ImageDownloader
+from .. import Crawler, Feeder, ImageDownloader, Parser
 
 
 class FlickrFeeder(Feeder):
-
     def feed(self, apikey, max_num=4000, **kwargs):
         if max_num > 4000:
             max_num = 4000
-            self.logger.warning(
-                'max_num exceeds 4000, set it to 4000 automatically.')
-        base_url = 'https://api.flickr.com/services/rest/?'
-        params = {
-            'method': 'flickr.photos.search',
-            'api_key': apikey,
-            'format': 'json',
-            'nojsoncallback': 1
-        }
+            self.logger.warning("max_num exceeds 4000, set it to 4000 automatically.")
+        base_url = "https://api.flickr.com/services/rest/?"
+        params = {"method": "flickr.photos.search", "api_key": apikey, "format": "json", "nojsoncallback": 1}
         for key in kwargs:
-            if key in ['user_id', 'tags', 'tag_mode', 'text', 'license',
-                       'sort', 'privacy_filter', 'accuracy', 'safe_search',
-                       'content_type', 'machine_tags', 'machine_tag_mode',
-                       'group_id', 'contacts', 'woe_id', 'place_id', 'has_geo',
-                       'geo_context', 'lat', 'lon', 'radius', 'radius_units',
-                       'is_commons', 'in_gallery', 'is_getty', 'extras',
-                       'per_page', 'page',
-                       'color_codes', 'styles', 'orientation']:  # yapf: disable
+            if key in [
+                "user_id",
+                "tags",
+                "tag_mode",
+                "text",
+                "license",
+                "sort",
+                "privacy_filter",
+                "accuracy",
+                "safe_search",
+                "content_type",
+                "machine_tags",
+                "machine_tag_mode",
+                "group_id",
+                "contacts",
+                "woe_id",
+                "place_id",
+                "has_geo",
+                "geo_context",
+                "lat",
+                "lon",
+                "radius",
+                "radius_units",
+                "is_commons",
+                "in_gallery",
+                "is_getty",
+                "extras",
+                "per_page",
+                "page",
+                "color_codes",
+                "styles",
+                "orientation",
+            ]:  # yapf: disable
                 params[key] = kwargs[key]
-            elif key in ['min_upload_date', 'max_upload_date',
-                         'min_taken_date', 'max_taken_date']:  # yapf: disable
+            elif key in ["min_upload_date", "max_upload_date", "min_taken_date", "max_taken_date"]:  # yapf: disable
                 val = kwargs[key]
                 if isinstance(val, datetime.date):
-                    params[key] = val.strftime('%Y-%m-%d')
+                    params[key] = val.strftime("%Y-%m-%d")
                 elif isinstance(val, (int, str)):
                     params[key] = val
                 else:
-                    self.logger.error('%s is invalid', key)
+                    self.logger.error("%s is invalid", key)
             else:
-                self.logger.error('Unrecognized search param: %s', key)
+                self.logger.error("Unrecognized search param: %s", key)
         url = base_url + urlencode(params)
-        per_page = params.get('per_page', 100)
-        page = params.get('page', 1)
+        per_page = params.get("per_page", 100)
+        page = params.get("page", 1)
         page_max = int(math.ceil(4000.0 / per_page))
         for i in range(page, page + page_max):
-            if self.signal.get('reach_max_num'):
+            if self.signal.get("reach_max_num"):
                 break
-            complete_url = '{}&page={}'.format(url, i)
+            complete_url = f"{url}&page={i}"
             while True:
                 try:
                     self.output(complete_url, block=True)
                 except:
-                    if self.signal.get('reach_max_num'):
+                    if self.signal.get("reach_max_num"):
                         break
                 else:
                     break
-            self.logger.debug('put url to url_queue: {}'.format(complete_url))
+            self.logger.debug(f"put url to url_queue: {complete_url}")
 
 
 class FlickrParser(Parser):
-
     def parse(self, response, apikey, size_preference=None):
-        content = json.loads(response.content.decode('utf-8', 'ignore'))
-        if content['stat'] != 'ok':
+        content = json.loads(response.content.decode("utf-8", "ignore"))
+        if content["stat"] != "ok":
             return
-        photos = content['photos']['photo']
+        photos = content["photos"]["photo"]
         for photo in photos:
-            photo_id = photo['id']
-            base_url = 'https://api.flickr.com/services/rest/?'
+            photo_id = photo["id"]
+            base_url = "https://api.flickr.com/services/rest/?"
             params = {
-                'method': 'flickr.photos.getSizes',
-                'api_key': apikey,
-                'photo_id': photo_id,
-                'format': 'json',
-                'nojsoncallback': 1
+                "method": "flickr.photos.getSizes",
+                "api_key": apikey,
+                "photo_id": photo_id,
+                "format": "json",
+                "nojsoncallback": 1,
             }
             try:
                 ret = self.session.get(base_url + urlencode(params))
                 info = json.loads(ret.content.decode())
             except:
                 continue
             else:
-                if info['stat'] == 'ok':
-                    urls = {
-                        str(item['label']).lower(): item['source']
-                        for item in info['sizes']['size']
-                    }
+                if info["stat"] == "ok":
+                    urls = {str(item["label"]).lower(): item["source"] for item in info["sizes"]["size"]}
                 else:
                     continue
                 for sz in size_preference:
                     if sz in urls:
                         yield dict(file_url=urls[sz], meta=photo)
                         break
 
 
 class FlickrImageCrawler(Crawler):
-
-    def __init__(self,
-                 apikey=None,
-                 feeder_cls=FlickrFeeder,
-                 parser_cls=FlickrParser,
-                 downloader_cls=ImageDownloader,
-                 *args,
-                 **kwargs):
+    def __init__(
+        self,
+        apikey=None,
+        feeder_cls=FlickrFeeder,
+        parser_cls=FlickrParser,
+        downloader_cls=ImageDownloader,
+        *args,
+        **kwargs,
+    ):
         if apikey is None:
-            apikey = os.getenv('FLICKR_APIKEY')
+            apikey = os.getenv("FLICKR_APIKEY")
             if not apikey:
-                raise RuntimeError('apikey is not specified')
+                raise RuntimeError("apikey is not specified")
         self.apikey = apikey
-        super(FlickrImageCrawler, self).__init__(
-            feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
+        super().__init__(feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
 
-    def crawl(self,
-              max_num=1000,
-              size_preference=None,
-              min_size=None,
-              max_size=None,
-              file_idx_offset=0,
-              overwrite=False,
-              **kwargs):
-        kwargs['apikey'] = self.apikey
+    def crawl(
+        self,
+        max_num=1000,
+        size_preference=None,
+        min_size=None,
+        max_size=None,
+        file_idx_offset=0,
+        overwrite=False,
+        **kwargs,
+    ):
+        kwargs["apikey"] = self.apikey
 
         default_order = [
-            'original', 'large 2048', 'large 1600', 'large', 'medium 800',
-            'medium 640', 'medium', 'small 320', 'small', 'thumbnail',
-            'large Square', 'square'
+            "original",
+            "large 2048",
+            "large 1600",
+            "large",
+            "medium 800",
+            "medium 640",
+            "medium",
+            "small 320",
+            "small",
+            "thumbnail",
+            "large Square",
+            "square",
         ]
         if size_preference is None:
             size_preference = default_order
         elif isinstance(size_preference, str):
             assert size_preference in default_order
             size_preference = [size_preference]
         else:
             for sz in size_preference:
                 assert sz in default_order
-        super(FlickrImageCrawler, self).crawl(
+        super().crawl(
             feeder_kwargs=kwargs,
-            parser_kwargs=dict(
-                apikey=self.apikey, size_preference=size_preference),
+            parser_kwargs=dict(apikey=self.apikey, size_preference=size_preference),
             downloader_kwargs=dict(
                 max_num=max_num,
                 min_size=min_size,
                 max_size=max_size,
                 file_idx_offset=file_idx_offset,
-                overwrite=overwrite))
+                overwrite=overwrite,
+            ),
+        )
```

### Comparing `icrawler-0.6.6/icrawler/builtin/greedy.py` & `icrawler-0.6.7/icrawler/builtin/greedy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,95 @@
-# -*- coding: utf-8 -*-
-
 import re
 import time
+from urllib.parse import urljoin, urlsplit
 
 from bs4 import BeautifulSoup
-from six.moves.urllib.parse import urljoin, urlsplit
 
-from icrawler import Crawler, Feeder, Parser, ImageDownloader
+from .. import Crawler, Feeder, ImageDownloader, Parser
 
 
 class GreedyFeeder(Feeder):
-
     def feed(self, domains):
         for domain in domains:
             self.output(domain)
-        while not self.signal.get('reach_max_num'):
+        while not self.signal.get("reach_max_num"):
             time.sleep(1)
 
 
 class GreedyParser(Parser):
-
     def __init__(self, *args, **kwargs):
-        self.pattern = re.compile(
-            r'(http|\/\/)(.*)\.(jpg|jpeg|png|bmp|gif|tiff)')
-        super(GreedyParser, self).__init__(*args, **kwargs)
+        self.pattern = re.compile(r"(http|\/\/)(.*)\.(jpg|jpeg|png|bmp|gif|tiff)")
+        super().__init__(*args, **kwargs)
 
     def is_in_domain(self, url, domains):
         for domain in domains:
             if domain in url:
                 return True
         return False
 
     def parse(self, response, domains):
-        soup = BeautifulSoup(
-            response.content.decode('utf-8', 'ignore'), 'lxml')
-        tags = soup.find_all('img', src=True)
+        soup = BeautifulSoup(response.content.decode("utf-8", "ignore"), "lxml")
+        tags = soup.find_all("img", src=True)
         for tag in tags:
-            if re.match(self.pattern, tag['src']):
-                if tag['src'].startswith('//'):
-                    img_url = 'http:' + tag['src']
+            if re.match(self.pattern, tag["src"]):
+                if tag["src"].startswith("//"):
+                    img_url = "http:" + tag["src"]
                 else:
-                    img_url = tag['src']
+                    img_url = tag["src"]
                 yield dict(file_url=img_url)
         tags = soup.find_all(href=True)
-        base_url = '{0.scheme}://{0.netloc}'.format(urlsplit(response.url))
+        base_url = "{0.scheme}://{0.netloc}".format(urlsplit(response.url))
         for tag in tags:
-            href = tag['href']
+            href = tag["href"]
             # deal with urls start with '//' or '/' or '#'
             if len(href) < 2:
                 continue
-            if href[0:2] == '//':
-                href = 'http:' + href.rstrip('/')
-            elif href[0] == '/':
-                href = urljoin(base_url, href.strip('/'))
-            elif href[0] == '#':
+            if href[0:2] == "//":
+                href = "http:" + href.rstrip("/")
+            elif href[0] == "/":
+                href = urljoin(base_url, href.strip("/"))
+            elif href[0] == "#":
                 continue
             else:
-                href = urljoin(base_url, href.rstrip('/'))
+                href = urljoin(base_url, href.rstrip("/"))
             # if it is a image url
             if re.match(self.pattern, href):
                 yield dict(file_url=href)
             else:
                 # discard urls such as 'www.example.com/file.zip'
                 # TODO: deal with '#' in the urls
-                tmp = href.split('/')[-1].split('.')
-                if len(tmp) > 1 and tmp[-1] not in [
-                        'html', 'shtml', 'shtm', 'php', 'jsp', 'asp'
-                ]:
+                tmp = href.split("/")[-1].split(".")
+                if len(tmp) > 1 and tmp[-1] not in ["html", "shtml", "shtm", "php", "jsp", "asp"]:
                     continue
                 # discard urls such as 'javascript:void(0)'
-                elif href.find('javascript', 0, 10) == 0:
+                elif href.find("javascript", 0, 10) == 0:
                     continue
                 # discard urls such as 'android-app://xxxxxxxxx'
-                elif urlsplit(href).scheme not in ['http', 'https', 'ftp']:
+                elif urlsplit(href).scheme not in ["http", "https", "ftp"]:
                     continue
                 # urls of the same domain
                 elif self.is_in_domain(href, domains):
                     yield href
 
 
 class GreedyImageCrawler(Crawler):
+    def __init__(
+        self, feeder_cls=GreedyFeeder, parser_cls=GreedyParser, downloader_cls=ImageDownloader, *args, **kwargs
+    ):
+        super().__init__(feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
 
-    def __init__(self,
-                 feeder_cls=GreedyFeeder,
-                 parser_cls=GreedyParser,
-                 downloader_cls=ImageDownloader,
-                 *args,
-                 **kwargs):
-        super(GreedyImageCrawler, self).__init__(
-            feeder_cls, parser_cls, downloader_cls, *args, **kwargs)
-
-    def crawl(self,
-              domains,
-              max_num=0,
-              min_size=None,
-              max_size=None,
-              file_idx_offset=0):
+    def crawl(self, domains, max_num=0, min_size=None, max_size=None, file_idx_offset=0):
         if isinstance(domains, str):
             domains = [domains]
         elif not isinstance(domains, list):
-            self.logger.error('domains must be a string or a list')
+            self.logger.error("domains must be a string or a list")
         for i in range(len(domains)):
-            if not domains[i].startswith('http'):
-                domains[i] = 'http://' + domains[i]
-            domains[i] = domains[i].rstrip('/')
-        super(GreedyImageCrawler, self).crawl(
-            feeder_kwargs={'domains': domains},
-            parser_kwargs={'domains': domains},
+            if not domains[i].startswith("http"):
+                domains[i] = "http://" + domains[i]
+            domains[i] = domains[i].rstrip("/")
+        super().crawl(
+            feeder_kwargs={"domains": domains},
+            parser_kwargs={"domains": domains},
             downloader_kwargs=dict(
-                max_num=max_num,
-                min_size=min_size,
-                max_size=max_size,
-                file_idx_offset=file_idx_offset))
+                max_num=max_num, min_size=min_size, max_size=max_size, file_idx_offset=file_idx_offset
+            ),
+        )
```

### Comparing `icrawler-0.6.6/icrawler/crawler.py` & `icrawler-0.6.7/icrawler/crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# -*- coding: utf-8 -*-
 """Crawler base class"""
 
 import logging
 import sys
 import time
 from importlib import import_module
 
-from icrawler import Downloader, Feeder, Parser
-from icrawler import storage as storage_package
-from icrawler.storage import BaseStorage
-from icrawler.utils import ProxyPool, Session, Signal
+from . import storage as storage_package
+from .downloader import Downloader
+from .feeder import Feeder
+from .parser import Parser
+from .storage import BaseStorage
+from .utils import ProxyPool, Session, Signal
 
 
-class Crawler(object):
+class Crawler:
     """Base class for crawlers
 
     Attributes:
         session (Session): A Session object.
         feeder (Feeder): A Feeder object.
         parser (Parser): A Parser object.
         downloader (Downloader): A Downloader object.
         signal (Signal): A Signal object shared by all components,
                          used for communication among threads
         logger (Logger): A Logger object used for logging
     """
 
-    def __init__(self,
-                 feeder_cls=Feeder,
-                 parser_cls=Parser,
-                 downloader_cls=Downloader,
-                 feeder_threads=1,
-                 parser_threads=1,
-                 downloader_threads=1,
-                 storage={
-                     'backend': 'FileSystem',
-                     'root_dir': 'images'
-                 },
-                 log_level=logging.INFO,
-                 extra_feeder_args=None,
-                 extra_parser_args=None,
-                 extra_downloader_args=None):
+    def __init__(
+        self,
+        feeder_cls=Feeder,
+        parser_cls=Parser,
+        downloader_cls=Downloader,
+        feeder_threads=1,
+        parser_threads=1,
+        downloader_threads=1,
+        storage={"backend": "FileSystem", "root_dir": "images"},
+        log_level=logging.INFO,
+        extra_feeder_args=None,
+        extra_parser_args=None,
+        extra_downloader_args=None,
+    ):
         """Init components with class names and other arguments.
 
         Args:
             feeder_cls: class of feeder
             parser_cls: class of parser
             downloader_cls: class of downloader.
             feeder_threads: thread number used by feeder
@@ -57,70 +57,64 @@
         self.set_proxy_pool()
         self.set_session()
         self.init_signal()
         self.set_storage(storage)
         # set feeder, parser and downloader
         feeder_kwargs = {} if extra_feeder_args is None else extra_feeder_args
         parser_kwargs = {} if extra_parser_args is None else extra_parser_args
-        downloader_kwargs = ({} if extra_downloader_args is None else
-                             extra_downloader_args)
-        self.feeder = feeder_cls(feeder_threads, self.signal, self.session,
-                                 **feeder_kwargs)
-        self.parser = parser_cls(parser_threads, self.signal, self.session,
-                                 **parser_kwargs)
-        self.downloader = downloader_cls(downloader_threads, self.signal,
-                                         self.session, self.storage,
-                                         **downloader_kwargs)
+        downloader_kwargs = {} if extra_downloader_args is None else extra_downloader_args
+        self.feeder = feeder_cls(feeder_threads, self.signal, self.session, **feeder_kwargs)
+        self.parser = parser_cls(parser_threads, self.signal, self.session, **parser_kwargs)
+        self.downloader = downloader_cls(
+            downloader_threads, self.signal, self.session, self.storage, **downloader_kwargs
+        )
         # connect all components
         self.feeder.connect(self.parser).connect(self.downloader)
 
     def set_logger(self, log_level=logging.INFO):
         """Configure the logger with log_level."""
         logging.basicConfig(
-            format='%(asctime)s - %(levelname)s - %(name)s - %(message)s',
-            level=log_level,
-            stream=sys.stderr)
+            format="%(asctime)s - %(levelname)s - %(name)s - %(message)s", level=log_level, stream=sys.stderr
+        )
         self.logger = logging.getLogger(__name__)
-        logging.getLogger('requests').setLevel(logging.WARNING)
+        logging.getLogger("requests").setLevel(logging.WARNING)
 
     def init_signal(self):
         """Init signal
 
         3 signals are added: ``feeder_exited``, ``parser_exited`` and
         ``reach_max_num``.
         """
         self.signal = Signal()
-        self.signal.set(
-            feeder_exited=False, parser_exited=False, reach_max_num=False)
+        self.signal.set(feeder_exited=False, parser_exited=False, reach_max_num=False)
 
     def set_storage(self, storage):
         """Set storage backend for downloader
 
         For full list of storage backend supported, please see :mod:`storage`.
 
         Args:
             storage (dict or BaseStorage): storage backend configuration or instance
 
         """
         if isinstance(storage, BaseStorage):
             self.storage = storage
         elif isinstance(storage, dict):
-            if 'backend' not in storage and 'root_dir' in storage:
-                storage['backend'] = 'FileSystem'
+            if "backend" not in storage and "root_dir" in storage:
+                storage["backend"] = "FileSystem"
             try:
-                backend_cls = getattr(storage_package, storage['backend'])
+                backend_cls = getattr(storage_package, storage["backend"])
             except AttributeError:
                 try:
-                    backend_cls = import_module(storage['backend'])
+                    backend_cls = import_module(storage["backend"])
                 except ImportError:
-                    self.logger.error('cannot find backend module %s',
-                                      storage['backend'])
+                    self.logger.error("cannot find backend module %s", storage["backend"])
                     sys.exit()
             kwargs = storage.copy()
-            del kwargs['backend']
+            del kwargs["backend"]
             self.storage = backend_cls(**kwargs)
         else:
             raise TypeError('"storage" must be a storage object or dict')
 
     def set_proxy_pool(self, pool=None):
         """Construct a proxy pool
 
@@ -136,57 +130,52 @@
 
         Args:
             headers: A dict of headers (default None, thus using the default
                      header to init the session)
         """
         if headers is None:
             headers = {
-                'User-Agent':
-                ('Mozilla/5.0 (Windows NT 10.0; Win64; x64)'
-                 ' AppleWebKit/537.36 (KHTML, like Gecko) '
-                 'Chrome/88.0.4324.104 Safari/537.36')
+                "User-Agent": (
+                    "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
+                    " AppleWebKit/537.36 (KHTML, like Gecko) "
+                    "Chrome/88.0.4324.104 Safari/537.36"
+                )
             }
         elif not isinstance(headers, dict):
             raise TypeError('"headers" must be a dict object')
 
         self.session = Session(self.proxy_pool)
         self.session.headers.update(headers)
 
-    def crawl(self,
-              feeder_kwargs=None,
-              parser_kwargs=None,
-              downloader_kwargs=None):
+    def crawl(self, feeder_kwargs=None, parser_kwargs=None, downloader_kwargs=None):
         """Start crawling
 
         This method will start feeder, parser and download and wait
         until all threads exit.
 
         Args:
             feeder_kwargs (dict, optional): Arguments to be passed to ``feeder.start()``
             parser_kwargs (dict, optional): Arguments to be passed to ``parser.start()``
             downloader_kwargs (dict, optional): Arguments to be passed to
                 ``downloader.start()``
         """
         self.signal.reset()
-        self.logger.info('start crawling...')
+        self.logger.info("start crawling...")
 
         feeder_kwargs = {} if feeder_kwargs is None else feeder_kwargs
         parser_kwargs = {} if parser_kwargs is None else parser_kwargs
         downloader_kwargs = {} if downloader_kwargs is None else downloader_kwargs
 
-        self.logger.info('starting %d feeder threads...',
-                         self.feeder.thread_num)
+        self.logger.info("starting %d feeder threads...", self.feeder.thread_num)
         self.feeder.start(**feeder_kwargs)
 
-        self.logger.info('starting %d parser threads...',
-                         self.parser.thread_num)
+        self.logger.info("starting %d parser threads...", self.parser.thread_num)
         self.parser.start(**parser_kwargs)
 
-        self.logger.info('starting %d downloader threads...',
-                         self.downloader.thread_num)
+        self.logger.info("starting %d downloader threads...", self.downloader.thread_num)
         self.downloader.start(**downloader_kwargs)
 
         while True:
             if not self.feeder.is_alive():
                 self.signal.set(feeder_exited=True)
             if not self.parser.is_alive():
                 self.signal.set(parser_exited=True)
@@ -197,8 +186,8 @@
         if not self.feeder.in_queue.empty():
             self.feeder.clear_buffer()
         if not self.parser.in_queue.empty():
             self.parser.clear_buffer()
         if not self.downloader.in_queue.empty():
             self.downloader.clear_buffer(True)
 
-        self.logger.info('Crawling task done!')
+        self.logger.info("Crawling task done!")
```

### Comparing `icrawler-0.6.6/icrawler/downloader.py` & `icrawler-0.6.7/icrawler/downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-
+import queue
+from io import BytesIO
 from threading import current_thread
+from urllib.parse import urlparse
 
 from PIL import Image
-from six import BytesIO
-from six.moves import queue
-from six.moves.urllib.parse import urlparse
 
-from icrawler.utils import ThreadPool
+from .utils import ThreadPool
 
 
 class Downloader(ThreadPool):
     """Base class for downloader.
 
     A thread pool of downloader threads, in charge of downloading files and
     saving them in the corresponding paths.
@@ -26,16 +24,15 @@
         thread_num (int): The number of downloader threads.
         lock (Lock): A threading.Lock object.
         storage (BaseStorage): storage backend.
     """
 
     def __init__(self, thread_num, signal, session, storage):
         """Init Parser with some shared variables."""
-        super(Downloader, self).__init__(
-            thread_num, out_queue=None, name='downloader')
+        super().__init__(thread_num, out_queue=None, name="downloader")
         self.signal = signal
         self.session = session
         self.storage = storage
         self.file_idx_offset = 0
         self.clear_status()
 
     def clear_status(self):
@@ -49,15 +46,15 @@
             file_idx_offset: It can be either an integer or 'auto'. If set
                 to an integer, the filename will start from
                 ``file_idx_offset`` + 1. If set to ``'auto'``, the filename
                 will start from existing max file index plus 1.
         """
         if isinstance(file_idx_offset, int):
             self.file_idx_offset = file_idx_offset
-        elif file_idx_offset == 'auto':
+        elif file_idx_offset == "auto":
             self.file_idx_offset = self.storage.max_file_idx()
         else:
             raise ValueError('"file_idx_offset" must be an integer or `auto`')
 
     def get_filename(self, task, default_ext):
         """Set the path where the image will be saved.
 
@@ -68,88 +65,84 @@
 
         Args:
             task (dict): The task dict got from ``task_queue``.
 
         Output:
             Filename with extension.
         """
-        url_path = urlparse(task['file_url'])[2]
-        extension = url_path.split('.')[-1] if '.' in url_path else default_ext
+        url_path = urlparse(task["file_url"])[2]
+        extension = url_path.split(".")[-1] if "." in url_path else default_ext
         file_idx = self.fetched_num + self.file_idx_offset
-        return '{:06d}.{}'.format(file_idx, extension)
+        return f"{file_idx:06d}.{extension}"
 
     def reach_max_num(self):
         """Check if downloaded images reached max num.
 
         Returns:
             bool: if downloaded images reached max num.
         """
-        if self.signal.get('reach_max_num'):
+        if self.signal.get("reach_max_num"):
             return True
         if self.max_num > 0 and self.fetched_num >= self.max_num:
             return True
         else:
             return False
 
     def keep_file(self, task, response, **kwargs):
         return True
 
-    def download(self,
-                 task,
-                 default_ext,
-                 timeout=5,
-                 max_retry=3,
-                 overwrite=False,
-                 **kwargs):
+    def download(self, task, default_ext, timeout=5, max_retry=3, overwrite=False, **kwargs):
         """Download the image and save it to the corresponding path.
 
         Args:
             task (dict): The task dict got from ``task_queue``.
             timeout (int): Timeout of making requests for downloading images.
             max_retry (int): the max retry times if the request fails.
             **kwargs: reserved arguments for overriding.
         """
-        file_url = task['file_url']
-        task['success'] = False
-        task['filename'] = None
+        file_url = task["file_url"]
+        task["success"] = False
+        task["filename"] = None
         retry = max_retry
 
         if not overwrite:
             with self.lock:
                 self.fetched_num += 1
                 filename = self.get_filename(task, default_ext)
                 if self.storage.exists(filename):
-                    self.logger.info('skip downloading file %s', filename)
+                    self.logger.info("skip downloading file %s", filename)
                     return
                 self.fetched_num -= 1
 
-        while retry > 0 and not self.signal.get('reach_max_num'):
+        while retry > 0 and not self.signal.get("reach_max_num"):
             try:
                 response = self.session.get(file_url, timeout=timeout)
             except Exception as e:
-                self.logger.error('Exception caught when downloading file %s, '
-                                  'error: %s, remaining retry times: %d',
-                                  file_url, e, retry - 1)
+                self.logger.error(
+                    "Exception caught when downloading file %s, " "error: %s, remaining retry times: %d",
+                    file_url,
+                    e,
+                    retry - 1,
+                )
             else:
                 if self.reach_max_num():
                     self.signal.set(reach_max_num=True)
                     break
                 elif response.status_code != 200:
-                    self.logger.error('Response status code %d, file %s',
-                                      response.status_code, file_url)
+                    self.logger.error("Response status code %d, file %s", response.status_code, file_url)
                     break
                 elif not self.keep_file(task, response, **kwargs):
                     break
                 with self.lock:
                     self.fetched_num += 1
                     filename = self.get_filename(task, default_ext)
-                self.logger.info('image #%s\t%s', self.fetched_num, file_url)
+                self.logger.info("image #%s\t%s", self.fetched_num, file_url)
                 self.storage.write(filename, response.content)
-                task['success'] = True
-                task['filename'] = filename
+                task["success"] = True
+                task["filename"] = filename
                 break
             finally:
                 retry -= 1
 
     def process_meta(self, task):
         """Process some meta data of the images.
 
@@ -164,22 +157,17 @@
 
     def start(self, file_idx_offset=0, *args, **kwargs):
         self.clear_status()
         self.set_file_idx_offset(file_idx_offset)
         self.init_workers(*args, **kwargs)
         for worker in self.workers:
             worker.start()
-            self.logger.debug('thread %s started', worker.name)
+            self.logger.debug("thread %s started", worker.name)
 
-    def worker_exec(self,
-                    max_num,
-                    default_ext='',
-                    queue_timeout=5,
-                    req_timeout=5,
-                    **kwargs):
+    def worker_exec(self, max_num, default_ext="", queue_timeout=5, req_timeout=5, **kwargs):
         """Target method of workers.
 
         Get task from ``task_queue`` and then download files and process meta
         data. A downloader thread will exit in either of the following cases:
 
         1. All parser threads have exited and the task_queue is empty.
         2. Downloaded image number has reached required number(max_num).
@@ -187,45 +175,41 @@
         Args:
             queue_timeout (int): Timeout of getting tasks from ``task_queue``.
             req_timeout (int): Timeout of making requests for downloading pages.
             **kwargs: Arguments passed to the :func:`download` method.
         """
         self.max_num = max_num
         while True:
-            if self.signal.get('reach_max_num'):
-                self.logger.info('downloaded images reach max num, thread %s'
-                                 ' is ready to exit',
-                                 current_thread().name)
+            if self.signal.get("reach_max_num"):
+                self.logger.info(
+                    "downloaded images reach max num, thread %s" " is ready to exit", current_thread().name
+                )
                 break
             try:
                 task = self.in_queue.get(timeout=queue_timeout)
             except queue.Empty:
-                if self.signal.get('parser_exited'):
-                    self.logger.info('no more download task for thread %s',
-                                     current_thread().name)
+                if self.signal.get("parser_exited"):
+                    self.logger.info("no more download task for thread %s", current_thread().name)
                     break
                 else:
-                    self.logger.info('%s is waiting for new download tasks',
-                                     current_thread().name)
+                    self.logger.info("%s is waiting for new download tasks", current_thread().name)
             except:
-                self.logger.error('exception in thread %s',
-                                  current_thread().name)
+                self.logger.error("exception in thread %s", current_thread().name)
             else:
                 self.download(task, default_ext, req_timeout, **kwargs)
                 self.process_meta(task)
                 self.in_queue.task_done()
-        self.logger.info('thread {} exit'.format(current_thread().name))
+        self.logger.info(f"thread {current_thread().name} exit")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.logger.info('all downloader threads exited')
+        self.logger.info("all downloader threads exited")
 
 
 class ImageDownloader(Downloader):
-    """Downloader specified for images.
-    """
+    """Downloader specified for images."""
 
     def _size_lt(self, sz1, sz2):
         return max(sz1) <= max(sz2) and min(sz1) <= min(sz2)
 
     def _size_gt(self, sz1, sz2):
         return max(sz1) >= max(sz2) and min(sz1) >= min(sz2)
 
@@ -239,37 +223,29 @@
             min_size (tuple or None): minimum size of required images.
             max_size (tuple or None): maximum size of required images.
         Returns:
             bool: whether to keep the image.
         """
         try:
             img = Image.open(BytesIO(response.content))
-        except (IOError, OSError):
+        except OSError:
             return False
-        task['img_size'] = img.size
+        task["img_size"] = img.size
         if min_size and not self._size_gt(img.size, min_size):
             return False
         if max_size and not self._size_lt(img.size, max_size):
             return False
         return True
 
     def get_filename(self, task, default_ext):
-        url_path = urlparse(task['file_url'])[2]
-        if '.' in url_path:
-            extension = url_path.split('.')[-1]
-            if extension.lower() not in [
-                    'jpg', 'jpeg', 'png', 'bmp', 'tiff', 'gif', 'ppm', 'pgm'
-            ]:
+        url_path = urlparse(task["file_url"])[2]
+        if "." in url_path:
+            extension = url_path.split(".")[-1]
+            if extension.lower() not in ["jpg", "jpeg", "png", "bmp", "tiff", "gif", "ppm", "pgm"]:
                 extension = default_ext
         else:
             extension = default_ext
         file_idx = self.fetched_num + self.file_idx_offset
-        return '{:06d}.{}'.format(file_idx, extension)
+        return f"{file_idx:06d}.{extension}"
 
-    def worker_exec(self,
-                    max_num,
-                    default_ext='jpg',
-                    queue_timeout=5,
-                    req_timeout=5,
-                    **kwargs):
-        super(ImageDownloader, self).worker_exec(
-            max_num, default_ext, queue_timeout, req_timeout, **kwargs)
+    def worker_exec(self, max_num, default_ext="jpg", queue_timeout=5, req_timeout=5, **kwargs):
+        super().worker_exec(max_num, default_ext, queue_timeout, req_timeout, **kwargs)
```

### Comparing `icrawler-0.6.6/icrawler/feeder.py` & `icrawler-0.6.7/icrawler/feeder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-
 import os.path as osp
 from threading import current_thread
 
-from icrawler.utils import ThreadPool
+from .utils import ThreadPool
 
 
 class Feeder(ThreadPool):
     """Base class for feeder.
 
     A thread pool of feeder threads, in charge of feeding urls to parsers.
 
@@ -22,59 +20,58 @@
         workers (list): A list storing all the threading.Thread objects
             of the feeder.
         lock (Lock): A :class:`Lock` instance shared by all feeder threads.
     """
 
     def __init__(self, thread_num, signal, session):
         """Init Feeder with some shared variables."""
-        super(Feeder, self).__init__(
-            thread_num=thread_num, in_queue=None, name='feeder')
+        super().__init__(thread_num=thread_num, in_queue=None, name="feeder")
         self.signal = signal
         self.session = session
 
     def feed(self, **kwargs):
         """Feed urls.
 
         This method should be implemented by users.
         """
         raise NotImplementedError
 
     def worker_exec(self, **kwargs):
         """Target function of workers"""
         self.feed(**kwargs)
-        self.logger.info('thread {} exit'.format(current_thread().name))
+        self.logger.info(f"thread {current_thread().name} exit")
 
     def __exit__(self):
-        self.logger.info('all feeder threads exited')
+        self.logger.info("all feeder threads exited")
 
 
 class UrlListFeeder(Feeder):
     """Url list feeder which feed a list of urls"""
 
     def feed(self, url_list, offset=0, max_num=0):
         if isinstance(url_list, str):
             if osp.isfile(url_list):
-                with open(url_list, 'r') as fin:
-                    url_list = [line.rstrip('\n') for line in fin]
+                with open(url_list) as fin:
+                    url_list = [line.rstrip("\n") for line in fin]
             else:
-                raise IOError('url list file {} not found'.format(url_list))
+                raise OSError(f"url list file {url_list} not found")
         elif not isinstance(url_list, list):
             raise TypeError('"url_list" can only be a filename or a str list')
 
         if offset < 0 or offset >= len(url_list):
             raise ValueError('"offset" exceed the list length')
         else:
             if max_num > 0:
                 end_idx = min(len(url_list), offset + max_num)
             else:
                 end_idx = len(url_list)
             for i in range(offset, end_idx):
                 url = url_list[i]
                 self.out_queue.put(url)
-                self.logger.debug('put url to url_queue: {}'.format(url))
+                self.logger.debug(f"put url to url_queue: {url}")
 
 
 class SimpleSEFeeder(Feeder):
     """Simple search engine like Feeder"""
 
     def feed(self, url_template, keyword, offset, max_num, page_step):
         """Feed urls once
@@ -85,8 +82,8 @@
             offset: An integer indicating the starting index.
             max_num: An integer indicating the max number of images to be crawled.
             page_step: An integer added to offset after each iteration.
         """
         for i in range(offset, offset + max_num, page_step):
             url = url_template.format(keyword, i)
             self.out_queue.put(url)
-            self.logger.debug('put url to url_queue: {}'.format(url))
+            self.logger.debug(f"put url to url_queue: {url}")
```

### Comparing `icrawler-0.6.6/icrawler/parser.py` & `icrawler-0.6.7/icrawler/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# -*- coding: utf-8 -*-
-
 import logging
+import queue
 import time
 from threading import current_thread
+from urllib.parse import urlsplit
 
-from six.moves import queue
-from six.moves.urllib.parse import urlsplit
-
-from icrawler.utils import ThreadPool
+from .utils import ThreadPool
 
 
 class Parser(ThreadPool):
     """Base class for parser.
 
     A thread pool of parser threads, in charge of downloading and parsing pages,
     extracting file urls and put them into the input queue of downloader.
@@ -23,35 +20,31 @@
         threads: A list storing all the threading.Thread objects of the parser.
         thread_num: An integer indicating the number of threads.
         lock: A threading.Lock object.
     """
 
     def __init__(self, thread_num, signal, session):
         """Init Parser with some shared variables."""
-        super(Parser, self).__init__(thread_num, name='parser')
+        super().__init__(thread_num, name="parser")
         self.signal = signal
         self.session = session
 
     def parse(self, response, **kwargs):
         """Parse a page and extract image urls, then put it into task_queue.
 
         This method should be overridden by users.
 
         :Example:
 
         >>> task = {}
-        >>> self.output(task)
+        >>> self.output(task)  # doctest: +SKIP
         """
         raise NotImplementedError
 
-    def worker_exec(self,
-                    queue_timeout=2,
-                    req_timeout=5,
-                    max_retry=3,
-                    **kwargs):
+    def worker_exec(self, queue_timeout=2, req_timeout=5, max_retry=3, **kwargs):
         """Target method of workers.
 
         Firstly download the page and then call the :func:`parse` method.
         A parser thread will exit in either of the following cases:
 
         1. All feeder threads have exited and the ``url_queue`` is empty.
         2. Downloaded image number has reached required number.
@@ -59,73 +52,70 @@
         Args:
             queue_timeout (int): Timeout of getting urls from ``url_queue``.
             req_timeout (int): Timeout of making requests for downloading pages.
             max_retry (int): Max retry times if the request fails.
             **kwargs: Arguments to be passed to the :func:`parse` method.
         """
         while True:
-            if self.signal.get('reach_max_num'):
-                self.logger.info('downloaded image reached max num, thread %s '
-                                 'is ready to exit', current_thread().name)
+            if self.signal.get("reach_max_num"):
+                self.logger.info(
+                    "downloaded image reached max num, thread %s " "is ready to exit", current_thread().name
+                )
                 break
             # get the page url
             try:
                 url = self.in_queue.get(timeout=queue_timeout)
             except queue.Empty:
-                if self.signal.get('feeder_exited'):
-                    self.logger.info(
-                        'no more page urls for thread %s to parse',
-                        current_thread().name)
+                if self.signal.get("feeder_exited"):
+                    self.logger.info("no more page urls for thread %s to parse", current_thread().name)
                     break
                 else:
-                    self.logger.info('%s is waiting for new page urls',
-                                     current_thread().name)
+                    self.logger.info("%s is waiting for new page urls", current_thread().name)
                     continue
             except:
-                self.logger.error('exception in thread %s',
-                                  current_thread().name)
+                self.logger.error("exception in thread %s", current_thread().name)
                 continue
             else:
-                self.logger.debug('start fetching page {}'.format(url))
+                self.logger.debug(f"start fetching page {url}")
             # fetch and parse the page
             retry = max_retry
             while retry > 0:
                 try:
-                    base_url = '{0.scheme}://{0.netloc}'.format(urlsplit(url))
-                    response = self.session.get(url,
-                                                timeout=req_timeout,
-                                                headers={'Referer': base_url})
+                    base_url = "{0.scheme}://{0.netloc}".format(urlsplit(url))
+                    response = self.session.get(url, timeout=req_timeout, headers={"Referer": base_url})
                 except Exception as e:
                     self.logger.error(
-                        'Exception caught when fetching page %s, '
-                        'error: %s, remaining retry times: %d', url, e,
-                        retry - 1)
+                        "Exception caught when fetching page %s, " "error: %s, remaining retry times: %d",
+                        url,
+                        e,
+                        retry - 1,
+                    )
                 else:
-                    self.logger.info('parsing result page {}'.format(url))
+                    self.logger.info(f"parsing result page {url}")
                     for task in self.parse(response, **kwargs):
-                        while not self.signal.get('reach_max_num'):
+                        while not self.signal.get("reach_max_num"):
                             try:
                                 if isinstance(task, dict):
                                     self.output(task, timeout=1)
                                 elif isinstance(task, str):
                                     # this case only work for GreedyCrawler,
                                     # which need to feed the url back to
                                     # url_queue, dirty implementation
                                     self.input(task, timeout=1)
                             except queue.Full:
                                 time.sleep(1)
                             except Exception as e:
                                 self.logger.error(
-                                    'Exception caught when put task %s into '
-                                    'queue, error: %s', task, url)
+                                    "Exception caught when put task %s into " "queue, error: %s", task, url
+                                )
                             else:
                                 break
-                        if self.signal.get('reach_max_num'):
+                        if self.signal.get("reach_max_num"):
                             break
                     self.in_queue.task_done()
                     break
                 finally:
                     retry -= 1
-        self.logger.info('thread {} exit'.format(current_thread().name))
+        self.logger.info(f"thread {current_thread().name} exit")
 
     def __exit__(self):
-        logging.info('all parser threads exited')
+        logging.info("all parser threads exited")
```

### Comparing `icrawler-0.6.6/icrawler/storage/base.py` & `icrawler-0.6.7/icrawler/storage/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-
 from abc import ABCMeta, abstractmethod
 
 
-class BaseStorage(object):
+class BaseStorage:
     """Base class of backend storage"""
 
     __metaclass__ = ABCMeta
 
     @abstractmethod
     def write(self, id, data):
         """Abstract interface of writing data
```

### Comparing `icrawler-0.6.6/icrawler/storage/filesystem.py` & `icrawler-0.6.7/icrawler/storage/filesystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# -*- coding: utf-8 -*-
-
 import os
 import os.path as osp
 
 import six
 
-from icrawler.storage import BaseStorage
+from .base import BaseStorage
 
 
 class FileSystem(BaseStorage):
     """Use filesystem as storage backend.
 
     The id is filename and data is stored as text files or binary files.
     """
@@ -21,15 +19,15 @@
         filepath = osp.join(self.root_dir, id)
         folder = osp.dirname(filepath)
         if not osp.isdir(folder):
             try:
                 os.makedirs(folder)
             except OSError:
                 pass
-        mode = 'w' if isinstance(data, six.string_types) else 'wb'
+        mode = "w" if isinstance(data, str) else "wb"
         with open(filepath, mode) as fout:
             fout.write(data)
 
     def exists(self, id):
         return osp.exists(osp.join(self.root_dir, id))
 
     def max_file_idx(self):
```

### Comparing `icrawler-0.6.6/icrawler/storage/google_storage.py` & `icrawler-0.6.7/icrawler/storage/google_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-from icrawler.storage import BaseStorage
 from io import BytesIO
 
+from .base import BaseStorage
+
 
 class GoogleStorage(BaseStorage):
     """Google Storage backend.
 
     The id is filename and data is stored as text files or binary files.
     The root_dir is the bucket address such as gs://<your_bucket>/<your_directory>.
     """
 
     def __init__(self, root_dir):
         try:
             from google.cloud import storage
         except ImportError:
-            print('GoogleStorage backend requires the package '
-                  '"google-cloud-storage", execute '
-                  '"pip install google-cloud-storage" to install it.')
+            print(
+                "GoogleStorage backend requires the package "
+                '"google-cloud-storage", execute '
+                '"pip install google-cloud-storage" to install it.'
+            )
 
         self.client = storage.Client()
-        bucket_str = root_dir[5:].split('/')[0]
+        bucket_str = root_dir[5:].split("/")[0]
         self.bucket = self.client.get_bucket(bucket_str)
-        self.folder_str = root_dir[6 + len(bucket_str):]
-        if self.folder_str[0] == '/':
+        self.folder_str = root_dir[6 + len(bucket_str) :]
+        if self.folder_str[0] == "/":
             self.folder_str = self.folder_str[1:]
 
     def write(self, id, data):
-        blob = self.bucket.blob(self.folder_str + '/' + id)
+        blob = self.bucket.blob(self.folder_str + "/" + id)
         data_buffer = BytesIO(data)
         blob.upload_from_file(file_obj=data_buffer, size=len(data))
 
     def exists(self, id):
-        blob = self.bucket.blob(self.folder_str + '/' + id)
+        blob = self.bucket.blob(self.folder_str + "/" + id)
         return blob.exists()
 
     def max_file_idx(self):
         return len(self.bucket.list_blobs(prefix=self.folder_str))
```

### Comparing `icrawler-0.6.6/icrawler/utils/cached_queue.py` & `icrawler-0.6.7/icrawler/utils/cached_queue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 from collections import OrderedDict
+from queue import Queue
 
-from six.moves.queue import Queue
 
-
-class CachedQueue(Queue, object):
+class CachedQueue(Queue):
     """Queue with cache
 
     This queue is used in :class:`ThreadPool`, it enables parser and downloader
     to check if the page url or the task has been seen or processed before.
 
     Attributes:
         _cache (OrderedDict): cache, elements are stored as keys of it.
         cache_capacity (int): maximum size of cache.
 
     """
 
     def __init__(self, *args, **kwargs):
-        super(CachedQueue, self).__init__(*args, **kwargs)
-        if 'cache_capacity' in kwargs:
-            self.cache_capacity = kwargs['cache_capacity']
+        super().__init__(*args, **kwargs)
+        if "cache_capacity" in kwargs:
+            self.cache_capacity = kwargs["cache_capacity"]
         else:
             self.cache_capacity = 0
         self._cache = OrderedDict()
 
     def is_duplicated(self, item):
         """Check whether the item has been in the cache
 
@@ -42,24 +41,22 @@
         elif isinstance(item, list):
             hashable_item = frozenset(item)
         else:
             hashable_item = item
         if hashable_item in self._cache:
             return True
         else:
-            if self.cache_capacity > 0 and len(
-                    self._cache) >= self.cache_capacity:
+            if self.cache_capacity > 0 and len(self._cache) >= self.cache_capacity:
                 self._cache.popitem(False)
             self._cache[hashable_item] = 1
             return False
 
     def put(self, item, block=True, timeout=None, dup_callback=None):
-        """Put an item to queue if it is not duplicated.
-        """
+        """Put an item to queue if it is not duplicated."""
         if not self.is_duplicated(item):
-            super(CachedQueue, self).put(item, block, timeout)
+            super().put(item, block, timeout)
         else:
             if dup_callback:
                 dup_callback(item)
 
     def put_nowait(self, item, dup_callback=None):
         self.put(item, block=False, dup_callback=dup_callback)
```

### Comparing `icrawler-0.6.6/icrawler/utils/proxy_pool.py` & `icrawler-0.6.7/icrawler/utils/proxy_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,30 @@
-# -*- coding: utf-8 -*-
-
 import json
 import logging
+import queue
 import random
 import threading
 import time
 
 import requests
 from bs4 import BeautifulSoup
 
-from six.moves import queue
-
 
-class Proxy(object):
+class Proxy:
     """Proxy class
 
     Attributes:
         addr (str): A string with IP and port, for example '123.123.123.123:8080'
         protocol (str): 'http' or 'https'
         weight (float): A float point number indicating the probability of being
             selected, the weight is based on the connection time and stability
         last_checked (time): A UNIX timestamp indicating when the proxy was checked
     """
 
-    def __init__(self,
-                 addr=None,
-                 protocol='http',
-                 weight=1.0,
-                 last_checked=None):
+    def __init__(self, addr=None, protocol="http", weight=1.0, last_checked=None):
         self.addr = addr
         self.protocol = protocol
         self.weight = weight
         if last_checked is None:
             self.last_checked = int(time.time())
         else:
             self.last_checked = last_checked
@@ -47,22 +40,18 @@
     def to_dict(self):
         """convert detailed proxy info into a dict
 
         Returns:
             dict: A dict with four keys: ``addr``, ``protocol``,
                   ``weight`` and ``last_checked``
         """
-        return dict(
-            addr=self.addr,
-            protocol=self.protocol,
-            weight=self.weight,
-            last_checked=self.last_checked)
+        return dict(addr=self.addr, protocol=self.protocol, weight=self.weight, last_checked=self.last_checked)
 
 
-class ProxyPool(object):
+class ProxyPool:
     """Proxy pool class
 
     ProxyPool provides friendly apis to manage proxies.
 
     Attributes:
         idx (dict): Index for http proxy list and https proxy list.
         test_url (dict): A dict containing two urls, when testing if a proxy
@@ -83,21 +72,18 @@
         """Init the pool from a json file.
 
         Args:
             filename (str, optional): if the filename is provided, proxies
                 will be load from it.
 
         """
-        self.idx = {'http': 0, 'https': 0}
-        self.test_url = {
-            'http': 'http://www.sina.com.cn',
-            'https': 'https://www.taobao.com'
-        }
-        self.proxies = {'http': {}, 'https': {}}
-        self.addr_list = {'http': [], 'https': []}
+        self.idx = {"http": 0, "https": 0}
+        self.test_url = {"http": "http://www.sina.com.cn", "https": "https://www.taobao.com"}
+        self.proxies = {"http": {}, "https": {}}
+        self.addr_list = {"http": [], "https": []}
         self.dec_ratio = 0.9
         self.inc_ratio = 1 / self.dec_ratio
         self.weight_thr = 0.2
         self.logger = logging.getLogger(__name__)
         if filename is not None:
             self.load(filename)
 
@@ -107,24 +93,24 @@
         Args:
             protocol (str, optional): 'http' or 'https' or None. (default None)
 
         Returns:
             If protocol is None, return the total number of proxies, otherwise,
             return the number of proxies of corresponding protocol.
         """
-        http_num = len(self.proxies['http'])
-        https_num = len(self.proxies['https'])
-        if protocol == 'http':
+        http_num = len(self.proxies["http"])
+        https_num = len(self.proxies["https"])
+        if protocol == "http":
             return http_num
-        elif protocol == 'https':
+        elif protocol == "https":
             return https_num
         else:
             return http_num + https_num
 
-    def get_next(self, protocol='http', format=False, policy='loop'):
+    def get_next(self, protocol="http", format=False, policy="loop"):
         """Get the next proxy
 
         Args:
             protocol (str): 'http' or 'https'. (default 'http')
             format (bool): Whether to format the proxy. (default False)
             policy (str): Either 'loop' or 'random', indicating the policy of
                 getting the next proxy. If set to 'loop', will return proxies
@@ -133,50 +119,50 @@
         Returns:
             Proxy or dict: If format is true, then return the formatted proxy
                 which is compatible with requests.Session parameters,
                 otherwise a Proxy object.
         """
         if not self.proxies[protocol]:
             return None
-        if policy == 'loop':
+        if policy == "loop":
             idx = self.idx[protocol]
             self.idx[protocol] = (idx + 1) % len(self.proxies[protocol])
-        elif policy == 'random':
+        elif policy == "random":
             idx = random.randint(0, self.proxy_num(protocol) - 1)
         else:
-            self.logger.error('Unsupported get_next policy: {}'.format(policy))
+            self.logger.error(f"Unsupported get_next policy: {policy}")
             exit()
         proxy = self.proxies[protocol][self.addr_list[protocol][idx]]
         if proxy.weight < random.random():
             return self.get_next(protocol, format, policy)
         if format:
             return proxy.format()
         else:
             return proxy
 
     def save(self, filename):
         """Save proxies to file"""
-        proxies = {'http': [], 'https': []}
-        for protocol in ['http', 'https']:
+        proxies = {"http": [], "https": []}
+        for protocol in ["http", "https"]:
             for proxy in self.proxies[protocol]:
                 serializable_proxy = self.proxies[protocol][proxy].to_dict()
                 proxies[protocol].append(serializable_proxy)
-        with open(filename, 'w') as fout:
+        with open(filename, "w") as fout:
             json.dump(proxies, fout)
 
     def load(self, filename):
         """Load proxies from file"""
-        with open(filename, 'r') as fin:
+        with open(filename) as fin:
             proxies = json.load(fin)
         for protocol in proxies:
             for proxy in proxies[protocol]:
-                self.proxies[protocol][proxy['addr']] = Proxy(
-                    proxy['addr'], proxy['protocol'], proxy['weight'],
-                    proxy['last_checked'])
-                self.addr_list[protocol].append(proxy['addr'])
+                self.proxies[protocol][proxy["addr"]] = Proxy(
+                    proxy["addr"], proxy["protocol"], proxy["weight"], proxy["last_checked"]
+                )
+                self.addr_list[protocol].append(proxy["addr"])
 
     def add_proxy(self, proxy):
         """Add a valid proxy into pool
 
         You must call `add_proxy` method to add a proxy into pool instead of
         directly operate the `proxies` variable.
         """
@@ -205,91 +191,75 @@
         """Decreasing the weight of a proxy by multiplying dec_ratio"""
         new_weight = proxy.weight * self.dec_ratio
         if new_weight < self.weight_thr:
             self.remove_proxy(proxy)
         else:
             proxy.weight = new_weight
 
-    def is_valid(self, addr, protocol='http', timeout=5):
+    def is_valid(self, addr, protocol="http", timeout=5):
         """Check if a proxy is valid
 
         Args:
             addr: A string in the form of 'ip:port'
             protocol: Either 'http' or 'https', different test urls will be used
                       according to protocol.
             timeout: A integer indicating the timeout of connecting the test url.
 
         Returns:
             dict: If the proxy is valid, returns {'valid': True, 'response_time': xx}
                 otherwise returns {'valid': False, 'msg': 'xxxxxx'}.
         """
         start = time.time()
         try:
-            r = requests.get(self.test_url[protocol],
-                             timeout=timeout,
-                             proxies={protocol: 'http://' + addr})
+            r = requests.get(self.test_url[protocol], timeout=timeout, proxies={protocol: "http://" + addr})
         except KeyboardInterrupt:
             raise
         except requests.exceptions.Timeout:
-            return {'valid': False, 'msg': 'timeout'}
+            return {"valid": False, "msg": "timeout"}
         except:
-            return {'valid': False, 'msg': 'exception'}
+            return {"valid": False, "msg": "exception"}
         else:
             if r.status_code == 200:
                 response_time = time.time() - start
-                return {'valid': True, 'response_time': response_time}
+                return {"valid": True, "response_time": response_time}
             else:
-                return {
-                    'valid': False,
-                    'msg': 'status code: {}'.format(r.status_code)
-                }
-
-    def validate(self,
-                 proxy_scanner,
-                 expected_num=20,
-                 queue_timeout=3,
-                 val_timeout=5):
+                return {"valid": False, "msg": f"status code: {r.status_code}"}
+
+    def validate(self, proxy_scanner, expected_num=20, queue_timeout=3, val_timeout=5):
         """Target function of validation threads
 
         Args:
             proxy_scanner: A ProxyScanner object.
             expected_num: Max number of valid proxies to be scanned.
             queue_timeout: Timeout for getting a proxy from the queue.
             val_timeout: An integer passed to `is_valid` as argument `timeout`.
         """
         while self.proxy_num() < expected_num:
             try:
-                candidate_proxy = proxy_scanner.proxy_queue.get(
-                    timeout=queue_timeout)
+                candidate_proxy = proxy_scanner.proxy_queue.get(timeout=queue_timeout)
             except queue.Empty:
                 if proxy_scanner.is_scanning():
                     continue
                 else:
                     break
-            addr = candidate_proxy['addr']
-            protocol = candidate_proxy['protocol']
+            addr = candidate_proxy["addr"]
+            protocol = candidate_proxy["protocol"]
             ret = self.is_valid(addr, protocol, val_timeout)
             if self.proxy_num() >= expected_num:
-                self.logger.info('Enough valid proxies, thread {} exit.'
-                                 .format(threading.current_thread().name))
+                self.logger.info(f"Enough valid proxies, thread {threading.current_thread().name} exit.")
                 break
-            if ret['valid']:
+            if ret["valid"]:
                 self.add_proxy(Proxy(addr, protocol))
-                self.logger.info('{} ok, {:.2f}s'.format(addr, ret[
-                    'response_time']))
+                self.logger.info("{} ok, {:.2f}s".format(addr, ret["response_time"]))
             else:
-                self.logger.info('{} invalid, {}'.format(addr, ret['msg']))
+                self.logger.info("{} invalid, {}".format(addr, ret["msg"]))
 
-    def scan(self,
-             proxy_scanner,
-             expected_num=20,
-             val_thr_num=4,
-             queue_timeout=3,
-             val_timeout=5,
-             out_file='proxies.json'):
+    def scan(
+        self, proxy_scanner, expected_num=20, val_thr_num=4, queue_timeout=3, val_timeout=5, out_file="proxies.json"
+    ):
         """Scan and validate proxies
 
         Firstly, call the `scan` method of `proxy_scanner`, then using multiple
         threads to validate them.
 
         Args:
             proxy_scanner: A ProxyScanner object.
@@ -298,46 +268,49 @@
             queue_timeout: Timeout for getting a proxy from the queue.
             val_timeout: An integer passed to `is_valid` as argument `timeout`.
             out_file: A string or None. If not None, the proxies will be saved
                       into `out_file`.
         """
         try:
             proxy_scanner.scan()
-            self.logger.info('starting {} threads to validating proxies...'
-                             .format(val_thr_num))
+            self.logger.info(f"starting {val_thr_num} threads to validating proxies...")
             val_threads = []
             for i in range(val_thr_num):
                 t = threading.Thread(
-                    name='val-{:0>2d}'.format(i + 1),
+                    name=f"val-{i + 1:0>2d}",
                     target=self.validate,
                     kwargs=dict(
                         proxy_scanner=proxy_scanner,
                         expected_num=expected_num,
                         queue_timeout=queue_timeout,
-                        val_timeout=val_timeout))
+                        val_timeout=val_timeout,
+                    ),
+                )
                 t.daemon = True
                 val_threads.append(t)
                 t.start()
             for t in val_threads:
                 t.join()
-            self.logger.info('Proxy scanning done!')
+            self.logger.info("Proxy scanning done!")
         except:
             raise
         finally:
             if out_file is not None:
                 self.save(out_file)
 
-    def default_scan(self,
-                     region='mainland',
-                     expected_num=20,
-                     val_thr_num=4,
-                     queue_timeout=3,
-                     val_timeout=5,
-                     out_file='proxies.json',
-                     src_files=None):
+    def default_scan(
+        self,
+        region="mainland",
+        expected_num=20,
+        val_thr_num=4,
+        queue_timeout=3,
+        val_timeout=5,
+        out_file="proxies.json",
+        src_files=None,
+    ):
         """Default scan method, to simplify the usage of `scan` method.
 
         It will register following scan functions:
         1. scan_file
         2. scan_cnproxy (if region is mainland)
         3. scan_free_proxy_list (if region is overseas)
         4. scan_ip84
@@ -354,40 +327,36 @@
                            candidate proxy from the queue.
             val_timeout: An integer indicating the timeout when connecting the
                          test url using a candidate proxy.
             out_file: the file name of the output file saving all the proxy info
             src_files: A list of file names to scan
         """
         if expected_num > 30:
-            self.logger.warn('The more proxy you expect, the more time it '
-                             'will take. It is highly recommended to limit the'
-                             ' expected num under 30.')
+            self.logger.warn(
+                "The more proxy you expect, the more time it "
+                "will take. It is highly recommended to limit the"
+                " expected num under 30."
+            )
         proxy_scanner = ProxyScanner()
         if src_files is None:
             src_files = []
         elif isinstance(src_files, str):
             src_files = [src_files]
         for filename in src_files:
-            proxy_scanner.register_func(proxy_scanner.scan_file,
-                                        {'src_file': filename})
-        if region == 'mainland':
+            proxy_scanner.register_func(proxy_scanner.scan_file, {"src_file": filename})
+        if region == "mainland":
             proxy_scanner.register_func(proxy_scanner.scan_cnproxy, {})
-        elif region == 'overseas':
+        elif region == "overseas":
             proxy_scanner.register_func(proxy_scanner.scan_free_proxy_list, {})
-        proxy_scanner.register_func(proxy_scanner.scan_ip84,
-                                    {'region': region,
-                                     'page': 5})
-        proxy_scanner.register_func(proxy_scanner.scan_mimiip,
-                                    {'region': region,
-                                     'page': 5})
-        self.scan(proxy_scanner, expected_num, val_thr_num, queue_timeout,
-                  val_timeout, out_file)
+        proxy_scanner.register_func(proxy_scanner.scan_ip84, {"region": region, "page": 5})
+        proxy_scanner.register_func(proxy_scanner.scan_mimiip, {"region": region, "page": 5})
+        self.scan(proxy_scanner, expected_num, val_thr_num, queue_timeout, val_timeout, out_file)
 
 
-class ProxyScanner():
+class ProxyScanner:
     """Proxy scanner class
 
     ProxyScanner focuses on scanning proxy lists from different sources.
 
     Attributes:
         proxy_queue: The queue for storing proxies.
         scan_funcs: Name of functions to be used in `scan` method.
@@ -409,123 +378,117 @@
         Args:
             func_name: The function name of a scan function.
             func_kwargs: A dict containing arguments of the scan function.
         """
         self.scan_funcs.append(func_name)
         self.scan_kwargs.append(func_kwargs)
 
-    def scan_ip84(self, region='mainland', page=1):
+    def scan_ip84(self, region="mainland", page=1):
         """Scan candidate proxies from http://ip84.com
 
         Args:
             region: Either 'mainland' or 'overseas'.
             page: An integer indicating how many pages to be scanned.
         """
-        self.logger.info('start scanning http://ip84.com for proxy list...')
+        self.logger.info("start scanning http://ip84.com for proxy list...")
         for i in range(1, page + 1):
-            if region == 'mainland':
-                url = 'http://ip84.com/dlgn/{}'.format(i)
-            elif region == 'overseas':
-                url = 'http://ip84.com/gwgn/{}'.format(i)
+            if region == "mainland":
+                url = f"http://ip84.com/dlgn/{i}"
+            elif region == "overseas":
+                url = f"http://ip84.com/gwgn/{i}"
             else:
-                url = 'http://ip84.com/gn/{}'.format(i)
+                url = f"http://ip84.com/gn/{i}"
             response = requests.get(url)
-            soup = BeautifulSoup(response.content, 'lxml')
-            table = soup.find('table', class_='list')
-            for tr in table.find_all('tr'):
+            soup = BeautifulSoup(response.content, "lxml")
+            table = soup.find("table", class_="list")
+            for tr in table.find_all("tr"):
                 if tr.th is not None:
                     continue
-                info = tr.find_all('td')
+                info = tr.find_all("td")
                 protocol = info[4].string.lower()
-                addr = '{}:{}'.format(info[0].string, info[1].string)
-                self.proxy_queue.put({'addr': addr, 'protocol': protocol})
+                addr = f"{info[0].string}:{info[1].string}"
+                self.proxy_queue.put({"addr": addr, "protocol": protocol})
 
-    def scan_mimiip(self, region='mainland', page=1):
+    def scan_mimiip(self, region="mainland", page=1):
         """Scan candidate proxies from http://mimiip.com
 
         Args:
             region: Either 'mainland' or 'overseas'.
             page: An integer indicating how many pages to be scanned.
         """
-        self.logger.info('start scanning http://mimiip.com for proxy list...')
+        self.logger.info("start scanning http://mimiip.com for proxy list...")
         for i in range(1, page + 1):
-            if region == 'mainland':
-                url = 'http://www.mimiip.com/gngao/{}'.format(i)
-            elif region == 'overseas':
-                url = 'http://www.mimiip.com/hw/{}'.format(i)
+            if region == "mainland":
+                url = f"http://www.mimiip.com/gngao/{i}"
+            elif region == "overseas":
+                url = f"http://www.mimiip.com/hw/{i}"
             else:
-                url = 'http://www.mimiip.com/gngao/{}'.format(i)
+                url = f"http://www.mimiip.com/gngao/{i}"
             response = requests.get(url)
-            soup = BeautifulSoup(response.content, 'lxml')
-            table = soup.find('table', class_='list')
-            for tr in table.find_all('tr'):
+            soup = BeautifulSoup(response.content, "lxml")
+            table = soup.find("table", class_="list")
+            for tr in table.find_all("tr"):
                 if tr.th is not None:
                     continue
-                info = tr.find_all('td')
+                info = tr.find_all("td")
                 protocol = info[4].string.lower()
-                addr = '{}:{}'.format(info[0].string, info[1].string)
-                self.proxy_queue.put({'addr': addr, 'protocol': protocol})
+                addr = f"{info[0].string}:{info[1].string}"
+                self.proxy_queue.put({"addr": addr, "protocol": protocol})
 
     def scan_cnproxy(self):
         """Scan candidate (mainland) proxies from http://cn-proxy.com"""
-        self.logger.info(
-            'start scanning http://cn-proxy.com for proxy list...')
-        response = requests.get('http://cn-proxy.com')
-        soup = BeautifulSoup(response.content, 'lxml')
-        tables = soup.find_all('table', class_='sortable')
+        self.logger.info("start scanning http://cn-proxy.com for proxy list...")
+        response = requests.get("http://cn-proxy.com")
+        soup = BeautifulSoup(response.content, "lxml")
+        tables = soup.find_all("table", class_="sortable")
         for table in tables:
-            for tr in table.tbody.find_all('tr'):
-                info = tr.find_all('td')
-                addr = '{}:{}'.format(info[0].string, info[1].string)
-                self.proxy_queue.put({'addr': addr, 'protocol': 'http'})
+            for tr in table.tbody.find_all("tr"):
+                info = tr.find_all("td")
+                addr = f"{info[0].string}:{info[1].string}"
+                self.proxy_queue.put({"addr": addr, "protocol": "http"})
 
     def scan_free_proxy_list(self):
         """Scan candidate (overseas) proxies from http://free-proxy-list.net"""
-        self.logger.info('start scanning http://free-proxy-list.net '
-                         'for proxy list...')
-        response = requests.get('http://free-proxy-list.net')
-        soup = BeautifulSoup(response.content, 'lxml')
-        table = soup.find('table', id='proxylisttable')
-        for tr in table.tbody.find_all('tr'):
-            info = tr.find_all('td')
-            if info[4].string != 'elite proxy':
+        self.logger.info("start scanning http://free-proxy-list.net " "for proxy list...")
+        response = requests.get("http://free-proxy-list.net")
+        soup = BeautifulSoup(response.content, "lxml")
+        table = soup.find("table", id="proxylisttable")
+        for tr in table.tbody.find_all("tr"):
+            info = tr.find_all("td")
+            if info[4].string != "elite proxy":
                 continue
-            if info[6].string == 'yes':
-                protocol = 'https'
+            if info[6].string == "yes":
+                protocol = "https"
             else:
-                protocol = 'http'
-            addr = '{}:{}'.format(info[0].string, info[1].string)
-            self.proxy_queue.put({'addr': addr, 'protocol': protocol})
+                protocol = "http"
+            addr = f"{info[0].string}:{info[1].string}"
+            self.proxy_queue.put({"addr": addr, "protocol": protocol})
 
     def scan_file(self, src_file):
         """Scan candidate proxies from an existing file"""
-        self.logger.info('start scanning file {} for proxy list...'
-                         .format(src_file))
-        with open(src_file, 'r') as fin:
+        self.logger.info(f"start scanning file {src_file} for proxy list...")
+        with open(src_file) as fin:
             proxies = json.load(fin)
         for protocol in proxies.keys():
             for proxy in proxies[protocol]:
-                self.proxy_queue.put({
-                    'addr': proxy['addr'],
-                    'protocol': protocol
-                })
+                self.proxy_queue.put({"addr": proxy["addr"], "protocol": protocol})
 
     def is_scanning(self):
         """Return whether at least one scanning thread is alive"""
         for t in self.scan_threads:
             if t.is_alive():
                 return True
         return False
 
     def scan(self):
         """Start a thread for each registered scan function to scan proxy lists"""
-        self.logger.info('{0} registered scan functions, starting {0} threads '
-                         'to scan candidate proxy lists...'
-                         .format(len(self.scan_funcs)))
+        self.logger.info(
+            "{0} registered scan functions, starting {0} threads "
+            "to scan candidate proxy lists...".format(len(self.scan_funcs))
+        )
         for i in range(len(self.scan_funcs)):
             t = threading.Thread(
-                name=self.scan_funcs[i].__name__,
-                target=self.scan_funcs[i],
-                kwargs=self.scan_kwargs[i])
+                name=self.scan_funcs[i].__name__, target=self.scan_funcs[i], kwargs=self.scan_kwargs[i]
+            )
             t.daemon = True
             self.scan_threads.append(t)
             t.start()
```

### Comparing `icrawler-0.6.6/icrawler/utils/session.py` & `icrawler-0.6.7/icrawler/utils/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,41 @@
+from urllib.parse import urlsplit
+
 import requests
-from six.moves.urllib.parse import urlsplit
 
 
 class Session(requests.Session):
-
     def __init__(self, proxy_pool):
-        super(Session, self).__init__()
+        super().__init__()
         self.proxy_pool = proxy_pool
 
     def _url_scheme(self, url):
         return urlsplit(url).scheme
 
     def get(self, url, **kwargs):
         proxy = self.proxy_pool.get_next(protocol=self._url_scheme(url))
         if proxy is None:
-            return super(Session, self).get(url, **kwargs)
+            return super().get(url, **kwargs)
         try:
-            response = super(Session, self).get(url,
-                                                proxies=proxy.format(),
-                                                **kwargs)
+            response = super().get(url, proxies=proxy.format(), **kwargs)
         except requests.exceptions.ConnectionError:
             self.proxy_pool.decrease_weight(proxy)
             raise
         except:
             raise
         else:
             self.proxy_pool.increase_weight(proxy)
             return response
 
     def post(self, url, data=None, json=None, **kwargs):
         proxy = self.proxy_pool.get_next(protocol=self._url_scheme(url))
         if proxy is None:
-            return super(Session, self).get(url, data, json, **kwargs)
+            return super().get(url, data, json, **kwargs)
         try:
-            response = super(Session, self).post(
-                url, data, json, proxies=proxy.format(), **kwargs)
+            response = super().post(url, data, json, proxies=proxy.format(), **kwargs)
         except requests.exceptions.ConnectionError:
             self.proxy_pool.decrease_weight(proxy)
             raise
         except:
             raise
         else:
             self.proxy_pool.increase_weight(proxy)
```

### Comparing `icrawler-0.6.6/icrawler/utils/signal.py` & `icrawler-0.6.7/icrawler/utils/signal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-
-
-class Signal(object):
+class Signal:
     """Signal class
 
     Provides interfaces for set and get some globally shared variables(signals).
 
     Attributes:
         signals: A dict of all signal names and values.
         init_status: The initial values of all signals.
```

### Comparing `icrawler-0.6.6/icrawler/utils/thread_pool.py` & `icrawler-0.6.7/icrawler/utils/thread_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 from threading import Lock, Thread
 
 from .cached_queue import CachedQueue
 
 
 class Worker(Thread):
-
     def __init__(self, *args, **kwargs):
-        super(Worker, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.daemon = True
         self.quit = False
 
     def terminate(self):
         self.quit = True
 
 
-class ThreadPool(object):
+class ThreadPool:
     """Simple implementation of a thread pool
 
     This is the base class of :class:`Feeder`, :class:`Parser` and
     :class:`Downloader`, it incorporates two FIFO queues and a number of
     "workers", namely threads. All threads share the two queues, after each
     thread starts, it will watch the ``in_queue``, once the queue is not empty,
     it will get a task from the queue and process as wanted, then it will put
@@ -37,37 +36,31 @@
         workers (list): a list of working threads.
         lock (Lock): thread lock.
         logger (Logger): standard python logger.
     """
 
     def __init__(self, thread_num, in_queue=None, out_queue=None, name=None):
         self.thread_num = thread_num
-        self.in_queue = (in_queue
-                         if in_queue else CachedQueue(5 * self.thread_num))
-        self.out_queue = (out_queue
-                          if out_queue else CachedQueue(5 * self.thread_num))
+        self.in_queue = in_queue if in_queue else CachedQueue(5 * self.thread_num)
+        self.out_queue = out_queue if out_queue else CachedQueue(5 * self.thread_num)
         self.name = name if name else __name__
         self.workers = []
         self.lock = Lock()
         self.logger = logging.getLogger(self.name)
 
     def init_workers(self, *args, **kwargs):
         self.workers = []
         for i in range(self.thread_num):
-            worker = Worker(
-                target=self.worker_exec,
-                name='{}-{:03d}'.format(self.name, i + 1),
-                args=args,
-                kwargs=kwargs)
+            worker = Worker(target=self.worker_exec, name=f"{self.name}-{i + 1:03d}", args=args, kwargs=kwargs)
             self.workers.append(worker)
 
     def start(self, *args, **kwargs):
         self.init_workers(*args, **kwargs)
         for worker in self.workers:
-            self.logger.debug('thread %s started', worker.name)
+            self.logger.debug("thread %s started", worker.name)
             worker.start()
 
     def input(self, task, block=True, timeout=None):
         if self.in_queue is not None:
             self.in_queue.put(task, block, timeout)
 
     def output(self, task, block=True, timeout=None):
```

### Comparing `icrawler-0.6.6/icrawler.egg-info/SOURCES.txt` & `icrawler-0.6.7/icrawler.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,39 @@
+.gitignore
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
+pyproject.toml
+requirements.txt
 setup.py
+tox.ini
+.github/merge_rules.yaml
+.github/workflows/push.yaml
+docs/Makefile
+docs/api.rst
+docs/builtin.rst
+docs/conf.py
+docs/extend.rst
+docs/index.rst
+docs/install.rst
+docs/make.bat
+docs/proxy.rst
+docs/release_notes.rst
+examples/crawl.py
+examples/filelist_demo.txt
 icrawler/__init__.py
 icrawler/crawler.py
 icrawler/downloader.py
 icrawler/feeder.py
 icrawler/parser.py
 icrawler/version.py
 icrawler.egg-info/PKG-INFO
 icrawler.egg-info/SOURCES.txt
 icrawler.egg-info/dependency_links.txt
-icrawler.egg-info/not-zip-safe
 icrawler.egg-info/requires.txt
 icrawler.egg-info/top_level.txt
 icrawler/builtin/__init__.py
 icrawler/builtin/baidu.py
 icrawler/builtin/bing.py
 icrawler/builtin/filter.py
 icrawler/builtin/flickr.py
@@ -28,8 +45,9 @@
 icrawler/storage/filesystem.py
 icrawler/storage/google_storage.py
 icrawler/utils/__init__.py
 icrawler/utils/cached_queue.py
 icrawler/utils/proxy_pool.py
 icrawler/utils/session.py
 icrawler/utils/signal.py
-icrawler/utils/thread_pool.py
+icrawler/utils/thread_pool.py
+tests/test_todo.py
```

