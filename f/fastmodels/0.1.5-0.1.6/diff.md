# Comparing `tmp/fastmodels-0.1.5.tar.gz` & `tmp/fastmodels-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmodels-0.1.5.tar", last modified: Thu Jun 15 10:30:58 2023, max compression
+gzip compressed data, was "fastmodels-0.1.6.tar", last modified: Fri Jun 30 08:04:16 2023, max compression
```

## Comparing `fastmodels-0.1.5.tar` & `fastmodels-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 10:30:58.637375 fastmodels-0.1.5/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      141 2023-06-15 10:30:58.637375 fastmodels-0.1.5/PKG-INFO
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      623 2023-06-15 10:21:31.000000 fastmodels-0.1.5/README.md
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 10:30:58.633378 fastmodels-0.1.5/fastmodels/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:19:35.000000 fastmodels-0.1.5/fastmodels/__init__.py
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      484 2023-06-15 10:29:23.000000 fastmodels-0.1.5/fastmodels/cli.py
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 10:30:58.637375 fastmodels-0.1.5/fastmodels/datavalidator/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:01:48.000000 fastmodels-0.1.5/fastmodels/datavalidator/__init__.py
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      979 2023-06-15 09:05:15.000000 fastmodels-0.1.5/fastmodels/datavalidator/validator.py
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 10:30:58.637375 fastmodels-0.1.5/fastmodels/tests/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:17:25.000000 fastmodels-0.1.5/fastmodels/tests/__init__.py
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      649 2023-06-15 09:20:20.000000 fastmodels-0.1.5/fastmodels/tests/test_validator.py
-drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 10:30:58.633378 fastmodels-0.1.5/fastmodels.egg-info/
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      141 2023-06-15 10:30:58.000000 fastmodels-0.1.5/fastmodels.egg-info/PKG-INFO
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      404 2023-06-15 10:30:58.000000 fastmodels-0.1.5/fastmodels.egg-info/SOURCES.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        1 2023-06-15 10:30:58.000000 fastmodels-0.1.5/fastmodels.egg-info/dependency_links.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       51 2023-06-15 10:30:58.000000 fastmodels-0.1.5/fastmodels.egg-info/entry_points.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       11 2023-06-15 10:30:58.000000 fastmodels-0.1.5/fastmodels.egg-info/requires.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       11 2023-06-15 10:30:58.000000 fastmodels-0.1.5/fastmodels.egg-info/top_level.txt
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       38 2023-06-15 10:30:58.637375 fastmodels-0.1.5/setup.cfg
--rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      389 2023-06-15 10:30:07.000000 fastmodels-0.1.5/setup.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-30 08:04:16.535632 fastmodels-0.1.6/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      141 2023-06-30 08:04:16.535632 fastmodels-0.1.6/PKG-INFO
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      623 2023-06-15 10:21:31.000000 fastmodels-0.1.6/README.md
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-30 08:04:16.535632 fastmodels-0.1.6/fastmodels/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:19:35.000000 fastmodels-0.1.6/fastmodels/__init__.py
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)     1083 2023-06-30 08:02:27.000000 fastmodels-0.1.6/fastmodels/cli.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-30 08:04:16.535632 fastmodels-0.1.6/fastmodels/datavalidator/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:01:48.000000 fastmodels-0.1.6/fastmodels/datavalidator/__init__.py
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)     1672 2023-06-30 07:36:28.000000 fastmodels-0.1.6/fastmodels/datavalidator/validator.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-30 08:04:16.535632 fastmodels-0.1.6/fastmodels/tests/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        0 2023-06-15 09:17:25.000000 fastmodels-0.1.6/fastmodels/tests/__init__.py
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      649 2023-06-15 09:20:20.000000 fastmodels-0.1.6/fastmodels/tests/test_validator.py
+drwxrwxr-x   0 zandersun  (1000) zandersun  (1000)        0 2023-06-30 08:04:16.535632 fastmodels-0.1.6/fastmodels.egg-info/
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      141 2023-06-30 08:04:16.000000 fastmodels-0.1.6/fastmodels.egg-info/PKG-INFO
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      404 2023-06-30 08:04:16.000000 fastmodels-0.1.6/fastmodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)        1 2023-06-30 08:04:16.000000 fastmodels-0.1.6/fastmodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       51 2023-06-30 08:04:16.000000 fastmodels-0.1.6/fastmodels.egg-info/entry_points.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       11 2023-06-30 08:04:16.000000 fastmodels-0.1.6/fastmodels.egg-info/requires.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       11 2023-06-30 08:04:16.000000 fastmodels-0.1.6/fastmodels.egg-info/top_level.txt
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)       38 2023-06-30 08:04:16.535632 fastmodels-0.1.6/setup.cfg
+-rw-rw-r--   0 zandersun  (1000) zandersun  (1000)      389 2023-06-30 07:28:02.000000 fastmodels-0.1.6/setup.py
```

### Comparing `fastmodels-0.1.5/README.md` & `fastmodels-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fastmodels-0.1.5/fastmodels/tests/test_validator.py` & `fastmodels-0.1.6/fastmodels/tests/test_validator.py`

 * *Files identical despite different names*

