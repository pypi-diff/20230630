# Comparing `tmp/problem_bank_helpers-0.1.8.tar.gz` & `tmp/problem_bank_helpers-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_helpers-0.1.8.tar", max compression
+gzip compressed data, was "problem_bank_helpers-0.1.9.tar", max compression
```

## Comparing `problem_bank_helpers-0.1.8.tar` & `problem_bank_helpers-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0        1 2021-06-14 01:41:43.016309 problem_bank_helpers-0.1.8/LICENSE
--rw-r--r--   0        0        0     1244 2021-06-14 01:41:43.033406 problem_bank_helpers-0.1.8/README.md
--rw-r--r--   0        0        0      783 2021-09-20 01:05:17.907474 problem_bank_helpers-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       59 2021-09-20 01:05:23.794844 problem_bank_helpers-0.1.8/src/problem_bank_helpers/__init__.py
--rw-r--r--   0        0        0    10035 2021-09-20 01:04:57.243384 problem_bank_helpers-0.1.8/src/problem_bank_helpers/problem_bank_helpers.py
--rw-r--r--   0        0        0     2069 2021-09-20 01:05:39.641224 problem_bank_helpers-0.1.8/setup.py
--rw-r--r--   0        0        0     2040 2021-09-20 01:05:39.641657 problem_bank_helpers-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-06-14 01:41:43.016309 problem_bank_helpers-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1244 2021-06-14 01:41:43.033405 problem_bank_helpers-0.1.9/README.md
+-rw-r--r--   0        0        0      783 2022-01-02 06:27:06.219645 problem_bank_helpers-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       59 2022-01-02 06:27:22.047869 problem_bank_helpers-0.1.9/src/problem_bank_helpers/__init__.py
+-rw-r--r--   0        0        0    10554 2022-01-02 05:50:00.099601 problem_bank_helpers-0.1.9/src/problem_bank_helpers/problem_bank_helpers.py
+-rw-r--r--   0        0        0     2069 2022-01-02 06:29:41.919962 problem_bank_helpers-0.1.9/setup.py
+-rw-r--r--   0        0        0     2040 2022-01-02 06:29:41.920435 problem_bank_helpers-0.1.9/PKG-INFO
```

### Comparing `problem_bank_helpers-0.1.8/README.md` & `problem_bank_helpers-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_helpers-0.1.8/pyproject.toml` & `problem_bank_helpers-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_helpers"
-version = "0.1.8"
+version = "0.1.9"
 description = "Helpful utilities for the open problem bank."
 authors = ["Firas Moosvi and Jake Bobowski"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_helpers.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_helpers"
 repository = "https://github.com/open-resources/problem_bank_helpers"
```

### Comparing `problem_bank_helpers-0.1.8/src/problem_bank_helpers/problem_bank_helpers.py` & `problem_bank_helpers-0.1.9/src/problem_bank_helpers/problem_bank_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # Author: Firas Moosvi, Jake Bobowski, others
 # Date: 2021-06-13
 
 from collections import defaultdict
 import numpy as np
 import sigfig
+import pandas as pd
+
+## Load data and dictionaries
+#global names,jumpers,vehicles,manual_vehicles,metals,T_c
+names = pd.read_csv("data/names.csv")["Names"].tolist()
+jumpers = pd.read_csv("data/jumpers.csv")["Jumpers"].tolist()
+vehicles = pd.read_csv("data/vehicles.csv")["Vehicles"].tolist()
+manual_vehicles = pd.read_csv("data/manual_vehicles.csv")["Manual Vehicles"].tolist()
+metals = pd.read_csv("data/metals.csv")["Metal"].tolist()
+T_c = pd.read_csv("data/metals.csv")["Temp Coeffecient"].tolist()
+## End Load data
 
 def create_data2():
 
     nested_dict = lambda: defaultdict(nested_dict)
     return nested_dict()
 
 def sigfigs(x):
```

### Comparing `problem_bank_helpers-0.1.8/setup.py` & `problem_bank_helpers-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.20.3,<2.0.0', 'sigfig>=1.1.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'problem-bank-helpers',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Helpful utilities for the open problem bank.',
     'long_description': '# Problem Bank Helpers \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_helpers/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_helpers)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_helpers/badge/?version=latest)](https://problem_bank_helpers.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_helpers\n```\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_helpers.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_helpers/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Firas Moosvi and Jake Bobowski',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_helpers',
```

### Comparing `problem_bank_helpers-0.1.8/PKG-INFO` & `problem_bank_helpers-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-helpers
-Version: 0.1.8
+Version: 0.1.9
 Summary: Helpful utilities for the open problem bank.
 Home-page: https://github.com/open-resources/problem_bank_helpers
 License: MIT
 Author: Firas Moosvi and Jake Bobowski
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

