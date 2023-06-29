# Comparing `tmp/aiotus-0.1.8.tar.gz` & `tmp/aiotus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiotus-0.1.8.tar", last modified: Tue Oct 13 21:15:12 2020, max compression
+gzip compressed data, was "dist/aiotus-0.1.9.tar", last modified: Sun Jul 11 09:15:36 2021, max compression
```

## Comparing `aiotus-0.1.8.tar` & `aiotus-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)      124 2020-10-13 21:15:03.000000 aiotus-0.1.8/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (116)      138 2020-10-13 21:15:03.000000 aiotus-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2387 2020-10-13 21:15:03.000000 aiotus-0.1.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (116)      758 2020-10-13 21:15:03.000000 aiotus-0.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      154 2020-10-13 21:15:03.000000 aiotus-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      118 2020-10-13 21:15:03.000000 aiotus-0.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-10-13 21:15:03.000000 aiotus-0.1.8/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (116)    10174 2020-10-13 21:15:03.000000 aiotus-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2020-10-13 21:15:03.000000 aiotus-0.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     4830 2020-10-13 21:15:12.000000 aiotus-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3284 2020-10-13 21:15:03.000000 aiotus-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus/
--rw-r--r--   0 runner    (1001) docker     (116)      340 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     8593 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     2794 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/creation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2761 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (116)       53 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/log.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)    11905 2020-10-13 21:15:03.000000 aiotus-0.1.8/aiotus/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4830 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      877 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      119 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-10-13 21:15:12.000000 aiotus-0.1.8/aiotus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      591 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      799 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (116)       63 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (116)      270 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/source/aiotus.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       98 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/source/entrypoint.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3507 2020-10-13 21:15:03.000000 aiotus-0.1.8/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)       31 2020-10-13 21:15:03.000000 aiotus-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      327 2020-10-13 21:15:03.000000 aiotus-0.1.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      283 2020-10-13 21:15:12.000000 aiotus-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1441 2020-10-13 21:15:03.000000 aiotus-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-13 21:15:12.000000 aiotus-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     7665 2020-10-13 21:15:03.000000 aiotus-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)    13192 2020-10-13 21:15:03.000000 aiotus-0.1.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (116)     3006 2020-10-13 21:15:03.000000 aiotus-0.1.8/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2624 2020-10-13 21:15:03.000000 aiotus-0.1.8/tests/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (116)    11057 2020-10-13 21:15:03.000000 aiotus-0.1.8/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (116)     2955 2020-10-13 21:15:03.000000 aiotus-0.1.8/tests/test_tls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-07-11 09:15:28.000000 aiotus-0.1.9/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-07-11 09:15:28.000000 aiotus-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2387 2021-07-11 09:15:28.000000 aiotus-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2021-07-11 09:15:28.000000 aiotus-0.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2021-07-11 09:15:28.000000 aiotus-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-07-11 09:15:28.000000 aiotus-0.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-07-11 09:15:28.000000 aiotus-0.1.9/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (121)    10174 2021-07-11 09:15:28.000000 aiotus-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2021-07-11 09:15:28.000000 aiotus-0.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     4830 2021-07-11 09:15:36.000000 aiotus-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3284 2021-07-11 09:15:28.000000 aiotus-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/aiotus/
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9025 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2948 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2761 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    12591 2021-07-11 09:15:28.000000 aiotus-0.1.9/aiotus/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/aiotus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4830 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-11 09:15:35.000000 aiotus-0.1.9/aiotus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/source/aiotus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/source/entrypoint.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3507 2021-07-11 09:15:28.000000 aiotus-0.1.9/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-11 09:15:28.000000 aiotus-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2021-07-11 09:15:28.000000 aiotus-0.1.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2021-07-11 09:15:36.000000 aiotus-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-07-11 09:15:28.000000 aiotus-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-11 09:15:36.000000 aiotus-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     7665 2021-07-11 09:15:28.000000 aiotus-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13200 2021-07-11 09:15:28.000000 aiotus-0.1.9/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-07-11 09:15:28.000000 aiotus-0.1.9/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2840 2021-07-11 09:15:28.000000 aiotus-0.1.9/tests/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11209 2021-07-11 09:15:28.000000 aiotus-0.1.9/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2948 2021-07-11 09:15:28.000000 aiotus-0.1.9/tests/test_tls.py
```

### Comparing `aiotus-0.1.8/.github/workflows/ci.yml` & `aiotus-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/.github/workflows/release.yml` & `aiotus-0.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/LICENSE.txt` & `aiotus-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/Makefile` & `aiotus-0.1.9/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -66,18 +66,25 @@
 	tar -xf ${TUSD_ARCHIVE} --strip-components 1 tusd_linux_${TUSD_ARCH}/tusd
 	touch $@
 
 tests/nginx.key tests/selfsigned.crt:
 	openssl req \
 	    -new -x509 -nodes\
 	    -days 3650 \
