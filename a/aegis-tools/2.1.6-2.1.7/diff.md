# Comparing `tmp/aegis-tools-2.1.6.tar.gz` & `tmp/aegis-tools-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.6.tar", last modified: Wed May 24 02:40:42 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.7.tar", last modified: Fri Jun 30 00:03:16 2023, max compression
```

## Comparing `aegis-tools-2.1.6.tar` & `aegis-tools-2.1.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.565545 aegis-tools-2.1.6/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.6/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.6/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.6/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.6/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-05-24 02:10:52.000000 aegis-tools-2.1.6/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.6/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42782 2023-05-24 01:47:27.000000 aegis-tools-2.1.6/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.573545 aegis-tools-2.1.6/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.6/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.6/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.6/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.6/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.1.6/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.6/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.585545 aegis-tools-2.1.6/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.6/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.6/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.6/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.6/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.6/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.6/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.6/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.6/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.6/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.6/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.6/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.6/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.6/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.6/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73800 2023-05-24 02:36:08.000000 aegis-tools-2.1.6/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-05-24 02:40:42.000000 aegis-tools-2.1.6/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-05-24 02:40:42.593545 aegis-tools-2.1.6/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-05-22 20:48:40.000000 aegis-tools-2.1.6/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.396596 aegis-tools-2.1.7/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.7/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18804 2023-05-12 16:02:53.000000 aegis-tools-2.1.7/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.7/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.7/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-05-24 02:49:53.000000 aegis-tools-2.1.7/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7559 2023-05-24 02:47:45.000000 aegis-tools-2.1.7/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    43046 2023-05-24 02:50:29.000000 aegis-tools-2.1.7/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.404596 aegis-tools-2.1.7/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.7/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.7/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.7/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.7/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-05-22 20:40:27.000000 aegis-tools-2.1.7/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31598 2023-06-30 00:02:27.000000 aegis-tools-2.1.7/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.7/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.7/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.7/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.7/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-04-27 02:34:36.000000 aegis-tools-2.1.7/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.7/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.7/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.7/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.7/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.7/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.7/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.7/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.7/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.7/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73800 2023-05-24 02:36:08.000000 aegis-tools-2.1.7/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-06-30 00:03:16.000000 aegis-tools-2.1.7/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-06-30 00:03:16.412596 aegis-tools-2.1.7/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-06-30 00:02:53.000000 aegis-tools-2.1.7/setup.py
```

### Comparing `aegis-tools-2.1.6/LICENSE` & `aegis-tools-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/PKG-INFO` & `aegis-tools-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.6
+Version: 2.1.7
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.6/README.md` & `aegis-tools-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/aegis_.py` & `aegis-tools-2.1.7/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/build.py` & `aegis-tools-2.1.7/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/config.py` & `aegis-tools-2.1.7/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/database.py` & `aegis-tools-2.1.7/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/hydra.py` & `aegis-tools-2.1.7/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/mailer.py` & `aegis-tools-2.1.7/aegis/mailer.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,18 @@
         email_tracking = aegis.model.EmailTracking.get_id(email_tracking_id, dbconn=dbconn)
         email_type = aegis.model.EmailType.get_id(email_tracking['email_type_id'], dbconn=dbconn)
         email_data = json.loads(email_tracking['email_data'])
         # Check to/from emails and format accordingly
         from_email = aegis.model.Email.get_id(email_tracking['from_email_id'], dbconn=dbconn)
         email_data['from_addr'] = from_email['email']
         to_email = aegis.model.Email.get_id(email_tracking['to_email_id'], dbconn=dbconn)
+        if to_email['delete_dttm']:
+            logging.error("Not sending to deleted email_id: %s", to_email['to_email_id'])
+            email_tracking.mark_deleted(dbconn=dbconn)
+            return False
         email_data['to_addr'] = to_email['email']
         # Turn this into a (first_name or email) if it's a member
         if to_email['member_id']:
             to_member = aegis.model.Member.get_auth(to_email['member_id'], dbconn=dbconn)
             if to_member:
                 email_data['to_email'] = to_email['email']
                 if to_member.get('google_user', {}).get('name'):
