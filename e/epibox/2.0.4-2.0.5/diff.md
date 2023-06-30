# Comparing `tmp/epibox-2.0.4.tar.gz` & `tmp/epibox-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epibox-2.0.4.tar", last modified: Fri Jun 30 14:00:24 2023, max compression
+gzip compressed data, was "epibox-2.0.5.tar", last modified: Fri Jun 30 15:16:06 2023, max compression
```

## Comparing `epibox-2.0.4.tar` & `epibox-2.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.481168 epibox-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-30 14:00:12.000000 epibox-2.0.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-30 14:00:12.000000 epibox-2.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 14:00:12.000000 epibox-2.0.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 14:00:12.000000 epibox-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 14:00:12.000000 epibox-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 14:00:24.481168 epibox-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-30 14:00:12.000000 epibox-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.477168 epibox-2.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 14:00:12.000000 epibox-2.0.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.477168 epibox-2.0.4/epibox/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.477168 epibox-2.0.4/epibox/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/get_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/read_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/run_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/common/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/config_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.481168 epibox-2.0.4/epibox/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/devices/connect_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/devices/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/devices/manage_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.481168 epibox-2.0.4/epibox/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/exceptions/exception_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/exceptions/system_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.481168 epibox-2.0.4/epibox/mqtt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/mqtt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/mqtt_manager/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/mqtt_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.481168 epibox-2.0.4/epibox/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-30 14:00:12.000000 epibox-2.0.4/epibox/run/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:00:24.477168 epibox-2.0.4/epibox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 14:00:24.000000 epibox-2.0.4/epibox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:00:24.481168 epibox-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-30 14:00:12.000000 epibox-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.202814 epibox-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-30 15:15:54.000000 epibox-2.0.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-30 15:15:54.000000 epibox-2.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 15:15:54.000000 epibox-2.0.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 15:15:54.000000 epibox-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 15:15:54.000000 epibox-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 15:16:06.202814 epibox-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-30 15:15:54.000000 epibox-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.194814 epibox-2.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 15:15:54.000000 epibox-2.0.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.194814 epibox-2.0.5/epibox/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.198814 epibox-2.0.5/epibox/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/get_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/read_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/run_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/common/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/config_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.198814 epibox-2.0.5/epibox/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/devices/connect_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/devices/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/devices/manage_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.202814 epibox-2.0.5/epibox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/exceptions/exception_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/exceptions/system_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.202814 epibox-2.0.5/epibox/mqtt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/mqtt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/mqtt_manager/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/mqtt_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.202814 epibox-2.0.5/epibox/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-30 15:15:54.000000 epibox-2.0.5/epibox/run/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:16:06.198814 epibox-2.0.5/epibox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 15:16:06.000000 epibox-2.0.5/epibox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-30 15:16:06.000000 epibox-2.0.5/epibox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:16:06.000000 epibox-2.0.5/epibox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 15:16:06.000000 epibox-2.0.5/epibox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:16:05.000000 epibox-2.0.5/epibox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-30 15:16:06.000000 epibox-2.0.5/epibox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 15:16:06.000000 epibox-2.0.5/epibox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:16:06.202814 epibox-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-30 15:15:54.000000 epibox-2.0.5/setup.py
```

### Comparing `epibox-2.0.4/CONTRIBUTING.rst` & `epibox-2.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/LICENSE` & `epibox-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/PKG-INFO` & `epibox-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.4
+Version: 2.0.5
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.4/README.md` & `epibox-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/docs/Makefile` & `epibox-2.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/docs/conf.py` & `epibox-2.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/docs/installation.rst` & `epibox-2.0.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/docs/make.bat` & `epibox-2.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/common/get_defaults.py` & `epibox-2.0.5/epibox/common/get_defaults.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/common/open_file.py` & `epibox-2.0.5/epibox/common/open_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/common/process_data.py` & `epibox-2.0.5/epibox/common/process_data.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/common/read_modules.py` & `epibox-2.0.5/epibox/common/read_modules.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/common/run_system.py` & `epibox-2.0.5/epibox/common/run_system.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/common/setup.py` & `epibox-2.0.5/epibox/common/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,17 @@
     if opt["initial_dir"] == "EpiBOX Core":
         drive_path = os.path.join(Path.home(), "Documents", "EpiBOX Core")
         opt["initial_dir"] = os.path.join(drive_path, "acquisitions")
 
     else:
         if platform == "linux" or platform == "linux2":
             # linux
