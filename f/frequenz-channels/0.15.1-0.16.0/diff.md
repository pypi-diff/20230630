# Comparing `tmp/frequenz-channels-0.15.1.tar.gz` & `tmp/frequenz-channels-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-channels-0.15.1.tar", last modified: Tue May 23 14:19:20 2023, max compression
+gzip compressed data, was "frequenz-channels-0.16.0.tar", last modified: Fri Jun 30 15:11:31 2023, max compression
```

## Comparing `frequenz-channels-0.15.1.tar` & `frequenz-channels-0.16.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      539 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/src/
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.241454 frequenz-channels-0.15.1/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/src/frequenz/channels/
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_anycast.py
--rw-r--r--   0 runner    (1001) docker     (122)     6348 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (122)    12090 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/src/frequenz/channels/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4249 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_merge.py
--rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_merge_named.py
--rw-r--r--   0 runner    (1001) docker     (122)     6924 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_select.py
--rw-r--r--   0 runner    (1001) docker     (122)    25535 2023-05-23 14:19:09.000000 frequenz-channels-0.15.1/src/frequenz/channels/util/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 14:19:20.245454 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-23 14:19:20.000000 frequenz-channels-0.15.1/src/frequenz_channels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.571517 frequenz-channels-0.16.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/src/frequenz/channels/
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/_anycast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6348 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/_bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12090 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/src/frequenz/channels/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4821 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4249 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/_merge_named.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15976 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/_select.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27024 2023-06-30 15:11:21.000000 frequenz-channels-0.16.0/src/frequenz/channels/util/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 15:11:31.575518 frequenz-channels-0.16.0/src/frequenz_channels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-30 15:11:31.000000 frequenz-channels-0.16.0/src/frequenz_channels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-30 15:11:31.000000 frequenz-channels-0.16.0/src/frequenz_channels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 15:11:31.000000 frequenz-channels-0.16.0/src/frequenz_channels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-30 15:11:31.000000 frequenz-channels-0.16.0/src/frequenz_channels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-30 15:11:31.000000 frequenz-channels-0.16.0/src/frequenz_channels.egg-info/top_level.txt
```

### Comparing `frequenz-channels-0.15.1/CONTRIBUTING.md` & `frequenz-channels-0.16.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/LICENSE` & `frequenz-channels-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/PKG-INFO` & `frequenz-channels-0.16.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: frequenz-channels
-Version: 0.15.1
+Version: 0.16.0
 Summary: Channel implementations for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-channels-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-channels-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-channels-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support
 Keywords: frequenz,channel
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 # Frequenz channels
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-channels-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-channels-python/actions/workflows/ci.yaml)
```

### Comparing `frequenz-channels-0.15.1/README.md` & `frequenz-channels-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/docs/css/mkdocstrings.css` & `frequenz-channels-0.16.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/docs/css/style.css` & `frequenz-channels-0.16.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/docs/logo.png` & `frequenz-channels-0.16.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/docs/mkdocstrings_autoapi.py` & `frequenz-channels-0.16.0/docs/mkdocstrings_autoapi.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/mkdocs.yml` & `frequenz-channels-0.16.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/pyproject.toml` & `frequenz-channels-0.16.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,35 +11,32 @@
 keywords = ["frequenz", "channel"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
   "Topic :: Software Development :: Libraries",
 ]
