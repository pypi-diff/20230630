# Comparing `tmp/nics-1.0.0rc8.tar.gz` & `tmp/nics-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-asyza3eh/nics-1.0.0rc8.tar", last modified: Thu Jun 29 21:06:05 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-6dn_qnr6/nics-1.0.0rc9.tar", last modified: Thu Jun 29 21:12:50 2023, max compression
```

## Comparing `nics-1.0.0rc8.tar` & `nics-1.0.0rc9.tar`

### file list

```diff
@@ -1,36 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 21:05:48.000000 nics-1.0.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 21:05:48.000000 nics-1.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:06:05.000000 nics-1.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 21:05:48.000000 nics-1.0.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/main/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_404_and_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_sass_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/main/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/workflows_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-29 21:05:48.000000 nics-1.0.0rc8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 21:06:05.000000 nics-1.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 21:05:48.000000 nics-1.0.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 21:12:33.000000 nics-1.0.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 21:12:33.000000 nics-1.0.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:12:50.000000 nics-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 21:12:33.000000 nics-1.0.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/404.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/assets/nics-logo500.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/2 -- Bar -- bar/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-29 21:12:33.000000 nics-1.0.0rc9/nics/main/wizard/workflows_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 21:12:50.000000 nics-1.0.0rc9/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-29 21:12:33.000000 nics-1.0.0rc9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 21:12:50.000000 nics-1.0.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 21:12:33.000000 nics-1.0.0rc9/setup.py
```

### Comparing `nics-1.0.0rc8/LICENSE` & `nics-1.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/PKG-INFO` & `nics-1.0.0rc9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc8/nics/main/__init__.py` & `nics-1.0.0rc9/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/__init__.py` & `nics-1.0.0rc9/nics/main/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/copying_template.py` & `nics-1.0.0rc9/nics/main/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/inspect.py` & `nics-1.0.0rc9/nics/main/compile/inspect.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/update_404_and_favicon.py` & `nics-1.0.0rc9/nics/main/compile/update_404_and_favicon.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/update_docs_tree.py` & `nics-1.0.0rc9/nics/main/compile/update_docs_tree.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/update_header.py` & `nics-1.0.0rc9/nics/main/compile/update_header.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/compile/update_jekyll_config.py` & `nics-1.0.0rc9/nics/main/compile/update_jekyll_config.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/constants.py` & `nics-1.0.0rc9/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/wizard/__init__.py` & `nics-1.0.0rc9/nics/main/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/wizard/inspect.py` & `nics-1.0.0rc9/nics/main/wizard/inspect.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/wizard/settings_writer.py` & `nics-1.0.0rc9/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics/main/wizard/workflows_writer.py` & `nics-1.0.0rc9/nics/main/wizard/workflows_writer.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc8/nics.egg-info/PKG-INFO` & `nics-1.0.0rc9/nics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc8/pyproject.toml` & `nics-1.0.0rc9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "1.0.0rc8"
+version = "1.0.0rc9"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

