# Comparing `tmp/har2tree-1.9.1.tar.gz` & `tmp/har2tree-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2tree-1.9.1.tar", max compression
+gzip compressed data, was "har2tree-1.9.2.tar", max compression
```

## Comparing `har2tree-1.9.1.tar` & `har2tree-1.9.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1803 2021-02-09 14:47:49.631324 har2tree-1.9.1/LICENSE
--rw-r--r--   0        0        0      402 2021-05-18 22:02:46.972352 har2tree-1.9.1/README.md
--rw-r--r--   0        0        0      286 2021-05-05 11:05:29.286384 har2tree-1.9.1/har2tree/__init__.py
--rw-r--r--   0        0        0    37888 2021-09-06 13:58:47.928727 har2tree-1.9.1/har2tree/har2tree.py
--rw-r--r--   0        0        0    13103 2021-09-29 11:57:35.805311 har2tree-1.9.1/har2tree/helper.py
--rw-r--r--   0        0        0    25741 2021-09-29 11:55:16.676146 har2tree-1.9.1/har2tree/nodes.py
--rw-r--r--   0        0        0     3571 2021-06-22 23:39:13.616195 har2tree-1.9.1/har2tree/parser.py
--rw-r--r--   0        0        0        0 2021-05-03 15:42:45.532814 har2tree-1.9.1/har2tree/py.typed
--rw-r--r--   0        0        0     1785 2021-10-07 16:11:36.279685 har2tree-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     1390 2021-10-07 16:12:40.001596 har2tree-1.9.1/setup.py
--rw-r--r--   0        0        0     1755 2021-10-07 16:12:40.001901 har2tree-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1803 2021-02-09 14:47:49.631324 har2tree-1.9.2/LICENSE
+-rw-r--r--   0        0        0      402 2021-05-18 22:02:46.972352 har2tree-1.9.2/README.md
+-rw-r--r--   0        0        0      286 2021-05-05 11:05:29.286384 har2tree-1.9.2/har2tree/__init__.py
+-rw-r--r--   0        0        0    39001 2021-11-30 10:08:16.902319 har2tree-1.9.2/har2tree/har2tree.py
+-rw-r--r--   0        0        0    13103 2021-09-29 11:57:35.805311 har2tree-1.9.2/har2tree/helper.py
+-rw-r--r--   0        0        0    25741 2021-11-29 09:47:21.922876 har2tree-1.9.2/har2tree/nodes.py
+-rw-r--r--   0        0        0     3571 2021-06-22 23:39:13.616195 har2tree-1.9.2/har2tree/parser.py
+-rw-r--r--   0        0        0        0 2021-05-03 15:42:45.532814 har2tree-1.9.2/har2tree/py.typed
+-rw-r--r--   0        0        0     1731 2021-11-30 13:47:42.323329 har2tree-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1390 2021-11-30 13:51:00.731922 har2tree-1.9.2/setup.py
+-rw-r--r--   0        0        0     1806 2021-11-30 13:51:00.732166 har2tree-1.9.2/PKG-INFO
```

### Comparing `har2tree-1.9.1/LICENSE` & `har2tree-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `har2tree-1.9.1/har2tree/har2tree.py` & `har2tree-1.9.2/har2tree/har2tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
-import logging
-from typing import Dict, Any, List, Optional, Tuple, Set, Union, Callable
+import hashlib
 import json
-from urllib.parse import unquote_plus
+import logging
+
+from collections import defaultdict
+from datetime import datetime, timedelta
+from functools import wraps, lru_cache
 from io import BytesIO
 from operator import itemgetter
-from collections import defaultdict
+from pathlib import Path
+from typing import Dict, Any, List, Optional, Tuple, Set, Union, Callable
+from urllib.parse import unquote_plus
+
 from .helper import rebuild_url, Har2TreeError, Har2TreeLogAdapter
 from .nodes import HostNode, URLNode
-from datetime import datetime, timedelta
-from functools import wraps
 
 # Dev debug mode is a mode that will print lots of things and will only be usable
 # by someone with a pretty deep understanding of har2tree and how the tree is built
 # The goal is to have a relatively simple way to investigate the construction of a tree itself
 # In order to enable it, it is assumed that you have the repository cloned on your machine
 # 1. Switch dev_debug_mode to True
 # 2. path_to_debug_files set a path to a directory of your choice, where you will create a file "url" or "hostname", with one line (the URL or the hostname)
@@ -426,14 +429,35 @@
         return self.url_tree.user_agent
 
     @property
     def start_time(self) -> datetime:
         """Start time of the capture"""
         return self.url_tree.start_time
 
+    @lru_cache
+    def build_all_hashes(self, algorithm: str='sha1') -> Dict[str, List[URLNode]]:
+        '''Build on demand hashes for all the ressources of the tree, in the alorighm provided by the user'''
+        if algorithm not in hashlib.algorithms_available:
+            raise Har2TreeError(f'Invalid algorithm ({algorithm}), only the following are supported: {hashlib.algorithms_available}')
+
+        to_return: Dict[str, List[URLNode]] = defaultdict(list)
+        for urlnode in self.url_tree.traverse():
+            if urlnode.empty_response:
+                continue
+            h = hashlib.new(algorithm)
+            h.update(urlnode.body.getbuffer())
+            to_return[h.hexdigest()].append(urlnode)
+            if hasattr(urlnode, 'embedded_ressources'):
+                for _mimetype, blobs in urlnode.embedded_ressources.items():
+                    for blob in blobs:
+                        h = hashlib.new(algorithm)
+                        h.update(blob[1].getbuffer())
+                        to_return[h.hexdigest()].append(urlnode)
+        return to_return
+
     def _load_url_entries(self) -> None:
         '''Initialize the list of nodes to attach to the tree (as URLNode),
         and create a list of note for each URL we have in the HAR document'''
 
         got_final_redirect: bool = False
 
         #  NOTE 2021-09-06 - Clear URL entries:
```

