# Comparing `tmp/kdslibs-0.0.8.tar.gz` & `tmp/kdslibs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdslibs-0.0.8.tar", last modified: Mon Jun 12 16:25:55 2023, max compression
+gzip compressed data, was "kdslibs-0.0.9.tar", last modified: Sun Jun 25 17:36:51 2023, max compression
```

## Comparing `kdslibs-0.0.8.tar` & `kdslibs-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-12 16:25:55.941564 kdslibs-0.0.8/
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.8/LICENSE
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-12 16:25:55.941564 kdslibs-0.0.8/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.8/README.md
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-12 16:25:55.941564 kdslibs-0.0.8/kdslibs/
--rw-r--r--   0 diwa      (1000) diwa      (1000)     1531 2023-06-12 16:20:05.000000 kdslibs-0.0.8/kdslibs/__init__.py
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-12 16:25:55.941564 kdslibs-0.0.8/kdslibs.egg-info/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/SOURCES.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/dependency_links.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/top_level.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-12 16:25:55.941564 kdslibs-0.0.8/setup.cfg
--rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-12 16:25:49.000000 kdslibs-0.0.8/setup.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-25 17:36:51.609633 kdslibs-0.0.9/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.9/LICENSE
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      295 2023-06-25 17:36:51.609633 kdslibs-0.0.9/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.9/README.md
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-25 17:36:51.609633 kdslibs-0.0.9/kdslibs/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)     2032 2023-06-25 17:34:25.000000 kdslibs-0.0.9/kdslibs/__init__.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-25 17:36:51.609633 kdslibs-0.0.9/kdslibs.egg-info/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      295 2023-06-25 17:36:51.000000 kdslibs-0.0.9/kdslibs.egg-info/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-25 17:36:51.000000 kdslibs-0.0.9/kdslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-25 17:36:51.000000 kdslibs-0.0.9/kdslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-25 17:36:51.000000 kdslibs-0.0.9/kdslibs.egg-info/top_level.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-25 17:36:51.609633 kdslibs-0.0.9/setup.cfg
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      429 2023-06-25 17:36:47.000000 kdslibs-0.0.9/setup.py
```

