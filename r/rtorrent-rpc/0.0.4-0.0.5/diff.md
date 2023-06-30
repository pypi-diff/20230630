# Comparing `tmp/rtorrent_rpc-0.0.4.tar.gz` & `tmp/rtorrent_rpc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.0.4.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.0.5.tar", max compression
```

## Comparing `rtorrent_rpc-0.0.4.tar` & `rtorrent_rpc-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/LICENSE
--rw-r--r--   0        0        0     2511 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      741 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/readme.md
--rw-r--r--   0        0        0    22474 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     1812 2023-06-30 00:40:27.405560 rtorrent_rpc-0.0.4/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2511 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      741 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/readme.md
+-rw-r--r--   0        0        0    22601 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     1812 2023-06-30 00:45:58.965145 rtorrent_rpc-0.0.5/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.5/PKG-INFO
```

### Comparing `rtorrent_rpc-0.0.4/LICENSE` & `rtorrent_rpc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.4/pyproject.toml` & `rtorrent_rpc-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.0.4"
+version = "0.0.5"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.0.4/readme.md` & `rtorrent_rpc-0.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.4/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.0.5/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import time
-import typing
 import urllib.parse
 import xmlrpc.client
 from collections.abc import Iterator
-from pathlib import Path
-from typing import Any, Literal, TypeAlias, TypedDict
+from typing import Any, Literal, Protocol, TypeAlias, TypedDict
 
 from rtorrent_xmlrpc import SCGIServerProxy
 from typing_extensions import NotRequired
 
 __all__ = ["RTorrent"]
 
 Unknown: TypeAlias = Any
 
 
-class _MultiCall(TypedDict):
+class MultiCall(TypedDict):
     methodName: str
     params: NotRequired[Any]
 
 
 def _encode_tags(tags: list[str] | None) -> str:
     if not tags:
         return ""
 
     return ",".join(urllib.parse.quote(t) for t in {x.strip() for x in tags} if t)
 
 
-class _DownloadRpc(typing.Protocol):
+class _DownloadRpc(Protocol):
     def save_resume(self, info_hash: str) -> None:
         ...
 
     def multicall2(self, _: Literal[""], vide: str, *commands: str) -> Any:
         ...
 
 
+class _SystemRpc(Protocol):
+    def multicall(self, commands: list[MultiCall]) -> Any:
+        ...
+
+
 class RTorrent:
     def __init__(self, address: str):
         u = urllib.parse.urlparse(address)
         if u.scheme == "scgi":
             self.rpc = SCGIServerProxy(address)
         else:
             self.rpc = xmlrpc.client.ServerProxy(address)
 
-    def get_session_path(self) -> Path:
-        return Path(self.rpc.session.path())
+    def get_session_path(self) -> str:
+        return self.rpc.session.path()
 
     def add_torrent_by_file(
         self,
         content: bytes,
         directory: str,
         tags: list[str] | None = None,
     ) -> None:
@@ -61,26 +64,26 @@
 
         if tags:
             params.append(f'd.custom1.set="{_encode_tags(tags)}"')
 
         self.rpc.load.raw_start_verbose(*params)
 
     def stop_torrent(self, info_hash: str) -> None:
-        self.rpc.system.multicall(
+        self.system.multicall(
             [
-                _MultiCall(methodName="d.stop", params=[info_hash]),
-                _MultiCall(methodName="d.close", params=[info_hash]),
+                MultiCall(methodName="d.stop", params=[info_hash]),
+                MultiCall(methodName="d.close", params=[info_hash]),
             ]
         )
 
     def start_torrent(self, info_hash: str) -> None:
-        self.rpc.system.multicall(
+        self.system.multicall(
             [
-                _MultiCall(methodName="d.open", params=[info_hash]),
-                _MultiCall(methodName="d.start", params=[info_hash]),
+                MultiCall(methodName="d.open", params=[info_hash]),
+                MultiCall(methodName="d.start", params=[info_hash]),
             ]
         )
 
     def set_torrent_base_directory(self, info_hash: str, directory: str) -> None:
         self.rpc.d.directory_base.set(info_hash, directory)
 
     def download_list(self) -> list[str]:
@@ -89,14 +92,18 @@
     def system_list_methods(self) -> list[str]:
         return self.rpc.system.listMethods()
 
     def d_tracker_send_scrape(self, info_hash: str, delay: Unknown) -> None:
         return self.rpc.d.tracker.send_scrape(info_hash, delay)
 
     @property
+    def system(self) -> _SystemRpc:
+        return self.rpc.system
+
+    @property
     def d(self) -> _DownloadRpc:
         return self.rpc.d
 
     def d_save_resume(self, info_hash: str) -> None:
         return self.rpc.d.save_resume(info_hash)
 
     def d_set_tags(self, info_hash: str, tags: Iterator[str]) -> None:
```

### Comparing `rtorrent_rpc-0.0.4/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.0.5/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.4/PKG-INFO` & `rtorrent_rpc-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
```

