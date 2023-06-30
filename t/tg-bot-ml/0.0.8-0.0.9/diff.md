# Comparing `tmp/tg_bot_ml-0.0.8.tar.gz` & `tmp/tg_bot_ml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_bot_ml-0.0.8.tar", last modified: Thu Jun 22 08:06:02 2023, max compression
+gzip compressed data, was "tg_bot_ml-0.0.9.tar", last modified: Thu Jun 22 15:36:57 2023, max compression
```

## Comparing `tg_bot_ml-0.0.8.tar` & `tg_bot_ml-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-22 06:12:10.000000 tg_bot_ml-0.0.8/LICENSE
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      149 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/README.md
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/setup.cfg
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1259 2023-06-22 08:05:49.000000 tg_bot_ml-0.0.8/setup.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/tg_bot_ml/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/__init__.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-22 07:54:23.000000 tg_bot_ml-0.0.8/tg_bot_ml/img_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1383 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/table_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/tg_bot.py
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.8/tg_bot_ml/utils.py
-drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 08:06:02.915734 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1007 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/PKG-INFO
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/requires.txt
--rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-22 08:06:02.000000 tg_bot_ml-0.0.8/tg_bot_ml.egg-info/top_level.txt
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 15:36:57.673215 tg_bot_ml-0.0.9/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)    35149 2023-06-22 06:12:10.000000 tg_bot_ml-0.0.9/LICENSE
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2832 2023-06-22 15:36:57.673215 tg_bot_ml-0.0.9/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1517 2023-06-22 15:33:36.000000 tg_bot_ml-0.0.9/README.md
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       38 2023-06-22 15:36:57.673215 tg_bot_ml-0.0.9/setup.cfg
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1409 2023-06-22 15:36:53.000000 tg_bot_ml-0.0.9/setup.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 15:36:57.673215 tg_bot_ml-0.0.9/tg_bot_ml/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.9/tg_bot_ml/__init__.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     3162 2023-06-22 07:54:23.000000 tg_bot_ml-0.0.9/tg_bot_ml/img_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     1383 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.9/tg_bot_ml/table_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2273 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.9/tg_bot_ml/tg_bot.py
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      720 2023-06-22 06:12:46.000000 tg_bot_ml-0.0.9/tg_bot_ml/utils.py
+drwxrwxr-x   0 dmitry    (1000) dmitry    (1000)        0 2023-06-22 15:36:57.673215 tg_bot_ml-0.0.9/tg_bot_ml.egg-info/
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)     2832 2023-06-22 15:36:57.000000 tg_bot_ml-0.0.9/tg_bot_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)      305 2023-06-22 15:36:57.000000 tg_bot_ml-0.0.9/tg_bot_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)        1 2023-06-22 15:36:57.000000 tg_bot_ml-0.0.9/tg_bot_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       71 2023-06-22 15:36:57.000000 tg_bot_ml-0.0.9/tg_bot_ml.egg-info/requires.txt
+-rw-rw-r--   0 dmitry    (1000) dmitry    (1000)       10 2023-06-22 15:36:57.000000 tg_bot_ml-0.0.9/tg_bot_ml.egg-info/top_level.txt
```

### Comparing `tg_bot_ml-0.0.8/LICENSE` & `tg_bot_ml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.8/tg_bot_ml/img_bot.py` & `tg_bot_ml-0.0.9/tg_bot_ml/img_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.8/tg_bot_ml/table_bot.py` & `tg_bot_ml-0.0.9/tg_bot_ml/table_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.8/tg_bot_ml/tg_bot.py` & `tg_bot_ml-0.0.9/tg_bot_ml/tg_bot.py`

 * *Files identical despite different names*

### Comparing `tg_bot_ml-0.0.8/tg_bot_ml/utils.py` & `tg_bot_ml-0.0.9/tg_bot_ml/utils.py`

 * *Files identical despite different names*

