# Comparing `tmp/adaptwms-0.1.1.tar.gz` & `tmp/adaptwms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptwms-0.1.1.tar", max compression
+gzip compressed data, was "adaptwms-0.1.2.tar", max compression
```

## Comparing `adaptwms-0.1.1.tar` & `adaptwms-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-30 19:34:53.010438 adaptwms-0.1.1/LICENSE
--rw-r--r--   0        0        0     2523 2023-06-30 19:34:53.010438 adaptwms-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/__init__.py
--rw-r--r--   0        0        0       63 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/admin.py
--rw-r--r--   0        0        0      148 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/apps.py
--rw-r--r--   0        0        0        0 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/models.py
--rw-r--r--   0        0        0       60 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/tests.py
--rw-r--r--   0        0        0     1000 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/translator.py
--rw-r--r--   0        0        0     1515 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/views.py
--rw-r--r--   0        0        0      488 2023-06-30 19:34:53.014438 adaptwms-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 adaptwms-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 19:45:13.251359 adaptwms-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2523 2023-06-30 19:45:13.251359 adaptwms-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/admin.py
+-rw-r--r--   0        0        0      148 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/apps.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/models.py
+-rw-r--r--   0        0        0     1010 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/templates/pages/interface.html
+-rw-r--r--   0        0        0      176 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/templates/template.html
+-rw-r--r--   0        0        0       60 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/tests.py
+-rw-r--r--   0        0        0     1000 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/translator.py
+-rw-r--r--   0        0        0     1515 2023-06-30 19:45:13.251359 adaptwms-0.1.2/adaptwms/views.py
+-rw-r--r--   0        0        0      523 2023-06-30 19:45:13.251359 adaptwms-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 adaptwms-0.1.2/PKG-INFO
```

### Comparing `adaptwms-0.1.1/LICENSE` & `adaptwms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.1/README.md` & `adaptwms-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.1/adaptwms/translator.py` & `adaptwms-0.1.2/adaptwms/translator.py`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.1/adaptwms/views.py` & `adaptwms-0.1.2/adaptwms/views.py`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.1/PKG-INFO` & `adaptwms-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptwms
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight OpenStreetMap adapter for WMS services as Django app
 Home-page: https://github.com/v3l0c1r4pt0r/adaptwms
 Author: v3l0c1r4pt0r
 Author-email: v3l0c1r4pt0r@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

