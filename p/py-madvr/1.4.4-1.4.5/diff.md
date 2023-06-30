# Comparing `tmp/py_madvr-1.4.4.tar.gz` & `tmp/py_madvr-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.4.4.tar", last modified: Thu Jun 22 03:05:54 2023, max compression
+gzip compressed data, was "py_madvr-1.4.5.tar", last modified: Fri Jun 30 16:46:15 2023, max compression
```

## Comparing `py_madvr-1.4.4.tar` & `py_madvr-1.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.013437 py_madvr-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 03:05:39.000000 py_madvr-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-22 03:05:54.013437 py_madvr-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-22 03:05:39.000000 py_madvr-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.009437 py_madvr-1.4.4/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.009437 py_madvr-1.4.4/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-22 03:05:53.000000 py_madvr-1.4.4/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 03:05:54.000000 py_madvr-1.4.4/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:05:53.000000 py_madvr-1.4.4/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 03:05:53.000000 py_madvr-1.4.4/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:05:54.013437 py_madvr-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 03:05:39.000000 py_madvr-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.013437 py_madvr-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:39.000000 py_madvr-1.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-22 03:05:39.000000 py_madvr-1.4.4/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 16:46:01.000000 py_madvr-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 16:46:15.149544 py_madvr-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-30 16:46:01.000000 py_madvr-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-06-30 16:46:01.000000 py_madvr-1.4.5/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 16:46:15.000000 py_madvr-1.4.5/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:46:15.149544 py_madvr-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 16:46:01.000000 py_madvr-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:15.149544 py_madvr-1.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:46:01.000000 py_madvr-1.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-30 16:46:01.000000 py_madvr-1.4.5/tests/testMadVR.py
```

### Comparing `py_madvr-1.4.4/LICENSE` & `py_madvr-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.4/PKG-INFO` & `py_madvr-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.4.4
+Version: 1.4.5
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.4/madvr/commands.py` & `py_madvr-1.4.5/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.4/madvr/madvr.py` & `py_madvr-1.4.5/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,17 +339,15 @@
                     )
             except ConnectionResetError:
                 self.logger.warning(
                     "Connection reset by peer. Attempting to reconnect..."
                 )
                 await self._reconnect()
             except (AttributeError, asyncio.TimeoutError, OSError) as err:
-                self.logger.debug(
-                    "Reading notifications failed or timed out: %s", err
-                )
+                self.logger.debug("Reading notifications failed or timed out: %s", err)
                 await asyncio.sleep(5)
                 continue
 
             if not msg:
                 await asyncio.sleep(1)
                 continue
 
@@ -364,16 +362,18 @@
             title, *signal_info = notification.split(" ")
             # dont process empty values
             if not signal_info:
                 continue
             # at least madvr sends attributes in a consistent order
             # could use zip here but why? this works and is simple
             if "NoSignal" in title:
+                self.msg_dict["is_signal"] = False
                 return
             if "IncomingSignalInfo" in title:
+                self.msg_dict["is_signal"] = True
                 self.msg_dict["incoming_res"] = signal_info[0]
                 self.msg_dict["incoming_frame_rate"] = signal_info[1]
                 self.msg_dict["incoming_color_space"] = signal_info[3]
                 self.msg_dict["incoming_bit_depth"] = signal_info[4]
                 self.msg_dict["hdr_flag"] = "HDR" in signal_info[5]
                 self.msg_dict["incoming_colorimetry"] = signal_info[6]
                 self.msg_dict["incoming_black_levels"] = signal_info[7]
```

### Comparing `py_madvr-1.4.4/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.5/py_madvr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.4.4
+Version: 1.4.5
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.4/setup.py` & `py_madvr-1.4.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.4.4",
+    version="1.4.5",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.4.4/tests/testMadVR.py` & `py_madvr-1.4.5/tests/testMadVR.py`

 * *Files identical despite different names*

