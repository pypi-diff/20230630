# Comparing `tmp/delphai_fastapi-0.1.7.tar.gz` & `tmp/delphai_fastapi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-0.1.7.tar", max compression
+gzip compressed data, was "delphai_fastapi-0.1.8.tar", max compression
```

## Comparing `delphai_fastapi-0.1.7.tar` & `delphai_fastapi-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/app.py
--rw-r--r--   0        0        0     3173 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     3584 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/job_posts/__init__.py
--rw-r--r--   0        0        0      912 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/job_posts/models.py
--rw-r--r--   0        0        0     1808 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/models.py
--rw-r--r--   0        0        0        0 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/news_articles/__init__.py
--rw-r--r--   0        0        0     1115 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/news_articles/models.py
--rw-r--r--   0        0        0     1342 2023-06-30 09:04:42.315786 delphai_fastapi-0.1.7/delphai_fastapi/types.py
--rw-r--r--   0        0        0      468 2023-06-30 09:05:18.526642 delphai_fastapi-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.7/setup.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2521 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     3822 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     3584 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/job_posts/__init__.py
+-rw-r--r--   0        0        0      912 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/job_posts/models.py
+-rw-r--r--   0        0        0     1808 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/models.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/news_articles/__init__.py
+-rw-r--r--   0        0        0     1135 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/news_articles/models.py
+-rw-r--r--   0        0        0     1342 2023-06-30 10:59:54.322178 delphai_fastapi-0.1.8/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      446 2023-06-30 11:00:23.394258 delphai_fastapi-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.8/setup.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 delphai_fastapi-0.1.8/PKG-INFO
```

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/app.py` & `delphai_fastapi-0.1.8/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/auth.py` & `delphai_fastapi-0.1.8/delphai_fastapi/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import httpx
 import logging
 
 from typing import Annotated, Any, Optional
 
-from delphai_utils.keycloak import decode_token
 from fastapi import Depends, HTTPException, Request, status
 from fastapi.security import OAuth2AuthorizationCodeBearer
-from jose import JOSEError
+from jose import JOSEError, jwt
 
 from .decorators import returns_errors
 
 
 TokenPayload = Optional[dict[str, Any]]
 
 logger = logging.getLogger(__file__)
@@ -117,7 +117,34 @@
         return self._roles
 
     @property
     def is_api_client(self):
         return self._request.url.hostname.lower().startswith("api.delphai") and (
             "api" in self.roles
         )
+
+
+trusted_public_keys = {}
+
+
+async def decode_token(access_token: str) -> str:
+    if not trusted_public_keys:
+        await _async_fetch_keys()
+
+    decode_args = {"audience": "delphai-gateway", "options": {"leeway": 10}}
+
+    try:
+        return jwt.decode(access_token, trusted_public_keys, **decode_args)
+    except JOSEError:
+        await _async_fetch_keys()
+        return jwt.decode(access_token, trusted_public_keys, **decode_args)
+
+
+http_client = httpx.AsyncClient()
+
+
+async def _async_fetch_keys():
+    global trusted_public_keys
+
+    response = await http_client.get(f"{AUTH_BASE_URL}/certs")
+    response.raise_for_status()
+    trusted_public_keys = response.json()
```

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/companies/models.py` & `delphai_fastapi-0.1.8/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/job_posts/models.py` & `delphai_fastapi-0.1.8/delphai_fastapi/job_posts/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/models.py` & `delphai_fastapi-0.1.8/delphai_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/news_articles/models.py` & `delphai_fastapi-0.1.8/delphai_fastapi/news_articles/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 from enum import Enum
 from fastapi_camelcase import CamelModel
 from pydantic import Field
 from typing import List, Optional
 
-from ..types import Label, ObjectId
+from ..models import Label
+from ..types import ObjectId
 
 
 class NewsArticleType(str, Enum):
     NEWS = "news"
     PRESS_RELEASE = "press release"
```

### Comparing `delphai_fastapi-0.1.7/delphai_fastapi/types.py` & `delphai_fastapi-0.1.8/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-0.1.7/setup.py` & `delphai_fastapi-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,23 @@
  'delphai_fastapi.job_posts',
  'delphai_fastapi.news_articles']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['delphai-utils[keycloak]>=3,<4',
- 'fastapi-camelcase>=1,<2',
+['fastapi-camelcase>=1,<2',
  'fastapi>=0,<1',
- 'pymongo>=4,<5']
+ 'httpx>=0,<1',
+ 'pymongo>3',
+ 'python-jose>=3.3,<4.0']
 
 setup_kwargs = {
     'name': 'delphai-fastapi',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Package for fastAPI models',
     'long_description': 'None',
     'author': 'Berinike Tech',
     'author_email': 'berinike@delphai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

