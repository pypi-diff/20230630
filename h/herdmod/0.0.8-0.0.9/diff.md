# Comparing `tmp/herdmod-0.0.8.tar.gz` & `tmp/herdmod-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herdmod-0.0.8.tar", last modified: Fri Jun 30 14:04:56 2023, max compression
+gzip compressed data, was "herdmod-0.0.9.tar", last modified: Fri Jun 30 14:08:48 2023, max compression
```

## Comparing `herdmod-0.0.8.tar` & `herdmod-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.712213 herdmod-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 14:04:42.000000 herdmod-0.0.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 14:04:42.000000 herdmod-0.0.8/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 14:04:42.000000 herdmod-0.0.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 14:04:56.712213 herdmod-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 14:04:42.000000 herdmod-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.708213 herdmod-0.0.8/herdmod/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.708213 herdmod-0.0.8/herdmod/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.708213 herdmod-0.0.8/herdmod/listen/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/listen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/listen/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.708213 herdmod-0.0.8/herdmod/nav/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/nav/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.708213 herdmod-0.0.8/herdmod/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 14:04:42.000000 herdmod-0.0.8/herdmod/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:04:56.708213 herdmod-0.0.8/herdmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 14:04:56.000000 herdmod-0.0.8/herdmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 14:04:56.000000 herdmod-0.0.8/herdmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:04:56.000000 herdmod-0.0.8/herdmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 14:04:56.000000 herdmod-0.0.8/herdmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 14:04:56.000000 herdmod-0.0.8/herdmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:04:56.712213 herdmod-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 14:04:42.000000 herdmod-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.706180 herdmod-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 14:08:37.000000 herdmod-0.0.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 14:08:37.000000 herdmod-0.0.9/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 14:08:37.000000 herdmod-0.0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 14:08:48.706180 herdmod-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-30 14:08:37.000000 herdmod-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.702180 herdmod-0.0.9/herdmod/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.706180 herdmod-0.0.9/herdmod/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.706180 herdmod-0.0.9/herdmod/listen/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/listen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/listen/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.706180 herdmod-0.0.9/herdmod/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/nav/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.706180 herdmod-0.0.9/herdmod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 14:08:37.000000 herdmod-0.0.9/herdmod/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:08:48.706180 herdmod-0.0.9/herdmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-30 14:08:48.000000 herdmod-0.0.9/herdmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-30 14:08:48.000000 herdmod-0.0.9/herdmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:08:48.000000 herdmod-0.0.9/herdmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 14:08:48.000000 herdmod-0.0.9/herdmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 14:08:48.000000 herdmod-0.0.9/herdmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:08:48.706180 herdmod-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 14:08:37.000000 herdmod-0.0.9/setup.py
```

### Comparing `herdmod-0.0.8/COPYING` & `herdmod-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/COPYING.lesser` & `herdmod-0.0.9/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/NOTICE` & `herdmod-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/PKG-INFO` & `herdmod-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.8
+Version: 0.0.9
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.0.8/README.md` & `herdmod-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/herdmod/helpers/helpers.py` & `herdmod-0.0.9/herdmod/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/herdmod/listen/listen.py` & `herdmod-0.0.9/herdmod/listen/listen.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,17 @@
         **kwargs
     ):
         request = await self.send_message(identifier[0], text, *args, **kwargs)
         response = await self.listen(
             identifier, filters, listener_type, timeout
         )
         if response:
-            response.request = await self.get_messages(identifier[0], request.id)
+            response.request = await self.get_messages(
+                identifier[0], request.id, replies=0
+            )
 
         return response
 
     """
     needed for matching when message_id or
     user_id is null, and to take precedence
     """
```

### Comparing `herdmod-0.0.8/herdmod/nav/pagination.py` & `herdmod-0.0.9/herdmod/nav/pagination.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/herdmod/utils/utils.py` & `herdmod-0.0.9/herdmod/utils/utils.py`

 * *Files identical despite different names*

### Comparing `herdmod-0.0.8/herdmod.egg-info/PKG-INFO` & `herdmod-0.0.9/herdmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herdmod
-Version: 0.0.8
+Version: 0.0.9
 Summary: A monkeypatcher add-on for Pyroherd
 Home-page: https://github.com/OnTheHerd/herdmod
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `herdmod-0.0.8/setup.py` & `herdmod-0.0.9/setup.py`

 * *Files identical despite different names*

