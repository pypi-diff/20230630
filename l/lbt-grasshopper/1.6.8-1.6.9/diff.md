# Comparing `tmp/lbt-grasshopper-1.6.8.tar.gz` & `tmp/lbt-grasshopper-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbt-grasshopper-1.6.8.tar", last modified: Tue Feb  7 21:17:28 2023, max compression
+gzip compressed data, was "dist/lbt-grasshopper-1.6.9.tar", last modified: Wed Feb  8 02:24:29 2023, max compression
```

## Comparing `lbt-grasshopper-1.6.8.tar` & `lbt-grasshopper-1.6.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/CI_STATUS.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   730519 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/gradients.png
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/installer.gh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/lbt_grasshopper/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/pass_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/ruby-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-07 21:17:28.000000 lbt-grasshopper-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-02-07 21:16:21.000000 lbt-grasshopper-1.6.8/uninstaller.gh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/CI_STATUS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   730519 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/gradients.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/installer.gh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/lbt_grasshopper/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/pass_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/ruby-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-08 02:24:29.000000 lbt-grasshopper-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-02-08 02:23:14.000000 lbt-grasshopper-1.6.9/uninstaller.gh
```

### Comparing `lbt-grasshopper-1.6.8/.github/workflows/ci.yaml` & `lbt-grasshopper-1.6.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/.github/workflows/dependency-release.yaml` & `lbt-grasshopper-1.6.9/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/CI_STATUS.md` & `lbt-grasshopper-1.6.9/CI_STATUS.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/LICENSE` & `lbt-grasshopper-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/PKG-INFO` & `lbt-grasshopper-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.6.8
+Version: 1.6.9
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.6.8/README.md` & `lbt-grasshopper-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/gradients.png` & `lbt-grasshopper-1.6.9/gradients.png`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/installer.gh` & `lbt-grasshopper-1.6.9/installer.gh`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/lbt_grasshopper.egg-info/PKG-INFO` & `lbt-grasshopper-1.6.9/lbt_grasshopper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.6.8
+Version: 1.6.9
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.6.8/setup.py` & `lbt-grasshopper-1.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.6.8/uninstaller.gh` & `lbt-grasshopper-1.6.9/uninstaller.gh`

 * *Files identical despite different names*

