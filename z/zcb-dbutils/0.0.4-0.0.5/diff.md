# Comparing `tmp/zcb_dbutils-0.0.4.tar.gz` & `tmp/zcb_dbutils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcb_dbutils-0.0.4.tar", last modified: Wed Jun 28 10:46:27 2023, max compression
+gzip compressed data, was "zcb_dbutils-0.0.5.tar", last modified: Thu Jun 29 12:59:57 2023, max compression
```

## Comparing `zcb_dbutils-0.0.4.tar` & `zcb_dbutils-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 10:46:26.380865 zcb_dbutils-0.0.4/
--rwxrwxrwx   0 root         (0) root         (0)      736 2023-06-28 10:46:26.379865 zcb_dbutils-0.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      337 2023-06-28 10:44:08.000000 zcb_dbutils-0.0.4/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-28 10:46:26.381865 zcb_dbutils-0.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-28 10:46:23.000000 zcb_dbutils-0.0.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 10:46:26.315886 zcb_dbutils-0.0.4/zcb_dbutils/
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-28 10:37:05.000000 zcb_dbutils-0.0.4/zcb_dbutils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3666 2022-10-25 12:58:40.000000 zcb_dbutils-0.0.4/zcb_dbutils/dbutils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-28 10:46:26.367866 zcb_dbutils-0.0.4/zcb_dbutils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      736 2023-06-28 10:46:26.000000 zcb_dbutils-0.0.4/zcb_dbutils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      239 2023-06-28 10:46:26.000000 zcb_dbutils-0.0.4/zcb_dbutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-28 10:46:26.000000 zcb_dbutils-0.0.4/zcb_dbutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-28 10:46:26.000000 zcb_dbutils-0.0.4/zcb_dbutils.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-06-28 10:46:26.000000 zcb_dbutils-0.0.4/zcb_dbutils.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:44.033681 zcb_dbutils-0.0.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1083 2023-06-28 11:16:31.000000 zcb_dbutils-0.0.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2023-06-30 02:02:44.031681 zcb_dbutils-0.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      797 2023-06-30 02:02:09.000000 zcb_dbutils-0.0.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-30 02:02:44.034681 zcb_dbutils-0.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-30 02:01:49.000000 zcb_dbutils-0.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:43.926654 zcb_dbutils-0.0.5/test/
+-rwxrwxrwx   0 root         (0) root         (0)      757 2023-06-30 02:00:18.000000 zcb_dbutils-0.0.5/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:43.951915 zcb_dbutils-0.0.5/zcb_dbutils/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-28 10:37:05.000000 zcb_dbutils-0.0.5/zcb_dbutils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5738 2023-06-30 02:01:23.000000 zcb_dbutils-0.0.5/zcb_dbutils/dbutils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:44.012647 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      260 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/top_level.txt
```

### Comparing `zcb_dbutils-0.0.4/setup.py` & `zcb_dbutils-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'db utils with pymysql by chzcb'
 
 setup(
     name="zcb_dbutils",
     version=VERSION,
     author="chzcb",
     author_email="chzcb.04@163.com",
```

