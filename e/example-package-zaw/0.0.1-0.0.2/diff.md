# Comparing `tmp/example_package_zaw-0.0.1.tar.gz` & `tmp/example_package_zaw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_zaw-0.0.1.tar", last modified: Thu Jun 29 20:12:39 2023, max compression
+gzip compressed data, was "example_package_zaw-0.0.2.tar", last modified: Thu Jun 29 22:28:46 2023, max compression
```

## Comparing `example_package_zaw-0.0.1.tar` & `example_package_zaw-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:12:39.930455 example_package_zaw-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-06-29 20:07:08.000000 example_package_zaw-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      528 2023-06-29 20:12:39.930455 example_package_zaw-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-29 20:00:06.000000 example_package_zaw-0.0.1/README.md
--rw-rw-rw-   0        0        0      610 2023-06-29 20:12:21.000000 example_package_zaw-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 20:12:39.930455 example_package_zaw-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 20:12:39.930455 example_package_zaw-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 20:12:39.930455 example_package_zaw-0.0.1/src/example_package_zaw/
--rw-rw-rw-   0        0        0        0 2023-06-29 19:58:18.000000 example_package_zaw-0.0.1/src/example_package_zaw/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-29 19:58:48.000000 example_package_zaw-0.0.1/src/example_package_zaw/example.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:12:39.930455 example_package_zaw-0.0.1/src/example_package_zaw.egg-info/
--rw-rw-rw-   0        0        0      528 2023-06-29 20:12:39.000000 example_package_zaw-0.0.1/src/example_package_zaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-29 20:12:39.000000 example_package_zaw-0.0.1/src/example_package_zaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:12:39.000000 example_package_zaw-0.0.1/src/example_package_zaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-29 20:12:39.000000 example_package_zaw-0.0.1/src/example_package_zaw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:46.358945 example_package_zaw-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-29 20:07:08.000000 example_package_zaw-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-06-29 21:03:13.000000 example_package_zaw-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      528 2023-06-29 22:28:46.358945 example_package_zaw-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-29 20:00:06.000000 example_package_zaw-0.0.2/README.md
+-rw-rw-rw-   0        0        0      861 2023-06-29 22:28:11.000000 example_package_zaw-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-06-05 20:11:51.000000 example_package_zaw-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 22:28:46.358945 example_package_zaw-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:46.336686 example_package_zaw-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:46.343303 example_package_zaw-0.0.2/src/example_package_zaw/
+-rw-rw-rw-   0        0        0        0 2023-06-29 22:28:20.000000 example_package_zaw-0.0.2/src/example_package_zaw/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-06-29 22:22:41.000000 example_package_zaw-0.0.2/src/example_package_zaw/__main__.py
+-rw-rw-rw-   0        0        0     1853 2023-06-29 21:14:09.000000 example_package_zaw-0.0.2/src/example_package_zaw/example.py
+-rw-rw-rw-   0        0        0     1559 2023-06-06 00:13:47.000000 example_package_zaw-0.0.2/src/example_package_zaw/indi_va_table_template.html
+-rw-rw-rw-   0        0        0     5899 2023-05-25 22:08:09.000000 example_package_zaw-0.0.2/src/example_package_zaw/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0     2426 2023-06-07 04:09:05.000000 example_package_zaw-0.0.2/src/example_package_zaw/simpler_plot_config.json
+-rw-rw-rw-   0        0        0     2379 2023-06-06 00:21:59.000000 example_package_zaw-0.0.2/src/example_package_zaw/sum_va_table_template.html
+drwxrwxrwx   0        0        0        0 2023-06-29 22:28:46.358945 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/
+-rw-rw-rw-   0        0        0      528 2023-06-29 22:28:46.000000 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-06-29 22:28:46.000000 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 22:28:46.000000 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-29 22:28:46.000000 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 22:28:46.000000 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-29 22:28:46.000000 example_package_zaw-0.0.2/src/example_package_zaw.egg-info/top_level.txt
```

### Comparing `example_package_zaw-0.0.1/LICENSE` & `example_package_zaw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_zaw-0.0.1/PKG-INFO` & `example_package_zaw-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_zaw
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Zaw <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `example_package_zaw-0.0.1/src/example_package_zaw.egg-info/PKG-INFO` & `example_package_zaw-0.0.2/src/example_package_zaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-package-zaw
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Zaw <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

