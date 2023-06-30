# Comparing `tmp/runtimepy-1.7.0.tar.gz` & `tmp/runtimepy-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.7.0.tar", last modified: Mon Jun 26 08:30:41 2023, max compression
+gzip compressed data, was "runtimepy-1.7.1.tar", last modified: Fri Jun 30 00:24:55 2023, max compression
```

## Comparing `runtimepy-1.7.0.tar` & `runtimepy-1.7.1.tar`

### file list

```diff
@@ -1,148 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 08:29:19.000000 runtimepy-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 08:30:41.862507 runtimepy-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-26 08:29:19.000000 runtimepy-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 08:29:19.000000 runtimepy-1.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.850507 runtimepy-1.7.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.850507 runtimepy-1.7.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.846507 runtimepy-1.7.0/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/factory/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.850507 runtimepy-1.7.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:30:41.862507 runtimepy-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 08:29:19.000000 runtimepy-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 08:29:19.000000 runtimepy-1.7.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 08:29:19.000000 runtimepy-1.7.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 08:29:19.000000 runtimepy-1.7.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.655786 runtimepy-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 00:23:11.000000 runtimepy-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-30 00:24:55.655786 runtimepy-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 00:23:11.000000 runtimepy-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-30 00:23:11.000000 runtimepy-1.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.635786 runtimepy-1.7.1/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.635786 runtimepy-1.7.1/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.639786 runtimepy-1.7.1/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.639786 runtimepy-1.7.1/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.639786 runtimepy-1.7.1/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.639786 runtimepy-1.7.1/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.631786 runtimepy-1.7.1/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.639786 runtimepy-1.7.1/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/housekeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.643786 runtimepy-1.7.1/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.647786 runtimepy-1.7.1/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/task/basic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/task/basic/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 00:23:11.000000 runtimepy-1.7.1/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.635786 runtimepy-1.7.1/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-30 00:24:55.000000 runtimepy-1.7.1/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-30 00:24:55.000000 runtimepy-1.7.1/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:24:55.000000 runtimepy-1.7.1/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 00:24:55.000000 runtimepy-1.7.1/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 00:24:55.000000 runtimepy-1.7.1/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 00:24:55.000000 runtimepy-1.7.1/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 00:24:55.655786 runtimepy-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-30 00:23:11.000000 runtimepy-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:24:55.651786 runtimepy-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 00:23:11.000000 runtimepy-1.7.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 00:23:11.000000 runtimepy-1.7.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 00:23:11.000000 runtimepy-1.7.1/tests/test_resources.py
```

### Comparing `runtimepy-1.7.0/LICENSE` & `runtimepy-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/PKG-INFO` & `runtimepy-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.7.0
+Version: 1.7.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6a3f7b1658909aed705809485a62426b
+    hash=c18860c7914c78fabefbae5f111993f1
     =====================================
 -->
 
-# runtimepy ([1.7.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.7.0/README.md` & `runtimepy-1.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6a3f7b1658909aed705809485a62426b
+    hash=c18860c7914c78fabefbae5f111993f1
     =====================================
 -->
 
-# runtimepy ([1.7.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.7.0/pyproject.toml` & `runtimepy-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.7.0"
+version = "1.7.1"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.7.0/runtimepy/app.py` & `runtimepy-1.7.1/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/__init__.py` & `runtimepy-1.7.1/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/environment/__init__.py` & `runtimepy-1.7.1/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/environment/array.py` & `runtimepy-1.7.1/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/environment/base.py` & `runtimepy-1.7.1/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/environment/create.py` & `runtimepy-1.7.1/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/environment/file.py` & `runtimepy-1.7.1/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/environment/names.py` & `runtimepy-1.7.1/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/channel/registry.py` & `runtimepy-1.7.1/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/codec/protocol/base.py` & `runtimepy-1.7.1/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/codec/protocol/json.py` & `runtimepy-1.7.1/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/commands/all.py` & `runtimepy-1.7.1/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/commands/arbiter.py` & `runtimepy-1.7.1/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/commands/tui.py` & `runtimepy-1.7.1/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.7.1/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.7.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/entry.py` & `runtimepy-1.7.1/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/enum/__init__.py` & `runtimepy-1.7.1/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/enum/registry.py` & `runtimepy-1.7.1/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/enum/type.py` & `runtimepy-1.7.1/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/mapping.py` & `runtimepy-1.7.1/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/mixins/enum.py` & `runtimepy-1.7.1/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/mixins/regex.py` & `runtimepy-1.7.1/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/__init__.py` & `runtimepy-1.7.1/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/__init__.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/base.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.logging import LoggerMixin as _LoggerMixin
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 from vcorelib.namespace import NamespaceMixin as _NamespaceMixin
 
 # internal
+from runtimepy.net.arbiter.housekeeping import metrics_poller
 from runtimepy.net.arbiter.info import AppInfo, ConnectionMap
 from runtimepy.net.arbiter.task import (
     ArbiterTaskManager as _ArbiterTaskManager,
 )
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 
@@ -76,14 +77,17 @@
 
         if manager is None:
             manager = _ConnectionManager()
         self.manager = manager
 
         self.task_manager = _ArbiterTaskManager()
 