@@ -135,14 +139,15 @@
             domain_templates = cls.template_registry[kwargs['domain']]
             fn = domain_templates[email_type['email_type_name']]
             email_data = fn(email_data)
         kwargs['reply_to'] = email_data['from_addr']
         email_data['nl2br'] = aegis.stdlib.nl2br
         email_data['format_integer'] = aegis.stdlib.format_integer
         # It's a mouthful to convert this to Pacific time
+        # XXX TODO this should be on UTC, maybe without timezone information
         email_data['send_dttm_str'] = email_tracking['send_dttm'].astimezone(pytz.timezone('US/Pacific')).strftime('%b %d, %Y, %-H:%-M %p')
         email_data['options'] = options
         email_data['current_year'] = datetime.date.today().year
         email_data['email_tracking_id'] = email_tracking_id
         email_data['email_uuid'] = email_tracking['email_uuid']
         email_template = 'email/%s' % email_type['template_name']
         #kwargs['debug'] = True
```

### Comparing `aegis-tools-2.1.6/aegis/model.py` & `aegis-tools-2.1.7/aegis/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,14 +462,20 @@
 
     def mark_clicked(self, dbconn=None):
         if not dbconn:
             dbconn = db()
         sql = "UPDATE email_tracking SET click_dttm=NOW() WHERE email_tracking_id=%s AND click_dttm IS NULL"
         return dbconn.execute(sql, self['email_tracking_id'])
 
+    def mark_deleted(self, dbconn=None):
+        if not dbconn:
+            dbconn = db()
+        sql = "UPDATE email_tracking SET delete_dttm=NOW() WHERE email_tracking_id=%s AND delete_dttm IS NULL"
+        return dbconn.execute(sql, self['email_tracking_id'])
+
 
 class EmailLink(aegis.database.Row):
     table_name = 'email_link'
     id_column = 'email_link_id'
 
     @staticmethod
     def insert(email_id):
```

### Comparing `aegis-tools-2.1.6/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.7/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.7/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.7/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.7/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.7/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/google_signin.sql` & `aegis-tools-2.1.7/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.7/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.7/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/member_auth.sql` & `aegis-tools-2.1.7/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.7/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/sql/reports.sql` & `aegis-tools-2.1.7/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/stdlib.py` & `aegis-tools-2.1.7/aegis/stdlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import datetime
 import decimal
 import email.utils
 import functools
 import hashlib
 import inspect
 import ipaddress
+import itertools
 import json
 import logging
 import os
 import pprint
 import random
 import re
 import shlex
@@ -132,19 +133,19 @@
 def unique_list(iterable):
     m = set()
     return list(filter(lambda x: not (m.__contains__(x) or m.add(x)), iterable))
 
 # From the accepted answer on http://stackoverflow.com/questions/642763/python-intersection-of-two-lists
 # Preserves order of the items in the second iterable
 def stable_intersection(iter1, iter2):
-    return list(itertools.ifilter(set(iter1).__contains__, iter2))
+    return list(filter(set(iter1).__contains__, iter2))
 
 # Modified from above - remove items in 'iter_remove' from items in 'iter_keep'
 def stable_difference(iter_remove, iter_keep):
-    return list(itertools.ifilterfalse(set(iter_remove).__contains__, iter_keep))
+    return list(itertools.filterfalse(set(iter_remove).__contains__, iter_keep))
 
 def loopnext(iterable, itr):
     try:
         val = next(itr)
     except StopIteration:
         itr = iter(iterable)
         val = next(itr)
```

### Comparing `aegis-tools-2.1.6/aegis/templates/build.html` & `aegis-tools-2.1.7/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/build_confirm.html` & `aegis-tools-2.1.7/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/build_form.html` & `aegis-tools-2.1.7/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/build_view.html` & `aegis-tools-2.1.7/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/frame.html` & `aegis-tools-2.1.7/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/hydra.html` & `aegis-tools-2.1.7/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/hydra_form.html` & `aegis-tools-2.1.7/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.7/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/report.html` & `aegis-tools-2.1.7/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/report_form.html` & `aegis-tools-2.1.7/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/reports.html` & `aegis-tools-2.1.7/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/templates/w3.css` & `aegis-tools-2.1.7/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/threadpool.py` & `aegis-tools-2.1.7/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis/webapp.py` & `aegis-tools-2.1.7/aegis/webapp.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.7/aegis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.6
+Version: 2.1.7
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.6/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.7/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.6/setup.py` & `aegis-tools-2.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.6',
+    version = '2.1.7',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

