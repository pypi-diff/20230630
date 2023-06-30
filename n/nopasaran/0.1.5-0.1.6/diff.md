# Comparing `tmp/nopasaran-0.1.5.tar.gz` & `tmp/nopasaran-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.1.5.tar", last modified: Fri Jun 30 11:52:05 2023, max compression
+gzip compressed data, was "nopasaran-0.1.6.tar", last modified: Fri Jun 30 11:59:07 2023, max compression
```

## Comparing `nopasaran-0.1.5.tar` & `nopasaran-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.5/LICENSE
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:52:05.867192 nopasaran-0.1.5/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.5/README.md
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/nopasaran.egg-info/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:52:05.000000 nopasaran-0.1.5/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1003 2023-06-30 11:52:05.000000 nopasaran-0.1.5/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 11:52:05.000000 nopasaran-0.1.5/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       39 2023-06-30 11:52:05.000000 nopasaran-0.1.5/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 11:52:05.000000 nopasaran-0.1.5/nopasaran.egg-info/requires.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       10 2023-06-30 11:52:05.000000 nopasaran-0.1.5/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 11:52:05.867192 nopasaran-0.1.5/setup.cfg
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1204 2023-06-30 11:51:51.000000 nopasaran-0.1.5/setup.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:29:37.000000 nopasaran-0.1.5/src/__init__.py
--rwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)     1338 2023-06-30 11:51:20.000000 nopasaran-0.1.5/src/main.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/__init__.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/controllers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/controllers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1822 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/controllers/controller.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      583 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/controllers/factory.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/controllers/messages.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2121 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/controllers/protocol.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/interpreters/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/interpreters/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14736 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/interpreters/action_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4991 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/interpreters/condition_interpreter.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2436 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/ipsec_tunnels/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.5/src/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/machines/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/machines/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5209 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/machines/machine.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/parsers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/parsers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/parsers/interpreter_parser.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/src/nopasaran/sniffers/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.5/src/nopasaran/sniffers/__init__.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2248 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.5/src/nopasaran/utils.py
-drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:52:05.867192 nopasaran-0.1.5/tests/
--rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.5/tests/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    35149 2023-06-30 09:55:08.000000 nopasaran-0.1.6/LICENSE
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:59:07.777190 nopasaran-0.1.6/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3346 2023-06-30 10:22:58.000000 nopasaran-0.1.6/README.md
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/nopasaran.egg-info/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     3910 2023-06-30 11:59:07.000000 nopasaran-0.1.6/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1023 2023-06-30 11:59:07.000000 nopasaran-0.1.6/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        1 2023-06-30 11:59:07.000000 nopasaran-0.1.6/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       39 2023-06-30 11:59:07.000000 nopasaran-0.1.6/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       52 2023-06-30 11:59:07.000000 nopasaran-0.1.6/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       10 2023-06-30 11:59:07.000000 nopasaran-0.1.6/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)       38 2023-06-30 11:59:07.777190 nopasaran-0.1.6/setup.cfg
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1204 2023-06-30 11:59:05.000000 nopasaran-0.1.6/setup.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:29:37.000000 nopasaran-0.1.6/src/__init__.py
+-rwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)     1346 2023-06-30 11:57:50.000000 nopasaran-0.1.6/src/main.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      170 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/__init__.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/controllers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/controllers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     1828 2023-06-30 11:56:37.000000 nopasaran-0.1.6/src/nopasaran/controllers/controller.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      589 2023-06-30 11:56:34.000000 nopasaran-0.1.6/src/nopasaran/controllers/factory.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)      171 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/controllers/messages.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2127 2023-06-30 11:56:32.000000 nopasaran-0.1.6/src/nopasaran/controllers/protocol.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/interpreters/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/interpreters/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)    14760 2023-06-30 11:56:39.000000 nopasaran-0.1.6/src/nopasaran/interpreters/action_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4997 2023-06-30 11:56:55.000000 nopasaran-0.1.6/src/nopasaran/interpreters/condition_interpreter.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2442 2023-06-30 11:56:47.000000 nopasaran-0.1.6/src/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:58.000000 nopasaran-0.1.6/src/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4627 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/machines/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/machines/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     5245 2023-06-30 11:55:04.000000 nopasaran-0.1.6/src/nopasaran/machines/machine.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/parsers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/parsers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2575 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/parsers/interpreter_parser.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/src/nopasaran/sniffers/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 10:02:54.000000 nopasaran-0.1.6/src/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2254 2023-06-30 11:55:46.000000 nopasaran-0.1.6/src/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     4657 2023-06-30 09:55:08.000000 nopasaran-0.1.6/src/nopasaran/utils.py
+drwxr-xr-x   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 11:59:07.777190 nopasaran-0.1.6/tests/
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)        0 2023-06-30 09:55:08.000000 nopasaran-0.1.6/tests/__init__.py
+-rw-r--r--   0 benhabbo  (1000) benhabbo  (1000)     2215 2023-06-30 11:57:29.000000 nopasaran-0.1.6/tests/test_utils.py
```

### Comparing `nopasaran-0.1.5/LICENSE` & `nopasaran-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.5/PKG-INFO` & `nopasaran-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.5
+Version: 0.1.6
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.5/README.md` & `nopasaran-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.5/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.1.6/nopasaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.1.5
+Version: 0.1.6
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nopasaran-0.1.5/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.1.6/nopasaran.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 src/nopasaran/ipsec_tunnels/ipsec_conf.py
 src/nopasaran/machines/__init__.py
 src/nopasaran/machines/machine.py
 src/nopasaran/parsers/__init__.py
 src/nopasaran/parsers/interpreter_parser.py
 src/nopasaran/sniffers/__init__.py
 src/nopasaran/sniffers/sniffer.py
