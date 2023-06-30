# Comparing `tmp/nopasaran-0.1.7.tar.gz` & `tmp/nopasaran-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.1.7.tar", last modified: Fri Jun 30 12:14:50 2023, max compression
+gzip compressed data, was "nopasaran-0.1.8.tar", last modified: Fri Jun 30 12:19:15 2023, max compression
```

## Comparing `nopasaran-0.1.7.tar` & `nopasaran-0.1.8.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.7/LICENSE
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:14:50.477187 nopasaran-0.1.7/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.7/README.md
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.467187 nopasaran-0.1.7/nopasaran.egg-info/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:14:50.000000 nopasaran-0.1.7/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1023 2023-06-30 12:14:50.000000 nopasaran-0.1.7/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 12:14:50.000000 nopasaran-0.1.7/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       39 2023-06-30 12:14:50.000000 nopasaran-0.1.7/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 12:14:50.000000 nopasaran-0.1.7/nopasaran.egg-info/requires.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       10 2023-06-30 12:14:50.000000 nopasaran-0.1.7/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 12:14:50.477187 nopasaran-0.1.7/setup.cfg
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1204 2023-06-30 12:14:39.000000 nopasaran-0.1.7/setup.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:29:37.000000 nopasaran-0.1.7/src/__init__.py
--rwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)     1342 2023-06-30 12:11:57.000000 nopasaran-0.1.7/src/main.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/__init__.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/controllers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/controllers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1824 2023-06-30 12:13:06.000000 nopasaran-0.1.7/src/nopasaran/controllers/controller.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      585 2023-06-30 12:12:40.000000 nopasaran-0.1.7/src/nopasaran/controllers/factory.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/controllers/messages.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2123 2023-06-30 12:12:30.000000 nopasaran-0.1.7/src/nopasaran/controllers/protocol.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/interpreters/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/interpreters/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14744 2023-06-30 12:10:59.000000 nopasaran-0.1.7/src/nopasaran/interpreters/action_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4993 2023-06-30 12:11:11.000000 nopasaran-0.1.7/src/nopasaran/interpreters/condition_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2438 2023-06-30 12:11:19.000000 nopasaran-0.1.7/src/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/ipsec_tunnels/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.7/src/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/machines/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/machines/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5221 2023-06-30 12:11:37.000000 nopasaran-0.1.7/src/nopasaran/machines/machine.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/parsers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/parsers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/parsers/interpreter_parser.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/src/nopasaran/sniffers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.7/src/nopasaran/sniffers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2250 2023-06-30 12:13:27.000000 nopasaran-0.1.7/src/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.7/src/nopasaran/utils.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:14:50.477187 nopasaran-0.1.7/tests/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.7/tests/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2222 2023-06-30 12:07:18.000000 nopasaran-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.8/LICENSE
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:19:15.547186 nopasaran-0.1.8/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.8/README.md
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.537186 nopasaran-0.1.8/nopasaran.egg-info/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      975 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       10 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 12:19:15.547186 nopasaran-0.1.8/setup.cfg
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1104 2023-06-30 12:19:07.000000 nopasaran-0.1.8/setup.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.537186 nopasaran-0.1.8/src/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1342 2023-06-30 12:18:33.000000 nopasaran-0.1.8/src/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.537186 nopasaran-0.1.8/src/nopasaran/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/controllers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/controllers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1824 2023-06-30 12:13:06.000000 nopasaran-0.1.8/src/nopasaran/controllers/controller.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      585 2023-06-30 12:12:40.000000 nopasaran-0.1.8/src/nopasaran/controllers/factory.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/controllers/messages.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2123 2023-06-30 12:12:30.000000 nopasaran-0.1.8/src/nopasaran/controllers/protocol.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/interpreters/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/interpreters/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14744 2023-06-30 12:10:59.000000 nopasaran-0.1.8/src/nopasaran/interpreters/action_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4993 2023-06-30 12:11:11.000000 nopasaran-0.1.8/src/nopasaran/interpreters/condition_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2438 2023-06-30 12:11:19.000000 nopasaran-0.1.8/src/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/machines/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/machines/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5221 2023-06-30 12:11:37.000000 nopasaran-0.1.8/src/nopasaran/machines/machine.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/parsers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/parsers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/parsers/interpreter_parser.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/sniffers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.8/src/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2250 2023-06-30 12:13:27.000000 nopasaran-0.1.8/src/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/utils.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/tests/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/tests/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2222 2023-06-30 12:07:18.000000 nopasaran-0.1.8/tests/test_utils.py
```

### Comparing `nopasaran-0.1.7/LICENSE` & `nopasaran-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/PKG-INFO` & `nopasaran-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.7
+Version: 0.1.8
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.7/README.md` & `nopasaran-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.1.8/nopasaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.7
+Version: 0.1.8
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.7/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.1.8/nopasaran.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 LICENSE
 README.md
 setup.py
 nopasaran.egg-info/PKG-INFO
 nopasaran.egg-info/SOURCES.txt
 nopasaran.egg-info/dependency_links.txt
-nopasaran.egg-info/entry_points.txt
 nopasaran.egg-info/requires.txt
 nopasaran.egg-info/top_level.txt
 src/__init__.py
-src/main.py
 src/nopasaran/__init__.py
 src/nopasaran/utils.py
 src/nopasaran/controllers/__init__.py
 src/nopasaran/controllers/controller.py
 src/nopasaran/controllers/factory.py
 src/nopasaran/controllers/messages.py
 src/nopasaran/controllers/protocol.py
```

### Comparing `nopasaran-0.1.7/setup.py` & `nopasaran-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,23 @@
 # Read requirements from requirements.txt file
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 setup(
     name="nopasaran",
-    version="0.1.7",
+    version="0.1.8",
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
-    install_requires=requirements,
-    entry_points={
-        "console_scripts": [
-            "nopasaran = src:main"
-        ]
-    }
+    install_requires=requirements
 )
```

### Comparing `nopasaran-0.1.7/src/main.py` & `nopasaran-0.1.8/src/__init__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/controllers/controller.py` & `nopasaran-0.1.8/src/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/controllers/factory.py` & `nopasaran-0.1.8/src/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/controllers/protocol.py` & `nopasaran-0.1.8/src/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.1.8/src/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.1.8/src/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.1.8/src/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/machines/machine.py` & `nopasaran-0.1.8/src/nopasaran/machines/machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.1.8/src/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/sniffers/sniffer.py` & `nopasaran-0.1.8/src/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/src/nopasaran/utils.py` & `nopasaran-0.1.8/src/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.7/tests/test_utils.py` & `nopasaran-0.1.8/tests/test_utils.py`

 * *Files identical despite different names*

