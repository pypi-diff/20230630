# Comparing `tmp/moesifwsgi-1.8.0.tar.gz` & `tmp/moesifwsgi-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moesifwsgi-1.8.0.tar", last modified: Thu Jun 15 14:54:28 2023, max compression
+gzip compressed data, was "dist/moesifwsgi-1.8.1.tar", last modified: Thu Jun 29 23:52:20 2023, max compression
```

## Comparing `moesifwsgi-1.8.0.tar` & `moesifwsgi-1.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-15 14:54:28.349210 moesifwsgi-1.8.0/
--rwxr-xr-x   0 keyur      (501) staff       (20)    11911 2020-06-25 11:08:31.000000 moesifwsgi-1.8.0/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2020-04-19 17:20:34.000000 moesifwsgi-1.8.0/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    22049 2023-06-15 14:54:28.349443 moesifwsgi-1.8.0/PKG-INFO
--rwxr-xr-x   0 keyur      (501) staff       (20)    17163 2023-06-15 14:36:10.000000 moesifwsgi-1.8.0/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-15 14:54:28.347047 moesifwsgi-1.8.0/moesifwsgi/
--rw-r--r--   0 keyur      (501) staff       (20)       26 2020-04-19 17:20:34.000000 moesifwsgi-1.8.0/moesifwsgi/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     4634 2020-12-29 19:45:45.000000 moesifwsgi-1.8.0/moesifwsgi/client_ip.py
--rw-r--r--   0 keyur      (501) staff       (20)     4570 2023-06-15 14:36:10.000000 moesifwsgi-1.8.0/moesifwsgi/config_manager.py
--rw-r--r--   0 keyur      (501) staff       (20)     3526 2023-05-12 21:29:24.000000 moesifwsgi-1.8.0/moesifwsgi/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     1067 2023-04-20 01:32:27.000000 moesifwsgi-1.8.0/moesifwsgi/http_response_catcher.py
--rw-r--r--   0 keyur      (501) staff       (20)    10434 2023-04-20 01:32:27.000000 moesifwsgi-1.8.0/moesifwsgi/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     9708 2023-06-15 14:36:10.000000 moesifwsgi-1.8.0/moesifwsgi/middleware.py
--rw-r--r--   0 keyur      (501) staff       (20)     3071 2023-05-12 21:29:36.000000 moesifwsgi-1.8.0/moesifwsgi/moesif_data_holder.py
--rw-r--r--   0 keyur      (501) staff       (20)     2344 2020-12-29 19:47:50.000000 moesifwsgi-1.8.0/moesifwsgi/parse_body.py
--rw-r--r--   0 keyur      (501) staff       (20)     4018 2022-01-13 23:06:22.000000 moesifwsgi-1.8.0/moesifwsgi/regex_config_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     8531 2023-04-20 01:32:27.000000 moesifwsgi-1.8.0/moesifwsgi/update_companies.py
--rw-r--r--   0 keyur      (501) staff       (20)     8100 2023-04-20 01:32:27.000000 moesifwsgi-1.8.0/moesifwsgi/update_users.py
--rw-r--r--   0 keyur      (501) staff       (20)     6887 2023-06-15 14:36:10.000000 moesifwsgi-1.8.0/moesifwsgi/workers.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-15 14:54:28.348983 moesifwsgi-1.8.0/moesifwsgi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    22049 2023-06-15 14:54:28.000000 moesifwsgi-1.8.0/moesifwsgi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      581 2023-06-15 14:54:28.000000 moesifwsgi-1.8.0/moesifwsgi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2023-06-15 14:54:28.000000 moesifwsgi-1.8.0/moesifwsgi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)      130 2023-06-15 14:54:28.000000 moesifwsgi-1.8.0/moesifwsgi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       11 2023-06-15 14:54:28.000000 moesifwsgi-1.8.0/moesifwsgi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2023-06-15 14:54:28.349900 moesifwsgi-1.8.0/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3693 2023-06-15 14:36:10.000000 moesifwsgi-1.8.0/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-29 23:52:20.336958 moesifwsgi-1.8.1/
+-rwxr-xr-x   0 keyur      (501) staff       (20)    11911 2020-06-25 11:08:31.000000 moesifwsgi-1.8.1/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2020-04-19 17:20:34.000000 moesifwsgi-1.8.1/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    22428 2023-06-29 23:52:20.337592 moesifwsgi-1.8.1/PKG-INFO
+-rwxr-xr-x   0 keyur      (501) staff       (20)    17486 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-29 23:52:20.334104 moesifwsgi-1.8.1/moesifwsgi/
+-rw-r--r--   0 keyur      (501) staff       (20)       26 2020-04-19 17:20:34.000000 moesifwsgi-1.8.1/moesifwsgi/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4634 2020-12-29 19:45:45.000000 moesifwsgi-1.8.1/moesifwsgi/client_ip.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4570 2023-06-15 14:36:10.000000 moesifwsgi-1.8.1/moesifwsgi/config_manager.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3526 2023-05-12 21:29:24.000000 moesifwsgi-1.8.1/moesifwsgi/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     1067 2023-04-20 01:32:27.000000 moesifwsgi-1.8.1/moesifwsgi/http_response_catcher.py
+-rw-r--r--   0 keyur      (501) staff       (20)    10558 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/moesifwsgi/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     9910 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/moesifwsgi/middleware.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3071 2023-05-12 21:29:36.000000 moesifwsgi-1.8.1/moesifwsgi/moesif_data_holder.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2344 2020-12-29 19:47:50.000000 moesifwsgi-1.8.1/moesifwsgi/parse_body.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4018 2022-01-13 23:06:22.000000 moesifwsgi-1.8.1/moesifwsgi/regex_config_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8531 2023-04-20 01:32:27.000000 moesifwsgi-1.8.1/moesifwsgi/update_companies.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8100 2023-04-20 01:32:27.000000 moesifwsgi-1.8.1/moesifwsgi/update_users.py
+-rw-r--r--   0 keyur      (501) staff       (20)     6887 2023-06-15 14:36:10.000000 moesifwsgi-1.8.1/moesifwsgi/workers.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-29 23:52:20.336746 moesifwsgi-1.8.1/moesifwsgi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    22428 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      581 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)      130 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       11 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2023-06-29 23:52:20.339119 moesifwsgi-1.8.1/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3693 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/setup.py
```

### Comparing `moesifwsgi-1.8.0/LICENSE` & `moesifwsgi-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/PKG-INFO` & `moesifwsgi-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.8.0
+Version: 1.8.1
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
 Description: # Moesif Middleware for Python WSGI based Frameworks
         