-            drive_path = os.path.join("/media", os.getlogin(), opt["initial_dir"])
+            import pwd
+            drive_path = os.path.join(
+                "/media", pwd.getpwuid(os.getuid())[0], opt["initial_dir"])
         elif platform == "darwin":
             # macos
             drive_path = os.path.join("/Volumes", opt["initial_dir"])
         else:
             drive_path = opt["initial_dir"]
 
         init_connect_time = time.time()
@@ -145,12 +147,13 @@
 
             if os.path.isdir(drive_path):
                 opt["initial_dir"] = os.path.join(drive_path, "acquisitions")
                 break
 
             else:
                 if time.time() - init_connect_time > 3 * i:
-                    message_info = client.publish("rpi", str(["INSERT STORAGE"]))
+                    message_info = client.publish(
+                        "rpi", str(["INSERT STORAGE"]))
                     if message_info.rc == 4:
                         raise MQTTConnectionError
 
     return opt
```

### Comparing `epibox-2.0.4/epibox/common/write_file.py` & `epibox-2.0.5/epibox/common/write_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/devices/connect_device.py` & `epibox-2.0.5/epibox/devices/connect_device.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/devices/header.py` & `epibox-2.0.5/epibox/devices/header.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/devices/manage_devices.py` & `epibox-2.0.5/epibox/devices/manage_devices.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/exceptions/exception_manager.py` & `epibox-2.0.5/epibox/exceptions/exception_manager.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/exceptions/system_exceptions.py` & `epibox-2.0.5/epibox/exceptions/system_exceptions.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox/mqtt_manager/message_handler.py` & `epibox-2.0.5/epibox/mqtt_manager/message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 def send_default(client):
 
     ######## Available drives ########
     listDrives = ["DRIVES"]
 
     if platform == "linux" or platform == "linux2":
         # linux
-        drive_path = os.path.join("/media", os.getlogin())
+        import pwd
+        drive_path = os.path.join("/media", pwd.getpwuid(os.getuid())[0])
         drives = [os.path.join(drive_path, d) for d in os.listdir(drive_path)]
     elif platform == "darwin":
         # macos
         drive_path = "/Volumes"
         drives = [os.path.join(drive_path, d) for d in os.listdir(drive_path)]
     else:
         import win32api
@@ -72,15 +73,14 @@
     )  # raises ValueError and TypeError
     if message_info.rc == 4:
         raise MQTTConnectionError
 
 
 def on_message(client, userdata, message):
 
-    username = os.getlogin()
     message = str(message.payload.decode("utf-8"))
     message = ast.literal_eval(message)
 
     if message[0] == "RESTART":
         # client.loop_stop()
         # client.keepAlive = False
         config_debug.log("Not sure what to do here yet")
@@ -114,21 +114,20 @@
         send_default(client)
 
     ######## New default configuration ########
 
     elif message[0] == "NEW CONFIG DEFAULT":
         defaults = get_default()
 
-        username = os.getlogin()
-
         for key in message[1].keys():
             defaults[key] = message[1][key]
 
         with open(
-            os.path.join(Path.home(), "Documents", "EpiBOX Core", "args.json"), "w+"
+            os.path.join(Path.home(), "Documents",
+                         "EpiBOX Core", "args.json"), "w+"
         ) as json_file:
             json.dump(defaults, json_file)
 
         msg = json.dumps(["RECEIVED DEFAULT"])
         message_info = client.publish(topic="rpi", qos=2, payload=msg)
         if message_info.rc == 4:
             raise MQTTConnectionError
```

### Comparing `epibox-2.0.4/epibox/run/run.py` & `epibox-2.0.5/epibox/run/run.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/epibox.egg-info/PKG-INFO` & `epibox-2.0.5/epibox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.4
+Version: 2.0.5
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.4/epibox.egg-info/SOURCES.txt` & `epibox-2.0.5/epibox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epibox-2.0.4/setup.py` & `epibox-2.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     include_package_data=True,
     keywords=["epibox", "signal acquisition", "Raspberry Pi"],
     name="epibox",
     packages=find_packages(include=["epibox", "epibox.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/anascacais/epibox",
-    version="2.0.4",
+    version="2.0.5",
     zip_safe=False,
 )
```

