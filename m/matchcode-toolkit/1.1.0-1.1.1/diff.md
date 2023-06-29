# Comparing `tmp/matchcode-toolkit-1.1.0.tar.gz` & `tmp/matchcode-toolkit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchcode-toolkit-1.1.0.tar", last modified: Fri Jun 23 01:01:05 2023, max compression
+gzip compressed data, was "matchcode-toolkit-1.1.1.tar", last modified: Thu Jun 29 22:05:39 2023, max compression
```

## Comparing `matchcode-toolkit-1.1.0.tar` & `matchcode-toolkit-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/
--rw-rw-r--   0 jono      (1000) jono      (1000)      104 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/AUTHORS.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      306 2023-06-23 00:59:25.000000 matchcode-toolkit-1.1.0/CHANGELOG.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      217 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/MANIFEST.in
--rw-rw-r--   0 jono      (1000) jono      (1000)      752 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/NOTICE
--rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)     2516 2023-06-06 00:27:30.000000 matchcode-toolkit-1.1.0/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/apache-2.0.LICENSE
--rw-rw-r--   0 jono      (1000) jono      (1000)      923 2023-06-23 01:01:01.000000 matchcode-toolkit-1.1.0/pyproject.toml
--rw-rw-r--   0 jono      (1000) jono      (1000)     1356 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/setup.cfg
--rw-rw-r--   0 jono      (1000) jono      (1000)       92 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/setup.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/src/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/src/matchcode_toolkit/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     4815 2023-06-22 23:11:27.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/fingerprinting.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2023-06-06 00:27:30.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/halohash.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-06-06 00:47:57.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     2461 2023-06-22 19:21:36.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2023-06-22 19:21:32.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit/plugin_fingerprint.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/
--rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)      764 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)      222 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-03-07 02:11:31.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 jono      (1000) jono      (1000)      165 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/requires.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       18 2023-06-23 01:01:05.000000 matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/tests/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4975 2023-06-22 19:21:39.000000 matchcode-toolkit-1.1.0/tests/test_fingerprinting.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.491279 matchcode-toolkit-1.1.0/tests/testfiles/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-23 01:01:05.495279 matchcode-toolkit-1.1.0/tests/testfiles/fingerprinting/
--rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      104 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/AUTHORS.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      404 2023-06-29 22:03:39.000000 matchcode-toolkit-1.1.1/CHANGELOG.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      217 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/MANIFEST.in
+-rw-rw-r--   0 jono      (1000) jono      (1000)      752 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/NOTICE
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2516 2023-06-06 00:27:30.000000 matchcode-toolkit-1.1.1/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)    11357 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/apache-2.0.LICENSE
+-rw-rw-r--   0 jono      (1000) jono      (1000)      923 2023-06-29 22:03:39.000000 matchcode-toolkit-1.1.1/pyproject.toml
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1356 2023-06-29 22:05:39.866454 matchcode-toolkit-1.1.1/setup.cfg
+-rw-rw-r--   0 jono      (1000) jono      (1000)       92 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/setup.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.858455 matchcode-toolkit-1.1.1/src/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/src/matchcode_toolkit/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4885 2023-06-29 22:03:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit/fingerprinting.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    14288 2023-06-06 00:27:30.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit/halohash.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/src/matchcode_toolkit/pipelines/
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2023-06-06 00:47:57.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit/pipelines/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2461 2023-06-29 22:03:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1445 2023-06-29 22:03:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit/plugin_fingerprint.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3186 2023-06-29 22:05:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)      764 2023-06-29 22:05:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-06-29 22:05:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)      222 2023-06-29 22:05:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2023-03-07 02:11:31.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 jono      (1000) jono      (1000)      165 2023-06-29 22:05:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       18 2023-06-29 22:05:39.000000 matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/tests/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4975 2023-06-29 22:03:39.000000 matchcode-toolkit-1.1.1/tests/test_fingerprinting.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/tests/testfiles/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2023-06-29 22:05:39.862455 matchcode-toolkit-1.1.1/tests/testfiles/fingerprinting/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4793 2023-04-13 19:04:55.000000 matchcode-toolkit-1.1.1/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json
```

### Comparing `matchcode-toolkit-1.1.0/NOTICE` & `matchcode-toolkit-1.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/PKG-INFO` & `matchcode-toolkit-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/purldb/tree/main/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `matchcode-toolkit-1.1.0/README.rst` & `matchcode-toolkit-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/apache-2.0.LICENSE` & `matchcode-toolkit-1.1.1/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/pyproject.toml` & `matchcode-toolkit-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "matchcode-toolkit"
-version = "1.1.0"
+version = "1.1.1"
 
 [build-system]
 requires = ["setuptools >= 50", "wheel", "setuptools_scm[toml] >= 6"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # this is used populated when creating a git archive
```

### Comparing `matchcode-toolkit-1.1.0/setup.cfg` & `matchcode-toolkit-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = matchcode-toolkit
-version = 1.1.0
+version = 1.1.1
 license = Apache-2.0
 description = matchcode-toolkit
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/nexB/purldb/tree/main/matchcode-toolkit
 author = nexB. Inc. and others
 author_email = info@aboutcode.org
```

### Comparing `matchcode-toolkit-1.1.0/src/matchcode_toolkit/fingerprinting.py` & `matchcode-toolkit-1.1.1/src/matchcode_toolkit/fingerprinting.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     return _create_directory_fingerprint(features)
 
 
 def _compute_directory_fingerprints(directory, codebase):
     """
     Compute fingerprints for `directory` from `codebase`
     """
-    children = [r for r in directory.walk(codebase) if r.is_file]
+    # We do not want to add empty files to our fingerprint
+    children = [r for r in directory.walk(codebase) if r.is_file and r.size]
     if len(children) == 1:
         return
 
     directory_content_fingerprint = create_content_fingerprint(children)
     if hasattr(directory, 'directory_content_fingerprint'):
         directory.directory_content_fingerprint = directory_content_fingerprint
     else:
```

### Comparing `matchcode-toolkit-1.1.0/src/matchcode_toolkit/halohash.py` & `matchcode-toolkit-1.1.1/src/matchcode_toolkit/halohash.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py` & `matchcode-toolkit-1.1.1/src/matchcode_toolkit/pipelines/scan_and_fingerprint_package.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/src/matchcode_toolkit/plugin_fingerprint.py` & `matchcode-toolkit-1.1.1/src/matchcode_toolkit/plugin_fingerprint.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/PKG-INFO` & `matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchcode-toolkit
-Version: 1.1.0
+Version: 1.1.1
 Summary: matchcode-toolkit
 Home-page: https://github.com/nexB/purldb/tree/main/matchcode-toolkit
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `matchcode-toolkit-1.1.0/src/matchcode_toolkit.egg-info/SOURCES.txt` & `matchcode-toolkit-1.1.1/src/matchcode_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/tests/test_fingerprinting.py` & `matchcode-toolkit-1.1.1/tests/test_fingerprinting.py`

 * *Files identical despite different names*

### Comparing `matchcode-toolkit-1.1.0/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json` & `matchcode-toolkit-1.1.1/tests/testfiles/fingerprinting/abbrev-1.0.3-i.json`

 * *Files identical despite different names*

