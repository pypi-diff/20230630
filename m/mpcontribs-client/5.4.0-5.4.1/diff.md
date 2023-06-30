# Comparing `tmp/mpcontribs-client-5.4.0.tar.gz` & `tmp/mpcontribs-client-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.4.0.tar", last modified: Fri Jun 23 01:21:03 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.4.1.tar", last modified: Fri Jun 30 18:13:28 2023, max compression
```

## Comparing `mpcontribs-client-5.4.0.tar` & `mpcontribs-client-5.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.384965 mpcontribs-client-5.4.0/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.384965 mpcontribs-client-5.4.0/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    87013 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.384965 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 01:21:03.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.856181 mpcontribs-client-5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 18:13:28.856181 mpcontribs-client-5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    87020 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:13:28.000000 mpcontribs-client-5.4.1/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:13:28.856181 mpcontribs-client-5.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:13:28.852181 mpcontribs-client-5.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 18:13:17.000000 mpcontribs-client-5.4.1/tests/test_client.py
```

### Comparing `mpcontribs-client-5.4.0/LICENSE` & `mpcontribs-client-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.0/PKG-INFO` & `mpcontribs-client-5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.4.0
+Version: 5.4.1
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.4.0/README.md` & `mpcontribs-client-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.0/mpcontribs/client/__init__.py` & `mpcontribs-client-5.4.1/mpcontribs/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
             major=now.year, minor=now.month, patch=now.day,
             prerelease=(str(now.hour), str(now.minute))
         )
     else:
         while retries < max_retries:
             try:
                 r = requests.get(f"{url}/healthcheck", timeout=5)
-                if r.status_code == 200:
+                if r.status_code in {200, 403}:
                     return r.json().get("version")
                 else:
                     retries += 1
                     logger.warning(
                         f"Healthcheck for {url} failed ({r.status_code})! Wait 30s."
                     )
                     time.sleep(30)
```

### Comparing `mpcontribs-client-5.4.0/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.4.1/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.4.0
+Version: 5.4.1
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.4.0/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.4.1/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.0/requirements/deployment.txt` & `mpcontribs-client-5.4.1/requirements/deployment.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=MPContribs/mpcontribs-client/requirements/deployment.txt --resolver=backtracking MPContribs/mpcontribs-client/setup.py python/requirements.txt
 #
+annotated-types==0.5.0
+    # via pydantic
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -28,26 +30,28 @@
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.57.2
+emmet-core==0.58.0
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 ipython==8.14.0
@@ -105,15 +109,15 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==1.5.3
     # via
     #   -r python/requirements.txt
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
@@ -134,21 +138,23 @@
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.9
+pydantic==2.0
     # via emmet-core
+pydantic-core==2.0.1
+    # via pydantic
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 pyparsing==3.1.0
@@ -185,15 +191,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via
     #   -r python/requirements.txt
     #   pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 simplejson==3.19.1
     # via
@@ -229,23 +235,22 @@
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   pydantic-core
     #   swagger-spec-validator
-tzdata==2023.3
-    # via pandas
 ujson==5.8.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 uncertainties==3.1.7
     # via pymatgen
 uri-template==1.3.0
     # via jsonschema
 urllib3==2.0.3
```

### Comparing `mpcontribs-client-5.4.0/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.4.1/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 ipython==8.14.0
@@ -104,15 +106,15 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -138,15 +140,15 @@
     #   pymatgen
 pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
@@ -183,15 +185,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -225,15 +227,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.4.0/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.1/requirements/macos-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
@@ -50,23 +50,29 @@
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipython==8.14.0
+ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
@@ -102,43 +108,45 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
@@ -163,26 +171,26 @@
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
@@ -266,18 +274,19 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
+    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
@@ -287,10 +296,12 @@
     # via jsonschema
 urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
+zipp==3.15.0
+    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.0/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -42,14 +40,16 @@
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
@@ -94,29 +94,29 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -144,15 +144,15 @@
     #   pymatgen
 pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
@@ -231,15 +231,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.1/requirements/macos-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
@@ -50,27 +50,27 @@
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipython==8.12.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
@@ -106,45 +106,43 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
@@ -169,26 +167,26 @@
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
@@ -226,15 +224,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -272,15 +270,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.4.1/requirements/macos-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
@@ -106,15 +108,15 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -140,15 +142,15 @@
     #   pymatgen
 pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
@@ -185,15 +187,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -227,15 +229,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -50,14 +48,16 @@
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
@@ -119,15 +119,15 @@
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -165,26 +165,26 @@
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
@@ -222,15 +222,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -268,15 +268,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 ipython==8.14.0
@@ -102,15 +104,15 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -136,15 +138,15 @@
     #   pymatgen
 pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
@@ -181,15 +183,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -223,15 +225,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 iniconfig==2.0.0
@@ -115,15 +117,15 @@
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -161,26 +163,26 @@
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
@@ -218,15 +220,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -264,15 +266,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
```

### Comparing `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
@@ -40,25 +40,25 @@
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
-ipython==8.12.2
+    # via matplotlib
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
@@ -92,44 +92,42 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
@@ -142,15 +140,15 @@
     #   pymatgen
 pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
@@ -187,15 +185,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -229,15 +227,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.1/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
@@ -104,30 +106,30 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -167,26 +169,26 @@
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
@@ -270,15 +272,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.4.1/requirements/macos-latest_py3.8.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -40,23 +42,27 @@
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via matplotlib
-ipython==8.14.0
+    # via
+    #   jsonschema
+    #   matplotlib
+ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
@@ -90,42 +96,44 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.25.0
+numpy==1.24.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
@@ -138,15 +146,15 @@
     #   pymatgen
 pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
@@ -225,15 +233,15 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
```

### Comparing `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.1/requirements/macos-latest_py3.10_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -48,22 +50,22 @@
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
 fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
+frozendict==2.3.8
+    # via pymatgen
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
 ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
@@ -117,15 +119,15 @@
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.2
+pandas==2.0.3
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -163,26 +165,26 @@
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.31
+pymatgen==2023.6.28
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
 pymongo==4.4.0
     # via mpcontribs-client (setup.py)
 pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
 pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
@@ -220,15 +222,15 @@
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
 ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
-scipy==1.10.1
+scipy==1.11.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
 simplejson==3.19.1
     # via
     #   bravado
     #   bravado-core
@@ -266,19 +268,18 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.3
+typing-extensions==4.7.0
     # via
     #   bravado
     #   emmet-core
-    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
 ujson==5.8.0
     # via mpcontribs-client (setup.py)
@@ -288,12 +289,10 @@
     # via jsonschema
 urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
-    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.4.0/setup.py` & `mpcontribs-client-5.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.4.0/tests/test_client.py` & `mpcontribs-client-5.4.1/tests/test_client.py`

 * *Files identical despite different names*

