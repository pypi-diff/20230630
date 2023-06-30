# Comparing `tmp/ogsapi-0.5.0.tar.gz` & `tmp/ogsapi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.5.0.tar", last modified: Wed May  3 03:37:30 2023, max compression
+gzip compressed data, was "ogsapi-0.6.0.tar", last modified: Fri Jun 30 03:15:39 2023, max compression
```

## Comparing `ogsapi-0.5.0.tar` & `ogsapi-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.497280 ogsapi-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-05-03 03:37:14.000000 ogsapi-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5554 2023-05-03 03:37:30.497280 ogsapi-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5120 2023-05-03 03:37:14.000000 ogsapi-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-03 03:37:14.000000 ogsapi-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 03:37:30.497280 ogsapi-0.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.492280 ogsapi-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.494280 ogsapi-0.5.0/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 03:37:14.000000 ogsapi-0.5.0/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41525 2023-05-03 03:37:14.000000 ogsapi-0.5.0/src/ogsapi/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 03:37:30.496280 ogsapi-0.5.0/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5554 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 03:37:30.000000 ogsapi-0.5.0/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:15:39.457999 ogsapi-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-06-30 03:15:26.000000 ogsapi-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-30 03:15:39.456999 ogsapi-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-06-30 03:15:26.000000 ogsapi-0.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-30 03:15:26.000000 ogsapi-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 03:15:39.457999 ogsapi-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:15:39.454999 ogsapi-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:15:39.455999 ogsapi-0.6.0/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-30 03:15:26.000000 ogsapi-0.6.0/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22257 2023-06-30 03:15:26.000000 ogsapi-0.6.0/src/ogsapi/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    14926 2023-06-30 03:15:26.000000 ogsapi-0.6.0/src/ogsapi/ogsgame.py
+-rw-rw-rw-   0 root         (0) root         (0)     6720 2023-06-30 03:15:26.000000 ogsapi-0.6.0/src/ogsapi/ogssocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:15:39.456999 ogsapi-0.6.0/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-30 03:15:39.000000 ogsapi-0.6.0/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      291 2023-06-30 03:15:39.000000 ogsapi-0.6.0/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:15:39.000000 ogsapi-0.6.0/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-30 03:15:39.000000 ogsapi-0.6.0/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 03:15:39.000000 ogsapi-0.6.0/src/ogsapi.egg-info/top_level.txt
```

### Comparing `ogsapi-0.5.0/LICENSE` & `ogsapi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.5.0/PKG-INFO` & `ogsapi-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.5.0
+Version: 0.6.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -43,15 +43,15 @@
 ```bash
 pip3 uninstall python-engineio python-socketio
 pip3 install -r requirements.txt
 ```
 ## Usage
 
 ```python
-from ogsapi.api import OGSClient
+from ogsapi.client import OGSClient
 
 ogs = OGSClient('your_client_id', 'your_client_secret', 'your_username', 'your_password')
 ```
 This will authenticate you to OGS using your API credentials, and connect you to the Realtime API Socket. You can now call the usable functions.
 
 ## Implemented API Functions
 *NOTE* All usernames are case sensitive
@@ -155,31 +155,31 @@
     - [ ] reset
     - [ ] reset-chats
     - [x] undo_accepted
     - [x] undo_canceled
     - [x] undo_requested
   - Client to Server
     - [ ] annul
-    - [ ] cancel
-    - [ ] chat
+    - [x] cancel
+    - [x] chat
     - [ ] chat/remove
     - [ ] clear_delayed_resign
     - [ ] conditional_moves/set
     - [x] connect
     - [ ] delayed_resign
     - [x] disconnect
     - [ ] latency
     - [ ] log
     - [x] move
-    - [ ] pause
+    - [x] pause
     - [ ] removed_stones/accept
     - [ ] removed_stones/reject
     - [ ] removed_stones/set
     - [x] resign
