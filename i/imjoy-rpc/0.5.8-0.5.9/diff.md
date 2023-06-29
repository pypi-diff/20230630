# Comparing `tmp/imjoy-rpc-0.5.8.tar.gz` & `tmp/imjoy-rpc-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imjoy-rpc-0.5.8.tar", last modified: Tue May  3 09:57:01 2022, max compression
+gzip compressed data, was "imjoy-rpc-0.5.9.tar", last modified: Tue May  3 11:51:24 2022, max compression
```

## Comparing `imjoy-rpc-0.5.8.tar` & `imjoy-rpc-0.5.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/imjoy_rpc/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-03 09:56:58.000000 imjoy-rpc-0.5.8/imjoy_rpc/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/imjoy_rpc/connection/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/connection/colab_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    10937 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/connection/imjoy_colab.html
--rw-r--r--   0 runner    (1001) docker     (121)    11618 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/connection/jupyter_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/connection/pyodide_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8936 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/connection/socketio_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/imjoy_rpc/core_connection/
--rw-r--r--   0 runner    (1001) docker     (121)     7809 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/core_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/imjoy_rpc/hypha/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/hypha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/hypha/pyodide_websocket.py
--rw-r--r--   0 runner    (1001) docker     (121)    51177 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/hypha/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8514 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/hypha/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/hypha/websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    34167 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    26446 2022-05-03 09:56:58.000000 imjoy-rpc-0.5.8/imjoy_rpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/imjoy_rpc/werkzeug/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/werkzeug/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6670 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/werkzeug/_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14403 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/imjoy_rpc/werkzeug/local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-03 09:57:00.000000 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-03 09:57:01.000000 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 09:57:00.000000 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 09:56:00.000000 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-05-03 09:57:01.000000 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-03 09:57:01.000000 imjoy-rpc-0.5.8/imjoy_rpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:57:01.412767 imjoy-rpc-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-03 09:56:58.000000 imjoy-rpc-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-05-03 09:56:58.000000 imjoy-rpc-0.5.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-05-03 09:55:47.000000 imjoy-rpc-0.5.8/tests/test_jupyter_rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-03 09:56:58.000000 imjoy-rpc-0.5.8/tests/test_websocket_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.453513 imjoy-rpc-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-03 11:51:24.453513 imjoy-rpc-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.449514 imjoy-rpc-0.5.9/imjoy_rpc/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-03 11:51:21.000000 imjoy-rpc-0.5.9/imjoy_rpc/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.449514 imjoy-rpc-0.5.9/imjoy_rpc/connection/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/connection/colab_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10937 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/connection/imjoy_colab.html
+-rw-r--r--   0 runner    (1001) docker     (121)    11618 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/connection/jupyter_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/connection/pyodide_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8936 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/connection/socketio_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.449514 imjoy-rpc-0.5.9/imjoy_rpc/core_connection/
+-rw-r--r--   0 runner    (1001) docker     (121)     7809 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/core_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.453513 imjoy-rpc-0.5.9/imjoy_rpc/hypha/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/hypha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/hypha/pyodide_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51177 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/hypha/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8514 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/hypha/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/hypha/websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34167 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27372 2022-05-03 11:51:21.000000 imjoy-rpc-0.5.9/imjoy_rpc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.453513 imjoy-rpc-0.5.9/imjoy_rpc/werkzeug/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/werkzeug/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6670 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/werkzeug/_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14403 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/imjoy_rpc/werkzeug/local.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.449514 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-05-03 11:51:23.000000 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-03 11:51:24.000000 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 11:51:23.000000 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 11:50:25.000000 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-05-03 11:51:24.000000 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-03 11:51:24.000000 imjoy-rpc-0.5.9/imjoy_rpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-05-03 11:51:24.453513 imjoy-rpc-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 11:51:24.453513 imjoy-rpc-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/tests/test_jupyter_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-03 11:50:13.000000 imjoy-rpc-0.5.9/tests/test_websocket_rpc.py
```

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/__init__.py` & `imjoy-rpc-0.5.9/imjoy_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/connection/colab_connection.py` & `imjoy-rpc-0.5.9/imjoy_rpc/connection/colab_connection.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/connection/imjoy_colab.html` & `imjoy-rpc-0.5.9/imjoy_rpc/connection/imjoy_colab.html`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/connection/jupyter_connection.py` & `imjoy-rpc-0.5.9/imjoy_rpc/connection/jupyter_connection.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/connection/pyodide_connection.py` & `imjoy-rpc-0.5.9/imjoy_rpc/connection/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/connection/socketio_connection.py` & `imjoy-rpc-0.5.9/imjoy_rpc/connection/socketio_connection.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/core_connection/__init__.py` & `imjoy-rpc-0.5.9/imjoy_rpc/core_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/hypha/pyodide_websocket.py` & `imjoy-rpc-0.5.9/imjoy_rpc/hypha/pyodide_websocket.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/hypha/rpc.py` & `imjoy-rpc-0.5.9/imjoy_rpc/hypha/rpc.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/hypha/utils.py` & `imjoy-rpc-0.5.9/imjoy_rpc/hypha/utils.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/hypha/websocket_client.py` & `imjoy-rpc-0.5.9/imjoy_rpc/hypha/websocket_client.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/rpc.py` & `imjoy-rpc-0.5.9/imjoy_rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/utils.py` & `imjoy-rpc-0.5.9/imjoy_rpc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -645,25 +645,46 @@
         formData.append("file", file);
         if(append) formData.append("append", "1");
         request.send(formData);
         return request
     }
     """
     )
+
+    _sync_xhr_put = eval(
+        """globalThis._sync_xhr_put = function(url, rawData, type, append){
+        if(append) throw new Error("append is not supported for put requests");
+        var request = new XMLHttpRequest();
+        request.open('PUT', url, false);  // `false` makes the request synchronous
+        var formData = new FormData();
+        var file = new Blob([new Uint8Array(rawData)],{type});
+        request.send(file);
+        return request
+    }
+    """
+    )
     IS_PYODIDE = True
 except ImportError:
     from urllib.request import Request, urlopen
 
     IS_PYODIDE = False
 
 
 class HTTPFile(io.IOBase):
     """A virtual file for reading content via HTTP."""
 
-    def __init__(self, url, mode="r", encoding=None, newline=None, name=None):
+    def __init__(
+        self,
+        url,
+        mode="r",
+        encoding=None,
+        newline=None,
+        name=None,
+        upload_method="POST",
+    ):
         """Initialize the http file object."""
         self._url = url
         self._pos = 0
         self._size = None
         self._mode = mode
         self.name = name
         assert mode in ["r", "rb", "w", "wb", "a", "ab"]
@@ -671,14 +692,16 @@
         self._newline = newline or os.linesep
         if "w" not in self._mode:
             # make a request so we can see the self._size
             self._request_range(0, 0)
             assert self._size is not None
         self._chunk = 1024
         self._initial_request = True
+        assert upload_method in ["POST", "PUT"]
+        self._upload_method = upload_method
 
     def tell(self):
         """Tell the position of the pointer."""
         return self._pos
 
     def write(self, content):
         """Write content to file."""
@@ -770,15 +793,22 @@
     def _upload(self, content):
         if IS_PYODIDE:
             if self._initial_request and "a" not in self._mode:
                 append = False
             else:
                 append = True
 
-            req = _sync_xhr_post(self._url, content, "application/octet-stream", append)
+            if self._upload_method == "POST":
+                req = _sync_xhr_post(
+                    self._url, content, "application/octet-stream", append
+                )
+            elif self._upload_method == "PUT":
+                req = _sync_xhr_post(
+                    self._url, content, "application/octet-stream", append
+                )
             if req.status != 200:
                 raise Exception(f"Failed to write: {req.response}, {req.status}")
 
             if self._initial_request:
                 self._initial_request = False
         else:
             raise NotImplementedError
```

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/werkzeug/_compat.py` & `imjoy-rpc-0.5.9/imjoy_rpc/werkzeug/_compat.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc/werkzeug/local.py` & `imjoy-rpc-0.5.9/imjoy_rpc/werkzeug/local.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/imjoy_rpc.egg-info/SOURCES.txt` & `imjoy-rpc-0.5.9/imjoy_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/setup.py` & `imjoy-rpc-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/tests/conftest.py` & `imjoy-rpc-0.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/tests/test_jupyter_rpc.py` & `imjoy-rpc-0.5.9/tests/test_jupyter_rpc.py`

 * *Files identical despite different names*

### Comparing `imjoy-rpc-0.5.8/tests/test_websocket_rpc.py` & `imjoy-rpc-0.5.9/tests/test_websocket_rpc.py`

 * *Files identical despite different names*

