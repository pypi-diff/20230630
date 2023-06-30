# Comparing `tmp/wtfutil-1.0.8-py2.py3-none-any.whl.zip` & `tmp/wtfutil-1.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13585 bytes, number of entries: 9
+Zip file size: 13683 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-24 15:22 wtfutil/__init__.py
 -rw-rw-rw-  2.0 fat     2851 b- defN 23-Feb-24 15:22 wtfutil/notifyutil.py
 -rw-rw-rw-  2.0 fat    21949 b- defN 23-Feb-24 15:22 wtfutil/sqlutil.py
--rw-rw-rw-  2.0 fat    17254 b- defN 23-Feb-24 15:23 wtfutil/util.py
--rw-rw-rw-  2.0 fat     1489 b- defN 23-Feb-24 17:14 wtfutil-1.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2171 b- defN 23-Feb-24 17:14 wtfutil-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Feb-24 17:14 wtfutil-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Feb-24 17:14 wtfutil-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      686 b- defN 23-Feb-24 17:14 wtfutil-1.0.8.dist-info/RECORD
-9 files, 46518 bytes uncompressed, 12415 bytes compressed:  73.3%
+-rw-rw-rw-  2.0 fat    17524 b- defN 23-Mar-11 15:07 wtfutil/util.py
+-rw-rw-rw-  2.0 fat     1489 b- defN 23-Mar-11 15:09 wtfutil-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2197 b- defN 23-Mar-11 15:09 wtfutil-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Mar-11 15:09 wtfutil-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-11 15:09 wtfutil-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      686 b- defN 23-Mar-11 15:09 wtfutil-1.0.9.dist-info/RECORD
+9 files, 46814 bytes uncompressed, 12513 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: wtfutil/sqlutil.py
 Comment: 
 
 Filename: wtfutil/util.py
 Comment: 
 
-Filename: wtfutil-1.0.8.dist-info/LICENSE
+Filename: wtfutil-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: wtfutil-1.0.8.dist-info/METADATA
+Filename: wtfutil-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: wtfutil-1.0.8.dist-info/WHEEL
+Filename: wtfutil-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: wtfutil-1.0.8.dist-info/top_level.txt
+Filename: wtfutil-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wtfutil-1.0.8.dist-info/RECORD
+Filename: wtfutil-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wtfutil/util.py

```diff
@@ -14,14 +14,15 @@
 import re
 import ssl
 from io import BytesIO
 from socket import gethostbyname
 from typing import Any
 from urllib.parse import unquote, quote, urljoin
 from urllib.parse import urlparse
+import tldextract
 
 import faker
 import requests
 import urllib3
 from requests_cache import CachedSession
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.ssl_ import create_urllib3_context
@@ -539,7 +540,17 @@
 
 def get_resource(filename):
     resource_path = get_resource_dir(sys._getframe(1).f_code.co_filename) + "/" + filename
     if Path(resource_path).exists():
         return str(Path(resource_path).absolute())
     if Path(filename).expanduser().exists():
         return str(Path(filename).expanduser().absolute())
+
+
+def get_maindomain(subdomain):
+    # get the main domain from subdomain
+    tld = tldextract.extract(subdomain)
+    if tld.suffix != '':
+        domain = f'{tld.domain}.{tld.suffix}'
+    else:
+        domain = tld.domain
+    return domain
```

## Comparing `wtfutil-1.0.8.dist-info/LICENSE` & `wtfutil-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wtfutil-1.0.8.dist-info/METADATA` & `wtfutil-1.0.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtfutil
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python utility.
 Home-page: https://github.com/vicrack
 Author: vicrack
 Author-email: 18179821+ViCrack@users.noreply.github.com
 Platform: any
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
@@ -27,14 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymysql
 Requires-Dist: faker
 Requires-Dist: requests
 Requires-Dist: cacheout
 Requires-Dist: requests-cache
