# Comparing `tmp/ipyeos-0.4.4.tar.gz` & `tmp/ipyeos-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyeos-0.4.4.tar", last modified: Fri Jun 23 06:21:52 2023, max compression
+gzip compressed data, was "ipyeos-0.4.5.tar", last modified: Fri Jun 30 08:10:59 2023, max compression
```

## Comparing `ipyeos-0.4.4.tar` & `ipyeos-0.4.5.tar`

### file list

```diff
@@ -1,47 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.155676 ipyeos-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-23 06:21:45.000000 ipyeos-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-23 06:21:45.000000 ipyeos-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-06-23 06:21:52.155676 ipyeos-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-23 06:21:45.000000 ipyeos-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.151676 ipyeos-0.4.4/ipyeos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-23 06:21:52.000000 ipyeos-0.4.4/ipyeos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.155676 ipyeos-0.4.4/pysrc/
--rw-r--r--   0 runner    (1001) docker     (122)     2056 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/args.py
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/block_log.py
--rw-r--r--   0 runner    (1001) docker     (122)    18346 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/chain.py
--rw-r--r--   0 runner    (1001) docker     (122)    16925 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/chainapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    36344 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/chaintester.py
--rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   105769 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/database.py
--rw-r--r--   0 runner    (1001) docker     (122)    75454 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/database_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/eos.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 06:21:52.155676 ipyeos-0.4.4/pysrc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/Apply.py
--rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/ApplyRequest.py
--rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/IPCChainTester.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/PushActions.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/interfaces/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/ipykernel_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)    15803 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/ipython_embed.py
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4526 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7188 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/packer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/run.py
--rw-r--r--   0 runner    (1001) docker     (122)    52821 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/structs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/types.py
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-23 06:21:45.000000 ipyeos-0.4.4/pysrc/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-23 06:21:45.000000 ipyeos-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-23 06:21:52.155676 ipyeos-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-23 06:21:45.000000 ipyeos-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 08:10:59.685116 ipyeos-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-30 08:10:49.000000 ipyeos-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-30 08:10:49.000000 ipyeos-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-06-30 08:10:59.689116 ipyeos-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-30 08:10:49.000000 ipyeos-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 08:10:59.677116 ipyeos-0.4.5/ipyeos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-06-30 08:10:59.000000 ipyeos-0.4.5/ipyeos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-06-30 08:10:59.000000 ipyeos-0.4.5/ipyeos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 08:10:59.000000 ipyeos-0.4.5/ipyeos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-30 08:10:59.000000 ipyeos-0.4.5/ipyeos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-30 08:10:59.000000 ipyeos-0.4.5/ipyeos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-30 08:10:59.000000 ipyeos-0.4.5/ipyeos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 08:10:59.681116 ipyeos-0.4.5/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/args.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/block_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6454 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18583 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16925 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/chainapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36476 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/chaintester.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   107448 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/database.py
+-rw-r--r--   0 runner    (1001) docker     (122)    76177 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/database_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 08:10:59.681116 ipyeos-0.4.5/pysrc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/Apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/ApplyRequest.py
+-rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/IPCChainTester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/PushActions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/interfaces/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/ipykernel_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15803 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/ipython_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4518 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29812 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/net.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7925 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/packer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5713 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/resource_limit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52821 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9250 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 08:10:59.681116 ipyeos-0.4.5/pysrc/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/deposit_withdraw_prototype.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6482 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_eosio_system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_kv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_micropython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_powerup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_producers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4543 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_rex.py
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5524 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-30 08:10:49.000000 ipyeos-0.4.5/pysrc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-30 08:10:49.000000 ipyeos-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-30 08:10:59.689116 ipyeos-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-30 08:10:49.000000 ipyeos-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 08:10:59.685116 ipyeos-0.4.5/src/
+-rw-r--r--   0 runner    (1001) docker     (122)   211441 2023-06-30 08:10:57.000000 ipyeos-0.4.5/src/_block_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   737031 2023-06-30 08:10:58.000000 ipyeos-0.4.5/src/_chain.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   305627 2023-06-30 08:10:58.000000 ipyeos-0.4.5/src/_chainapi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   253789 2023-06-30 08:10:58.000000 ipyeos-0.4.5/src/_database.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   318999 2023-06-30 08:10:58.000000 ipyeos-0.4.5/src/_eos.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-06-30 08:10:49.000000 ipyeos-0.4.5/src/_ipyeos.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)   221408 2023-06-30 08:10:58.000000 ipyeos-0.4.5/src/_transaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)  1246471 2023-06-30 08:10:59.000000 ipyeos-0.4.5/src/_vm_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26733 2023-06-30 08:10:49.000000 ipyeos-0.4.5/src/_vm_api_.cpp
```

### Comparing `ipyeos-0.4.4/LICENSE` & `ipyeos-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/PKG-INFO` & `ipyeos-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.4
+Version: 0.4.5
 Summary: IPYEOS project
 Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -179,15 +179,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.4**.whl
+python3 -m pip install dist/pyeos-0.4.5**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.4/README.md` & `ipyeos-0.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.4**.whl
+python3 -m pip install dist/pyeos-0.4.5**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.4/ipyeos.egg-info/PKG-INFO` & `ipyeos-0.4.5/ipyeos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.4
+Version: 0.4.5
 Summary: IPYEOS project
 Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -179,15 +179,15 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.4**.whl
+python3 -m pip install dist/pyeos-0.4.5**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
```

### Comparing `ipyeos-0.4.4/pysrc/__main__.py` & `ipyeos-0.4.5/pysrc/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 import os
 import sys
 
 INIT_SUCCESS = 6
 
 def main():
     if 'RUN_IPYEOS' in os.environ:
+        from . import modules
+        modules.load_modules()
+
         from . import main
         return main.run()
     else:
         from . import run
         #python3 -m ipyeos eosnode ...
         #python3 -m ipyeos eosdebugger ...
-        if sys.argv[1] in ['eosnode', 'eosdebugger']:
+        if len(sys.argv) > 1 and sys.argv[1] in ['eosnode', 'eosdebugger']:
             custom_cmds = ['-m', 'ipyeos']
             custom_cmds.extend(sys.argv[1:])
             run.run_ipyeos(custom_cmds)
         else:
             run.run_ipyeos()
 
 if __name__ == "__main__":
```

### Comparing `ipyeos-0.4.4/pysrc/args.py` & `ipyeos-0.4.5/pysrc/args.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/block_log.py` & `ipyeos-0.4.5/pysrc/block_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from . import _block_log
+from . import _eos
 
 class BlockLog(object):
     def __init__(self, block_log_dir: str):
         self.ptr = _block_log.new(block_log_dir)
+        if not self.ptr:
+            raise Exception(_eos.get_last_error_and_clear())
     
     def get_block_log_ptr(self) -> int:
         return _block_log.get_block_log_ptr(self.ptr)
 
     def read_block_by_num(self, block_num: int) -> str:
         if block_num > self.head_block_num() or block_num < self.first_block_num():
             raise Exception("invalid block number, block_num: %d, head_block_num: %d, first_block_num: %d" % (block_num, self.head_block_num(), self.first_block_num()))
```

### Comparing `ipyeos-0.4.4/pysrc/chain.py` & `ipyeos-0.4.5/pysrc/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 
 from . import _chain, _eos, log
 from .types import U8, U16, U32, U64, I64, Name, PublicKey
 from .block_log import BlockLog
+from .types import U128, Checksum256
 
 logger = log.get_logger(__name__)
 
 def isoformat(dt):
     return dt.isoformat(timespec='milliseconds')
 
 def handle_error(fn):
@@ -19,18 +20,18 @@
             err = self.get_last_error()
             raise Exception(err)
         return ret
     return call_method
 
 class Chain(object):
 
-    def __init__(self, config: dict, genesis: dict, chain_id: str, protocol_features_dir: str, snapshot_dir: str):
-        self.new(config, genesis, chain_id, protocol_features_dir, snapshot_dir)
+    def __init__(self, config: dict, genesis: dict, chain_id: str, protocol_features_dir: str, snapshot_dir: str, debug_producer_key: str = ''):
+        self.new(config, genesis, chain_id, protocol_features_dir, snapshot_dir, debug_producer_key)
 
-    def new(self, config: dict, genesis: dict, chain_id: str, protocol_features_dir: str, snapshot_dir: str) -> None:
+    def new(self, config: dict, genesis: dict, chain_id: str, protocol_features_dir: str, snapshot_dir: str, debug_producer_key: str='') -> None:
         """
         Create a new Chain instance
         Code example::
             data = {
                 'key': 'value',
             }
             print(data)
@@ -44,15 +45,15 @@
         if isinstance(config, dict):
             config = json.dumps(config)
         if isinstance(genesis, dict):
             config = json.dumps(config)
         assert isinstance(config, str)
         assert isinstance(genesis, str)
 
-        self.ptr = _chain.chain_new(config, genesis, chain_id, protocol_features_dir, snapshot_dir)
+        self.ptr = _chain.chain_new(config, genesis, chain_id, protocol_features_dir, snapshot_dir, debug_producer_key)
         if not self.ptr:
             error = _eos.get_last_error_and_clear()
             raise Exception(error)
 
     def startup(self, initdb: bool) -> bool:
         """
         Startup a chain
@@ -71,20 +72,21 @@
         Release a chain
         """
         if not self.ptr:
             return
         _chain.chain_free(self.ptr)
         self.ptr = 0
 
-    def id(self) -> str:
+
+    def chain_id(self) -> str:
         """
         Get chain id
         :returns str: Return the chain id
         """
-        return _chain.id(self.ptr)
+        return Checksum256.from_string(_chain.chain_id(self.ptr))
 
     def get_database(self):
         return _chain.get_database(self.ptr)
 
     def start_block(self, _time: Union[datetime, str], confirm_block_count: int=0, features: Optional[list]=None) -> None:
         """
         Start a new block
@@ -170,59 +172,48 @@
         blacklist = json.dumps(blacklist)
         _chain.set_action_blacklist(self.ptr, blacklist)
 
     def set_key_blacklist(self, blacklist) -> None:
         blacklist = json.dumps(blacklist)
         _chain.set_key_blacklist(self.ptr, blacklist)
 
+
     def head_block_num(self) -> int:
         return _chain.head_block_num(self.ptr)
 
-    def head_block_time(self) -> datetime:
-        iso_time = _chain.head_block_time(self.ptr)
-        return datetime.strptime(iso_time, "%Y-%m-%dT%H:%M:%S.%f")
+    def head_block_time(self) -> int:
+        return _chain.head_block_time(self.ptr)
 
-    def head_block_id(self) -> str:
-        return _chain.head_block_id(self.ptr)
+    def head_block_id(self) -> Checksum256:
+        block_id = _chain.head_block_id(self.ptr)
+        return Checksum256.from_string(block_id)
 
     def head_block_producer(self) -> Name:
         return _chain.head_block_producer(self.ptr)
 
     def head_block_header(self) -> dict:
         ret = _chain.head_block_header(self.ptr)
         return json.loads(ret)
 
     def head_block_state(self) -> dict:
         ret = _chain.head_block_state(self.ptr)
         return json.loads(ret)
 
+    def earliest_available_block_num(self) -> U32:
+        return _chain.earliest_available_block_num(self.ptr)
+
+    def last_irreversible_block_time(self) -> I64:
+        return _chain.last_irreversible_block_time(self.ptr)
+
     def fork_db_head_block_num(self) -> int:
         return _chain.fork_db_head_block_num(self.ptr)
 
     def fork_db_head_block_id(self) -> str:
         return _chain.fork_db_head_block_id(self.ptr)
 
-    def fork_db_head_block_time(self) -> str:
-        return _chain.fork_db_head_block_time(self.ptr)
-
-    def fork_db_head_block_producer(self) -> Name:
-        return _chain.fork_db_head_block_producer(self.ptr)
-
-    def fork_db_pending_head_block_num(self) -> int:
-        return _chain.fork_db_pending_head_block_num(self.ptr)
-
-    def fork_db_pending_head_block_id(self) -> str:
-        return _chain.fork_db_pending_head_block_id(self.ptr)
-
-    def fork_db_pending_head_block_time(self) -> str:
-        return _chain.fork_db_pending_head_block_time(self.ptr)
-
-    def fork_db_pending_head_block_producer(self) -> Name:
-        return _chain.fork_db_pending_head_block_producer(self.ptr)
-
     def pending_block_time(self) -> int:
         return _chain.pending_block_time(self.ptr)
 
     def pending_block_producer(self) -> Name:
         return _chain.pending_block_producer(self.ptr)
 
     def pending_block_signing_key(self) -> str:
@@ -243,19 +234,21 @@
         ret = _chain.pending_producers(self.ptr)
         return json.loads(ret)
 
     def proposed_producers(self) -> dict:
         ret = _chain.proposed_producers(self.ptr)
         return json.loads(ret)
 
+
     def last_irreversible_block_num(self) -> int:
         return _chain.last_irreversible_block_num(self.ptr)
 
-    def last_irreversible_block_id(self) -> str:
-        return _chain.last_irreversible_block_id(self.ptr)
+    def last_irreversible_block_id(self) -> Checksum256:
+        block_id = _chain.last_irreversible_block_id(self.ptr)
+        return Checksum256.from_string(block_id)
 
     def fetch_block_by_number(self, block_num) -> bytes:
         return _chain.fetch_block_by_number(self.ptr, block_num, raw_block)
 
     def fetch_block_by_id(self, block_id) -> bytes:
         return _chain.fetch_block_by_id(self.ptr, block_id)
 
@@ -355,17 +348,14 @@
 
     def contracts_console(self) -> bool:
         return _chain.contracts_console(self.ptr)
 
     def is_uuos_mainnet(self) -> bool:
         return _chain.is_uuos_mainnet(self.ptr)
 
-    def id(self) -> str:
-        return _chain.id(self.ptr)
-
     def get_read_mode(self) -> int:
         return _chain.get_read_mode(self.ptr)
 
     def get_validation_mode(self) -> int:
         return _chain.get_validation_mode(self.ptr)
 
     def set_subjective_cpu_leeway(self, leeway: int) -> None:
@@ -405,28 +395,37 @@
         if not result:
             result = _eos.get_last_error_and_clear()
         result = json.loads(result)
         if 'except' in result:
             raise Exception(result)
         return result
 
-    def push_block(self, log: BlockLog, block_num: int) -> bool:
-        if block_num > log.head_block_num() or block_num < log.first_block_num():
-            raise Exception("invalid block number, block_num: %d, head_block_num: %d, first_block_num: %d" % (block_num, log.head_block_num(), log.first_block_num()))
-        ret = _chain.push_block(self.ptr, log.get_block_log_ptr(), block_num)
+    def push_block(self, blog: BlockLog, block_num: int) -> bool:
+        if block_num > blog.head_block_num() or block_num < blog.first_block_num():
+            raise Exception("invalid block number, block_num: %d, head_block_num: %d, first_block_num: %d" % (block_num, blog.head_block_num(), blog.first_block_num()))
+        ret = _chain.push_block(self.ptr, blog.get_block_log_ptr(), block_num)
         if not ret:
             err = _eos.get_last_error_and_clear()
             if err:
                 raise Exception(err)
             else:
                 raise Exception("invalid block num")
         return True
 
