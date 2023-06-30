# Comparing `tmp/pypdns-2.0.0.tar.gz` & `tmp/pypdns-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdns-2.0.0.tar", max compression
+gzip compressed data, was "pypdns-2.1.0.tar", max compression
```

## Comparing `pypdns-2.0.0.tar` & `pypdns-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1576 2019-12-19 12:24:43.000000 pypdns-2.0.0/LICENSE
--rw-r--r--   0        0        0      486 2020-01-30 12:30:15.365842 pypdns-2.0.0/README.md
--rw-r--r--   0        0        0      134 2020-01-30 12:13:38.068649 pypdns-2.0.0/pypdns/__init__.py
--rw-r--r--   0        0        0    11746 2022-07-14 15:59:51.700603 pypdns-2.0.0/pypdns/api.py
--rw-r--r--   0        0        0      474 2022-07-14 13:38:43.317167 pypdns-2.0.0/pypdns/errors.py
--rw-r--r--   0        0        0        0 2020-01-30 12:16:15.384858 pypdns-2.0.0/pypdns/py.typed
--rw-r--r--   0        0        0     1029 2022-07-14 15:57:19.356550 pypdns-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1177 2022-07-14 16:03:44.107815 pypdns-2.0.0/setup.py
--rw-r--r--   0        0        0     1577 2022-07-14 16:03:44.107987 pypdns-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1576 2019-12-19 12:24:43.000000 pypdns-2.1.0/LICENSE
+-rw-r--r--   0        0        0      486 2020-01-30 12:30:15.365842 pypdns-2.1.0/README.md
+-rw-r--r--   0        0        0      134 2020-01-30 12:13:38.068649 pypdns-2.1.0/pypdns/__init__.py
+-rw-r--r--   0        0        0    11776 2023-06-30 10:14:39.987080 pypdns-2.1.0/pypdns/api.py
+-rw-r--r--   0        0        0      474 2022-07-14 13:38:43.317167 pypdns-2.1.0/pypdns/errors.py
+-rw-r--r--   0        0        0        0 2020-01-30 12:16:15.384858 pypdns-2.1.0/pypdns/py.typed
+-rw-r--r--   0        0        0     1066 2023-06-30 10:13:41.114809 pypdns-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 pypdns-2.1.0/PKG-INFO
```

### Comparing `pypdns-2.0.0/LICENSE` & `pypdns-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdns-2.0.0/pypdns/api.py` & `pypdns-2.1.0/pypdns/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
             # No authentication defined.
             pass
 
         if https_proxy_string is not None:
             proxy = {'https': https_proxy_string}
             self.session.proxies.update(proxy)
 
-    def _query(self, q: str, sort_by: str = 'time_last', timeout: int = None) -> List[Dict[str, Optional[Union[str, int, bool, List[str], Dict[Any, Any]]]]]:
+    def _query(self, q: str, sort_by: str = 'time_last', timeout: Optional[int] = None) -> List[Dict[str, Optional[Union[str, int, bool, List[str], Dict[Any, Any]]]]]:
         logger.debug("start query() q=[%s]", q)
         if sort_by not in sort_choice:
             raise PDNSError(f'You can only sort by {", ".join(sort_choice)}')
         response: Union[Response, CachedResponse] = self.session.get(f'{self.url}/{q}', timeout=timeout if timeout else 30)
         if response.status_code != 200:
             self._handle_http_error(response)
         to_return = []
@@ -262,18 +262,18 @@
             except Exception:
                 logger.exception("except query() q=[%s]", q)
                 raise PDNSError(f'Unable to decode JSON object: {line}')
             to_return.append(obj)
         to_return = sorted(to_return, key=lambda k: k[sort_by])
         return to_return
 
-    def rfc_query(self, q: str, /, *, sort_by: str = 'time_last', timeout: int = None) -> List[PDNSRecord]:
+    def rfc_query(self, q: str, /, *, sort_by: str = 'time_last', timeout: Optional[int] = None) -> List[PDNSRecord]:
         return [PDNSRecord(record) for record in self._query(q, sort_by, timeout)]
 
-    def query(self, q: str, sort_by: str = 'time_last', timeout: int = None) -> List[Dict]:
+    def query(self, q: str, sort_by: str = 'time_last', timeout: Optional[int] = None) -> List[Dict]:
         # This method (almost) returns the response from the server but turns the times into python datetime.
         # It was a bad design decision hears ago. Use rfc_query instead for something saner.
         # This method will be deprecated.
         records = self._query(q, sort_by, timeout)
         for record in records:
             record['time_first'] = datetime.fromtimestamp(record['time_first'])  # type: ignore
             record['time_last'] = datetime.fromtimestamp(record['time_last'])  # type: ignore
```

### Comparing `pypdns-2.0.0/pyproject.toml` & `pypdns-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypdns"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python API for PDNS."
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "GPL-3.0+"
 
 readme = "README.md"
 
 repository = "https://github.com/CIRCL/PyPDNS"
@@ -14,27 +14,28 @@
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Science/Research',
     'Intended Audience :: Telecommunications Industry',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Security',
     'Topic :: Internet'
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/CIRCL/PyPDNS/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-requests-cache = "^0.9.5"
-dnspython = "^2.2.1"
-
-[tool.poetry.dev-dependencies]
-mypy = "^0.961"
-types-requests = "^2.28.1"
-pytest = "^7.1.2"
+python = "^3.8.1"
+requests-cache = "^1.0.1"
+dnspython = "^2.3.0"
+
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.4.1"
+types-requests = "^2.31.0.1"
+pytest = "^7.4.0"
 
 [build-system]
-requires = ["poetry_core>=1.0", "setuptools"]
+requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pypdns-2.0.0/PKG-INFO` & `pypdns-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pypdns
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python API for PDNS.
 Home-page: https://github.com/CIRCL/PyPDNS
 License: GPL-3.0+
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
-Requires-Dist: dnspython (>=2.2.1,<3.0.0)
-Requires-Dist: requests-cache (>=0.9.5,<0.10.0)
+Requires-Dist: dnspython (>=2.3.0,<3.0.0)
+Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/CIRCL/PyPDNS/issues
 Project-URL: Documentation, https://github.com/CIRCL/PyPDNS
 Project-URL: Repository, https://github.com/CIRCL/PyPDNS
 Description-Content-Type: text/markdown
 
 Client API for PDNS
 ===================
```

