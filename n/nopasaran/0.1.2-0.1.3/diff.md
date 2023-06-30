# Comparing `tmp/nopasaran-0.1.2.tar.gz` & `tmp/nopasaran-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.1.2.tar", last modified: Fri Jun 30 11:05:55 2023, max compression
+gzip compressed data, was "nopasaran-0.1.3.tar", last modified: Fri Jun 30 11:30:26 2023, max compression
```

## Comparing `nopasaran-0.1.2.tar` & `nopasaran-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.2/LICENSE
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:05:55.447202 nopasaran-0.1.2/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.2/README.md
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.437202 nopasaran-0.1.2/modules/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/__init__.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/modules/controllers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/controllers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1822 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/controllers/controller.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      583 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/controllers/factory.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/controllers/messages.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2121 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/controllers/protocol.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/modules/interpreters/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/interpreters/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14736 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/interpreters/action_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4991 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/interpreters/condition_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2436 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/interpreters/transition_interpreter.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/modules/ipsec_tunnels/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.2/modules/ipsec_tunnels/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/modules/machines/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/machines/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5209 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/machines/machine.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/modules/parsers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/parsers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/parsers/interpreter_parser.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/modules/sniffers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.2/modules/sniffers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2248 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/sniffers/sniffer.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.2/modules/utils.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/nopasaran.egg-info/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:05:55.000000 nopasaran-0.1.2/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      861 2023-06-30 11:05:55.000000 nopasaran-0.1.2/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 11:05:55.000000 nopasaran-0.1.2/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       40 2023-06-30 11:05:55.000000 nopasaran-0.1.2/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 11:05:55.000000 nopasaran-0.1.2/nopasaran.egg-info/requires.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       14 2023-06-30 11:05:55.000000 nopasaran-0.1.2/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 11:05:55.447202 nopasaran-0.1.2/setup.cfg
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1205 2023-06-30 11:05:22.000000 nopasaran-0.1.2/setup.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:05:55.447202 nopasaran-0.1.2/tests/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.2/tests/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.3/LICENSE
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:30:26.767197 nopasaran-0.1.3/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.3/README.md
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/nopasaran.egg-info/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:30:26.000000 nopasaran-0.1.3/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      965 2023-06-30 11:30:26.000000 nopasaran-0.1.3/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 11:30:26.000000 nopasaran-0.1.3/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       44 2023-06-30 11:30:26.000000 nopasaran-0.1.3/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 11:30:26.000000 nopasaran-0.1.3/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       10 2023-06-30 11:30:26.000000 nopasaran-0.1.3/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 11:30:26.767197 nopasaran-0.1.3/setup.cfg
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1209 2023-06-30 11:26:41.000000 nopasaran-0.1.3/setup.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:29:37.000000 nopasaran-0.1.3/src/__init__.py
+-rwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)     1415 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/main.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/controllers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/controllers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1822 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/controllers/controller.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      583 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/controllers/factory.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/controllers/messages.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2121 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/controllers/protocol.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/interpreters/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/interpreters/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14736 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/interpreters/action_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4991 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/interpreters/condition_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2436 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/interpreters/transition_interpreter.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/ipsec_tunnels/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.3/src/modules/ipsec_tunnels/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/machines/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/machines/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5209 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/machines/machine.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/parsers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/parsers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/parsers/interpreter_parser.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/src/modules/sniffers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.3/src/modules/sniffers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2248 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/sniffers/sniffer.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.3/src/modules/utils.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:30:26.767197 nopasaran-0.1.3/tests/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.3/tests/__init__.py
```

### Comparing `nopasaran-0.1.2/LICENSE` & `nopasaran-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/PKG-INFO` & `nopasaran-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.2
+Version: 0.1.3
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.2/README.md` & `nopasaran-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/controllers/controller.py` & `nopasaran-0.1.3/src/modules/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/controllers/factory.py` & `nopasaran-0.1.3/src/modules/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/controllers/protocol.py` & `nopasaran-0.1.3/src/modules/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/interpreters/action_interpreter.py` & `nopasaran-0.1.3/src/modules/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/interpreters/condition_interpreter.py` & `nopasaran-0.1.3/src/modules/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/interpreters/transition_interpreter.py` & `nopasaran-0.1.3/src/modules/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.1.3/src/modules/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/machines/machine.py` & `nopasaran-0.1.3/src/modules/machines/machine.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/parsers/interpreter_parser.py` & `nopasaran-0.1.3/src/modules/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/sniffers/sniffer.py` & `nopasaran-0.1.3/src/modules/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/modules/utils.py` & `nopasaran-0.1.3/src/modules/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.2/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.1.3/nopasaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.2
+Version: 0.1.3
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.2/setup.py` & `nopasaran-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Read requirements from requirements.txt file
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 setup(
     name="nopasaran",
-    version="0.1.2",
+    version="0.1.3",
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
@@ -25,11 +25,11 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     install_requires=requirements,
     entry_points={
         "console_scripts": [
-            "nopasaran = main:main"
+            "nopasaran = src.main:main"
         ]
     }
 )
```

