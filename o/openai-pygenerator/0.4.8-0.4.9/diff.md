# Comparing `tmp/openai-pygenerator-0.4.8.tar.gz` & `tmp/openai-pygenerator-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.8.tar", last modified: Fri Jun 30 07:29:30 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.9.tar", last modified: Fri Jun 30 18:18:52 2023, max compression
```

## Comparing `openai-pygenerator-0.4.8.tar` & `openai-pygenerator-0.4.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.536298 openai-pygenerator-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.536298 openai-pygenerator-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/src/openai_pygenerator/openai_pygenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/src/openai_pygenerator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-30 07:29:30.000000 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-30 07:29:30.000000 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 07:29:30.000000 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 07:29:30.000000 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 07:29:30.000000 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 07:29:30.000000 openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 07:29:30.540298 openai-pygenerator-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-30 07:29:20.000000 openai-pygenerator-0.4.8/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.690683 openai-pygenerator-0.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.682683 openai-pygenerator-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.686683 openai-pygenerator-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-30 18:18:52.690683 openai-pygenerator-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-30 18:18:52.690683 openai-pygenerator-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.682683 openai-pygenerator-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.686683 openai-pygenerator-0.4.9/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/src/openai_pygenerator/openai_pygenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/src/openai_pygenerator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.690683 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-30 18:18:52.000000 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-30 18:18:52.000000 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:18:52.000000 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 18:18:52.000000 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 18:18:52.000000 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 18:18:52.000000 openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:18:52.690683 openai-pygenerator-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-30 18:18:42.000000 openai-pygenerator-0.4.9/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.8/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/.pre-commit-config.yaml` & `openai-pygenerator-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/.pylintrc` & `openai-pygenerator-0.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/LICENSE.txt` & `openai-pygenerator-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/PKG-INFO` & `openai-pygenerator-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.8
+Version: 0.4.9
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.8/README.md` & `openai-pygenerator-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/pyproject.toml` & `openai-pygenerator-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.9/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.9/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
             n=n,
             temperature=temperature,
         )
         logger.debug("response = %s", result)
         for choice in result.choices:
             yield choice.message
     except (
+        openai.error.Timeout,
         urllib3.exceptions.TimeoutError,
         RateLimitError,
         APIError,
         ServiceUnavailableError,
     ) as err:
         if isinstance(err, APIError) and not (err.http_status in [524, 502]):
             raise
```

### Comparing `openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.8
+Version: 0.4.9
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.8/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.9/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.8/tests/test_gpt.py` & `openai-pygenerator-0.4.9/tests/test_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=redefined-outer-name
 
 from typing import Iterable
 
+import openai.error
 import pytest
 import urllib3.exceptions as urlex
 from openai.error import APIError, RateLimitError, ServiceUnavailableError
 from openai.openai_object import OpenAIObject
 
 from openai_pygenerator import (
     GPT_MAX_RETRIES,
@@ -79,14 +80,15 @@
 @pytest.mark.parametrize(
     "error",
     [
         RateLimitError("rate limited", http_status=429),
         APIError("Gateway Timeout", http_status=524),
         ServiceUnavailableError("Service unavailable"),
         urlex.ReadTimeoutError("test-pool", "http://test", "read timeout"),
+        openai.error.Timeout,
     ],
 )
 def test_generate_completion_error(mock_openai, mock_sleep, error):
     mock_openai.side_effect = [error] * GPT_MAX_RETRIES
 
     with pytest.raises(Exception):
         _ = list(gpt_completions([]))
```