+        # Ensure that connection metrics are polled.
+        self.task_manager.register(metrics_poller(self.manager))
+
         if stop_sig is None:
             stop_sig = _asyncio.Event()
         self.stop_sig = stop_sig
 
         _NamespaceMixin.__init__(self, namespace=namespace)
 
         # A fallback application. Set a class attribute so this can be more
```

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/config.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/config.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/factory/task.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/imports.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/info.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/task.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/udp.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.7.1/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/connection.py` & `runtimepy-1.7.1/runtimepy/net/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,14 @@
         self.metrics = ConnectionMetrics()
 
         self._tasks: _List[_asyncio.Task[None]] = []
         self.initialized = _asyncio.Event()
         self.disabled_event = _asyncio.Event()
         self.init()
 
-    def reset_metrics(self) -> None:
-        """Reset connection metrics."""
-        self.metrics.tx.reset()
-        self.metrics.rx.reset()
-
     def init(self) -> None:
         """Initialize this instance."""
 
     async def async_init(self) -> bool:
         """A runtime initialization routine (executes during 'process')."""
         return True
```

### Comparing `runtimepy-1.7.0/runtimepy/net/factories/__init__.py` & `runtimepy-1.7.1/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/manager.py` & `runtimepy-1.7.1/runtimepy/net/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,61 @@
 # built-in
 import asyncio as _asyncio
 from typing import List as _List
 from typing import Optional as _Optional
 
 # third-party
 from vcorelib.asyncio import log_exceptions as _log_exceptions
+from vcorelib.math import default_time_ns as _default_time_ns
 
 # internal
 from runtimepy.net.connection import Connection as _Connection
 
 
 class ConnectionManager:
     """A class for managing connection processing at runtime."""
 
     def __init__(self) -> None:
         """Initialize this connection manager."""
         self.queue: _asyncio.Queue[_Connection] = _asyncio.Queue()
         self._running = False
+        self._conns: _List[_Connection] = []
+
+    @property
+    def num_connections(self) -> int:
+        """Return the number of managed connections."""
+        return len(self._conns)
+
+    def reset_metrics(self) -> None:
+        """Reset connection metrics."""
+        for conn in self._conns:
+            conn.metrics.reset()
+
+    def poll_metrics(self, time_ns: int = None) -> None:
+        """Poll connection metrics."""
+
+        if time_ns is None:
+            time_ns = _default_time_ns()
+
+        for conn in self._conns:
+            conn.metrics.poll(time_ns=time_ns)
 
     async def manage(self, stop_sig: _asyncio.Event) -> None:
         """Handle incoming connections until the stop signal is set."""
 
         # Allow this method to be reentrant.
         if self._running:
             await stop_sig.wait()
             return
 
         self._running = True
 
         stop_sig_task = _asyncio.create_task(stop_sig.wait())
         tasks: _List[_asyncio.Task[None]] = []
-        conns: _List[_Connection] = []
+        self._conns = []
         new_conn_task: _Optional[_asyncio.Task[_Connection]] = None
 
         while not stop_sig.is_set():
             # Create a new-connection handler.
             if new_conn_task is None:
                 # Wait for a connection to be established.
                 new_conn_task = _asyncio.create_task(self.queue.get())
@@ -51,21 +72,21 @@
                 return_when=_asyncio.FIRST_COMPLETED,
             )
 
             # Filter completed tasks out of the working set.
             next_tasks = _log_exceptions(tasks)
 
             # Filter out disabled connections.
-            conns = [x for x in conns if not x.disabled]
+            self._conns = [x for x in self._conns if not x.disabled]
 
             # If a new connection was made, register a task for processing
             # it.
             if new_conn_task.done():
                 new_conn = new_conn_task.result()
-                conns.append(new_conn)
+                self._conns.append(new_conn)
                 next_tasks.append(
                     _asyncio.create_task(new_conn.process(stop_sig=stop_sig))
                 )
                 new_conn_task = None
 
             # If the stop signal was sent, cancel existing connections.
             if stop_sig.is_set():
```

### Comparing `runtimepy-1.7.0/runtimepy/net/metrics.py` & `runtimepy-1.7.1/runtimepy/net/metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,77 @@
 """
 A module implementing a connection-metrics structure.
 """
 
 # third-party
-from vcorelib.math import RateTracker
+from vcorelib.math import RateTracker as _RateTracker
 
 # internal
 from runtimepy.primitives import Float as _Float
 from runtimepy.primitives import Uint32 as _Uint32
 from runtimepy.primitives import Uint64 as _Uint64
 
+METRICS_DEPTH = 50
+
 
 class ChannelMetrics:
     """Metrics for a network channel."""
 
     def __init__(self) -> None:
         """Initialize this instance."""
 
         self.messages = _Uint32()
+        self.message_rate = _Float()
+        self._message_rate_tracker = _RateTracker(depth=METRICS_DEPTH)
+
         self.bytes = _Uint64()
         self.kbps = _Float()
