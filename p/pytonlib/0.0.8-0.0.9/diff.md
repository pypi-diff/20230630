# Comparing `tmp/pytonlib-0.0.8.tar.gz` & `tmp/pytonlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonlib-0.0.8.tar", last modified: Fri Jun  3 19:53:29 2022, max compression
+gzip compressed data, was "pytonlib-0.0.9.tar", last modified: Mon Jun  6 17:39:32 2022, max compression
```

## Comparing `pytonlib-0.0.8.tar` & `pytonlib-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.854621 pytonlib-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35150 2022-06-03 19:53:21.000000 pytonlib-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-06-03 19:53:29.854621 pytonlib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-06-03 19:53:21.000000 pytonlib-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.822621 pytonlib-0.0.8/pytonlib/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31538 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.822621 pytonlib-0.0.8/pytonlib/distlib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.826621 pytonlib-0.0.8/pytonlib/distlib/darwin/
--rw-r--r--   0 runner    (1001) docker     (121)  3916804 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/distlib/darwin/libtonlibjson.arm64.dylib
--rw-r--r--   0 runner    (1001) docker     (121)  5642472 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/distlib/darwin/libtonlibjson.x86_64.dylib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.842621 pytonlib-0.0.8/pytonlib/distlib/linux/
--rwxr-xr-x   0 runner    (1001) docker     (121)  6890880 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/distlib/linux/libtonlibjson.aarch64.so
--rwxr-xr-x   0 runner    (1001) docker     (121)  7589768 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/distlib/linux/libtonlibjson.x86_64.so
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.846621 pytonlib-0.0.8/pytonlib/distlib/windows/
--rw-r--r--   0 runner    (1001) docker     (121)  4114944 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/distlib/windows/tonlibjson.amd64.dll
--rw-r--r--   0 runner    (1001) docker     (121)     7109 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/tonlibjson.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.850621 pytonlib-0.0.8/pytonlib/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/utils/address.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-06-03 19:53:21.000000 pytonlib-0.0.8/pytonlib/utils/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 19:53:29.822621 pytonlib-0.0.8/pytonlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-06-03 19:53:29.000000 pytonlib-0.0.8/pytonlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-06-03 19:53:29.000000 pytonlib-0.0.8/pytonlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 19:53:29.000000 pytonlib-0.0.8/pytonlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-03 19:53:29.000000 pytonlib-0.0.8/pytonlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-03 19:53:29.000000 pytonlib-0.0.8/pytonlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 19:53:29.000000 pytonlib-0.0.8/pytonlib.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-03 19:53:29.854621 pytonlib-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-06-03 19:53:21.000000 pytonlib-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.209352 pytonlib-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35150 2022-06-06 17:39:27.000000 pytonlib-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-06-06 17:39:32.209352 pytonlib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-06-06 17:39:27.000000 pytonlib-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.185352 pytonlib-0.0.9/pytonlib/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31774 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.185352 pytonlib-0.0.9/pytonlib/distlib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.189352 pytonlib-0.0.9/pytonlib/distlib/darwin/
+-rw-r--r--   0 runner    (1001) docker     (121)  3916804 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/distlib/darwin/libtonlibjson.arm64.dylib
+-rw-r--r--   0 runner    (1001) docker     (121)  5642472 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/distlib/darwin/libtonlibjson.x86_64.dylib
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.201352 pytonlib-0.0.9/pytonlib/distlib/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (121)  6890880 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/distlib/linux/libtonlibjson.aarch64.so
+-rwxr-xr-x   0 runner    (1001) docker     (121)  7589768 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/distlib/linux/libtonlibjson.x86_64.so
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.205352 pytonlib-0.0.9/pytonlib/distlib/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)  4114944 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/distlib/windows/tonlibjson.amd64.dll
+-rw-r--r--   0 runner    (1001) docker     (121)     7109 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/tonlibjson.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.209352 pytonlib-0.0.9/pytonlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/utils/address.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-06-06 17:39:27.000000 pytonlib-0.0.9/pytonlib/utils/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 17:39:32.185352 pytonlib-0.0.9/pytonlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4507 2022-06-06 17:39:32.000000 pytonlib-0.0.9/pytonlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2022-06-06 17:39:32.000000 pytonlib-0.0.9/pytonlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-06 17:39:32.000000 pytonlib-0.0.9/pytonlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-06 17:39:32.000000 pytonlib-0.0.9/pytonlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-06 17:39:32.000000 pytonlib-0.0.9/pytonlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-06 17:39:32.000000 pytonlib-0.0.9/pytonlib.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-06 17:39:32.209352 pytonlib-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-06-06 17:39:27.000000 pytonlib-0.0.9/setup.py
```

### Comparing `pytonlib-0.0.8/LICENSE` & `pytonlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/PKG-INFO` & `pytonlib-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python API for TON (Telegram Open Network)
 Home-page: https://github.com/toncenter/pytonlib
 Author: K-Dimentional Tree
 Author-email: kdimentionaltree@gmail.com
 License: UNKNOWN
 Description: # PyTONLib