-tests/__init__.py
+tests/__init__.py
+tests/test_utils.py
```

### Comparing `nopasaran-0.1.5/setup.py` & `nopasaran-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Read requirements from requirements.txt file
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 setup(
     name="nopasaran",
-    version="0.1.5",
+    version="0.1.6",
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

### Comparing `nopasaran-0.1.5/src/main.py` & `nopasaran-0.1.6/src/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Import libraries
 import argparse
 import json
 from scapy.all import *
 from twisted.internet.threads import deferToThread
 from twisted.internet import reactor
-from src.nopasaran.machines import Machine
+from src.nopasaran.machines.machine import Machine
   
 if __name__ == '__main__':
   # Set up argument parser
   parser = argparse.ArgumentParser(
     prog='ROLE', 
     epilog="See '<command> --help' for more information on a command."
   )
```

### Comparing `nopasaran-0.1.5/src/nopasaran/controllers/controller.py` & `nopasaran-0.1.6/src/nopasaran/controllers/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from twisted.internet import reactor
 
-from modules.controllers.factory import NodeClientFactory, NodeServerFactory
+from src.nopasaran.controllers.factory import NodeClientFactory, NodeServerFactory
 from twisted.internet.ssl import Certificate, PrivateCertificate
 
 class Controller():
     def __init__(self, root_certificate_file, own_private_certificate_file):        
         file_root = open(root_certificate_file, "rb")
         root_certificate = file_root.read()
         file_root.close()
```

### Comparing `nopasaran-0.1.5/src/nopasaran/controllers/factory.py` & `nopasaran-0.1.6/src/nopasaran/controllers/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from twisted.internet.protocol import ReconnectingClientFactory, ServerFactory
 
-from modules.controllers.protocol import NodeClientProtocol, NodeServerProtocol
+from src.nopasaran.controllers.protocol import NodeClientProtocol, NodeServerProtocol
 
 class NodeClientFactory(ReconnectingClientFactory):
     protocol = NodeClientProtocol
     
     def __init__(self, state_machine, variable):
         self.state_machine = state_machine
         self.variable = variable
```

### Comparing `nopasaran-0.1.5/src/nopasaran/controllers/protocol.py` & `nopasaran-0.1.6/src/nopasaran/controllers/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 from twisted.internet.protocol import Protocol
 
-from modules.controllers.messages import JSONMessage, Status
+from src.nopasaran.controllers.messages import JSONMessage, Status
 
 class NodeProtocol(Protocol):
     remote_status = Status.DISCONNECTED.name
     local_status = Status.DISCONNECTED.name
     is_active = True
     queue = []
```

### Comparing `nopasaran-0.1.5/src/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.1.6/src/nopasaran/interpreters/action_interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import cmd
 import time
 import json
 
 from scapy.all import send
 from twisted.internet.threads import deferToThread
 
-from modules.controllers.messages import JSONMessage, Status
-from modules.parsers.interpreter_parser import InterpreterParser
-from modules.controllers.controller import ClientController, ServerController
-from modules.utils import *
+from src.nopasaran.controllers.messages import JSONMessage, Status
+from src.nopasaran.parsers.interpreter_parser import InterpreterParser
+from src.nopasaran.controllers.controller import ClientController, ServerController
+from src.nopasaran.utils import *
 
 
 class ActionInterpreter(cmd.Cmd):
     def onecmd(self, line, machine):
         cmd, arg, line = self.parseline(line)
         if not line:
             return self.emptyline()
```

### Comparing `nopasaran-0.1.5/src/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.1.6/src/nopasaran/interpreters/condition_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cmd
-from modules.parsers.interpreter_parser import InterpreterParser
+from src.nopasaran.parsers.interpreter_parser import InterpreterParser
 
 class ConditionInterpreter(cmd.Cmd):
     """
     A custom ConditionInterpreter class that inherits from cmd.Cmd.
 
     This class interprets conditions in the context of a command-line interface.
     """
```

### Comparing `nopasaran-0.1.5/src/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.1.6/src/nopasaran/interpreters/transition_interpreter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cmd
 
-from modules.parsers.interpreter_parser import InterpreterParser
+from src.nopasaran.parsers.interpreter_parser import InterpreterParser
 
 
 class TransitionInterpreter(cmd.Cmd):
     """
     Custom TransitionInterpreter class inheriting from cmd.Cmd.
     This class interprets transition commands in the context of a command-line interface.
     """
```

### Comparing `nopasaran-0.1.5/src/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.1.6/src/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.5/src/nopasaran/machines/machine.py` & `nopasaran-0.1.6/src/nopasaran/machines/machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from enum import Enum
 
 from twisted.internet.threads import deferToThread
 
-from modules.utils import *
-from modules.interpreters.action_interpreter import ActionInterpreter
-from modules.interpreters.condition_interpreter import ConditionInterpreter
-from modules.interpreters.transition_interpreter import TransitionInterpreter
-from modules.controllers.controller import ClientController, ServerController
-from modules.sniffers.sniffer import Sniffer
+from src.nopasaran.utils import *
+from src.nopasaran.interpreters.action_interpreter import ActionInterpreter
+from src.nopasaran.interpreters.condition_interpreter import ConditionInterpreter
+from src.nopasaran.interpreters.transition_interpreter import TransitionInterpreter
+from src.nopasaran.controllers.controller import ClientController, ServerController
+from src.nopasaran.sniffers.sniffer import Sniffer
 
 class Command(Enum):
     EXECUTE_ACTION = 0
     ASSIGN_VARIABLES = 1
     SET_STATE = 2
 
 class Machine:
```

### Comparing `nopasaran-0.1.5/src/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.1.6/src/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.1.5/src/nopasaran/sniffers/sniffer.py` & `nopasaran-0.1.6/src/nopasaran/sniffers/sniffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from modules.utils import *
+from src.nopasaran.utils import *
 from scapy.all import AsyncSniffer, Ether, sniff
 
 class Sniffer(AsyncSniffer):
     """
     Custom Sniffer class inheriting from the AsyncSniffer of Scapy.
     """
     def __init__(self, machine, filter=''):
```

### Comparing `nopasaran-0.1.5/src/nopasaran/utils.py` & `nopasaran-0.1.6/src/nopasaran/utils.py`

 * *Files identical despite different names*

