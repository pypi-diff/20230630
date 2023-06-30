# Comparing `tmp/asterisk-plus-agent-2.5.1.tar.gz` & `tmp/asterisk-plus-agent-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asterisk-plus-agent-2.5.1.tar", last modified: Wed Jun 28 15:16:24 2023, max compression
+gzip compressed data, was "asterisk-plus-agent-3.0.0.tar", last modified: Fri Jun 30 13:09:40 2023, max compression
```

## Comparing `asterisk-plus-agent-2.5.1.tar` & `asterisk-plus-agent-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-28 15:16:24.905399 asterisk-plus-agent-2.5.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1098 2023-06-28 15:16:24.905399 asterisk-plus-agent-2.5.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      453 2023-06-27 11:21:53.000000 asterisk-plus-agent-2.5.1/README.rst
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-28 15:16:24.905399 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1098 2023-06-28 15:16:24.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      344 2023-06-28 15:16:24.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-28 15:16:24.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-06-28 15:16:24.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-27 11:25:54.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2023-06-28 15:16:24.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       20 2023-06-28 15:16:24.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)    22608 2023-06-28 14:47:29.000000 asterisk-plus-agent-2.5.1/asterisk_plus_agent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-28 15:16:24.905399 asterisk-plus-agent-2.5.1/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1659 2023-06-28 14:47:29.000000 asterisk-plus-agent-2.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:09:40.376874 asterisk-plus-agent-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-06-30 13:09:40.376874 asterisk-plus-agent-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-06-30 13:09:34.000000 asterisk-plus-agent-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 13:09:40.376874 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-30 13:09:40.000000 asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 13:09:40.376874 asterisk-plus-agent-3.0.0/setup.cfg
```

### Comparing `asterisk-plus-agent-2.5.1/PKG-INFO` & `asterisk-plus-agent-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asterisk-plus-agent
-Version: 2.5.1
+Version: 3.0.0
 Summary: Asterisk Plus PBX Agent
 Home-page: https://odoopbx.com
 Author: Odooist
 Author-email: odooist@gmail.com
 License: Odoo Enterprise Edition License v1.0
 Description: =======================================
         The Asterisk Plus PBX Agent application
@@ -14,15 +14,17 @@
         
         Latest Asterisk Plus modules require the latest Agent. 
         
         If you have outdates Odoo modules see the release history for the corresponding  version and install it.
         
         For example, to install version 1.1 enter the following command:
         
-        pip3 install asterisk-plus-agent==1.1
+        pip3 install asterisk-plus-agent==2.5
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
```

### Comparing `asterisk-plus-agent-2.5.1/asterisk_plus_agent.egg-info/PKG-INFO` & `asterisk-plus-agent-3.0.0/asterisk_plus_agent.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asterisk-plus-agent
-Version: 2.5.1
+Version: 3.0.0
 Summary: Asterisk Plus PBX Agent
 Home-page: https://odoopbx.com
 Author: Odooist
 Author-email: odooist@gmail.com
 License: Odoo Enterprise Edition License v1.0
 Description: =======================================
         The Asterisk Plus PBX Agent application
@@ -14,15 +14,17 @@
         
         Latest Asterisk Plus modules require the latest Agent. 
         
         If you have outdates Odoo modules see the release history for the corresponding  version and install it.
         
         For example, to install version 1.1 enter the following command:
         
-        pip3 install asterisk-plus-agent==1.1
+        pip3 install asterisk-plus-agent==2.5
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
```