-        self._kbps_tracker = RateTracker()
-        self.stale = True
+        self._kbps_tracker = _RateTracker(depth=METRICS_DEPTH)
+
+    def poll(self, time_ns: int = None) -> None:
+        """Poll kbps tracking."""
+
+        self.kbps.raw.value = self._kbps_tracker.poll(time_ns=time_ns)
+        self.message_rate.raw.value = self._message_rate_tracker.poll(
+            time_ns=time_ns
+        )
 
     def increment(self, count: int, time_ns: int = None) -> None:
         """Update tracking."""
 
+        self.messages.raw.value += 1
+        self.message_rate.raw.value = self._message_rate_tracker(
+            time_ns=time_ns
+        )
+
         self.bytes.raw.value += count
-        self._kbps_tracker(time_ns=time_ns, value=float(count))
-        self.stale = False
+        self.kbps.raw.value = self._kbps_tracker(
+            time_ns=time_ns, value=float(count) / 1000.0
+        )
 
     def reset(self) -> None:
         """Reset metrics."""
 
         self.messages.raw.value = 0
         self.bytes.raw.value = 0
         self.kbps.raw.value = 0.0
         self._kbps_tracker()
-        self.stale = True
 
 
 class ConnectionMetrics:
     """Metrics for a network connection."""
 
     def __init__(self) -> None:
         """Initialize this instance."""
 
         self.tx = ChannelMetrics()
         self.rx = ChannelMetrics()
+
+    def reset(self) -> None:
+        """Reset metrics."""
+        self.tx.reset()
+        self.rx.reset()
+
+    def poll(self, time_ns: int = None) -> None:
+        """Poll channels."""
+        self.tx.poll(time_ns=time_ns)
+        self.rx.poll(time_ns=time_ns)
```

### Comparing `runtimepy-1.7.0/runtimepy/net/mixin.py` & `runtimepy-1.7.1/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/tcp/connection.py` & `runtimepy-1.7.1/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.7.1/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.7.1/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/udp/connection.py` & `runtimepy-1.7.1/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/util.py` & `runtimepy-1.7.1/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/net/websocket/connection.py` & `runtimepy-1.7.1/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/__init__.py` & `runtimepy-1.7.1/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/array.py` & `runtimepy-1.7.1/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/base.py` & `runtimepy-1.7.1/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/bool.py` & `runtimepy-1.7.1/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/byte_order.py` & `runtimepy-1.7.1/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/field/__init__.py` & `runtimepy-1.7.1/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/field/fields.py` & `runtimepy-1.7.1/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.7.1/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.7.1/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/float.py` & `runtimepy-1.7.1/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/int.py` & `runtimepy-1.7.1/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/string.py` & `runtimepy-1.7.1/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/type/__init__.py` & `runtimepy-1.7.1/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/type/base.py` & `runtimepy-1.7.1/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/type/float.py` & `runtimepy-1.7.1/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/primitives/type/int.py` & `runtimepy-1.7.1/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/registry/__init__.py` & `runtimepy-1.7.1/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/registry/bool.py` & `runtimepy-1.7.1/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/registry/item.py` & `runtimepy-1.7.1/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/registry/name.py` & `runtimepy-1.7.1/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/schemas.py` & `runtimepy-1.7.1/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/task/asynchronous.py` & `runtimepy-1.7.1/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/task/basic/manager.py` & `runtimepy-1.7.1/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/task/basic/metrics.py` & `runtimepy-1.7.1/runtimepy/task/basic/metrics.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/task/basic/periodic.py` & `runtimepy-1.7.1/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/tui/channels/__init__.py` & `runtimepy-1.7.1/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy/tui/task.py` & `runtimepy-1.7.1/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.7.1/runtimepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.7.0
+Version: 1.7.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=6a3f7b1658909aed705809485a62426b
+    hash=c18860c7914c78fabefbae5f111993f1
     =====================================
 -->
 
-# runtimepy ([1.7.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.7.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.7.1/runtimepy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 runtimepy/net/arbiter/task.py
 runtimepy/net/arbiter/tcp.py
 runtimepy/net/arbiter/udp.py
 runtimepy/net/arbiter/websocket.py
 runtimepy/net/arbiter/factory/__init__.py
 runtimepy/net/arbiter/factory/connection.py
 runtimepy/net/arbiter/factory/task.py
+runtimepy/net/arbiter/housekeeping/__init__.py
 runtimepy/net/factories/__init__.py
 runtimepy/net/tcp/__init__.py
 runtimepy/net/tcp/connection.py
 runtimepy/net/tcp/telnet/__init__.py
 runtimepy/net/tcp/telnet/codes.py
 runtimepy/net/udp/__init__.py
 runtimepy/net/udp/connection.py
```

### Comparing `runtimepy-1.7.0/setup.py` & `runtimepy-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/tests/test_entry.py` & `runtimepy-1.7.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.7.0/tests/test_mapping.py` & `runtimepy-1.7.1/tests/test_mapping.py`

 * *Files identical despite different names*

