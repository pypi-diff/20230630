# Comparing `tmp/aibabyllmclient-1.0.tar.gz` & `tmp/aibabyllmclient-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibabyllmclient-1.0.tar", last modified: Fri Jun 30 01:37:19 2023, max compression
+gzip compressed data, was "aibabyllmclient-1.1.tar", last modified: Fri Jun 30 02:17:50 2023, max compression
```

## Comparing `aibabyllmclient-1.0.tar` & `aibabyllmclient-1.1.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 01:37:19.922679 aibabyllmclient-1.0/
--rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 01:37:19.922679 aibabyllmclient-1.0/PKG-INFO
-drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 01:37:19.922679 aibabyllmclient-1.0/aibabyllmclient.egg-info/
--rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 01:37:19.000000 aibabyllmclient-1.0/aibabyllmclient.egg-info/PKG-INFO
--rw-rw-r--   0 zh        (1000) zh        (1000)      164 2023-06-30 01:37:19.000000 aibabyllmclient-1.0/aibabyllmclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 01:37:19.000000 aibabyllmclient-1.0/aibabyllmclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 01:37:19.000000 aibabyllmclient-1.0/aibabyllmclient.egg-info/top_level.txt
--rw-rw-r--   0 zh        (1000) zh        (1000)       38 2023-06-30 01:37:19.922679 aibabyllmclient-1.0/setup.cfg
--rw-rw-r--   0 zh        (1000) zh        (1000)      319 2023-06-30 01:33:30.000000 aibabyllmclient-1.0/setup.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:17:50.867912 aibabyllmclient-1.1/
+-rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:17:50.867912 aibabyllmclient-1.1/PKG-INFO
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:17:50.867912 aibabyllmclient-1.1/aibabyllmclient/
+-rw-rw-r--   0 zh        (1000) zh        (1000)        0 2023-06-30 02:14:45.000000 aibabyllmclient-1.1/aibabyllmclient/__init__.py
+-rw-rw-r--   0 zh        (1000) zh        (1000)     3300 2023-06-30 01:35:46.000000 aibabyllmclient-1.1/aibabyllmclient/llmserver_call.py
+-rw-rw-r--   0 zh        (1000) zh        (1000)      603 2023-06-30 01:36:24.000000 aibabyllmclient-1.1/aibabyllmclient/main.py
+drwxrwxr-x   0 zh        (1000) zh        (1000)        0 2023-06-30 02:17:50.867912 aibabyllmclient-1.1/aibabyllmclient.egg-info/
+-rw-rw-r--   0 zh        (1000) zh        (1000)      131 2023-06-30 02:17:50.000000 aibabyllmclient-1.1/aibabyllmclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zh        (1000) zh        (1000)      250 2023-06-30 02:17:50.000000 aibabyllmclient-1.1/aibabyllmclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)        1 2023-06-30 02:17:50.000000 aibabyllmclient-1.1/aibabyllmclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)       16 2023-06-30 02:17:50.000000 aibabyllmclient-1.1/aibabyllmclient.egg-info/top_level.txt
+-rw-rw-r--   0 zh        (1000) zh        (1000)       38 2023-06-30 02:17:50.867912 aibabyllmclient-1.1/setup.cfg
+-rw-rw-r--   0 zh        (1000) zh        (1000)      319 2023-06-30 02:16:53.000000 aibabyllmclient-1.1/setup.py
```

