# Comparing `tmp/rtorrent_rpc-0.0.3.tar.gz` & `tmp/rtorrent_rpc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.0.3.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.0.4.tar", max compression
```

## Comparing `rtorrent_rpc-0.0.3.tar` & `rtorrent_rpc-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/LICENSE
--rw-r--r--   0        0        0     2511 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      745 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/readme.md
--rw-r--r--   0        0        0    22474 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     1627 2023-06-30 00:36:34.290526 rtorrent_rpc-0.0.3/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2511 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      741 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/readme.md
+-rw-r--r--   0        0        0    22474 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     1812 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.4/PKG-INFO
```

### Comparing `rtorrent_rpc-0.0.3/LICENSE` & `rtorrent_rpc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.3/pyproject.toml` & `rtorrent_rpc-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.0.3"
+version = "0.0.4"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.0.3/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.0.4/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.3/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.0.4/rtorrent_rpc/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 import bencodepy
 
 __all__ = ["add_completed_resume_file"]
 
 
 def add_completed_resume_file(base_save_path: Path, torrent_content: bytes) -> bytes:
+    """update torrent content, add resume data to torrent.
+
+    based on [rtorrent_fast_resume.pl](https://github.com/rakshasa/rtorrent/blob/master/doc/rtorrent_fast_resume.pl)
+    """
     data: dict[bytes, Any] = bencodepy.bdecode(torrent_content)
 
     piece_length = data[b"info"][b"piece length"]
     files = []
 
     t_files = data[b"info"].get(b"files")
```

### Comparing `rtorrent_rpc-0.0.3/PKG-INFO` & `rtorrent_rpc-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
@@ -20,15 +20,15 @@
 Requires-Dist: rtorrent-xmlrpc (>=0.0.3,<0.0.4)
 Requires-Dist: typing-extensions (>=4.1.0)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
-[![PyPI](https://img.shields.io/pypi/v/transmission-rpc)](https://pypi.org/project/rtorrent-rpc/)
+[![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 
 `rtorrent-rpc` is a python wrapper on top of rtorrent XML RPC protocol,
 hosted on GitHub at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
 
 ## Introduction
```

