# Comparing `tmp/scs-host-posix-2.5.2.tar.gz` & `tmp/scs-host-posix-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-host-posix-2.5.2.tar", last modified: Mon Jun 26 13:23:39 2023, max compression
+gzip compressed data, was "scs-host-posix-2.5.3.tar", last modified: Fri Jun 30 08:17:40 2023, max compression
```

## Comparing `scs-host-posix-2.5.2.tar` & `scs-host-posix-2.5.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1212 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      504 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)       16 2023-06-26 13:23:15.000000 scs-host-posix-2.5.2/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2049 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.994645 scs-host-posix-2.5.2/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/src/scs_host/
--rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-26 13:23:15.000000 scs-host-posix-2.5.2/src/scs_host/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/src/scs_host/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1865 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/client/http_streaming_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4757 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/client/mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3209 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/client/sftp_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/src/scs_host/comms/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/comms/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4972 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/comms/domain_socket.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3433 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/comms/network_socket.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3821 2023-06-26 09:33:48.000000 scs-host-posix-2.5.2/src/scs_host/comms/stdio.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/src/scs_host/sys/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/sys/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2463 2022-08-17 09:53:07.000000 scs-host-posix-2.5.2/src/scs_host/sys/host.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:23:38.998645 scs-host-posix-2.5.2/src/scs_host_posix.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1212 2023-06-26 13:23:38.000000 scs-host-posix-2.5.2/src/scs_host_posix.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      633 2023-06-26 13:23:38.000000 scs-host-posix-2.5.2/src/scs_host_posix.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 13:23:38.000000 scs-host-posix-2.5.2/src/scs_host_posix.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       16 2023-06-26 13:23:38.000000 scs-host-posix-2.5.2/src/scs_host_posix.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-26 13:23:38.000000 scs-host-posix-2.5.2/src/scs_host_posix.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1212 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      504 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-30 08:17:13.000000 scs-host-posix-2.5.3/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2049 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.089055 scs-host-posix-2.5.3/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.089055 scs-host-posix-2.5.3/src/scs_host/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-30 08:17:13.000000 scs-host-posix-2.5.3/src/scs_host/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/src/scs_host/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1865 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/client/http_streaming_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4757 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/client/mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3209 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/client/sftp_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/src/scs_host/comms/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/comms/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4972 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/comms/domain_socket.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3433 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/comms/network_socket.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3821 2023-06-26 09:33:48.000000 scs-host-posix-2.5.3/src/scs_host/comms/stdio.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/src/scs_host/sys/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/sys/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2463 2022-08-17 09:53:07.000000 scs-host-posix-2.5.3/src/scs_host/sys/host.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-30 08:17:40.093055 scs-host-posix-2.5.3/src/scs_host_posix.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1212 2023-06-30 08:17:40.000000 scs-host-posix-2.5.3/src/scs_host_posix.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      592 2023-06-30 08:17:40.000000 scs-host-posix-2.5.3/src/scs_host_posix.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-30 08:17:40.000000 scs-host-posix-2.5.3/src/scs_host_posix.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-30 08:17:40.000000 scs-host-posix-2.5.3/src/scs_host_posix.egg-info/top_level.txt
```

### Comparing `scs-host-posix-2.5.2/LICENSE` & `scs-host-posix-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/PKG-INFO` & `scs-host-posix-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-host-posix
-Version: 2.5.2
+Version: 2.5.3
 Summary: Host abstractions for data consumers running POSIX-compliant operating systems, including Windows 10.
 Home-page: https://github.com/south-coast-science/scs_host_posix
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-host-posix-2.5.2/setup.py` & `scs-host-posix-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/client/http_streaming_client.py` & `scs-host-posix-2.5.3/src/scs_host/client/http_streaming_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/client/mqtt_client.py` & `scs-host-posix-2.5.3/src/scs_host/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/client/sftp_client.py` & `scs-host-posix-2.5.3/src/scs_host/client/sftp_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/comms/domain_socket.py` & `scs-host-posix-2.5.3/src/scs_host/comms/domain_socket.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/comms/network_socket.py` & `scs-host-posix-2.5.3/src/scs_host/comms/network_socket.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/comms/stdio.py` & `scs-host-posix-2.5.3/src/scs_host/comms/stdio.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host/sys/host.py` & `scs-host-posix-2.5.3/src/scs_host/sys/host.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-2.5.2/src/scs_host_posix.egg-info/PKG-INFO` & `scs-host-posix-2.5.3/src/scs_host_posix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-host-posix
-Version: 2.5.2
+Version: 2.5.3
 Summary: Host abstractions for data consumers running POSIX-compliant operating systems, including Windows 10.
 Home-page: https://github.com/south-coast-science/scs_host_posix
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-host-posix-2.5.2/src/scs_host_posix.egg-info/SOURCES.txt` & `scs-host-posix-2.5.3/src/scs_host_posix.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 src/scs_host/comms/network_socket.py
 src/scs_host/comms/stdio.py
 src/scs_host/sys/__init__.py
 src/scs_host/sys/host.py
 src/scs_host_posix.egg-info/PKG-INFO
 src/scs_host_posix.egg-info/SOURCES.txt
 src/scs_host_posix.egg-info/dependency_links.txt
-src/scs_host_posix.egg-info/requires.txt
 src/scs_host_posix.egg-info/top_level.txt
```