-	    -subj '/CN=localhost' \
+	    -subj '/' \
+	    -addext 'subjectAltName = DNS:localhost' \
 	    -keyout tests/nginx.key \
 	    -out tests/selfsigned.crt
 
+show-certificate: tests/selfsigned.crt
+	@openssl x509 \
+	    -text \
+	    -in $< \
+	    -noout
+
 clean:
 	@rm -f \
 	    .coverage
 	@rm -rf \
 	    .mypy_cache \
 	    .pytest_cache \
 	    .xprocess \
@@ -98,9 +105,10 @@
 .PHONY: \
 	black \
 	clean \
 	doc \
 	flake8-check \
 	isort-check \
 	mypy-check \
+	show-certificate \
 	test \
 	veryclean
```

### Comparing `aiotus-0.1.8/PKG-INFO` & `aiotus-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asynchronous tus (tus.io) client library
 Home-page: https://github.com/JenSte/aiotus
 Author: Jens Steinhauser
 Author-email: jens.steinhauser@gmail.com
 License: Apache 2
 Project-URL: Documentation, https://aiotus.readthedocs.io
 Description: <h1 align="center">aiotus - Asynchronous tus client library</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiotus Version: 0.1.8 Summary: Asynchronous tus
+Metadata-Version: 2.1 Name: aiotus Version: 0.1.9 Summary: Asynchronous tus
 (tus.io) client library Home-page: https://github.com/JenSte/aiotus Author:
 Jens Steinhauser Author-email: jens.steinhauser@gmail.com License: Apache 2
 Project-URL: Documentation, https://aiotus.readthedocs.io Description:
             ****** aiotus - Asynchronous tus client library ******
   [License:_Apache_2.0] [Python_Versions] [Mypy_Checked] [Code_Style:_black]
 [CI_Status] [Code_Coverage] [Quality_Gate] [Documentation_Status] [PyPI_Package
                                    Version]