+Requires-Dist: tldextract
 
 
 # wftutil
 
 <a href="https://pypi.python.org/pypi/wtfutil"><img src="https://img.shields.io/pypi/v/wtfutil.svg"></a>
 <a href="https://pypi.python.org/pypi/wtfutil"><img src="https://img.shields.io/pypi/pyversions/wtfutil.svg"></a>
 =================================================================================================================
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wtfutil Version: 1.0.8 Summary: A Python utility.
+Metadata-Version: 2.1 Name: wtfutil Version: 1.0.9 Summary: A Python utility.
 Home-page: https://github.com/vicrack Author: vicrack Author-email:
 18179821+ViCrack@users.noreply.github.com Platform: any Classifier: Topic ::
 Utilities Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: BSD License Classifier: Topic :: Software Development ::
 Libraries Classifier: Development Status :: 5 - Production/Stable Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 2 Classifier: Programming Language :: Python :: 2.6 Classifier: Programming
@@ -11,16 +11,17 @@
 Language :: Python :: 3.5 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pymysql Requires-Dist: faker Requires-Dist: requests Requires-Dist: cacheout
-Requires-Dist: requests-cache # wftutil [https://img.shields.io/pypi/v/
-wtfutil.svg] [https://img.shields.io/pypi/pyversions/wtfutil.svg]
+Requires-Dist: requests-cache Requires-Dist: tldextract # wftutil [https://
+img.shields.io/pypi/v/wtfutil.svg] [https://img.shields.io/pypi/pyversions/
+wtfutil.svg]
 =================================================================================================================
 ## â¤ The Basics A Python utility ## â¤ Installation Of course, the
 recommended installation method is `pipenv
 pipenv.org>`\_:: ```bash pipenv install wtfutil ``` or ```bash pip install
 wtfutil ``` ## â¤ Features ```python from wtfutil import util ``` ```python
 from wtfutil import sqlutil ``` ## â¤ Thank You Thanks for checking this
 library out! I hope you find it useful. Of course, there's always room for
```

## Comparing `wtfutil-1.0.8.dist-info/RECORD` & `wtfutil-1.0.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 wtfutil/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wtfutil/notifyutil.py,sha256=vnNQEMvnF79jl2GP3iqG5nvH63YTOcm9NBHOTOEUs4M,2851
 wtfutil/sqlutil.py,sha256=6Zm5aWt-QJERgmjHXD3eBDLbrYMK2oMb_VlGl-hI6wk,21949
-wtfutil/util.py,sha256=4_WsMYiI2jsjPNwfQ5onj9C5m9FGaH_YsYHsHAZqVec,17254
-wtfutil-1.0.8.dist-info/LICENSE,sha256=jAyLImq7Nv1_BRhL4F3fGyHVp3dub8Cc69D8WtKYcfA,1489
-wtfutil-1.0.8.dist-info/METADATA,sha256=DEBJx49viyVvj44DXKc18ViMRV73TFbeSbNu2sDlaCw,2171
-wtfutil-1.0.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-wtfutil-1.0.8.dist-info/top_level.txt,sha256=9DPfjFjh-xEnAu6akMSTYmQTGcysHkUl4sT90YKqy0Q,8
-wtfutil-1.0.8.dist-info/RECORD,,
+wtfutil/util.py,sha256=dJk1xtN0lau1W8FtJxvkNlauh4hTtWsY30hgcpQNWr0,17524
+wtfutil-1.0.9.dist-info/LICENSE,sha256=jAyLImq7Nv1_BRhL4F3fGyHVp3dub8Cc69D8WtKYcfA,1489
+wtfutil-1.0.9.dist-info/METADATA,sha256=Geq4ND9OiWSO-_yW-wL3jB_B90jzG07OGSwRKLPDZ4Y,2197
+wtfutil-1.0.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+wtfutil-1.0.9.dist-info/top_level.txt,sha256=9DPfjFjh-xEnAu6akMSTYmQTGcysHkUl4sT90YKqy0Q,8
+wtfutil-1.0.9.dist-info/RECORD,,
```

