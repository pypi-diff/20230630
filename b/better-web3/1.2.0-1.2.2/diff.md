# Comparing `tmp/better_web3-1.2.0.tar.gz` & `tmp/better_web3-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.2.0.tar", max compression
+gzip compressed data, was "better_web3-1.2.2.tar", max compression
```

## Comparing `better_web3-1.2.0.tar` & `better_web3-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      377 2023-06-28 12:16:08.388000 better_web3-1.2.0/better_web3/__init__.py
--rw-r--r--   0        0        0     9454 2023-06-28 12:32:41.774000 better_web3-1.2.0/better_web3/batch_call.py
--rw-r--r--   0        0        0    12783 2023-06-28 12:13:28.651000 better_web3-1.2.0/better_web3/chain.py
--rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.2.0/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.2.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.2.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0      609 2023-06-28 12:32:25.796000 better_web3-1.2.0/better_web3/contract/__pycache__/abi.cpython-311.pyc
--rw-r--r--   0        0        0     2861 2023-06-28 12:47:45.841000 better_web3-1.2.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.2.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.2.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.2.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.2.0/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.2.0/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.2.0/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.2.0/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.2.0/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0      295 2023-06-28 12:32:24.657000 better_web3-1.2.0/better_web3/contract/abi.py
--rw-r--r--   0        0        0     1217 2023-06-28 12:35:30.364000 better_web3-1.2.0/better_web3/contract/contract.py
--rw-r--r--   0        0        0     1749 2023-06-22 18:23:50.372000 better_web3-1.2.0/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2873 2023-06-22 18:23:50.412000 better_web3-1.2.0/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6182 2023-06-22 17:29:46.245000 better_web3-1.2.0/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.2.0/better_web3/enums.py
--rw-r--r--   0        0        0      199 2023-06-28 11:42:15.433000 better_web3-1.2.0/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      445 2023-06-28 12:32:10.840000 better_web3-1.2.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.2.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.2.0/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     1519 2023-06-28 12:32:10.893000 better_web3-1.2.0/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.2.0/better_web3/utils/eth.py
--rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.2.0/better_web3/utils/file.py
--rw-r--r--   0        0        0      733 2023-06-28 11:42:15.546000 better_web3-1.2.0/better_web3/utils/other.py
--rw-r--r--   0        0        0     1474 2023-06-29 11:26:53.088000 better_web3-1.2.0/better_web3/wallet.py
--rw-r--r--   0        0        0      455 2023-06-28 12:13:28.586000 better_web3-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      406 2023-06-23 11:07:22.626000 better_web3-1.2.0/README.md
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 better_web3-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      414 2023-06-30 17:38:45.992000 better_web3-1.2.2/better_web3/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-30 17:09:01.017000 better_web3-1.2.2/better_web3/_paths.py
+-rw-r--r--   0        0        0     9454 2023-06-28 12:32:41.774000 better_web3-1.2.2/better_web3/batch_call.py
+-rw-r--r--   0        0        0    12864 2023-06-30 17:28:39.870000 better_web3-1.2.2/better_web3/chain.py
+-rw-r--r--   0        0        0      769 2023-06-30 17:47:42.447000 better_web3-1.2.2/better_web3/chains.py
+-rw-r--r--   0        0        0     1173 2023-06-30 17:27:26.072000 better_web3-1.2.2/better_web3/chains.toml
+-rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.2.2/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.2.2/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.2.2/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      609 2023-06-28 12:32:25.796000 better_web3-1.2.2/better_web3/contract/__pycache__/abi.cpython-311.pyc
+-rw-r--r--   0        0        0     2861 2023-06-28 12:47:45.841000 better_web3-1.2.2/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.2.2/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.2.2/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.2.2/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.2.2/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.2.2/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.2.2/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.2.2/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.2.2/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0      295 2023-06-28 12:32:24.657000 better_web3-1.2.2/better_web3/contract/abi.py
+-rw-r--r--   0        0        0     1217 2023-06-28 12:35:30.364000 better_web3-1.2.2/better_web3/contract/contract.py
+-rw-r--r--   0        0        0     1749 2023-06-22 18:23:50.372000 better_web3-1.2.2/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2873 2023-06-22 18:23:50.412000 better_web3-1.2.2/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6182 2023-06-22 17:29:46.245000 better_web3-1.2.2/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.2.2/better_web3/enums.py
+-rw-r--r--   0        0        0      199 2023-06-28 11:42:15.433000 better_web3-1.2.2/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-28 12:32:10.840000 better_web3-1.2.2/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.2.2/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.2.2/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1519 2023-06-28 12:32:10.893000 better_web3-1.2.2/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.2.2/better_web3/utils/eth.py
+-rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.2.2/better_web3/utils/file.py
+-rw-r--r--   0        0        0      733 2023-06-28 11:42:15.546000 better_web3-1.2.2/better_web3/utils/other.py
+-rw-r--r--   0        0        0     1474 2023-06-29 11:26:53.088000 better_web3-1.2.2/better_web3/wallet.py
+-rw-r--r--   0        0        0      445 2023-06-30 19:21:32.461000 better_web3-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-06-23 11:07:22.626000 better_web3-1.2.2/README.md
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 better_web3-1.2.2/PKG-INFO
```

### Comparing `better_web3-1.2.0/better_web3/batch_call.py` & `better_web3-1.2.2/better_web3/batch_call.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/chain.py` & `better_web3-1.2.2/better_web3/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 class Chain:
     def __init__(
             self,
             rpc: str,
             *,
             name: str = "EVM Chain",
+            is_testnet: bool = False,
             # Native token
             symbol: str = "ETH",
             decimals: int = 18,
             # Explorer
             explorer_url: str = None,
             # Connection settings
             provider_timeout: int = 15,
@@ -49,14 +50,15 @@
             multicall_v3_address: ChecksumAddress | str = None,
             # Batch request
             batch_request_size: int = 500,
             batch_request_delay: int = 1,
     ):
         self._rpc = rpc
         self.name = name
