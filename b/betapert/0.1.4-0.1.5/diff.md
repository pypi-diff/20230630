# Comparing `tmp/betapert-0.1.4.tar.gz` & `tmp/betapert-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betapert-0.1.4.tar", max compression
+gzip compressed data, was "betapert-0.1.5.tar", max compression
```

## Comparing `betapert-0.1.4.tar` & `betapert-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1597 2023-06-28 12:18:24.678241 betapert-0.1.4/README.md
--rw-r--r--   0        0        0     2713 2023-06-26 19:52:51.563296 betapert-0.1.4/betapert/__init__.py
--rw-r--r--   0        0        0     2814 2023-06-25 14:04:25.514803 betapert-0.1.4/betapert/funcs.py
--rw-r--r--   0        0        0      833 2023-06-28 12:18:27.159196 betapert-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 22:47:37.319709 betapert-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1099 2023-06-26 19:51:56.628431 betapert-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     1972 2023-06-25 13:03:16.467533 betapert-0.1.4/tests/test_frozen.py
--rw-r--r--   0        0        0      864 2023-06-25 14:04:25.517734 betapert-0.1.4/tests/test_generalization.py
--rw-r--r--   0        0        0     3790 2023-06-25 13:55:10.358243 betapert-0.1.4/tests/test_mpert_parametrized.py
--rw-r--r--   0        0        0     1487 2023-06-25 14:04:25.516401 betapert-0.1.4/tests/test_special_cases.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 betapert-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1597 2023-06-28 12:18:24.678241 betapert-0.1.5/README.md
+-rw-r--r--   0        0        0     4359 2023-06-30 17:47:22.818316 betapert-0.1.5/betapert/__init__.py
+-rw-r--r--   0        0        0     2814 2023-06-25 14:04:25.514803 betapert-0.1.5/betapert/funcs.py
+-rw-r--r--   0        0        0      833 2023-06-30 18:52:14.678593 betapert-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 22:47:37.319709 betapert-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1099 2023-06-26 19:51:56.628431 betapert-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     1972 2023-06-25 13:03:16.467533 betapert-0.1.5/tests/test_frozen.py
+-rw-r--r--   0        0        0      864 2023-06-25 14:04:25.517734 betapert-0.1.5/tests/test_generalization.py
+-rw-r--r--   0        0        0     3790 2023-06-25 13:55:10.358243 betapert-0.1.5/tests/test_mpert_parametrized.py
+-rw-r--r--   0        0        0     1487 2023-06-25 14:04:25.516401 betapert-0.1.5/tests/test_special_cases.py
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 betapert-0.1.5/PKG-INFO
```

### Comparing `betapert-0.1.4/README.md` & `betapert-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/betapert/funcs.py` & `betapert-0.1.5/betapert/funcs.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/pyproject.toml` & `betapert-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "betapert"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/tadamcz/betapert"
 description = "Top-level package for beta-PERT distribution."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `betapert-0.1.4/tests/conftest.py` & `betapert-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/tests/test_frozen.py` & `betapert-0.1.5/tests/test_frozen.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/tests/test_generalization.py` & `betapert-0.1.5/tests/test_generalization.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/tests/test_mpert_parametrized.py` & `betapert-0.1.5/tests/test_mpert_parametrized.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/tests/test_special_cases.py` & `betapert-0.1.5/tests/test_special_cases.py`

 * *Files identical despite different names*

### Comparing `betapert-0.1.4/PKG-INFO` & `betapert-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betapert
-Version: 0.1.4
+Version: 0.1.5
 Summary: Top-level package for beta-PERT distribution.
 Home-page: https://github.com/tadamcz/betapert
 Author: Tom Adamczewski
 Author-email: tadamczewskipublic@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

