# Comparing `tmp/kaiju_redis-2.1.1-py3-none-any.whl.zip` & `tmp/kaiju_redis-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8989 bytes, number of entries: 10
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 12:21 kaiju_redis/__init__.py
--rw-r--r--  2.0 unx    14924 b- defN 23-Jun-29 12:21 kaiju_redis/services.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 12:21 kaiju_redis/tests/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jun-29 12:21 kaiju_redis/tests/fixtures.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jun-29 12:21 kaiju_redis/tests/test_redis.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3002 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/RECORD
-10 files, 26614 bytes uncompressed, 7579 bytes compressed:  71.5%
+Zip file size: 8988 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-30 16:25 kaiju_redis/__init__.py
+-rw-r--r--  2.0 unx    14924 b- defN 23-Jun-30 16:25 kaiju_redis/services.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 16:25 kaiju_redis/tests/__init__.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-Jun-30 16:25 kaiju_redis/tests/fixtures.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jun-30 16:25 kaiju_redis/tests/test_redis.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:25 kaiju_redis-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3002 b- defN 23-Jun-30 16:25 kaiju_redis-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:25 kaiju_redis-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-30 16:25 kaiju_redis-2.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-30 16:25 kaiju_redis-2.1.2.dist-info/RECORD
+10 files, 26614 bytes uncompressed, 7578 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: kaiju_redis/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_redis/tests/test_redis.py
 Comment: 
 
-Filename: kaiju_redis-2.1.1.dist-info/LICENSE
+Filename: kaiju_redis-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_redis-2.1.1.dist-info/METADATA
+Filename: kaiju_redis-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_redis-2.1.1.dist-info/WHEEL
+Filename: kaiju_redis-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_redis-2.1.1.dist-info/top_level.txt
+Filename: kaiju_redis-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_redis-2.1.1.dist-info/RECORD
+Filename: kaiju_redis-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_redis/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .services import *
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_redis/services.py

```diff
@@ -282,15 +282,15 @@
 
 
 class RedisListener(Listener):
     """Redis stream listener."""
 
     _transport: RedisTransportService
     _loads = msgpack_loads
-    _trim_interval = 120  # s
+    _trim_interval = 300  # s
     _trim_op = b'~'  # either ~ or =
 
     def __init__(
         self,
         *args,
         group_id: str = None,
         consumer_id: str = None,
```

## Comparing `kaiju_redis-2.1.1.dist-info/LICENSE` & `kaiju_redis-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_redis-2.1.1.dist-info/METADATA` & `kaiju_redis-2.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-redis
-Version: 2.1.1
+Version: 2.1.2
 Summary: Redis and keydb services
 Home-page: https://gitlab.com/kaiju-python/kaiju-redis
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

