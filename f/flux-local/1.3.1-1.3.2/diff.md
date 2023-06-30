# Comparing `tmp/flux-local-1.3.1.tar.gz` & `tmp/flux-local-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-1.3.1.tar", last modified: Sun Jun 11 04:43:03 2023, max compression
+gzip compressed data, was "flux-local-1.3.2.tar", last modified: Fri Jun 30 03:36:11 2023, max compression
```

## Comparing `flux-local-1.3.1.tar` & `flux-local-1.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 04:42:53.000000 flux-local-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-11 04:43:03.138561 flux-local-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-11 04:42:53.000000 flux-local-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.134560 flux-local-1.3.1/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-11 04:42:53.000000 flux-local-1.3.1/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 04:43:03.000000 flux-local-1.3.1/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-11 04:43:03.138561 flux-local-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 04:42:53.000000 flux-local-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:43:03.138561 flux-local-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-11 04:42:53.000000 flux-local-1.3.1/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:36:11.320758 flux-local-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 03:35:57.000000 flux-local-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-30 03:36:11.320758 flux-local-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-30 03:35:57.000000 flux-local-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:36:11.316758 flux-local-1.3.2/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:36:11.320758 flux-local-1.3.2/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-30 03:35:57.000000 flux-local-1.3.2/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:36:11.316758 flux-local-1.3.2/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-30 03:36:11.000000 flux-local-1.3.2/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-30 03:36:11.000000 flux-local-1.3.2/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:36:11.000000 flux-local-1.3.2/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 03:36:11.000000 flux-local-1.3.2/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 03:36:11.000000 flux-local-1.3.2/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 03:36:11.000000 flux-local-1.3.2/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-30 03:36:11.320758 flux-local-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 03:35:57.000000 flux-local-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:36:11.320758 flux-local-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 03:35:57.000000 flux-local-1.3.2/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-30 03:35:57.000000 flux-local-1.3.2/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-30 03:35:57.000000 flux-local-1.3.2/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-30 03:35:57.000000 flux-local-1.3.2/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-30 03:35:57.000000 flux-local-1.3.2/tests/test_manifest.py
```

### Comparing `flux-local-1.3.1/LICENSE` & `flux-local-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/PKG-INFO` & `flux-local-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.3.1
+Version: 1.3.2
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-1.3.1/README.md` & `flux-local-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/command.py` & `flux-local-1.3.2/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/exceptions.py` & `flux-local-1.3.2/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/git_repo.py` & `flux-local-1.3.2/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/helm.py` & `flux-local-1.3.2/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/kustomize.py` & `flux-local-1.3.2/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/manifest.py` & `flux-local-1.3.2/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/build.py` & `flux-local-1.3.2/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/diff.py` & `flux-local-1.3.2/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/flux_local.py` & `flux-local-1.3.2/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/format.py` & `flux-local-1.3.2/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/get.py` & `flux-local-1.3.2/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/selector.py` & `flux-local-1.3.2/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local/tool/test.py` & `flux-local-1.3.2/flux_local/tool/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,15 @@
         if test_path:
             parts = test_path.split("::")
             query.path.path = Path(parts[0])
 
             # If a real file path, then clear so it is not a test nodeid filter
             if test_path.startswith(".") or test_path.startswith("/"):
                 test_path = None
+        query.kustomization.namespace = query.cluster.namespace
         query.kustomization.skip_crds = True
         query.helm_release.enabled = enable_helm
         query.helm_release.namespace = None
         query.cluster_policy.enabled = enable_kyverno
         options = selector.options(**kwargs)
 
         nest_asyncio.apply()
```

### Comparing `flux-local-1.3.1/flux_local/tool/visitor.py` & `flux-local-1.3.2/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/flux_local.egg-info/PKG-INFO` & `flux-local-1.3.2/flux_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.3.1
+Version: 1.3.2
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-1.3.1/flux_local.egg-info/SOURCES.txt` & `flux-local-1.3.2/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/setup.cfg` & `flux-local-1.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 1.3.1
+version = 1.3.2
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-1.3.1/tests/test_command.py` & `flux-local-1.3.2/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/tests/test_git_repo.py` & `flux-local-1.3.2/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/tests/test_helm.py` & `flux-local-1.3.2/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/tests/test_kustomize.py` & `flux-local-1.3.2/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.3.1/tests/test_manifest.py` & `flux-local-1.3.2/tests/test_manifest.py`

 * *Files identical despite different names*

