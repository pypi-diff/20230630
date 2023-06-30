# Comparing `tmp/genagg-0.0.3.tar.gz` & `tmp/genagg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genagg-0.0.3.tar", last modified: Tue Nov 30 18:45:33 2021, max compression
+gzip compressed data, was "genagg-1.0.0.tar", last modified: Fri Jun 30 14:42:18 2023, max compression
```

## Comparing `genagg-0.0.3.tar` & `genagg-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2021-11-30 18:45:33.702762 genagg-0.0.3/
--rw-r--r--   0 smorad     (501) staff       (20)      221 2021-11-30 18:45:33.702653 genagg-0.0.3/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     1957 2021-11-29 18:32:07.000000 genagg-0.0.3/README.md
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2021-11-30 18:45:33.702061 genagg-0.0.3/genagg/
--rw-r--r--   0 smorad     (501) staff       (20)     3079 2021-11-30 18:21:38.000000 genagg-0.0.3/genagg/AggGNN.py
--rw-r--r--   0 smorad     (501) staff       (20)     3703 2021-11-30 17:37:30.000000 genagg-0.0.3/genagg/GenAgg.py
--rw-r--r--   0 smorad     (501) staff       (20)     4618 2021-11-30 18:43:14.000000 genagg-0.0.3/genagg/GenAggSparse.py
--rw-r--r--   0 smorad     (501) staff       (20)     1396 2021-11-29 18:32:07.000000 genagg-0.0.3/genagg/MLP.py
--rw-r--r--   0 smorad     (501) staff       (20)      246 2021-11-29 18:32:07.000000 genagg-0.0.3/genagg/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2021-11-30 18:45:33.702534 genagg-0.0.3/genagg.egg-info/
--rw-r--r--   0 smorad     (501) staff       (20)      221 2021-11-30 18:45:33.000000 genagg-0.0.3/genagg.egg-info/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)      257 2021-11-30 18:45:33.000000 genagg-0.0.3/genagg.egg-info/SOURCES.txt
--rw-r--r--   0 smorad     (501) staff       (20)        1 2021-11-30 18:45:33.000000 genagg-0.0.3/genagg.egg-info/dependency_links.txt
--rw-r--r--   0 smorad     (501) staff       (20)       20 2021-11-30 18:45:33.000000 genagg-0.0.3/genagg.egg-info/requires.txt
--rw-r--r--   0 smorad     (501) staff       (20)        7 2021-11-30 18:45:33.000000 genagg-0.0.3/genagg.egg-info/top_level.txt
--rw-r--r--   0 smorad     (501) staff       (20)       38 2021-11-30 18:45:33.702794 genagg-0.0.3/setup.cfg
--rw-r--r--   0 smorad     (501) staff       (20)      344 2021-11-30 18:44:38.000000 genagg-0.0.3/setup.py
+drwxr-xr-x   0 ryko       (501) staff       (20)        0 2023-06-30 14:42:18.106290 genagg-1.0.0/
+-rw-r--r--   0 ryko       (501) staff       (20)      127 2023-06-30 14:42:18.106186 genagg-1.0.0/PKG-INFO
+drwxr-xr-x   0 ryko       (501) staff       (20)        0 2023-06-30 14:42:18.105397 genagg-1.0.0/genagg/
+-rw-r--r--   0 ryko       (501) staff       (20)       55 2022-11-22 16:48:21.000000 genagg-1.0.0/genagg/__init__.py
+-rw-r--r--   0 ryko       (501) staff       (20)     2135 2023-05-16 15:06:56.000000 genagg-1.0.0/genagg/genagg.py
+-rw-r--r--   0 ryko       (501) staff       (20)     2783 2023-05-16 15:07:49.000000 genagg-1.0.0/genagg/mlp_forrev.py
+drwxr-xr-x   0 ryko       (501) staff       (20)        0 2023-06-30 14:42:18.106025 genagg-1.0.0/genagg.egg-info/
+-rw-r--r--   0 ryko       (501) staff       (20)      127 2023-06-30 14:42:18.000000 genagg-1.0.0/genagg.egg-info/PKG-INFO
+-rw-r--r--   0 ryko       (501) staff       (20)      214 2023-06-30 14:42:18.000000 genagg-1.0.0/genagg.egg-info/SOURCES.txt
+-rw-r--r--   0 ryko       (501) staff       (20)        1 2023-06-30 14:42:18.000000 genagg-1.0.0/genagg.egg-info/dependency_links.txt
+-rw-r--r--   0 ryko       (501) staff       (20)       53 2023-06-30 14:42:18.000000 genagg-1.0.0/genagg.egg-info/requires.txt
+-rw-r--r--   0 ryko       (501) staff       (20)        7 2023-06-30 14:42:18.000000 genagg-1.0.0/genagg.egg-info/top_level.txt
+-rw-r--r--   0 ryko       (501) staff       (20)       38 2023-06-30 14:42:18.106327 genagg-1.0.0/setup.cfg
+-rw-r--r--   0 ryko       (501) staff       (20)      333 2023-06-30 14:38:15.000000 genagg-1.0.0/setup.py
```

