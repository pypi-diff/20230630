# Comparing `tmp/egune-0.2.8.tar.gz` & `tmp/egune-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egune-0.2.8.tar", last modified: Tue Apr 11 03:08:25 2023, max compression
+gzip compressed data, was "egune-0.2.9.tar", last modified: Fri Apr 21 04:22:25 2023, max compression
```

## Comparing `egune-0.2.8.tar` & `egune-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 bilguun   (1000) bilguun   (1000)        0 2023-04-11 03:08:25.778063 egune-0.2.8/
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)     1073 2023-02-10 02:45:00.000000 egune-0.2.8/LICENSE
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)      342 2023-04-11 03:08:25.778063 egune-0.2.8/PKG-INFO
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)        0 2023-02-10 02:45:00.000000 egune-0.2.8/README.md
-drwxrwxr-x   0 bilguun   (1000) bilguun   (1000)        0 2023-04-11 03:08:25.778063 egune-0.2.8/egune/
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)        0 2023-03-01 04:05:07.000000 egune-0.2.8/egune/__init__.py
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)     4704 2023-03-30 06:15:28.000000 egune-0.2.8/egune/dataclasses.py
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)     3213 2023-04-11 03:07:41.000000 egune-0.2.8/egune/definitions.py
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)    13848 2023-03-02 07:34:54.000000 egune-0.2.8/egune/difference.py
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)     2946 2023-03-01 03:20:55.000000 egune-0.2.8/egune/enumerators.py
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)     2119 2023-03-01 07:45:48.000000 egune-0.2.8/egune/logger.py
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)     4777 2023-03-01 03:10:50.000000 egune-0.2.8/egune/utils.py
-drwxrwxr-x   0 bilguun   (1000) bilguun   (1000)        0 2023-04-11 03:08:25.778063 egune-0.2.8/egune.egg-info/
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)      342 2023-04-11 03:08:25.000000 egune-0.2.8/egune.egg-info/PKG-INFO
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)      310 2023-04-11 03:08:25.000000 egune-0.2.8/egune.egg-info/SOURCES.txt
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)        1 2023-04-11 03:08:25.000000 egune-0.2.8/egune.egg-info/dependency_links.txt
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)       13 2023-04-11 03:08:25.000000 egune-0.2.8/egune.egg-info/requires.txt
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)        6 2023-04-11 03:08:25.000000 egune-0.2.8/egune.egg-info/top_level.txt
--rwxr-xr-x   0 bilguun   (1000) bilguun   (1000)       68 2023-02-10 02:45:00.000000 egune-0.2.8/egunesh
--rw-rw-r--   0 bilguun   (1000) bilguun   (1000)       38 2023-04-11 03:08:25.778063 egune-0.2.8/setup.cfg
--rw-r--r--   0 bilguun   (1000) bilguun   (1000)      631 2023-04-11 03:08:22.000000 egune-0.2.8/setup.py
+drwxrwxr-x   0 bilguun   (1000) docker     (999)        0 2023-04-21 04:22:25.933211 egune-0.2.9/
+-rw-r--r--   0 bilguun   (1000) docker     (999)     1073 2023-02-10 02:45:00.000000 egune-0.2.9/LICENSE
+-rw-rw-r--   0 bilguun   (1000) docker     (999)      342 2023-04-21 04:22:25.933211 egune-0.2.9/PKG-INFO
+-rw-r--r--   0 bilguun   (1000) docker     (999)        0 2023-02-10 02:45:00.000000 egune-0.2.9/README.md
+drwxrwxr-x   0 bilguun   (1000) docker     (999)        0 2023-04-21 04:22:25.933211 egune-0.2.9/egune/
+-rw-r--r--   0 bilguun   (1000) docker     (999)        0 2023-03-01 04:05:07.000000 egune-0.2.9/egune/__init__.py
+-rw-rw-r--   0 bilguun   (1000) docker     (999)     4704 2023-03-30 06:15:28.000000 egune-0.2.9/egune/dataclasses.py
+-rw-rw-r--   0 bilguun   (1000) docker     (999)     3219 2023-04-21 04:22:07.000000 egune-0.2.9/egune/definitions.py
+-rw-rw-r--   0 bilguun   (1000) docker     (999)    13848 2023-03-02 07:34:54.000000 egune-0.2.9/egune/difference.py
+-rw-rw-r--   0 bilguun   (1000) docker     (999)     2946 2023-03-01 03:20:55.000000 egune-0.2.9/egune/enumerators.py
+-rw-r--r--   0 bilguun   (1000) docker     (999)     2119 2023-03-01 07:45:48.000000 egune-0.2.9/egune/logger.py
+-rw-r--r--   0 bilguun   (1000) docker     (999)     4777 2023-03-01 03:10:50.000000 egune-0.2.9/egune/utils.py
+drwxrwxr-x   0 bilguun   (1000) docker     (999)        0 2023-04-21 04:22:25.933211 egune-0.2.9/egune.egg-info/
+-rw-r--r--   0 bilguun   (1000) docker     (999)      342 2023-04-21 04:22:25.000000 egune-0.2.9/egune.egg-info/PKG-INFO
+-rw-r--r--   0 bilguun   (1000) docker     (999)      310 2023-04-21 04:22:25.000000 egune-0.2.9/egune.egg-info/SOURCES.txt
+-rw-r--r--   0 bilguun   (1000) docker     (999)        1 2023-04-21 04:22:25.000000 egune-0.2.9/egune.egg-info/dependency_links.txt
+-rw-rw-r--   0 bilguun   (1000) docker     (999)       13 2023-04-21 04:22:25.000000 egune-0.2.9/egune.egg-info/requires.txt
+-rw-r--r--   0 bilguun   (1000) docker     (999)        6 2023-04-21 04:22:25.000000 egune-0.2.9/egune.egg-info/top_level.txt
+-rwxr-xr-x   0 bilguun   (1000) docker     (999)       68 2023-02-10 02:45:00.000000 egune-0.2.9/egunesh
+-rw-rw-r--   0 bilguun   (1000) docker     (999)       38 2023-04-21 04:22:25.933211 egune-0.2.9/setup.cfg
+-rw-r--r--   0 bilguun   (1000) docker     (999)      631 2023-04-21 04:22:24.000000 egune-0.2.9/setup.py
```

### Comparing `egune-0.2.8/LICENSE` & `egune-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `egune-0.2.8/egune/dataclasses.py` & `egune-0.2.9/egune/dataclasses.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.8/egune/definitions.py` & `egune-0.2.9/egune/definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     def build_issue(self, slotDefs: List[SlotDef], id=None, context=None, userMessage=None):
         filled_slots = {}
         for slotDef in slotDefs:
             slotName = slotDef.name
             if slotDef.canUsePrev:
                 if context is not None:
-                    for prev_issue in (context.activeIssues + context.inactiveIssues):
+                    for prev_issue in (context.activeIssues + context.inactiveIssues)[::-1]:
                         if slotName in prev_issue.slotValues:
                             filled_slots[slotName] = deepcopy(
                                 prev_issue.slotValues[slotName]
                             )
                             break
             if userMessage is not None:
                 for entity_name in slotDef.entities:
```

### Comparing `egune-0.2.8/egune/difference.py` & `egune-0.2.9/egune/difference.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.8/egune/enumerators.py` & `egune-0.2.9/egune/enumerators.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.8/egune/logger.py` & `egune-0.2.9/egune/logger.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.8/egune/utils.py` & `egune-0.2.9/egune/utils.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.8/setup.py` & `egune-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='egune',
-    version='0.2.8',
+    version='0.2.9',
     scripts=['egunesh'],
     author="Bilguun Chinzorig",
     author_email="bilguun@bolorsoft.com",
     description="Egune Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

