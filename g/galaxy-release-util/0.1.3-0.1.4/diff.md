# Comparing `tmp/galaxy-release-util-0.1.3.tar.gz` & `tmp/galaxy-release-util-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-release-util-0.1.3.tar", last modified: Wed Jun 28 09:36:30 2023, max compression
+gzip compressed data, was "galaxy-release-util-0.1.4.tar", last modified: Fri Jun 30 20:40:16 2023, max compression
```

## Comparing `galaxy-release-util-0.1.3.tar` & `galaxy-release-util-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/galaxy_release_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/bootstrap_history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/galaxy_release_util/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/cli/release_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/github_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    26254 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/point_release.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/galaxy_release_util/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-28 09:36:30.000000 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-28 09:36:30.000000 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 09:36:30.000000 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-28 09:36:30.000000 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-28 09:36:30.000000 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-28 09:36:30.000000 galaxy-release-util-0.1.3/galaxy_release_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:36:30.409322 galaxy-release-util-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-28 09:36:20.000000 galaxy-release-util-0.1.3/tests/test_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:16.809409 galaxy-release-util-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-30 20:40:16.809409 galaxy-release-util-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:16.805409 galaxy-release-util-0.1.4/galaxy_release_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/bootstrap_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:16.809409 galaxy-release-util-0.1.4/galaxy_release_util/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/cli/release_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/point_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/galaxy_release_util/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:16.809409 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-30 20:40:16.000000 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 20:40:16.000000 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 20:40:16.000000 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 20:40:16.000000 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 20:40:16.000000 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 20:40:16.000000 galaxy-release-util-0.1.4/galaxy_release_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-30 20:40:16.809409 galaxy-release-util-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 20:40:16.809409 galaxy-release-util-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-30 20:40:06.000000 galaxy-release-util-0.1.4/tests/test_release.py
```

### Comparing `galaxy-release-util-0.1.3/LICENSE.txt` & `galaxy-release-util-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/PKG-INFO` & `galaxy-release-util-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,19 @@
 -------
 
 .. to_doc
 
 
 
 ------------------
+0.1.4 (30-06-2023)
+------------------
+* Skip empty prerelease changelog when parsing changelog
+
+------------------
 0.1.3 (28-06-2023)
 ------------------
 * Add step/checkbox on updating db revision identifier
 * Bootstrap history fixes
 
 ------------------
 0.1.2 (12-06-2023)
```

### Comparing `galaxy-release-util-0.1.3/README.rst` & `galaxy-release-util-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util/bootstrap_history.py` & `galaxy-release-util-0.1.4/galaxy_release_util/bootstrap_history.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util/cli/options.py` & `galaxy-release-util-0.1.4/galaxy_release_util/cli/options.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util/github_client.py` & `galaxy-release-util-0.1.4/galaxy_release_util/github_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util/metadata.py` & `galaxy-release-util-0.1.4/galaxy_release_util/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util/point_release.py` & `galaxy-release-util-0.1.4/galaxy_release_util/point_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def datetime_date(self) -> datetime.datetime:
         if self.date:
             return datetime.datetime.fromisoformat(self.date)
         raise Exception(f"Changelog item for version {self.version} is missing date.")
 
     @property
     def is_empty_devrelease(self):
-        return self.version.is_devrelease and not self.changes
+        return (self.version.is_devrelease or self.version.is_prerelease) and not self.changes
 
     def __str__(self) -> str:
         change_lines = "\n".join(self.changes)
         if self.date:
             version_line = f"{self.version} ({self.date})"
         else:
             version_line = str(self.version)
```

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util.egg-info/PKG-INFO` & `galaxy-release-util-0.1.4/galaxy_release_util.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,19 @@
 -------
 
 .. to_doc
 
 
 
 ------------------
+0.1.4 (30-06-2023)
+------------------
+* Skip empty prerelease changelog when parsing changelog
+
+------------------
 0.1.3 (28-06-2023)
 ------------------
 * Add step/checkbox on updating db revision identifier
 * Bootstrap history fixes
 
 ------------------
 0.1.2 (12-06-2023)
```

### Comparing `galaxy-release-util-0.1.3/galaxy_release_util.egg-info/SOURCES.txt` & `galaxy-release-util-0.1.4/galaxy_release_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.3/setup.cfg` & `galaxy-release-util-0.1.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-release-util
 url = https://github.com/galaxyproject/galaxy-release-util
-version = 0.1.3
+version = 0.1.4
 
 [options]
 include_package_data = True
 install_requires = 
 	build
 	click
 	docutils
```

### Comparing `galaxy-release-util-0.1.3/tests/test_release.py` & `galaxy-release-util-0.1.4/tests/test_release.py`

 * *Files identical despite different names*

