# Comparing `tmp/rosetta-ce-1.3.4.tar.gz` & `tmp/rosetta-ce-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.4.tar", last modified: Fri Jun 30 09:03:52 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.5.tar", last modified: Fri Jun 30 09:38:33 2023, max compression
```

## Comparing `rosetta-ce-1.3.4.tar` & `rosetta-ce-1.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.272039 rosetta-ce-1.3.4/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.4/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:03:52.271760 rosetta-ce-1.3.4/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.4/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.264836 rosetta-ce-1.3.4/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.4/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.266949 rosetta-ce-1.3.4/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.4/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.4/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.4/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.4/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.4/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    39105 2023-06-30 09:03:21.000000 rosetta-ce-1.3.4/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.4/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.269365 rosetta-ce-1.3.4/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 09:03:52.272080 rosetta-ce-1.3.4/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 09:03:32.000000 rosetta-ce-1.3.4/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.271228 rosetta-ce-1.3.4/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.4/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.4/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.4/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.690719 rosetta-ce-1.3.5/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.5/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:38:33.690377 rosetta-ce-1.3.5/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.5/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.684242 rosetta-ce-1.3.5/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.5/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.686149 rosetta-ce-1.3.5/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.5/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.5/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.5/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.5/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.5/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    39169 2023-06-30 09:38:06.000000 rosetta-ce-1.3.5/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.5/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.688181 rosetta-ce-1.3.5/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 09:38:33.690764 rosetta-ce-1.3.5/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 09:38:19.000000 rosetta-ce-1.3.5/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.689791 rosetta-ce-1.3.5/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.5/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.5/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.5/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.4/LICENSE` & `rosetta-ce-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/PKG-INFO` & `rosetta-ce-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.4
+Version: 1.3.5
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.4/README.md` & `rosetta-ce-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/rosetta/constants/sensors.py` & `rosetta-ce-1.3.5/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/rosetta/constants/sources.py` & `rosetta-ce-1.3.5/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/rosetta/constants/systems.py` & `rosetta-ce-1.3.5/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/rosetta/rconverter.py` & `rosetta-ce-1.3.5/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/rosetta/rfaker.py` & `rosetta-ce-1.3.5/rosetta/rfaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,16 @@
                 action = random.choice(observables.action) if observables and observables.action \
                     else random.choice(ACTIONS)
                 generic_cef = f"CEF:0|{vendor}|{product}|{version}|{log_id}|{timestamp}|{severity}|src_ip={src_ip} " \
                               f"src_port={src_port} dst_ip={dst_ip} dst_port={dst_port} proto={protocol} " \
                               f"rule={rule_id} act={action}"
                 if observables:
                     for observable, observable_value in vars(observables).items():
-                        generic_cef += f" {observable}={observable_value}"
+                        if observable_value:
+                            generic_cef += f" {observable}={random.choice(observable_value)}"
                 cef_messages.append(generic_cef)
         return cef_messages
 
     @classmethod
     def leef(cls, count, timestamp: Optional[datetime] = None, vendor: Optional[str] = None,
              product: Optional[str] = None, version: Optional[str] = None,
              observables: Optional[Observables] = None) -> List[str]:
```

### Comparing `rosetta-ce-1.3.4/rosetta/rsender.py` & `rosetta-ce-1.3.5/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.5/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.4
+Version: 1.3.5
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.4/setup.py` & `rosetta-ce-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.4",
+    version="1.3.5",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.4/tests/test_rconverter.py` & `rosetta-ce-1.3.5/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/tests/test_rfaker.py` & `rosetta-ce-1.3.5/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.4/tests/test_rsender.py` & `rosetta-ce-1.3.5/tests/test_rsender.py`

 * *Files identical despite different names*

