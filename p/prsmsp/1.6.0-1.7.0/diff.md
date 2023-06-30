# Comparing `tmp/prsmsp-1.6.0.tar.gz` & `tmp/prsmsp-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prsmsp-1.6.0.tar", last modified: Tue May 16 18:59:47 2023, max compression
+gzip compressed data, was "prsmsp-1.7.0.tar", last modified: Fri Jun 30 09:45:26 2023, max compression
```

## Comparing `prsmsp-1.6.0.tar` & `prsmsp-1.7.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.344678 prsmsp-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-16 18:59:47.344678 prsmsp-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-16 18:59:36.000000 prsmsp-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/abstracts/abcpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/factories/auth_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.344678 prsmsp-1.6.0/prsmsp/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/farazsms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/ghasedaksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/kavenegar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/mediana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/melipayamak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/niksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/sapak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/smsdotir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/smsone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/webonesms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 18:59:47.344678 prsmsp-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 18:59:36.000000 prsmsp-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.344678 prsmsp-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.450571 prsmsp-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-30 09:45:26.450571 prsmsp-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-30 09:45:14.000000 prsmsp-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.442571 prsmsp-1.7.0/prsmsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.442571 prsmsp-1.7.0/prsmsp/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/abstracts/abcpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.442571 prsmsp-1.7.0/prsmsp/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/exceptions/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/exceptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/exceptions/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.442571 prsmsp-1.7.0/prsmsp/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/factories/auth_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.446571 prsmsp-1.7.0/prsmsp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.450571 prsmsp-1.7.0/prsmsp/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/farazsms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/ghasedaksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/kavenegar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/mediana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/melipayamak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/niksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/sapak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/smsdotir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/smsone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-30 09:45:14.000000 prsmsp-1.7.0/prsmsp/panels/webonesms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.442571 prsmsp-1.7.0/prsmsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-30 09:45:26.000000 prsmsp-1.7.0/prsmsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 09:45:26.000000 prsmsp-1.7.0/prsmsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:45:26.000000 prsmsp-1.7.0/prsmsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 09:45:26.000000 prsmsp-1.7.0/prsmsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 09:45:26.000000 prsmsp-1.7.0/prsmsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 09:45:26.000000 prsmsp-1.7.0/prsmsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-30 09:45:26.450571 prsmsp-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 09:45:14.000000 prsmsp-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:26.450571 prsmsp-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 09:45:14.000000 prsmsp-1.7.0/tests/test_app.py
```

### Comparing `prsmsp-1.6.0/PKG-INFO` & `prsmsp-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.6.0
+Version: 1.7.0
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prsmsp Version: 1.6.0 Summary: Package to work with
+Metadata-Version: 2.1 Name: prsmsp Version: 1.7.0 Summary: Package to work with
 sms panels Home-page: https://github.com/parsariyahi/prsmsp Author: Parsa
 Riyahi Author-email: pany.parsariyahi@gmail.com License: MIT License Project-
 URL: Homepage, https://github.com/parsariyahi/prsmsp Project-URL:
 Documentation, https://prsmsp.readthedocs.io/en/latest/ Project-URL: Source,
 https://github.com/parsariyahi/prsmsp Project-URL: Tracker, https://github.com/
 parsariyahi/prsmsp/issues Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `prsmsp-1.6.0/README.md` & `prsmsp-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/factories/auth_factory.py` & `prsmsp-1.7.0/prsmsp/factories/auth_factory.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/models/response.py` & `prsmsp-1.7.0/prsmsp/models/response.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/farazsms.py` & `prsmsp-1.7.0/prsmsp/panels/farazsms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/ghasedaksms.py` & `prsmsp-1.7.0/prsmsp/panels/ghasedaksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/kavenegar.py` & `prsmsp-1.7.0/prsmsp/panels/kavenegar.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/mediana.py` & `prsmsp-1.7.0/prsmsp/panels/mediana.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/melipayamak.py` & `prsmsp-1.7.0/prsmsp/panels/melipayamak.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/niksms.py` & `prsmsp-1.7.0/prsmsp/panels/niksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/sapak.py` & `prsmsp-1.7.0/prsmsp/panels/sapak.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/smsdotir.py` & `prsmsp-1.7.0/prsmsp/panels/smsdotir.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/smsone.py` & `prsmsp-1.7.0/prsmsp/panels/smsone.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp/panels/webonesms.py` & `prsmsp-1.7.0/prsmsp/panels/webonesms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.6.0/prsmsp.egg-info/PKG-INFO` & `prsmsp-1.7.0/prsmsp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.6.0
+Version: 1.7.0
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prsmsp Version: 1.6.0 Summary: Package to work with
+Metadata-Version: 2.1 Name: prsmsp Version: 1.7.0 Summary: Package to work with
 sms panels Home-page: https://github.com/parsariyahi/prsmsp Author: Parsa
 Riyahi Author-email: pany.parsariyahi@gmail.com License: MIT License Project-
 URL: Homepage, https://github.com/parsariyahi/prsmsp Project-URL:
 Documentation, https://prsmsp.readthedocs.io/en/latest/ Project-URL: Source,
 https://github.com/parsariyahi/prsmsp Project-URL: Tracker, https://github.com/
 parsariyahi/prsmsp/issues Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `prsmsp-1.6.0/prsmsp.egg-info/SOURCES.txt` & `prsmsp-1.7.0/prsmsp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.cfg
 setup.py
 prsmsp/__init__.py
+prsmsp/panel.py
 prsmsp.egg-info/PKG-INFO
 prsmsp.egg-info/SOURCES.txt
 prsmsp.egg-info/dependency_links.txt
 prsmsp.egg-info/not-zip-safe
 prsmsp.egg-info/requires.txt
 prsmsp.egg-info/top_level.txt
 prsmsp/abstracts/__init__.py
```

### Comparing `prsmsp-1.6.0/setup.cfg` & `prsmsp-1.7.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prsmsp
-version = 1.6.0
+version = 1.7.0
 author = Parsa Riyahi
 author_email = pany.parsariyahi@gmail.com
 description = Package to work with sms panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = file: LICENSE
```

