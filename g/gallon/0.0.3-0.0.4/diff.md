# Comparing `tmp/gallon-0.0.3.tar.gz` & `tmp/gallon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallon-0.0.3.tar", max compression
+gzip compressed data, was "gallon-0.0.4.tar", max compression
```

## Comparing `gallon-0.0.3.tar` & `gallon-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.3/README.md
--rw-r--r--   0        0        0      264 2023-06-30 07:01:59.904811 gallon-0.0.3/gallon/__init__.py
--rw-r--r--   0        0        0     4218 2023-06-30 07:27:51.666714 gallon-0.0.3/gallon/client.py
--rw-r--r--   0        0        0     9500 2023-06-30 07:01:56.168728 gallon-0.0.3/gallon/data.py
--rw-r--r--   0        0        0     1634 2023-06-30 07:23:38.755867 gallon-0.0.3/gallon/decorators.py
--rw-r--r--   0        0        0     2320 2023-06-30 07:01:56.616738 gallon-0.0.3/gallon/helpers.py
--rw-r--r--   0        0        0     3864 2023-06-30 09:51:40.217546 gallon-0.0.3/gallon/objects.py
--rw-r--r--   0        0        0     6638 2023-06-30 10:03:59.027419 gallon-0.0.3/gallon/server.py
--rw-r--r--   0        0        0        0 2023-06-30 08:25:20.676613 gallon-0.0.3/gallon/templating.py
--rw-r--r--   0        0        0      296 2023-06-30 10:04:54.485363 gallon-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 gallon-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.4/README.md
+-rw-r--r--   0        0        0      264 2023-06-30 07:01:59.904811 gallon-0.0.4/gallon/__init__.py
+-rw-r--r--   0        0        0     4225 2023-06-30 11:31:13.484283 gallon-0.0.4/gallon/client.py
+-rw-r--r--   0        0        0     9296 2023-06-30 11:30:39.436538 gallon-0.0.4/gallon/data.py
+-rw-r--r--   0        0        0     1634 2023-06-30 07:23:38.755867 gallon-0.0.4/gallon/decorators.py
+-rw-r--r--   0        0        0     2320 2023-06-30 07:01:56.616738 gallon-0.0.4/gallon/helpers.py
+-rw-r--r--   0        0        0     3864 2023-06-30 09:51:40.217546 gallon-0.0.4/gallon/objects.py
+-rw-r--r--   0        0        0     6653 2023-06-30 10:11:22.074974 gallon-0.0.4/gallon/server.py
+-rw-r--r--   0        0        0        0 2023-06-30 08:25:20.676613 gallon-0.0.4/gallon/templating.py
+-rw-r--r--   0        0        0      296 2023-06-30 11:30:41.020526 gallon-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 gallon-0.0.4/PKG-INFO
```

### Comparing `gallon-0.0.3/gallon/client.py` & `gallon-0.0.4/gallon/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         with conn.getresponse() as res:
             response_headers = self._parse_response_headers(res)
             response_body = self._parse_response_body(res, response_headers)
             response = Response(
                 status=res.status, headers=response_headers, body=response_body
             )
-            return response
+            return response.dict()
 
     def _prepare_body(self, request: Request):
         """Prepare the body based on the content type"""
         _json = request.json()
         if _json is None:
             return None
         if request.content_type == "application/x-www-form-urlencoded":
```

### Comparing `gallon-0.0.3/gallon/data.py` & `gallon-0.0.4/gallon/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,21 +185,14 @@
             setattr(self, name, value)
 
     def __repr__(self):
         """Return a string representation of the data class instance."""
         return f"<{self.__class__.__name__} {self.__dict__}>"
 
 
-def exclude(dct: dict):
-    """
-    Return a new dictionary that excludes entries with None values from the input dictionary.
-    """
-    return {k: v for k, v in dct.items() if v is not None}
-
-
 class GallonEncoder(json.JSONEncoder):
     """
     A JSONEncoder subclass that knows how to encode date/time, UUID, bytes, and custom types.
     """
 
     def default(self, o):
         """Return a serializable version of the given object."""
@@ -221,15 +214,15 @@
     """
     Convert a dictionary to a JSON-formatted string and then parse it back to a dictionary.
     This is used to serialize and then deserialize a dictionary, effectively cloning it.
     Optionally exclude entries with None values.
     """
     string = json.dumps(dct, cls=GallonEncoder)
     if exclude_none:
-        return exclude(json.loads(string))
+        return json.loads(string)
     return json.loads(string)
 
 
 class GallonModel(DataClass):
     """
     A data class that can convert itself to a dictionary or a JSON-formatted string.
     """
```

### Comparing `gallon-0.0.3/gallon/decorators.py` & `gallon-0.0.4/gallon/decorators.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.3/gallon/helpers.py` & `gallon-0.0.4/gallon/helpers.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.3/gallon/objects.py` & `gallon-0.0.4/gallon/objects.py`

 * *Files identical despite different names*

### Comparing `gallon-0.0.3/gallon/server.py` & `gallon-0.0.4/gallon/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             raw_response = handler(request)  # handler's return value
             response = make_response(
                 raw_response
             )  # use make_response to format it properly
             self.send_response(response.status)
             for key, value in response.headers.items():
                 self.send_header(key, value)
-            self.send_header("Content-Length", str(len(response.body)))
+            self.send_header("Content-Length", str(len(response.body))) # type: ignore
             self.send_header("Access-Control-Allow-Origin", "*")
             self.send_header("Access-Control-Allow-Headers", "*")
             self.send_header("Access-Control-Allow-Methods", "*")
             self.send_header("Access-Control-Allow-Credentials", "true")
             self.send_header("Access-Control-Max-Age", "86400")
             self.end_headers()
             assert response.body is not None
```

