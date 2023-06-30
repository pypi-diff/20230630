# Comparing `tmp/funkagent-0.0.2.tar.gz` & `tmp/funkagent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkagent-0.0.2.tar", max compression
+gzip compressed data, was "funkagent-0.0.3.tar", max compression
```

## Comparing `funkagent-0.0.2.tar` & `funkagent-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       62 2023-06-28 02:20:17.486654 funkagent-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-18 11:40:51.943567 funkagent-0.0.2/funkagent/__init__.py
--rw-r--r--   0        0        0     5374 2023-06-20 04:10:41.717528 funkagent-0.0.2/funkagent/agents.py
--rw-r--r--   0        0        0     2059 2023-06-28 02:32:49.032389 funkagent-0.0.2/funkagent/parser.py
--rw-r--r--   0        0        0      330 2023-06-28 02:34:15.838360 funkagent-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 funkagent-0.0.2/setup.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 funkagent-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-06-28 02:20:17.486654 funkagent-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 11:40:51.943567 funkagent-0.0.3/funkagent/__init__.py
+-rw-r--r--   0        0        0     5374 2023-06-20 04:10:41.717528 funkagent-0.0.3/funkagent/agents.py
+-rw-r--r--   0        0        0     2059 2023-06-28 02:32:49.032389 funkagent-0.0.3/funkagent/parser.py
+-rw-r--r--   0        0        0      330 2023-06-30 04:32:15.115306 funkagent-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 funkagent-0.0.3/setup.py
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 funkagent-0.0.3/PKG-INFO
```

### Comparing `funkagent-0.0.2/funkagent/agents.py` & `funkagent-0.0.3/funkagent/agents.py`

 * *Files identical despite different names*

### Comparing `funkagent-0.0.2/funkagent/parser.py` & `funkagent-0.0.3/funkagent/parser.py`

 * *Files identical despite different names*

### Comparing `funkagent-0.0.2/setup.py` & `funkagent-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['openai>=0.27.8,<0.28.0']
 
 setup_kwargs = {
     'name': 'funkagent',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Minimal agent framework using OpenAI functions',
     'long_description': '# FunkAgent\n\nGet started with:\n\n```\npip install funkagent\n```\n',
     'author': 'James Briggs',
     'author_email': 'james@aurelio.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `funkagent-0.0.2/PKG-INFO` & `funkagent-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funkagent
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimal agent framework using OpenAI functions
 Author: James Briggs
 Author-email: james@aurelio.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

