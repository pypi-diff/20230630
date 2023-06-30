# Comparing `tmp/fonttoolsWB-0.2.0.tar.gz` & `tmp/fonttoolsWB-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonttoolsWB-0.2.0.tar", last modified: Mon Jun 12 15:42:34 2023, max compression
+gzip compressed data, was "fonttoolsWB-0.2.1.tar", last modified: Fri Jun 30 15:55:34 2023, max compression
```

## Comparing `fonttoolsWB-0.2.0.tar` & `fonttoolsWB-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.765546 fonttoolsWB-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.761546 fonttoolsWB-0.2.0/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.763546 fonttoolsWB-0.2.0/Lib/fonttoolsWB/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.765546 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/application.yml
--rw-rw-rw-   0 root         (0) root         (0)     2379 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/firstRun.py
--rw-rw-rw-   0 root         (0) root         (0)     9767 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/splashscreen.png
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.764546 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2641 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2641 2023-06-12 15:42:34.765546 fonttoolsWB-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-06-12 15:42:34.766546 fonttoolsWB-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:55:34.282737 fonttoolsWB-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:55:34.279737 fonttoolsWB-0.2.1/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:55:34.280737 fonttoolsWB-0.2.1/Lib/fonttoolsWB/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:55:34.281737 fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/application.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/firstRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     9767 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/splashscreen.png
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:55:34.281737 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-30 15:55:34.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-30 15:55:34.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:55:34.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-30 15:55:34.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-30 15:55:34.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-30 15:55:34.000000 fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-30 15:55:34.282737 fonttoolsWB-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2023-06-30 15:55:34.282737 fonttoolsWB-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-30 15:55:32.000000 fonttoolsWB-0.2.1/setup.py
```

### Comparing `fonttoolsWB-0.2.0/LICENSE` & `fonttoolsWB-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/application.yml` & `fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/application.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,7 +18,9 @@
   Installation: default
 - Name: uitools
   Installation: default
 - Name: widgetinspector
   Installation: optional
 - Name: namespace
   Installation: optional
+- Name: htmlpanel
+  Installation: optional
```

### Comparing `fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/firstRun.py` & `fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/firstRun.py`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/splashscreen.png` & `fonttoolsWB-0.2.1/Lib/fonttoolsWB/data/splashscreen.png`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/PKG-INFO` & `fonttoolsWB-0.2.1/Lib/fonttoolsWB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.2.0
+Version: 0.2.1
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
```

### Comparing `fonttoolsWB-0.2.0/PKG-INFO` & `fonttoolsWB-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.2.0
+Version: 0.2.1
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
```

### Comparing `fonttoolsWB-0.2.0/README.md` & `fonttoolsWB-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.0/setup.cfg` & `fonttoolsWB-0.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.1
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -56,26 +56,27 @@
 
 [options]
 packages = find:
 package_dir = 
 	=Lib
 python_requires = >=3.8
 install_requires = 
-	wbBase>=0.2
-	wbpFonttools>=0.2
+	wbBase>=0.2.2
+	wbpFonttools>=0.2.1
 	wbpLoglist>=0.2
 	wbpOutput>=0.2
 	wbpShell>=0.2
 	wbpTextedit>=0.2
 	wbpUItools>=0.2
 
 [options.extras_require]
 develop = 
 	wbpNamespace>=0.2
 	wbpWidgetinspector>=0.2
+	wbpHTMLpanel>=0.2.3
 
 [options.packages.find]
 where = Lib
 
 [options.package_data]
 fonttoolsWB.data = 
 	splashscreen.png
```

