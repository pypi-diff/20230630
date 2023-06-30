# Comparing `tmp/playwrightcapture-1.20.9.tar.gz` & `tmp/playwrightcapture-1.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.9.tar", max compression
+gzip compressed data, was "playwrightcapture-1.21.0.tar", max compression
```

## Comparing `playwrightcapture-1.20.9.tar` & `playwrightcapture-1.21.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.9/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.9/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.9/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    37604 2023-06-26 11:33:09.009980 playwrightcapture-1.20.9/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.9/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.9/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.9/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1826 2023-06-26 11:39:18.215411 playwrightcapture-1.20.9/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.9/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.21.0/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.21.0/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.21.0/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    37664 2023-06-26 17:28:11.136863 playwrightcapture-1.21.0/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.21.0/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.21.0/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.21.0/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1826 2023-06-30 14:13:31.901153 playwrightcapture-1.21.0/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.21.0/PKG-INFO
```

### Comparing `playwrightcapture-1.20.9/LICENSE` & `playwrightcapture-1.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.9/README.md` & `playwrightcapture-1.21.0/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.9/playwrightcapture/capture.py` & `playwrightcapture-1.21.0/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,15 +569,16 @@
             if self._exception_is_network_error(e):
                 # Expected errors
                 self.logger.info(f'Unable to process {url}: {e.message}')
                 if e.name == 'net::ERR_CONNECTION_RESET':
                     self.should_retry = True
             elif e.name in ['NS_BINDING_CANCELLED_OLD_LOAD',
                             'NS_BINDING_ABORTED',
-                            'NS_ERROR_PARSED_DATA_CACHED']:
+                            'NS_ERROR_PARSED_DATA_CACHED',
+                            'NS_ERROR_DOCUMENT_NOT_CACHED']:
                 # this one sounds like something we can retry...
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Download is starting',
                             'Connection closed',
                             'Navigation interrupted by another one',
                             'Navigation failed because page was closed!',
```

### Comparing `playwrightcapture-1.20.9/playwrightcapture/helpers.py` & `playwrightcapture-1.21.0/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.9/pyproject.toml` & `playwrightcapture-1.21.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.9"
+version = "1.21.0"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.20.9/PKG-INFO` & `playwrightcapture-1.21.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.9
+Version: 1.21.0
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

