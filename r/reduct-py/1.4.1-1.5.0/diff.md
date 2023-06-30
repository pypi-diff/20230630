# Comparing `tmp/reduct_py-1.4.1-py3-none-any.whl.zip` & `tmp/reduct_py-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 10327 bytes, number of entries: 10
--rw-r--r--  2.0 unx      320 b- defN 23-Jun-05 21:18 reduct/__init__.py
--rw-r--r--  2.0 unx    11150 b- defN 23-Jun-05 21:18 reduct/bucket.py
--rw-r--r--  2.0 unx     6151 b- defN 23-Jun-05 21:18 reduct/client.py
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-05 21:18 reduct/error.py
--rw-r--r--  2.0 unx     3430 b- defN 23-Jun-05 21:18 reduct/http.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5002 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-05 21:18 reduct_py-1.4.1.dist-info/RECORD
-10 files, 28460 bytes uncompressed, 9049 bytes compressed:  68.2%
+Zip file size: 11980 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      342 b- defN 23-Jun-30 20:39 reduct/__init__.py
+-rw-r--r--  2.0 unx    11484 b- defN 23-Jun-30 20:39 reduct/bucket.py
+-rw-r--r--  2.0 unx     6320 b- defN 23-Jun-30 20:39 reduct/client.py
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-30 20:39 reduct/error.py
+-rw-r--r--  2.0 unx     3852 b- defN 23-Jun-30 20:39 reduct/http.py
+-rw-r--r--  2.0 unx     4784 b- defN 23-Jun-30 20:39 reduct/record.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-30 20:40 reduct_py-1.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5022 b- defN 23-Jun-30 20:40 reduct_py-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 20:40 reduct_py-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-30 20:40 reduct_py-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jun-30 20:40 reduct_py-1.5.0.dist-info/RECORD
+11 files, 34284 bytes uncompressed, 10594 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: reduct/error.py
 Comment: 
 
 Filename: reduct/http.py
 Comment: 
 
-Filename: reduct_py-1.4.1.dist-info/LICENSE
+Filename: reduct/record.py
 Comment: 
 
-Filename: reduct_py-1.4.1.dist-info/METADATA
+Filename: reduct_py-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: reduct_py-1.4.1.dist-info/WHEEL
+Filename: reduct_py-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: reduct_py-1.4.1.dist-info/top_level.txt
+Filename: reduct_py-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: reduct_py-1.4.1.dist-info/RECORD
+Filename: reduct_py-1.5.0.dist-info/top_level.txt
+Comment: 
+
+Filename: reduct_py-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reduct/__init__.py

```diff
@@ -1,16 +1,17 @@
 """Reduct module"""
+from reduct.record import Record
+
 from reduct.bucket import (
     QuotaType,
     Bucket,
     BucketInfo,
     BucketSettings,
     EntryInfo,
     BucketFullInfo,
-    Record,
 )
 
 from reduct.client import (
     Client,
     ServerInfo,
     BucketList,
     Token,
```

## reduct/bucket.py