### Comparing `har2tree-1.9.1/har2tree/helper.py` & `har2tree-1.9.2/har2tree/helper.py`

 * *Files identical despite different names*

### Comparing `har2tree-1.9.1/har2tree/nodes.py` & `har2tree-1.9.2/har2tree/nodes.py`

 * *Files identical despite different names*

### Comparing `har2tree-1.9.1/har2tree/parser.py` & `har2tree-1.9.2/har2tree/parser.py`

 * *Files identical despite different names*

### Comparing `har2tree-1.9.1/pyproject.toml` & `har2tree-1.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "har2tree"
-version = "1.9.1"
+version = "1.9.2"
 description = "HTTP Archive (HAR) to ETE Toolkit generator"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/har2tree"
 documentation = "https://har2tree.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -26,27 +26,24 @@
 python = ">=3.8,<3.11"
 ete3 = "^3.1.2"
 beautifulsoup4 = "^4.10"
 lxml = "^4.6.3"
 six = "^1.16.0"
 publicsuffix2 = "^2.20191221"
 filetype = "^1.0.8"
-numpy = "^1.21.2"
+numpy = "^1.21.4"
 w3lib = "^1.22.0"
-Sphinx = { version = "^4.2.0", optional = true }
+Sphinx = { version = "^4.3.0", optional = true }
 cchardet = "^2.1.7"
 
 [tool.poetry.dev-dependencies]
-coverage = "^5.5"
-coveralls = "^3.0.1"
-codecov = "^2.1.12"
 mypy = "^0.910"
-nose = "^1.3.7"
-ipython = "^7.27.0"
-jupyterlab = "^3.1.18"
+ipython = "^7.30.0"
+jupyterlab = "^3.2.4"
+pytest-cov = "^3.0.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "myst-parser"]
 
 [build-system]
 requires = ["poetry_core>=1.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `har2tree-1.9.1/setup.py` & `har2tree-1.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 install_requires = \
 ['beautifulsoup4>=4.10,<5.0',
  'cchardet>=2.1.7,<3.0.0',
  'ete3>=3.1.2,<4.0.0',
  'filetype>=1.0.8,<2.0.0',
  'lxml>=4.6.3,<5.0.0',
- 'numpy>=1.21.2,<2.0.0',
+ 'numpy>=1.21.4,<2.0.0',
  'publicsuffix2>=2.20191221,<3.0',
  'six>=1.16.0,<2.0.0',
  'w3lib>=1.22.0,<2.0.0']
 
 extras_require = \
-{'docs': ['Sphinx>=4.2.0,<5.0.0']}
+{'docs': ['Sphinx>=4.3.0,<5.0.0']}
 
 setup_kwargs = {
     'name': 'har2tree',
-    'version': '1.9.1',
+    'version': '1.9.2',
     'description': 'HTTP Archive (HAR) to ETE Toolkit generator',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/har2tree/badge/?version=latest)](https://har2tree.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/Lookyloo/har2tree/branch/main/graph/badge.svg)](https://codecov.io/gh/Lookyloo/har2tree)\n\nHar2Tree\n========\n\n\nThis package generate a tree out of a HAR dump.\n\n\nInstallation\n============\n\n```bash\npip install har2tree\n```\n',
     'author': 'Raphaël Vinot',
     'author_email': 'raphael.vinot@circl.lu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Lookyloo/har2tree',
```

### Comparing `har2tree-1.9.1/PKG-INFO` & `har2tree-1.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: har2tree
-Version: 1.9.1
+Version: 1.9.2
 Summary: HTTP Archive (HAR) to ETE Toolkit generator
 Home-page: https://github.com/Lookyloo/har2tree
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.2.0,<5.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=4.3.0,<5.0.0); extra == "docs"
 Requires-Dist: beautifulsoup4 (>=4.10,<5.0)
 Requires-Dist: cchardet (>=2.1.7,<3.0.0)
 Requires-Dist: ete3 (>=3.1.2,<4.0.0)
 Requires-Dist: filetype (>=1.0.8,<2.0.0)
 Requires-Dist: lxml (>=4.6.3,<5.0.0)
-Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: numpy (>=1.21.4,<2.0.0)
 Requires-Dist: publicsuffix2 (>=2.20191221,<3.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: w3lib (>=1.22.0,<2.0.0)
 Project-URL: Documentation, https://har2tree.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Lookyloo/har2tree
 Description-Content-Type: text/markdown
```