@@ -111,21 +111,28 @@
         ### Other WSGI frameworks
         
         If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
         Please read the documentation for your specific framework on how to add middleware.
         
         ## Configuration options
         
+        The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+        Also, Moesif adds the following to the environ variable
+        ```
+        environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
+        environ["moesif.response_body_chunks"] - A response body chunks
+        environ["moesif.response_headers"] - A dict representing the response headers
+        ```
+        
         #### __`APPLICATION_ID`__
         (__required__), _string_, is obtained via your Moesif Account, this is required.
         
         #### __`SKIP`__
         (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-        and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
-        environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+        and returns true if you want to skip this particular event.
         
         #### __`IDENTIFY_USER`__
         (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
         but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
         
         #### __`IDENTIFY_COMPANY`__
         (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
```

### Comparing `moesifwsgi-1.8.0/README.md` & `moesifwsgi-1.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,28 @@
 ### Other WSGI frameworks
 
 If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
 Please read the documentation for your specific framework on how to add middleware.
 
 ## Configuration options
 
+The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+Also, Moesif adds the following to the environ variable
+```
+environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
+environ["moesif.response_body_chunks"] - A response body chunks
+environ["moesif.response_headers"] - A dict representing the response headers
+```
+
 #### __`APPLICATION_ID`__
 (__required__), _string_, is obtained via your Moesif Account, this is required.
 
 #### __`SKIP`__
 (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
-environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+and returns true if you want to skip this particular event.
 
 #### __`IDENTIFY_USER`__
 (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
 but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
 
 #### __`IDENTIFY_COMPANY`__
 (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
```

### Comparing `moesifwsgi-1.8.0/moesifwsgi/client_ip.py` & `moesifwsgi-1.8.1/moesifwsgi/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/config_manager.py` & `moesifwsgi-1.8.1/moesifwsgi/config_manager.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/event_mapper.py` & `moesifwsgi-1.8.1/moesifwsgi/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/http_response_catcher.py` & `moesifwsgi-1.8.1/moesifwsgi/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/logger_helper.py` & `moesifwsgi-1.8.1/moesifwsgi/logger_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,19 @@
             else:
                 content_length = int(content_length)
                 body = environ['wsgi.input'].read(content_length)
 
             if isinstance(body, str):
                 environ['wsgi.input'] = StringIO(body) # reset request body for the nested app Python2
                 encoded_body, transfer_encoding = self.parse_body.parse_string_body(body, content_encoding, None)
+                environ['moesif.request_body'] = encoded_body
             else:
                 environ['wsgi.input'] = BytesIO(body) # reset request body for the nested app Python3
                 encoded_body, transfer_encoding = self.parse_body.parse_bytes_body(body, content_encoding, None)
+                environ['moesif.request_body'] = encoded_body
         else:
             content_length = 0
         return content_length, encoded_body, transfer_encoding
 
     @classmethod
     def transform_token(cls, token):
         if not isinstance(token, str):
```

### Comparing `moesifwsgi-1.8.0/moesifwsgi/middleware.py` & `moesifwsgi-1.8.1/moesifwsgi/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,14 +119,18 @@
                     for pair in response_headers:
                         response_headers_mapping[pair[0]] = pair[1]
                 except Exception as e:
                     logger.exception("Error while parsing response headers", e)
             return start_response(status, response_headers, *args)
         response_chunks = event_info.finish_response(self.app(environ, _start_response))
 
+        # Add response chunks and response headers to the environ
+        environ["moesif.response_body_chunks"] = response_chunks
+        environ["moesif.response_headers"] = response_headers_mapping
+
         try:
             logger.debug(f"event response time: {event_info.response_time}")
         except Exception as e:
             logger.exception(f"Error while fetching response time", e)
 
         self.add_user_and_metadata(event_info, environ, response_headers_mapping)
```

### Comparing `moesifwsgi-1.8.0/moesifwsgi/moesif_data_holder.py` & `moesifwsgi-1.8.1/moesifwsgi/moesif_data_holder.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/parse_body.py` & `moesifwsgi-1.8.1/moesifwsgi/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/regex_config_helper.py` & `moesifwsgi-1.8.1/moesifwsgi/regex_config_helper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/update_companies.py` & `moesifwsgi-1.8.1/moesifwsgi/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/update_users.py` & `moesifwsgi-1.8.1/moesifwsgi/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi/workers.py` & `moesifwsgi-1.8.1/moesifwsgi/workers.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/moesifwsgi.egg-info/PKG-INFO` & `moesifwsgi-1.8.1/moesifwsgi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.8.0
+Version: 1.8.1
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
 Description: # Moesif Middleware for Python WSGI based Frameworks
         
@@ -111,21 +111,28 @@
         ### Other WSGI frameworks
         
         If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
         Please read the documentation for your specific framework on how to add middleware.
         
         ## Configuration options
         
+        The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+        Also, Moesif adds the following to the environ variable
+        ```
+        environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
+        environ["moesif.response_body_chunks"] - A response body chunks
+        environ["moesif.response_headers"] - A dict representing the response headers
+        ```
+        
         #### __`APPLICATION_ID`__
         (__required__), _string_, is obtained via your Moesif Account, this is required.
         
         #### __`SKIP`__
         (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-        and returns true if you want to skip this particular event. The app is the original WSGI app instance, and the
-        environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+        and returns true if you want to skip this particular event.
         
         #### __`IDENTIFY_USER`__
         (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
         but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
         
         #### __`IDENTIFY_COMPANY`__
         (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
```

### Comparing `moesifwsgi-1.8.0/moesifwsgi.egg-info/SOURCES.txt` & `moesifwsgi-1.8.1/moesifwsgi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.0/setup.py` & `moesifwsgi-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifwsgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.8.0',
+    version='1.8.1',
 
     description='Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-wsgi/',
```

