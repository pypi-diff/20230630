# Comparing `tmp/spaces-0.6.0.tar.gz` & `tmp/spaces-0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.6.0.tar", max compression
+gzip compressed data, was "spaces-0.6b1.tar", max compression
```

## Comparing `spaces-0.6.0.tar` & `spaces-0.6b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.6.0/README.md
--rw-r--r--   0        0        0     1489 2023-06-30 16:02:58.255535 spaces-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.6.0/spaces/__init__.py
--rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.6.0/spaces/config.py
--rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.6.0/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-29 12:42:06.802062 spaces-0.6.0/spaces/gpu/client.py
--rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.6.0/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3581 2023-06-29 12:16:02.996586 spaces-0.6.0/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.6.0/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.6.0/spaces/gradio.py
--rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.6.0/spaces/utils.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.6.0/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.6b1/README.md
+-rw-r--r--   0        0        0     1489 2023-06-30 16:02:24.855918 spaces-0.6b1/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.6b1/spaces/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.6b1/spaces/config.py
+-rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.6b1/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-29 12:42:06.802062 spaces-0.6b1/spaces/gpu/client.py
+-rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.6b1/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3581 2023-06-29 12:16:02.996586 spaces-0.6b1/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.6b1/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.6b1/spaces/gradio.py
+-rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.6b1/spaces/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.6b1/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.6b1/PKG-INFO
```

### Comparing `spaces-0.6.0/pyproject.toml` & `spaces-0.6b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.6.0"
+version = "0.6b1"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
```

### Comparing `spaces-0.6.0/spaces/gpu/client.py` & `spaces-0.6b1/spaces/gpu/client.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.0/spaces/gpu/decorator.py` & `spaces-0.6b1/spaces/gpu/decorator.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.0/spaces/gpu/torch.py` & `spaces-0.6b1/spaces/gpu/torch.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.0/spaces/gpu/wrappers.py` & `spaces-0.6b1/spaces/gpu/wrappers.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.0/spaces/gradio.py` & `spaces-0.6b1/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.0/spaces/utils.py` & `spaces-0.6b1/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.0/setup.py` & `spaces-0.6b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.6.0',
+    'version': '0.6b1',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.6.0/PKG-INFO` & `spaces-0.6b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.6.0
+Version: 0.6b1
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

