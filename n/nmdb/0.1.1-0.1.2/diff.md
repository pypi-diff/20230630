# Comparing `tmp/nmdb-0.1.1.tar.gz` & `tmp/nmdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmdb-0.1.1.tar", last modified: Fri Jun 30 11:25:08 2023, max compression
+gzip compressed data, was "nmdb-0.1.2.tar", last modified: Fri Jun 30 15:14:28 2023, max compression
```

## Comparing `nmdb-0.1.1.tar` & `nmdb-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/
--rw-r--r--   0 steigies  (3114) steigies  (3114)      678 2023-06-29 13:29:12.000000 nmdb-0.1.1/LICENSE.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)     2713 2023-06-30 11:25:08.608123 nmdb-0.1.1/PKG-INFO
--rw-r--r--   0 steigies  (3114) steigies  (3114)      831 2023-06-30 11:12:49.000000 nmdb-0.1.1/README.md
--rw-r--r--   0 steigies  (3114) steigies  (3114)     2559 2023-06-30 11:24:36.000000 nmdb-0.1.1/pyproject.toml
--rw-r--r--   0 steigies  (3114) steigies  (3114)       38 2023-06-30 11:25:08.608123 nmdb-0.1.1/setup.cfg
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.604123 nmdb-0.1.1/src/
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/
--rw-r--r--   0 steigies  (3114) steigies  (3114)      107 2023-06-28 15:44:30.000000 nmdb-0.1.1/src/nmdb/.nmdbrc
--rw-r--r--   0 steigies  (3114) steigies  (3114)      108 2023-06-28 11:42:04.000000 nmdb-0.1.1/src/nmdb/__init__.py
--rw-r--r--   0 steigies  (3114) steigies  (3114)     4807 2023-01-15 19:24:36.000000 nmdb-0.1.1/src/nmdb/nest.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/nest_multi/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     1516 2023-06-29 15:26:28.000000 nmdb-0.1.1/src/nmdb/nest_multi/__init__.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/nest_single/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     1615 2023-06-29 15:26:48.000000 nmdb-0.1.1/src/nmdb/nest_single/__init__.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb/realtime/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     1487 2023-06-29 15:23:39.000000 nmdb-0.1.1/src/nmdb/realtime/__init__.py
-drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 11:25:08.608123 nmdb-0.1.1/src/nmdb.egg-info/
--rw-r--r--   0 steigies  (3114) steigies  (3114)     2713 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/PKG-INFO
--rw-r--r--   0 steigies  (3114) steigies  (3114)      380 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/SOURCES.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)        1 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/dependency_links.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)      150 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/entry_points.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)       55 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/requires.txt
--rw-r--r--   0 steigies  (3114) steigies  (3114)        5 2023-06-30 11:25:08.000000 nmdb-0.1.1/src/nmdb.egg-info/top_level.txt
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      678 2023-06-29 13:29:12.000000 nmdb-0.1.2/LICENSE.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2984 2023-06-30 15:14:28.884425 nmdb-0.1.2/PKG-INFO
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1102 2023-06-30 15:14:16.000000 nmdb-0.1.2/README.md
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2631 2023-06-30 15:13:48.000000 nmdb-0.1.2/pyproject.toml
+-rw-r--r--   0 steigies  (3114) steigies  (3114)       38 2023-06-30 15:14:28.884425 nmdb-0.1.2/setup.cfg
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/nmdb/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      107 2023-06-28 15:44:30.000000 nmdb-0.1.2/src/nmdb/.nmdbrc
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      108 2023-06-28 11:42:04.000000 nmdb-0.1.2/src/nmdb/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/nmdb/conf2022/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2015 2023-06-30 15:07:26.000000 nmdb-0.1.2/src/nmdb/conf2022/__init__.py
+-rw-r--r--   0 steigies  (3114) steigies  (3114)   101351 2023-06-30 14:05:55.000000 nmdb-0.1.2/src/nmdb/conf2022/gle70.dat
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     4807 2023-01-15 19:24:36.000000 nmdb-0.1.2/src/nmdb/nest.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/nmdb/nest_multi/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1516 2023-06-29 15:26:28.000000 nmdb-0.1.2/src/nmdb/nest_multi/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/nmdb/nest_single/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1615 2023-06-29 15:26:48.000000 nmdb-0.1.2/src/nmdb/nest_single/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/nmdb/realtime/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     1487 2023-06-29 15:23:39.000000 nmdb-0.1.2/src/nmdb/realtime/__init__.py
+drwxr-xr-x   0 steigies  (3114) steigies  (3114)        0 2023-06-30 15:14:28.884425 nmdb-0.1.2/src/nmdb.egg-info/
+-rw-r--r--   0 steigies  (3114) steigies  (3114)     2984 2023-06-30 15:14:28.000000 nmdb-0.1.2/src/nmdb.egg-info/PKG-INFO
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      438 2023-06-30 15:14:28.000000 nmdb-0.1.2/src/nmdb.egg-info/SOURCES.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)        1 2023-06-30 15:14:28.000000 nmdb-0.1.2/src/nmdb.egg-info/dependency_links.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)      185 2023-06-30 15:14:28.000000 nmdb-0.1.2/src/nmdb.egg-info/entry_points.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)       63 2023-06-30 15:14:28.000000 nmdb-0.1.2/src/nmdb.egg-info/requires.txt
+-rw-r--r--   0 steigies  (3114) steigies  (3114)        5 2023-06-30 15:14:28.000000 nmdb-0.1.2/src/nmdb.egg-info/top_level.txt
```

### Comparing `nmdb-0.1.1/LICENSE.txt` & `nmdb-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.1/PKG-INFO` & `nmdb-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python examples to access data from the Neutron Monitor database
 Author-email: "Christian T. Steigies" <steigies@nmdb.eu>
 Maintainer-email: "Christian T. Steigies" <steigies@nmdb.eu>
 License: Copyright (C) 2008-2023 Christian T. Steigies <steigies@nmdb.eu>
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
@@ -58,14 +58,18 @@
 - `nmdb_realtime` is an example to access realtime data,
 as presented in a [tutorial][realtime] at the [NMDB hybrid conference in 2022][conf2022].
 
 - `nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
 [NEST][nest] interface into a pandas dataframe.
 These examples use the nest module from the nmdb package to generate html strings to query NEST.
 
+- `nmdb_conf2022` is the script that creates the coverpage plot for the 2022 NMDB conference.
+The plot shows GLE70 data as downloaded from NMDB 
+(with the data header manually edited so that the data can be read easily with pandas). 
+The plots are created using seaborn.
 
 --- 
 
 [nmdb]: https://nmdb.eu
 [realtime]: https://conf2022.nmdb.eu/abstract/s6/steigies/
 [conf2022]: https://conf2022.nmdb.eu
 [nest]: https://www.nmdb.eu/nest/
```

