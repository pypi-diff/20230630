# Comparing `tmp/foursight_smaht-0.0.0.1b1.tar.gz` & `tmp/foursight_smaht-0.0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_smaht-0.0.0.1b1.tar", max compression
+gzip compressed data, was "foursight_smaht-0.0.0.1b2.tar", max compression
```

## Comparing `foursight_smaht-0.0.0.1b1.tar` & `foursight_smaht-0.0.0.1b2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2023-06-29 16:16:46.829708 foursight_smaht-0.0.0.1b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-29 16:16:46.830680 foursight_smaht-0.0.0.1b1/chalicelib_smaht/__init__.py
--rw-r--r--   0        0        0     1030 2023-06-30 14:13:49.029298 foursight_smaht-0.0.0.1b1/chalicelib_smaht/app_utils.py
--rw-r--r--   0        0        0      873 2023-06-30 14:21:01.676349 foursight_smaht-0.0.0.1b1/chalicelib_smaht/buckets.py
--rw-r--r--   0        0        0     4805 2023-06-29 16:16:46.831422 foursight_smaht-0.0.0.1b1/chalicelib_smaht/check_schedules.py
--rw-r--r--   0        0        0    13354 2023-06-30 14:22:35.139013 foursight_smaht-0.0.0.1b1/chalicelib_smaht/check_setup.json
--rw-r--r--   0        0        0     9278 2023-06-29 16:16:46.832258 foursight_smaht-0.0.0.1b1/chalicelib_smaht/check_setup.json-local
--rw-r--r--   0        0        0      249 2023-06-29 16:16:46.832595 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/__init__.py
--rw-r--r--   0        0        0     9652 2023-06-30 14:35:43.119450 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/audit_checks.py
--rw-r--r--   0        0        0     2883 2023-06-30 14:12:30.984804 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-06-29 16:16:46.833562 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/es_checks.py
--rw-r--r--   0        0        0      262 2023-06-29 16:16:46.833957 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2023-06-29 16:16:46.834082 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2023-06-29 16:16:46.834353 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2023-06-29 16:16:46.834575 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4019 2023-06-30 14:28:16.941473 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/utils.py
--rw-r--r--   0        0        0    39037 2023-06-30 14:29:26.276042 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2572 2023-06-30 14:12:31.026319 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-06-29 16:16:46.836068 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    22581 2023-06-30 14:40:29.435109 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/system_checks.py
--rw-r--r--   0        0        0    59196 2023-06-30 14:41:50.645088 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/wfr_checks.py
--rw-r--r--   0        0        0    57441 2023-06-30 14:42:15.050104 foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/wrangler_checks.py
--rw-r--r--   0        0        0      773 2023-06-30 14:12:30.981074 foursight_smaht-0.0.0.1b1/chalicelib_smaht/deploy.py
--rw-r--r--   0        0        0      601 2023-06-30 14:23:10.247383 foursight_smaht-0.0.0.1b1/chalicelib_smaht/package.py
--rw-r--r--   0        0        0      253 2023-06-30 16:58:20.012820 foursight_smaht-0.0.0.1b1/chalicelib_smaht/vars.py
--rw-r--r--   0        0        0     1121 2023-06-30 17:27:40.509361 foursight_smaht-0.0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b1/setup.py
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 16:16:46.829708 foursight_smaht-0.0.0.1b2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-29 16:16:46.830680 foursight_smaht-0.0.0.1b2/chalicelib_smaht/__init__.py
+-rw-r--r--   0        0        0     1030 2023-06-30 14:13:49.029298 foursight_smaht-0.0.0.1b2/chalicelib_smaht/app_utils.py
+-rw-r--r--   0        0        0      873 2023-06-30 14:21:01.676349 foursight_smaht-0.0.0.1b2/chalicelib_smaht/buckets.py
+-rw-r--r--   0        0        0     4805 2023-06-29 16:16:46.831422 foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_schedules.py
+-rw-r--r--   0        0        0    13354 2023-06-30 14:22:35.139013 foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-06-29 16:16:46.832258 foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json-local
+-rw-r--r--   0        0        0      249 2023-06-29 16:16:46.832595 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/__init__.py
+-rw-r--r--   0        0        0     9652 2023-06-30 14:35:43.119450 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/audit_checks.py
+-rw-r--r--   0        0        0     2883 2023-06-30 14:12:30.984804 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-06-29 16:16:46.833562 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/es_checks.py
+-rw-r--r--   0        0        0      262 2023-06-29 16:16:46.833957 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2023-06-29 16:16:46.834082 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2023-06-29 16:16:46.834353 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2023-06-29 16:16:46.834575 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4019 2023-06-30 14:28:16.941473 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39037 2023-06-30 14:29:26.276042 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2572 2023-06-30 14:12:31.026319 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-06-29 16:16:46.836068 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    22581 2023-06-30 14:40:29.435109 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/system_checks.py
+-rw-r--r--   0        0        0    59196 2023-06-30 14:41:50.645088 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wfr_checks.py
+-rw-r--r--   0        0        0    57441 2023-06-30 14:42:15.050104 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      773 2023-06-30 14:12:30.981074 foursight_smaht-0.0.0.1b2/chalicelib_smaht/deploy.py
+-rw-r--r--   0        0        0      601 2023-06-30 14:23:10.247383 foursight_smaht-0.0.0.1b2/chalicelib_smaht/package.py
+-rw-r--r--   0        0        0      253 2023-06-30 16:58:20.012820 foursight_smaht-0.0.0.1b2/chalicelib_smaht/vars.py
+-rw-r--r--   0        0        0     1122 2023-06-30 18:28:49.358366 foursight_smaht-0.0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b2/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b2/PKG-INFO
```

### Comparing `foursight_smaht-0.0.0.1b1/LICENSE.txt` & `foursight_smaht-0.0.0.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/app_utils.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/buckets.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/check_schedules.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/check_setup.json` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/check_setup.json-local` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/audit_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/ecs_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/es_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/lifecycle_utils.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/linecount_dicts.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/utils.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/wfr_utils.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/helpers/wfrset_utils.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/lifecycle_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/system_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/wfr_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/checks/wrangler_checks.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/deploy.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/chalicelib_smaht/package.py` & `foursight_smaht-0.0.0.1b2/chalicelib_smaht/package.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b1/pyproject.toml` & `foursight_smaht-0.0.0.1b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-smaht"
-version = "0.0.0.1b1"
+version = "0.0.0.1b2"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_smaht" }
 ]
 
