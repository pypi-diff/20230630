# Comparing `tmp/epibox-2.0.2.tar.gz` & `tmp/epibox-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epibox-2.0.2.tar", last modified: Thu Jun 29 17:29:13 2023, max compression
+gzip compressed data, was "epibox-2.0.3.tar", last modified: Fri Jun 30 13:40:50 2023, max compression
```

## Comparing `epibox-2.0.2.tar` & `epibox-2.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.009562 epibox-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 17:29:03.000000 epibox-2.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-29 17:29:03.000000 epibox-2.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 17:29:03.000000 epibox-2.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 17:29:03.000000 epibox-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-29 17:29:03.000000 epibox-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-29 17:29:13.005562 epibox-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-29 17:29:03.000000 epibox-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/get_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/read_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/run_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/config_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/connect_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/manage_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/exceptions/exception_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/exceptions/system_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/mqtt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/mqtt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/mqtt_manager/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/mqtt_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/run/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-29 17:29:13.000000 epibox-2.0.2/epibox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:29:13.009562 epibox-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-29 17:29:03.000000 epibox-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-30 13:40:41.000000 epibox-2.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-30 13:40:41.000000 epibox-2.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 13:40:41.000000 epibox-2.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 13:40:41.000000 epibox-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 13:40:41.000000 epibox-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 13:40:50.963282 epibox-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-30 13:40:41.000000 epibox-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.959282 epibox-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 13:40:41.000000 epibox-2.0.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.959282 epibox-2.0.3/epibox/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/epibox/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/get_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/read_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/run_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/common/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/config_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/epibox/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/devices/connect_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/devices/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/devices/manage_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/epibox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/exceptions/exception_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/exceptions/system_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/epibox/mqtt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/mqtt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/mqtt_manager/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/mqtt_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/epibox/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-30 13:40:41.000000 epibox-2.0.3/epibox/run/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:40:50.963282 epibox-2.0.3/epibox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 13:40:50.000000 epibox-2.0.3/epibox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:40:50.963282 epibox-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-30 13:40:41.000000 epibox-2.0.3/setup.py
```

### Comparing `epibox-2.0.2/CONTRIBUTING.rst` & `epibox-2.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/LICENSE` & `epibox-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/PKG-INFO` & `epibox-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.2
+Version: 2.0.3
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.2/README.md` & `epibox-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/docs/Makefile` & `epibox-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/docs/conf.py` & `epibox-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/docs/installation.rst` & `epibox-2.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/docs/make.bat` & `epibox-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/common/get_defaults.py` & `epibox-2.0.3/epibox/common/get_defaults.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         Path.home(), "Documents", "EpiBOX Core")
     defaults_path = os.path.join(defaults_dir, "args.json")
 
     defaults = {
             "initial_dir": "EpiBOX Core",
             "fs": 1000,
             "channels": [],
-            "devices_mac": {"MAC1": "COM3"},
+            "devices_mac": {"MAC1": "34:94:54:5E:32:2E"},
             "save_raw": "true",
             "patient_id": "default",
             "service": "scientisst",
         }
 
     if os.path.isdir(defaults_dir):
```

### Comparing `epibox-2.0.2/epibox/common/open_file.py` & `epibox-2.0.3/epibox/common/open_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/common/process_data.py` & `epibox-2.0.3/epibox/common/process_data.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/common/read_modules.py` & `epibox-2.0.3/epibox/common/read_modules.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/common/run_system.py` & `epibox-2.0.3/epibox/common/run_system.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/common/setup.py` & `epibox-2.0.3/epibox/common/setup.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/common/write_file.py` & `epibox-2.0.3/epibox/common/write_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/devices/connect_device.py` & `epibox-2.0.3/epibox/devices/connect_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 )
 
 
 def connect_device(address, client, devices, service):
 
     connected = False
     devices = [d for d in devices if d]  # remove None
-    config_debug.log(f" devices: {devices}")
 
     if address in [d.address for d in devices]:
         try:
             config_debug.log(
                 f"{address} state: {[d.state()for d in devices if d.address==address]}"
             )
             connected = True
```

### Comparing `epibox-2.0.2/epibox/devices/header.py` & `epibox-2.0.3/epibox/devices/header.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/devices/manage_devices.py` & `epibox-2.0.3/epibox/devices/manage_devices.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/exceptions/exception_manager.py` & `epibox-2.0.3/epibox/exceptions/exception_manager.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/exceptions/system_exceptions.py` & `epibox-2.0.3/epibox/exceptions/system_exceptions.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/mqtt_manager/message_handler.py` & `epibox-2.0.3/epibox/mqtt_manager/message_handler.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox/run/run.py` & `epibox-2.0.3/epibox/run/run.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/epibox.egg-info/PKG-INFO` & `epibox-2.0.3/epibox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.2
+Version: 2.0.3
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.2/epibox.egg-info/SOURCES.txt` & `epibox-2.0.3/epibox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epibox-2.0.2/setup.py` & `epibox-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     include_package_data=True,
     keywords=["epibox", "signal acquisition", "Raspberry Pi"],
     name="epibox",
     packages=find_packages(include=["epibox", "epibox.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/anascacais/epibox",
-    version="2.0.2",
+    version="2.0.3",
     zip_safe=False,
 )
```