-    - [ ] resume
+    - [x] resume
     - [ ] timed_out
     - [x] undo/accept
-    - [ ] undo/cancel
-    - [ ] undo/request
+    - [x] undo/cancel
+    - [x] undo/request
 - [x] Implement proper challenge creation
 - [x] Create open challenge
 - [ ] Handle accepting / rejecting counting
```

### Comparing `ogsapi-0.5.0/README.md` & `ogsapi-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ```bash
 pip3 uninstall python-engineio python-socketio
 pip3 install -r requirements.txt
 ```
 ## Usage
 
 ```python
-from ogsapi.api import OGSClient
+from ogsapi.client import OGSClient
 
 ogs = OGSClient('your_client_id', 'your_client_secret', 'your_username', 'your_password')
 ```
 This will authenticate you to OGS using your API credentials, and connect you to the Realtime API Socket. You can now call the usable functions.
 
 ## Implemented API Functions
 *NOTE* All usernames are case sensitive
@@ -143,31 +143,31 @@
     - [ ] reset
     - [ ] reset-chats
     - [x] undo_accepted
     - [x] undo_canceled
     - [x] undo_requested
   - Client to Server
     - [ ] annul
-    - [ ] cancel
-    - [ ] chat
+    - [x] cancel
+    - [x] chat
     - [ ] chat/remove
     - [ ] clear_delayed_resign
     - [ ] conditional_moves/set
     - [x] connect
     - [ ] delayed_resign
     - [x] disconnect
     - [ ] latency
     - [ ] log
     - [x] move
-    - [ ] pause
+    - [x] pause
     - [ ] removed_stones/accept
     - [ ] removed_stones/reject
     - [ ] removed_stones/set
     - [x] resign
-    - [ ] resume
+    - [x] resume
     - [ ] timed_out
     - [x] undo/accept
-    - [ ] undo/cancel
-    - [ ] undo/request
+    - [x] undo/cancel
+    - [x] undo/request
 - [x] Implement proper challenge creation
 - [x] Create open challenge
 - [ ] Handle accepting / rejecting counting
```

### Comparing `ogsapi-0.5.0/pyproject.toml` & `ogsapi-0.6.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `ogsapi-0.5.0/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.6.0/src/ogsapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.5.0
+Version: 0.6.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -43,15 +43,15 @@
 ```bash
 pip3 uninstall python-engineio python-socketio
 pip3 install -r requirements.txt
 ```
 ## Usage
 
 ```python
-from ogsapi.api import OGSClient
+from ogsapi.client import OGSClient
 
 ogs = OGSClient('your_client_id', 'your_client_secret', 'your_username', 'your_password')
 ```
 This will authenticate you to OGS using your API credentials, and connect you to the Realtime API Socket. You can now call the usable functions.
 
 ## Implemented API Functions
 *NOTE* All usernames are case sensitive
@@ -155,31 +155,31 @@
     - [ ] reset
     - [ ] reset-chats
     - [x] undo_accepted
     - [x] undo_canceled
     - [x] undo_requested
   - Client to Server
     - [ ] annul
-    - [ ] cancel
-    - [ ] chat
+    - [x] cancel
+    - [x] chat
     - [ ] chat/remove
     - [ ] clear_delayed_resign
     - [ ] conditional_moves/set
     - [x] connect
     - [ ] delayed_resign
     - [x] disconnect
     - [ ] latency
     - [ ] log
     - [x] move
-    - [ ] pause
+    - [x] pause
     - [ ] removed_stones/accept
     - [ ] removed_stones/reject
     - [ ] removed_stones/set
     - [x] resign
-    - [ ] resume
+    - [x] resume
     - [ ] timed_out
     - [x] undo/accept
-    - [ ] undo/cancel
-    - [ ] undo/request
+    - [x] undo/cancel
+    - [x] undo/request
 - [x] Implement proper challenge creation
 - [x] Create open challenge
 - [ ] Handle accepting / rejecting counting
```

