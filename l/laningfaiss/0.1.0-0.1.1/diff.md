# Comparing `tmp/laningfaiss-0.1.0.tar.gz` & `tmp/laningfaiss-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/laningfaiss-0.1.0.tar", last modified: Wed Jun 14 03:28:25 2023, max compression
+gzip compressed data, was "dist/laningfaiss-0.1.1.tar", last modified: Fri Jun 30 03:11:28 2023, max compression
```

## Comparing `laningfaiss-0.1.0.tar` & `laningfaiss-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-23 06:17:06.000000 laningfaiss-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-06-14 03:28:06.000000 laningfaiss-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-23 06:17:06.000000 laningfaiss-0.1.0/laningfaiss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10277 2023-06-14 03:28:06.000000 laningfaiss-0.1.0/laningfaiss/requester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/laningfaiss.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 03:28:25.000000 laningfaiss-0.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      791 2023-03-23 06:38:33.000000 laningfaiss-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-23 06:18:38.000000 laningfaiss-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-06-14 03:33:01.000000 laningfaiss-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-23 06:18:38.000000 laningfaiss-0.1.1/laningfaiss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-29 10:22:47.000000 laningfaiss-0.1.1/laningfaiss/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10840 2023-06-30 03:02:51.000000 laningfaiss-0.1.1/laningfaiss/requester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/laningfaiss.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 03:11:28.000000 laningfaiss-0.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      791 2023-03-23 06:38:42.000000 laningfaiss-0.1.1/setup.py
```

### Comparing `laningfaiss-0.1.0/README.md` & `laningfaiss-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,9 +24,11 @@
 
 ```
 
 
 ### Install From GitLab
 
 ```bash
-pip install laningfaiss==0.0.12 --index-url http://__token__:sT2KnzLCX7avQ9t1MeA1@git.dev.laningtech.net/api/v4/projects/669/packages/pypi/simple
+pip install laningfaiss==0.1.0 \
+--index-url http://__token__:sT2KnzLCX7avQ9t1MeA1@git.dev.laningtech.net/api/v4/projects/669/packages/pypi/simple \
+--trusted-host git.dev.laningtech.net
 ```
```

### Comparing `laningfaiss-0.1.0/laningfaiss/requester.py` & `laningfaiss-0.1.1/laningfaiss/requester.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,82 @@
+import traceback
 from os.path import join as path_join
 from typing import List, Any
 
 import faiss
 import numpy as np
-from httpx import AsyncClient
+from httpx import AsyncClient, ConnectTimeout
+
+from . import exceptions
 
 
 class Requester:
     def __init__(self, base_url: str, timeout):
         self.base_url = base_url
         self.timeout = timeout
 
     async def request(self, method, url, retry=3, **kwargs):
         response = None
         exc = None
         for _ in range(retry):
             try:
-                async with AsyncClient() as client:
-                    response = await client.request(method, url, **kwargs)
-                    break
+                response = await self.way(method, url, **kwargs)
+                break
             except Exception as e:
+                print(f"laningfaiss exception {e}. Retrying...")
                 exc = e
 
         if response is None:
-            raise exc
+            if isinstance(exc, ConnectTimeout):
+                raise exceptions.TimeoutException(f"Connection timed out. {url}")
+            else:
+                traceback.print_exc()
+                raise exceptions.UnknownException(exc)
+
+        else:
+            return response
+
+    async def way(self, method, url, retry=3, **kwargs):
+        async with AsyncClient() as client:
+            response = await client.request(method, url, **kwargs)
         return response
 
     @staticmethod
-    def parse(response):
-        assert response.status_code == 200, f"{response.status_code} {response.reason_phrase}"
+    def parse(response, url):
+        if response.status_code != 200:
+            raise exceptions.APIException(f"Unexpected httpstatus {response.status_code} from {url}")
         data = response.json()
-        assert data["code"] == 0, data["msg"]
+        if data["code"] != 0:
+            raise exceptions.ExplicitException(f"Unexpected code {data['code']} from {url} and say: {data['msg']}")
         return data
 
     async def get(self, path: str, json=None):
         url = path_join(self.base_url, path)
         resp = await self.request("GET", url, json=json, timeout=self.timeout)
