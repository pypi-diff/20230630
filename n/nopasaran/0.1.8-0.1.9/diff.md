# Comparing `tmp/nopasaran-0.1.8.tar.gz` & `tmp/nopasaran-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.1.8.tar", last modified: Fri Jun 30 12:19:15 2023, max compression
+gzip compressed data, was "nopasaran-0.1.9.tar", last modified: Fri Jun 30 12:30:06 2023, max compression
```

## Comparing `nopasaran-0.1.8.tar` & `nopasaran-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.8/LICENSE
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:19:15.547186 nopasaran-0.1.8/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.8/README.md
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.537186 nopasaran-0.1.8/nopasaran.egg-info/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      975 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/requires.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       10 2023-06-30 12:19:15.000000 nopasaran-0.1.8/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 12:19:15.547186 nopasaran-0.1.8/setup.cfg
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1104 2023-06-30 12:19:07.000000 nopasaran-0.1.8/setup.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.537186 nopasaran-0.1.8/src/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1342 2023-06-30 12:18:33.000000 nopasaran-0.1.8/src/__init__.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.537186 nopasaran-0.1.8/src/nopasaran/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/__init__.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/controllers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/controllers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1824 2023-06-30 12:13:06.000000 nopasaran-0.1.8/src/nopasaran/controllers/controller.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      585 2023-06-30 12:12:40.000000 nopasaran-0.1.8/src/nopasaran/controllers/factory.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/controllers/messages.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2123 2023-06-30 12:12:30.000000 nopasaran-0.1.8/src/nopasaran/controllers/protocol.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/interpreters/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/interpreters/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14744 2023-06-30 12:10:59.000000 nopasaran-0.1.8/src/nopasaran/interpreters/action_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4993 2023-06-30 12:11:11.000000 nopasaran-0.1.8/src/nopasaran/interpreters/condition_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2438 2023-06-30 12:11:19.000000 nopasaran-0.1.8/src/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/machines/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/machines/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5221 2023-06-30 12:11:37.000000 nopasaran-0.1.8/src/nopasaran/machines/machine.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/parsers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/parsers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/parsers/interpreter_parser.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/src/nopasaran/sniffers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.8/src/nopasaran/sniffers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2250 2023-06-30 12:13:27.000000 nopasaran-0.1.8/src/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.8/src/nopasaran/utils.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:19:15.547186 nopasaran-0.1.8/tests/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.8/tests/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2222 2023-06-30 12:07:18.000000 nopasaran-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.757183 nopasaran-0.1.9/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.9/LICENSE
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:30:06.757183 nopasaran-0.1.9/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.9/README.md
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1508 2023-06-30 12:28:03.000000 nopasaran-0.1.9/nopasaran/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran/controllers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/controllers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1814 2023-06-30 12:29:37.000000 nopasaran-0.1.9/nopasaran/controllers/controller.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      575 2023-06-30 12:29:35.000000 nopasaran-0.1.9/nopasaran/controllers/factory.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/controllers/messages.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2113 2023-06-30 12:29:33.000000 nopasaran-0.1.9/nopasaran/controllers/protocol.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran/interpreters/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/interpreters/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14704 2023-06-30 12:29:06.000000 nopasaran-0.1.9/nopasaran/interpreters/action_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4983 2023-06-30 12:29:03.000000 nopasaran-0.1.9/nopasaran/interpreters/condition_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2428 2023-06-30 12:29:01.000000 nopasaran-0.1.9/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.9/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran/machines/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/machines/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5161 2023-06-30 12:28:40.000000 nopasaran-0.1.9/nopasaran/machines/machine.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran/parsers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/parsers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/parsers/interpreter_parser.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.757183 nopasaran-0.1.9/nopasaran/sniffers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.9/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2240 2023-06-30 12:28:18.000000 nopasaran-0.1.9/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.9/nopasaran/utils.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.747183 nopasaran-0.1.9/nopasaran.egg-info/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 12:30:06.000000 nopasaran-0.1.9/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      883 2023-06-30 12:30:06.000000 nopasaran-0.1.9/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 12:30:06.000000 nopasaran-0.1.9/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 12:30:06.000000 nopasaran-0.1.9/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       16 2023-06-30 12:30:06.000000 nopasaran-0.1.9/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 12:30:06.757183 nopasaran-0.1.9/setup.cfg
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1104 2023-06-30 12:25:26.000000 nopasaran-0.1.9/setup.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 12:30:06.757183 nopasaran-0.1.9/tests/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.9/tests/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2222 2023-06-30 12:07:18.000000 nopasaran-0.1.9/tests/test_utils.py
```

### Comparing `nopasaran-0.1.8/LICENSE` & `nopasaran-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.8/PKG-INFO` & `nopasaran-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.8
+Version: 0.1.9
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.8/README.md` & `nopasaran-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.8/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.1.9/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.8
+Version: 0.1.9
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.8/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.1.9/nopasaran.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 LICENSE
 README.md
 setup.py
