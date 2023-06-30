# Comparing `tmp/w3bstream_client_python-0.4.1.tar.gz` & `tmp/w3bstream_client_python-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.4.1.tar", last modified: Fri Jun 30 06:18:02 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.4.2.tar", last modified: Fri Jun 30 06:24:25 2023, max compression
```

## Comparing `w3bstream_client_python-0.4.1.tar` & `w3bstream_client_python-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:18:02.656290 w3bstream_client_python-0.4.1/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-30 06:18:02.656290 w3bstream_client_python-0.4.1/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-30 06:18:02.656290 w3bstream_client_python-0.4.1/setup.cfg
--rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-30 06:17:58.000000 w3bstream_client_python-0.4.1/setup.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:18:02.656290 w3bstream_client_python-0.4.1/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       59 2023-06-30 06:15:46.000000 w3bstream_client_python-0.4.1/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3852 2023-06-30 06:10:51.000000 w3bstream_client_python-0.4.1/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:18:02.656290 w3bstream_client_python-0.4.1/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-30 06:18:02.000000 w3bstream_client_python-0.4.1/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-30 06:18:02.000000 w3bstream_client_python-0.4.1/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-30 06:18:02.000000 w3bstream_client_python-0.4.1/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-30 06:18:02.000000 w3bstream_client_python-0.4.1/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:24:25.025397 w3bstream_client_python-0.4.2/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-30 06:24:25.025397 w3bstream_client_python-0.4.2/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-30 06:24:25.025397 w3bstream_client_python-0.4.2/setup.cfg
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-30 06:24:11.000000 w3bstream_client_python-0.4.2/setup.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:24:25.025397 w3bstream_client_python-0.4.2/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-06-30 06:23:43.000000 w3bstream_client_python-0.4.2/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3852 2023-06-30 06:10:51.000000 w3bstream_client_python-0.4.2/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:24:25.025397 w3bstream_client_python-0.4.2/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-30 06:24:25.000000 w3bstream_client_python-0.4.2/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-30 06:24:25.000000 w3bstream_client_python-0.4.2/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-30 06:24:25.000000 w3bstream_client_python-0.4.2/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-30 06:24:25.000000 w3bstream_client_python-0.4.2/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-0.4.1/w3bstream_client_python/client.py` & `w3bstream_client_python-0.4.2/w3bstream_client_python/client.py`

 * *Files identical despite different names*