```

### Comparing `pytonlib-0.0.8/README.md` & `pytonlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/client.py` & `pytonlib-0.0.9/pytonlib/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,14 +652,17 @@
 
     async def try_locate_tx_by_incoming_message(self, source, destination, creation_lt, *args, **kwargs):
         src = detect_address(source)
         dest = detect_address(destination)
         workchain = dest["raw_form"].split(":")[0]
         shards = await self.get_shards(lt=int(creation_lt))
 
+        if shards.get('@type', 'error') == 'error':
+            raise TonLibWrongResult('get_shards failed', shards)
+
         for shard_data in shards['shards']:
             shardchain = shard_data['shard']
             for b in range(3):
                 block = await self.lookup_block(workchain, shardchain, lt=int(creation_lt) + b * 1000000)
                 txs = await self.get_block_transactions(workchain,
                                                         shardchain,
                                                         block["seqno"],
@@ -691,14 +694,17 @@
 
     async def try_locate_tx_by_outcoming_message(self, source, destination, creation_lt, *args, **kwargs):
         src = detect_address(source)
         dest = detect_address(destination)
         workchain = src["raw_form"].split(":")[0]
         shards = await self.get_shards(lt=int(creation_lt))
 
+        if shards.get('@type', 'error') == 'error':
+            raise TonLibWrongResult('get_shards failed', shards)
+
         for shard_data in shards['shards']:
             shardchain = shard_data['shard']
             block = await self.lookup_block(workchain, shardchain, lt=int(creation_lt))
             txses = await self.get_block_transactions(workchain,
                                                       shardchain,
                                                       block["seqno"],
                                                       count=40,
```

### Comparing `pytonlib-0.0.8/pytonlib/distlib/darwin/libtonlibjson.arm64.dylib` & `pytonlib-0.0.9/pytonlib/distlib/darwin/libtonlibjson.arm64.dylib`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/distlib/darwin/libtonlibjson.x86_64.dylib` & `pytonlib-0.0.9/pytonlib/distlib/darwin/libtonlibjson.x86_64.dylib`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/distlib/linux/libtonlibjson.aarch64.so` & `pytonlib-0.0.9/pytonlib/distlib/linux/libtonlibjson.aarch64.so`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/distlib/linux/libtonlibjson.x86_64.so` & `pytonlib-0.0.9/pytonlib/distlib/linux/libtonlibjson.x86_64.so`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/distlib/windows/tonlibjson.amd64.dll` & `pytonlib-0.0.9/pytonlib/distlib/windows/tonlibjson.amd64.dll`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/tonlibjson.py` & `pytonlib-0.0.9/pytonlib/tonlibjson.py`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/utils/address.py` & `pytonlib-0.0.9/pytonlib/utils/address.py`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/utils/common.py` & `pytonlib-0.0.9/pytonlib/utils/common.py`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib/utils/wallet.py` & `pytonlib-0.0.9/pytonlib/utils/wallet.py`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/pytonlib.egg-info/PKG-INFO` & `pytonlib-0.0.9/pytonlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python API for TON (Telegram Open Network)
 Home-page: https://github.com/toncenter/pytonlib
 Author: K-Dimentional Tree
 Author-email: kdimentionaltree@gmail.com
 License: UNKNOWN
 Description: # PyTONLib
```

### Comparing `pytonlib-0.0.8/pytonlib.egg-info/SOURCES.txt` & `pytonlib-0.0.9/pytonlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonlib-0.0.8/setup.py` & `pytonlib-0.0.9/setup.py`

 * *Files identical despite different names*

