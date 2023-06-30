# Comparing `tmp/lb-nightly-configuration-0.3.1.tar.gz` & `tmp/lb_nightly_configuration-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb-nightly-configuration-0.3.1.tar", max compression
+gzip compressed data, was "lb_nightly_configuration-0.3.2.tar", max compression
```

## Comparing `lb-nightly-configuration-0.3.1.tar` & `lb_nightly_configuration-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35147 2021-11-02 13:30:07.199002 lb-nightly-configuration-0.3.1/LICENSE
--rw-r--r--   0        0        0    12346 2022-09-19 11:17:26.898141 lb-nightly-configuration-0.3.1/lb/nightly/configuration/__init__.py
--rw-r--r--   0        0        0      865 2021-11-02 13:30:07.201002 lb-nightly-configuration-0.3.1/lb/nightly/configuration/defaults.py
--rw-r--r--   0        0        0    35177 2022-09-15 09:11:54.887125 lb-nightly-configuration-0.3.1/lb/nightly/configuration/project.py
--rw-r--r--   0        0        0    17115 2022-05-30 08:28:35.626295 lb-nightly-configuration-0.3.1/lb/nightly/configuration/slot.py
--rw-r--r--   0        0        0    10561 2022-05-30 08:40:54.130285 lb-nightly-configuration-0.3.1/lb/nightly/configuration/utils.py
--rw-r--r--   0        0        0     1187 2022-09-19 11:17:26.928142 lb-nightly-configuration-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 lb-nightly-configuration-0.3.1/setup.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 lb-nightly-configuration-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-02-01 16:04:58.852806 lb_nightly_configuration-0.3.2/LICENSE
+-rw-r--r--   0        0        0    12339 2023-06-30 17:28:26.578173 lb_nightly_configuration-0.3.2/lb/nightly/configuration/__init__.py
+-rw-r--r--   0        0        0      938 2023-06-30 17:12:39.062958 lb_nightly_configuration-0.3.2/lb/nightly/configuration/constants.py
+-rw-r--r--   0        0        0    35177 2023-06-30 17:12:39.062958 lb_nightly_configuration-0.3.2/lb/nightly/configuration/project.py
+-rw-r--r--   0        0        0    17069 2023-06-30 17:12:39.062958 lb_nightly_configuration-0.3.2/lb/nightly/configuration/slot.py
+-rw-r--r--   0        0        0    10561 2023-02-01 16:04:58.852806 lb_nightly_configuration-0.3.2/lb/nightly/configuration/utils.py
+-rw-r--r--   0        0        0     1187 2023-06-30 17:28:26.586174 lb_nightly_configuration-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 lb_nightly_configuration-0.3.2/PKG-INFO
```

### Comparing `lb-nightly-configuration-0.3.1/LICENSE` & `lb_nightly_configuration-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-nightly-configuration-0.3.1/lb/nightly/configuration/__init__.py` & `lb_nightly_configuration-0.3.2/lb/nightly/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 import json
 import logging
 import os
 import re
 import sys
 from collections import namedtuple
 from urllib.parse import urlsplit, urlunsplit
 from urllib.request import urlopen
 
