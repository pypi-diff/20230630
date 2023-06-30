# Comparing `tmp/nmdb-0.1.0.tar.gz` & `tmp/nmdb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmdb-0.1.0.tar", last modified: Thu Jun 29 15:27:53 2023, max compression
+gzip compressed data, was "nmdb-0.1.1.tar", last modified: Fri Jun 30 11:25:08 2023, max compression
```

## Comparing `nmdb-0.1.0.tar` & `nmdb-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.414962 nmdb-0.1.0/
--rw-r--r--   0 steigies  (3114) steigies  (3114)      678 2023-06-29 13:29:12.000000 nmdb-0.1.0/LICENSE.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)     2512 2023-06-29 15:27:53.414962 nmdb-0.1.0/PKG-INFO
--rw-r--r--   0 steigies  (3114) steigies  (3114)      637 2023-06-29 15:19:40.000000 nmdb-0.1.0/README.md
--rw-r--r--   0 steigies  (3114) steigies  (3114)     3374 2023-06-29 13:27:51.000000 nmdb-0.1.0/pyproject.toml
--rw-r--r--   0 steigies  (3114) steigies  (3114)       38 2023-06-29 15:27:53.414962 nmdb-0.1.0/setup.cfg
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.410962 nmdb-0.1.0/src/
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.414962 nmdb-0.1.0/src/nmdb/
--rw-r--r--   0 steigies  (3114) steigies  (3114)      107 2023-06-28 15:44:30.000000 nmdb-0.1.0/src/nmdb/.nmdbrc
--rw-r--r--   0 steigies  (3114) steigies  (3114)      108 2023-06-28 11:42:04.000000 nmdb-0.1.0/src/nmdb/__init__.py
--rw-r--r--   0 steigies  (3114) steigies  (3114)     4807 2023-01-15 19:24:36.000000 nmdb-0.1.0/src/nmdb/nest.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.414962 nmdb-0.1.0/src/nmdb.egg-info/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     2512 2023-06-29 15:27:53.000000 nmdb-0.1.0/src/nmdb.egg-info/PKG-INFO
--rw-r--r--   0 steigies  (3114) steigies  (3114)      380 2023-06-29 15:27:53.000000 nmdb-0.1.0/src/nmdb.egg-info/SOURCES.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)        1 2023-06-29 15:27:53.000000 nmdb-0.1.0/src/nmdb.egg-info/dependency_links.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)      150 2023-06-29 15:27:53.000000 nmdb-0.1.0/src/nmdb.egg-info/entry_points.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)       67 2023-06-29 15:27:53.000000 nmdb-0.1.0/src/nmdb.egg-info/requires.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)       52 2023-06-29 15:27:53.000000 nmdb-0.1.0/src/nmdb.egg-info/top_level.txt
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.414962 nmdb-0.1.0/src/nmdb_nest_multi/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     1516 2023-06-29 15:26:28.000000 nmdb-0.1.0/src/nmdb_nest_multi/__init__.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.414962 nmdb-0.1.0/src/nmdb_nest_single/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     1615 2023-06-29 15:26:48.000000 nmdb-0.1.0/src/nmdb_nest_single/__init__.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-29 15:27:53.414962 nmdb-0.1.0/src/nmdb_realtime/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     1487 2023-06-29 15:23:39.000000 nmdb-0.1.0/src/nmdb_realtime/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      678 2023-06-29 13:29:12.000000 nmdb-0.1.1/LICENSE.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2713 2023-06-30 11:25:08.608123 nmdb-0.1.1/PKG-INFO
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      831 2023-06-30 11:12:49.000000 nmdb-0.1.1/README.md
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2559 2023-06-30 11:24:36.000000 nmdb-0.1.1/pyproject.toml
+-rw-r--r--   0 steigies  (3114) steigies  (3114)       38 2023-06-30 11:25:08.608123 nmdb-0.1.1/setup.cfg
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.604123 nmdb-0.1.1/src/
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      107 2023-06-28 15:44:30.000000 nmdb-0.1.1/src/nmdb/.nmdbrc
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      108 2023-06-28 11:42:04.000000 nmdb-0.1.1/src/nmdb/__init__.py
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     4807 2023-01-15 19:24:36.000000 nmdb-0.1.1/src/nmdb/nest.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/nest_multi/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1516 2023-06-29 15:26:28.000000 nmdb-0.1.1/src/nmdb/nest_multi/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/nest_single/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1615 2023-06-29 15:26:48.000000 nmdb-0.1.1/src/nmdb/nest_single/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/realtime/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1487 2023-06-29 15:23:39.000000 nmdb-0.1.1/src/nmdb/realtime/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb.egg-info/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2713 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/PKG-INFO
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      380 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/SOURCES.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)        1 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/dependency_links.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      150 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/entry_points.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)       55 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/requires.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)        5 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/top_level.txt
```

### Comparing `nmdb-0.1.0/LICENSE.txt` & `nmdb-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.0/PKG-INFO` & `nmdb-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nmdb
-Version: 0.1.0
-Summary: Python examples to work with the Neutron Monitor database
+Version: 0.1.1
+Summary: Python examples to access data from the Neutron Monitor database
 Author-email: "Christian T. Steigies" <steigies@nmdb.eu>
 Maintainer-email: "Christian T. Steigies" <steigies@nmdb.eu>
 License: Copyright (C) 2008-2023 Christian T. Steigies <steigies@nmdb.eu>
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
@@ -39,24 +39,32 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Access the Neutron Monitor database with python
 
 ![NMDB Logo](https://www.nmdb.eu/img/nmdb-6.png "NMDB")
 
-The nmdb project provides python functions to access the
+This package provides python functions to access data from the
 [Neutron Monitor database][nmdb].
 
----
+# Installation
 
-`nmdb_realtime` is an example to access realtime data,
+You can install directly from PyPI using
+```
+pip install nmdb
+```
+
+# Usage
+
+- `nmdb_realtime` is an example to access realtime data,
 as presented in a [tutorial][realtime] at the [NMDB hybrid conference in 2022][conf2022].
 
-`nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
+- `nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
 [NEST][nest] interface into a pandas dataframe.
+These examples use the nest module from the nmdb package to generate html strings to query NEST.
 
 
 --- 
 
 [nmdb]: https://nmdb.eu
 [realtime]: https://conf2022.nmdb.eu/abstract/s6/steigies/
 [conf2022]: https://conf2022.nmdb.eu
```

### Comparing `nmdb-0.1.0/README.md` & `nmdb-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # Access the Neutron Monitor database with python
 
 ![NMDB Logo](https://www.nmdb.eu/img/nmdb-6.png "NMDB")
 
-The nmdb project provides python functions to access the
+This package provides python functions to access data from the
 [Neutron Monitor database][nmdb].
 
----
+# Installation
 
-`nmdb_realtime` is an example to access realtime data,
+You can install directly from PyPI using
+```
+pip install nmdb
+```
+
+# Usage
+
+- `nmdb_realtime` is an example to access realtime data,
 as presented in a [tutorial][realtime] at the [NMDB hybrid conference in 2022][conf2022].
 
-`nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
+- `nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
 [NEST][nest] interface into a pandas dataframe.
+These examples use the nest module from the nmdb package to generate html strings to query NEST.
 
 
 --- 
 
 [nmdb]: https://nmdb.eu
 [realtime]: https://conf2022.nmdb.eu/abstract/s6/steigies/
 [conf2022]: https://conf2022.nmdb.eu
```

### Comparing `nmdb-0.1.0/pyproject.toml` & `nmdb-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "nmdb"  # Required
-version = "0.1.0"
-description = "Python examples to work with the Neutron Monitor database"
+version = "0.1.1"
+description = "Python examples to access data from the Neutron Monitor database"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["cosmic rays", "database"] 
 authors = [
   {name = "Christian T. Steigies", email = "steigies@nmdb.eu" }
 ]
@@ -41,15 +41,15 @@
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
   "datetime",
-  "mysqlclient",
+#  "mysqlclient",
   "pandas",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
@@ -57,38 +57,23 @@
 #
 # Similar to `dependencies` above, these must be valid existing
 # projects.
 [project.optional-dependencies] # Optional
 dev = ["check-manifest"]
 test = ["coverage"]
 
-# List URLs that are relevant to your project
-#
-# This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
-# https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-# https://packaging.python.org/specifications/core-metadata/#home-page-optional
-#
-# Examples listed include a pattern for specifying where the package tracks
-# issues, where the source is hosted, where to say thanks to the package
-# maintainers, and where to support the project financially. The key is
-# what's used to render the link text on PyPI.
 [project.urls]  # Optional
-#"Homepage" = "https://github.com/pypa/sampleproject"
-#"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
-#"Funding" = "https://donate.pypi.org"
-#"Say Thanks!" = "http://saythanks.io/to/example"
-#"Source" = "https://github.com/pypa/sampleproject/"
 "Homepage" = "https://nmdb.eu"
 "Source" = "https://github.com/steigies/nmdb/"
 
 [project.scripts]
 nmdb = "nmdb:main"
-nmdb_nest_single = "nmdb_nest_single:main"
-nmdb_nest_multi = "nmdb_nest_multi:main"
-nmdb_realtime = "nmdb_realtime:main"
+nmdb_nest_single = "nmdb.nest_single:main"
+nmdb_nest_multi = "nmdb.nest_multi:main"
+nmdb_realtime = "nmdb.realtime:main"
 
 [tool.setuptools]
 package-data = {"nmdb" = [".nmdbrc"]}
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `nmdb-0.1.0/src/nmdb/nest.py` & `nmdb-0.1.1/src/nmdb/nest.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.0/src/nmdb.egg-info/PKG-INFO` & `nmdb-0.1.1/src/nmdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nmdb
-Version: 0.1.0
-Summary: Python examples to work with the Neutron Monitor database
+Version: 0.1.1
+Summary: Python examples to access data from the Neutron Monitor database
 Author-email: "Christian T. Steigies" <steigies@nmdb.eu>
 Maintainer-email: "Christian T. Steigies" <steigies@nmdb.eu>
 License: Copyright (C) 2008-2023 Christian T. Steigies <steigies@nmdb.eu>
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
         the Free Software Foundation, either version 3 of the License, or
@@ -39,24 +39,32 @@
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Access the Neutron Monitor database with python
 
 ![NMDB Logo](https://www.nmdb.eu/img/nmdb-6.png "NMDB")
 
-The nmdb project provides python functions to access the
+This package provides python functions to access data from the
 [Neutron Monitor database][nmdb].
 
----
+# Installation
 
-`nmdb_realtime` is an example to access realtime data,
+You can install directly from PyPI using
+```
+pip install nmdb
+```
+
+# Usage
+
+- `nmdb_realtime` is an example to access realtime data,
 as presented in a [tutorial][realtime] at the [NMDB hybrid conference in 2022][conf2022].
 
-`nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
+- `nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
 [NEST][nest] interface into a pandas dataframe.
+These examples use the nest module from the nmdb package to generate html strings to query NEST.
 
 
 --- 
 
 [nmdb]: https://nmdb.eu
 [realtime]: https://conf2022.nmdb.eu/abstract/s6/steigies/
 [conf2022]: https://conf2022.nmdb.eu
```

### Comparing `nmdb-0.1.0/src/nmdb_nest_multi/__init__.py` & `nmdb-0.1.1/src/nmdb/nest_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.0/src/nmdb_nest_single/__init__.py` & `nmdb-0.1.1/src/nmdb/nest_single/__init__.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.0/src/nmdb_realtime/__init__.py` & `nmdb-0.1.1/src/nmdb/realtime/__init__.py`

 * *Files identical despite different names*