+nopasaran/__init__.py
+nopasaran/utils.py
 nopasaran.egg-info/PKG-INFO
 nopasaran.egg-info/SOURCES.txt
 nopasaran.egg-info/dependency_links.txt
 nopasaran.egg-info/requires.txt
 nopasaran.egg-info/top_level.txt
-src/__init__.py
-src/nopasaran/__init__.py
-src/nopasaran/utils.py
-src/nopasaran/controllers/__init__.py
-src/nopasaran/controllers/controller.py
-src/nopasaran/controllers/factory.py
-src/nopasaran/controllers/messages.py
-src/nopasaran/controllers/protocol.py
-src/nopasaran/interpreters/__init__.py
-src/nopasaran/interpreters/action_interpreter.py
-src/nopasaran/interpreters/condition_interpreter.py
-src/nopasaran/interpreters/transition_interpreter.py
-src/nopasaran/ipsec_tunnels/__init__.py
-src/nopasaran/ipsec_tunnels/ipsec_conf.py
-src/nopasaran/machines/__init__.py
-src/nopasaran/machines/machine.py
-src/nopasaran/parsers/__init__.py
-src/nopasaran/parsers/interpreter_parser.py
-src/nopasaran/sniffers/__init__.py
-src/nopasaran/sniffers/sniffer.py
+nopasaran/controllers/__init__.py
+nopasaran/controllers/controller.py
+nopasaran/controllers/factory.py
+nopasaran/controllers/messages.py
+nopasaran/controllers/protocol.py
+nopasaran/interpreters/__init__.py
+nopasaran/interpreters/action_interpreter.py
+nopasaran/interpreters/condition_interpreter.py
+nopasaran/interpreters/transition_interpreter.py
+nopasaran/ipsec_tunnels/__init__.py
+nopasaran/ipsec_tunnels/ipsec_conf.py
+nopasaran/machines/__init__.py
+nopasaran/machines/machine.py
+nopasaran/parsers/__init__.py
+nopasaran/parsers/interpreter_parser.py
+nopasaran/sniffers/__init__.py
+nopasaran/sniffers/sniffer.py
 tests/__init__.py
 tests/test_utils.py
