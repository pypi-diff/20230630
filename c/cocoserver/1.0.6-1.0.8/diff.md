# Comparing `tmp/cocoserver-1.0.6.tar.gz` & `tmp/cocoserver-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoserver-1.0.6.tar", last modified: Thu Jun 29 02:31:00 2023, max compression
+gzip compressed data, was "cocoserver-1.0.8.tar", last modified: Thu Jun 29 23:28:16 2023, max compression
```

## Comparing `cocoserver-1.0.6.tar` & `cocoserver-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 02:31:00.299595 cocoserver-1.0.6/
--rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-24 13:34:32.000000 cocoserver-1.0.6/LICENSE
--rw-r--r--   0 culler     (501) staff       (20)     2964 2023-06-29 02:31:00.299142 cocoserver-1.0.6/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)     1977 2023-06-25 15:33:55.000000 cocoserver-1.0.6/README.rst
--rw-r--r--   0 culler     (501) staff       (20)     1287 2023-06-28 01:20:09.000000 cocoserver-1.0.6/pyproject.toml
--rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-29 02:31:00.299762 cocoserver-1.0.6/setup.cfg
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 02:31:00.292916 cocoserver-1.0.6/src/
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 02:31:00.296486 cocoserver-1.0.6/src/cocoserver/
--rw-r--r--   0 culler     (501) staff       (20)     6703 2023-06-29 02:30:34.000000 cocoserver-1.0.6/src/cocoserver/__init__.py
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 02:31:00.298377 cocoserver-1.0.6/src/cocoserver.egg-info/
--rw-r--r--   0 culler     (501) staff       (20)     2964 2023-06-29 02:31:00.000000 cocoserver-1.0.6/src/cocoserver.egg-info/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)      212 2023-06-29 02:31:00.000000 cocoserver-1.0.6/src/cocoserver.egg-info/SOURCES.txt
--rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-29 02:31:00.000000 cocoserver-1.0.6/src/cocoserver.egg-info/dependency_links.txt
--rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-29 02:31:00.000000 cocoserver-1.0.6/src/cocoserver.egg-info/top_level.txt
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.250645 cocoserver-1.0.8/
+-rw-r--r--   0 culler     (501) staff       (20)    18092 2023-06-26 20:10:54.000000 cocoserver-1.0.8/LICENSE
+-rw-r--r--   0 culler     (501) staff       (20)     2964 2023-06-29 23:28:16.250441 cocoserver-1.0.8/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)     1977 2023-06-26 20:10:54.000000 cocoserver-1.0.8/README.rst
+-rw-r--r--   0 culler     (501) staff       (20)     1287 2023-06-28 01:52:55.000000 cocoserver-1.0.8/pyproject.toml
+-rw-r--r--   0 culler     (501) staff       (20)       38 2023-06-29 23:28:16.250703 cocoserver-1.0.8/setup.cfg
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.248308 cocoserver-1.0.8/src/
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.249223 cocoserver-1.0.8/src/cocoserver/
+-rw-r--r--   0 culler     (501) staff       (20)     7565 2023-06-29 23:23:16.000000 cocoserver-1.0.8/src/cocoserver/__init__.py
+drwxr-xr-x   0 culler     (501) staff       (20)        0 2023-06-29 23:28:16.250159 cocoserver-1.0.8/src/cocoserver.egg-info/
+-rw-r--r--   0 culler     (501) staff       (20)     2964 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/PKG-INFO
+-rw-r--r--   0 culler     (501) staff       (20)      212 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/SOURCES.txt
+-rw-r--r--   0 culler     (501) staff       (20)        1 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/dependency_links.txt
+-rw-r--r--   0 culler     (501) staff       (20)       11 2023-06-29 23:28:16.000000 cocoserver-1.0.8/src/cocoserver.egg-info/top_level.txt
```

### Comparing `cocoserver-1.0.6/LICENSE` & `cocoserver-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.6/PKG-INFO` & `cocoserver-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.6
+Version: 1.0.8
 Summary: A local HTTP server for compressed content.
 Author-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Maintainer-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Project-URL: Homepage, https://github.com/3-manifolds/cocoserver
 Project-URL: Bug Tracker, https://github.com/3-manifolds/cocoserver/issues
 Keywords: http,server,gzip,documentation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cocoserver-1.0.6/README.rst` & `cocoserver-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.6/pyproject.toml` & `cocoserver-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cocoserver-1.0.6/src/cocoserver/__init__.py` & `cocoserver-1.0.8/src/cocoserver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import email
 import shutil
 import datetime
 import webbrowser
 import urllib.parse
 import importlib.metadata
 