```

### Comparing `aiotus-0.1.8/README.md` & `aiotus-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/aiotus/common.py` & `aiotus-0.1.9/aiotus/common.py`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/aiotus/core.py` & `aiotus-0.1.9/aiotus/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,25 +71,26 @@
     """Get the number of uploaded bytes.
 
     :param session: HTTP session to use for connections.
     :param location: The upload endpoint to query.
     :param ssl: SSL validation mode, passed on to aiohttp.
     :param headers: Optional headers used in the request.
     :return: The number of bytes that are already on the server.
+    :raises ProtocolError: When the server does not comply to the tus protocol.
     """
 
     tus_headers = dict(headers or {})
     tus_headers["Tus-Resumable"] = common.TUS_PROTOCOL_VERSION
 
     logger.debug(f'Getting offset of "{location}"...')
     async with await session.head(location, headers=tus_headers, ssl=ssl) as response:
         response.raise_for_status()
 
         if "Upload-Offset" not in response.headers:
-            raise RuntimeError(
+            raise common.ProtocolError(
                 f"HEAD request succeeded for {location}, "
                 'but no "Upload-Offset" header in response.'
             )
 
         return _parse_positive_integer_header(response.headers, "Upload-Offset")
 
 
@@ -122,14 +123,17 @@
     """Get the metadata associated with an upload.
 
     :param session: HTTP session to use for connections.
     :param location: The upload endpoint to query.
     :param ssl: SSL validation mode, passed on to aiohttp.
     :param headers: Optional headers used in the request.
     :return: The metadata of the upload.
+    :raises ProtocolError: When the server does not comply to the tus protocol.
+
+    .. # noqa: DAR401 asyncio.CancelledError
     """
 
     tus_headers = dict(headers or {})
     tus_headers["Tus-Resumable"] = common.TUS_PROTOCOL_VERSION
 
     logger.debug(f'Getting metadata of "{location}"...')
     async with await session.head(location, headers=tus_headers, ssl=ssl) as response:
@@ -158,14 +162,16 @@
 
     :param session: HTTP session to use for connections.
     :param location: The endpoint to upload to.
     :param buffer: The data to upload.
     :param ssl: SSL validation mode, passed on to aiohttp.
     :param chunksize: The size of individual chunks to upload at a time.
     :param headers: Optional headers used in the request.
+    :raises ProtocolError: When the server does not comply to the tus protocol.
+    :raises RuntimeError: When reading of the file fails.
     """
 
     loop = asyncio.get_event_loop()
 
     total_size = await loop.run_in_executor(None, buffer.seek, 0, io.SEEK_END)
 
     # The position in the file where we currently read from.
@@ -235,14 +241,15 @@
     """Get the server's configuration.
 
     :param session: HTTP session to use for connections.
     :param url: The creation endpoint of the server.
     :param ssl: SSL validation mode, passed on to aiohttp.
     :param headers: Optional headers used in the request.
     :return: An object describing the server's configuration.
+    :raises ProtocolError: When the server does not comply to the tus protocol.
     """
 
     logger.debug("Querying server configuration...")
     async with await session.options(url, headers=headers, ssl=ssl) as response:
         response.raise_for_status()
 
         if "Tus-Version" not in response.headers:
```

### Comparing `aiotus-0.1.8/aiotus/creation.py` & `aiotus-0.1.9/aiotus/creation.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     :param file: The file object to upload.
         Used to determine the length of data to be uploaded. If not given, the
         corresponding HTTP header is not included in the request.
     :param metadata: Additional metadata for the upload.
     :param ssl: SSL validation mode, passed on to aiohttp.
     :param headers: Optional headers used in the request.
     :return: The URL to upload the data to.
+    :raises ProtocolError: When the server does not comply to the tus protocol.
     """
 
     tus_headers = dict(headers or {})
     tus_headers["Tus-Resumable"] = common.TUS_PROTOCOL_VERSION
 
     if file is not None:
         loop = asyncio.get_event_loop()
@@ -74,16 +75,19 @@
             return " " + encoded_string
 
         pairs = [f"{k}{encode_value(v)}" for k, v in metadata.items()]
         tus_headers["Upload-Metadata"] = ",".join(pairs)
 
     logger.debug("Creating upload...")
     async with await session.post(url, headers=tus_headers, ssl=ssl) as response:
+        response.raise_for_status()
         if response.status != 201:
             raise common.ProtocolError(
                 f"Wrong status code {response.status}, expected 201."
             )
 
         if "Location" not in response.headers:
-            raise RuntimeError('Upload created, but no "Location" header in response.')
+            raise common.ProtocolError(
+                'Upload created, but no "Location" header in response.'
+            )
 
         return yarl.URL(response.headers["Location"])
```

### Comparing `aiotus-0.1.8/aiotus/entrypoint.py` & `aiotus-0.1.9/aiotus/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/aiotus/retry.py` & `aiotus-0.1.9/aiotus/retry.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
 import aiohttp
-import tenacity  # type: ignore
+import tenacity
 import yarl
 
 from . import common, core, creation
 from .log import logger
 
 T = TypeVar("T")
 
@@ -102,21 +102,25 @@
                 f"{s.capitalize()} failed, "
                 f"retrying in {duration:.0f} second(s): {value}"
             )
 
     return log
 
 
-def _make_retrying(s: str, config: RetryConfiguration) -> tenacity.AsyncRetrying:
+def _make_retrying(
+    s: str, config: RetryConfiguration
+) -> tenacity.AsyncRetrying:  # type: ignore
     """Create a tenacity retry object."""
 
-    return tenacity.AsyncRetrying(
-        retry=tenacity.retry_if_exception_type(aiohttp.ClientError),
-        stop=tenacity.stop_after_attempt(config.retry_attempts),
-        wait=tenacity.wait_exponential(max=config.max_retry_period_seconds),
+    return tenacity.AsyncRetrying(  # type: ignore
+        retry=tenacity.retry_if_exception_type(aiohttp.ClientError),  # type: ignore
+        stop=tenacity.stop_after_attempt(config.retry_attempts),  # type: ignore
+        wait=tenacity.wait_exponential(  # type: ignore
+            max=config.max_retry_period_seconds
+        ),
         before=_make_log_before_function(s),
         before_sleep=_make_log_before_sleep_function(s),
     )
 
 
 async def upload(
     endpoint: Union[str, yarl.URL],
@@ -138,14 +142,16 @@
     :param file: The file to upload.
     :param metadata: Additional metadata for the upload.
     :param client_session: An aiohttp ClientSession to use.
     :param config: Settings to customize the retry behaviour.
     :param headers: Optional headers used in the request.
     :param chunksize: The size of individual chunks to upload at a time.
     :return: The location where the file was uploaded to (if the upload succeeded).
+
+    .. # noqa: DAR401 asyncio.CancelledError
     """
 
     url = yarl.URL(endpoint)
 
     if metadata is None:
         metadata = {}
 
