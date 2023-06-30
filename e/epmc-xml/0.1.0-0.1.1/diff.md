# Comparing `tmp/epmc_xml-0.1.0.tar.gz` & `tmp/epmc_xml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epmc_xml-0.1.0.tar", max compression
+gzip compressed data, was "epmc_xml-0.1.1.tar", max compression
```

## Comparing `epmc_xml-0.1.0.tar` & `epmc_xml-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      334 2023-05-30 19:07:41.122842 epmc_xml-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-30 18:58:25.315802 epmc_xml-0.1.0/epmc_xml/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-30 19:15:50.996869 epmc_xml-0.1.0/epmc_xml/article.py
--rw-r--r--   0        0        0     2501 2023-05-31 08:15:33.009305 epmc_xml-0.1.0/epmc_xml/fetch.py
--rw-r--r--   0        0        0      429 2023-05-30 18:38:41.389833 epmc_xml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 epmc_xml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 15:04:36.154342 epmc_xml-0.1.1/LICENSE
+-rw-r--r--   0        0        0      334 2023-05-30 19:07:41.122842 epmc_xml-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 18:58:25.315802 epmc_xml-0.1.1/epmc_xml/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-30 19:15:50.996869 epmc_xml-0.1.1/epmc_xml/article.py
+-rw-r--r--   0        0        0     2866 2023-06-30 15:02:35.841091 epmc_xml-0.1.1/epmc_xml/fetch.py
+-rw-r--r--   0        0        0      428 2023-06-30 15:12:03.284847 epmc_xml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 epmc_xml-0.1.1/PKG-INFO
```

### Comparing `epmc_xml-0.1.0/epmc_xml/article.py` & `epmc_xml-0.1.1/epmc_xml/article.py`

 * *Files identical despite different names*

### Comparing `epmc_xml-0.1.0/PKG-INFO` & `epmc_xml-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: epmc-xml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Get articles from Europe PMC as xml for further processing
 License: MIT
 Author: Andrew Green
 Author-email: a.f.green1@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ratelimiter (>=1.2.0.post0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Europe PMC python client
```

