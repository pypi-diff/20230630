# Comparing `tmp/rtorrent_rpc-0.0.2.tar.gz` & `tmp/rtorrent_rpc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.0.2.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.0.3.tar", max compression
```

## Comparing `rtorrent_rpc-0.0.2.tar` & `rtorrent_rpc-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-30 00:32:55.086449 rtorrent_rpc-0.0.2/LICENSE
--rw-r--r--   0        0        0     2875 2023-06-30 00:32:55.086449 rtorrent_rpc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      745 2023-06-30 00:32:55.086449 rtorrent_rpc-0.0.2/readme.md
--rw-r--r--   0        0        0    22474 2023-06-30 00:32:55.086449 rtorrent_rpc-0.0.2/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     1502 2023-06-30 00:32:55.086449 rtorrent_rpc-0.0.2/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2511 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/readme.md
+-rw-r--r--   0        0        0    22474 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     1627 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.3/PKG-INFO
```

### Comparing `rtorrent_rpc-0.0.2/LICENSE` & `rtorrent_rpc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.2/pyproject.toml` & `rtorrent_rpc-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.0.2"
+version = "0.0.3"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -16,19 +16,18 @@
     'Intended Audience :: Developers',
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: Implementation :: CPython',
-    'Programming Language :: Python :: Implementation :: PyPy',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10"
 # dependencies
 typing-extensions = ">=4.1.0"
 rtorrent-xmlrpc = "^0.0.3"
 bencode-py = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
@@ -45,44 +44,31 @@
 pre-commit = { version = "==3.3.3", markers = "implementation_name != 'pypy'", python = "^3.9" }
 mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
 ruff = "0.0.275"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
-[tool.isort]
-default_section = 'THIRDPARTY'
-indent = '    '
-profile = 'black'
-known_first_party = 'transmission_rpc'
-length_sort = true
-line_length = 120
-no_lines_before = 'LOCALFOLDER'
-use_parentheses = true
-include_trailing_comma = true
-
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
 
 [tool.mypy]
 python_version = "3.10"
 disallow_untyped_defs = true
 ignore_missing_imports = true
 warn_return_any = false
 warn_unused_configs = true
 show_error_codes = true
 
 [tool.black]
-line-length = 120
-target-version = ['py37']
+target-version = ['py310']
 
 
 [tool.ruff]
 extend-exclude = ["docs"]
-line-length = 120
 select = [
     "B",
     "C",
     "E",
     "F",
     "G",
     "I",
@@ -124,17 +110,15 @@
     'RUF002',
     'S301',
     'S314',
     'S101',
     'N815',
     'S104',
     'C901',
-    'ISC003',
     'PLR0913',
-    'I001',
     'RUF001',
     'SIM108',
     'TCH003',
     'RUF003',
     'RET504',
     'TRY300',
     'TRY003',
```

### Comparing `rtorrent_rpc-0.0.2/readme.md` & `rtorrent_rpc-0.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.2/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.0.3/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import typing
 import urllib.parse
 import xmlrpc.client
 from collections.abc import Iterator
 from pathlib import Path
-from typing import Any, TypedDict, Literal, TypeAlias
+from typing import Any, Literal, TypeAlias, TypedDict
 
 from rtorrent_xmlrpc import SCGIServerProxy
 from typing_extensions import NotRequired
 
 __all__ = ["RTorrent"]
 
 Unknown: TypeAlias = Any
```

### Comparing `rtorrent_rpc-0.0.2/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.0.3/rtorrent_rpc/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,23 +21,29 @@
             if not file_path.exists():
                 files.append({b"complete": 0, b"mtime": 0, b"priority": 0})
                 continue
 
             stat = file_path.lstat()
             if stat.st_size == file[b"length"]:
                 files.append(
-                    {b"complete": int(file.length / piece_length), b"mtime": int(stat.st_mtime), b"priority": 1}
+                    {
+                        b"complete": int(file.length / piece_length),
+                        b"mtime": int(stat.st_mtime),
+                        b"priority": 1,
+                    }
                 )
             else:
                 files.append({b"complete": 0, b"mtime": 0, b"priority": 1})
     else:
         # return torrent_content
         stat = base_save_path.joinpath(data[b"info"][b"name"]).lstat()
         if stat.st_size == data[b"info"][b"length"]:
-            files.append({b"complete": piece_count, b"mtime": int(stat.st_mtime), b"priority": 1})
+            files.append(
+                {b"complete": piece_count, b"mtime": int(stat.st_mtime), b"priority": 1}
+            )
         else:
             return torrent_content
 
     data[b"rtorrent"] = None
     del data[b"rtorrent"]
 
     data[b"libtorrent_resume"] = {b"bitfield": piece_count, b"files": files}
```

### Comparing `rtorrent_rpc-0.0.2/PKG-INFO` & `rtorrent_rpc-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: bencode-py (>=4.0.0,<5.0.0)
 Requires-Dist: rtorrent-xmlrpc (>=0.0.3,<0.0.4)
 Requires-Dist: typing-extensions (>=4.1.0)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
```

