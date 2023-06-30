# Comparing `tmp/rosetta-ce-1.3.1.tar.gz` & `tmp/rosetta-ce-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.1.tar", last modified: Thu Jun 29 15:23:42 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.2.tar", last modified: Thu Jun 29 15:55:58 2023, max compression
```

## Comparing `rosetta-ce-1.3.1.tar` & `rosetta-ce-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.410446 rosetta-ce-1.3.1/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.1/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:23:42.410121 rosetta-ce-1.3.1/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.1/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.404608 rosetta-ce-1.3.1/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.1/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.406458 rosetta-ce-1.3.1/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.1/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.1/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.1/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.1/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.1/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    33530 2023-06-29 15:05:33.000000 rosetta-ce-1.3.1/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8454 2023-06-29 15:22:28.000000 rosetta-ce-1.3.1/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.408362 rosetta-ce-1.3.1/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 15:23:42.410504 rosetta-ce-1.3.1/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 15:22:47.000000 rosetta-ce-1.3.1/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.409611 rosetta-ce-1.3.1/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.1/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.1/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.1/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:55:58.045958 rosetta-ce-1.3.2/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.2/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:55:58.045611 rosetta-ce-1.3.2/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.2/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:55:58.037195 rosetta-ce-1.3.2/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.2/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:55:58.039345 rosetta-ce-1.3.2/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.2/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.2/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.2/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.2/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.2/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    33530 2023-06-29 15:05:33.000000 rosetta-ce-1.3.2/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.2/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:55:58.043299 rosetta-ce-1.3.2/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:55:57.000000 rosetta-ce-1.3.2/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 15:55:58.000000 rosetta-ce-1.3.2/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 15:55:57.000000 rosetta-ce-1.3.2/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 15:55:57.000000 rosetta-ce-1.3.2/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 15:55:57.000000 rosetta-ce-1.3.2/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 15:55:58.046006 rosetta-ce-1.3.2/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 15:55:28.000000 rosetta-ce-1.3.2/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:55:58.044736 rosetta-ce-1.3.2/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.2/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.2/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.2/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.1/LICENSE` & `rosetta-ce-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/PKG-INFO` & `rosetta-ce-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.1
+Version: 1.3.2
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.1/README.md` & `rosetta-ce-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/rosetta/constants/sensors.py` & `rosetta-ce-1.3.2/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/rosetta/constants/sources.py` & `rosetta-ce-1.3.2/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/rosetta/constants/systems.py` & `rosetta-ce-1.3.2/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/rosetta/rconverter.py` & `rosetta-ce-1.3.2/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/rosetta/rfaker.py` & `rosetta-ce-1.3.2/rosetta/rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/rosetta/rsender.py` & `rosetta-ce-1.3.2/rosetta/rsender.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
                         print(f"Worker: {self.worker_name} sending log message to {ip_address} ")
                         sock.sendto(fake_message[0].encode(), (ip_address, int(port)))
                 elif self.data_type in ["JSON", "INCIDENT"]:
                     if self.data_type == "JSON":
                         fake_message = Events.json(count=1, timestamp=self.datetime_obj, observables=self.observables)
                     if self.data_type == "INCIDENT":
                         fake_message = [{
-                            "alert": Events.incidents(count=1, observables=self.observables, fields=self.fields)
+                            "alert": Events.incidents(count=1, observables=self.observables, vendor=self.vendor,
+                                                      version=self.version, product=self.product, fields=self.fields)
                         }]
                     if '://' not in self.destination:
                         url = 'http://' + self.destination
                     else:
                         url = self.destination
                     warnings.filterwarnings("ignore", category=InsecureRequestWarning)
                     print(f"Worker: {self.worker_name} sending log message to {url} ")
```

### Comparing `rosetta-ce-1.3.1/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.2/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.1
+Version: 1.3.2
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.1/setup.py` & `rosetta-ce-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.1",
+    version="1.3.2",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.1/tests/test_rconverter.py` & `rosetta-ce-1.3.2/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/tests/test_rfaker.py` & `rosetta-ce-1.3.2/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.1/tests/test_rsender.py` & `rosetta-ce-1.3.2/tests/test_rsender.py`

 * *Files identical despite different names*