-requires-python = ">= 3.8, < 4"
+requires-python = ">= 3.11, < 4"
 dependencies = ["watchfiles >= 0.15.0, < 0.20.0"]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 docs = [
   "mike == 1.1.2",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.0",
-  "mkdocs-material == 9.1.14",
+  "mkdocs-material == 9.1.17",
   "mkdocs-section-index == 0.3.5",
-  "mkdocstrings[python] == 0.21.2",
+  "mkdocstrings[python] == 0.22.0",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-channels-python/releases"
 Repository = "https://github.com/frequenz-floss/frequenz-channels-python"
 Issues = "https://github.com/frequenz-floss/frequenz-channels-python/issues"
 Support = "https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support"
```

### Comparing `frequenz-channels-0.15.1/src/conftest.py` & `frequenz-channels-0.16.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/__init__.py` & `frequenz-channels-0.16.0/src/frequenz/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/_anycast.py` & `frequenz-channels-0.16.0/src/frequenz/channels/_anycast.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     In cases where each message need to be received by every receiver, a
     [Broadcast][frequenz.channels.Broadcast] channel may be used.
 
     Uses an [deque][collections.deque] internally, so Anycast channels are not
     thread-safe.
 
     When there are multiple channel receivers, they can be awaited
-    simultaneously using [Select][frequenz.channels.util.Select],
+    simultaneously using [select][frequenz.channels.util.select],
     [Merge][frequenz.channels.util.Merge] or
     [MergeNamed][frequenz.channels.util.MergeNamed].
 
     Example:
         ``` python
         async def send(sender: channel.Sender) -> None:
             while True:
```

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/_base_classes.py` & `frequenz-channels-0.16.0/src/frequenz/channels/_base_classes.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/_bidirectional.py` & `frequenz-channels-0.16.0/src/frequenz/channels/_bidirectional.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/_broadcast.py` & `frequenz-channels-0.16.0/src/frequenz/channels/_broadcast.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     receivers.
 
     Internally, a broadcast receiver's buffer is implemented with just
     append/pop operations on either side of a [deque][collections.deque], which
     are thread-safe.  Because of this, `Broadcast` channels are thread-safe.
 
     When there are multiple channel receivers, they can be awaited
-    simultaneously using [Select][frequenz.channels.util.Select],
+    simultaneously using [select][frequenz.channels.util.select],
     [Merge][frequenz.channels.util.Merge] or
     [MergeNamed][frequenz.channels.util.MergeNamed].
 
     Example:
         ``` python
         async def send(sender: channel.Sender) -> None:
             while True:
```

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/_exceptions.py` & `frequenz-channels-0.16.0/src/frequenz/channels/_exceptions.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/util/__init__.py` & `frequenz-channels-0.16.0/src/frequenz/channels/util/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Channel utilities.
 
 A module with several utilities to work with channels:
 
+* [Event][frequenz.channels.util.Event]:
+  A [receiver][frequenz.channels.Receiver] that can be made ready through an event.
+
 * [FileWatcher][frequenz.channels.util.FileWatcher]:
   A [receiver][frequenz.channels.Receiver] that watches for file events.
 
 * [Merge][frequenz.channels.util.Merge]:
   A [receiver][frequenz.channels.Receiver] that merge messages coming from
   multiple receivers into a single stream.
 
@@ -16,35 +19,48 @@
   A [receiver][frequenz.channels.Receiver] that merge messages coming from
   multiple receivers into a single named stream, allowing to identify the
   origin of each message.
 
 * [Timer][frequenz.channels.util.Timer]:
   A [receiver][frequenz.channels.Receiver] that ticks at certain intervals.
 
-* [Select][frequenz.channels.util.Select]: A helper to select the next
-  available message for each [receiver][frequenz.channels.Receiver] in a group
-  of receivers.
+* [select][frequenz.channels.util.select]:  Iterate over the values of all
+  [receivers][frequenz.channels.Receiver] as new values become available.
 """
 
+from ._event import Event
 from ._file_watcher import FileWatcher
 from ._merge import Merge
 from ._merge_named import MergeNamed
-from ._select import Select
+from ._select import (
+    Selected,
+    SelectError,
+    SelectErrorGroup,
+    UnhandledSelectedError,
+    select,
+    selected_from,
+)
 from ._timer import (
     MissedTickPolicy,
     SkipMissedAndDrift,
     SkipMissedAndResync,
     Timer,
     TriggerAllMissed,
 )
 
 __all__ = [
+    "Event",
     "FileWatcher",
     "Merge",
     "MergeNamed",
     "MissedTickPolicy",
-    "Timer",
-    "Select",
+    "SelectError",
+    "SelectErrorGroup",
+    "Selected",
     "SkipMissedAndDrift",
     "SkipMissedAndResync",
+    "Timer",
     "TriggerAllMissed",
+    "UnhandledSelectedError",
+    "select",
+    "selected_from",
 ]
```

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/util/_file_watcher.py` & `frequenz-channels-0.16.0/src/frequenz/channels/util/_file_watcher.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/util/_merge.py` & `frequenz-channels-0.16.0/src/frequenz/channels/util/_merge.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/util/_merge_named.py` & `frequenz-channels-0.16.0/src/frequenz/channels/util/_merge_named.py`

 * *Files identical despite different names*

### Comparing `frequenz-channels-0.15.1/src/frequenz/channels/util/_timer.py` & `frequenz-channels-0.16.0/src/frequenz/channels/util/_timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,22 @@
 
         Returns:
             The next tick time (in microseconds) according to
                 `missed_tick_policy`.
         """
         return 0  # dummy value to avoid darglint warnings
 
+    def __repr__(self) -> str:
+        """Return a string representation of the instance.
+
+        Returns:
+            The string representation of the instance.
+        """
+        return f"{type(self).__name__}()"
+
 
 class TriggerAllMissed(MissedTickPolicy):
     """A policy that triggers all the missed ticks immediately until it catches up.
 
     Example:
         Assume a timer with interval 1 second, the tick `T0` happens exactly
         at time 0, the second tick, `T1`, happens at time 1.2 (0.2 seconds
@@ -238,14 +246,30 @@
             The next tick time (in microseconds).
         """
         drift = now - scheduled_tick_time
         if drift > self._tolerance:
             return now + interval
         return scheduled_tick_time + interval
 
+    def __str__(self) -> str:
+        """Return a string representation of the instance.
+
+        Returns:
+            The string representation of the instance.
+        """
+        return f"{type(self).__name__}({self.delay_tolerance})"
+
+    def __repr__(self) -> str:
+        """Return a string representation of the instance.
+
+        Returns:
+            The string representation of the instance.
+        """
+        return f"{type(self).__name__}({self.delay_tolerance=})"
+
 
 class Timer(Receiver[timedelta]):
     """A timer receiver that triggers every `interval` time.
 
     The timer as microseconds resolution, so the `interval` must be at least
     1 microsecond.
 
@@ -279,72 +303,70 @@
 
     Example: Periodic timer example
         ```python
         async for drift in Timer.periodic(timedelta(seconds=1.0)):
             print(f"The timer has triggered {drift=}")
         ```
 
-        But you can also use [`Select`][frequenz.channels.util.Select] to combine it
-        with other receivers, and even start it (semi) manually:
+        But you can also use a [`select`][frequenz.channels.util.select] to combine
+        it with other receivers, and even start it (semi) manually:
 
         ```python
         import logging
-        from frequenz.channels.util import Select
+        from frequenz.channels.util import select, selected_from
         from frequenz.channels import Broadcast
 
         timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
         chan = Broadcast[int]("input-chan")
-        receiver1 = chan.new_receiver()
+        battery_data = chan.new_receiver()
 
         timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
         # Do some other initialization, the timer will start automatically if
         # a message is awaited (or manually via `reset()`).
-        select = Select(bat_1=receiver1, timer=timer)
-        while await select.ready():
-            if msg := select.bat_1:
-                if val := msg.inner:
-                    battery_soc = val
-                else:
+        async for selected in select(battery_data, timer):
+            if selected_from(selected, battery_data):
+                if selected.was_closed():
                     logging.warning("battery channel closed")
-            elif drift := select.timer:
+                    continue
+                battery_soc = selected.value
+            elif selected_from(selected, timer):
                 # Print some regular battery data
                 print(f"Battery is charged at {battery_soc}%")
         ```
 
     Example: Timeout example
         ```python
         import logging
-        from frequenz.channels.util import Select
+        from frequenz.channels.util import select, selected_from
         from frequenz.channels import Broadcast
 
         def process_data(data: int):
             logging.info("Processing data: %d", data)
 
         def do_heavy_processing(data: int):
             logging.info("Heavy processing data: %d", data)
 
         timer = Timer.timeout(timedelta(seconds=1.0), auto_start=False)
         chan1 = Broadcast[int]("input-chan-1")
         chan2 = Broadcast[int]("input-chan-2")
-        receiver1 = chan1.new_receiver()
-        receiver2 = chan2.new_receiver()
-        select = Select(bat_1=receiver1, heavy_process=receiver2, timeout=timer)
-        while await select.ready():
-            if msg := select.bat_1:
-                if val := msg.inner:
-                    process_data(val)
-                    timer.reset()
-                else:
+        battery_data = chan1.new_receiver()
+        heavy_process = chan2.new_receiver()
+        async for selected in select(battery_data, heavy_process, timer):
+            if selected_from(selected, battery_data):
+                if selected.was_closed():
                     logging.warning("battery channel closed")
-            if msg := select.heavy_process:
-                if val := msg.inner:
-                    do_heavy_processing(val)
-                else:
+                    continue
+                process_data(selected.value)
+                timer.reset()
+            elif selected_from(selected, heavy_process):
+                if selected.was_closed():
                     logging.warning("processing channel closed")
-            elif drift := select.timeout:
+                    continue
+                do_heavy_processing(selected.value)
+            elif selected_from(selected, timer):
                 logging.warning("No data received in time")
         ```
 
         In this case `do_heavy_processing` might take 2 seconds, and we don't
         want our timeout timer to trigger for the missed ticks, and want the
         next tick to be relative to the time timer was last triggered.
     """
@@ -361,17 +383,18 @@
         """Create an instance.
 
         See the class documentation for details.
 
         Args:
             interval: The time between timer ticks. Must be at least
                 1 microsecond.
-            missed_tick_policy: The policy of the timer when it misses
-                a tick. See the documentation of `MissedTickPolicy` for
-                details.
+            missed_tick_policy: The policy of the timer when it misses a tick.
+                Commonly one of `TriggerAllMissed`, `SkipMissedAndResync`, `SkipMissedAndDrift`
+                or a custom class deriving from `MissedTickPolicy`. See the
+                documentation of the each class for more details.
             auto_start: Whether the timer should be started when the
                 instance is created. This can only be `True` if there is
                 already a running loop or an explicit `loop` that is running
                 was passed.
             loop: The event loop to use to track time. If `None`,
                 `asyncio.get_running_loop()` will be used.
 
@@ -676,7 +699,26 @@
     def _now(self) -> int:
         """Return the current monotonic clock time in microseconds.
 
         Returns:
             The current monotonic clock time in microseconds.
         """
         return _to_microseconds(self._loop.time())
+
+    def __str__(self) -> str:
+        """Return a string representation of the timer.
+
+        Returns:
+            The string representation of the timer.
+        """
+        return f"{type(self).__name__}({self.interval})"
+
+    def __repr__(self) -> str:
+        """Return a string representation of the timer.
+
+        Returns:
+            The string representation of the timer.
+        """
+        return (
+            f"{type(self).__name__}<{self.interval=}, {self.missed_tick_policy=}, "
+            f"{self.loop=}, {self.is_running=}>"
+        )
```

### Comparing `frequenz-channels-0.15.1/src/frequenz_channels.egg-info/PKG-INFO` & `frequenz-channels-0.16.0/src/frequenz_channels.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: frequenz-channels
-Version: 0.15.1
+Version: 0.16.0
 Summary: Channel implementations for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-channels-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-channels-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-channels-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-channels-python/discussions/categories/support
 Keywords: frequenz,channel
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 # Frequenz channels
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-channels-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-channels-python/actions/workflows/ci.yaml)
```

### Comparing `frequenz-channels-0.15.1/src/frequenz_channels.egg-info/SOURCES.txt` & `frequenz-channels-0.16.0/src/frequenz_channels.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/frequenz/channels/_anycast.py
 src/frequenz/channels/_base_classes.py
 src/frequenz/channels/_bidirectional.py
 src/frequenz/channels/_broadcast.py
 src/frequenz/channels/_exceptions.py
 src/frequenz/channels/py.typed
 src/frequenz/channels/util/__init__.py
+src/frequenz/channels/util/_event.py
 src/frequenz/channels/util/_file_watcher.py
 src/frequenz/channels/util/_merge.py
 src/frequenz/channels/util/_merge_named.py
 src/frequenz/channels/util/_select.py
 src/frequenz/channels/util/_timer.py
 src/frequenz_channels.egg-info/PKG-INFO
 src/frequenz_channels.egg-info/SOURCES.txt
```