+from .constants import VALID_PLATFORM_RE
 from .project import DBASE, PARAM, DataProject, Package, Project
 from .slot import Slot, slot_factory
 from .utils import configToString, save
 
 
 def service_config(config_file=None, silent=False):
     """
@@ -281,17 +282,15 @@
         for x in getattr(slot, field_name):
             try:
                 re.compile(x)
             except Exception as err:
                 good = False
                 log.error("%s: invalid value %r: %s", field_name, x, err)
 
-    good &= check_list_of_strings(
-        "platforms", "platform", r"^[a-z0-9_+]+-[a-z0-9_]+-[a-z0-9_+]+-[a-z0-9_+]+$"
-    )
+    good &= check_list_of_strings("platforms", "platform", VALID_PLATFORM_RE)
     good &= check_list_of_strings("env", "env setting", r"^[a-zA-Z_][a-z0-9A-Z_]*=")
 
     return good
 
 
 def check_config():
     from argparse import ArgumentParser
```

### Comparing `lb-nightly-configuration-0.3.1/lb/nightly/configuration/defaults.py` & `lb_nightly_configuration-0.3.2/lb/nightly/configuration/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 DEFAULT_BUILD_TOOL = "cmake"
 DEFAULT_CHECKOUT_METHOD = "default"
+VALID_PLATFORM_RE = r"^[0-9a-z_+.]+-[0-9a-z_]+-[0-9a-z_+]+-[0-9a-z_+]+$"
```

### Comparing `lb-nightly-configuration-0.3.1/lb/nightly/configuration/project.py` & `lb_nightly_configuration-0.3.2/lb/nightly/configuration/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import copy
 import logging
 import os
 import re
 from hashlib import sha256
 from pathlib import Path
 
-from .defaults import DEFAULT_CHECKOUT_METHOD
+from .constants import DEFAULT_CHECKOUT_METHOD
 from .utils import _ContainedList, applyenv, write_patch
 
 __log__ = logging.getLogger(__name__)
 
 # constants
 GP_EXP = re.compile(r"gaudi_project\(([^)]+)\)")
 HT_EXP = re.compile(r"set\(\s*heptools_version\s+([^)]+)\)")
@@ -667,15 +667,14 @@
             path = ""
             slotname = ""
             slotbid = ""
 
         filename = self.name
 
         if stage == "build":
-
             path = os.path.join(path, "packs", platform)
             filename = ".".join(
                 list(
                     filter(
                         None,
                         [
                             filename,
```

### Comparing `lb-nightly-configuration-0.3.1/lb/nightly/configuration/slot.py` & `lb_nightly_configuration-0.3.2/lb/nightly/configuration/slot.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ###############################################################################
 import logging
 import os
 import re
 from collections import OrderedDict
 from pathlib import Path
 
-from .defaults import DEFAULT_BUILD_TOOL
+from .constants import DEFAULT_BUILD_TOOL, VALID_PLATFORM_RE
 from .project import STANDARD_CONTAINERS, DataProject, Package, Project, ProjectsList
 from .utils import applyenv
 
 __log__ = logging.getLogger(__name__)
 
 _slot_factories = set()
 
@@ -100,17 +100,15 @@
             desc = (self.__doc__ or "<no description>").strip()
         self.desc = desc
 
         self.platforms = kwargs.get("platforms", [])
         if isinstance(self.platforms, str):
             self.platforms = [self.platforms]
         for p in self.platforms:
-            assert re.match(r"^[0-9a-z_+]+-[0-9a-z_]+-[0-9a-z_+]+-[0-9a-z_+]+$", p), (
-                "invalid platform: %r" % p
-            )
+            assert re.match(VALID_PLATFORM_RE, p), "invalid platform: %r" % p
 
         self.error_exceptions = kwargs.get("error_exceptions", [])
         self.warning_exceptions = kwargs.get("warning_exceptions", [])
 
         self.preconditions = kwargs.get("preconditions", [])
 
         self.cache_entries = kwargs.get("cache_entries", {})
```

### Comparing `lb-nightly-configuration-0.3.1/lb/nightly/configuration/utils.py` & `lb_nightly_configuration-0.3.2/lb/nightly/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `lb-nightly-configuration-0.3.1/pyproject.toml` & `lb_nightly_configuration-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lb-nightly-configuration"
-version = "0.3.1"
+version = "0.3.2"
 description = "classes and functions to suppot the LHCb Nightly Build System configuration"
 authors = [
     "Marco Clemencic <marco.clemencic@cern.ch>",
     "Maciej Szymanski <maciej.szymanski@cern.ch>",
     "LHCb Core Software <lhcb-core-soft@cern.ch>"
 ]
 license = "GPL-3.0-only"
```

### Comparing `lb-nightly-configuration-0.3.1/PKG-INFO` & `lb_nightly_configuration-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lb-nightly-configuration
-Version: 0.3.1
+Version: 0.3.2
 Summary: classes and functions to suppot the LHCb Nightly Build System configuration
 License: GPL-3.0-only
 Author: Marco Clemencic
 Author-email: marco.clemencic@cern.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: graph
 Requires-Dist: GitPython (>=3.1.18,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: configurator (>=2.6.0,<3.0.0)
-Requires-Dist: networkx (>=2.6.1,<3.0.0); extra == "graph"
+Requires-Dist: networkx (>=2.6.1,<3.0.0) ; extra == "graph"
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
```