+        self.is_testnet = is_testnet
         self.token = NativeToken(symbol=symbol, decimals=decimals)
         self.explorer_url = explorer_url
 
         self.http_session = self._prepare_http_session(retry_count)
         self.timeout = provider_timeout
         self.slow_timeout = slow_provider_timeout
 
@@ -78,15 +80,15 @@
         return HTTPProvider(
             self._rpc,
             request_kwargs={"timeout": timeout},
             session=self.http_session,
         )
 
     def __repr__(self):
-        return f"Chain(rpc={self.rpc})"
+        return f"Chain(rpc=\"{self.rpc})\""
 
     def __str__(self):
         return f"<{self.name}>"
 
     @staticmethod
     def _prepare_http_session(retry_count: int) -> requests.Session:
         """
```

### Comparing `better_web3-1.2.0/better_web3/contract/__pycache__/abi.cpython-311.pyc` & `better_web3-1.2.2/better_web3/contract/__pycache__/abi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.2.2/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-1.2.2/better_web3/contract/__pycache__/erc20.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-1.2.2/better_web3/contract/__pycache__/erc721.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.2.2/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/abi/erc1155.json` & `better_web3-1.2.2/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/abi/erc20.json` & `better_web3-1.2.2/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/abi/erc721.json` & `better_web3-1.2.2/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.2.2/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/contract.py` & `better_web3-1.2.2/better_web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/erc20.py` & `better_web3-1.2.2/better_web3/contract/erc20.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/erc721.py` & `better_web3-1.2.2/better_web3/contract/erc721.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/contract/multicall.py` & `better_web3-1.2.2/better_web3/contract/multicall.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.2.2/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-1.2.2/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-1.2.2/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/utils/eth.py` & `better_web3-1.2.2/better_web3/utils/eth.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/utils/file.py` & `better_web3-1.2.2/better_web3/utils/file.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/utils/other.py` & `better_web3-1.2.2/better_web3/utils/other.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/better_web3/wallet.py` & `better_web3-1.2.2/better_web3/wallet.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.0/PKG-INFO` & `better_web3-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.2.0
-Summary: Chain, Explorer, Contracts(Multicall, ERC20/ERC721), batch calls and other..
+Version: 1.2.2
+Summary: Chain, Contracts(Multicall, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