@@ -20,15 +20,15 @@
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 magma-suite = "^1.2.2"
 tibanna-ff = "^1.3.0"
 MarkupSafe = "1.1.1"
-foursight-core = "4.3.0.1b40"
+foursight-core = "^4.3.0.1b46"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 cgap-pipeline-utils = "23.0"
 pytest = "5.1.2"
 
 [tool.poetry.dev-dependencies]
 chalice = "^1.21.6"
```

### Comparing `foursight_smaht-0.0.0.1b1/setup.py` & `foursight_smaht-0.0.0.1b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,30 @@
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'cgap-pipeline-utils==23.0',
  'click>=7.1.2,<8.0.0',
  'dcicutils>=7.5.1,<8.0.0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.3.0.1b40',
+ 'foursight-core>=4.3.0.1b46,<5.0.0.0',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.12.5,<2.0.0',
  'magma-suite>=1.2.2,<2.0.0',
  'pytest==5.1.2',
  'pytz>=2020.1,<2021.0',
  'tibanna-ff>=1.3.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-smaht',
-    'version': '0.0.0.1b1',
+    'version': '0.0.0.1b2',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_smaht-0.0.0.1b1/PKG-INFO` & `foursight_smaht-0.0.0.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-smaht
-Version: 0.0.0.1b1
+Version: 0.0.0.1b2
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: cgap-pipeline-utils (==23.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: dcicutils (>=7.5.1,<8.0.0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.3.0.1b40)
+Requires-Dist: foursight-core (>=4.3.0.1b46,<5.0.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: magma-suite (>=1.2.2,<2.0.0)
 Requires-Dist: pytest (==5.1.2)
 Requires-Dist: pytz (>=2020.1,<2021.0)
 Requires-Dist: tibanna-ff (>=1.3.0,<2.0.0)
```

