# Comparing `tmp/yea-wandb-0.9.8.tar.gz` & `tmp/yea-wandb-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yea-wandb-0.9.8.tar", last modified: Wed May 10 14:20:36 2023, max compression
+gzip compressed data, was "yea-wandb-0.9.9.tar", last modified: Thu May 25 18:15:25 2023, max compression
```

## Comparing `yea-wandb-0.9.8.tar` & `yea-wandb-0.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.877453 yea-wandb-0.9.8/
--rw-r--r--   0 jeff       (501) staff       (20)     1075 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/LICENSE
--rw-r--r--   0 jeff       (501) staff       (20)       58 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)      154 2023-05-10 14:20:36.877152 yea-wandb-0.9.8/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      885 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/README.md
--rw-r--r--   0 jeff       (501) staff       (20)      112 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/pyproject.toml
--rw-r--r--   0 jeff       (501) staff       (20)       38 2023-05-10 14:20:36.877647 yea-wandb-0.9.8/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)      543 2023-05-10 14:19:45.000000 yea-wandb-0.9.8/setup.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.855986 yea-wandb-0.9.8/src/
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.869980 yea-wandb-0.9.8/src/yea_wandb/
--rw-r--r--   0 jeff       (501) staff       (20)       68 2023-05-10 14:19:45.000000 yea-wandb-0.9.8/src/yea_wandb/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)     6163 2022-06-21 16:50:06.000000 yea-wandb-0.9.8/src/yea_wandb/artifact_emu.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     8703 2023-05-10 14:18:59.000000 yea-wandb-0.9.8/src/yea_wandb/backend.py
--rw-r--r--   0 jeff       (501) staff       (20)     1676 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/hook.py
--rw-r--r--   0 jeff       (501) staff       (20)     3486 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/mitm.py
--rw-r--r--   0 jeff       (501) staff       (20)     9312 2022-07-08 02:01:53.000000 yea-wandb-0.9.8/src/yea_wandb/mock_requests.py
--rw-r--r--   0 jeff       (501) staff       (20)   106220 2023-05-10 14:19:45.000000 yea-wandb-0.9.8/src/yea_wandb/mock_server.py
--rw-r--r--   0 jeff       (501) staff       (20)    10623 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/plugin.py
--rw-r--r--   0 jeff       (501) staff       (20)     4847 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/setup.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.876194 yea-wandb-0.9.8/src/yea_wandb.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)      154 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      545 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       43 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/not-zip-safe
--rw-r--r--   0 jeff       (501) staff       (20)       43 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)       10 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/top_level.txt
+drwxr-xr-x   0 szymon     (502) staff       (20)        0 2023-05-25 18:15:25.571685 yea-wandb-0.9.9/
+-rw-r--r--   0 szymon     (502) staff       (20)     1075 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/LICENSE
+-rw-r--r--   0 szymon     (502) staff       (20)       58 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/MANIFEST.in
+-rw-r--r--   0 szymon     (502) staff       (20)      154 2023-05-25 18:15:25.571533 yea-wandb-0.9.9/PKG-INFO
+-rw-r--r--   0 szymon     (502) staff       (20)      885 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/README.md
+-rw-r--r--   0 szymon     (502) staff       (20)      112 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/pyproject.toml
+-rw-r--r--   0 szymon     (502) staff       (20)       38 2023-05-25 18:15:25.571730 yea-wandb-0.9.9/setup.cfg
+-rw-r--r--   0 szymon     (502) staff       (20)      543 2023-05-25 15:41:32.000000 yea-wandb-0.9.9/setup.py
+drwxr-xr-x   0 szymon     (502) staff       (20)        0 2023-05-25 18:15:25.566998 yea-wandb-0.9.9/src/
+drwxr-xr-x   0 szymon     (502) staff       (20)        0 2023-05-25 18:15:25.570279 yea-wandb-0.9.9/src/yea_wandb/
+-rw-r--r--   0 szymon     (502) staff       (20)       68 2023-05-25 15:41:32.000000 yea-wandb-0.9.9/src/yea_wandb/__init__.py
+-rw-r--r--   0 szymon     (502) staff       (20)     6163 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/artifact_emu.py
+-rwxr-xr-x   0 szymon     (502) staff       (20)     8703 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/backend.py
+-rw-r--r--   0 szymon     (502) staff       (20)     1676 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/hook.py
+-rw-r--r--   0 szymon     (502) staff       (20)     3486 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/mitm.py
+-rw-r--r--   0 szymon     (502) staff       (20)     9312 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/mock_requests.py
+-rw-r--r--   0 szymon     (502) staff       (20)   106331 2023-05-25 15:41:32.000000 yea-wandb-0.9.9/src/yea_wandb/mock_server.py
+-rw-r--r--   0 szymon     (502) staff       (20)    10623 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/plugin.py
+-rw-r--r--   0 szymon     (502) staff       (20)     4847 2023-05-12 10:10:25.000000 yea-wandb-0.9.9/src/yea_wandb/setup.py
+drwxr-xr-x   0 szymon     (502) staff       (20)        0 2023-05-25 18:15:25.571321 yea-wandb-0.9.9/src/yea_wandb.egg-info/
+-rw-r--r--   0 szymon     (502) staff       (20)      154 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 szymon     (502) staff       (20)      545 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 szymon     (502) staff       (20)        1 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 szymon     (502) staff       (20)       43 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/entry_points.txt
+-rw-r--r--   0 szymon     (502) staff       (20)        1 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 szymon     (502) staff       (20)       43 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/requires.txt
+-rw-r--r--   0 szymon     (502) staff       (20)       10 2023-05-25 18:15:25.000000 yea-wandb-0.9.9/src/yea_wandb.egg-info/top_level.txt
```

### Comparing `yea-wandb-0.9.8/LICENSE` & `yea-wandb-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/README.md` & `yea-wandb-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/setup.py` & `yea-wandb-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """yea setup."""
 
 from setuptools import setup
 
 
 setup(
     name="yea-wandb",
-    version="0.9.8",
+    version="0.9.9",
     description="Test harness wandb plugin",
     packages=["yea_wandb"],
     install_requires=[
         "Flask",
         "requests",
         "responses",
         "pandas",
```

### Comparing `yea-wandb-0.9.8/src/yea_wandb/artifact_emu.py` & `yea-wandb-0.9.9/src/yea_wandb/artifact_emu.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb/backend.py` & `yea-wandb-0.9.9/src/yea_wandb/backend.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb/hook.py` & `yea-wandb-0.9.9/src/yea_wandb/hook.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb/mitm.py` & `yea-wandb-0.9.9/src/yea_wandb/mitm.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb/mock_requests.py` & `yea-wandb-0.9.9/src/yea_wandb/mock_requests.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb/mock_server.py` & `yea-wandb-0.9.9/src/yea_wandb/mock_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,22 +113,25 @@
     app = create_app(ctx)
     mock = RequestsMock(app, ctx)
     # We mock out all requests libraries, couldn't find a way to mock the core lib
     sdk_path = "wandb.sdk"
     # From previous wandb_gql transport library.
     mocker.patch("wandb_gql.transport.requests.requests", mock)
 
+    mocker.patch("wandb.sdk.artifacts.public_artifact.requests", mock)
+    mocker.patch(
+        "wandb.sdk.artifacts.storage_policies.wandb_storage_policy.requests", mock
+    )
     mocker.patch("wandb.wandb_sdk.lib.gql_request.requests", mock)
     mocker.patch("wandb.wandb_sdk.internal.file_stream.requests", mock)
     mocker.patch("wandb.wandb_sdk.internal.internal_api.requests", mock)
     mocker.patch("wandb.wandb_sdk.internal.update.requests", mock)
     mocker.patch("wandb.wandb_sdk.internal.sender.requests", mock)
     mocker.patch("wandb.apis.public.requests", mock)
     mocker.patch("wandb.util.requests", mock)
-    mocker.patch("wandb.wandb_sdk.wandb_artifacts.requests", mock)
     mocker.patch("azure.core.pipeline.transport._requests_basic.requests", mock)
     print("Patched requests everywhere", os.getpid())
     return mock
 
 
 def run(ctx):
     if ctx["resume"]:
```

### Comparing `yea-wandb-0.9.8/src/yea_wandb/plugin.py` & `yea-wandb-0.9.9/src/yea_wandb/plugin.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb/setup.py` & `yea-wandb-0.9.9/src/yea_wandb/setup.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.8/src/yea_wandb.egg-info/SOURCES.txt` & `yea-wandb-0.9.9/src/yea_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

