# Comparing `tmp/server-roberta-0.0.4.tar.gz` & `tmp/server-roberta-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server-roberta-0.0.4.tar", last modified: Thu Jun  1 01:46:35 2023, max compression
+gzip compressed data, was "server-roberta-0.4.3.tar", last modified: Fri Jun 30 19:03:54 2023, max compression
```

## Comparing `server-roberta-0.0.4.tar` & `server-roberta-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.909309 server-roberta-0.0.4/
--rw-rw-rw-   0        0        0    11404 2022-09-13 09:02:44.000000 server-roberta-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2479 2023-06-01 01:46:35.898034 server-roberta-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1873 2022-09-13 09:02:44.000000 server-roberta-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.877088 server-roberta-0.0.4/py/
-drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.888068 server-roberta-0.0.4/py/serverRoberta/
--rw-rw-rw-   0        0        0      112 2023-06-01 01:41:50.000000 server-roberta-0.0.4/py/serverRoberta/__init__.py
--rw-rw-rw-   0        0        0      108 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/datos.py
--rw-rw-rw-   0        0        0     2987 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/encrypt.py
--rw-rw-rw-   0        0        0     4021 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/robertaModel.py
--rw-rw-rw-   0        0        0     3692 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/server.py
--rw-rw-rw-   0        0        0      801 2023-06-01 01:45:40.000000 server-roberta-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.897037 server-roberta-0.0.4/server_roberta.egg-info/
--rw-rw-rw-   0        0        0     2479 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 01:46:35.909309 server-roberta-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:03:54.959348 server-roberta-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 19:03:54.959348 server-roberta-0.4.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:03:54.959348 server-roberta-0.4.3/serverRoberta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/datos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/robertaModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/roberta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/roberta_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-30 19:02:17.000000 server-roberta-0.4.3/serverRoberta/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:03:54.959348 server-roberta-0.4.3/server_roberta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 19:03:54.000000 server-roberta-0.4.3/server_roberta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:03:54.959348 server-roberta-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-30 19:02:17.000000 server-roberta-0.4.3/setup.py
```

### Comparing `server-roberta-0.0.4/py/serverRoberta/encrypt.py` & `server-roberta-0.4.3/serverRoberta/encrypt.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.4/py/serverRoberta/robertaModel.py` & `server-roberta-0.4.3/serverRoberta/robertaModel.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.4/py/serverRoberta/server.py` & `server-roberta-0.4.3/serverRoberta/server.py`

 * *Files identical despite different names*