@@ -156,36 +162,38 @@
         ctx: Union[aiohttp.ClientSession, AsyncContextManager[aiohttp.ClientSession]]
         if client_session is None:
             ctx = aiohttp.ClientSession()
         else:
             ctx = asyncnullcontext(client_session)
 
         async with ctx as session:
-            location: yarl.URL
-            location = await retrying_create.call(
-                creation.create,
-                session,
-                url,
-                file,
-                metadata,
-                ssl=config.ssl,
-                headers=headers,
-            )
+            async for attempt in retrying_create:
+                with attempt:
+                    location = await creation.create(
+                        session,
+                        url,
+                        file,
+                        metadata,
+                        ssl=config.ssl,
+                        headers=headers,
+                    )
+
             if not location.is_absolute():
                 location = url / location.path
 
-            await retrying_upload_file.call(
-                core.upload_buffer,
-                session,
-                location,
-                file,
-                ssl=config.ssl,
-                chunksize=chunksize,
-                headers=headers,
-            )
+            async for attempt in retrying_upload_file:
+                with attempt:
+                    await core.upload_buffer(
+                        session,
+                        location,
+                        file,
+                        ssl=config.ssl,
+                        chunksize=chunksize,
+                        headers=headers,
+                    )
 
             return location
     except asyncio.CancelledError:  # pragma: no cover
         raise
     except tenacity.RetryError as e:
         logger.error(
             f"Unable to upload file, even after retrying: {e.last_attempt.exception()}"
@@ -207,14 +215,16 @@
     In case of a communication error, this function retries.
 
     :param endpoint: The location of the upload.
     :param client_session: An aiohttp ClientSession to use.
     :param config: Settings to customize the retry behaviour.
     :param headers: Optional headers used in the request.
     :return: The metadata associated with the upload.
+
+    .. # noqa: DAR401 asyncio.CancelledError
     """
 
     if isinstance(endpoint, str):
         url = yarl.URL(endpoint)
     else:
         url = endpoint
 
@@ -225,19 +235,19 @@
         if client_session is None:
             ctx = aiohttp.ClientSession()
         else:
             ctx = asyncnullcontext(client_session)
 
         async with ctx as session:
             md: common.Metadata
-            md = await retrying_metadata.call(
-                core.metadata, session, url, ssl=config.ssl, headers=headers
-            )
-
-            return md
+            async for attempt in retrying_metadata:
+                with attempt:
+                    return await core.metadata(
+                        session, url, ssl=config.ssl, headers=headers
+                    )
     except asyncio.CancelledError:  # pragma: no cover
         raise
     except tenacity.RetryError as e:
         logger.error(
             f"Unable to get metadata, even after retrying: {e.last_attempt.exception()}"
         )
 
@@ -285,16 +295,19 @@
     :param endpoint: The creation endpoint of the server.
     :param files: The files to upload.
     :param metadata: Additional metadata for the final upload.
     :param client_session: An aiohttp ClientSession to use.
     :param config: Settings to customize the retry behaviour.
     :param headers: Optional headers used in the request.
     :param chunksize: The size of individual chunks to upload at a time.
-    :param parallel_upload: The number of parallel uploads to do concurrently.
+    :param parallel_uploads: The number of parallel uploads to do concurrently.
     :return: The location of the final (concatenated) file on the server.
+    :raises RuntimeError: If the server does not support the "concatenation" extension.
+
+    .. # noqa: DAR401 asyncio.CancelledError
     """
 
     url = yarl.URL(endpoint)
 
     if metadata is None:
         metadata = {}
 
@@ -308,17 +321,19 @@
         else:
             ctx = asyncnullcontext(client_session)
 
         async with ctx as session:
             #
             # Check if the server supports the "concatenation" extension.
             #
-            server_config = await retrying_config.call(
-                core.configuration, session, url, ssl=config.ssl, headers=headers
-            )
+            async for attempt in retrying_config:
+                with attempt:
+                    server_config = await core.configuration(
+                        session, url, ssl=config.ssl, headers=headers
+                    )
 
             if "concatenation" not in server_config.protocol_extensions:
                 raise RuntimeError(
                     'Server does not support the "concatenation" extension.'
                 )
 
             #
@@ -352,26 +367,24 @@
 
             #
             # Do the final concatenation.
             #
             final_headers = dict(headers or {})
             final_headers.update({"Upload-Concat": concat_header})
 
-            location: yarl.URL
-            location = await retrying_create.call(
-                creation.create,
-                session,
-                url,
-                None,
-                metadata,
-                ssl=config.ssl,
-                headers=final_headers,
-            )
-
-            return location
+            async for attempt in retrying_create:
+                with attempt:
+                    return await creation.create(
+                        session,
+                        url,
+                        None,
+                        metadata,
+                        ssl=config.ssl,
+                        headers=final_headers,
+                    )
     except asyncio.CancelledError:  # pragma: no cover
         raise
     except tenacity.RetryError as e:
         logger.error(
             f"Unable to upload files, even after retrying: {e.last_attempt.exception()}"
         )
     except Exception as e:
```

### Comparing `aiotus-0.1.8/aiotus.egg-info/PKG-INFO` & `aiotus-0.1.9/aiotus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asynchronous tus (tus.io) client library
 Home-page: https://github.com/JenSte/aiotus
 Author: Jens Steinhauser
 Author-email: jens.steinhauser@gmail.com
 License: Apache 2
 Project-URL: Documentation, https://aiotus.readthedocs.io
 Description: <h1 align="center">aiotus - Asynchronous tus client library</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiotus Version: 0.1.8 Summary: Asynchronous tus
+Metadata-Version: 2.1 Name: aiotus Version: 0.1.9 Summary: Asynchronous tus
 (tus.io) client library Home-page: https://github.com/JenSte/aiotus Author:
 Jens Steinhauser Author-email: jens.steinhauser@gmail.com License: Apache 2
 Project-URL: Documentation, https://aiotus.readthedocs.io Description:
             ****** aiotus - Asynchronous tus client library ******
   [License:_Apache_2.0] [Python_Versions] [Mypy_Checked] [Code_Style:_black]
 [CI_Status] [Code_Coverage] [Quality_Gate] [Documentation_Status] [PyPI_Package
                                    Version]
```

### Comparing `aiotus-0.1.8/aiotus.egg-info/SOURCES.txt` & `aiotus-0.1.9/aiotus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/docs/Makefile` & `aiotus-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/docs/make.bat` & `aiotus-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/docs/source/conf.py` & `aiotus-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/docs/source/index.rst` & `aiotus-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/docs/source/usage.rst` & `aiotus-0.1.9/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/setup.py` & `aiotus-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiotus",
-    version="0.1.8",
+    version="0.1.9",
     author="Jens Steinhauser",
     author_email="jens.steinhauser@gmail.com",
     description="Asynchronous tus (tus.io) client library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JenSte/aiotus",
     project_urls={"Documentation": "https://aiotus.readthedocs.io"},
@@ -32,11 +32,11 @@
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP",
         "Typing :: Typed",
     ],
     python_requires=">=3.7",
