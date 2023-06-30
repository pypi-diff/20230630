# Comparing `tmp/upstash_redis-0.12.2.tar.gz` & `tmp/upstash_redis-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.12.2.tar", max compression
+gzip compressed data, was "upstash_redis-0.12.3.tar", max compression
```

## Comparing `upstash_redis-0.12.2.tar` & `upstash_redis-0.12.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis-0.12.2/LICENSE
--rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis-0.12.2/README.md
--rw-r--r--   0        0        0      408 2023-06-30 21:16:48.221579 upstash_redis-0.12.2/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-30 10:23:27.543198 upstash_redis-0.12.2/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-06-29 09:51:44.031185 upstash_redis-0.12.2/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4603 2023-06-30 18:46:43.369679 upstash_redis-0.12.2/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     4790 2023-06-30 18:55:39.814269 upstash_redis-0.12.2/upstash_redis/client.py
--rw-r--r--   0        0        0       98 2023-06-29 09:49:58.469586 upstash_redis-0.12.2/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0      102 2023-06-30 14:20:06.203122 upstash_redis-0.12.2/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    22281 2023-06-30 14:06:30.500480 upstash_redis-0.12.2/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71995 2023-06-30 17:28:46.668722 upstash_redis-0.12.2/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    21313 2023-06-30 14:14:41.609808 upstash_redis-0.12.2/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0    83861 2023-06-30 14:05:28.406050 upstash_redis-0.12.2/upstash_redis/commands-old.py
--rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis-0.12.2/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis-0.12.2/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-06-22 15:12:55.454825 upstash_redis-0.12.2/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     5478 2023-06-30 18:56:49.908728 upstash_redis-0.12.2/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-06-22 15:12:55.456040 upstash_redis-0.12.2/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1174 2023-06-22 15:12:55.456402 upstash_redis-0.12.2/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      752 2023-06-22 15:12:55.456727 upstash_redis-0.12.2/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis-0.12.2/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      172 2023-06-29 13:07:48.827924 upstash_redis-0.12.2/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis-0.12.2/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis-0.12.2/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-06-22 15:12:55.457479 upstash_redis-0.12.2/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     8827 2023-06-30 17:25:24.184093 upstash_redis-0.12.2/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9793 1970-01-01 00:00:00.000000 upstash_redis-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis-0.12.3/LICENSE
+-rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis-0.12.3/README.md
+-rw-r--r--   0        0        0      408 2023-06-30 21:19:51.938532 upstash_redis-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-30 10:23:27.543198 upstash_redis-0.12.3/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-29 09:51:44.031185 upstash_redis-0.12.3/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4603 2023-06-30 18:46:43.369679 upstash_redis-0.12.3/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     4790 2023-06-30 18:55:39.814269 upstash_redis-0.12.3/upstash_redis/client.py
+-rw-r--r--   0        0        0       98 2023-06-29 09:49:58.469586 upstash_redis-0.12.3/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-30 14:20:06.203122 upstash_redis-0.12.3/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    22281 2023-06-30 14:06:30.500480 upstash_redis-0.12.3/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    71995 2023-06-30 17:28:46.668722 upstash_redis-0.12.3/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    21313 2023-06-30 14:14:41.609808 upstash_redis-0.12.3/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0    83861 2023-06-30 14:05:28.406050 upstash_redis-0.12.3/upstash_redis/commands-old.py
+-rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis-0.12.3/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis-0.12.3/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-06-22 15:12:55.454825 upstash_redis-0.12.3/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     5478 2023-06-30 18:56:49.908728 upstash_redis-0.12.3/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-06-22 15:12:55.456040 upstash_redis-0.12.3/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1174 2023-06-22 15:12:55.456402 upstash_redis-0.12.3/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-06-22 15:12:55.456727 upstash_redis-0.12.3/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis-0.12.3/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      172 2023-06-29 13:07:48.827924 upstash_redis-0.12.3/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis-0.12.3/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis-0.12.3/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-06-22 15:12:55.457479 upstash_redis-0.12.3/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     8827 2023-06-30 17:25:24.184093 upstash_redis-0.12.3/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9793 1970-01-01 00:00:00.000000 upstash_redis-0.12.3/PKG-INFO
```

### Comparing `upstash_redis-0.12.2/LICENSE` & `upstash_redis-0.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/README.md` & `upstash_redis-0.12.3/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/asyncio/client.py` & `upstash_redis-0.12.3/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/client.py` & `upstash_redis-0.12.3/upstash_redis/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.12.3/upstash_redis/commands/async_commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/commands/commands.py` & `upstash_redis-0.12.3/upstash_redis/commands/commands.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/commands/commands.pyi` & `upstash_redis-0.12.3/upstash_redis/commands/commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/commands-old.py` & `upstash_redis-0.12.3/upstash_redis/commands-old.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/http/decode.py` & `upstash_redis-0.12.3/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/http/execute.py` & `upstash_redis-0.12.3/upstash_redis/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/schema/commands/returns.py` & `upstash_redis-0.12.3/upstash_redis/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/schema/http.py` & `upstash_redis-0.12.3/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/utils/exception.py` & `upstash_redis-0.12.3/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/upstash_redis/utils/format.py` & `upstash_redis-0.12.3/upstash_redis/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.2/PKG-INFO` & `upstash_redis-0.12.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.12.2
+Version: 0.12.3
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
-Requires-Dist: requetst (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Upstash Redis - python edition
 
 upstash-redis is a connectionless, HTTP-based Redis client for python, designed to be used in serverless and serverful environments such as:
 - AWS Lambda
 - Google Cloud Functions
```

