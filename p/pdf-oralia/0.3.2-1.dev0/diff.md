# Comparing `tmp/pdf_oralia-0.3.2.tar.gz` & `tmp/pdf_oralia-1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_oralia-0.3.2.tar", max compression
+gzip compressed data, was "pdf_oralia-1.dev0.tar", max compression
```

## Comparing `pdf_oralia-0.3.2.tar` & `pdf_oralia-1.dev0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       73 2023-06-27 10:06:56.067452 pdf_oralia-0.3.2/README.md
--rw-r--r--   0        0        0        0 2022-09-25 16:31:06.006810 pdf_oralia-0.3.2/pdf_oralia/__init__.py
--rw-r--r--   0        0        0     3056 2023-06-27 10:06:56.057452 pdf_oralia-0.3.2/pdf_oralia/extract.py
--rw-r--r--   0        0        0       59 2023-06-27 10:06:56.057452 pdf_oralia-0.3.2/pdf_oralia/pages/__init__.py
--rw-r--r--   0        0        0     2206 2023-06-28 08:49:15.626889 pdf_oralia-0.3.2/pdf_oralia/pages/charge.py
--rw-r--r--   0        0        0     4206 2023-06-28 08:44:52.543543 pdf_oralia-0.3.2/pdf_oralia/pages/locataire.py
--rw-r--r--   0        0        0       99 2023-06-27 10:06:56.057452 pdf_oralia-0.3.2/pdf_oralia/pages/patrimoine.py
--rw-r--r--   0        0        0      904 2023-06-27 10:06:56.057452 pdf_oralia-0.3.2/pdf_oralia/pages/recapitulatif.py
--rw-r--r--   0        0        0     1542 2023-06-28 08:10:13.303448 pdf_oralia-0.3.2/pdf_oralia/scripts.py
--rw-r--r--   0        0        0      563 2023-06-30 11:38:30.976690 pdf_oralia-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 pdf_oralia-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       73 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/__init__.py
+-rw-r--r--   0        0        0     3056 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/extract.py
+-rw-r--r--   0        0        0       59 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/charge.py
+-rw-r--r--   0        0        0     4206 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/locataire.py
+-rw-r--r--   0        0        0       99 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/patrimoine.py
+-rw-r--r--   0        0        0      904 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/recapitulatif.py
+-rw-r--r--   0        0        0     1542 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/scripts.py
+-rw-r--r--   0        0        0      562 2023-06-30 11:31:19.790868 pdf_oralia-1.dev0/pyproject.toml
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 pdf_oralia-1.dev0/PKG-INFO
```

### Comparing `pdf_oralia-0.3.2/pdf_oralia/extract.py` & `pdf_oralia-1.dev0/pdf_oralia/extract.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.2/pdf_oralia/pages/charge.py` & `pdf_oralia-1.dev0/pdf_oralia/pages/charge.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.2/pdf_oralia/pages/locataire.py` & `pdf_oralia-1.dev0/pdf_oralia/pages/locataire.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.2/pdf_oralia/pages/recapitulatif.py` & `pdf_oralia-1.dev0/pdf_oralia/pages/recapitulatif.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.2/pdf_oralia/scripts.py` & `pdf_oralia-1.dev0/pdf_oralia/scripts.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.2/pyproject.toml` & `pdf_oralia-1.dev0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-oralia"
-version = "v0.3.2"
+version = "1.dev"
 description = ""
 authors = ["Bertrand Benjamin <benjamin.bertrand@opytex.org>"]
 readme = "README.md"
 packages = [{include = "pdf_oralia"}]
 
 [tool.poetry.scripts]
 pdf-oralia = "pdf_oralia.scripts:main"
```

### Comparing `pdf_oralia-0.3.2/PKG-INFO` & `pdf_oralia-1.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-oralia
-Version: 0.3.2
+Version: 1.dev0
 Summary: 
 Author: Bertrand Benjamin
 Author-email: benjamin.bertrand@opytex.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

