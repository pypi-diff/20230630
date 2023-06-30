# Comparing `tmp/typedb-client-2.8.0.tar.gz` & `tmp/typedb-client-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedb-client-2.8.0.tar", last modified: Tue Mar 22 12:16:40 2022, max compression
+gzip compressed data, was "typedb-client-2.9.0.tar", last modified: Wed May 25 13:41:37 2022, max compression
```

## Comparing `typedb-client-2.8.0.tar` & `typedb-client-2.9.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/
--rw-r--r--   0 grabl     (1000) grabl     (1000)     3091 2022-03-22 12:16:40.752391 typedb-client-2.8.0/PKG-INFO
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1840 2022-03-22 12:16:40.000000 typedb-client-2.8.0/README.md
--rw-r--r--   0 grabl     (1000) grabl     (1000)       67 2022-03-22 12:16:40.752391 typedb-client-2.8.0/setup.cfg
--rw-r--r--   0 grabl     (1000) grabl     (1000)     1982 2022-03-22 12:16:40.000000 typedb-client-2.8.0/setup.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/api/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/api/answer/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/answer/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2229 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/answer/concept_map.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1159 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/answer/concept_map_group.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1202 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/answer/numeric.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1111 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/answer/numeric_group.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/api/concept/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     5764 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/concept.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2293 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/concept_manager.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/api/concept/thing/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/thing/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4314 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/thing/attribute.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1418 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/thing/entity.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2055 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/thing/relation.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2309 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/thing/thing.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/api/concept/type/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     8383 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/attribute_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1709 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/entity_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2131 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/relation_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1935 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/role_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2663 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/thing_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1840 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/concept/type/type.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.744391 typedb-client-2.8.0/typedb/api/connection/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1906 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/client.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1516 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/credential.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2382 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/database.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     5479 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/options.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2062 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/session.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2847 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/transaction.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1454 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/connection/user.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/api/logic/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/logic/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1308 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/logic/explanation.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1206 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/logic/logic_manager.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1609 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/logic/rule.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/api/query/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/query/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1450 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/query/future.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2556 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/api/query/query_manager.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3996 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/client.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/common/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/common/concurrent/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/concurrent/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1658 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/concurrent/atomic.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1881 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/concurrent/lock.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2407 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/concurrent/scheduled_executor.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     7245 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/exception.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2102 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/label.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/common/rpc/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/rpc/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)    26055 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/rpc/request_builder.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3558 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/common/rpc/stub.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/concept/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/__init__.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/concept/answer/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/answer/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     6242 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/answer/concept_map.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1945 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/answer/concept_map_group.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2211 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/answer/numeric.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1487 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/answer/numeric_group.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1072 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/concept.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3721 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/concept_manager.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/concept/proto/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/proto/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3153 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/proto/concept_proto_builder.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     5129 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/proto/concept_proto_reader.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/concept/thing/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/thing/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     9250 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/thing/attribute.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2284 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/thing/entity.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4209 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/thing/relation.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     5367 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/thing/thing.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.748391 typedb-client-2.8.0/typedb/concept/type/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)    11565 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/attribute_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1941 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/entity_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3035 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/relation_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2596 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/role_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4134 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/thing_type.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4696 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/concept/type/type.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb/connection/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3674 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/client.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb/connection/cluster/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     5641 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/client.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)    10394 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/database.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4064 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/database_manager.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3187 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/server_client.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4358 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/session.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     7167 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/stub.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2271 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/user.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3205 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/cluster/user_manager.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb/connection/core/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/core/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1842 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/core/client.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1376 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/core/stub.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     1486 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/database.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2350 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/database_manager.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4794 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/session.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     4625 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/connection/transaction.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb/logic/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/logic/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2894 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/logic/explanation.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     2201 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/logic/logic_manager.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3894 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/logic/rule.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb/query/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/query/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     5717 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/query/query_manager.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb/stream/
--rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/stream/__init__.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     6136 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/stream/bidirectional_stream.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     6741 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/stream/request_transmitter.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3120 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/stream/response_collector.py
--rw-rw-r--   0 grabl     (1000) grabl     (1000)     3315 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb/stream/response_part_iterator.py
-drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-03-22 12:16:40.752391 typedb-client-2.8.0/typedb_client.egg-info/
--rw-r--r--   0 grabl     (1000) grabl     (1000)     3091 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb_client.egg-info/PKG-INFO
--rw-r--r--   0 grabl     (1000) grabl     (1000)     3584 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb_client.egg-info/SOURCES.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb_client.egg-info/dependency_links.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb_client.egg-info/not-zip-safe
--rw-r--r--   0 grabl     (1000) grabl     (1000)       55 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb_client.egg-info/requires.txt
--rw-r--r--   0 grabl     (1000) grabl     (1000)        7 2022-03-22 12:16:40.000000 typedb-client-2.8.0/typedb_client.egg-info/top_level.txt
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.927925 typedb-client-2.9.0/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     2816 2022-05-25 13:41:37.927925 typedb-client-2.9.0/PKG-INFO
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1840 2022-05-25 13:41:36.000000 typedb-client-2.9.0/README.md
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       67 2022-05-25 13:41:37.927925 typedb-client-2.9.0/setup.cfg
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     1982 2022-05-25 13:41:36.000000 typedb-client-2.9.0/setup.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.907924 typedb-client-2.9.0/typedb/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.907924 typedb-client-2.9.0/typedb/api/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.907924 typedb-client-2.9.0/typedb/api/answer/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/answer/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2229 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/answer/concept_map.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1159 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/answer/concept_map_group.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1202 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/answer/numeric.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1111 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/answer/numeric_group.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.907924 typedb-client-2.9.0/typedb/api/concept/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5764 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/concept.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2293 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/concept_manager.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.911924 typedb-client-2.9.0/typedb/api/concept/thing/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/thing/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4314 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/thing/attribute.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1418 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/thing/entity.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2055 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/thing/relation.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2309 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/thing/thing.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.911924 typedb-client-2.9.0/typedb/api/concept/type/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     8499 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/attribute_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1709 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/entity_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2356 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/relation_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1935 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/role_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3182 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/thing_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1840 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/concept/type/type.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.911924 typedb-client-2.9.0/typedb/api/connection/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1906 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/client.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1516 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/credential.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2382 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/database.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5479 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/options.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2062 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/session.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2847 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/transaction.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1454 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/connection/user.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.911924 typedb-client-2.9.0/typedb/api/logic/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/logic/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1308 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/logic/explanation.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1206 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/logic/logic_manager.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1609 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/logic/rule.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.915924 typedb-client-2.9.0/typedb/api/query/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/query/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1450 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/query/future.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2556 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/api/query/query_manager.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3996 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/client.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.915924 typedb-client-2.9.0/typedb/common/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.915924 typedb-client-2.9.0/typedb/common/concurrent/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/concurrent/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1658 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/concurrent/atomic.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1881 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/concurrent/lock.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2407 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/concurrent/scheduled_executor.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     7245 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/exception.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2102 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/label.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.915924 typedb-client-2.9.0/typedb/common/rpc/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/rpc/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)    28598 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/rpc/request_builder.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3558 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/common/rpc/stub.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.915924 typedb-client-2.9.0/typedb/concept/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/__init__.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.915924 typedb-client-2.9.0/typedb/concept/answer/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/answer/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     6242 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/answer/concept_map.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1945 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/answer/concept_map_group.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2211 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/answer/numeric.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1487 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/answer/numeric_group.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1072 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/concept.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3721 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/concept_manager.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.919925 typedb-client-2.9.0/typedb/concept/proto/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/proto/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3153 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/proto/concept_proto_builder.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5129 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/proto/concept_proto_reader.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.919925 typedb-client-2.9.0/typedb/concept/thing/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/thing/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     9250 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/thing/attribute.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2284 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/thing/entity.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4209 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/thing/relation.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5367 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/thing/thing.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.919925 typedb-client-2.9.0/typedb/concept/type/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)    11936 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/attribute_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1941 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/entity_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3626 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/relation_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2596 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/role_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5676 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/thing_type.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4696 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/concept/type/type.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.919925 typedb-client-2.9.0/typedb/connection/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3674 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/client.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.923925 typedb-client-2.9.0/typedb/connection/cluster/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5641 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/client.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)    10394 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/database.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4064 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/database_manager.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3187 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/server_client.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4358 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/session.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     7167 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/stub.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2271 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/user.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3205 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/cluster/user_manager.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.923925 typedb-client-2.9.0/typedb/connection/core/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/core/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1842 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/core/client.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1376 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/core/stub.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     1486 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/database.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2350 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/database_manager.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4794 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/session.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     4625 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/connection/transaction.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.923925 typedb-client-2.9.0/typedb/logic/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/logic/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2894 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/logic/explanation.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     2201 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/logic/logic_manager.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3894 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/logic/rule.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.923925 typedb-client-2.9.0/typedb/query/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/query/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     5717 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/query/query_manager.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.923925 typedb-client-2.9.0/typedb/stream/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/stream/__init__.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     6136 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/stream/bidirectional_stream.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     6741 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/stream/request_transmitter.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3120 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/stream/response_collector.py
+-rw-rw-r--   0 grabl     (1000) grabl     (1000)     3315 2022-05-25 13:41:36.000000 typedb-client-2.9.0/typedb/stream/response_part_iterator.py
+drwxr-xr-x   0 grabl     (1000) grabl     (1000)        0 2022-05-25 13:41:37.927925 typedb-client-2.9.0/typedb_client.egg-info/
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     2816 2022-05-25 13:41:37.000000 typedb-client-2.9.0/typedb_client.egg-info/PKG-INFO
+-rw-r--r--   0 grabl     (1000) grabl     (1000)     3584 2022-05-25 13:41:37.000000 typedb-client-2.9.0/typedb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-05-25 13:41:37.000000 typedb-client-2.9.0/typedb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        1 2022-05-25 13:41:37.000000 typedb-client-2.9.0/typedb_client.egg-info/not-zip-safe
+-rw-r--r--   0 grabl     (1000) grabl     (1000)       55 2022-05-25 13:41:37.000000 typedb-client-2.9.0/typedb_client.egg-info/requires.txt
+-rw-r--r--   0 grabl     (1000) grabl     (1000)        7 2022-05-25 13:41:37.000000 typedb-client-2.9.0/typedb_client.egg-info/top_level.txt
```

### Comparing `typedb-client-2.8.0/PKG-INFO` & `typedb-client-2.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,15 @@
 Metadata-Version: 2.1
 Name: typedb-client
