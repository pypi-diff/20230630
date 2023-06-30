# Comparing `tmp/micropython-captive-dhcp-server-0.0.3.dev0.tar.gz` & `tmp/micropython-captive-dhcp-server-0.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-captive-dhcp-server-0.0.3.dev0.tar", last modified: Thu Jun 29 20:20:05 2023, max compression
+gzip compressed data, was "micropython-captive-dhcp-server-0.0.4.dev0.tar", last modified: Fri Jun 30 10:24:01 2023, max compression
```

## Comparing `micropython-captive-dhcp-server-0.0.3.dev0.tar` & `micropython-captive-dhcp-server-0.0.4.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:20:05.964919 micropython-captive-dhcp-server-0.0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 20:20:05.964919 micropython-captive-dhcp-server-0.0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:20:05.960919 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:20:05.964919 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 20:20:05.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-29 20:20:05.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:20:05.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:20:05.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 20:20:05.000000 micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-29 20:20:05.964919 micropython-captive-dhcp-server-0.0.3.dev0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-29 20:20:02.000000 micropython-captive-dhcp-server-0.0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:24:01.475311 micropython-captive-dhcp-server-0.0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 10:24:01.475311 micropython-captive-dhcp-server-0.0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:24:01.475311 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:24:01.475311 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 10:24:01.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-30 10:24:01.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:24:01.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:24:01.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 10:24:01.000000 micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-30 10:24:01.475311 micropython-captive-dhcp-server-0.0.4.dev0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-30 10:23:55.000000 micropython-captive-dhcp-server-0.0.4.dev0/setup.py
```

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/LICENSE` & `micropython-captive-dhcp-server-0.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/PKG-INFO` & `micropython-captive-dhcp-server-0.0.4.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-captive-dhcp-server
-Version: 0.0.3.dev0
+Version: 0.0.4.dev0
 Summary: Micropython asyncio simplistic dhcp server for use with captive portals
 Author-email: Patrick McAndrew <patrick@urg.name>
 Project-URL: Homepage, https://github.com/urg/micropython-captive-dhcp-server
 Project-URL: Repository, https://github.com/urg/micropython-captive-dhcp-server
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server/packet.py` & `micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server/packet.py`

 * *Files identical despite different names*

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server/server.py` & `micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,30 +40,31 @@
             "255.255.255.255", 68, socket.AF_INET, socket.SOCK_DGRAM
         )[0][4]
         print(f"Broadcasting Response: {reply}")
         udpb.sendto(reply, broadcast_addr)
         udpb.close()
 
     async def run(self, server_ip: str, netmask: str):
-        try:
-            udps = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        udps = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        udps.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        udps.setblocking(False)
 
-            # set non-blocking otherwise execution will stop at 'recvfrom'
-            # until a connection is received and this will prevent the other
-            # async threads from running
-            udps.setblocking(False)
-
-            addr = socket.getaddrinfo("0.0.0.0", 67, socket.AF_INET, socket.SOCK_DGRAM)[
-                0
-            ][4]
-            udps.bind(addr)
-            print("Starting server on port 67")
-        except Exception:
-            print("Failed to bind to port")
-            return
+        bound = False
+        while not bound:
+            try:
+                gc.collect()
+                addr = socket.getaddrinfo(
+                    "0.0.0.0", 67, socket.AF_INET, socket.SOCK_DGRAM
+                )[0][4]
+                udps.bind(addr)
+                print("Starting server on port 67")
+                bound = True
+            except Exception as e:
+                print(f"Failed to bind to port {e}")
+                time.sleep(0.5)
 
         while True:
             try:
                 gc.collect()
 
                 data, addr = udps.recvfrom(2048)
                 print("Incoming data...")
@@ -95,15 +96,7 @@
             except OSError:
                 await asyncio.sleep_ms(500)
 
             except Exception:
                 await asyncio.sleep_ms(500)
 
         udps.close()
-
-
-if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
-    server = CaptiveDhcpServer()
-    loop.create_task(server.run("192.168.4.1", "255.255.255.0"))
-    loop.run_forever()
-    loop.close()
```

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/micropython_captive_dhcp_server.egg-info/PKG-INFO` & `micropython-captive-dhcp-server-0.0.4.dev0/micropython_captive_dhcp_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-captive-dhcp-server
-Version: 0.0.3.dev0
+Version: 0.0.4.dev0
 Summary: Micropython asyncio simplistic dhcp server for use with captive portals
 Author-email: Patrick McAndrew <patrick@urg.name>
 Project-URL: Homepage, https://github.com/urg/micropython-captive-dhcp-server
 Project-URL: Repository, https://github.com/urg/micropython-captive-dhcp-server
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/pyproject.toml` & `micropython-captive-dhcp-server-0.0.4.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micropython-captive-dhcp-server"
-version = "0.0.3.dev"
+version = "0.0.4.dev"
 description = "Micropython asyncio simplistic dhcp server for use with captive portals"
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "License :: OSI Approved :: MIT License",
```

### Comparing `micropython-captive-dhcp-server-0.0.3.dev0/setup.cfg` & `micropython-captive-dhcp-server-0.0.4.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = "micropython-captive-dhcp-server"
-version = "0.0.3.dev"
+version = "0.0.4.dev"
 description = "Micropython asyncio simplistic dhcp server for use with captive portals"
 classifiers = 
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: Implementation :: MicroPython
 	License :: OSI Approved :: MIT License
```

