# Comparing `tmp/funbuild-202306301655.tar.gz` & `tmp/funbuild-202306301707.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funbuild-202306301655.tar", last modified: Fri Jun 30 08:55:56 2023, max compression
+gzip compressed data, was "funbuild-202306301707.tar", last modified: Fri Jun 30 09:07:25 2023, max compression
```

## Comparing `funbuild-202306301655.tar` & `funbuild-202306301707.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.633218 funbuild-202306301655/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:52:20.000000 funbuild-202306301655/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 08:55:56.633218 funbuild-202306301655/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       66 2023-06-30 08:53:11.000000 funbuild-202306301655/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.621217 funbuild-202306301655/funbuild/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.629217 funbuild-202306301655/funbuild/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       27 2023-06-30 08:53:14.000000 funbuild-202306301655/funbuild/core/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5399 2023-06-30 08:53:21.000000 funbuild-202306301655/funbuild/core/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1398 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/core/version.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.629217 funbuild-202306301655/funbuild/git/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/git/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/git/repo.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.629217 funbuild-202306301655/funbuild/manage/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       43 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/manage/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2725 2023-06-30 08:53:30.000000 funbuild-202306301655/funbuild/manage/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       36 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/manage/port.md
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10670 2023-06-30 08:53:32.000000 funbuild-202306301655/funbuild/manage/supervisord.conf
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.629217 funbuild-202306301655/funbuild/shell/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       80 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/shell/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1172 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/shell/core.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.629217 funbuild-202306301655/funbuild/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       34 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/temp/core.json
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/temp/core.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.633218 funbuild-202306301655/funbuild/tool/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       32 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/tool/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      167 2023-06-30 08:53:35.000000 funbuild-202306301655/funbuild/tool/build.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      860 2023-06-30 08:52:20.000000 funbuild-202306301655/funbuild/tool/fastapi.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:55:56.625218 funbuild-202306301655/funbuild.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 08:55:56.000000 funbuild-202306301655/funbuild.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      665 2023-06-30 08:55:56.000000 funbuild-202306301655/funbuild.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 08:55:56.000000 funbuild-202306301655/funbuild.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       52 2023-06-30 08:55:56.000000 funbuild-202306301655/funbuild.egg-info/entry_points.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       10 2023-06-30 08:55:56.000000 funbuild-202306301655/funbuild.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-06-30 08:55:56.000000 funbuild-202306301655/funbuild.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 08:55:56.633218 funbuild-202306301655/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      559 2023-06-30 08:55:28.000000 funbuild-202306301655/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:52:20.000000 funbuild-202306301707/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 09:07:25.809501 funbuild-202306301707/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       66 2023-06-30 08:53:11.000000 funbuild-202306301707/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.805500 funbuild-202306301707/funbuild/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       27 2023-06-30 08:53:14.000000 funbuild-202306301707/funbuild/core/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     5399 2023-06-30 08:53:21.000000 funbuild-202306301707/funbuild/core/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1398 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/core/version.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild/git/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/git/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/git/repo.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild/manage/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       43 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/manage/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2725 2023-06-30 08:53:30.000000 funbuild-202306301707/funbuild/manage/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       36 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/manage/port.md
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10670 2023-06-30 08:53:32.000000 funbuild-202306301707/funbuild/manage/supervisord.conf
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild/shell/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       80 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/shell/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1172 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/shell/core.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       34 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/temp/core.json
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/temp/core.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild/tool/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       32 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/tool/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      167 2023-06-30 08:53:35.000000 funbuild-202306301707/funbuild/tool/build.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      860 2023-06-30 08:52:20.000000 funbuild-202306301707/funbuild/tool/fastapi.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:07:25.809501 funbuild-202306301707/funbuild.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-06-30 09:07:25.000000 funbuild-202306301707/funbuild.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      665 2023-06-30 09:07:25.000000 funbuild-202306301707/funbuild.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 09:07:25.000000 funbuild-202306301707/funbuild.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       52 2023-06-30 09:07:25.000000 funbuild-202306301707/funbuild.egg-info/entry_points.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       10 2023-06-30 09:07:25.000000 funbuild-202306301707/funbuild.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-06-30 09:07:25.000000 funbuild-202306301707/funbuild.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 09:07:25.809501 funbuild-202306301707/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      559 2023-06-30 08:55:28.000000 funbuild-202306301707/setup.py
```

### Comparing `funbuild-202306301655/LICENSE` & `funbuild-202306301707/LICENSE`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild/core/core.py` & `funbuild-202306301707/funbuild/core/core.py`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild/core/version.py` & `funbuild-202306301707/funbuild/core/version.py`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild/manage/core.py` & `funbuild-202306301707/funbuild/manage/core.py`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild/manage/supervisord.conf` & `funbuild-202306301707/funbuild/manage/supervisord.conf`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild/shell/core.py` & `funbuild-202306301707/funbuild/shell/core.py`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild/tool/fastapi.py` & `funbuild-202306301707/funbuild/tool/fastapi.py`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/funbuild.egg-info/SOURCES.txt` & `funbuild-202306301707/funbuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funbuild-202306301655/setup.py` & `funbuild-202306301707/setup.py`

 * *Files identical despite different names*