```diff
@@ -1,27 +1,24 @@
 """Bucket API"""
 import asyncio
 import json
 import time
 from contextlib import asynccontextmanager
-from dataclasses import dataclass
 from enum import Enum
 from typing import (
     Optional,
     List,
     AsyncIterator,
     Union,
-    Callable,
-    Awaitable,
-    Dict,
 )
 
 from pydantic import BaseModel
 
 from reduct.http import HttpClient
+from reduct.record import Record, parse_batched_records, parse_record
 
 
 class QuotaType(Enum):
     """determines if database has a fixed size"""
 
     NONE = "NONE"
     FIFO = "FIFO"
@@ -93,59 +90,14 @@
     settings: BucketSettings
     """settings of bucket"""
 
     entries: List[EntryInfo]
     """information about entries of bucket"""
 
 
-@dataclass
-class Record:
-    """Record in a query"""
-
-    timestamp: int
-    """UNIX timestamp in microseconds"""
-    size: int
-    """size of data"""
-    last: bool
-    """last record in the query. Deprecated: doesn't work for some cases"""
-    content_type: str
-    """content type of data"""
-    read_all: Callable[[None], Awaitable[bytes]]
-    """read all data"""
-    read: Callable[[int], AsyncIterator[bytes]]
-    """read data in chunks"""
-
-    labels: Dict[str, str]
-    """labels of record"""
-
-
-LABEL_PREFIX = "x-reduct-label-"
-
-
-def _parse_record(resp, last=True):
-    timestamp = int(resp.headers["x-reduct-time"])
-    size = int(resp.headers["content-length"])
-    content_type = resp.headers.get("content-type", "application/octet-stream")
-    labels = dict(
-        (name[len(LABEL_PREFIX) :], value)
-        for name, value in resp.headers.items()
-        if name.startswith(LABEL_PREFIX)
-    )
-
-    return Record(
-        timestamp=timestamp,
-        size=size,
-        last=last,
-        read_all=resp.read,
-        read=resp.content.iter_chunked,
-        labels=labels,
-        content_type=content_type,
-    )
-
-
 class Bucket:
     """A bucket of data in Reduct Storage"""
 
     def __init__(self, name: str, http: HttpClient):
         self._http = http
         self.name = name
 
@@ -195,35 +147,37 @@
         Raises:
             ReductError: if there is an HTTP error
         """
         await self._http.request_all("DELETE", f"/b/{self.name}")
 
     @asynccontextmanager
     async def read(
-        self, entry_name: str, timestamp: Optional[int] = None
-    ) -> AsyncIterator[Record]:
+        self, entry_name: str, timestamp: Optional[int] = None, head: bool = False
+    ) -> Record:
         """
         Read a record from entry
         Args:
             entry_name: name of entry in the bucket
             timestamp: UNIX timestamp in microseconds - if None: get the latest record
+            head: if True: get only the header of a recod with metadata
         Returns:
-            async context, which generates Records
+            async context with a record
         Raises:
             ReductError: if there is an HTTP error
         Examples:
             >>> async def reader():
             >>>     async with bucket.read("entry", timestamp=123456789) as record:
             >>>         data = await record.read_all()
         """
         params = {"ts": int(timestamp)} if timestamp else None
+        method = "HEAD" if head else "GET"
         async with self._http.request(
-            "GET", f"/b/{self.name}/{entry_name}", params=params
+            method, f"/b/{self.name}/{entry_name}", params=params
         ) as resp:
-            yield _parse_record(resp)
+            yield parse_record(resp)
 
     async def write(
         self,
         entry_name: str,
         data: Union[bytes, AsyncIterator[bytes]],
         timestamp: Optional[int] = None,
         content_length: Optional[int] = None,
@@ -281,35 +235,49 @@
         Args:
             entry_name: name of entry in the bucket
             start: the beginning of the time interval
             stop: the end of the time interval
             ttl: Time To Live of the request in seconds
         Keyword Args:
             include (dict): query records which have all labels from this dict
-            exclude (dict): query records which doesn't have all labels from this dict
+            exclude (dict): query records which doesn't have all labels from this
+            head (bool): if True: get only the header of a recod with metadata
         Returns:
              AsyncIterator[Record]: iterator to the records
 
         Examples:
             >>> async for record in bucket.query("entry-1", stop=time.time_ns() / 1000):
             >>>     data: bytes = record.read_all()
             >>>     # or
             >>>     async for chunk in record.read(n=1024):
             >>>         print(chunk)
         """
         query_id = await self._query(entry_name, start, stop, ttl, **kwargs)
         last = False
-        while not last:
-            async with self._http.request(
-                "GET", f"/b/{self.name}/{entry_name}?q={query_id}"
-            ) as resp:
-                if resp.status == 204:
-                    return
-                last = int(resp.headers["x-reduct-last"]) != 0
-                yield _parse_record(resp, last)
+        method = "HEAD" if "head" in kwargs and kwargs["head"] else "GET"
+
+        if self._http.api_version and self._http.api_version >= "1.5":
+            while not last:
+                async with self._http.request(
+                    method, f"/b/{self.name}/{entry_name}/batch?q={query_id}"
+                ) as resp:
+                    if resp.status == 204:
+                        return
+                    async for record in parse_batched_records(resp):
+                        last = record.last
+                        yield record
+        else:
+            while not last:
+                async with self._http.request(
+                    method, f"/b/{self.name}/{entry_name}?q={query_id}"
+                ) as resp:
+                    if resp.status == 204:
+                        return
+                    last = int(resp.headers["x-reduct-last"]) != 0
+                    yield parse_record(resp, last)
 
     async def get_full_info(self) -> BucketFullInfo:
         """
         Get full information about bucket (settings, statistics, entries)
         """
         return BucketFullInfo.parse_raw(
             await self._http.request_all("GET", f"/b/{self.name}")
@@ -324,36 +292,51 @@
         Args:
             entry_name: name of entry in the bucket
             start: the beginning timestamp to read records
             poll_interval: inteval to ask new records in seconds
         Keyword Args:
             include (dict): query records which have all labels from this dict
             exclude (dict): query records which doesn't have all labels from this dict
+            head (bool): if True: get only the header of a recod with metadata
         Returns:
              AsyncIterator[Record]: iterator to the records
 
         Examples:
             >>> async for record in bucket.subscribes("entry-1"):
             >>>     data: bytes = record.read_all()
             >>>     # or
             >>>     async for chunk in record.read(n=1024):
             >>>         print(chunk)
         """
         query_id = await self._query(
             entry_name, start, None, poll_interval * 2 + 1, continuous=True, **kwargs
         )
-        while True:
-            async with self._http.request(
-                "GET", f"/b/{self.name}/{entry_name}?q={query_id}"
-            ) as resp:
-                if resp.status == 204:
-                    await asyncio.sleep(poll_interval)
-                    continue
 
-                yield _parse_record(resp, False)
+        method = "HEAD" if "head" in kwargs and kwargs["head"] else "GET"
+        if self._http.api_version and self._http.api_version >= "1.5":
+            while True:
+                async with self._http.request(
+                    method, f"/b/{self.name}/{entry_name}/batch?q={query_id}"
+                ) as resp:
+                    if resp.status == 204:
+                        await asyncio.sleep(poll_interval)
+                        continue
+
+                    async for record in parse_batched_records(resp):
+                        yield record
+        else:
+            while True:
+                async with self._http.request(
+                    method, f"/b/{self.name}/{entry_name}?q={query_id}"
+                ) as resp:
+                    if resp.status == 204:
+                        await asyncio.sleep(poll_interval)
+                        continue
+
+                    yield parse_record(resp, False)
 
     async def _query(self, entry_name, start, stop, ttl, **kwargs):
         params = {}
         if start:
             params["start"] = int(start)
         if stop:
             params["stop"] = int(stop)
```