-__version__ = '1.0.6'
+__version__ = '1.0.8'
 
 class GzipHTTPRequestHandler(SimpleHTTPRequestHandler):
     def __init__(self, *args, **kwargs):
         self.logfile = kwargs.pop('logfile', None)
         super().__init__(*args, **kwargs)
 
     def log_message(self, format, *args):
@@ -32,15 +32,14 @@
 
         This sends the response code and MIME headers.
 
         Return value is either a file object (which has to be copied
         to the outputfile by the caller unless the command was HEAD,
         and must be closed by the caller under all circumstances), or
         None, in which case the caller has nothing further to do.
-
         """
         path = self.translate_path(self.path)
         have_gz = False
         f = None
         if os.path.isdir(path):
             parts = urllib.parse.urlsplit(self.path)
             if not parts.path.endswith('/'):
@@ -133,35 +132,49 @@
             # Ignore exceptions when the browser closes the connection
             # while receiving a response. They seem to try again anyway.
             pass
 
 class StaticServer:
     """Runs an HTTP server in a background thread.
 
-    The server serves static files, possibly gzipped, from a specified
-    root directory.
-    """ 
-
+    The server serves static files, optionally gzipped in advance, from
+    a specified root directory.  Only the GET and HEAD methods are
+    supported.  Query strings are ignored. Thus form submission and file
+    uploads are not supported.
+    """
     def __init__(self, root_dir, logfile=None):
         self.site_root = os.path.abspath(root_dir)
         self.httpd = None
         self.logfile = logfile
         if logfile and not hasattr(logfile, 'write'):
             raise ValueError('The logfile must have a write method.')
-        
+
     def start(self):
+        """Start the server and return its address."""
+        # Only listen on the loopback interface.  This server is
+        # not intended to be accessed from the internet.
         server_address = ('127.0.0.1', 0)
         handler = partial(GzipHTTPRequestHandler,
                               directory=self.site_root,
                               logfile=self.logfile)
         self.httpd = ThreadingHTTPServer(server_address, handler)
         self.server_thread = Thread(target=self.httpd.serve_forever,
                                         daemon=True)
         self.server_thread.start()
+        return tuple(self.httpd.server_address)
 
     def visit(self, path=''):
+        """Use the default browser to open a page on the site."""
         if not self.httpd or not self.server_thread.is_alive():
             self.start()
-        port = self.httpd.server_address[1]
-        url = os.path.join('http://localhost:%s' % port, path)
+        address, port = self.httpd.server_address
+        # The localhost domain could get resolved to a different
+        # address by a nasty nameserver.  So it is safer to use
+        # the dotted quad address for the loopback interface.
+        url = os.path.join('http://%s:%s/%s' % (address, port, path))
         webbrowser.open_new_tab(url)
-        
+
+    def address(self):
+        """Return the ip address of this server."""
+        if not self.httpd or not self.server_thread.is_alive():
+            raise ValueError('Server is not running')
+        return self.httpd.server_address
```

### Comparing `cocoserver-1.0.6/src/cocoserver.egg-info/PKG-INFO` & `cocoserver-1.0.8/src/cocoserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocoserver
-Version: 1.0.6
+Version: 1.0.8
 Summary: A local HTTP server for compressed content.
 Author-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Maintainer-email: Marc Culler <culler@users.noreply.github.com>, "Nathan M. Dunfield" <nathan@dunfield.info>, Matthias Görner <enischte@gmail.com>
 Project-URL: Homepage, https://github.com/3-manifolds/cocoserver
 Project-URL: Bug Tracker, https://github.com/3-manifolds/cocoserver/issues
 Keywords: http,server,gzip,documentation
 Classifier: Development Status :: 3 - Alpha
```

