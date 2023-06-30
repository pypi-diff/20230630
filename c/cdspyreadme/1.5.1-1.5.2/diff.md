# Comparing `tmp/cdspyreadme-1.5.1.tar.gz` & `tmp/cdspyreadme-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdspyreadme-1.5.1.tar", last modified: Wed Jun  7 09:08:00 2023, max compression
+gzip compressed data, was "cdspyreadme-1.5.2.tar", last modified: Fri Jun 30 12:58:09 2023, max compression
```

## Comparing `cdspyreadme-1.5.1.tar` & `cdspyreadme-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/
--rw-r--r--   0 gilles.landais  (1382) gilles.landais  (1381)     1523 2021-02-25 08:29:36.000000 cdspyreadme-1.5.1/LICENSE.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     5135 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/PKG-INFO
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     4548 2022-03-21 17:27:54.000000 cdspyreadme-1.5.1/README.md
-drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/cdspyreadme/
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)    18391 2021-06-11 07:12:14.000000 cdspyreadme-1.5.1/cdspyreadme/CDSColumn.py
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      213 2021-04-30 10:20:23.000000 cdspyreadme-1.5.1/cdspyreadme/MRT.template
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      993 2022-06-01 07:50:01.000000 cdspyreadme-1.5.1/cdspyreadme/ReadMe.template
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      236 2023-06-07 08:59:15.000000 cdspyreadme-1.5.1/cdspyreadme/__init__.py
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      339 2021-02-25 08:29:19.000000 cdspyreadme-1.5.1/cdspyreadme/bytebybyte.template
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)    31325 2023-03-14 10:56:06.000000 cdspyreadme-1.5.1/cdspyreadme/core.py
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     6943 2023-06-07 08:57:54.000000 cdspyreadme-1.5.1/cdspyreadme/core_test.py
-drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/cdspyreadme.egg-info/
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     5135 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/PKG-INFO
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      398 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/SOURCES.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)        1 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/dependency_links.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       27 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/requires.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       12 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/top_level.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       67 2021-06-11 07:27:38.000000 cdspyreadme-1.5.1/pyproject.toml
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       38 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/setup.cfg
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     1091 2021-06-11 08:39:58.000000 cdspyreadme-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:09.670789 cdspyreadme-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-30 12:58:09.670789 cdspyreadme-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:09.666789 cdspyreadme-1.5.2/cdspyreadme/
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/CDSColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/MRT.template
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/ReadMe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/bytebybyte.template
+-rw-r--r--   0 runner    (1001) docker     (123)    31325 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/cdspyreadme/core_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:58:09.670789 cdspyreadme-1.5.2/cdspyreadme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-30 12:58:09.000000 cdspyreadme-1.5.2/cdspyreadme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-30 12:58:09.000000 cdspyreadme-1.5.2/cdspyreadme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:58:09.000000 cdspyreadme-1.5.2/cdspyreadme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 12:58:09.000000 cdspyreadme-1.5.2/cdspyreadme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 12:58:09.000000 cdspyreadme-1.5.2/cdspyreadme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 12:58:09.670789 cdspyreadme-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-30 12:57:49.000000 cdspyreadme-1.5.2/setup.py
```

### Comparing `cdspyreadme-1.5.1/LICENSE.txt` & `cdspyreadme-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5.1/PKG-INFO` & `cdspyreadme-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cdspyreadme
-Version: 1.5.1
+Version: 1.5.2
 Summary: ReadMe generator package (cdspyreadme)
 Home-page: https://github.com/cds-astro/cds.pyreadme
 Author: Gilles Landais (CDS)
-License: UNKNOWN
 Keywords: astronomy
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -194,9 +192,7 @@
 tablemaker = cdspyreadme.CDSTablesMaker()
 table = tablemaker.addTable(tab)
 
 tablemaker = cdspyreadme.CDSTablesMaker()
 table = tablemaker.addTable(tab)
 tablemaker.writeCDSTables()
 ```
-
-
```

### Comparing `cdspyreadme-1.5.1/README.md` & `cdspyreadme-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5.1/cdspyreadme/CDSColumn.py` & `cdspyreadme-1.5.2/cdspyreadme/CDSColumn.py`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5.1/cdspyreadme/ReadMe.template` & `cdspyreadme-1.5.2/cdspyreadme/ReadMe.template`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5.1/cdspyreadme/core.py` & `cdspyreadme-1.5.2/cdspyreadme/core.py`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5.1/cdspyreadme/core_test.py` & `cdspyreadme-1.5.2/cdspyreadme/core_test.py`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5.1/cdspyreadme.egg-info/PKG-INFO` & `cdspyreadme-1.5.2/cdspyreadme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cdspyreadme
-Version: 1.5.1
+Version: 1.5.2
 Summary: ReadMe generator package (cdspyreadme)
 Home-page: https://github.com/cds-astro/cds.pyreadme
 Author: Gilles Landais (CDS)
-License: UNKNOWN
 Keywords: astronomy
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -194,9 +192,7 @@
 tablemaker = cdspyreadme.CDSTablesMaker()
 table = tablemaker.addTable(tab)
 
 tablemaker = cdspyreadme.CDSTablesMaker()
 table = tablemaker.addTable(tab)
 tablemaker.writeCDSTables()
 ```
-
-
```

### Comparing `cdspyreadme-1.5.1/setup.py` & `cdspyreadme-1.5.2/setup.py`

 * *Files identical despite different names*