## reduct/client.py

```diff
@@ -1,10 +1,10 @@
 """Main client code"""
 from datetime import datetime
-from typing import Optional, List
+from typing import Optional, List, Dict
 
 from pydantic import BaseModel
 
 from reduct.bucket import BucketInfo, BucketSettings, Bucket
 from reduct.http import HttpClient
 from reduct.error import ReductError
 
@@ -90,29 +90,34 @@
     """token for authentication"""
 
 
 class Client:
     """HTTP Client for Reduct Storage HTTP API"""
 
     def __init__(
-        self, url: str, api_token: Optional[str] = None, timeout: Optional[float] = None
+        self,
+        url: str,
+        api_token: Optional[str] = None,
+        timeout: Optional[float] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
     ):
         """
         Constructor
 
         Args:
             url: URL to connect to the storage
             api_token: API token if the storage uses it for authorization
             timeout: total timeout for connection, request and response in seconds
+            extra_headers: extra headers to send with each request
 
         Examples:
             >>> client = Client("http://127.0.0.1:8383")
             >>> info = await client.info()
         """
-        self._http = HttpClient(url.rstrip("/"), api_token, timeout)
+        self._http = HttpClient(url.rstrip("/"), api_token, timeout, extra_headers)
 
     async def info(self) -> ServerInfo:
         """
         Get high level server info
 
         Returns:
             ServerInfo:
```

## reduct/http.py

