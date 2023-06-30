# Comparing `tmp/szh_toolbox-0.0.6.tar.gz` & `tmp/szh_toolbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szh_toolbox-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "szh_toolbox-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `szh_toolbox-0.0.6.tar` & `szh_toolbox-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       12 2023-06-29 04:49:53.240161 szh_toolbox-0.0.6/README.md
--rw-r--r--   0        0        0      664 2023-06-29 06:39:45.708070 szh_toolbox-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-06-29 06:35:42.398384 szh_toolbox-0.0.6/src/szh_toolbox/__init__.py
--rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.6/src/szh_toolbox/commond.py
--rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.6/src/szh_toolbox/namelist.py
--rw-r--r--   0        0        0     2793 2023-06-29 06:39:39.421182 szh_toolbox-0.0.6/src/szh_toolbox/namelistwps.py
--rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.6/src/szh_toolbox/test.py
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 szh_toolbox-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1202 2023-06-30 05:00:52.117540 szh_toolbox-0.0.7/README.md
+-rw-r--r--   0        0        0      691 2023-06-30 15:09:37.467679 szh_toolbox-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3509 2023-06-30 04:38:54.950176 szh_toolbox-0.0.7/src/szh_toolbox/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.7/src/szh_toolbox/commond.py
+-rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.7/src/szh_toolbox/namelist.py
+-rw-r--r--   0        0        0     2793 2023-06-29 06:39:39.421182 szh_toolbox-0.0.7/src/szh_toolbox/namelistwps.py
+-rw-r--r--   0        0        0     4028 2023-06-30 15:06:38.250074 szh_toolbox-0.0.7/src/szh_toolbox/noaa_download.py
+-rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.7/src/szh_toolbox/test.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 szh_toolbox-0.0.7/PKG-INFO
```

### Comparing `szh_toolbox-0.0.6/pyproject.toml` & `szh_toolbox-0.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["flit_core>=3.9"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "szh_toolbox"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
-  { name="Example Author", email="author@example.com" },
+  { name="szh", email="suo.zh@qq.com"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 greetc = "szh_toolbox.commond:main"
-stwps = "szh_toolbox.namelistwps:main"
+st-wps = "szh_toolbox.namelistwps:main"
+st-noaa = "szh_toolbox.noaa_download:main"
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `szh_toolbox-0.0.6/src/szh_toolbox/namelist.py` & `szh_toolbox-0.0.7/src/szh_toolbox/namelist.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.6/src/szh_toolbox/namelistwps.py` & `szh_toolbox-0.0.7/src/szh_toolbox/namelistwps.py`

 * *Files identical despite different names*