-Version: 2.8.0
+Version: 2.9.0
 Summary: TypeDB Client for Python
 Home-page: https://github.com/vaticle/typedb-client-python/
 Author: Vaticle
 Author-email: community@vaticle.com
 License: Apache-2.0
-Description: # TypeDB Client for Python
-        
-        [![Grabl](https://grabl.io/api/status/vaticle/typedb-client-python/badge.svg)](https://grabl.io/vaticle/typedb)
-        [![GitHub release](https://img.shields.io/github/release/vaticle/typedb-client-python.svg)](https://github.com/vaticle/typedb/releases/latest)
-        [![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
-        [![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
-        
-        ## Client Architecture
-        To learn about the mechanism that a TypeDB Client uses to set up communication with databases running on the TypeDB Server, refer to [TypeDB > Client API > Overview](http://docs.vaticle.com/docs/client-api/overview).
-        
-        ## API Reference
-        To learn about the methods available for executing queries and retrieving their answers using Client Python, refer to [TypeDB > Client API > Python > API Reference](http://docs.vaticle.com/docs/client-api/python#api-reference).
-        
-        ## Concept API
-        To learn about the methods available on the concepts retrieved as the answers to TypeQL queries, refer to [TypeDB > Concept API > Overview](http://docs.vaticle.com/docs/concept-api/overview)
-        
-        ## Install TypeDB Client for Python through Pip
-        ```
-        pip install typedb-client
-        ```
-        If multiple Python versions are available, you may wish to use
-        ```
-        pip3 install typedb-client
-        ```
-        
-        In your python program, import from typedb.client:
-        ```py
-        from typedb.client import *
-        
-        client = TypeDB.core_client(address=TypeDB.DEFAULT_ADDRESS)
-        ```
-        
 Keywords: typedb database graph knowledgebase knowledge-engineering
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -52,7 +18,43 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
+
+# TypeDB Client for Python
+
+[![Grabl](https://grabl.io/api/status/vaticle/typedb-client-python/badge.svg)](https://grabl.io/vaticle/typedb)
+[![GitHub release](https://img.shields.io/github/release/vaticle/typedb-client-python.svg)](https://github.com/vaticle/typedb/releases/latest)
+[![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
+[![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
+
+## Client Architecture
+To learn about the mechanism that a TypeDB Client uses to set up communication with databases running on the TypeDB Server, refer to [TypeDB > Client API > Overview](http://docs.vaticle.com/docs/client-api/overview).
+
+## API Reference
+To learn about the methods available for executing queries and retrieving their answers using Client Python, refer to [TypeDB > Client API > Python > API Reference](http://docs.vaticle.com/docs/client-api/python#api-reference).
+
+## Concept API
+To learn about the methods available on the concepts retrieved as the answers to TypeQL queries, refer to [TypeDB > Concept API > Overview](http://docs.vaticle.com/docs/concept-api/overview)
+
+## Install TypeDB Client for Python through Pip
+```
+pip install typedb-client
+```
+If multiple Python versions are available, you may wish to use
+```
+pip3 install typedb-client
+```
+
+In your python program, import from typedb.client:
+```py
+from typedb.client import *
+
+client = TypeDB.core_client(address=TypeDB.DEFAULT_ADDRESS)
+```
+
+
```

### Comparing `typedb-client-2.8.0/README.md` & `typedb-client-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/setup.py` & `typedb-client-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 from setuptools import setup
 from setuptools import find_packages
 
 packages = find_packages()
 
 setup(
     name = "typedb-client",
-    version = "2.8.0",
+    version = "2.9.0",
     description = "TypeDB Client for Python",
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers = ["Programming Language :: Python", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.5", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Environment :: Console", "Topic :: Database :: Front-Ends"],
     keywords = "typedb database graph knowledgebase knowledge-engineering",
     url = "https://github.com/vaticle/typedb-client-python/",
     author = "Vaticle",
     author_email = "community@vaticle.com",
     license = "Apache-2.0",
     packages=packages,
-    install_requires=['typedb-protocol==2.6.0', 'grpcio==1.43.0', 'protobuf==3.15.5'],
+    install_requires=['typedb-protocol==2.9.0', 'grpcio==1.43.0', 'protobuf==3.15.5'],
     zip_safe=False,
 )
```

### Comparing `typedb-client-2.8.0/typedb/api/answer/concept_map.py` & `typedb-client-2.9.0/typedb/api/answer/concept_map.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/answer/concept_map_group.py` & `typedb-client-2.9.0/typedb/api/answer/concept_map_group.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/answer/numeric.py` & `typedb-client-2.9.0/typedb/api/answer/numeric.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/answer/numeric_group.py` & `typedb-client-2.9.0/typedb/api/answer/numeric_group.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/concept.py` & `typedb-client-2.9.0/typedb/api/concept/concept.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/concept_manager.py` & `typedb-client-2.9.0/typedb/api/concept/concept_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/thing/attribute.py` & `typedb-client-2.9.0/typedb/api/concept/thing/attribute.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/thing/entity.py` & `typedb-client-2.9.0/typedb/api/concept/thing/entity.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/thing/relation.py` & `typedb-client-2.9.0/typedb/api/concept/thing/relation.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/thing/thing.py` & `typedb-client-2.9.0/typedb/api/concept/thing/thing.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/type/attribute_type.py` & `typedb-client-2.9.0/typedb/api/concept/type/attribute_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,18 @@
         pass
 
     @abstractmethod
     def get_owners(self, only_key: bool = False) -> Iterator[ThingType]:
         pass
 
     @abstractmethod
+    def get_owners_explicit(self, only_key: bool = False) -> Iterator[ThingType]:
+        pass
+
+    @abstractmethod
     def as_boolean(self) -> "RemoteBooleanAttributeType":
         pass
 
     @abstractmethod
     def as_long(self) -> "RemoteLongAttributeType":
         pass
```

### Comparing `typedb-client-2.8.0/typedb/api/concept/type/entity_type.py` & `typedb-client-2.9.0/typedb/api/concept/type/entity_type.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/type/relation_type.py` & `typedb-client-2.9.0/typedb/api/concept/type/relation_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Iterator, Union
+from typing import TYPE_CHECKING, Iterator, Union, Optional
 
 from typedb.api.concept.thing.relation import Relation
 from typedb.api.concept.type.role_type import RoleType
 from typedb.api.concept.type.thing_type import ThingType, RemoteThingType
 
 if TYPE_CHECKING:
     from typedb.api.connection.transaction import TypeDBTransaction
@@ -46,25 +46,33 @@
         pass
 
     @abstractmethod
     def get_instances(self) -> Iterator["Relation"]:
         pass
 
     @abstractmethod
-    def get_relates(self, role_label: str = None) -> Union[RoleType, Iterator[RoleType]]:
+    def get_relates(self, role_label: str = None) -> Union["RoleType", Iterator["RoleType"]]:
+        pass
+
+    @abstractmethod
+    def get_relates_explicit(self) -> Iterator["RoleType"]:
+        pass
+
+    @abstractmethod
+    def get_relates_overridden(self, role_label: str) -> Optional["RoleType"]:
         pass
 
     @abstractmethod
     def set_relates(self, role_label: str, overridden_label: str = None) -> None:
         pass
 
     @abstractmethod
     def unset_relates(self, role_label: str) -> None:
         pass
 
     @abstractmethod
-    def get_subtypes(self) -> Iterator[RelationType]:
+    def get_subtypes(self) -> Iterator["RelationType"]:
         pass
 
     @abstractmethod
-    def set_supertype(self, relation_type: RelationType) -> None:
+    def set_supertype(self, relation_type: "RelationType") -> None:
         pass
```

### Comparing `typedb-client-2.8.0/typedb/api/concept/type/role_type.py` & `typedb-client-2.9.0/typedb/api/concept/type/role_type.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/concept/type/thing_type.py` & `typedb-client-2.9.0/typedb/api/concept/type/thing_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Iterator
+from typing import TYPE_CHECKING, Iterator, Optional
 
 from typedb.api.concept.thing.thing import Thing
-from typedb.api.concept.type.type import Type, RemoteType
 from typedb.api.concept.type.role_type import RoleType
+from typedb.api.concept.type.type import Type, RemoteType
 
 if TYPE_CHECKING:
     from typedb.api.concept.type.attribute_type import AttributeType
     from typedb.api.connection.transaction import TypeDBTransaction
 
 
 class ThingType(Type, ABC):
@@ -71,21 +71,37 @@
         pass
 
     @abstractmethod
     def set_owns(self, attribute_type: "AttributeType", overridden_type: "AttributeType" = None, is_key: bool = False) -> None:
         pass
 
     @abstractmethod
-    def get_plays(self) -> Iterator[RoleType]:
+    def get_plays(self) -> Iterator["RoleType"]:
+        pass
+
+    @abstractmethod
+    def get_plays_explicit(self) -> Iterator["RoleType"]:
+        pass
+
+    @abstractmethod
+    def get_plays_overridden(self, role_type: "RoleType") -> Optional["RoleType"]:
         pass
 
     @abstractmethod
     def get_owns(self, value_type: "AttributeType.ValueType" = None, keys_only: bool = False) -> Iterator["AttributeType"]:
         pass
 
     @abstractmethod
+    def get_owns_explicit(self, value_type: "AttributeType.ValueType" = None, keys_only: bool = False) -> Iterator["AttributeType"]:
+        pass
+
+    @abstractmethod
+    def get_owns_overridden(self, attribute_type: "AttributeType") -> Optional["AttributeType"]:
+        pass
+
+    @abstractmethod
     def unset_plays(self, role_type: "RoleType") -> None:
         pass
 
     @abstractmethod
     def unset_owns(self, attribute_type: "AttributeType") -> None:
         pass
```

### Comparing `typedb-client-2.8.0/typedb/api/concept/type/type.py` & `typedb-client-2.9.0/typedb/api/concept/type/type.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/client.py` & `typedb-client-2.9.0/typedb/api/connection/client.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/credential.py` & `typedb-client-2.9.0/typedb/api/connection/credential.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/database.py` & `typedb-client-2.9.0/typedb/api/connection/database.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/options.py` & `typedb-client-2.9.0/typedb/api/connection/options.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/session.py` & `typedb-client-2.9.0/typedb/api/connection/session.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/transaction.py` & `typedb-client-2.9.0/typedb/api/connection/transaction.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/connection/user.py` & `typedb-client-2.9.0/typedb/api/connection/user.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/logic/explanation.py` & `typedb-client-2.9.0/typedb/api/logic/explanation.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/logic/logic_manager.py` & `typedb-client-2.9.0/typedb/api/logic/logic_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/logic/rule.py` & `typedb-client-2.9.0/typedb/api/logic/rule.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/query/future.py` & `typedb-client-2.9.0/typedb/api/query/future.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/api/query/query_manager.py` & `typedb-client-2.9.0/typedb/api/query/query_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/client.py` & `typedb-client-2.9.0/typedb/client.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/common/concurrent/atomic.py` & `typedb-client-2.9.0/typedb/common/concurrent/atomic.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/common/concurrent/lock.py` & `typedb-client-2.9.0/typedb/common/concurrent/lock.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/common/concurrent/scheduled_executor.py` & `typedb-client-2.9.0/typedb/common/concurrent/scheduled_executor.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/common/exception.py` & `typedb-client-2.9.0/typedb/common/exception.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/common/label.py` & `typedb-client-2.9.0/typedb/common/label.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/common/rpc/request_builder.py` & `typedb-client-2.9.0/typedb/common/rpc/request_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,48 +78,53 @@
 # ClusterDatabaseManager
 
 def cluster_database_manager_get_req(name: str):
     req = cluster_database_proto.ClusterDatabaseManager.Get.Req()
     req.name = name
     return req
 
+
 def cluster_database_manager_all_req():
     return cluster_database_proto.ClusterDatabaseManager.All.Req()
 
 
 # ClusterUserManager
 
 def cluster_user_manager_all_req():
     return cluster_user_proto.ClusterUserManager.All.Req()
 
+
 def cluster_user_manager_create_req(username: str, password: str):
     req = cluster_user_proto.ClusterUserManager.Create.Req()
     req.username = username
     req.password = password
     return req
 
+
 def cluster_user_manager_contains_req(username: str):
     req = cluster_user_proto.ClusterUserManager.Contains.Req()
     req.username = username
     return req
 
 
 # ClusterUser
 
 def cluster_user_password_req(username: str, password: str):
     req = cluster_user_proto.ClusterUser.Password.Req()
     req.username = username
     req.password = password
     return req
 
+
 def cluster_user_token_req(username: str):
     req = cluster_user_proto.ClusterUser.Token.Req()
     req.username = username
     return req
 
+
 def cluster_user_delete_req(username: str):
     req = cluster_user_proto.ClusterUser.Delete.Req()
     req.username = username
     return req
 
 
 # Session
@@ -458,43 +463,79 @@
 
 def thing_type_get_plays_req(label: Label):
     req = concept_proto.Type.Req()
     req.thing_type_get_plays_req.CopyFrom(concept_proto.ThingType.GetPlays.Req())
     return type_req(req, label)
 
 
-def thing_type_set_plays_req(label: Label, role_type: concept_proto.Type, overridden_role_type: concept_proto.Type = None):
+def thing_type_get_plays_explicit_req(label: Label):
+    req = concept_proto.Type.Req()
+    req.thing_type_get_plays_explicit_req.CopyFrom(concept_proto.ThingType.GetPlaysExplicit.Req())
+    return type_req(req, label)
+
+
+def thing_type_get_plays_overridden(label: Label, role_type: concept_proto.Type):
+    req = concept_proto.Type.Req()
+    get_plays_overridden_req = concept_proto.Type.GetPlaysOverridden.Req()
+    get_plays_overridden_req.role_type.CopyFrom(role_type)
+    req.thing_type_get_plays_overridden_req.CopyFrom(get_plays_overridden_req)
+    return type_req(req, label)
+
+
+def thing_type_set_plays_req(label: Label, role_type: concept_proto.Type,
+                             overridden_role_type: concept_proto.Type = None):
     req = concept_proto.Type.Req()
     set_plays_req = concept_proto.ThingType.SetPlays.Req()
-    set_plays_req.role.CopyFrom(role_type)
+    set_plays_req.role_type.CopyFrom(role_type)
     if overridden_role_type:
-        set_plays_req.overridden_role.CopyFrom(overridden_role_type)
+        set_plays_req.overridden_type.CopyFrom(overridden_role_type)
     req.thing_type_set_plays_req.CopyFrom(set_plays_req)
     return type_req(req, label)
 
 
 def thing_type_unset_plays_req(label: Label, role_type: concept_proto.Type):
     req = concept_proto.Type.Req()
     unset_plays_req = concept_proto.ThingType.UnsetPlays.Req()
-    unset_plays_req.role.CopyFrom(role_type)
+    unset_plays_req.role_type.CopyFrom(role_type)
     req.thing_type_unset_plays_req.CopyFrom(unset_plays_req)
     return type_req(req, label)
 
 
-def thing_type_get_owns_req(label: Label, value_type: concept_proto.AttributeType.ValueType = None, keys_only: bool = False):
+def thing_type_get_owns_req(label: Label, value_type: concept_proto.AttributeType.ValueType = None,
+                            keys_only: bool = False):
     req = concept_proto.Type.Req()
     get_owns_req = concept_proto.ThingType.GetOwns.Req()
     get_owns_req.keys_only = keys_only
     if value_type:
         get_owns_req.value_type = value_type
     req.thing_type_get_owns_req.CopyFrom(get_owns_req)
     return type_req(req, label)
 
 
-def thing_type_set_owns_req(label: Label, attribute_type: concept_proto.Type, overridden_type: concept_proto.Type = None, is_key: bool = False):
+def thing_type_get_owns_explicit_req(label: Label, value_type: concept_proto.AttributeType.ValueType = None,
+                                     keys_only: bool = False):
+    req = concept_proto.Type.Req()
+    get_owns_explicit_req = concept_proto.ThingType.GetOwnsExplicit.Req()
+    get_owns_explicit_req.keys_only = keys_only
+    if value_type:
+        get_owns_explicit_req.value_type = value_type
+    req.thing_type_get_owns_explicit_req.CopyFrom(get_owns_explicit_req)
+    return type_req(req, label)
+
+
+def thing_type_get_owns_overridden_req(label: Label, attribute_type: concept_proto.Type):
+    req = concept_proto.Type.Req()
+    get_owns_overridden_req = concept_proto.ThingType.GetOwnsOverridden.Req()
+    get_owns_overridden_req.attribute_type.CopyFrom(attribute_type)
+    req.thing_type_get_owns_overridden_req.CopyFrom(get_owns_overridden_req)
+    return type_req(req, label)
+
+
+def thing_type_set_owns_req(label: Label, attribute_type: concept_proto.Type,
+                            overridden_type: concept_proto.Type = None, is_key: bool = False):
     req = concept_proto.Type.Req()
     set_owns_req = concept_proto.ThingType.SetOwns.Req()
     set_owns_req.attribute_type.CopyFrom(attribute_type)
     set_owns_req.is_key = is_key
     if overridden_type:
         set_owns_req.overridden_type.CopyFrom(overridden_type)
     req.thing_type_set_owns_req.CopyFrom(set_owns_req)
@@ -540,14 +581,28 @@
         get_relates_req.label = role_label
         req.relation_type_get_relates_for_role_label_req.CopyFrom(get_relates_req)
     else:
         req.relation_type_get_relates_req.CopyFrom(concept_proto.RelationType.GetRelates.Req())
     return type_req(req, label)
 
 
+def relation_type_get_relates_explicit_req(label: Label):
+    req = concept_proto.Type.Req()
+    req.relation_type_get_relates_explicit_req.CopyFrom(concept_proto.RelationType.GetRelatesExplicit.Req())
+    return type_req(req, label)
+
+
+def relation_type_get_relates_overridden_req(label: Label, role_label: str):
+    req = concept_proto.Type.Req()
+    get_relates_overridden_req = concept_proto.RelationType.GetRelatesOverridden.Req()
+    get_relates_overridden_req.label = role_label
+    req.relation_type_get_relates_overridden_req.CopyFrom(get_relates_overridden_req)
+    return type_req(req, label)
+
+
 def relation_type_set_relates_req(label: Label, role_label: str, overridden_label: str = None):
     req = concept_proto.Type.Req()
     set_relates_req = concept_proto.RelationType.SetRelates.Req()
     set_relates_req.label = role_label
     if overridden_label:
         set_relates_req.overridden_label = overridden_label
     req.relation_type_set_relates_req.CopyFrom(set_relates_req)
@@ -568,14 +623,22 @@
     req = concept_proto.Type.Req()
     get_owners_req = concept_proto.AttributeType.GetOwners.Req()
     get_owners_req.only_key = only_key
     req.attribute_type_get_owners_req.CopyFrom(get_owners_req)
     return type_req(req, label)
 
 
+def attribute_type_get_owners_explicit_req(label: Label, only_key: bool = False):
+    req = concept_proto.Type.Req()
+    get_owners_explicit_req = concept_proto.AttributeType.GetOwnersExplicit.Req()
+    get_owners_explicit_req.only_key = only_key
+    req.attribute_type_get_owners_explicit_req.CopyFrom(get_owners_explicit_req)
+    return type_req(req, label)
+
+
 def attribute_type_put_req(label: Label, value: concept_proto.Attribute.Value):
     req = concept_proto.Type.Req()
     put_req = concept_proto.AttributeType.Put.Req()
     put_req.value.CopyFrom(value)
     req.attribute_type_put_req.CopyFrom(put_req)
     return type_req(req, label)
```

### Comparing `typedb-client-2.8.0/typedb/common/rpc/stub.py` & `typedb-client-2.9.0/typedb/common/rpc/stub.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/answer/concept_map.py` & `typedb-client-2.9.0/typedb/concept/answer/concept_map.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/answer/concept_map_group.py` & `typedb-client-2.9.0/typedb/concept/answer/concept_map_group.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/answer/numeric.py` & `typedb-client-2.9.0/typedb/concept/answer/numeric.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/answer/numeric_group.py` & `typedb-client-2.9.0/typedb/concept/answer/numeric_group.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/concept.py` & `typedb-client-2.9.0/typedb/concept/concept.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/concept_manager.py` & `typedb-client-2.9.0/typedb/concept/concept_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/proto/concept_proto_builder.py` & `typedb-client-2.9.0/typedb/concept/proto/concept_proto_builder.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/proto/concept_proto_reader.py` & `typedb-client-2.9.0/typedb/concept/proto/concept_proto_reader.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/thing/attribute.py` & `typedb-client-2.9.0/typedb/concept/thing/attribute.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/thing/entity.py` & `typedb-client-2.9.0/typedb/concept/thing/entity.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/thing/relation.py` & `typedb-client-2.9.0/typedb/concept/thing/relation.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/thing/thing.py` & `typedb-client-2.9.0/typedb/concept/thing/thing.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/type/attribute_type.py` & `typedb-client-2.9.0/typedb/concept/type/attribute_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 from typedb.api.concept.type.attribute_type import AttributeType, RemoteAttributeType, BooleanAttributeType, \
     RemoteBooleanAttributeType, LongAttributeType, RemoteLongAttributeType, DoubleAttributeType, \
     RemoteDoubleAttributeType, StringAttributeType, RemoteStringAttributeType, DateTimeAttributeType, \
     RemoteDateTimeAttributeType
 from typedb.common.exception import TypeDBClientException, INVALID_CONCEPT_CASTING
 from typedb.common.label import Label
 from typedb.common.rpc.request_builder import attribute_type_get_owners_req, attribute_type_put_req, \
-    attribute_type_get_req, attribute_type_get_regex_req, attribute_type_set_regex_req
+    attribute_type_get_req, attribute_type_get_regex_req, attribute_type_set_regex_req, \
+    attribute_type_get_owners_explicit_req
 from typedb.concept.proto import concept_proto_builder, concept_proto_reader
 from typedb.concept.type.thing_type import _ThingType, _RemoteThingType
 
 
 class _AttributeType(AttributeType, _ThingType):
 
     ROOT_LABEL = Label.of("attribute")
@@ -97,16 +98,22 @@
         stream = super(_RemoteAttributeType, self).get_subtypes()
         if self.is_root() and self.get_value_type() is not AttributeType.ValueType.OBJECT:
             return (subtype for subtype in stream if subtype.get_value_type() is self.get_value_type() or subtype.get_label() == self.get_label())
         else:
             return stream
 
     def get_owners(self, only_key: bool = False):
-        return (concept_proto_reader.thing_type(tt) for rp in self.stream(attribute_type_get_owners_req(self.get_label(), only_key))
-                for tt in rp.attribute_type_get_owners_res_part.owners)
+        return (concept_proto_reader.thing_type(tt)
+                for rp in self.stream(attribute_type_get_owners_req(self.get_label(), only_key))
+                for tt in rp.attribute_type_get_owners_res_part.thing_types)
+
+    def get_owners_explicit(self, only_key: bool = False):
+        return (concept_proto_reader.thing_type(tt)
+                for rp in self.stream(attribute_type_get_owners_explicit_req(self.get_label(), only_key))
+                for tt in rp.attribute_type_get_owners_explicit_res_part.thing_types)
 
     def put_internal(self, proto_value: concept_proto.Attribute.Value):
         res = self.execute(attribute_type_put_req(self.get_label(), proto_value)).attribute_type_put_res
         return concept_proto_reader.attribute(res.attribute)
 
     def get_internal(self, proto_value: concept_proto.Attribute.Value):
         res = self.execute(attribute_type_get_req(self.get_label(), proto_value)).attribute_type_get_res
```

### Comparing `typedb-client-2.8.0/typedb/concept/type/entity_type.py` & `typedb-client-2.9.0/typedb/concept/type/entity_type.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/concept/type/relation_type.py` & `typedb-client-2.9.0/typedb/concept/type/role_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,58 +14,51 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-from typing import Iterator, TYPE_CHECKING
 
 import typedb_protocol.common.concept_pb2 as concept_proto
 
-from typedb.api.concept.thing.relation import Relation
-from typedb.api.concept.type.relation_type import RelationType, RemoteRelationType
+from typedb.api.concept.type.role_type import RoleType, RemoteRoleType
 from typedb.common.label import Label
-from typedb.common.rpc.request_builder import relation_type_create_req, relation_type_get_relates_req, \
-    relation_type_set_relates_req, relation_type_unset_relates_req
-from typedb.concept.thing.relation import _Relation
-from typedb.concept.type.role_type import _RoleType
-from typedb.concept.type.thing_type import _ThingType, _RemoteThingType
+from typedb.common.rpc.request_builder import role_type_get_relation_types_req, role_type_get_players_req
+from typedb.concept.proto import concept_proto_reader
+from typedb.concept.type.type import _Type, _RemoteType
 
 
-class _RelationType(RelationType, _ThingType):
+class _RoleType(_Type, RoleType):
 
     @staticmethod
     def of(type_proto: concept_proto.Type):
-        return _RelationType(Label.of(type_proto.label), type_proto.root)
+        return _RoleType(Label.of(type_proto.scope, type_proto.label), type_proto.root)
 
     def as_remote(self, transaction):
-        return _RemoteRelationType(transaction, self.get_label(), self.is_root())
+        return _RemoteRoleType(transaction, self.get_label(), self.is_root())
 
-    def as_relation_type(self) -> "RelationType":
+    def as_role_type(self) -> "RoleType":
         return self
 
 
-class _RemoteRelationType(_RemoteThingType, RemoteRelationType):
+class _RemoteRoleType(_RemoteType, RemoteRoleType):
 
     def as_remote(self, transaction):
-        return _RemoteRelationType(transaction, self.get_label(), self.is_root())
+        return _RemoteRoleType(transaction, self.get_label(), self.is_root())
 
-    def as_relation_type(self) -> "RemoteRelationType":
+    def as_role_type(self) -> "RemoteRoleType":
         return self
 
-    def create(self):
-        return _Relation.of(self.execute(relation_type_create_req(self.get_label())).relation_type_create_res.relation)
+    def get_relation_type(self):
+        return self._transaction_ext.concepts().get_relation_type(self.get_label().scope())
 
-    def get_relates(self, role_label: str = None):
-        if role_label:
-            res = self.execute(relation_type_get_relates_req(self.get_label(), role_label)).relation_type_get_relates_for_role_label_res
-            return _RoleType.of(res.role_type) if res.HasField("role_type") else None
-        else:
-            return (_RoleType.of(rt) for rp in self.stream(relation_type_get_relates_req(self.get_label()))
-                    for rt in rp.relation_type_get_relates_res_part.roles)
+    def get_relation_types(self):
+        return (concept_proto_reader.type_(rt) for rp in self.stream(role_type_get_relation_types_req(self.get_label()))
+                for rt in rp.role_type_get_relation_types_res_part.relation_types)
+
+    def get_players(self):
+        return (concept_proto_reader.thing_type(tt) for rp in self.stream(role_type_get_players_req(self.get_label()))
+                for tt in rp.role_type_get_players_res_part.thing_types)
 
-    def set_relates(self, role_label: str, overridden_label: str = None):
-        self.execute(relation_type_set_relates_req(self.get_label(), role_label, overridden_label))
-
-    def unset_relates(self, role_label: str):
-        self.execute(relation_type_unset_relates_req(self.get_label(), role_label))
+    def is_deleted(self) -> bool:
+        return self.get_relation_type() is not None and self.get_relation_type().as_remote(self._transaction_ext).get_relates(self.get_label().name()) is not None
```

### Comparing `typedb-client-2.8.0/typedb/concept/type/thing_type.py` & `typedb-client-2.9.0/typedb/concept/type/thing_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-from typing import Iterator
 
 from typedb.api.concept.type.attribute_type import AttributeType
 from typedb.api.concept.type.role_type import RoleType
 from typedb.api.concept.type.thing_type import ThingType, RemoteThingType
-from typedb.common.label import Label
 from typedb.common.rpc.request_builder import thing_type_set_supertype_req, thing_type_get_instances_req, \
     thing_type_set_abstract_req, thing_type_unset_abstract_req, thing_type_set_plays_req, thing_type_set_owns_req, \
-    thing_type_get_plays_req, thing_type_get_owns_req, thing_type_unset_plays_req, thing_type_unset_owns_req
+    thing_type_get_plays_req, thing_type_get_owns_req, thing_type_unset_plays_req, thing_type_unset_owns_req, \
+    thing_type_get_owns_explicit_req, thing_type_get_owns_overridden_req, thing_type_get_plays_explicit_req, \
+    thing_type_get_plays_overridden
 from typedb.concept.proto import concept_proto_builder, concept_proto_reader
 from typedb.concept.type.type import _Type, _RemoteType
 
 
 class _ThingType(ThingType, _Type):
 
     def as_remote(self, transaction):
@@ -61,25 +61,51 @@
     def set_abstract(self):
         self.execute(thing_type_set_abstract_req(self.get_label()))
 
     def unset_abstract(self):
         self.execute(thing_type_unset_abstract_req(self.get_label()))
 
     def set_plays(self, role_type: RoleType, overridden_role_type: RoleType = None):
-        self.execute(thing_type_set_plays_req(self.get_label(), concept_proto_builder.role_type(role_type), concept_proto_builder.role_type(overridden_role_type)))
+        self.execute(thing_type_set_plays_req(self.get_label(), concept_proto_builder.role_type(role_type),
+                                              concept_proto_builder.role_type(overridden_role_type)))
 
-    def set_owns(self, attribute_type: AttributeType, overridden_type: AttributeType = None, is_key: bool = False):
-        self.execute(thing_type_set_owns_req(self.get_label(), concept_proto_builder.thing_type(attribute_type), concept_proto_builder.thing_type(overridden_type), is_key))
+    def unset_plays(self, role_type: RoleType):
+        self.execute(thing_type_unset_plays_req(self.get_label(), concept_proto_builder.role_type(role_type)))
 
     def get_plays(self):
         return (concept_proto_reader.type_(t) for rp in self.stream(thing_type_get_plays_req(self.get_label()))
-                for t in rp.thing_type_get_plays_res_part.roles)
+                for t in rp.thing_type_get_plays_res_part.role_types)
 
-    def get_owns(self, value_type: AttributeType.ValueType = None, keys_only: bool = False):
-        return (concept_proto_reader.type_(t) for rp in self.stream(thing_type_get_owns_req(self.get_label(), value_type.proto() if value_type else None, keys_only))
-                for t in rp.thing_type_get_owns_res_part.attribute_types)
+    def get_plays_explicit(self):
+        return (concept_proto_reader.type_(t) for rp in self.stream(thing_type_get_plays_explicit_req(self.get_label()))
+                for t in rp.thing_type_get_plays_explicit_res_part.role_types)
+
+    def get_plays_overridden(self, role_type: "RoleType"):
+        res = self.execute(thing_type_get_plays_overridden(
+            self.get_label(), concept_proto_builder.role_type(role_type)
+        )).thing_type_get_plays_overridden_res
+        return concept_proto_reader.type_(res.role_type) if res.HasField("role_type") else None
 
-    def unset_plays(self, role_type: RoleType):
-        self.execute(thing_type_unset_plays_req(self.get_label(), concept_proto_builder.role_type(role_type)))
+    def set_owns(self, attribute_type: AttributeType, overridden_type: AttributeType = None, is_key: bool = False):
+        self.execute(thing_type_set_owns_req(self.get_label(), concept_proto_builder.thing_type(attribute_type),
+                                             concept_proto_builder.thing_type(overridden_type), is_key))
 
     def unset_owns(self, attribute_type: AttributeType):
         self.execute(thing_type_unset_owns_req(self.get_label(), concept_proto_builder.thing_type(attribute_type)))
+
+    def get_owns(self, value_type: AttributeType.ValueType = None, keys_only: bool = False):
+        return (concept_proto_reader.type_(t)
+                for rp in self.stream(
+            thing_type_get_owns_req(self.get_label(), value_type.proto() if value_type else None, keys_only))
+                for t in rp.thing_type_get_owns_res_part.attribute_types)
+
+    def get_owns_explicit(self, value_type: AttributeType.ValueType = None, keys_only: bool = False):
+        return (concept_proto_reader.type_(t)
+                for rp in self.stream(
+            thing_type_get_owns_explicit_req(self.get_label(), value_type.proto() if value_type else None, keys_only))
+                for t in rp.thing_type_get_owns_explicit_res_part.attribute_types)
+
+    def get_owns_overridden(self, attribute_type: "AttributeType"):
+        res = self.execute(thing_type_get_owns_overridden_req(
+            self.get_label(), concept_proto_builder.thing_type(attribute_type)
+        )).thing_type_get_owns_overridden_res
+        return concept_proto_reader.attribute_type(res.attribute_type) if res.HasField("attribute_type") else None
```

### Comparing `typedb-client-2.8.0/typedb/concept/type/type.py` & `typedb-client-2.9.0/typedb/concept/type/type.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/client.py` & `typedb-client-2.9.0/typedb/connection/client.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/client.py` & `typedb-client-2.9.0/typedb/connection/cluster/client.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/database.py` & `typedb-client-2.9.0/typedb/connection/cluster/database.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/database_manager.py` & `typedb-client-2.9.0/typedb/connection/cluster/database_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/server_client.py` & `typedb-client-2.9.0/typedb/connection/cluster/server_client.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/session.py` & `typedb-client-2.9.0/typedb/connection/cluster/session.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/stub.py` & `typedb-client-2.9.0/typedb/connection/cluster/stub.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/user.py` & `typedb-client-2.9.0/typedb/connection/cluster/user.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/cluster/user_manager.py` & `typedb-client-2.9.0/typedb/connection/cluster/user_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/core/client.py` & `typedb-client-2.9.0/typedb/connection/core/client.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/core/stub.py` & `typedb-client-2.9.0/typedb/connection/core/stub.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/database.py` & `typedb-client-2.9.0/typedb/connection/database.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/database_manager.py` & `typedb-client-2.9.0/typedb/connection/database_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/session.py` & `typedb-client-2.9.0/typedb/connection/session.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/connection/transaction.py` & `typedb-client-2.9.0/typedb/connection/transaction.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/logic/explanation.py` & `typedb-client-2.9.0/typedb/logic/explanation.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/logic/logic_manager.py` & `typedb-client-2.9.0/typedb/logic/logic_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/logic/rule.py` & `typedb-client-2.9.0/typedb/logic/rule.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/query/query_manager.py` & `typedb-client-2.9.0/typedb/query/query_manager.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/stream/bidirectional_stream.py` & `typedb-client-2.9.0/typedb/stream/bidirectional_stream.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/stream/request_transmitter.py` & `typedb-client-2.9.0/typedb/stream/request_transmitter.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/stream/response_collector.py` & `typedb-client-2.9.0/typedb/stream/response_collector.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb/stream/response_part_iterator.py` & `typedb-client-2.9.0/typedb/stream/response_part_iterator.py`

 * *Files identical despite different names*

### Comparing `typedb-client-2.8.0/typedb_client.egg-info/PKG-INFO` & `typedb-client-2.9.0/typedb_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,15 @@
 Metadata-Version: 2.1
 Name: typedb-client
-Version: 2.8.0
+Version: 2.9.0
 Summary: TypeDB Client for Python
 Home-page: https://github.com/vaticle/typedb-client-python/
 Author: Vaticle
 Author-email: community@vaticle.com
 License: Apache-2.0
-Description: # TypeDB Client for Python
-        
-        [![Grabl](https://grabl.io/api/status/vaticle/typedb-client-python/badge.svg)](https://grabl.io/vaticle/typedb)
-        [![GitHub release](https://img.shields.io/github/release/vaticle/typedb-client-python.svg)](https://github.com/vaticle/typedb/releases/latest)
-        [![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
-        [![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
-        [![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
-        
-        ## Client Architecture
-        To learn about the mechanism that a TypeDB Client uses to set up communication with databases running on the TypeDB Server, refer to [TypeDB > Client API > Overview](http://docs.vaticle.com/docs/client-api/overview).
-        
-        ## API Reference
-        To learn about the methods available for executing queries and retrieving their answers using Client Python, refer to [TypeDB > Client API > Python > API Reference](http://docs.vaticle.com/docs/client-api/python#api-reference).
-        
-        ## Concept API
-        To learn about the methods available on the concepts retrieved as the answers to TypeQL queries, refer to [TypeDB > Concept API > Overview](http://docs.vaticle.com/docs/concept-api/overview)
-        
-        ## Install TypeDB Client for Python through Pip
-        ```
-        pip install typedb-client
-        ```
-        If multiple Python versions are available, you may wish to use
-        ```
-        pip3 install typedb-client
-        ```
-        
-        In your python program, import from typedb.client:
-        ```py
-        from typedb.client import *
-        
-        client = TypeDB.core_client(address=TypeDB.DEFAULT_ADDRESS)
-        ```
-        
 Keywords: typedb database graph knowledgebase knowledge-engineering
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -52,7 +18,43 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
+
+# TypeDB Client for Python
+
+[![Grabl](https://grabl.io/api/status/vaticle/typedb-client-python/badge.svg)](https://grabl.io/vaticle/typedb)
+[![GitHub release](https://img.shields.io/github/release/vaticle/typedb-client-python.svg)](https://github.com/vaticle/typedb/releases/latest)
+[![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://vaticle.com/discord)
+[![Discussion Forum](https://img.shields.io/discourse/https/forum.vaticle.com/topics.svg)](https://forum.vaticle.com)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
+
+## Client Architecture
+To learn about the mechanism that a TypeDB Client uses to set up communication with databases running on the TypeDB Server, refer to [TypeDB > Client API > Overview](http://docs.vaticle.com/docs/client-api/overview).
+
+## API Reference
+To learn about the methods available for executing queries and retrieving their answers using Client Python, refer to [TypeDB > Client API > Python > API Reference](http://docs.vaticle.com/docs/client-api/python#api-reference).
+
+## Concept API
+To learn about the methods available on the concepts retrieved as the answers to TypeQL queries, refer to [TypeDB > Concept API > Overview](http://docs.vaticle.com/docs/concept-api/overview)
+
+## Install TypeDB Client for Python through Pip
+```
+pip install typedb-client
+```
+If multiple Python versions are available, you may wish to use
+```
+pip3 install typedb-client
+```
+
+In your python program, import from typedb.client:
+```py
+from typedb.client import *
+
+client = TypeDB.core_client(address=TypeDB.DEFAULT_ADDRESS)
+```
+
+
```

### Comparing `typedb-client-2.8.0/typedb_client.egg-info/SOURCES.txt` & `typedb-client-2.9.0/typedb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