-    install_requires=["aiohttp", "tenacity"],
+    install_requires=["aiohttp", "tenacity>=6.2.0"],
     setup_requires=["setuptools_scm"],
     use_scm_version={"local_scheme": "dirty-tag"},
 )
```

### Comparing `aiotus-0.1.8/tests/conftest.py` & `aiotus-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiotus-0.1.8/tests/test_core.py` & `aiotus-0.1.9/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         with pytest.raises(aiohttp.ClientResponseError):
             location = server.make_url("/not_found")
 
             async with aiohttp.ClientSession() as session:
                 await aiotus.core.offset(session, location)
 
         # Check if the check for the "Upload-Offset" header is working.
-        with pytest.raises(RuntimeError) as excinfo:
+        with pytest.raises(aiotus.ProtocolError) as excinfo:
             location = server.make_url("/no_offset")
 
             async with aiohttp.ClientSession() as session:
                 await aiotus.core.offset(session, location)
 
         assert 'no "Upload-Offset" header' in str(excinfo.value)
```

### Comparing `aiotus-0.1.8/tests/test_creation.py` & `aiotus-0.1.9/tests/test_creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,40 +27,48 @@
             await aiotus.creation.create(None, None, memory_file, metadata)
 
         assert "commas" in str(excinfo.value)
 
     async def test_create_wrong_status(self, aiohttp_server, memory_file):
         """Check if status code is checked correctly."""
 