-    def get_scheduled_transaction(self, sender_id: int, sender: Name) -> dict:
-        ret = _chain.get_scheduled_transaction(self.ptr, sender_id, sender)
+    def push_raw_block(self, raw_block: bytes) -> bool:
+        ret = _chain.push_raw_block(self.ptr, raw_block)
+        if not ret:
+            err = _eos.get_last_error_and_clear()
+            if err:
+                raise Exception(err)
+            raise Exception("unknown error")
+        return True
+
+    def get_scheduled_transaction(self, sender_id: U128, sender: Name) -> dict:
+        ret = _chain.get_scheduled_transaction(self.ptr, sender_id.to_bytes(16, 'little'), sender)
         if ret:
             return json.loads(ret)
 
     def get_scheduled_transactions(self) -> dict:
         ret = _chain.get_scheduled_transactions(self.ptr)
         return json.loads(ret)
 
@@ -475,24 +474,22 @@
                 args = b''
         return _chain.pack_action_args(self.ptr, name, action, args)
 
     def unpack_action_args(self, name: Name, action: Name, raw_args: bytes) -> dict:
         ret = _chain.unpack_action_args(self.ptr, name, action, raw_args)
         return json.loads(ret)
 
-    def gen_transaction(self, json_str, _actions: List, expiration: datetime, reference_block_id: str, _id: str, compress: bool, _private_keys: List) -> str:
-        if isinstance(expiration, datetime):
-            expiration = isoformat(expiration)
-
+    def gen_transaction(self, json_str, _actions: List, expiration: int, reference_block_id: str, _id: Union[str, Checksum256], compress: bool, _private_keys: List) -> str:
         if isinstance(_actions, list):
             _actions = json.dumps(_actions)
 
         if isinstance(_private_keys, list):
             _private_keys = json.dumps(_private_keys)
-
+        if isinstance(_id, Checksum256):
+            _id = _id.to_string()
         return _chain.gen_transaction(self.ptr, json_str, _actions, expiration, reference_block_id, _id, compress, _private_keys)
 
     def get_last_error(self) -> str:
         err = _eos.get_last_error_and_clear()
         try:
             return {'except': json.loads(err)}
         except json.JSONDecodeError:        
@@ -500,7 +497,13 @@
             return f'{{"except": {err}}}'
 
     def get_native_contract(self, contract: str) -> str:
         return _chain.get_native_contract(self.ptr, contract)
 
     def set_native_contract(self, contract: str, native_contract_lib: str) -> bool:
         return _chain.set_native_contract(self.ptr, contract, native_contract_lib)
+
+    def set_debug_producer_key(self, pub_key: str):
+        _chain.set_debug_producer_key(self.ptr, pub_key)
+
+    def get_debug_producer_key(self) -> str:
+        return _chain(self.ptr).get_debug_producer_key()
```

### Comparing `ipyeos-0.4.4/pysrc/chainapi.py` & `ipyeos-0.4.5/pysrc/chainapi.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/chaintester.py` & `ipyeos-0.4.5/pysrc/chaintester.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import os
 import shutil
 import subprocess
 import tempfile
 from datetime import datetime, timedelta, timezone
 from typing import Dict, List, Optional, Union
 
-import pytest
+from .modules import load_modules
+load_modules()
 
 from ipyeos import chain, chainapi, database, config
 
 from . import eos, log
 from .types import Name
 
 from .packer import Decoder
@@ -76,30 +77,29 @@
 
 genesis_test = {
   "initial_timestamp": "2018-06-01T12:00:00.000",
   "initial_key": "EOS6MRyAjQq8ud7hVNYcfnVPJqcVpscN5So8BhtHuGYqET5GDW5CV",
   "initial_configuration": {
     "max_block_net_usage": 1048576,
     "target_block_net_usage_pct": 1000,
-    "max_transaction_net_usage": 652441,
+    "max_transaction_net_usage": 524288,
     "base_per_transaction_net_usage": 12,
     "net_usage_leeway": 500,
     "context_free_discount_net_usage_num": 20,
     "context_free_discount_net_usage_den": 100,
-    "max_block_cpu_usage": 450000,
+    "max_block_cpu_usage": 200000,
     "target_block_cpu_usage_pct": 1000,
-    "max_transaction_cpu_usage": 300000,
+    "max_transaction_cpu_usage": 150000,
     "min_transaction_cpu_usage": 100,
     "max_transaction_lifetime": 3600,
     "deferred_trx_expiration_window": 600,
     "max_transaction_delay": 3888000,
     "max_inline_action_size": 524288,
     "max_inline_action_depth": 4,
-    "max_authority_depth": 6,
-    "max_action_return_value_size": 256,
+    "max_authority_depth": 6
   }
 }
 
 key_map = {
     'EOS6MRyAjQq8ud7hVNYcfnVPJqcVpscN5So8BhtHuGYqET5GDW5CV':'5KQwrPbwdL6PhXujxW37FSSQZ1JiwsST4cqQzDeyXtP79zkvFD3',
     'EOS61MgZLN7Frbc2J7giU7JdYjy2TqnfWFjZuLXvpHJoKzWAj7Nst':'5JEcwbckBCdmji5j8ZoMHLEUS8TqQiqBG1DRx1X9DN124GUok9s',
     'EOS5JuNfuZPATy8oPz9KMZV2asKf9m8fb2bSzftvhW55FKQFakzFL':'5JbDP55GXN7MLcNYKCnJtfKi9aD2HvHAdY7g8m67zFTAFkY1uBB',
@@ -191,19 +191,19 @@
         return hashlib.sha256(data).hexdigest()
     elif contains_chain_id(ver, first_block_num):
         return dec.read_bytes(32).hex()
     assert False, "unknown chain id"
 
 class ChainTester(object):
 
-    def __init__(self, initialize=True, data_dir=None, config_dir=None, snapshot_dir='', state_size=10*1024*1024, log_level=log_level_debug):
+    def __init__(self, initialize=True, data_dir=None, config_dir=None, snapshot_dir='', state_size=10*1024*1024, log_level=log_level_debug, debug_producer_key=''):
         atexit.register(self.free)
         self.is_temp_data_dir = True
         self.is_temp_config_dir = True
-
+        self.debug_producer_key=debug_producer_key
         chain_config['state_size'] = state_size
         chain_config['state_guard_size'] = int(state_size * 0.005)
 
         if data_dir:
             self.data_dir = data_dir
             self.is_temp_data_dir = False
         else:
@@ -236,15 +236,15 @@
             self.chain_id = read_chain_id_from_block_log(self.data_dir)
         else:
             init_database = True
             self.chain_id = ''
 
         self.chain_config = json.dumps(chain_config)
         self.genesis_test = json.dumps(genesis_test)
-        self.chain = chain.Chain(self.chain_config, self.genesis_test, self.chain_id, os.path.join(self.config_dir, "protocol_features"), snapshot_dir)
+        self.chain = chain.Chain(self.chain_config, self.genesis_test, self.chain_id, os.path.join(self.config_dir, "protocol_features"), snapshot_dir, debug_producer_key)
         self.chain.startup(init_database)
         self.api = chainapi.ChainApi(self.chain)
 
         self.db = database.Database(self.chain.get_database())
 
         # logger.info(self.api.get_info())
         # logger.info(self.api.get_account('eosio'))
@@ -495,19 +495,19 @@
         }
         ret = self.push_actions_ex([a], explicit_cpu_bill)
         # elapsed = ret['elapsed']
         # if not action == 'activate':
         #     logger.info(f'+++++{account} {action} {elapsed}')
         return ret
 
-    def gen_transaction(self, actions: List, json_str=False):
+    def gen_transaction(self, actions: List, json_str=False, compress=False):
         _actions = []
         for a in actions:
             _actions.append(self.gen_action(*a))