### Comparing `nmdb-0.1.1/pyproject.toml` & `nmdb-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nmdb"  # Required
-version = "0.1.1"
+version = "0.1.2"
 description = "Python examples to access data from the Neutron Monitor database"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["cosmic rays", "database"] 
 authors = [
   {name = "Christian T. Steigies", email = "steigies@nmdb.eu" }
@@ -43,14 +43,15 @@
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
   "datetime",
 #  "mysqlclient",
   "pandas",
+  "seaborn",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
@@ -66,14 +67,15 @@
 "Source" = "https://github.com/steigies/nmdb/"
 
 [project.scripts]
 nmdb = "nmdb:main"
 nmdb_nest_single = "nmdb.nest_single:main"
 nmdb_nest_multi = "nmdb.nest_multi:main"
 nmdb_realtime = "nmdb.realtime:main"
+nmdb_conf2022 = "nmdb.conf2022:main"
 
 [tool.setuptools]
-package-data = {"nmdb" = [".nmdbrc"]}
+package-data = {"nmdb" = [".nmdbrc", "conf2022/gle70.dat"]}
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `nmdb-0.1.1/src/nmdb/nest.py` & `nmdb-0.1.2/src/nmdb/nest.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.1/src/nmdb/nest_multi/__init__.py` & `nmdb-0.1.2/src/nmdb/nest_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.1/src/nmdb/nest_single/__init__.py` & `nmdb-0.1.2/src/nmdb/nest_single/__init__.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.1/src/nmdb/realtime/__init__.py` & `nmdb-0.1.2/src/nmdb/realtime/__init__.py`

 * *Files identical despite different names*

### Comparing `nmdb-0.1.1/src/nmdb.egg-info/PKG-INFO` & `nmdb-0.1.2/src/nmdb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python examples to access data from the Neutron Monitor database
 Author-email: "Christian T. Steigies" <steigies@nmdb.eu>
 Maintainer-email: "Christian T. Steigies" <steigies@nmdb.eu>
 License: Copyright (C) 2008-2023 Christian T. Steigies <steigies@nmdb.eu>
         
         This program is free software: you can redistribute it and/or modify
         it under the terms of the GNU General Public License as published by
@@ -58,14 +58,18 @@
 - `nmdb_realtime` is an example to access realtime data,
 as presented in a [tutorial][realtime] at the [NMDB hybrid conference in 2022][conf2022].
 
 - `nmdb_nest_single` and `nmdb_nest_multi` are examples to get data from the
 [NEST][nest] interface into a pandas dataframe.
 These examples use the nest module from the nmdb package to generate html strings to query NEST.
 
+- `nmdb_conf2022` is the script that creates the coverpage plot for the 2022 NMDB conference.
+The plot shows GLE70 data as downloaded from NMDB 
+(with the data header manually edited so that the data can be read easily with pandas). 
+The plots are created using seaborn.
 
 --- 
 
 [nmdb]: https://nmdb.eu
 [realtime]: https://conf2022.nmdb.eu/abstract/s6/steigies/
 [conf2022]: https://conf2022.nmdb.eu
 [nest]: https://www.nmdb.eu/nest/
```