-        async def handler_wrong_status(request):
-            raise aiohttp.web.HTTPBadRequest()
+        async def handler_status_200(request):
+            return aiohttp.web.Response(status=200)
+
+        async def handler_status_400(request):
+            return aiohttp.web.Response(status=400)
 
         app = aiohttp.web.Application()
-        app.router.add_route("POST", "/wrong_status", handler_wrong_status)
+        app.router.add_route("POST", "/status_200", handler_status_200)
+        app.router.add_route("POST", "/status_400", handler_status_400)
         server = await aiohttp_server(app)
 
         with pytest.raises(aiotus.ProtocolError) as excinfo:
-            endpoint = server.make_url("/wrong_status")
-
+            endpoint = server.make_url("/status_200")
             async with aiohttp.ClientSession() as session:
                 await aiotus.creation.create(session, endpoint, memory_file, {})
-
         assert "Wrong status code" in str(excinfo.value)
 
+        with pytest.raises(aiohttp.ClientResponseError) as excinfo:
+            endpoint = server.make_url("/status_400")
+            async with aiohttp.ClientSession() as session:
+                await aiotus.creation.create(session, endpoint, memory_file, {})
+        assert excinfo.value.status == 400
+
     async def test_create_no_location(self, aiohttp_server, memory_file):
         """Check if the check for the "Location" header is working."""
 
         async def handler_no_location(request):
             raise aiohttp.web.HTTPCreated()
 
         app = aiohttp.web.Application()
         app.router.add_route("POST", "/no_location", handler_no_location)
         server = await aiohttp_server(app)
 
-        with pytest.raises(RuntimeError) as excinfo:
+        with pytest.raises(aiotus.ProtocolError) as excinfo:
             endpoint = server.make_url("/no_location")
 
             async with aiohttp.ClientSession() as session:
                 await aiotus.creation.create(session, endpoint, memory_file, {})
 
         assert 'no "Location" header' in str(excinfo.value)
