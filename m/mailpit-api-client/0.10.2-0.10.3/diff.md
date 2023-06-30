# Comparing `tmp/mailpit-api-client-0.10.2.tar.gz` & `tmp/mailpit-api-client-0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailpit-api-client-0.10.2.tar", last modified: Fri Jun 30 13:32:05 2023, max compression
+gzip compressed data, was "mailpit-api-client-0.10.3.tar", last modified: Fri Jun 30 13:32:46 2023, max compression
```

## Comparing `mailpit-api-client-0.10.2.tar` & `mailpit-api-client-0.10.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/mailpit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/mailpit/client/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/mailpit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/testing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/mailpit/testing/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/mailpit_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-30 13:32:05.000000 mailpit-api-client-0.10.2/mailpit_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 13:32:05.000000 mailpit-api-client-0.10.2/mailpit_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:32:05.000000 mailpit-api-client-0.10.2/mailpit_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 13:32:05.000000 mailpit-api-client-0.10.2/mailpit_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 13:32:05.000000 mailpit-api-client-0.10.2/mailpit_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-30 13:31:54.000000 mailpit-api-client-0.10.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:32:05.017720 mailpit-api-client-0.10.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/testing/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/mailpit/testing/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 13:32:46.000000 mailpit-api-client-0.10.3/mailpit_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-30 13:32:36.000000 mailpit-api-client-0.10.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:32:46.216628 mailpit-api-client-0.10.3/setup.cfg
```

### Comparing `mailpit-api-client-0.10.2/LICENSE` & `mailpit-api-client-0.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.2/PKG-INFO` & `mailpit-api-client-0.10.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.10.2
+Version: 0.10.3
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -197,15 +197,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.10.2
+    0.10.3
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
```

### Comparing `mailpit-api-client-0.10.2/README.rst` & `mailpit-api-client-0.10.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.10.2
+    0.10.3
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
```

### Comparing `mailpit-api-client-0.10.2/mailpit/client/api.py` & `mailpit-api-client-0.10.3/mailpit/client/api.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.2/mailpit/client/models.py` & `mailpit-api-client-0.10.3/mailpit/client/models.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.2/mailpit/testing/pytest.py` & `mailpit-api-client-0.10.3/mailpit/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.2/mailpit/testing/unittest.py` & `mailpit-api-client-0.10.3/mailpit/testing/unittest.py`

 * *Files identical despite different names*

### Comparing `mailpit-api-client-0.10.2/mailpit_api_client.egg-info/PKG-INFO` & `mailpit-api-client-0.10.3/mailpit_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailpit-api-client
-Version: 0.10.2
+Version: 0.10.3
 Summary: A Mailpit API Client
 Author-email: Lars Liedtke <lars@familie-liedtke.net>
 License: GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -197,15 +197,15 @@
 -------------------------------------------------------------------
 API-client for https://github.com/axllent/mailpit written in Python
 -------------------------------------------------------------------
 
 :Authors:
     Lars Liedtke <corvan@gmx.de>
 :Version:
-    0.10.2
+    0.10.3
 
 ----------
 Motivation
 ----------
 For work, I thought about introducing integration testing.
 We are working with `Odoo <https://github.com/odoo/odoo>`_  and I wanted to test if e-mails created by Odoo really were sent.
 I remembered `mailhog <https://github.com/mailhog/MailHog>`_, which I discovered to be abandoned.
```

### Comparing `mailpit-api-client-0.10.2/pyproject.toml` & `mailpit-api-client-0.10.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mailpit-api-client"
-version = "0.10.2"
+version = "0.10.3"
 description = "A Mailpit API Client"
 authors = [{name = "Lars Liedtke", email = "lars@familie-liedtke.net"}]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Framework :: Pytest",
@@ -73,15 +73,15 @@
 pytest-docker = "^1.0.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 
 [tool.poetry.group.test.dependencies]
 black = "*"
-mypy = "^1.1.1"
+mypy = "^1.4.1"
 pylint = "*"
 respx = "*"
 pytest = "^7"
 
 [tool.poetry.group.pytest.dependencies]
 pytest = "^7"
```

