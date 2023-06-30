# Comparing `tmp/adaptwms-0.1.0.tar.gz` & `tmp/adaptwms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptwms-0.1.0.tar", max compression
+gzip compressed data, was "adaptwms-0.1.1.tar", max compression
```

## Comparing `adaptwms-0.1.0.tar` & `adaptwms-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     2523 2023-06-30 19:22:44.759502 adaptwms-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/__init__.py
--rw-r--r--   0        0        0       63 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/admin.py
--rw-r--r--   0        0        0      148 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/apps.py
--rw-r--r--   0        0        0        0 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/models.py
--rw-r--r--   0        0        0       60 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/tests.py
--rw-r--r--   0        0        0     1000 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/translator.py
--rw-r--r--   0        0        0     1515 2023-06-30 19:22:44.759502 adaptwms-0.1.0/adaptwms/views.py
--rw-r--r--   0        0        0      328 2023-06-30 19:22:44.759502 adaptwms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 adaptwms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 19:34:53.010438 adaptwms-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2523 2023-06-30 19:34:53.010438 adaptwms-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/admin.py
+-rw-r--r--   0        0        0      148 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/apps.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/models.py
+-rw-r--r--   0        0        0       60 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/tests.py
+-rw-r--r--   0        0        0     1000 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/translator.py
+-rw-r--r--   0        0        0     1515 2023-06-30 19:34:53.010438 adaptwms-0.1.1/adaptwms/views.py
+-rw-r--r--   0        0        0      488 2023-06-30 19:34:53.014438 adaptwms-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 adaptwms-0.1.1/PKG-INFO
```

### Comparing `adaptwms-0.1.0/README.md` & `adaptwms-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.0/adaptwms/translator.py` & `adaptwms-0.1.1/adaptwms/translator.py`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.0/adaptwms/views.py` & `adaptwms-0.1.1/adaptwms/views.py`

 * *Files identical despite different names*

### Comparing `adaptwms-0.1.0/PKG-INFO` & `adaptwms-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: adaptwms
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Lightweight OpenStreetMap adapter for WMS services as Django app
+Home-page: https://github.com/v3l0c1r4pt0r/adaptwms
 Author: v3l0c1r4pt0r
 Author-email: v3l0c1r4pt0r@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.2.2,<5.0.0)
 Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/v3l0c1r4pt0r/adaptwms
 Description-Content-Type: text/markdown
 
 # adaptwms
 Lightweight OpenStreetMap adapter for WMS services
 
 ## What it is?
```