```diff
@@ -1,10 +1,10 @@
 """Internal HTTP helper"""
 from contextlib import asynccontextmanager
-from typing import Optional, AsyncIterator
+from typing import Optional, AsyncIterator, Dict
 
 import aiohttp
 from aiohttp import ClientTimeout, ClientResponse
 from aiohttp.client_exceptions import ClientConnectorError
 
 from reduct.error import ReductError
 
@@ -13,23 +13,30 @@
 
 class HttpClient:
     """Wrapper for HTTP calls"""
 
     FILE_SIZE_FOR_100_CONTINUE = 256_000
 
     def __init__(
-        self, url: str, api_token: Optional[str] = None, timeout: Optional[float] = None
+        self,
+        url: str,
+        api_token: Optional[str] = None,
+        timeout: Optional[float] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
     ):
-        self.url = url + API_PREFIX
-        self.api_token = api_token
-        self.headers = (
+        self._url = url + API_PREFIX
+        self._api_token = api_token
+        self._headers = (
             {"Authorization": f"Bearer {api_token}"} if api_token is not None else {}
         )
-        self.timeout = ClientTimeout(timeout)
-        self.request_count = 0
+        if extra_headers:
+            self._headers.update(extra_headers)
+
+        self._timeout = ClientTimeout(timeout)
+        self._api_version = None
 
     @asynccontextmanager
     async def request(
         self, method: str, path: str = "", **kwargs
     ) -> AsyncIterator[ClientResponse]:
         """HTTP request with ReductError exception"""
 
@@ -53,36 +60,39 @@
             if kwargs["labels"]:
                 for name, value in kwargs["labels"].items():
                     extra_headers[f"x-reduct-label-{name}"] = str(value)
             del kwargs["labels"]
 
         connector = aiohttp.TCPConnector(force_close=True)
         async with aiohttp.ClientSession(
-            timeout=self.timeout, connector=connector
+            timeout=self._timeout, connector=connector
         ) as session:
             try:
                 async with session.request(
                     method,
-                    f"{self.url}{path.strip()}",
-                    headers=dict(self.headers, **extra_headers),
+                    f"{self._url}{path.strip()}",
+                    headers=dict(self._headers, **extra_headers),
                     expect100=expect100,
                     **kwargs,
                 ) as response:
+                    if self._api_version is None:
+                        self._api_version = response.headers.get("x-reduct-api")
+
                     if response.ok:
                         yield response
                     else:
                         if "x-reduct-error" in response.headers:
                             raise ReductError(
                                 response.status,
                                 response.headers["x-reduct-error"],
                             )
                         raise ReductError(response.status, "Unknown error")
             except ClientConnectorError:
                 raise ReductError(
-                    599, f"Connection failed, server {self.url} cannot be reached"
+                    599, f"Connection failed, server {self._url} cannot be reached"
                 ) from None
 
     async def request_all(self, method: str, path: str = "", **kwargs) -> bytes:
         """Http request"""
         async with self.request(method, path, **kwargs) as response:
             return await response.read()
 
@@ -90,7 +100,12 @@
         self, method: str, path: str = "", chunk_size=1024, **kwargs
     ) -> AsyncIterator[bytes]:
         """Http request"""
         async with self.request(method, path, **kwargs) as response:
             async for chunk in response.content.iter_chunked(chunk_size):
                 yield chunk
         return
+
+    @property
+    def api_version(self) -> Optional[str]:
+        """API version"""
+        return self._api_version
```

## Comparing `reduct_py-1.4.1.dist-info/LICENSE` & `reduct_py-1.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `reduct_py-1.4.1.dist-info/METADATA` & `reduct_py-1.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reduct-py
-Version: 1.4.1
+Version: 1.5.0
 Summary: ReductStore Client SDK for Python
 Author: Ciaran Moyne
 Author-email: Alexey Timin <atimin@gmail.com>
 Maintainer-email: Alexey Timin <atimin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexey Timin
@@ -39,28 +39,28 @@
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp (~=3.8)
 Requires-Dist: pydantic (~=1.9)
 Requires-Dist: deprecation (~=2.1)
 Provides-Extra: docs
 Requires-Dist: mkdocs (~=1.3) ; extra == 'docs'
 Requires-Dist: mkdocs-material (~=9.0) ; extra == 'docs'
 Requires-Dist: plantuml-markdown (~=3.5) ; extra == 'docs'
 Requires-Dist: mkdocs-same-dir (~=0.1) ; extra == 'docs'
 Requires-Dist: mkdocstrings[python] (~=0.19) ; extra == 'docs'
 Provides-Extra: format
-Requires-Dist: black (~=22.6) ; extra == 'format'
+Requires-Dist: black (<24.0,>=22.6) ; extra == 'format'
 Provides-Extra: lint
 Requires-Dist: pylint (~=2.14) ; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest (~=7.1) ; extra == 'test'
 Requires-Dist: pytest-mock (~=3.10) ; extra == 'test'
 Requires-Dist: pytest-asyncio (~=0.18) ; extra == 'test'
 
@@ -70,19 +70,20 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/reduct-py)](https://pypi.org/project/reduct-py/)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/reductstore/reduct-py/ci.yml?branch=main)](https://github.com/reductstore/reduct-py/actions)
 
 This package provides an asynchronous HTTP client for interacting with the [ReductStore](https://www.reduct.store) service.
 
 ## Features
 
-* Supports the [ReductStore HTTP API v1.4](https://docs.reduct.store/http-api)
+* Supports the [ReductStore HTTP API v1.5](https://docs.reduct.store/http-api)
 * Bucket management
 * API Token management
 * Write, read and query data
 * Labels
+* Batching records
 * Subscription on new data
 
 ## Install
 
 To install this package, run the following command:
 
 ```
@@ -115,13 +116,13 @@
         print(data)
 
 # Run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
 
-For more examples, see the [Quick Start](https://py.reduct.storgit ce/en/latest/docs/quick-start/).
+For more examples, see the [Quick Start](https://py.reduct.store/en/latest/docs/quick-start/).
 
 ## References
 
 * [Documentation](https://py.reduct.store/)
 * [ReductStore HTTP API](https://docs.reduct.store/http-api)
```

