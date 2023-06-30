# Comparing `tmp/ns_asphalt9-0.0.2.tar.gz` & `tmp/ns_asphalt9-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.0.2.tar", last modified: Fri Jun 30 07:19:51 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.0.3.tar", last modified: Fri Jun 30 07:35:25 2023, max compression
```

## Comparing `ns_asphalt9-0.0.2.tar` & `ns_asphalt9-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,50 @@
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.689252 ns_asphalt9-0.0.2/
--rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.2/LICENSE
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:19:51.689398 ns_asphalt9-0.0.2/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.2/README.md
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.687257 ns_asphalt9-0.0.2/ns_asphalt9/
--rw-r--r--   0 neo.sun    (502) staff       (20)     5062 2023-06-29 06:51:56.000000 ns_asphalt9-0.0.2/ns_asphalt9/main.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.688745 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)      320 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-06-30 07:19:51.000000 ns_asphalt9-0.0.2/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-06-30 07:19:51.689788 ns_asphalt9-0.0.2/setup.cfg
--rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.2/setup.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:19:51.688883 ns_asphalt9-0.0.2/tests/
--rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.2/tests/test_ocr.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.523656 ns_asphalt9-0.0.3/
+-rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.3/LICENSE
+-rw-r--r--   0 neo.sun    (502) staff       (20)      180 2023-06-30 07:35:13.000000 ns_asphalt9-0.0.3/MANIFEST.in
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:35:25.523754 ns_asphalt9-0.0.3/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.3/README.md
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.514191 ns_asphalt9-0.0.3/ns_asphalt9/
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.518220 ns_asphalt9-0.0.3/ns_asphalt9/core/
+-rw-r--r--   0 neo.sun    (502) staff       (20)       23 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.519435 ns_asphalt9-0.0.3/ns_asphalt9/core/actions/
+-rw-r--r--   0 neo.sun    (502) staff       (20)      245 2023-06-27 07:33:41.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      341 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3232 2023-06-28 09:14:48.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3841 2023-06-27 08:03:14.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3551 2023-06-28 11:15:02.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      706 2023-06-28 08:30:50.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/cache.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2556 2023-06-28 07:46:07.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/consts.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2150 2023-06-27 07:32:16.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/controller.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      498 2023-06-28 01:53:10.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.519791 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/
+-rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-26 05:07:57.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)    17447 2023-06-28 07:35:12.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.521811 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3097 2023-06-26 08:14:33.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2900 2023-06-26 08:18:26.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)   202347 2023-06-26 05:17:10.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3159 2023-06-26 08:11:35.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1542 2023-06-29 06:51:02.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1858 2023-06-29 06:53:17.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)    10879 2023-06-28 10:07:08.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/pages.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      265 2023-06-29 06:50:43.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2499 2023-06-28 11:21:11.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.523103 ns_asphalt9-0.0.3/ns_asphalt9/core/utils/
+-rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1022 2023-06-28 08:37:33.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      459 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1994 2023-06-27 10:03:16.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      860 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.3/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     5062 2023-06-30 07:28:10.000000 ns_asphalt9-0.0.3/ns_asphalt9/main.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.515358 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:35:25.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1187 2023-06-30 07:35:25.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:35:25.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-06-30 07:35:25.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-06-30 07:35:25.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-06-30 07:35:25.000000 ns_asphalt9-0.0.3/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-06-30 07:35:25.524135 ns_asphalt9-0.0.3/setup.cfg
+-rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.3/setup.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:35:25.523354 ns_asphalt9-0.0.3/tests/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.3/tests/test_ocr.py
```

### Comparing `ns_asphalt9-0.0.2/LICENSE` & `ns_asphalt9-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.2/PKG-INFO` & `ns_asphalt9-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.2/README.md` & `ns_asphalt9-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.2/ns_asphalt9/main.py` & `ns_asphalt9-0.0.3/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.2/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.0.3/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.2/setup.cfg` & `ns_asphalt9-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.2
+version = 0.0.3
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.0.2/tests/test_ocr.py` & `ns_asphalt9-0.0.3/tests/test_ocr.py`

 * *Files identical despite different names*

