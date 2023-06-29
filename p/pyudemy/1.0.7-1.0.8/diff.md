# Comparing `tmp/pyudemy-1.0.7.tar.gz` & `tmp/pyudemy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyudemy-1.0.7.tar", max compression
+gzip compressed data, was "pyudemy-1.0.8.tar", max compression
```

## Comparing `pyudemy-1.0.7.tar` & `pyudemy-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1071 2022-08-31 22:30:44.206403 pyudemy-1.0.7/LICENSE
--rw-r--r--   0        0        0     3204 2022-08-31 23:35:03.916461 pyudemy-1.0.7/README.md
--rw-r--r--   0        0        0      738 2022-08-31 23:51:19.426476 pyudemy-1.0.7/pyproject.toml
--rw-r--r--   0        0        0       48 2022-08-31 23:51:17.926475 pyudemy-1.0.7/pyudemy/__init__.py
--rw-r--r--   0        0        0     4465 2022-08-31 23:06:30.496435 pyudemy-1.0.7/pyudemy/udemy.py
--rw-r--r--   0        0        0     4003 2022-08-31 23:51:57.276569 pyudemy-1.0.7/setup.py
--rw-r--r--   0        0        0     3879 2022-08-31 23:51:57.276898 pyudemy-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-29 02:53:06.867524 pyudemy-1.0.8/LICENSE
+-rw-r--r--   0        0        0     3035 2023-06-29 02:53:06.867524 pyudemy-1.0.8/README.md
+-rw-r--r--   0        0        0      739 2023-06-29 03:12:24.257175 pyudemy-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-29 03:12:24.257175 pyudemy-1.0.8/pyudemy/__init__.py
+-rw-r--r--   0        0        0     4477 2023-06-29 03:12:06.497180 pyudemy-1.0.8/pyudemy/udemy.py
+-rw-r--r--   0        0        0     3761 1970-01-01 00:00:00.000000 pyudemy-1.0.8/PKG-INFO
```

### Comparing `pyudemy-1.0.7/LICENSE` & `pyudemy-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyudemy-1.0.7/README.md` & `pyudemy-1.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # Pyudemy
 
 [![Python package](https://github.com/hudsonbrendon/pyudemy/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/hudsonbrendon/pyudemy/actions/workflows/pythonpackage.yml)
-[![Build Status](https://travis-ci.org/hudsonbrendon/pyudemy.svg?branch=master)](https://travis-ci.org/hudsonbrendon/pyudemy)
 [![Github Issues](http://img.shields.io/github/issues/hudsonbrendon/pyudemy.svg?style=flat)](https://github.com/hudsonbrendon/pyudemy/issues?sort=updated&state=open)
 ![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)
 
 Simple integrate of API udemy.com with python
 
 # Quick start
 
 ```bash
 $ pip install pyudemy
 ```
-or
-
-```bash
-$ python setup.py install
-```
-
 # Authentication
 
 To make any calls to Udemy REST API, you will need to create an API client. API client consists of a bearer token, which is connected to a user account on Udemy.
 
 If you want to create an API client, [Sign up on udemy.com](https://www.udemy.com/join/) and go to API Clients page in your user profile. Once your API client request is approved, your newly created [API client](https://www.udemy.com/user/edit-api-clients/) will be active and your bearer token will be visible on [API Clients](https://www.udemy.com/user/edit-api-clients/) page.
 
 # Usage
```

### Comparing `pyudemy-1.0.7/pyproject.toml` & `pyudemy-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyudemy"
-version = "1.0.7"
+version = "1.0.8"
 description = "Simple integrate of API udemy.com with python"
 authors = ["Hudson Brendon <contato.hudsonbrendon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hudsonbrendon/pyudemy"
 homepage = "https://github.com/hudsonbrendon/pyudemy#readme"
 
@@ -26,8 +26,8 @@
 [settings]
 known_third_party = ["pytest", "requests"]
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
-profile = "black"
+profile = "black"
```

### Comparing `pyudemy-1.0.7/pyudemy/udemy.py` & `pyudemy-1.0.8/pyudemy/udemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         Args:
             id (int): Curriculum id.
 
         Returns:
             dict: List of curriculum items.
         """
         return requests.get(
-            self._get_full_url(f"courses/{id}/public-curriculum-items"),
+            self._get_full_url(f"courses/{id}/public-curriculum-items/?", **kwargs),
             auth=self._authentication,
         ).json()
 
     def course_reviews(self, id: int, **kwargs) -> dict:
         """Returns list of reviews items.
 
         To see the list of accepted parameters go to:
```

### Comparing `pyudemy-1.0.7/setup.py` & `pyudemy-1.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,123 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyudemy
+Version: 1.0.8
+Summary: Simple integrate of API udemy.com with python
+Home-page: https://github.com/hudsonbrendon/pyudemy#readme
+License: MIT
+Author: Hudson Brendon
+Author-email: contato.hudsonbrendon@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/hudsonbrendon/pyudemy
+Description-Content-Type: text/markdown
 
-packages = \
-['pyudemy']
+# Pyudemy
 
-package_data = \
-{'': ['*']}
+[![Python package](https://github.com/hudsonbrendon/pyudemy/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/hudsonbrendon/pyudemy/actions/workflows/pythonpackage.yml)
+[![Github Issues](http://img.shields.io/github/issues/hudsonbrendon/pyudemy.svg?style=flat)](https://github.com/hudsonbrendon/pyudemy/issues?sort=updated&state=open)
+![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)
 
-install_requires = \
-['requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pyudemy',
-    'version': '1.0.7',
-    'description': 'Simple integrate of API udemy.com with python',
-    'long_description': '# Pyudemy\n\n[![Python package](https://github.com/hudsonbrendon/pyudemy/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/hudsonbrendon/pyudemy/actions/workflows/pythonpackage.yml)\n[![Build Status](https://travis-ci.org/hudsonbrendon/pyudemy.svg?branch=master)](https://travis-ci.org/hudsonbrendon/pyudemy)\n[![Github Issues](http://img.shields.io/github/issues/hudsonbrendon/pyudemy.svg?style=flat)](https://github.com/hudsonbrendon/pyudemy/issues?sort=updated&state=open)\n![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)\n\nSimple integrate of API udemy.com with python\n\n# Quick start\n\n```bash\n$ pip install pyudemy\n```\nor\n\n```bash\n$ python setup.py install\n```\n\n# Authentication\n\nTo make any calls to Udemy REST API, you will need to create an API client. API client consists of a bearer token, which is connected to a user account on Udemy.\n\nIf you want to create an API client, [Sign up on udemy.com](https://www.udemy.com/join/) and go to API Clients page in your user profile. Once your API client request is approved, your newly created [API client](https://www.udemy.com/user/edit-api-clients/) will be active and your bearer token will be visible on [API Clients](https://www.udemy.com/user/edit-api-clients/) page.\n\n# Usage\n\nWith your key in hand, it\'s time to authenticate, so run:\n\n```python\n>>> from pyudemy import Udemy\n\n>>> udemy = Udemy(<CLIENT_ID>, <CLIENT_SECRET>)\n```\n\n# Courses\n\nReturns list of courses.\n\nTo see the list of accepted parameters go to:\n[https://www.udemy.com/developers/methods/get-courses-list/](https://www.udemy.com/developers/methods/get-courses-list/)\n\n```python\n>>> udemy.courses()\n```\nor\n\n```python\n>>> udemy.courses(page=1, page_size=1, ...)\n```\n\n# Course detail\n\nReturns course with specified id.\n\nTo see the list of accepted parameters go to:\n[https://www.udemy.com/developers/methods/get-courses-detail/](https://www.udemy.com/developers/methods/get-courses-detail/)\n\n```python\n>>> udemy.course_detail(<id>)\n```\n\n# Public curriculum\n\nReturns list of curriculum items.\n\nTo see the list of accepted parameters go to:\n[https://www.udemy.com/developers/methods/get-publiccurriculum-list/](https://www.udemy.com/developers/methods/get-publiccurriculum-list/)\n\n```python\n>>> udemy.public_curriculum(<id>)\n```\nor\n\n```python\n>>> udemy.public_curriculum(<id>, page=1, page_size=1)\n```\n\n# Course reviews\n\nReturns list of curriculum items.\n\nTo see the list of accepted parameters go to:\n[https://www.udemy.com/developers/methods/get-coursereviews-list/](https://www.udemy.com/developers/methods/get-coursereviews-list/)\n\n```python\n>>> udemy.course_reviews(<id>)\n```\nor\n\n```python\n>>> udemy.course_reviews(<id>, page=1, page_size=1)\n```\n# Controlling return Data\n\nYou can now control the return data from the API using a list of dictionaries passed under a parameter called "fields".\n![image](https://user-images.githubusercontent.com/33434582/160966081-b1f67fe2-48db-45d1-b102-95ef90e7c0cb.png)\n\n\nFor more info check Use of Fields and Field Lists at https://www.udemy.com/developers/affiliate/\n\n# Dependencies\n\n- Python >=3.8\n- [Pipenv](https://github.com/kennethreitz/pipenv)\n\n# License\n\n[MIT](http://en.wikipedia.org/wiki/MIT_License)\n',
-    'author': 'Hudson Brendon',
-    'author_email': 'contato.hudsonbrendon@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/hudsonbrendon/pyudemy#readme',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Simple integrate of API udemy.com with python
 
+# Quick start
+
+```bash
+$ pip install pyudemy
+```
+# Authentication
+
+To make any calls to Udemy REST API, you will need to create an API client. API client consists of a bearer token, which is connected to a user account on Udemy.
+
+If you want to create an API client, [Sign up on udemy.com](https://www.udemy.com/join/) and go to API Clients page in your user profile. Once your API client request is approved, your newly created [API client](https://www.udemy.com/user/edit-api-clients/) will be active and your bearer token will be visible on [API Clients](https://www.udemy.com/user/edit-api-clients/) page.
+
+# Usage
+
+With your key in hand, it's time to authenticate, so run:
+
+```python
+>>> from pyudemy import Udemy
+
+>>> udemy = Udemy(<CLIENT_ID>, <CLIENT_SECRET>)
+```
+
+# Courses
+
+Returns list of courses.
+
+To see the list of accepted parameters go to:
+[https://www.udemy.com/developers/methods/get-courses-list/](https://www.udemy.com/developers/methods/get-courses-list/)
+
+```python
+>>> udemy.courses()
+```
+or
+
+```python
+>>> udemy.courses(page=1, page_size=1, ...)
+```
+
+# Course detail
+
+Returns course with specified id.
+
+To see the list of accepted parameters go to:
+[https://www.udemy.com/developers/methods/get-courses-detail/](https://www.udemy.com/developers/methods/get-courses-detail/)
+
+```python
+>>> udemy.course_detail(<id>)
+```
+
+# Public curriculum
+
+Returns list of curriculum items.
+
+To see the list of accepted parameters go to:
+[https://www.udemy.com/developers/methods/get-publiccurriculum-list/](https://www.udemy.com/developers/methods/get-publiccurriculum-list/)
+
+```python
+>>> udemy.public_curriculum(<id>)
+```
+or
+
+```python
+>>> udemy.public_curriculum(<id>, page=1, page_size=1)
+```
+
+# Course reviews
+
+Returns list of curriculum items.
+
+To see the list of accepted parameters go to:
+[https://www.udemy.com/developers/methods/get-coursereviews-list/](https://www.udemy.com/developers/methods/get-coursereviews-list/)
+
+```python
+>>> udemy.course_reviews(<id>)
+```
+or
+
+```python
+>>> udemy.course_reviews(<id>, page=1, page_size=1)
+```
+# Controlling return Data
+
+You can now control the return data from the API using a list of dictionaries passed under a parameter called "fields".
+![image](https://user-images.githubusercontent.com/33434582/160966081-b1f67fe2-48db-45d1-b102-95ef90e7c0cb.png)
+
+
+For more info check Use of Fields and Field Lists at https://www.udemy.com/developers/affiliate/
+
+# Dependencies
+
+- Python >=3.8
+- [Pipenv](https://github.com/kennethreitz/pipenv)
+
+# License
+
+[MIT](http://en.wikipedia.org/wiki/MIT_License)
 
-setup(**setup_kwargs)
```