-        return self.gen_transaction_ex(_actions, json_str)
+        return self.gen_transaction_ex(_actions, json_str, compress)
 
     def get_required_keys(self, actions):
         fake_tx = {
             "expiration": "2021-09-01T16:15:16",
             "ref_block_num": 20676,
             "ref_block_prefix": 4052960473,
             "max_net_usage_words": 0,
@@ -534,17 +534,17 @@
     def get_required_private_keys(self, actions):
         required_keys = self.get_required_keys(actions)
         priv_keys = []
         for key in required_keys:
             priv_keys.append(key_map[key])
         return priv_keys
 
-    def gen_transaction_ex(self, actions: List, json_str=False):
-        chain_id = self.chain.id()
-        ref_block_id = self.chain.last_irreversible_block_id()
+    def gen_transaction_ex(self, actions: List, json_str=False, compress=False):
+        chain_id = self.chain.chain_id()
+        ref_block_id = self.chain.last_irreversible_block_id().to_string()
 
         priv_keys = self.get_required_private_keys(actions)
 
         for a in actions:
             if isinstance(a['data'], dict):
                 data = self.chain.pack_action_args(a['account'], a['name'], a['data'])
                 a['data'] = data.hex()
@@ -556,16 +556,16 @@
         actions = json.dumps(actions)
         # expiration = datetime.utcnow() + timedelta(seconds=60*60)
 
         expiration = self.chain.head_block_time()
         # now = datetime.utcnow()
         # if expiration < now:
         #     expiration = now
-        expiration = expiration + timedelta(seconds=60)
-        ret = self.chain.gen_transaction(json_str, actions, expiration, ref_block_id, chain_id, False, priv_keys)
+        expiration = expiration + 60*1e6
+        ret = self.chain.gen_transaction(json_str, actions, expiration, ref_block_id, chain_id, compress, priv_keys)
         if json_str:
             return json.loads(ret)
         return ret
 
     def push_actions(self, actions: List, explicit_cpu_bill=False):
         _actions = []
         for a in actions:
@@ -585,15 +585,15 @@
 
     def calc_pending_block_time(self):
         # base = self.chain.head_block_time()
         # return base + timedelta(microseconds=config.block_interval_us)
 
 #        self.chain.abort_block()
         now = datetime.utcnow()
-        base = self.chain.head_block_time()
+        base = self.chain.head_block_time
         if base < now:
             base = now
         min_time_to_next_block = config.block_interval_us - int(base.timestamp()*1e6) % config.block_interval_us
         # print('min_time_to_next_block:', min_time_to_next_block)
         block_time = base + timedelta(microseconds=min_time_to_next_block)
         if block_time - now < timedelta(microseconds=config.block_interval_us/10):
             # block_time += timedelta(microseconds=config.block_interval_us)
```

### Comparing `ipyeos-0.4.4/pysrc/config.py` & `ipyeos-0.4.5/pysrc/config.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/database.py` & `ipyeos-0.4.5/pysrc/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union, Tuple
 
 from . import _database
 from . import _eos
 from .types import U8, U16, U32, U64, I64, F64, Name, Checksum256
 from .packer import Encoder, Decoder
 from .database_objects import *
-from . import utils
+from .utils import i2b, u2b, f2b, to_bytes
 
 null_object_type = 0
 account_object_type = 1
 account_metadata_object_type = 2
 permission_object_type = 3
 permission_usage_object_type = 4
 permission_link_object_type = 5
@@ -47,24 +47,41 @@
 # UNUSED_account_history_object_type = 35 #              ///< Defined by history_plugin
 # UNUSED_action_history_object_type = 36 #               ///< Defined by history_plugin
 # UNUSED_reversible_block_object_type = 37
 protocol_state_object_type = 38
 account_ram_correction_object_type = 39
 code_object_type = 40
 database_header_object_type = 41
-      
+
+def parse_return_value(ret: int):
+    if ret == -2:
+        raise Exception(_eos.get_last_error_and_clear())
+    assert ret in (0, 1)
+    if ret:
+        return True
+    return False
+
 class Database:
     def __init__(self, db_ptr: int = 0):
         if not db_ptr:
             # default to get db ptr from chain_plugin.chain.db()
             self.db_ptr = _eos.get_database()
         else:
             self.db_ptr = db_ptr
         self.ptr = _database.new()
 
+    def create(self, tp, raw_data: bytes):
+        ret = _database.create(self.ptr, self.db_ptr, tp, raw_data)
+        if ret == -2:
+            raise Exception(_eos.get_last_error_and_clear())
+        assert ret in (0, 1)
+        if ret:
+            return True
+        return False
+
     def modify(self, tp: int, index_position: int, raw_key: bytes, raw_data: bytes):
         ret = _database.modify(self.ptr, self.db_ptr, tp, index_position, raw_key, raw_data)
         if ret == -2:
             raise Exception(_eos.get_last_error_and_clear())
         assert ret in (0, 1)
         if ret:
             return True
@@ -75,46 +92,46 @@
         if ret == -2:
             raise Exception(_eos.get_last_error_and_clear())
         return ret
 
     def walk_range(self, tp: int, index_position: int, lower_bound: Union[int, bytes], upper_bound: Union[int, bytes], cb, custom_data = None):
         if index_position == 0:
             if isinstance(lower_bound, int):
-                lower_bound = int.to_bytes(lower_bound, 8, 'little')
+                lower_bound = i2b(lower_bound)
             if isinstance(upper_bound, int):
-                upper_bound = int.to_bytes(upper_bound, 8, 'little')
+                upper_bound = i2b(upper_bound)
 
         ret = _database.walk_range(self.ptr, self.db_ptr, tp, index_position, lower_bound, upper_bound, cb, custom_data)
         if ret == -2:
             raise Exception(_eos.get_last_error_and_clear())
         return ret
 
     def find(self, tp: int, index_position: int, key: Union[int, bytes]):
         if index_position == 0 and isinstance(key, int):
-            key = int.to_bytes(key, 8, 'little')
+            key = i2b(key)
         ret, data = _database.find(self.ptr, self.db_ptr, tp, index_position, key)
         if ret == -2:
             raise Exception(_eos.get_last_error_and_clear())
         if ret == 0:
             return None
         return data
 
     def lower_bound(self, tp: int, index_position: int, key: Union[int, bytes]):
         if index_position == 0 and isinstance(key, int):
-            key = int.to_bytes(key, 8, 'little')
+            key = i2b(key)
         ret, data = _database.lower_bound(self.ptr, self.db_ptr, tp, index_position, key)
         if ret == -2:
             raise Exception(_eos.get_last_error_and_clear())
         if ret == 0:
             return None
         return data
 
     def upper_bound(self, tp: int, index_position: int, key: Union[int, bytes]):
         if index_position == 0 and isinstance(key, int):
-            key = int.to_bytes(key, 8, 'little')
+            key = i2b(key, 8)
 
         ret, data = _database.upper_bound(self.ptr, self.db_ptr, tp, index_position, key)
         if ret == -2:
             raise Exception(_eos.get_last_error_and_clear())
         if ret == 0:
             return None
         return data
@@ -126,19 +143,25 @@
         return ret
 
 # account_object_type = 1
 class AccountObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: AccountObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(account_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(account_object_type, AccountObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return AccountObject.unpack(dec)
 
     def find_by_name(self, account: Name):
@@ -160,25 +183,25 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(account_object_type, AccountObject.by_id, self.on_object_data, (cb, raw_data, user_data))
     
     def walk_by_name(self, cb, user_data=None, raw_data=False):
         return self.db.walk(account_object_type, AccountObject.by_name, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(account_object_type, AccountObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_name(self, lower_bound: Name, upper_bound: Name, cb, user_data=None, raw_data=False):
         lower_bound = eos.s2b(lower_bound)
         upper_bound = eos.s2b(upper_bound)
         return self.db.walk_range(account_object_type, AccountObject.by_name, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(account_object_type, AccountObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountObject.unpack(dec)
 
     def lower_bound_by_name(self, lower_bound: Name):
@@ -186,15 +209,15 @@
         data = self.db.lower_bound(account_object_type, AccountObject.by_name, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(account_object_type, AccountObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountObject.unpack(dec)
 
     def upper_bound_by_name(self, upper_bound: Name):
@@ -202,32 +225,38 @@
         data = self.db.upper_bound(account_object_type, AccountObject.by_name, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountObject.unpack(dec)
 
     def modify(self, perm: AccountObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(account_object_type, AccountObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(account_object_type)
 
 # account_metadata_object_type = 2
 class AccountMetadataObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: AccountMetadataObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(account_metadata_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(account_metadata_object_type, AccountMetadataObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return AccountMetadataObject.unpack(dec)
     
     def find_by_name(self, name: Name):
@@ -249,25 +278,25 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(account_metadata_object_type, AccountMetadataObject.by_id, self.on_object_data, (cb, raw_data, user_data))
     
     def walk_by_name(self, cb, user_data=None, raw_data=False):
         return self.db.walk(account_metadata_object_type, AccountMetadataObject.by_name, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(account_metadata_object_type, AccountMetadataObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_name(self, lower_bound: Name, upper_bound: Name, cb, user_data=None, raw_data=False):
         lower_bound = eos.s2b(lower_bound)
         upper_bound = eos.s2b(upper_bound)
         return self.db.walk_range(account_metadata_object_type, AccountMetadataObject.by_name, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(account_metadata_object_type, AccountMetadataObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountMetadataObject.unpack(dec)
 
     def lower_bound_by_name(self, lower_bound: Name):
@@ -275,15 +304,15 @@
         data = self.db.lower_bound(account_metadata_object_type, AccountMetadataObject.by_name, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountMetadataObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(account_metadata_object_type, AccountMetadataObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountMetadataObject.unpack(dec)
 
     def upper_bound_by_name(self, upper_bound: Name):
@@ -291,33 +320,39 @@
         data = self.db.upper_bound(account_metadata_object_type, AccountMetadataObject.by_name, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return AccountMetadataObject.unpack(dec)
 
     def modify(self, perm: AccountMetadataObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(account_metadata_object_type, AccountMetadataObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(account_metadata_object_type)
 
 # permission_object_type = 3
 class PermissionObjectIndex(object):
     
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: PermissionObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(permission_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(permission_object_type, PermissionObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionObject.unpack(dec)
     
     def find_by_parent(self, parent: I64, table_id: I64):
@@ -346,14 +381,23 @@
         key = PermissionObject.generate_key_by_name(name, table_id)
         data = self.db.find(permission_object_type, PermissionObject.by_name, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionObject.unpack(dec)
 
+    def modify(self, perm: PermissionObject):
+        key = i2b(perm.table_id)
+        enc = Encoder()
+        enc.pack(perm)
+        return self.db.modify(permission_object_type, PermissionObject.by_id, key, enc.get_bytes())
+
+    def row_count(self):
+        return self.db.row_count(permission_object_type)
+
     def on_object_data(self, tp, data, custom_data):
         cb, raw_data, user_data = custom_data
         if raw_data:
             return cb(data, user_data)
         dec = Decoder(data)
         obj = PermissionObject.unpack(dec)
         return cb(obj, user_data)
@@ -367,16 +411,16 @@
     def walk_by_owner(self, cb, user_data=None, raw_data=False):
         return self.db.walk(permission_object_type, PermissionObject.by_owner, self.on_object_data, (cb, raw_data, user_data))
     
     def walk_by_name(self, cb, user_data=None, raw_data=False):
         return self.db.walk(permission_object_type, PermissionObject.by_name, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(permission_object_type, PermissionObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_parent(self, lower_bound: Tuple[I64, I64], upper_bound: Tuple[I64, I64], cb, user_data=None, raw_data=False):
         lower_bound = PermissionObject.generate_key_by_parent(*lower_bound)
         upper_bound = PermissionObject.generate_key_by_parent(*upper_bound)
         return self.db.walk_range(permission_object_type, PermissionObject.by_parent, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
@@ -387,15 +431,15 @@
 
     def walk_range_by_name(self, lower_bound: Tuple[Name, I64], upper_bound: Tuple[Name, I64], cb, user_data=None, raw_data=False):
         lower_bound = PermissionObject.generate_key_by_name(*lower_bound)
         upper_bound = PermissionObject.generate_key_by_name(*upper_bound)
         return self.db.walk_range(permission_object_type, PermissionObject.by_name, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.lower_bound(permission_object_type, PermissionObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionObject.unpack(dec)
 
     def lower_bound_by_parent(self, parent: I64, table_id: I64):
@@ -419,15 +463,15 @@
         data = self.db.lower_bound(permission_object_type, PermissionObject.by_name, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionObject.unpack(dec)
 
     def upper_bound_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.upper_bound(permission_object_type, PermissionObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionObject.unpack(dec)
 
     def upper_bound_by_parent(self, parent: I64, table_id: I64):
@@ -450,38 +494,38 @@
         key = PermissionObject.generate_key_by_name(name, table_id)
         data = self.db.upper_bound(permission_object_type, PermissionObject.by_name, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionObject.unpack(dec)
 
-    def modify(self, perm: PermissionObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
-        enc = Encoder()
-        enc.pack(perm)
-        return self.db.modify(permission_object_type, PermissionObject.by_id, key, enc.get_bytes())
-
 # permission_usage_object_type = 4
 class PermissionUsageObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: PermissionUsageObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(permission_usage_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(permission_usage_object_type, PermissionUsageObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionUsageObject.unpack(dec)
 
     def modify(self, perm: PermissionUsageObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(permission_usage_object_type, PermissionUsageObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(permission_usage_object_type)
 
@@ -493,44 +537,50 @@
         obj = PermissionUsageObject.unpack(dec)
         return cb(obj, user_data)
 
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(permission_usage_object_type, PermissionUsageObject.by_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(permission_usage_object_type, PermissionUsageObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(permission_usage_object_type, PermissionUsageObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionUsageObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(permission_usage_object_type, PermissionUsageObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionUsageObject.unpack(dec)
 
 # permission_link_object_type = 5
 class PermissionLinkObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: PermissionLinkObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(permission_link_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(permission_link_object_type, PermissionLinkObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionLinkObject.unpack(dec)
     
     def find_by_action_name(self, action: Name, code: Name, message_type: Name):
@@ -546,15 +596,15 @@
         data = self.db.find(permission_link_object_type, PermissionLinkObject.by_permission_name, key)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionLinkObject.unpack(dec)
 
     def modify(self, perm: PermissionLinkObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(permission_link_object_type, PermissionLinkObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(permission_link_object_type)
 
@@ -572,30 +622,30 @@
     def walk_by_action_name(self, cb, user_data=None, raw_data=False):
         return self.db.walk(permission_link_object_type, PermissionLinkObject.by_action_name, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_permission_name(self, cb, user_data=None, raw_data=False):
         return self.db.walk(permission_link_object_type, PermissionLinkObject.by_permission_name, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(permission_link_object_type, PermissionLinkObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_action_name(self, lower_bound: Tuple[Name, Name, Name], upper_bound: Tuple[Name, Name, Name], cb, user_data=None, raw_data=False):
         lower_bound = PermissionLinkObject.generate_key_by_action_name(*lower_bound)
         upper_bound = PermissionLinkObject.generate_key_by_action_name(*upper_bound)
         return self.db.walk_range(permission_link_object_type, PermissionLinkObject.by_action_name, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_permission_name(self, lower_bound: Tuple[Name, Name, I64], upper_bound: Tuple[Name, Name, I64], cb, user_data=None, raw_data=False):
         lower_bound = PermissionLinkObject.generate_key_by_permission_name(*lower_bound)
         upper_bound = PermissionLinkObject.generate_key_by_permission_name(*upper_bound)
         return self.db.walk_range(permission_link_object_type, PermissionLinkObject.by_permission_name, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(permission_link_object_type, PermissionLinkObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionLinkObject.unpack(dec)
 
     def lower_bound_by_action_name(self, lower_bound: Tuple[Name, Name, Name]):
@@ -611,15 +661,15 @@
         data = self.db.lower_bound(permission_link_object_type, PermissionLinkObject.by_permission_name, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionLinkObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(permission_link_object_type, PermissionLinkObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return PermissionLinkObject.unpack(dec)
 
     def upper_bound_by_action_name(self, upper_bound: Tuple[Name, Name, Name]):
@@ -640,19 +690,25 @@
 
 
 # key_value_object_type = 7
 class KeyValueObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: KeyValueObject):
+        enc = Encoder()
+        perm.pack(enc)
+        ret = self.db.create(key_value_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(key_value_object_type, KeyValueObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return KeyValueObject.unpack(dec)
     
     def find_by_scope_primary(self, t_id: I64, primary_key: U64):
@@ -660,15 +716,15 @@
         data = self.db.find(key_value_object_type, KeyValueObject.by_scope_primary, key)
         if not data:
             return None
         dec = Decoder(data)
         return KeyValueObject.unpack(dec)
 
     def modify(self, perm: KeyValueObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(key_value_object_type, KeyValueObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(key_value_object_type)
 
@@ -683,25 +739,25 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(key_value_object_type, KeyValueObject.by_id, self.on_object_data, (cb, raw_data, user_data))
     
     def walk_by_scope_primary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(key_value_object_type, KeyValueObject.by_scope_primary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(key_value_object_type, KeyValueObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_scope_primary(self, lower_bound: Tuple[I64, U64], upper_bound: Tuple[I64, U64], cb, user_data=None, raw_data=False):
         lower_bound = KeyValueObject.generate_key_by_scope_primary(*lower_bound)
         upper_bound = KeyValueObject.generate_key_by_scope_primary(*upper_bound)
         return self.db.walk_range(key_value_object_type, KeyValueObject.by_scope_primary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(key_value_object_type, KeyValueObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return KeyValueObject.unpack(dec)
 
     def lower_bound_by_scope_primary(self, lower_bound: Tuple[I64, U64]):
@@ -709,15 +765,15 @@
         data = self.db.lower_bound(key_value_object_type, KeyValueObject.by_scope_primary, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return KeyValueObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(key_value_object_type, KeyValueObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return KeyValueObject.unpack(dec)
     
     def upper_bound_by_scope_primary(self, upper_bound: Tuple[I64, U64]):
@@ -729,43 +785,49 @@
         return KeyValueObject.unpack(dec)
 
 # index64_object_type = 8
 class Index64ObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: Index64Object):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(index64_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(index64_object_type, Index64Object.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index64Object.unpack(dec)
     
     def find_by_primary(self, t_id: I64, primary_key: U64):
-        key = int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        key = i2b(t_id) + u2b(primary_key)
         data = self.db.find(index64_object_type, Index64Object.by_primary, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index64Object.unpack(dec)
 
     def find_by_secondary(self, t_id: I64, secondary_key: U64, primary_key: U64):
-        key = utils.to_bytes(t_id, signed=True) + utils.to_bytes(secondary_key) + utils.to_bytes(primary_key)
+        key = i2b(t_id) + u2b(secondary_key) + u2b(primary_key)
         data = self.db.find(index64_object_type, Index64Object.by_secondary, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index64Object.unpack(dec)
 
     def modify(self, perm: Index64Object):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(index64_object_type, Index64Object.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(index64_object_type)
 
@@ -783,30 +845,30 @@
     def walk_by_primary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index64_object_type, Index64Object.by_primary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_secondary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index64_object_type, Index64Object.by_secondary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little')
-        upper_bound = int.to_bytes(upper_bound, 8, 'little')
+        lower_bound = u2b(lower_bound)
+        upper_bound = u2b(upper_bound)
         return self.db.walk_range(index64_object_type, Index64Object.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_primary(self, lower_bound: Tuple[I64, U64], upper_bound: Tuple[I64, U64], cb, user_data=None, raw_data=False):
         lower_bound = Index64Object.generate_key_by_primary(*lower_bound)
         upper_bound = Index64Object.generate_key_by_primary(*upper_bound)
         return self.db.walk_range(index64_object_type, Index64Object.by_primary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_secondary(self, lower_bound: Tuple[I64, U64, U64], upper_bound: Tuple[I64, U64, U64], cb, user_data=None, raw_data=False):
         lower_bound = Index64Object.generate_key_by_secondary(*lower_bound)
         upper_bound = Index64Object.generate_key_by_secondary(*upper_bound)
         return self.db.walk_range(index64_object_type, Index64Object.by_secondary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little')
+        lower_bound = u2b(lower_bound)
         data = self.db.lower_bound(index64_object_type, Index64Object.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index64Object.unpack(dec)
 
     def lower_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -822,15 +884,15 @@
         data = self.db.lower_bound(index64_object_type, Index64Object.by_secondary, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index64Object.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little')
+        upper_bound = u2b(upper_bound)
         data = self.db.upper_bound(index64_object_type, Index64Object.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index64Object.unpack(dec)
 
     def upper_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -850,43 +912,49 @@
         return Index64Object.unpack(dec)
 
 # index128_object_type = 9
 class Index128ObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: Index128Object):
+        enc = Encoder()
+        obj.pack(enc)
+        ret = self.db.create(index128_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(index128_object_type, Index128Object.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index128Object.unpack(dec)
     
     def find_by_primary(self, t_id: I64, primary_key: U64):
-        key = int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        key = i2b(t_id) + u2b(primary_key)
         data = self.db.find(index128_object_type, Index128Object.by_primary, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index128Object.unpack(dec)
     
     def find_by_secondary(self, t_id: I64, secondary_key: U128, primary_key: U64):
-        key = utils.to_bytes(t_id, signed=True) + utils.to_bytes(secondary_key, 16) + utils.to_bytes(primary_key)
+        key = i2b(t_id) + u2b(secondary_key, 16) + u2b(primary_key)
         data = self.db.find(index128_object_type, Index128Object.by_secondary, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index128Object.unpack(dec)
 
     def modify(self, perm: Index128Object):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(index128_object_type, Index128Object.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(index128_object_type)
 
@@ -904,30 +972,30 @@
     def walk_by_primary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index128_object_type, Index128Object.by_primary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_secondary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index128_object_type, Index128Object.by_secondary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(index128_object_type, Index128Object.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_primary(self, lower_bound: Tuple[I64, U64], upper_bound: Tuple[I64, U64], cb, user_data=None, raw_data=False):
         lower_bound = Index128Object.generate_key_by_primary(*lower_bound)
         upper_bound = Index128Object.generate_key_by_primary(*upper_bound)
         return self.db.walk_range(index128_object_type, Index128Object.by_primary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_secondary(self, lower_bound: Tuple[I64, U128, U64], upper_bound: Tuple[I64, U128, U64], cb, user_data=None, raw_data=False):
         lower_bound = Index128Object.generate_key_by_secondary(*lower_bound)
         upper_bound = Index128Object.generate_key_by_secondary(*upper_bound)
         return self.db.walk_range(index128_object_type, Index128Object.by_secondary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(index128_object_type, Index128Object.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index128Object.unpack(dec)
 
     def lower_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -943,15 +1011,15 @@
         data = self.db.lower_bound(index128_object_type, Index128Object.by_secondary, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index128Object.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(index128_object_type, Index128Object.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index128Object.unpack(dec)
 
     def upper_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -971,43 +1039,49 @@
         return Index128Object.unpack(dec)
 
 # index256_object_type = 10
 class Index256ObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: Index256Object):
+        enc = Encoder()
+        obj.pack(enc)
+        ret = self.db.create(index256_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(index256_object_type, Index256Object.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index256Object.unpack(dec)
     
     def find_by_primary(self, t_id: I64, primary_key: U64):
-        key = int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        key = i2b(t_id) + u2b(primary_key)
         data = self.db.find(index256_object_type, Index256Object.by_primary, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index256Object.unpack(dec)
     
     def find_by_secondary(self, t_id: I64, secondary_key: U256, primary_key: U64):
-        key = utils.to_bytes(t_id, signed=True) + utils.to_bytes(secondary_key, 32) + utils.to_bytes(primary_key)
+        key = i2b(t_id) + u2b(secondary_key, 32) + u2b(primary_key)
         data = self.db.find(index256_object_type, Index256Object.by_secondary, key)
         if not data:
             return None
         dec = Decoder(data)
         return Index256Object.unpack(dec)
 
     def modify(self, perm: Index256Object):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(index256_object_type, Index256Object.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(index256_object_type)
 
@@ -1025,30 +1099,30 @@
     def walk_by_primary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index256_object_type, Index256Object.by_primary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_secondary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index256_object_type, Index256Object.by_secondary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(index256_object_type, Index256Object.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_primary(self, lower_bound: Tuple[I64, U64], upper_bound: Tuple[I64, U64], cb, user_data=None, raw_data=False):
         lower_bound = Index256Object.generate_key_by_primary(*lower_bound)
         upper_bound = Index256Object.generate_key_by_primary(*upper_bound)
         return self.db.walk_range(index256_object_type, Index256Object.by_primary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_secondary(self, lower_bound: Tuple[I64, U256, U64], upper_bound: Tuple[I64, U256, U64], cb, user_data=None, raw_data=False):
         lower_bound = Index256Object.generate_key_by_secondary(*lower_bound)
         upper_bound = Index256Object.generate_key_by_secondary(*upper_bound)
         return self.db.walk_range(index256_object_type, Index256Object.by_secondary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(index256_object_type, Index256Object.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index256Object.unpack(dec)
 
     def lower_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -1064,15 +1138,15 @@
         data = self.db.lower_bound(index256_object_type, Index256Object.by_secondary, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index256Object.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(index256_object_type, Index256Object.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return Index256Object.unpack(dec)
     
     def upper_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -1092,43 +1166,49 @@
         return Index256Object.unpack(dec)
 
 # index_double_object_type = 11
 class IndexDoubleObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: IndexDoubleObject):
+        enc = Encoder()
+        obj.pack(enc)
+        ret = self.db.create(index_double_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(index_double_object_type, IndexDoubleObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return IndexDoubleObject.unpack(dec)
     
     def find_by_primary(self, t_id: I64, primary_key: U64):
-        key = int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        key = i2b(t_id) + u2b(primary_key)
         data = self.db.find(index_double_object_type, IndexDoubleObject.by_primary, key)
         if not data:
             return None
         dec = Decoder(data)
         return IndexDoubleObject.unpack(dec)
 
     def find_by_secondary(self, t_id: I64, secondary_key: F64, primary_key: U64):
-        key = utils.to_bytes(t_id) + utils.to_bytes(secondary_key) + utils.to_bytes(primary_key)
+        key = i2b(t_id) + f2b(secondary_key) + u2b(primary_key)
         data = self.db.find(index_double_object_type, IndexDoubleObject.by_secondary, key)
         if not data:
             return None
         dec = Decoder(data)
         return IndexDoubleObject.unpack(dec)
 
     def modify(self, perm: IndexDoubleObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(index_double_object_type, IndexDoubleObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(index_double_object_type)
 
@@ -1146,30 +1226,30 @@
     def walk_by_primary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index_double_object_type, IndexDoubleObject.by_primary, self.on_object_data, (cb, raw_data, user_data))
     
     def walk_by_secondary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index_double_object_type, IndexDoubleObject.by_secondary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(index_double_object_type, IndexDoubleObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_primary(self, lower_bound: Tuple[I64, U64], upper_bound: Tuple[I64, U64], cb, user_data=None, raw_data=False):
         lower_bound = IndexDoubleObject.generate_key_by_primary(*lower_bound)
         upper_bound = IndexDoubleObject.generate_key_by_primary(*upper_bound)
         return self.db.walk_range(index_double_object_type, IndexDoubleObject.by_primary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_secondary(self, lower_bound: Tuple[I64, F64, U64], upper_bound: Tuple[I64, F64, U64], cb, user_data=None, raw_data=False):
         lower_bound = IndexDoubleObject.generate_key_by_secondary(*lower_bound)
         upper_bound = IndexDoubleObject.generate_key_by_secondary(*upper_bound)
         return self.db.walk_range(index_double_object_type, IndexDoubleObject.by_secondary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(index_double_object_type, IndexDoubleObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return IndexDoubleObject.unpack(dec)
 
     def lower_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -1185,15 +1265,15 @@
         data = self.db.lower_bound(index_double_object_type, IndexDoubleObject.by_secondary, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return IndexDoubleObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(index_double_object_type, IndexDoubleObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return IndexDoubleObject.unpack(dec)
     
     def upper_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -1213,44 +1293,50 @@
         return IndexDoubleObject.unpack(dec)
 
 # index_long_double_object_type = 12
 class IndexLongDoubleObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: IndexLongDoubleObject):
+        enc = Encoder()
+        obj.pack(enc)
+        ret = self.db.create(index_long_double_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(index_long_double_object_type, IndexLongDoubleObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return IndexLongDoubleObject.unpack(dec)
 
     def find_by_primary(self, t_id: I64, primary_key: U64):
-        key = int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        key = i2b(t_id) + u2b(primary_key)
         data = self.db.find(index_long_double_object_type, IndexLongDoubleObject.by_primary, key)
         if not data:
             return None
         dec = Decoder(data)
         return IndexLongDoubleObject.unpack(dec)
 
     def find_by_secondary(self, t_id: I64, secondary_key: F128, primary_key: U64):
-        key = utils.to_bytes(t_id) + utils.to_bytes(secondary_key) + utils.to_bytes(primary_key)
+        key = i2b(t_id) + to_bytes(secondary_key) + u2b(primary_key)
         data = self.db.find(index_long_double_object_type, IndexLongDoubleObject.by_secondary, key)
         if not data:
             return None
         dec = Decoder(data)
         return IndexLongDoubleObject.unpack(dec)
 
 
     def modify(self, perm: IndexLongDoubleObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(index_long_double_object_type, IndexLongDoubleObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(index_long_double_object_type)
 
@@ -1268,30 +1354,30 @@
     def walk_by_primary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index_long_double_object_type, IndexLongDoubleObject.by_primary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_secondary(self, cb, user_data=None, raw_data=False):
         return self.db.walk(index_long_double_object_type, IndexLongDoubleObject.by_secondary, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(index_long_double_object_type, IndexLongDoubleObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_primary(self, lower_bound: Tuple[I64, U64], upper_bound: Tuple[I64, U64], cb, user_data=None, raw_data=False):
         lower_bound = IndexLongDoubleObject.generate_key_by_primary(*lower_bound)
         upper_bound = IndexLongDoubleObject.generate_key_by_primary(*upper_bound)
         return self.db.walk_range(index_long_double_object_type, IndexLongDoubleObject.by_primary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_secondary(self, lower_bound: Tuple[I64, F128, U64], upper_bound: Tuple[I64, F128, U64], cb, user_data=None, raw_data=False):
         lower_bound = IndexLongDoubleObject.generate_key_by_secondary(*lower_bound)
         upper_bound = IndexLongDoubleObject.generate_key_by_secondary(*upper_bound)
         return self.db.walk_range(index_long_double_object_type, IndexLongDoubleObject.by_secondary, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(index_long_double_object_type, IndexLongDoubleObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return IndexLongDoubleObject.unpack(dec)
 
     def lower_bound_by_primary(self, t_id: I64, lower_bound: U64):
@@ -1307,15 +1393,15 @@
         data = self.db.lower_bound(index_long_double_object_type, IndexLongDoubleObject.by_secondary, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return IndexLongDoubleObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(index_long_double_object_type, IndexLongDoubleObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return IndexLongDoubleObject.unpack(dec)
     
     def upper_bound_by_primary(self, t_id: I64, primary_key: U64):
@@ -1335,77 +1421,107 @@
         return IndexLongDoubleObject.unpack(dec)
 
 # global_property_object_type = 13
 class GlobalPropertyObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: GlobalPropertyObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(global_property_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
+    def get(self):
+        return self.find_by_id(0)
+
+    def set(self, perm: GlobalPropertyObject):
+        return self.modify(perm)
+
     def find(self):
         return self.find_by_id(0)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(global_property_object_type, GlobalPropertyObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return GlobalPropertyObject.unpack(dec)
 
     def modify(self, perm: GlobalPropertyObject):
-        key = int.to_bytes(0, 8, 'little', signed=True)
+        key = u2b(0)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(global_property_object_type, GlobalPropertyObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(global_property_object_type)
 
 # dynamic_global_property_object_type = 14
 class DynamicGlobalPropertyObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: DynamicGlobalPropertyObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(dynamic_global_property_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
+    def get(self):
+        return self.find_by_id(0)
+
+    def set(self, perm: DynamicGlobalPropertyObject):
+        return self.modify(perm)
+
     def find(self):
         return self.find_by_id(0)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(dynamic_global_property_object_type, DynamicGlobalPropertyObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return DynamicGlobalPropertyObject.unpack(dec)
 
     def modify(self, perm: DynamicGlobalPropertyObject):
-        key = int.to_bytes(0, 8, 'little', signed=True)
+        key = u2b(0)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(dynamic_global_property_object_type, DynamicGlobalPropertyObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(dynamic_global_property_object_type)
 
 # block_summary_object_type = 15
 class BlockSummaryObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: BlockSummaryObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(block_summary_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(block_summary_object_type, BlockSummaryObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return BlockSummaryObject.unpack(dec)
     
     def modify(self, perm: BlockSummaryObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(block_summary_object_type, BlockSummaryObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(block_summary_object_type)
 
@@ -1420,36 +1536,42 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(block_summary_object_type, BlockSummaryObject.by_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_block_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(block_summary_object_type, BlockSummaryObject.by_block_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(block_summary_object_type, BlockSummaryObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         return self.db.lower_bound(block_summary_object_type, BlockSummaryObject.by_id, lower_bound)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         return self.db.upper_bound(block_summary_object_type, BlockSummaryObject.by_id, upper_bound)
 
 # transaction_object_type = 16
 class TransactionObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: TransactionObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(transaction_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(transaction_object_type, TransactionObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return TransactionObject.unpack(dec)
 
     def find_by_trx_id(self, trx_id: Checksum256):
@@ -1457,23 +1579,23 @@
         data = self.db.find(transaction_object_type, TransactionObject.by_trx_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return TransactionObject.unpack(dec)
     
     def find_by_expiration(self, expiration: U32, table_id: I64):
-        key = utils.to_bytes(expiration, 4) + utils.to_bytes(table_id, signed=True)
+        key = u2b(expiration, 4) + i2b(table_id)
         data = self.db.find(transaction_object_type, TransactionObject.by_expiration, key)
         if not data:
             return None
         dec = Decoder(data)
         return TransactionObject.unpack(dec)
 
     def modify(self, perm: TransactionObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(transaction_object_type, TransactionObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(transaction_object_type)
 
@@ -1491,30 +1613,30 @@
     def walk_by_trx_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(transaction_object_type, TransactionObject.by_trx_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_expiration(self, cb, user_data=None, raw_data=False):
         return self.db.walk(transaction_object_type, TransactionObject.by_expiration, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(transaction_object_type, TransactionObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_trx_id(self, lower_bound: Checksum256, upper_bound: Checksum256, cb, user_data=None, raw_data=False):
         lower_bound = lower_bound.to_bytes()
         upper_bound = upper_bound.to_bytes()
         return self.db.walk_range(transaction_object_type, TransactionObject.by_trx_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_expiration(self, lower_bound: Union[U32, I64], upper_bound: Union[U32, I64], cb, user_data=None, raw_data=False):
         lower_bound = TransactionObject.generate_key_by_expiration(*lower_bound)
         upper_bound = TransactionObject.generate_key_by_expiration(*upper_bound)
         return self.db.walk_range(transaction_object_type, TransactionObject.by_expiration, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(transaction_object_type, TransactionObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return TransactionObject.unpack(dec)
 
     def lower_bound_by_trx_id(self, lower_bound: Checksum256):
@@ -1530,15 +1652,15 @@
         data = self.db.lower_bound(transaction_object_type, TransactionObject.by_expiration, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return TransactionObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(transaction_object_type, TransactionObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return TransactionObject.unpack(dec)
 
     def upper_bound_by_trx_id(self, upper_bound: Checksum256):
@@ -1558,19 +1680,25 @@
         return TransactionObject.unpack(dec)
 
 # generated_transaction_object_type = 17
 class GeneratedTransactionObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: GeneratedTransactionObject):
+        enc = Encoder()
+        obj.pack(enc)
+        ret = self.db.create(generated_transaction_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(generated_transaction_object_type, GeneratedTransactionObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return GeneratedTransactionObject.unpack(dec)
 
     def find_by_trx_id(self, trx_id: Union[str, Checksum256]):
@@ -1604,15 +1732,15 @@
         data = self.db.find(generated_transaction_object_type, GeneratedTransactionObject.by_sender_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return GeneratedTransactionObject.unpack(dec)
 
     def modify(self, perm: GeneratedTransactionObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(generated_transaction_object_type, GeneratedTransactionObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(generated_transaction_object_type)
 
@@ -1636,16 +1764,16 @@
     def walk_by_delay(self, cb, user_data=None, raw_data=False):
         return self.db.walk(generated_transaction_object_type, GeneratedTransactionObject.by_delay, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_sender_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(generated_transaction_object_type, GeneratedTransactionObject.by_sender_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(generated_transaction_object_type, GeneratedTransactionObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_trx_id(self, lower_bound: Union[bytes, Checksum256], upper_bound: Union[bytes, Checksum256], cb, user_data=None, raw_data=False):
         if isinstance(lower_bound, Checksum256):
             lower_bound = lower_bound.to_bytes()
         if isinstance(upper_bound, Checksum256):
             upper_bound = upper_bound.to_bytes()
@@ -1665,15 +1793,15 @@
 
     def walk_range_by_sender_id(self, lower_bound: Tuple[Name, U128], upper_bound: Tuple[Name, U128], cb, user_data=None, raw_data=False):
         lower_bound = GeneratedTransactionObject.generate_key_by_sender_id(*lower_bound)
         upper_bound = GeneratedTransactionObject.generate_key_by_sender_id(*upper_bound)
         return self.db.walk_range(generated_transaction_object_type, GeneratedTransactionObject.by_sender_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(generated_transaction_object_type, GeneratedTransactionObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return GeneratedTransactionObject.unpack(dec)
 
     def lower_bound_by_trx_id(self, lower_bound: Union[bytes, Checksum256]):
@@ -1709,15 +1837,15 @@
         data = self.db.lower_bound(generated_transaction_object_type, GeneratedTransactionObject.by_sender_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return GeneratedTransactionObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(generated_transaction_object_type, GeneratedTransactionObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return GeneratedTransactionObject.unpack(dec)
 
     def upper_bound_by_trx_id(self, upper_bound: Union[bytes, Checksum256]):
@@ -1757,19 +1885,25 @@
         return GeneratedTransactionObject.unpack(dec)
 
 # table_id_object_type = 30
 class TableIdObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: TableIdObject):
+        enc = Encoder()
+        perm.pack(enc)
+        ret = self.db.create(table_id_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(table_id_object_type, TableIdObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return TableIdObject.unpack(dec)
     
     def find_by_code_scope_table(self, code: Name, scope: Name, table: Name):
@@ -1777,15 +1911,15 @@
         data = self.db.find(table_id_object_type, TableIdObject.by_code_scope_table, key)
         if not data:
             return None
         dec = Decoder(data)
         return TableIdObject.unpack(dec)
 
     def modify(self, perm: TableIdObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(table_id_object_type, TableIdObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(table_id_object_type)
 
@@ -1800,25 +1934,25 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(table_id_object_type, TableIdObject.by_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_code_scope_table(self, cb, user_data=None, raw_data=False):
         return self.db.walk(table_id_object_type, TableIdObject.by_code_scope_table, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(table_id_object_type, TableIdObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_code_scope_table(self, lower_bound: Union[Name, Name, Name], upper_bound: Union[Name, Name, Name], cb, user_data=None, raw_data=False):
         lower_bound = TableIdObject.generate_key_by_code_scope_table(*lower_bound)
         upper_bound = TableIdObject.generate_key_by_code_scope_table(*upper_bound)
         return self.db.walk_range(table_id_object_type, TableIdObject.by_code_scope_table, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(table_id_object_type, TableIdObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return TableIdObject.unpack(dec)
     
     def lower_bound_by_code_scope_table(self, code: Name, scope: Name, table: Name):
@@ -1826,15 +1960,15 @@
         data = self.db.lower_bound(table_id_object_type, TableIdObject.by_code_scope_table, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return TableIdObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(table_id_object_type, TableIdObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return TableIdObject.unpack(dec)
     
     def upper_bound_by_code_scope_table(self, code: Name, scope: Name, table: Name):
@@ -1846,19 +1980,25 @@
         return TableIdObject.unpack(dec)
 
 # resource_limits_object_type = 31
 class ResourceLimitsObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: ResourceLimitsObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(resource_limits_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(resource_limits_object_type, ResourceLimitsObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsObject.unpack(dec)
     
     def find_by_owner(self, pending: bool, owner: Name):
@@ -1866,15 +2006,15 @@
         data = self.db.find(resource_limits_object_type, ResourceLimitsObject.by_owner, key)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsObject.unpack(dec)
 
     def modify(self, perm: ResourceLimitsObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(resource_limits_object_type, ResourceLimitsObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(resource_limits_object_type)
 
@@ -1889,25 +2029,25 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(resource_limits_object_type, ResourceLimitsObject.by_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_owner(self, cb, user_data=None, raw_data=False):
         return self.db.walk(resource_limits_object_type, ResourceLimitsObject.by_owner, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(resource_limits_object_type, ResourceLimitsObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_owner(self, lower_bound: Tuple[bool, Name], upper_bound: Tuple[bool, Name], cb, user_data=None, raw_data=False):
         lower_bound = ResourceLimitsObject.generate_key_by_owner(*lower_bound)
         upper_bound = ResourceLimitsObject.generate_key_by_owner(*upper_bound)
         return self.db.walk_range(resource_limits_object_type, ResourceLimitsObject.by_owner, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(resource_limits_object_type, ResourceLimitsObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsObject.unpack(dec)
 
     def lower_bound_by_owner(self, pending: bool, owner: Name):
@@ -1915,15 +2055,15 @@
         data = self.db.lower_bound(resource_limits_object_type, ResourceLimitsObject.by_owner, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(resource_limits_object_type, ResourceLimitsObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsObject.unpack(dec)
     
     def upper_bound_by_owner(self, pending: bool, owner: Name):
@@ -1935,19 +2075,25 @@
         return ResourceLimitsObject.unpack(dec)
 
 # resource_usage_object_type = 32
 class ResourceUsageObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: ResourceUsageObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(resource_usage_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(resource_usage_object_type, ResourceUsageObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceUsageObject.unpack(dec)
     
     def find_by_owner(self, owner: Name):
@@ -1955,15 +2101,15 @@
         data = self.db.find(resource_usage_object_type, ResourceUsageObject.by_owner, key)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceUsageObject.unpack(dec)
 
     def modify(self, perm: ResourceUsageObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(resource_usage_object_type, ResourceUsageObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(resource_usage_object_type)
 
@@ -1978,25 +2124,25 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(resource_usage_object_type, ResourceUsageObject.by_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_owner(self, cb, user_data=None, raw_data=False):
         return self.db.walk(resource_usage_object_type, ResourceUsageObject.by_owner, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, lower_bound: I64, upper_bound: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
+        upper_bound = i2b(upper_bound)
         return self.db.walk_range(resource_usage_object_type, ResourceUsageObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_owner(self, lower_bound: Name, upper_bound: Name, cb, user_data=None, raw_data=False):
         lower_bound = eos.s2b(lower_bound)
         upper_bound = eos.s2b(upper_bound)
         return self.db.walk_range(resource_usage_object_type, ResourceUsageObject.by_owner, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, lower_bound: I64):
-        lower_bound = int.to_bytes(lower_bound, 8, 'little', signed=True)
+        lower_bound = i2b(lower_bound)
         data = self.db.lower_bound(resource_usage_object_type, ResourceUsageObject.by_id, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceUsageObject.unpack(dec)
 
     def lower_bound_by_owner(self, lower_bound: Name):
@@ -2004,15 +2150,15 @@
         data = self.db.lower_bound(resource_usage_object_type, ResourceUsageObject.by_owner, lower_bound)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceUsageObject.unpack(dec)
 
     def upper_bound_by_id(self, upper_bound: I64):
-        upper_bound = int.to_bytes(upper_bound, 8, 'little', signed=True)
+        upper_bound = i2b(upper_bound)
         data = self.db.upper_bound(resource_usage_object_type, ResourceUsageObject.by_id, upper_bound)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceUsageObject.unpack(dec)
     
     def upper_bound_by_owner(self, upper_bound: Name):
@@ -2024,119 +2170,167 @@
         return ResourceUsageObject.unpack(dec)
 
 # resource_limits_state_object_type = 33
 class ResourceLimitsStateObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: ResourceLimitsStateObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(resource_limits_state_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
+    def get(self):
+        return self.find_by_id(0)
+
+    def set(self, perm: ResourceLimitsStateObject):
+        return self.modify(perm)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(resource_limits_state_object_type, ResourceLimitsStateObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsStateObject.unpack(dec)
 
     def modify(self, perm: ResourceLimitsStateObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(resource_limits_state_object_type, ResourceLimitsStateObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(resource_limits_state_object_type)
 
 # resource_limits_config_object_type = 34
 class ResourceLimitsConfigObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: ResourceLimitsConfigObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(resource_limits_config_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
+    def get(self):
+        return self.find_by_id(0)
+
+    def set(self, perm: ResourceLimitsConfigObject):
+        return self.modify(perm)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(resource_limits_config_object_type, ResourceLimitsConfigObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return ResourceLimitsConfigObject.unpack(dec)
 
     def modify(self, perm: ResourceLimitsConfigObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(resource_limits_config_object_type, ResourceLimitsConfigObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(resource_limits_config_object_type)
 
 # protocol_state_object_type = 38
 class ProtocolStateObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: ProtocolStateObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(protocol_state_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
+    def get(self):
+        return self.find_by_id(0)
+
+    def set(self, perm: ProtocolStateObject):
+        return self.modify(perm)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(protocol_state_object_type, ProtocolStateObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return ProtocolStateObject.unpack(dec)
 
     def modify(self, perm: ProtocolStateObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(protocol_state_object_type, ProtocolStateObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(protocol_state_object_type)
 
 # account_ram_correction_object_type = 39
 class AccountRamCorrectionObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: AccountRamCorrectionObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(account_ram_correction_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(account_ram_correction_object_type, AccountRamCorrectionObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return AccountRamCorrectionObject.unpack(dec)
 
     def modify(self, perm: AccountRamCorrectionObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(account_ram_correction_object_type, AccountRamCorrectionObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(account_ram_correction_object_type)
 
 # code_object_type = 40
 class CodeObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, obj: CodeObject):
+        enc = Encoder()
+        enc.pack(obj)
+        ret = self.db.create(code_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
     def find(self, table_id: I64):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(code_object_type, CodeObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return CodeObject.unpack(dec)
 
     def convert_code_hash(self, code_hash: Union[str, bytes, Checksum256]):
@@ -2146,15 +2340,15 @@
             code_hash = code_hash.to_bytes()
         assert isinstance(code_hash, bytes)
         assert len(code_hash) == 32, 'code_hash must be 32 bytes'
         return code_hash
 
     def find_by_code_hash(self, code_hash: Union[str, bytes, Checksum256], vm_type: U8, vm_version: U8):
         code_hash = self.convert_code_hash(code_hash)
-        key = code_hash + int.to_bytes(vm_type, 1, 'little') + int.to_bytes(vm_version, 1, 'little')
+        key = code_hash + u2b(vm_type, 1) + u2b(vm_version, 1)
         data = self.db.find(code_object_type, CodeObject.by_code_hash, key)
         if not data:
             return None
         dec = Decoder(data)
         return CodeObject.unpack(dec)
 
     def on_object_data(self, tp, data, custom_data):
@@ -2168,29 +2362,29 @@
     def walk_by_id(self, cb, user_data=None, raw_data=False):
         return self.db.walk(database.code_object_type, CodeObject.by_id, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_by_code_hash(self, cb, user_data=None, raw_data=False):
         return self.db.walk(database.code_object_type, CodeObject.by_code_hash, self.on_object_data, (cb, raw_data, user_data))
 
     def walk_range_by_id(self, start_id: I64, end_id: I64, cb, user_data=None, raw_data=False):
-        lower_bound = int.to_bytes(start_id, 8, 'little', signed=True)
-        upper_bound = int.to_bytes(end_id, 8, 'little', signed=True)
+        lower_bound = i2b(start_id)
+        upper_bound = i2b(end_id)
         return self.db.walk_range(database.code_object_type, CodeObject.by_id, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def convert_by_code_hash_key(self, key: Tuple[Union[str, bytes, Checksum256], U8, U8]):
         code_hash, vm_type, vm_version = key
-        return self.convert_code_hash(code_hash) + int.to_bytes(vm_type, 1, 'little') + int.to_bytes(vm_version, 1, 'little')
+        return self.convert_code_hash(code_hash) + u2b(vm_type) + u2b(vm_version, 1)
 
     def walk_range_by_code_hash(self, lower_bound: Tuple[Union[str, bytes, Checksum256], U8, U8], upper_bound: Tuple[Union[str, bytes, Checksum256], U8, U8], cb, user_data=None, raw_data=False):
         lower_bound = self.convert_by_code_hash_key(lower_bound)
         upper_bound = self.convert_by_code_hash_key(upper_bound)
         return self.db.walk_range(database.code_object_type, CodeObject.by_code_hash, lower_bound, upper_bound, self.on_object_data, (cb, raw_data, user_data))
 
     def lower_bound_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.lower_bound(code_object_type, CodeObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return CodeObject.unpack(dec)
 
     def lower_bound_by_code_hash(self, lower_bound: Tuple[Union[str, bytes, Checksum256], U8, U8]):
@@ -2198,15 +2392,15 @@
         data = self.db.lower_bound(code_object_type, CodeObject.by_code_hash, key)
         if not data:
             return None
         dec = Decoder(data)
         return CodeObject.unpack(dec)
 
     def upper_bound_by_id(self, table_id: I64):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.upper_bound(code_object_type, CodeObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return CodeObject.unpack(dec)
 
     def upper_bound_by_code_hash(self, upper_bound: Tuple[Union[str, bytes, Checksum256], U8, U8]):
@@ -2214,39 +2408,51 @@
         data = self.db.upper_bound(code_object_type, CodeObject.by_code_hash, key)
         if not data:
             return None
         dec = Decoder(data)
         return CodeObject.unpack(dec)
 
     def modify(self, perm: CodeObject):
-        key = int.to_bytes(perm.table_id, 8, 'little', signed=True)
+        key = i2b(perm.table_id)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(code_object_type, CodeObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(code_object_type)
 
 # database_header_object_type = 41
 class DatabaseHeaderObjectIndex(object):
     def __init__(self, db: Database):
         self.db = db
 
+    def create(self, perm: DatabaseHeaderObject):
+        enc = Encoder()
+        enc.pack(perm)
+        ret = self.db.create(database_header_object_type, enc.get_bytes())
+        return parse_return_value(ret)
+
+    def get(self):
+        return self.find_by_id(0)
+
+    def set(self, perm: DatabaseHeaderObject):
+        return self.modify(perm)
+
     def find(self, table_id=0):
         return self.find_by_id(table_id)
 
     def find_by_id(self, table_id=0):
-        key = int.to_bytes(table_id, 8, 'little', signed=True)
+        key = i2b(table_id)
         data = self.db.find(database_header_object_type, DatabaseHeaderObject.by_id, key)
         if not data:
             return None
         dec = Decoder(data)
         return DatabaseHeaderObject.unpack(dec)
 
     def modify(self, perm: DatabaseHeaderObject):
-        key = int.to_bytes(0, 8, 'little', signed=True)
+        key = u2b(0)
         enc = Encoder()
         enc.pack(perm)
         return self.db.modify(database_header_object_type, DatabaseHeaderObject.by_id, key, enc.get_bytes())
 
     def row_count(self):
         return self.db.row_count(database_header_object_type)
```

### Comparing `ipyeos-0.4.4/pysrc/database_objects.py` & `ipyeos-0.4.5/pysrc/database_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import base58
 import hashlib
 from typing import NewType, List, TypeVar, Generic, Optional, Union
 
 from . import database
 from . import eos
 from .types import U8, U16, U32, U64, I64, U128, U256, Name, TimePointSec, F128, PublicKey, Checksum256
 from .packer import Encoder, Decoder
 from .structs import PermissionLevel, KeyWeight, PermissionLevelWeight, WaitWeight, Authority, TimePoint
 from .structs import Variant
-from . import utils
+from .utils import to_bytes, i2b, u2b, f2b
 # struct account_object_ {
 #     account_name         name; //< name should not be changed within a chainbase modifier lambda
 #     block_timestamp_type creation_date;
 #     vector<char>          abi;
 # };
 
 class template(object):
@@ -32,19 +31,23 @@
     def unpack(cls, dec: Decoder):
         pass
 
 class AccountObject(object):
     by_id = 0
     by_name = 1
     def __init__(self, table_id: I64, name: Name, creation_date: U32, abi: bytes):
-        self.table_id = table_id
+        self._table_id = table_id
         self.name = name
         self.creation_date = creation_date
         self.abi = abi
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{name: {self.name}, creation_date: {self.creation_date}, abi: {self.abi}}}"
 
     def __eq__(self, other):
         return self.name == other.name \
             and self.creation_date == other.creation_date \
             and self.abi == other.abi
@@ -79,26 +82,30 @@
 # };
 
 class AccountMetadataObject(object):
     by_id = 0
     by_name = 1
     def __init__(self, table_id: I64, name: Name, recv_sequence: U64, auth_sequence: U64, code_sequence: U64, abi_sequence: U64, \
                 code_hash: Checksum256, last_code_update: I64, flags: U32, vm_type: U8, vm_version: U8):
-        self.table_id = table_id
+        self._table_id = table_id
         self.name = name
         self.recv_sequence = recv_sequence
         self.auth_sequence = auth_sequence
         self.code_sequence = code_sequence
         self.abi_sequence = abi_sequence
         self.code_hash = code_hash
         self.last_code_update = last_code_update
         self.flags = flags
         self.vm_type = vm_type
         self.vm_version = vm_version
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{name: {self.name}, recv_sequence: {self.recv_sequence}, \
         auth_sequence: {self.auth_sequence}, \
         code_sequence: {self.code_sequence}, \
         abi_sequence: {self.abi_sequence}, \
         code_hash: {self.code_hash}, \
         last_code_update: {self.last_code_update}, \
@@ -182,48 +189,52 @@
     """
     by_id = 0
     by_parent = 1
     by_owner = 2
     by_name = 3
 
     def __init__(self, table_id: I64, usage_id: I64, parent: I64, owner: Name, name: Name, last_updated: I64, auth: Authority):
-        self.table_id = table_id
+        self._table_id = table_id
         self.usage_id = usage_id
         self.parent = parent
         self.owner = owner
         self.name = name
         self.last_updated = last_updated
         self.auth = auth
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{table_id: {self.table_id}, usage_id: {self.usage_id}, parent: {self.parent}, owner: {self.owner}, name: {self.name}, last_updated: {self.last_updated}, auth: {self.auth}}}"
 
     def __eq__(self, other) -> bool:
         return self.usage_id == other.usage_id \
             and self.parent == other.parent \
             and self.owner == other.owner \
             and self.name == other.name \
             and self.last_updated == other.last_updated \
             and self.auth == other.auth
 
     @classmethod
     def generate_key_by_id(cls, table_id: I64):
-        return int.to_bytes(table_id, 8, 'little', signed=True)
+        return i2b(table_id)
 
     @classmethod
     def generate_key_by_parent(cls, parent: I64, table_id: I64):
-        return int.to_bytes(parent, 8, 'little', signed=True) + int.to_bytes(table_id, 8, 'little', signed=True)
+        return i2b(parent) + i2b(table_id)
 
     @classmethod
     def generate_key_by_owner(cls, owner: Name, name: Name):
         return eos.s2b(owner) + eos.s2b(name)
 
     @classmethod
     def generate_key_by_name(cls, name: Name, table_id: I64):
-        return eos.s2b(name) + int.to_bytes(table_id, 8, 'little', signed=True)
+        return eos.s2b(name) + i2b(table_id)
 
     def pack(self, enc: Encoder) -> int:
         pos = enc.get_pos()
         enc.pack_i64(self.usage_id)
         enc.pack_i64(self.parent)
         enc.pack_name(self.owner)
         enc.pack_name(self.name)
@@ -250,17 +261,21 @@
 # struct permission_usage_object_ {
 #     time_point        last_used;   ///< when this permission was last used
 # };
 
 class PermissionUsageObject(object):
     by_id = 0
     def __init__(self, table_id: I64, last_used: I64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.last_used = last_used
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{last_used: {self.last_used}}}"
 
     def __eq__(self, other):
         return self.last_used == other.last_used
 
     def pack(self, enc: Encoder) -> int:
@@ -286,20 +301,24 @@
 # };
 
 class PermissionLinkObject(object):
     by_id = 0
     by_action_name = 1
     by_permission_name = 2
     def __init__(self, table_id: I64, account: Name, code: Name, message_type: Name, required_permission: Name):
-        self.table_id = table_id
+        self._table_id = table_id
         self.account = account
         self.code = code
         self.message_type = message_type
         self.required_permission = required_permission
     
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{account: {self.account}, code: {self.code}, message_type: {self.message_type}, required_permission: {self.required_permission}}}"
     
     def __eq__(self, other):
         return self.account == other.account \
             and self.code == other.code \
             and self.message_type == other.message_type \
@@ -324,34 +343,38 @@
 
     @classmethod
     def generate_key_by_action_name(cls, account: Name, code: Name, message_type: Name):
         return eos.s2b(account) + eos.s2b(code) + eos.s2b(message_type)
     
     @classmethod
     def generate_key_by_permission_name(cls, account: Name, required_permission: Name, table_id: I64):
-        return eos.s2b(account) + eos.s2b(required_permission) + int.to_bytes(table_id, 8, 'little', signed=True)
+        return eos.s2b(account) + eos.s2b(required_permission) + i2b(table_id)
 
 
 # struct key_value_object_ {
 #     int64_t              t_id; //< t_id should not be changed within a chainbase modifier lambda
 #     uint64_t             primary_key; //< primary_key should not be changed within a chainbase modifier lambda
 #     account_name         payer;
 #     vector<char>         value;
 # };
 
 class KeyValueObject(object):
     by_id = 0
     by_scope_primary = 1
     def __init__(self, table_id: I64, t_id: I64, primary_key: U64, payer: Name, value: bytes):
-        self.table_id = table_id
+        self._table_id = table_id
         self.t_id = t_id
         self.primary_key = primary_key
         self.payer = payer
         self.value = value
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{t_id: {self.t_id}, primary_key: {self.primary_key}, payer: {self.payer}, value: {self.value}}}"
 
     def __eq__(self, other):
         return self.t_id == other.t_id \
             and self.primary_key == other.primary_key \
             and self.payer == other.payer \
@@ -372,35 +395,39 @@
         primary_key = dec.unpack_u64()
         payer = dec.unpack_name()
         value = dec.unpack_bytes()
         return KeyValueObject(table_id, t_id, primary_key, payer, value)
     
     @classmethod
     def generate_key_by_scope_primary(cls, t_id: I64, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(primary_key)
 
 # struct index64_object_ {
 #     int64_t       t_id; //< t_id should not be changed within a chainbase modifier lambda
 #     uint64_t      primary_key; //< primary_key should not be changed within a chainbase modifier lambda
 #     account_name  payer;
 #     uint64_t  secondary_key; //< secondary_key should not be changed within a chainbase modifier lambda
 # };
 
 class Index64Object(object):
     by_id = 0
     by_primary = 1
     by_secondary = 2
 
     def __init__(self, table_id: I64, t_id: I64, primary_key: U64, payer: Name, secondary_key: U64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.t_id = t_id
         self.primary_key = primary_key
         self.payer = payer
         self.secondary_key = secondary_key
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{t_id: {self.t_id}, primary_key: {self.primary_key}, payer: {self.payer}, secondary_key: {self.secondary_key}}}"
 
     def __eq__(self, other):
         return self.t_id == other.t_id \
             and self.primary_key == other.primary_key \
             and self.payer == other.payer \
@@ -421,38 +448,42 @@
         primary_key = dec.unpack_u64()
         payer = dec.unpack_name()
         secondary_key = dec.unpack_u64()
         return Index64Object(table_id, t_id, primary_key, payer, secondary_key)
 
     @classmethod
     def generate_key_by_primary(cls, t_id: I64, primary_key: U64):
-        return utils.to_bytes(t_id, 8, signed=True) + utils.to_bytes(primary_key, 8)
+        return i2b(t_id) + u2b(primary_key)
     
     @classmethod
     def generate_key_by_secondary(cls, t_id: I64, secondary_key: U64, primary_key: U64):
-        return utils.to_bytes(t_id, 8, signed=True) + utils.to_bytes(secondary_key, 8) + utils.to_bytes(primary_key, 8)
+        return i2b(t_id) + u2b(secondary_key) + u2b(primary_key)
 
 # struct index128_object_ {
 #     int64_t       t_id; //< t_id should not be changed within a chainbase modifier lambda
 #     uint64_t      primary_key; //< primary_key should not be changed within a chainbase modifier lambda
 #     account_name  payer;
 #     uint128_t  secondary_key; //< secondary_key should not be changed within a chainbase modifier lambda
 # };
 
 class Index128Object(object):
     by_id = 0
     by_primary = 1
     by_secondary = 2
     def __init__(self, table_id: I64, t_id: I64, primary_key: U64, payer: Name, secondary_key: U128):
-        self.table_id = table_id
+        self._table_id = table_id
         self.t_id = t_id
         self.primary_key = primary_key
         self.payer = payer
         self.secondary_key = secondary_key
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{t_id: {self.t_id}, primary_key: {self.primary_key}, payer: {self.payer}, secondary_key: {self.secondary_key}}}"
 
     def __eq__(self, other):
         return self.t_id == other.t_id \
             and self.primary_key == other.primary_key \
             and self.payer == other.payer \
@@ -473,39 +504,43 @@
         primary_key = dec.unpack_u64()
         payer = dec.unpack_name()
         secondary_key = dec.unpack_u128()
         return Index128Object(table_id, t_id, primary_key, payer, secondary_key)
 
     @classmethod
     def generate_key_by_primary(cls, t_id: I64, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(primary_key)
     
     @classmethod
     def generate_key_by_secondary(cls, t_id: I64, secondary_key: U128, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(secondary_key, 16, 'little') + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(secondary_key, 16) + u2b(primary_key)
 
 
 # struct index256_object_ {
 #     int64_t       t_id; //< t_id should not be changed within a chainbase modifier lambda
 #     uint64_t      primary_key; //< primary_key should not be changed within a chainbase modifier lambda
 #     account_name  payer;
 #     key256_t  secondary_key; //< secondary_key should not be changed within a chainbase modifier lambda
 # };
 
 class Index256Object(object):
     by_id = 0
     by_primary = 1
     by_secondary = 2
     def __init__(self, table_id: I64, t_id: I64, primary_key: U64, payer: Name, secondary_key: U256):
-        self.table_id = table_id
+        self._table_id = table_id
         self.t_id = t_id
         self.primary_key = primary_key
         self.payer = payer
         self.secondary_key = secondary_key
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{t_id: {self.t_id}, primary_key: {self.primary_key}, payer: {self.payer}, secondary_key: {self.secondary_key}}}"
 
     def __eq__(self, other):
         return self.t_id == other.t_id \
             and self.primary_key == other.primary_key \
             and self.payer == other.payer \
@@ -526,39 +561,43 @@
         primary_key = dec.unpack_u64()
         payer = dec.unpack_name()
         secondary_key = dec.unpack_u256()
         return Index256Object(table_id, t_id, primary_key, payer, secondary_key)
 
     @classmethod
     def generate_key_by_primary(cls, t_id: I64, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(primary_key)
     
     @classmethod
     def generate_key_by_secondary(cls, t_id: I64, secondary_key: U256, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(secondary_key, 32, 'little') + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(secondary_key, 32) + u2b(primary_key)
 
 
 # struct index_double_object_ {
 #     int64_t       t_id; //< t_id should not be changed within a chainbase modifier lambda
 #     uint64_t      primary_key; //< primary_key should not be changed within a chainbase modifier lambda
 #     account_name  payer;
 #     double  secondary_key; //< secondary_key should not be changed within a chainbase modifier lambda
 # };
 
 class IndexDoubleObject(object):
     by_id = 0
     by_primary = 1
     by_secondary = 2
     def __init__(self, table_id: I64, t_id: I64, primary_key: U64, payer: Name, secondary_key: float):
-        self.table_id = table_id
+        self._table_id = table_id
         self.t_id = t_id
         self.primary_key = primary_key
         self.payer = payer
         self.secondary_key = secondary_key
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{t_id: {self.t_id}, primary_key: {self.primary_key}, payer: {self.payer}, secondary_key: {self.secondary_key}}}"
 
     def __eq__(self, other):
         return self.t_id == other.t_id \
             and self.primary_key == other.primary_key \
             and self.payer == other.payer \
@@ -579,39 +618,43 @@
         primary_key = dec.unpack_u64()
         payer = dec.unpack_name()
         secondary_key = dec.unpack_double()
         return IndexDoubleObject(table_id, t_id, primary_key, payer, secondary_key)
 
     @classmethod
     def generate_key_by_primary(cls, t_id: I64, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(primary_key)
     
     @classmethod
     def generate_key_by_secondary(cls, t_id: I64, secondary_key: float, primary_key: U64):
-        return utils.to_bytes(t_id, signed=True) + utils.to_bytes(secondary_key) + utils.to_bytes(primary_key, 8)
+        return i2b(t_id) + f2b(secondary_key) + u2b(primary_key)
 
 
 # struct index_long_double_object_ {
 #     int64_t       t_id; //< t_id should not be changed within a chainbase modifier lambda
 #     uint64_t      primary_key; //< primary_key should not be changed within a chainbase modifier lambda
 #     account_name  payer;
 #     long double  secondary_key; //< secondary_key should not be changed within a chainbase modifier lambda
 # };
 
 class IndexLongDoubleObject(object):
     by_id = 0
     by_primary = 1
     by_secondary = 2
     def __init__(self, table_id: I64, t_id: I64, primary_key: U64, payer: Name, secondary_key: F128):
-        self.table_id = table_id
+        self._table_id = table_id
         self.t_id = t_id
         self.primary_key = primary_key
         self.payer = payer
         self.secondary_key = secondary_key
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{t_id: {self.t_id}, primary_key: {self.primary_key}, payer: {self.payer}, secondary_key: {self.secondary_key}}}"
 
     def __eq__(self, other):
         return self.t_id == other.t_id \
             and self.primary_key == other.primary_key \
             and self.payer == other.payer \
@@ -632,15 +675,15 @@
         primary_key = dec.unpack_u64()
         payer = dec.unpack_name()
         secondary_key = F128.unpack(dec)
         return IndexLongDoubleObject(table_id, t_id, primary_key, payer, secondary_key)
 
     @classmethod
     def generate_key_by_primary(cls, t_id: I64, primary_key: U64):
-        return int.to_bytes(t_id, 8, 'little', signed=True) + int.to_bytes(primary_key, 8, 'little')
+        return i2b(t_id) + u2b(primary_key)
     
     @classmethod
     def generate_key_by_secondary(cls, t_id: I64, secondary_key: F128, primary_key: U64):
         enc = Encoder()
         enc.pack_i64(t_id)
         enc.pack(secondary_key)
         enc.pack_u64(primary_key)
@@ -1057,17 +1100,21 @@
 # struct dynamic_global_property_object_ {
 #     uint64_t   global_action_sequence = 0;
 # };
 
 class DynamicGlobalPropertyObject(object):
     by_id = 0
     def __init__(self, table_id: I64, global_action_sequence: U64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.global_action_sequence = global_action_sequence
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{global_action_sequence: {self.global_action_sequence}}}"
 
     def __eq__(self, other):
         return self.global_action_sequence == other.global_action_sequence
 
     def pack(self, enc: Encoder) -> int:
@@ -1085,17 +1132,21 @@
 # struct block_summary_object_ {
 #     block_id_type  block_id;
 # };
 
 class BlockSummaryObject(object):
     by_id = 0
     def __init__(self, table_id: I64, block_id: Checksum256):
-        self.table_id = table_id
+        self._table_id = table_id
         self.block_id = block_id
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{block_id: {self.block_id}}}"
 
     def __eq__(self, other):
         return self.block_id == other.block_id
 
     def pack(self, enc: Encoder) -> int:
@@ -1115,18 +1166,22 @@
 # };
 
 class TransactionObject(object):
     by_id = 0
     by_trx_id = 1
     by_expiration = 2
     def __init__(self, table_id: I64, expiration: TimePointSec, trx_id: Checksum256):
-        self.table_id = table_id
+        self._table_id = table_id
         self.expiration = expiration
         self.trx_id = trx_id
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{expiration: {self.expiration}, trx_id: {self.trx_id}}}"
 
     def __eq__(self, other):
         return self.expiration == other.expiration \
             and self.trx_id == other.trx_id
 
@@ -1141,15 +1196,15 @@
         table_id = dec.unpack_i64()
         expiration = dec.unpack_u32()
         trx_id = dec.unpack(Checksum256)
         return TransactionObject(table_id, expiration, trx_id)
     
     @classmethod
     def generate_key_by_expiration(cls, expiration: U32, table_id: I64):
-        return utils.to_bytes(expiration, 4) + utils.to_bytes(table_id, signed=True)
+        return u2b(expiration, 4) + i2b(table_id)
 
 # struct generated_transaction_object_ {
 #     transaction_id_type           trx_id;
 #     account_name                  sender;
 #     uint128_t                     sender_id;
 #     account_name                  payer;
 #     time_point                    delay_until; /// this generated transaction will not be applied until the specified time
@@ -1162,24 +1217,28 @@
     by_id = 0
     by_trx_id = 1
     by_expiration = 2
     by_delay = 3
     by_sender_id = 4
 
     def __init__(self, table_id: I64, trx_id: Checksum256, sender: Name, sender_id: U128, payer: Name, delay_until: TimePoint, expiration: TimePoint, published: TimePoint, packed_trx: bytes):
-        self.table_id = table_id
+        self._table_id = table_id
         self.trx_id = trx_id
         self.sender = sender
         self.sender_id = sender_id
         self.payer = payer
         self.delay_until = delay_until
         self.expiration = expiration
         self.published = published
         self.packed_trx = packed_trx
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{trx_id: {self.trx_id}, sender: {self.sender}, sender_id: {self.sender_id}, payer: {self.payer}, delay_until: {self.delay_until}, expiration: {self.expiration}, published: {self.published}, packed_trx: {self.packed_trx}}}"
 
     def __eq__(self, other):
         return self.trx_id == other.trx_id \
             and self.sender == other.sender \
             and self.sender_id == other.sender_id \
@@ -1223,46 +1282,50 @@
                 packed_trx)
 
     @classmethod
     def generate_key_by_expiration(self, expiration: Union[I64, TimePoint], table_id: I64):
         if isinstance(expiration, TimePoint):
             expiration = expiration.time
         assert isinstance(expiration, int)
-        return int.to_bytes(expiration, 8, 'little', signed=True) + int.to_bytes(table_id, 8, 'little', signed=True)
+        return i2b(expiration) + i2b(table_id)
 
     @classmethod
     def generate_key_by_delay(self, delay_until: Union[I64, TimePoint], table_id: I64):
         if isinstance(delay_until, TimePoint):
             delay_until = delay_until.time
         assert isinstance(delay_until, int)
-        return int.to_bytes(delay_until, 8, 'little', signed=True) + int.to_bytes(table_id, 8, 'little', signed=True)
+        return i2b(delay_until) + i2b(table_id)
 
     @classmethod
     def generate_key_by_sender_id(self, sender: Name, sender_id: U128):
-        return  eos.s2b(sender) + int.to_bytes(sender_id, 16, 'little')
+        return  eos.s2b(sender) + u2b(sender_id, 16)
 
 # struct table_id_object_ {
 #     account_name   code;  //< code should not be changed within a chainbase modifier lambda
 #     scope_name     scope; //< scope should not be changed within a chainbase modifier lambda
 #     table_name     table; //< table should not be changed within a chainbase modifier lambda
 #     account_name   payer;
 #     uint32_t       count = 0; /// the number of elements in the table
 # };
 
 class TableIdObject(object):
     by_id = 0
     by_code_scope_table = 1
     def __init__(self, table_id: I64, code: Name, scope: Name, table: Name, payer: Name, count: U32):
-        self.table_id = table_id
+        self._table_id = table_id
         self.code = code
         self.scope = scope
         self.table = table
         self.payer = payer
         self.count = count
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{code: {self.code}, scope: {self.scope}, table: {self.table}, payer: {self.payer}, count: {self.count}}}"
 
     def __eq__(self, other):
         return self.code == other.code \
             and self.scope == other.scope \
             and self.table == other.table \
@@ -1301,21 +1364,25 @@
 #     int64_t ram_bytes = -1;
 # };
 
 class ResourceLimitsObject(object):
     by_id = 0
     by_owner = 1
     def __init__(self, table_id: I64, owner: Name, pending: bool, net_weight: I64, cpu_weight: I64, ram_bytes: I64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.owner = owner
         self.pending = pending
         self.net_weight = net_weight
         self.cpu_weight = cpu_weight
         self.ram_bytes = ram_bytes
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{owner: {self.owner}, pending: {self.pending}, net_weight: {self.net_weight}, cpu_weight: {self.cpu_weight}, ram_bytes: {self.ram_bytes}}}"
 
     def __eq__(self, other):
         return self.owner == other.owner \
             and self.net_weight == other.net_weight \
             and self.cpu_weight == other.cpu_weight \
@@ -1388,20 +1455,24 @@
 #     uint64_t                 ram_usage = 0;
 # };
 
 class ResourceUsageObject(object):
     by_id = 0
     by_owner = 1
     def __init__(self, table_id: I64, owner: Name, net_usage: UsageAccumulator, cpu_usage: UsageAccumulator, ram_usage: U64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.owner = owner
         self.net_usage = net_usage
         self.cpu_usage = cpu_usage
         self.ram_usage = ram_usage
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{owner: {self.owner}, net_usage: {self.net_usage}, cpu_usage: {self.cpu_usage}, ram_usage: {self.ram_usage}}}"
 
     def __eq__(self, other):
         return self.owner == other.owner \
             and self.net_usage == other.net_usage \
             and self.cpu_usage == other.cpu_usage \
@@ -1451,25 +1522,29 @@
                 pending_net_usage: U64,
                 pending_cpu_usage: U64,
                 total_net_weight: U64,
                 total_cpu_weight: U64,
                 total_ram_bytes: U64,
                 virtual_net_limit: U64,
                 virtual_cpu_limit: U64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.average_block_net_usage = average_block_net_usage
         self.average_block_cpu_usage = average_block_cpu_usage
         self.pending_net_usage = pending_net_usage
         self.pending_cpu_usage = pending_cpu_usage
         self.total_net_weight = total_net_weight
         self.total_cpu_weight = total_cpu_weight
         self.total_ram_bytes = total_ram_bytes
         self.virtual_net_limit = virtual_net_limit
         self.virtual_cpu_limit = virtual_cpu_limit
 
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{average_block_net_usage: {self.average_block_net_usage}, average_block_cpu_usage: {self.average_block_cpu_usage}, pending_net_usage: {self.pending_net_usage}, pending_cpu_usage: {self.pending_cpu_usage}, total_net_weight: {self.total_net_weight}, total_cpu_weight: {self.total_cpu_weight}, total_ram_bytes: {self.total_ram_bytes}, virtual_net_limit: {self.virtual_net_limit}, virtual_cpu_limit: {self.virtual_cpu_limit}}}"
     
     def __eq__(self, other):
         return self.average_block_net_usage == other.average_block_net_usage \
             and self.average_block_cpu_usage == other.average_block_cpu_usage \
             and self.pending_net_usage == other.pending_net_usage \
@@ -1593,20 +1668,24 @@
 #     uint32_t account_cpu_usage_average_window = config::account_cpu_usage_average_window_ms / config::block_interval_ms;
 #     uint32_t account_net_usage_average_window = config::account_net_usage_average_window_ms / config::block_interval_ms;
 # };
 
 class ResourceLimitsConfigObject(object):
     by_id = 0
     def __init__(self, table_id: I64, cpu_limit_parameters: ElasticLimitParameters, net_limit_parameters: ElasticLimitParameters, account_cpu_usage_average_window: U32, account_net_usage_average_window: U32):
-        self.table_id = table_id
+        self._table_id = table_id
         self.cpu_limit_parameters = cpu_limit_parameters
         self.net_limit_parameters = net_limit_parameters
         self.account_cpu_usage_average_window = account_cpu_usage_average_window
         self.account_net_usage_average_window = account_net_usage_average_window
     
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{cpu_limit_parameters: {self.cpu_limit_parameters}, net_limit_parameters: {self.net_limit_parameters}, account_cpu_usage_average_window: {self.account_cpu_usage_average_window}, account_net_usage_average_window: {self.account_net_usage_average_window}}}"
     
     def __eq__(self, other):
         return self.cpu_limit_parameters == other.cpu_limit_parameters \
             and self.net_limit_parameters == other.net_limit_parameters \
             and self.account_cpu_usage_average_window == other.account_cpu_usage_average_window \
@@ -1663,20 +1742,24 @@
 #     vector<string>                             whitelisted_intrinsics;
 #     uint32_t                                   num_supported_key_types = 0;
 # };
 
 class ProtocolStateObject(object):
     by_id = 0
     def __init__(self, table_id: I64, activated_protocol_features: List[ActivatedProtocolFeature], preactivated_protocol_features: List[Checksum256], whitelisted_intrinsics: List[str], num_supported_key_types: U32):
-        self.table_id = table_id
+        self._table_id = table_id
         self.activated_protocol_features = activated_protocol_features
         self.preactivated_protocol_features = preactivated_protocol_features
         self.whitelisted_intrinsics = whitelisted_intrinsics
         self.num_supported_key_types = num_supported_key_types
     
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{activated_protocol_features: {self.activated_protocol_features}, preactivated_protocol_features: {self.preactivated_protocol_features}, whitelisted_intrinsics: {self.whitelisted_intrinsics}, num_supported_key_types: {self.num_supported_key_types}}}"
     
     def __eq__(self, other):
         return self.activated_protocol_features == other.activated_protocol_features \
             and self.preactivated_protocol_features == other.preactivated_protocol_features \
             and self.whitelisted_intrinsics == other.whitelisted_intrinsics \
@@ -1708,18 +1791,22 @@
 #     account_name name; //< name should not be changed within a chainbase modifier lambda
 #     uint64_t     ram_correction = 0;
 # };
 
 class AccountRamCorrectionObject(object):
     by_id = 0
     def __init__(self, table_id: I64, name: Name, ram_correction: U64):
-        self.table_id = table_id
+        self._table_id = table_id
         self.name = name
         self.ram_correction = ram_correction
-    
+
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{name: {self.name}, ram_correction: {self.ram_correction}}}"
     
     def __eq__(self, other):
         return self.name == other.name and self.ram_correction == other.ram_correction
     
     def pack(self, enc: Encoder) -> int:
@@ -1727,15 +1814,15 @@
         enc.pack_name(self.name)
         enc.pack_u64(self.ram_correction)
         return enc.get_pos() - pos
     
     @classmethod
     def unpack(cls, dec: Decoder):
         table_id = dec.unpack_i64()
-        name = dec.unpack_name(dec)
+        name = dec.unpack_name()
         ram_correction = dec.unpack_u64()
         return AccountRamCorrectionObject(table_id, name, ram_correction)
 
 
 # struct code_object_ {
 #     digest_type  code_hash; //< code_hash should not be changed within a chainbase modifier lambda
 #     vector<char>  code;
@@ -1745,22 +1832,26 @@
 #     uint8_t      vm_version = 0; //< vm_version should not be changed within a chainbase modifier lambda
 # };
 
 class CodeObject(object):
     by_id = 0
     by_code_hash = 1
     def __init__(self, table_id: I64, code_hash: Checksum256, code: List[str], code_ref_count: U64, first_block_used: U32, vm_type: U8, vm_version: U8):
-        self.table_id = table_id
+        self._table_id = table_id
         self.code_hash = code_hash
         self.code = code
         self.code_ref_count = code_ref_count
         self.first_block_used = first_block_used
         self.vm_type = vm_type
         self.vm_version = vm_version
-    
+
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{code_hash: {self.code_hash}, code: {self.code}, code_ref_count: {self.code_ref_count}, first_block_used: {self.first_block_used}, vm_type: {self.vm_type}, vm_version: {self.vm_version}}}"
     
     def __eq__(self, other):
         return self.code_hash == other.code_hash \
             and self.code == other.code \
             and self.code_ref_count == other.code_ref_count \
@@ -1792,17 +1883,21 @@
 # struct database_header_object_ {
 #     uint32_t       version;
 # };
 
 class DatabaseHeaderObject(object):
     by_id = 0
     def __init__(self, table_id: I64, version: U32):
-        self.table_id = table_id
+        self._table_id = table_id
         self.version = version
-    
+
+    @property
+    def table_id(self):
+        return self._table_id
+
     def __repr__(self):
         return f"{{version: {self.version}}}"
     
     def __eq__(self, other):
         return self.version == other.version
     
     def pack(self, enc: Encoder) -> int:
```

### Comparing `ipyeos-0.4.4/pysrc/eos.py` & `ipyeos-0.4.5/pysrc/eos.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import json
 import sys
 from typing import Union
 from enum import Enum
 
 from . import _eos
-from .types import Name
 
 
 class NativeType:
     handshake_message = 0
     chain_size_message = 1
     go_away_message = 2
     time_message = 3
     notice_message = 4
     request_message = 5
     sync_request_message = 6
-    signed_block_v0 = 7         # which = 7
-    packed_transaction_v0 = 8   # which = 8
-    signed_block = 9            # which = 9
-    trx_message_v1 = 10         # which = 10
-    genesis_state = 11
-    abi_def = 12
-    transaction_type = 13
-    global_property_type = 14
+    signed_block = 7         # which = 7
+    packed_transaction = 8   # which = 8
+    genesis_state = 9
+    abi_def = 10
+    transaction_type = 11
+    global_property_type = 12
 
 class LogLevel(Enum):
     ALL = 0
     DEBUG = 1
     INFO = 2
     WARN = 3
     ERROR = 4
@@ -63,28 +60,31 @@
     if isinstance(obj, dict):
         obj = json.dumps(obj)
     else:
         assert isinstance(obj, (str, bytes))
     return _eos.pack_native_object(_type, obj)
 
 def unpack_native_object(_type: int, packed_obj: bytes) -> dict:
-    return _eos.unpack_native_object(_type, packed_obj)
+    ret = _eos.unpack_native_object(_type, packed_obj)
+    if not ret:
+        raise Exception(_eos.get_last_error_and_clear())
+    return ret
 
 def pack_block(obj: Union[dict, str]) -> bytes:
     if isinstance(obj, dict):
         obj = json.dumps(obj)
     else:
         assert isinstance(obj, (str, bytes))
     return _eos.pack_native_object(NativeType.signed_block, obj)
 
 def unpack_block(packed_obj: bytes) -> dict:
     return _eos.unpack_native_object(NativeType.signed_block, packed_obj)
 
 def unpack_transaction(packed_obj: bytes) -> dict:
-    return _eos.unpack_native_object(NativeType.packed_transaction_v0, packed_obj)
+    return _eos.unpack_native_object(NativeType.packed_transaction, packed_obj)
 
 def pack_abi(abi: str) -> bytes:
     if not abi:
         return b''
     return pack_native_object(NativeType.abi_def, abi)
 
 def s2n(s: str) -> int:
@@ -185,12 +185,12 @@
 
 def post(fn, *args, **kwargs):
     return _eos.post(fn, *args, **kwargs)
 
 def quit() -> None:
     _eos.quit()
 
-def set_debug_producer_key(pub_key: str):
-    _eos.set_debug_producer_key(pub_key)
+def base58_to_bytes(s: str):
+    return _eos.base58_to_bytes(s)
 
-def get_debug_producer_key() -> str:
-    return _eos.get_debug_producer_key()
+def bytes_to_base58(data: bytes) -> str:
+    return _eos.bytes_to_base58(data)
```

### Comparing `ipyeos-0.4.4/pysrc/interfaces/Apply.py` & `ipyeos-0.4.5/pysrc/interfaces/Apply.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/interfaces/ApplyRequest.py` & `ipyeos-0.4.5/pysrc/interfaces/ApplyRequest.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/interfaces/IPCChainTester.py` & `ipyeos-0.4.5/pysrc/interfaces/IPCChainTester.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/interfaces/PushActions.py` & `ipyeos-0.4.5/pysrc/interfaces/PushActions.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/interfaces/ttypes.py` & `ipyeos-0.4.5/pysrc/interfaces/ttypes.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/ipykernel_embed.py` & `ipyeos-0.4.5/pysrc/ipykernel_embed.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/ipython_embed.py` & `ipyeos-0.4.5/pysrc/ipython_embed.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/main.py` & `ipyeos-0.4.5/pysrc/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,15 @@
 /ipython start ipython
 /ikernel start ikernel
 /quit quit app
     '''
     return web.Response(text=commands)
 
 def print_help():
-    argv = sys.argv[1:]
-    argv[0] = 'ipyeos'
-    return eos.init(argv)
+    return eos.init(['ipyeos', '--help'])
 
 def _run_eos():
     argv = sys.argv[1:]
     argv[0] = 'ipyeos'
     ret = eos.init(argv)
     if not ret == 0:
         print('init return', ret)
@@ -131,16 +129,17 @@
 
     # result = await future
     # print("Result: ", result)
     print('all done!')
 
 def run():
     if sys.argv[1] == 'eosnode':
-        if sys.argv[2] in ['-h', '--help']:
+        if len(sys.argv) <= 2 or sys.argv[2] in ['-h', '--help']:
             return print_help()
+
         def start():
             asyncio.run(main())
             thread_queue.put(None)
         t = threading.Thread(target=start, daemon=True)
         t.start()
         while True:
             try:
```

### Comparing `ipyeos-0.4.4/pysrc/packer.py` & `ipyeos-0.4.5/pysrc/packer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import struct
 from typing import List, Type, Union, Any
 
 from . import eos
-from .types import U8, U16, U32, U64, I64, U128, U256, Name, Checksum256, PublicKey
+from .types import U8, I16, U16, U32, U64, I64, U128, U256, Name, Checksum256, PublicKey
 
 def pack_length(val: int):
     result = bytearray()
     while True:
         b = val & 0x7f
         val >>= 7
         if val > 0:
@@ -25,14 +25,27 @@
         v |= (b & 0x7f) << by
         by += 7
         n += 1
         if b & 0x80 == 0:
             break
     return v, n
 
+class Packer(object):
+    def pack(self, enc):
+        assert False, "Not implemented"
+
+    def get_bytes(self):
+        enc = Encoder()
+        self.pack(enc)
+        return enc.get_bytes()
+
+    @classmethod
+    def unpack(cls, dec):
+        assert False, "Not implemented"
+
 class Encoder(object):
 
     def __init__(self):
         self.data = []
         self.pos = 0
 
     def write_bytes(self, raw: bytes):
@@ -49,14 +62,19 @@
             self.write_bytes(b'\x00')
 
     def pack_u8(self, n: U8) -> int:
         raw = int.to_bytes(n, 1, 'little')
         self.write_bytes(raw)
         return 1
 
+    def pack_i16(self, n: I16):
+        raw = int.to_bytes(n, 2, 'little', signed=True)
+        self.write_bytes(raw)
+        return 2
+
     def pack_u16(self, n: U16) -> int:
         raw = int.to_bytes(n, 2, 'little')
         self.write_bytes(raw)
         return 2
 
     def pack_u32(self, n: U32) -> int:
         raw = int.to_bytes(n, 4, 'little')
@@ -136,19 +154,23 @@
         for item in l:
             if isinstance(item, str):
                 self.pack_string(item)
             else:
                 self.pack(item)
         return self.get_pos() - pos
 
-    def pack_optional(self, value: Any, tp: Type):
+    def pack_optional(self, value: Any, tp: Type=None):
         if value is None:
             self.pack_u8(0)
             return 1
         self.pack_u8(1)
+
+        if isinstance(value, Packer):
+            return self.pack(value) + 1
+
         if tp is U32:
             return self.pack_u32(value) + 1
         elif tp is U64:
             return self.pack_u64(value) + 1
         elif tp is U128:
             return self.pack_u128(value) + 1
         elif tp is U256:
@@ -166,20 +188,20 @@
 
     def get_bytes(self):
         return b''.join(self.data)
 
 class Decoder(object):
     def __init__(self, raw_data: bytes):
         self.raw_data = raw_data
-        self.pos = 0
+        self._pos = 0
 
     def read_bytes(self, size):
-        assert len(self.raw_data) >= self.pos + size
-        ret = self.raw_data[self.pos:self.pos+size]
-        self.pos += size
+        assert len(self.raw_data) >= self._pos + size
+        ret = self.raw_data[self._pos:self._pos+size]
+        self._pos += size
         return ret
 
     def unpack(self, unpacker):
         return unpacker.unpack(self)
 
     def unpack_name(self):
         name = self.read_bytes(8)
@@ -190,14 +212,18 @@
         assert ret == 0 or ret == 1
         return ret != 0
 
     def unpack_u8(self):
         ret = self.read_bytes(1)[0]
         return ret
 
+    def unpack_i16(self):
+        ret = int.from_bytes(self.read_bytes(2), 'little', signed=True)
+        return ret
+
     def unpack_u16(self):
         ret = int.from_bytes(self.read_bytes(2), 'little')
         return ret
 
     def unpack_u32(self):
         ret = int.from_bytes(self.read_bytes(4), 'little')
         return ret
@@ -273,11 +299,18 @@
     def unpack_public_key(self):
         ret = PublicKey.unpack(self)
         return ret
 
     def get_bytes(self, size):
         ret = self.read_bytes(size)
         return ret
+    
+    @property
+    def pos(self):
+        return self._pos
+
+    def reset_pos(self):
+        self._pos = 0
 
     def get_pos(self):
-        return self.pos
+        return self._pos
```

### Comparing `ipyeos-0.4.4/pysrc/rpc_server.py` & `ipyeos-0.4.5/pysrc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/run.py` & `ipyeos-0.4.5/pysrc/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                 command = 'eosnode'
             elif command.endswith('ipyeos'):
                 cmds = sys.argv[3:]
                 result = args.parse_args(cmds)
                 command = result.subparser
             else:
                 print('unknow command', sys.argv)
+                return
 
             if command == 'eosdebugger':
                 result = args.parse_parent_process_args()
                 url = f'http://{result.addr}:{result.rpc_server_port}/api/quit'
             elif command == 'eosnode':
                 url = 'http://127.0.0.1:7777/quit'
             else:
```

### Comparing `ipyeos-0.4.4/pysrc/server.py` & `ipyeos-0.4.5/pysrc/server.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.4/pysrc/structs.py` & `ipyeos-0.4.5/pysrc/structs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Type, TypeVar, Generic
 
 from .types import U8, U16, U32, U64, I64, Name, PublicKey
-from .packer import Encoder, Decoder
+from .packer import Encoder, Decoder, Packer
 
 T = TypeVar('T')
 
-class KeyWeight(object):
+class KeyWeight(Packer):
     #           shared_public_key key;
     #           weight_type       weight;
     def __init__(self, key: PublicKey, weight: U16):
         self.key = key
         self.weight = weight
 
     def __repr__(self):
@@ -25,15 +25,15 @@
 
     @classmethod
     def unpack(self, dec: Decoder):
         key = dec.unpack_public_key()
         weight = dec.unpack_u16()
         return KeyWeight(key, weight)
 
-class PermissionLevel(object):
+class PermissionLevel(Packer):
 
     def __init__(self, actor: Name, permission: Name):
         self.actor = actor
         self.permission = permission
 
     def __repr__(self):
         return f"{{actor: {self.actor}, permission: {self.permission})}}"
@@ -46,15 +46,15 @@
 
     @classmethod
     def unpack(self, dec: Decoder):
         actor = dec.unpack_name()
         permission = dec.unpack_name()
         return PermissionLevel(actor, permission)
 
-class PermissionLevelWeight(object):
+class PermissionLevelWeight(Packer):
     #       shared_vector<permission_level_weight>     accounts;
     #           permission_level  permission;
     #           weight_type       weight;
     def __init__(self, permission: PermissionLevel, weight: U16):
         self.permission = permission
         self.weight = weight
 
@@ -69,15 +69,15 @@
 
     @classmethod
     def unpack(cls, dec: Decoder):
         permission = PermissionLevel.unpack(dec)
         weight = dec.unpack_u16()
         return PermissionLevelWeight(permission, weight)
 
-class WaitWeight(object):
+class WaitWeight(Packer):
     #           uint32_t     wait_sec;
     #           weight_type  weight;
     def __init__(self, wait_sec: U32, weight: U16):
         self.wait_sec = wait_sec
         self.weight = weight
 
     def __repr__(self):
@@ -93,15 +93,15 @@
 
     @classmethod
     def unpack(cls, dec):
         wait_sec = dec.unpack_u32()
         weight = dec.unpack_u16()
         return WaitWeight(wait_sec, weight)
 
-class Authority(object):
+class Authority(Packer):
 #       uint32_t                                   threshold = 0;
 #       shared_vector<shared_key_weight>           keys;
 #           shared_public_key key;
 #           weight_type       weight;
 #       shared_vector<permission_level_weight>     accounts;
 #           permission_level  permission;
 #           weight_type       weight;
@@ -175,15 +175,15 @@
     @classmethod
     def unpack(cls, dec: Decoder, tp: T):
         type_id = dec.unpack_u8()
         value = tp.unpack(dec)
         return Variant(type_id, value)
 
 
-class TimePoint(object):
+class TimePoint(Packer):
     def __init__(self, time: I64):
         self.time = time
 
     def __repr__(self):
         return f"{{time: {self.time}}}"
 
     def __eq__(self, other) -> bool:
@@ -210,7 +210,86 @@
 #     def pack(self, enc: Encoder):
 #         enc.pack_u32(self.utc_seconds)
 
 #     @classmethod
 #     def unpack(cls, dec: Decoder):
 #         utc_seconds = dec.unpack_u32()
 #         return TimePointSec(utc_seconds)
+
+class Symbol(Packer):
+    def __init__(self, precision: U8, name: str):
+        assert len(name) <= 7 and name.isupper()
+        assert precision <= 18
+        self.precision = precision
+        self.name = name
+
+    def __repr__(self):
+        return f"{{precision: {self.precision}, name: {self.name}}}"
+
+    def __eq__(self, other) -> bool:
+        return self.precision == other.precision and self.name == other.name
+    
+    def pack(self, enc: Encoder):
+        pos = enc.get_pos()
+        enc.pack_u8(self.precision)
+        name = self.name.encode()
+        enc.write_bytes(name + b'\x00' * (7 - len(name)))
+        return enc.get_pos() - pos
+
+    @classmethod
+    def unpack(self, dec: Decoder):
+        precision = dec.unpack_u8()
+        name = dec.read_bytes(7)
+        name = name.rstrip(b'\x00').decode()
+        return Symbol(precision, name)
+
+class Asset(Packer):
+    def __init__(self, amount: I64, symbol: Symbol):
+        self.amount = amount
+        self.symbol = symbol
+
+    def __repr__(self):
+        return f"{{amount: {self.amount}, symbol: {self.symbol}}}"
+
+    def __eq__(self, other) -> bool:
+        return self.amount == other.amount and self.symbol == other.symbol
+
+    def pack(self, enc: Encoder) -> int:
+        pos = enc.get_pos()
+        enc.pack_i64(self.amount)
+        enc.pack(self.symbol)
+        return enc.get_pos() - pos
+
+    def unpack(dec: Decoder):
+        amount = dec.unpack_i64()
+        symbol = Symbol.unpack(dec)
+        return Asset(amount, symbol)
+
+class Transfer(Packer):
+    def __init__(self, sender: Name, recipient: Name, quantity: Asset, memo: str):
+        self.sender = sender
+        self.recipient = recipient
+        self.quantity = quantity
+        self.memo = memo
+
+    def __repr__(self):
+        return f"{{sender: {self.sender}, recipient: {self.recipient}, quantity: {self.quantity}, memo: {self.memo}}}"
+    
+    def __eq__(self, other) -> bool:
+        return self.sender == other.sender and self.recipient == other.recipient \
+                and self.quantity == other.quantity and self.memo == other.memo
+    
+    def pack(self, enc: Encoder) -> int:
+        pos = enc.get_pos()
+        enc.pack_name(self.sender)
+        enc.pack_name(self.recipient)
+        enc.pack(self.quantity)
+        enc.pack_string(self.memo)
+        return enc.get_pos() - pos
+    
+    @classmethod
+    def unpack(cls, dec: Decoder):
+        sender = dec.unpack_name()
+        recipient = dec.unpack_name()
+        quantity = Asset.unpack(dec)
+        memo = dec.unpack_string()
+        return cls(sender, recipient, quantity, memo)
```