```

### Comparing `aiotus-0.1.8/tests/test_entrypoint.py` & `aiotus-0.1.9/tests/test_entrypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 import unittest.mock
 
 import aiotus.entrypoint
 
 
 class TestAiotusClients:
     def test_aiotus_clients(self, tusd):
-        with unittest.mock.patch(
-            "sys.argv", ["aiotus-upload", "--debug", str(tusd.url) + "x", __file__]
-        ):
-            assert 1 == aiotus.entrypoint.aiotus_upload()
+        conf = aiotus.RetryConfiguration(1, 0.001, None)
+        defaults = (None, None, conf, None, 4 * 1024 * 1024)
+        with unittest.mock.patch.object(aiotus.upload, "__defaults__", defaults):
+            with unittest.mock.patch(
+                "sys.argv", ["aiotus-upload", "--debug", str(tusd.url) + "x", __file__]
+            ):
+                assert 1 == aiotus.entrypoint.aiotus_upload()
 
         with unittest.mock.patch(
             "sys.argv", ["aiotus-upload", str(tusd.url), __file__ + "x"]
         ):
             assert 1 == aiotus.entrypoint.aiotus_upload()
 
         with unittest.mock.patch(
```

### Comparing `aiotus-0.1.8/tests/test_retry.py` & `aiotus-0.1.9/tests/test_retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,17 @@
             stop=tenacity.stop_after_attempt(3),
             before=aiotus.retry._make_log_before_function("test"),
             before_sleep=aiotus.retry._make_log_before_sleep_function("test"),
         )
 
         with caplog.at_level(logging.INFO, logger="aiotus"):
             with pytest.raises(tenacity.RetryError):
-                await rt.call(TestTenacity.raise_runtime_error)
+                async for attempt in rt:
+                    with attempt:
+                        await TestTenacity.raise_runtime_error()
 
             lg = caplog.record_tuples
             assert len(lg) == 4
             assert lg[0][2] == "Test failed, retrying in 0 second(s): test error"
             assert lg[1][2] == "Trying test again, attempt number 2..."
             assert lg[2][2] == "Test failed, retrying in 0 second(s): test error"
             assert lg[3][2] == "Trying test again, attempt number 3..."
@@ -291,15 +293,17 @@
             stop=tenacity.stop_after_attempt(2),
             before=aiotus.retry._make_log_before_function("test"),
             before_sleep=aiotus.retry._make_log_before_sleep_function("test"),
         )
 
         with caplog.at_level(logging.INFO, logger="aiotus"):
             with pytest.raises(tenacity.RetryError):
-                await rt.call(TestTenacity.return_none)
+                async for attempt in rt:
+                    with attempt:
+                        await TestTenacity.return_none()
 
             lg = caplog.record_tuples
             assert len(lg) == 2
             assert lg[0][2] == "Test failed, retrying in 0 second(s): None"
             assert lg[1][2] == "Trying test again, attempt number 2..."
 
     @staticmethod
```

### Comparing `aiotus-0.1.8/tests/test_tls.py` & `aiotus-0.1.9/tests/test_tls.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 class TestTLS:
     async def test_upload_fail(self, nginx_proxy, memory_file):
         """Test failed upload to a TLS server."""
 
         # Make sure we actually use encryption, access via plain
         # HTTP shall fail.
         async with aiohttp.ClientSession() as session:
-            with pytest.raises(aiotus.ProtocolError) as excinfo:
+            with pytest.raises(aiohttp.ClientResponseError) as excinfo:
                 http_url = nginx_proxy.url.with_scheme("http")
                 await aiotus.creation.create(session, http_url, memory_file, {})
-            assert "Wrong status code" in str(excinfo.value)
+            assert excinfo.value.status == 400
 
         # As we use a self-signed certificate, the connection will fail.
         async with aiohttp.ClientSession() as session:
             with pytest.raises(aiohttp.ClientConnectorCertificateError) as excinfo:
                 await aiotus.creation.create(session, nginx_proxy.url, memory_file, {})
             assert "certificate verify failed: self signed certificate" in str(
                 excinfo.value
```

