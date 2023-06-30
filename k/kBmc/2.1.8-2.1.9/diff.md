# Comparing `tmp/kBmc-2.1.8.tar.gz` & `tmp/kBmc-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kBmc-2.1.8.tar", last modified: Sun Dec 19 05:13:27 2021, max compression
+gzip compressed data, was "dist/kBmc-2.1.9.tar", last modified: Sun Dec 19 05:30:59 2021, max compression
```

## Comparing `kBmc-2.1.8.tar` & `kBmc-2.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-19 05:13:27.000000 kBmc-2.1.8/
-drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-19 05:13:27.000000 kBmc-2.1.8/kBmc/
--rw-r--r--   0 kage      (1000) kage      (1000)    70182 2021-12-19 05:13:03.000000 kBmc-2.1.8/kBmc/__init__.py
-drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-19 05:13:27.000000 kBmc-2.1.8/kBmc.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)     3372 2021-12-19 05:13:27.000000 kBmc-2.1.8/kBmc.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      147 2021-12-19 05:13:27.000000 kBmc-2.1.8/kBmc.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2021-12-19 05:13:27.000000 kBmc-2.1.8/kBmc.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        5 2021-12-19 05:13:27.000000 kBmc-2.1.8/kBmc.egg-info/top_level.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.1.8/README.md
--rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.1.8/setup.py
--rw-rw-r--   0 kage      (1000) kage      (1000)     3372 2021-12-19 05:13:27.000000 kBmc-2.1.8/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)       38 2021-12-19 05:13:27.000000 kBmc-2.1.8/setup.cfg
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-19 05:30:59.000000 kBmc-2.1.9/
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-19 05:30:59.000000 kBmc-2.1.9/kBmc/
+-rw-r--r--   0 kage      (1000) kage      (1000)    70198 2021-12-19 05:30:38.000000 kBmc-2.1.9/kBmc/__init__.py
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2021-12-19 05:30:59.000000 kBmc-2.1.9/kBmc.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     3372 2021-12-19 05:30:59.000000 kBmc-2.1.9/kBmc.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      147 2021-12-19 05:30:59.000000 kBmc-2.1.9/kBmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2021-12-19 05:30:59.000000 kBmc-2.1.9/kBmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        5 2021-12-19 05:30:59.000000 kBmc-2.1.9/kBmc.egg-info/top_level.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.1.9/README.md
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.1.9/setup.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)     3372 2021-12-19 05:30:59.000000 kBmc-2.1.9/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)       38 2021-12-19 05:30:59.000000 kBmc-2.1.9/setup.cfg
```

### Comparing `kBmc-2.1.8/kBmc/__init__.py` & `kBmc-2.1.9/kBmc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,15 +575,15 @@
                         if rc[0]:
                             rc=True,km.findstr(rc[1],'- Boot Device Selector : (\w.*)')[0]
                     elif mode == 'status':
                         if km.krc(rc,chk=True):
                             status='No override'
                             efi=False
                             persistent=False
-                            for ii in rc[1].split('\n'):
+                            for ii in km.get_value(rc[1],1).split('\n'):
                                 if 'Options apply to all future boots' in ii:
                                     persistent=True
                                 elif 'BIOS EFI boot' in ii:
                                     efi=True
                                 elif 'Boot Device Selector :' in ii:
                                     status=ii.split(':')[1]
                                     break
```

### Comparing `kBmc-2.1.8/kBmc.egg-info/PKG-INFO` & `kBmc-2.1.9/kBmc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.1.8
+Version: 2.1.9
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Description: - Install
         ```javascript
         pip install kBmc
```

### Comparing `kBmc-2.1.8/README.md` & `kBmc-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kBmc-2.1.8/setup.py` & `kBmc-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `kBmc-2.1.8/PKG-INFO` & `kBmc-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.1.8
+Version: 2.1.9
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Description: - Install
         ```javascript
         pip install kBmc
```