-        return self.parse(resp)
+        return self.parse(resp, url)
 
     async def post(self, path: str, json=None):
         url = path_join(self.base_url, path)
         resp = await self.request("POST", url, json=json, timeout=self.timeout)
-        return self.parse(resp)
+        return self.parse(resp, url)
 
     async def close(self):
         pass
 
 
 class RequesterContext(Requester):
     def __init__(self, base_url: str, timeout):
         super().__init__(base_url, timeout)
         self.client = AsyncClient(
             timeout=timeout,
             # limits=httpx.Limits(max_keepalive_connections=10, max_connections=20),
         )
 
-    async def request(self, method, url, retry=3, **kwargs):
-        response = None
-        exc = None
-        for _ in range(retry):
-            try:
-                response = await self.client.request(method, url, **kwargs)
-                break
-            except Exception as e:
-                print(f"laningfaiss exception {e}. Retrying.")
-                exc = e
-
-        if response is None:
-            raise exc
-        return response
+    async def way(self, method, url, retry=3, **kwargs):
+        return await self.client.request(method, url, **kwargs)
 
     async def close(self):
         await self.client.aclose()
 
 
 class Router:
     def __init__(self, base_url, timeout=10):
@@ -162,16 +166,18 @@
         :param ids: 向量id
         :param vectors: 二维向量列表，类型可以是float64,uint8等
         :param train: 是否train， 将质心添加到索引中
         :param norm: 是否要做归一化
         :return: (是否成功: bool, 错误信息: str)
 
         """
-        assert len(ids) == len(vectors), "维度不同"
-        assert len(ids) > 0, "数据不能为空"
+        if len(ids) != len(vectors):
+            raise exceptions.InvalidException("输入向量与id数量不一致")
+        if len(ids) == 0:
+            raise exceptions.InvalidException("数据不能为空")
 
         vectors_arr = np.array(vectors)
         if norm:
             vectors_arr = vectors_arr / np.linalg.norm(vectors_arr, axis=1).reshape(vectors_arr.shape[0], 1)
         payloads = {
             "ids": ids,
             "vectors": vectors_arr.tolist(),
@@ -189,15 +195,16 @@
         搜索并返回topk结果
 
         :param vectors: 二维向量列表
         :param top_k: topk的k
         :param norm: 是否要做归一化
         :return: List[List[List(id: int64, sim: float)]]
         """
-        assert len(vectors) > 0, "数据不能为空"
+        if len(vectors) == 0:
+            raise exceptions.InvalidException("数据不能为空")
         vectors_arr = np.array(vectors)
         if norm:
             vectors_arr = vectors_arr / np.linalg.norm(vectors_arr, axis=1).reshape(vectors_arr.shape[0], 1)
 
         payloads = {
             "vectors": vectors_arr.tolist(),
             "k": top_k
@@ -214,15 +221,16 @@
         搜索并返回范围内的结果
 
         :param vectors: 二维向量列表
         :param radius: 范围值
         :param norm: 是否要做归一化
         :return: List[List[List(id: int64, sim: float)]]
         """
-        assert len(vectors) > 0, "数据不能为空"
+        if len(vectors) == 0:
+            raise exceptions.InvalidException("数据不能为空")
         vectors_arr = np.array(vectors)
         if norm:
             vectors_arr = vectors_arr / np.linalg.norm(vectors_arr, axis=1).reshape(vectors_arr.shape[0], 1)
 
         payloads = {
             "vectors": vectors_arr.tolist(),
             "radius": radius
@@ -240,15 +248,16 @@
     async def remove(self, ids: List[int]):
         """
         根据id删除向量
 
         :param ids: 向量id列表
         :return: (是否成功: bool, 错误信息: str)
         """
-        assert len(ids) > 0, "数据不能为空"
+        if len(ids) == 0:
+            raise exceptions.InvalidException("数据不能为空")
         payloads = {
             "ids": ids,
         }
         try:
             await self.requester.post("remove", json=payloads)
             return True, None
```

### Comparing `laningfaiss-0.1.0/setup.py` & `laningfaiss-0.1.1/setup.py`

 * *Files identical despite different names*

