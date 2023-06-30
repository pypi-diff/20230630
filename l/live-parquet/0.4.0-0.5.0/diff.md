# Comparing `tmp/live_parquet-0.4.0.tar.gz` & `tmp/live_parquet-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/live_parquet-0.4.0.tar", last modified: Fri Jun 30 12:54:47 2023, max compression
+gzip compressed data, was "live_parquet-0.5.0.tar", last modified: Fri Jun 30 13:24:32 2023, max compression
```

## Comparing `live_parquet-0.4.0.tar` & `live_parquet-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 12:54:47.217369 live_parquet-0.4.0/
--rw-r--r--   0 sultanfaisal   (502) staff       (20)     1030 2023-06-30 12:54:47.217232 live_parquet-0.4.0/PKG-INFO
--rw-r--r--   0 sultanfaisal   (502) staff       (20)      296 2023-06-29 15:51:54.000000 live_parquet-0.4.0/README.md
-drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 12:54:47.217028 live_parquet-0.4.0/live_parquet.egg-info/
--rw-r--r--   0 sultanfaisal   (502) staff       (20)     1030 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/PKG-INFO
--rw-r--r--   0 sultanfaisal   (502) staff       (20)      236 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/SOURCES.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/dependency_links.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)       65 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/entry_points.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)       51 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/requires.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-30 12:54:47.000000 live_parquet-0.4.0/live_parquet.egg-info/top_level.txt
--rw-r--r--   0 sultanfaisal   (502) staff       (20)       38 2023-06-30 12:54:47.217414 live_parquet-0.4.0/setup.cfg
--rw-r--r--   0 sultanfaisal   (502) staff       (20)     1093 2023-06-30 12:54:42.000000 live_parquet-0.4.0/setup.py
+drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 13:24:32.099110 live_parquet-0.5.0/
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       56 2023-06-30 13:24:32.099151 live_parquet-0.5.0/PKG-INFO
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)      296 2023-06-29 15:51:54.000000 live_parquet-0.5.0/README.md
+drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 13:24:32.098243 live_parquet-0.5.0/live_parquet/
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 13:15:54.000000 live_parquet-0.5.0/live_parquet/__init__.py
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)     1296 2023-06-29 14:57:13.000000 live_parquet-0.5.0/live_parquet/live_parquet_module.py
+drwxr-xr-x   0 sultanfaisal   (502) staff       (20)        0 2023-06-30 13:24:32.098992 live_parquet-0.5.0/live_parquet.egg-info/
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       56 2023-06-30 13:24:32.000000 live_parquet-0.5.0/live_parquet.egg-info/PKG-INFO
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)      307 2023-06-30 13:24:32.000000 live_parquet-0.5.0/live_parquet.egg-info/SOURCES.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)        1 2023-06-30 13:24:32.000000 live_parquet-0.5.0/live_parquet.egg-info/dependency_links.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       79 2023-06-30 13:24:32.000000 live_parquet-0.5.0/live_parquet.egg-info/entry_points.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       31 2023-06-30 13:24:32.000000 live_parquet-0.5.0/live_parquet.egg-info/requires.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       13 2023-06-30 13:24:32.000000 live_parquet-0.5.0/live_parquet.egg-info/top_level.txt
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)      281 2023-06-30 13:24:32.099348 live_parquet-0.5.0/setup.cfg
+-rw-r--r--   0 sultanfaisal   (502) staff       (20)       37 2023-06-30 13:18:05.000000 live_parquet-0.5.0/setup.py
```

