# Comparing `tmp/w3bstream_client_python-0.3.0.tar.gz` & `tmp/w3bstream_client_python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.3.0.tar", last modified: Sat Jun 24 07:21:10 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.4.0.tar", last modified: Fri Jun 30 06:13:05 2023, max compression
```

## Comparing `w3bstream_client_python-0.3.0.tar` & `w3bstream_client_python-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/setup.cfg
--rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-24 07:21:04.000000 w3bstream_client_python-0.3.0/setup.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 07:21:10.666302 w3bstream_client_python-0.3.0/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       49 2023-06-24 01:11:11.000000 w3bstream_client_python-0.3.0/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     1190 2023-06-24 07:19:44.000000 w3bstream_client_python-0.3.0/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 07:21:10.676302 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-24 07:21:10.000000 w3bstream_client_python-0.3.0/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:13:05.658678 w3bstream_client_python-0.4.0/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-30 06:13:05.658678 w3bstream_client_python-0.4.0/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-30 06:13:05.658678 w3bstream_client_python-0.4.0/setup.cfg
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-30 06:12:33.000000 w3bstream_client_python-0.4.0/setup.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:13:05.658678 w3bstream_client_python-0.4.0/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       49 2023-06-24 01:11:11.000000 w3bstream_client_python-0.4.0/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3852 2023-06-30 06:10:51.000000 w3bstream_client_python-0.4.0/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-30 06:13:05.658678 w3bstream_client_python-0.4.0/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-30 06:13:05.000000 w3bstream_client_python-0.4.0/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-30 06:13:05.000000 w3bstream_client_python-0.4.0/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-30 06:13:05.000000 w3bstream_client_python-0.4.0/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-30 06:13:05.000000 w3bstream_client_python-0.4.0/w3bstream_client_python.egg-info/top_level.txt
```