```

### Comparing `nopasaran-0.1.8/setup.py` & `nopasaran-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Read requirements from requirements.txt file
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 setup(
     name="nopasaran",
-    version="0.1.8",
+    version="0.1.9",
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

### Comparing `nopasaran-0.1.8/src/__init__.py` & `nopasaran-0.1.9/nopasaran/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Import libraries
+import logging
 import argparse
 import json
 from scapy.all import *
 from twisted.internet.threads import deferToThread
 from twisted.internet import reactor
-from nopasaran.machines.machine import Machine
+from machines.machine import Machine
+
   
 if __name__ == '__main__':
+  
+  logging.basicConfig(filename='conf.log', level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s - %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p %Z')
   # Set up argument parser
   parser = argparse.ArgumentParser(
     prog='ROLE', 
     epilog="See '<command> --help' for more information on a command."
   )
 
   # Set up base parser
```

### Comparing `nopasaran-0.1.8/src/nopasaran/controllers/controller.py` & `nopasaran-0.1.9/nopasaran/controllers/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from twisted.internet import reactor
 
-from nopasaran.controllers.factory import NodeClientFactory, NodeServerFactory
+from controllers.factory import NodeClientFactory, NodeServerFactory
 from twisted.internet.ssl import Certificate, PrivateCertificate
 
 class Controller():
     def __init__(self, root_certificate_file, own_private_certificate_file):        
         file_root = open(root_certificate_file, "rb")
         root_certificate = file_root.read()
         file_root.close()
```

### Comparing `nopasaran-0.1.8/src/nopasaran/controllers/factory.py` & `nopasaran-0.1.9/nopasaran/controllers/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from twisted.internet.protocol import ReconnectingClientFactory, ServerFactory
 
-from nopasaran.controllers.protocol import NodeClientProtocol, NodeServerProtocol
+from controllers.protocol import NodeClientProtocol, NodeServerProtocol
 
 class NodeClientFactory(ReconnectingClientFactory):
     protocol = NodeClientProtocol
     
     def __init__(self, state_machine, variable):
         self.state_machine = state_machine
         self.variable = variable
```

### Comparing `nopasaran-0.1.8/src/nopasaran/controllers/protocol.py` & `nopasaran-0.1.9/nopasaran/controllers/protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 from twisted.internet.protocol import Protocol
 
-from nopasaran.controllers.messages import JSONMessage, Status
+from controllers.messages import JSONMessage, Status
 
 class NodeProtocol(Protocol):
     remote_status = Status.DISCONNECTED.name
     local_status = Status.DISCONNECTED.name
     is_active = True
     queue = []
```

### Comparing `nopasaran-0.1.8/src/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.1.9/nopasaran/interpreters/action_interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import cmd
 import time
 import json
 
 from scapy.all import send
 from twisted.internet.threads import deferToThread
 
-from nopasaran.controllers.messages import JSONMessage, Status
-from nopasaran.parsers.interpreter_parser import InterpreterParser
-from nopasaran.controllers.controller import ClientController, ServerController
-from nopasaran.utils import *
+from controllers.messages import JSONMessage, Status
+from parsers.interpreter_parser import InterpreterParser
+from controllers.controller import ClientController, ServerController
+from utils import *
 
 
 class ActionInterpreter(cmd.Cmd):
     def onecmd(self, line, machine):
         cmd, arg, line = self.parseline(line)
         if not line:
             return self.emptyline()
```

### Comparing `nopasaran-0.1.8/src/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.1.9/nopasaran/interpreters/condition_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cmd
-from nopasaran.parsers.interpreter_parser import InterpreterParser
+from parsers.interpreter_parser import InterpreterParser
 
 class ConditionInterpreter(cmd.Cmd):
     """
     A custom ConditionInterpreter class that inherits from cmd.Cmd.
 
     This class interprets conditions in the context of a command-line interface.
     """
```

### Comparing `nopasaran-0.1.8/src/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.1.9/nopasaran/interpreters/transition_interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cmd
 
-from nopasaran.parsers.interpreter_parser import InterpreterParser
+from parsers.interpreter_parser import InterpreterParser
 
 
 class TransitionInterpreter(cmd.Cmd):
     """
     Custom TransitionInterpreter class inheriting from cmd.Cmd.
     This class interprets transition commands in the context of a command-line interface.
     """
```

### Comparing `nopasaran-0.1.8/src/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.1.9/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.8/src/nopasaran/machines/machine.py` & `nopasaran-0.1.9/nopasaran/machines/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
 
 from twisted.internet.threads import deferToThread
 
-from nopasaran.utils import *
-from nopasaran.interpreters.action_interpreter import ActionInterpreter
-from nopasaran.interpreters.condition_interpreter import ConditionInterpreter
-from nopasaran.interpreters.transition_interpreter import TransitionInterpreter
-from nopasaran.controllers.controller import ClientController, ServerController
-from nopasaran.sniffers.sniffer import Sniffer
+from utils import *
+from interpreters.action_interpreter import ActionInterpreter
+from interpreters.condition_interpreter import ConditionInterpreter
+from interpreters.transition_interpreter import TransitionInterpreter
+from controllers.controller import ClientController, ServerController
+from sniffers.sniffer import Sniffer
 
 class Command(Enum):
     EXECUTE_ACTION = 0
     ASSIGN_VARIABLES = 1
     SET_STATE = 2
 
 class Machine:
```

### Comparing `nopasaran-0.1.8/src/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.1.9/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.8/src/nopasaran/sniffers/sniffer.py` & `nopasaran-0.1.9/nopasaran/sniffers/sniffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nopasaran.utils import *
+from utils import *
 from scapy.all import AsyncSniffer, Ether, sniff
 
 class Sniffer(AsyncSniffer):
     """
     Custom Sniffer class inheriting from the AsyncSniffer of Scapy.
     """
     def __init__(self, machine, filter=''):
```

### Comparing `nopasaran-0.1.8/src/nopasaran/utils.py` & `nopasaran-0.1.9/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.8/tests/test_utils.py` & `nopasaran-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

