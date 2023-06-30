# Comparing `tmp/bids-validator-1.9.9.tar.gz` & `tmp/bids-validator-1.9.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bids-validator-1.9.9.tar", last modified: Mon Oct  3 16:21:27 2022, max compression
+gzip compressed data, was "bids-validator-1.9.9.dev0.tar", last modified: Thu Sep  1 18:46:20 2022, max compression
```

## Comparing `bids-validator-1.9.9.tar` & `bids-validator-1.9.9.dev0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 16:21:27.723331 bids-validator-1.9.9/
--rw-r--r--   0 root         (0) root         (0)     1128 2022-10-03 16:20:55.000000 bids-validator-1.9.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       95 2022-10-03 16:20:55.000000 bids-validator-1.9.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    38413 2022-10-03 16:21:27.723331 bids-validator-1.9.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    37698 2022-10-03 16:20:55.000000 bids-validator-1.9.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 16:21:27.723331 bids-validator-1.9.9/bids_validator/
--rw-r--r--   0 root         (0) root         (0)      187 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-10-03 16:21:27.723331 bids-validator-1.9.9/bids_validator/_version.py
--rw-r--r--   0 root         (0) root         (0)     5876 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/bids_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 16:21:27.723331 bids-validator-1.9.9/bids_validator/rules/
--rw-r--r--   0 root         (0) root         (0)      256 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/rules/associated_data_rules.json
--rw-r--r--   0 root         (0) root         (0)    21273 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/rules/file_level_rules.json
--rw-r--r--   0 root         (0) root         (0)      103 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/rules/phenotypic_rules.json
--rw-r--r--   0 root         (0) root         (0)     7156 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/rules/session_level_rules.json
--rw-r--r--   0 root         (0) root         (0)      212 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/rules/subject_level_rules.json
--rw-r--r--   0 root         (0) root         (0)     5314 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/rules/top_level_rules.json
--rw-r--r--   0 root         (0) root         (0)     1432 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/test_bids_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 16:21:27.723331 bids-validator-1.9.9/bids_validator/tsv/
--rw-r--r--   0 root         (0) root         (0)     1538 2022-10-03 16:20:55.000000 bids-validator-1.9.9/bids_validator/tsv/non_custom_columns.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-03 16:21:27.719331 bids-validator-1.9.9/bids_validator.egg-info/
--rw-r--r--   0 root         (0) root         (0)    38413 2022-10-03 16:21:27.000000 bids-validator-1.9.9/bids_validator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      650 2022-10-03 16:21:27.000000 bids-validator-1.9.9/bids_validator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-03 16:21:27.000000 bids-validator-1.9.9/bids_validator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-10-03 16:21:27.000000 bids-validator-1.9.9/bids_validator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1085 2022-10-03 16:21:27.723331 bids-validator-1.9.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      152 2022-10-03 16:20:55.000000 bids-validator-1.9.9/setup.py
--rw-r--r--   0 root         (0) root         (0)    78252 2022-10-03 16:20:55.000000 bids-validator-1.9.9/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/
+-rw-r--r--   0 root         (0) root         (0)     1128 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       95 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    38418 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    37698 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/bids_validator/
+-rw-r--r--   0 root         (0) root         (0)      187 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      503 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/bids_validator/_version.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/bids_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/bids_validator/rules/
+-rw-r--r--   0 root         (0) root         (0)      256 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/rules/associated_data_rules.json
+-rw-r--r--   0 root         (0) root         (0)    21273 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/rules/file_level_rules.json
+-rw-r--r--   0 root         (0) root         (0)      103 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/rules/phenotypic_rules.json
+-rw-r--r--   0 root         (0) root         (0)     7156 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/rules/session_level_rules.json
+-rw-r--r--   0 root         (0) root         (0)      212 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/rules/subject_level_rules.json
+-rw-r--r--   0 root         (0) root         (0)     5314 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/rules/top_level_rules.json
+-rw-r--r--   0 root         (0) root         (0)     1432 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/test_bids_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/bids_validator/tsv/
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/bids_validator/tsv/non_custom_columns.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/bids_validator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    38418 2022-09-01 18:46:20.000000 bids-validator-1.9.9.dev0/bids_validator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      650 2022-09-01 18:46:20.000000 bids-validator-1.9.9.dev0/bids_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-01 18:46:20.000000 bids-validator-1.9.9.dev0/bids_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-09-01 18:46:20.000000 bids-validator-1.9.9.dev0/bids_validator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1085 2022-09-01 18:46:20.406951 bids-validator-1.9.9.dev0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      152 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/setup.py
+-rw-r--r--   0 root         (0) root         (0)    78252 2022-09-01 18:45:57.000000 bids-validator-1.9.9.dev0/versioneer.py
```

### Comparing `bids-validator-1.9.9/LICENSE` & `bids-validator-1.9.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/PKG-INFO` & `bids-validator-1.9.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bids-validator
-Version: 1.9.9
+Version: 1.9.9.dev0
 Summary: Validator for the Brain Imaging Data Structure
 Home-page: https://github.com/bids-standard/bids-validator
 Author: PyBIDS developers
 Author-email: bids-discussion@googlegroups.com
 Maintainer: BIDS Developers
 Maintainer-email: bids-discussion@googlegroups.com
 License: MIT
```

### Comparing `bids-validator-1.9.9/README.md` & `bids-validator-1.9.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator/bids_validator.py` & `bids-validator-1.9.9.dev0/bids_validator/bids_validator.py`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator/rules/file_level_rules.json` & `bids-validator-1.9.9.dev0/bids_validator/rules/file_level_rules.json`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator/rules/session_level_rules.json` & `bids-validator-1.9.9.dev0/bids_validator/rules/session_level_rules.json`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator/rules/top_level_rules.json` & `bids-validator-1.9.9.dev0/bids_validator/rules/top_level_rules.json`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator/test_bids_validator.py` & `bids-validator-1.9.9.dev0/bids_validator/test_bids_validator.py`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator/tsv/non_custom_columns.json` & `bids-validator-1.9.9.dev0/bids_validator/tsv/non_custom_columns.json`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/bids_validator.egg-info/PKG-INFO` & `bids-validator-1.9.9.dev0/bids_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bids-validator
-Version: 1.9.9
+Version: 1.9.9.dev0
 Summary: Validator for the Brain Imaging Data Structure
 Home-page: https://github.com/bids-standard/bids-validator
 Author: PyBIDS developers
 Author-email: bids-discussion@googlegroups.com
 Maintainer: BIDS Developers
 Maintainer-email: bids-discussion@googlegroups.com
 License: MIT
```

### Comparing `bids-validator-1.9.9/bids_validator.egg-info/SOURCES.txt` & `bids-validator-1.9.9.dev0/bids_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/setup.cfg` & `bids-validator-1.9.9.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bids-validator-1.9.9/versioneer.py` & `bids-validator-1.9.9.dev0/versioneer.py`

 * *Files identical despite different names*

