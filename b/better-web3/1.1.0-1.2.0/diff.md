# Comparing `tmp/better_web3-1.1.0.tar.gz` & `tmp/better_web3-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.1.0.tar", max compression
+gzip compressed data, was "better_web3-1.2.0.tar", max compression
```

## Comparing `better_web3-1.1.0.tar` & `better_web3-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      332 2023-06-23 09:35:05.770000 better_web3-1.1.0/better_web3/__init__.py
--rw-r--r--   0        0        0     9431 2023-06-22 18:23:50.481000 better_web3-1.1.0/better_web3/batch_call.py
--rw-r--r--   0        0        0    12399 2023-06-23 10:58:37.851000 better_web3-1.1.0/better_web3/chain.py
--rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.1.0/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.1.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.1.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0      604 2023-06-05 07:45:48.506000 better_web3-1.1.0/better_web3/contract/__pycache__/abi.cpython-311.pyc
--rw-r--r--   0        0        0     3132 2023-06-07 15:59:49.144000 better_web3-1.1.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.1.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.1.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.1.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.1.0/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.1.0/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.1.0/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.1.0/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.1.0/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0      290 2023-06-05 07:40:59.110000 better_web3-1.1.0/better_web3/contract/abi.py
--rw-r--r--   0        0        0     1347 2023-06-07 12:04:43.463000 better_web3-1.1.0/better_web3/contract/contract.py
--rw-r--r--   0        0        0     1749 2023-06-22 18:23:50.372000 better_web3-1.1.0/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2873 2023-06-22 18:23:50.412000 better_web3-1.1.0/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6182 2023-06-22 17:29:46.245000 better_web3-1.1.0/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.1.0/better_web3/enums.py
--rw-r--r--   0        0        0      554 2023-06-23 09:34:50.577000 better_web3-1.1.0/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      796 2023-06-23 09:34:51.967000 better_web3-1.1.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.1.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     1167 2023-06-23 09:34:52.007000 better_web3-1.1.0/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     1125 2023-06-23 09:34:52.052000 better_web3-1.1.0/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.1.0/better_web3/utils/eth.py
--rw-r--r--   0        0        0      301 2023-06-23 09:34:50.776000 better_web3-1.1.0/better_web3/utils/file.py
--rw-r--r--   0        0        0      550 2023-06-23 09:34:50.673000 better_web3-1.1.0/better_web3/utils/other.py
--rw-r--r--   0        0        0      455 2023-06-19 19:00:52.064000 better_web3-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      406 2023-06-23 11:07:22.626000 better_web3-1.1.0/README.md
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 better_web3-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-06-28 12:16:08.388000 better_web3-1.2.0/better_web3/__init__.py
+-rw-r--r--   0        0        0     9454 2023-06-28 12:32:41.774000 better_web3-1.2.0/better_web3/batch_call.py
+-rw-r--r--   0        0        0    12783 2023-06-28 12:13:28.651000 better_web3-1.2.0/better_web3/chain.py
+-rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.2.0/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.2.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.2.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      609 2023-06-28 12:32:25.796000 better_web3-1.2.0/better_web3/contract/__pycache__/abi.cpython-311.pyc
+-rw-r--r--   0        0        0     2861 2023-06-28 12:47:45.841000 better_web3-1.2.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.2.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.2.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.2.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.2.0/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.2.0/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.2.0/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.2.0/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.2.0/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0      295 2023-06-28 12:32:24.657000 better_web3-1.2.0/better_web3/contract/abi.py
+-rw-r--r--   0        0        0     1217 2023-06-28 12:35:30.364000 better_web3-1.2.0/better_web3/contract/contract.py
+-rw-r--r--   0        0        0     1749 2023-06-22 18:23:50.372000 better_web3-1.2.0/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2873 2023-06-22 18:23:50.412000 better_web3-1.2.0/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6182 2023-06-22 17:29:46.245000 better_web3-1.2.0/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.2.0/better_web3/enums.py
+-rw-r--r--   0        0        0      199 2023-06-28 11:42:15.433000 better_web3-1.2.0/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-28 12:32:10.840000 better_web3-1.2.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.2.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.2.0/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1519 2023-06-28 12:32:10.893000 better_web3-1.2.0/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.2.0/better_web3/utils/eth.py
+-rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.2.0/better_web3/utils/file.py
+-rw-r--r--   0        0        0      733 2023-06-28 11:42:15.546000 better_web3-1.2.0/better_web3/utils/other.py
+-rw-r--r--   0        0        0     1474 2023-06-29 11:26:53.088000 better_web3-1.2.0/better_web3/wallet.py
+-rw-r--r--   0        0        0      455 2023-06-28 12:13:28.586000 better_web3-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-06-23 11:07:22.626000 better_web3-1.2.0/README.md
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 better_web3-1.2.0/PKG-INFO
```

### Comparing `better_web3-1.1.0/better_web3/batch_call.py` & `better_web3-1.2.0/better_web3/batch_call.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     BlockIdentifier,
     TxData,
     TxParams,
     TxReceipt,
     Wei,
 )
 
-from .utils import chunks, hex_block_identifier
+from .utils import chunks
+from .utils.eth import hex_block_identifier
 
 if TYPE_CHECKING:
     from .chain import Chain
 
 
 def build_payload(index: int, method: str, params: list) -> dict:
     return {"id": index, "jsonrpc": "2.0", "method": method, "params": params}
```

### Comparing `better_web3-1.1.0/better_web3/chain.py` & `better_web3-1.2.0/better_web3/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
 class Chain:
     def __init__(
             self,
             rpc: str,
             *,
+            name: str = "EVM Chain",
             # Native token
             symbol: str = "ETH",
             decimals: int = 18,
             # Explorer
             explorer_url: str = None,
             # Connection settings
             provider_timeout: int = 15,
@@ -47,14 +48,15 @@
             # Multicall
             multicall_v3_address: ChecksumAddress | str = None,
             # Batch request
             batch_request_size: int = 500,
             batch_request_delay: int = 1,
     ):
         self._rpc = rpc
+        self.name = name
         self.token = NativeToken(symbol=symbol, decimals=decimals)
         self.explorer_url = explorer_url
 
         self.http_session = self._prepare_http_session(retry_count)
         self.timeout = provider_timeout
         self.slow_timeout = slow_provider_timeout
 
@@ -76,18 +78,18 @@
         return HTTPProvider(
             self._rpc,
             request_kwargs={"timeout": timeout},
             session=self.http_session,
         )
 
     def __repr__(self):
-        try:
-            return f"Chain(id={self.chain_id}, rpc={self.rpc})"
-        except:  # TODO Определить исключение
-            return f"Chain(rpc={self.rpc})"
+        return f"Chain(rpc={self.rpc})"
+
+    def __str__(self):
+        return f"<{self.name}>"
 
     @staticmethod
     def _prepare_http_session(retry_count: int) -> requests.Session:
         """
         Prepare http session with custom pooling. See:
         https://urllib3.readthedocs.io/en/stable/advanced-usage.html
         https://2.python-requests.org/en/latest/api/#requests.adapters.HTTPAdapter
@@ -325,7 +327,19 @@
         return HexStr(tx_hash.hex())
 
     def _send_tx(self, tx: TxParams) -> HexBytes:
         return self.w3.eth.send_transaction(tx)
 
     def _send_raw_tx(self, raw_tx: bytes | HexStr) -> HexBytes:
         return self.w3.eth.send_raw_transaction(bytes(raw_tx))
+
+    def execute_fn(
+            self,
+            account: LocalAccount,
+            fn: ContractFunction,
+            *,
+            value: Wei = None,
+    ) -> tuple[TxReceipt, HexStr]:
+        tx = self.build_tx(fn, from_=account.address, value=value)
+        tx_hash = self.sign_and_send_tx(account, tx)
+        tx_receipt = self.wait_for_tx_receipt(tx_hash)
+        return tx_receipt, tx_hash
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `better_web3-1.1.0/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.2.0/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x5b728064 (Wed Jun  7 12:04:43 2023 UTC)
-files sz: 1347
+moddate:  0x12299c64 (Wed Jun 28 12:35:30 2023 UTC)
+files sz: 1217
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a070100640064056c086d095a
-      0a0100640064066c086d0b5a0b6d0c5a0c01006501720c640764086c0d6d
-      0e5a0e0100640764096c0f6d105a10010002004700640a8400640ba60200
-      00ab0200000000000000005a09640c5300
+      0a0100640064066c086d0b5a0b6d0c5a0c010065017206640764086c0d6d
+      0e5a0e01000200470064098400640aa6020000ab0200000000000000005a
+      09640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('TYPE_CHECKING',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (TYPE_CHECKING)
                 10 STORE_NAME               1 (TYPE_CHECKING)
@@ -55,181 +55,161 @@
                 68 IMPORT_FROM             11 (ContractEvents)
                 70 STORE_NAME              11 (ContractEvents)
                 72 IMPORT_FROM             12 (ContractFunctions)
                 74 STORE_NAME              12 (ContractFunctions)
                 76 POP_TOP
    
      9          78 LOAD_NAME                1 (TYPE_CHECKING)
-                80 POP_JUMP_FORWARD_IF_FALSE    12 (to 106)
+                80 POP_JUMP_FORWARD_IF_FALSE     6 (to 94)
    
     10          82 LOAD_CONST               7 (2)
                 84 LOAD_CONST               8 (('Chain',))
                 86 IMPORT_NAME             13 (chain)
                 88 IMPORT_FROM             14 (Chain)
                 90 STORE_NAME              14 (Chain)
                 92 POP_TOP
    
-    11          94 LOAD_CONST               7 (2)
-                96 LOAD_CONST               9 (('Explorer',))
-                98 IMPORT_NAME             15 (explorer)
-               100 IMPORT_FROM             16 (Explorer)
-               102 STORE_NAME              16 (Explorer)
-               104 POP_TOP
-   
-    14     >>  106 PUSH_NULL
-               108 LOAD_BUILD_CLASS
-               110 LOAD_CONST              10 (<code object Contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 14>)
-               112 MAKE_FUNCTION            0
-               114 LOAD_CONST              11 ('Contract')
-               116 PRECALL                  2
-               120 CALL                     2
-               130 STORE_NAME               9 (Contract)
-               132 LOAD_CONST              12 (None)
-               134 RETURN_VALUE
+    13     >>   94 PUSH_NULL
+                96 LOAD_BUILD_CLASS
+                98 LOAD_CONST               9 (<code object Contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 13>)
+               100 MAKE_FUNCTION            0
+               102 LOAD_CONST              10 ('Contract')
+               104 PRECALL                  2
+               108 CALL                     2
+               118 STORE_NAME               9 (Contract)
+               120 LOAD_CONST              11 (None)
+               122 RETURN_VALUE
    consts
       0
       ('TYPE_CHECKING',)
       ('ChecksumAddress',)
       ('to_checksum_address',)
       ('Web3',)
       ('Contract',)
       ('ContractEvents', 'ContractFunctions')
       2
       ('Chain',)
-      ('Explorer',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02640164026403650365047a0700006604640484
             045a05650664056507660264068404a6000000ab0000000000000000005a
-            086506641064078404a6000000ab0000000000000000005a096506641164
-            098404a6000000ab0000000000000000005a0a65066405650b6602640a84
-            04a6000000ab0000000000000000005a0c6506640565046602640b8404a6
-            000000ab0000000000000000005a0d6506640c8400a6000000ab00000000
-            00000000005a0e65066405650f6602640d8404a6000000ab000000000000
-            0000005a106506640565116602640e8404a6000000ab0000000000000000
-            005a12640f5300
-          14           0 RESUME                   0
+            086506640e64078404a6000000ab0000000000000000005a096506640565
+            0a660264088404a6000000ab0000000000000000005a0b65066405650466
+            0264098404a6000000ab0000000000000000005a0c6506640a8400a60000
+            00ab0000000000000000005a0d65066405650e6602640b8404a6000000ab
+            0000000000000000005a0f6506640565106602640c8404a6000000ab0000
+            000000000000005a11640d5300
+          13           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Contract')
                        8 STORE_NAME               2 (__qualname__)
          
-          15          10 LOAD_CONST               1 ('chain')
+          14          10 LOAD_CONST               1 ('chain')
                       12 LOAD_CONST               2 ('Chain')
                       14 LOAD_CONST               3 ('address')
                       16 LOAD_NAME                3 (ChecksumAddress)
                       18 LOAD_NAME                4 (str)
                       20 BINARY_OP                7 (|)
                       24 BUILD_TUPLE              4
-                      26 LOAD_CONST               4 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 15>)
+                      26 LOAD_CONST               4 (<code object __init__, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 14>)
                       28 MAKE_FUNCTION            4 (annotations)
                       30 STORE_NAME               5 (__init__)
          
-          21          32 LOAD_NAME                6 (property)
+          20          32 LOAD_NAME                6 (property)
          
-          22          34 LOAD_CONST               5 ('return')
+          21          34 LOAD_CONST               5 ('return')
                       36 LOAD_NAME                7 (Web3)
                       38 BUILD_TUPLE              2
-                      40 LOAD_CONST               6 (<code object w3, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 21>)
+                      40 LOAD_CONST               6 (<code object w3, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 20>)
                       42 MAKE_FUNCTION            4 (annotations)
          
-          21          44 PRECALL                  0
+          20          44 PRECALL                  0
                       48 CALL                     0
          
-          22          58 STORE_NAME               8 (w3)
+          21          58 STORE_NAME               8 (w3)
          
-          25          60 LOAD_NAME                6 (property)
+          24          60 LOAD_NAME                6 (property)
          
-          26          62 LOAD_CONST              16 (('return', 'Chain'))
-                      64 LOAD_CONST               7 (<code object chain, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 25>)
+          25          62 LOAD_CONST              14 (('return', 'Chain'))
+                      64 LOAD_CONST               7 (<code object chain, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 24>)
                       66 MAKE_FUNCTION            4 (annotations)
          
-          25          68 PRECALL                  0
+          24          68 PRECALL                  0
                       72 CALL                     0
          
-          26          82 STORE_NAME               9 (chain)
-         
-          29          84 LOAD_NAME                6 (property)
-         
-          30          86 LOAD_CONST              17 (('return', 'Explorer'))
-                      88 LOAD_CONST               9 (<code object explorer, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 29>)
-                      90 MAKE_FUNCTION            4 (annotations)
+          25          82 STORE_NAME               9 (chain)
          
-          29          92 PRECALL                  0
-                      96 CALL                     0
+          28          84 LOAD_NAME                6 (property)
          
-          30         106 STORE_NAME              10 (explorer)
+          29          86 LOAD_CONST               5 ('return')
+                      88 LOAD_NAME               10 (Web3Contract)
+                      90 BUILD_TUPLE              2
+                      92 LOAD_CONST               8 (<code object contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 28>)
+                      94 MAKE_FUNCTION            4 (annotations)
          
-          33         108 LOAD_NAME                6 (property)
+          28          96 PRECALL                  0
+                     100 CALL                     0
          
-          34         110 LOAD_CONST               5 ('return')
-                     112 LOAD_NAME               11 (Web3Contract)
-                     114 BUILD_TUPLE              2
-                     116 LOAD_CONST              10 (<code object contract, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 33>)
-                     118 MAKE_FUNCTION            4 (annotations)
+          29         110 STORE_NAME              11 (contract)
          
-          33         120 PRECALL                  0
-                     124 CALL                     0
+          32         112 LOAD_NAME                6 (property)
          
-          34         134 STORE_NAME              12 (contract)
+          33         114 LOAD_CONST               5 ('return')
+                     116 LOAD_NAME                4 (str)
+                     118 BUILD_TUPLE              2
+                     120 LOAD_CONST               9 (<code object address, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 32>)
+                     122 MAKE_FUNCTION            4 (annotations)
          
-          37         136 LOAD_NAME                6 (property)
+          32         124 PRECALL                  0
+                     128 CALL                     0
          
-          38         138 LOAD_CONST               5 ('return')
-                     140 LOAD_NAME                4 (str)
-                     142 BUILD_TUPLE              2
-                     144 LOAD_CONST              11 (<code object address, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 37>)
-                     146 MAKE_FUNCTION            4 (annotations)
+          33         138 STORE_NAME              12 (address)
          
-          37         148 PRECALL                  0
-                     152 CALL                     0
+          36         140 LOAD_NAME                6 (property)
          
-          38         162 STORE_NAME              13 (address)
+          37         142 LOAD_CONST              10 (<code object abi, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 36>)
+                     144 MAKE_FUNCTION            0
          
-          41         164 LOAD_NAME                6 (property)
+          36         146 PRECALL                  0
+                     150 CALL                     0
          
-          42         166 LOAD_CONST              12 (<code object abi, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 41>)
-                     168 MAKE_FUNCTION            0
+          37         160 STORE_NAME              13 (abi)
          
-          41         170 PRECALL                  0
-                     174 CALL                     0
+          40         162 LOAD_NAME                6 (property)
          
-          42         184 STORE_NAME              14 (abi)
+          41         164 LOAD_CONST               5 ('return')
+                     166 LOAD_NAME               14 (ContractFunctions)
+                     168 BUILD_TUPLE              2
+                     170 LOAD_CONST              11 (<code object functions, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 40>)
+                     172 MAKE_FUNCTION            4 (annotations)
          
-          45         186 LOAD_NAME                6 (property)
+          40         174 PRECALL                  0
+                     178 CALL                     0
          
-          46         188 LOAD_CONST               5 ('return')
-                     190 LOAD_NAME               15 (ContractFunctions)
-                     192 BUILD_TUPLE              2
-                     194 LOAD_CONST              13 (<code object functions, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 45>)
-                     196 MAKE_FUNCTION            4 (annotations)
+          41         188 STORE_NAME              15 (functions)
          
-          45         198 PRECALL                  0
-                     202 CALL                     0
+          44         190 LOAD_NAME                6 (property)
          
-          46         212 STORE_NAME              16 (functions)
+          45         192 LOAD_CONST               5 ('return')
+                     194 LOAD_NAME               16 (ContractEvents)
+                     196 BUILD_TUPLE              2
+                     198 LOAD_CONST              12 (<code object events, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 44>)
+                     200 MAKE_FUNCTION            4 (annotations)
          
-          49         214 LOAD_NAME                6 (property)
+          44         202 PRECALL                  0
+                     206 CALL                     0
          
-          50         216 LOAD_CONST               5 ('return')
-                     218 LOAD_NAME               17 (ContractEvents)
-                     220 BUILD_TUPLE              2
-                     222 LOAD_CONST              14 (<code object events, file "H:\Мой диск\Projects\Python\better_web3\better_web3\contract\contract.py", line 49>)
-                     224 MAKE_FUNCTION            4 (annotations)
-         
-          49         226 PRECALL                  0
-                     230 CALL                     0
-         
-          50         240 STORE_NAME              18 (events)
-                     242 LOAD_CONST              15 (None)
-                     244 RETURN_VALUE
+          45         216 STORE_NAME              17 (events)
+                     218 LOAD_CONST              13 (None)
+                     220 RETURN_VALUE
          consts
             'Contract'
             'chain'
             'Chain'
             'address'
             code
                argcount  : 4
@@ -239,34 +219,34 @@
                code
                   0x97007401000000000000000000007c02740200000000000000000000a6
                   020000ab020000000000000000720f7405000000000000000000007c02a6
                   010000ab0100000000000000007d027c017c005f0300000000000000007c
                   006a0300000000000000006a0400000000000000006a0500000000000000
                   00a00600000000000000000000000000000000000000007c027c03ac01a6
                   020000ab0200000000000000007c005f07000000000000000064005300
-                15           0 RESUME                   0
+                14           0 RESUME                   0
                
-                16           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                15           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                2 (address)
                             16 LOAD_GLOBAL              2 (str)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_JUMP_FORWARD_IF_FALSE    15 (to 74)
                
-                17          44 LOAD_GLOBAL              5 (NULL + to_checksum_address)
+                16          44 LOAD_GLOBAL              5 (NULL + to_checksum_address)
                             56 LOAD_FAST                2 (address)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               2 (address)
                
-                18     >>   74 LOAD_FAST                1 (chain)
+                17     >>   74 LOAD_FAST                1 (chain)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_chain)
                
-                19          88 LOAD_FAST                0 (self)
+                18          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                3 (_chain)
                            100 LOAD_ATTR                4 (w3)
                            110 LOAD_ATTR                5 (eth)
                            120 LOAD_METHOD              6 (contract)
                            142 LOAD_FAST                2 (address)
                            144 LOAD_FAST                3 (abi)
                            146 KW_NAMES                 1
@@ -281,209 +261,184 @@
                   ('abi',)
                names      ('isinstance', 'str', 'to_checksum_address', '_chain', 'w3', 'eth', 'contract', '_contract')
                varnames   ('self', 'chain', 'address', 'abi')
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       '__init__'
-               firstlineno 15
+               firstlineno 14
                lnotab 0x02012a011e010e01
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                21           0 RESUME                   0
+                20           0 RESUME                   0
                
-                23           2 LOAD_FAST                0 (self)
+                22           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_chain)
                             14 LOAD_ATTR                1 (w3)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_chain', 'w3')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'w3'
-               firstlineno 21
+               firstlineno 20
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-                25           0 RESUME                   0
+                24           0 RESUME                   0
                
-                27           2 LOAD_FAST                0 (self)
+                26           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_chain)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_chain',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'chain'
-               firstlineno 25
-               lnotab 0x0202
-            'Explorer'
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 1
-               flags     : 3
-               code 0x97007c006a0000000000000000006a0100000000000000005300
-                29           0 RESUME                   0
-               
-                31           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (_chain)
-                            14 LOAD_ATTR                1 (explorer)
-                            24 RETURN_VALUE
-               consts
-                  None
-               names      ('_chain', 'explorer')
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
-               name       'explorer'
-               firstlineno 29
+               firstlineno 24
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-                33           0 RESUME                   0
+                28           0 RESUME                   0
                
-                35           2 LOAD_FAST                0 (self)
+                30           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_contract',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'contract'
-               firstlineno 33
+               firstlineno 28
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                37           0 RESUME                   0
+                32           0 RESUME                   0
                
-                39           2 LOAD_FAST                0 (self)
+                34           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (address)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'address')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'address'
-               firstlineno 37
+               firstlineno 32
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                41           0 RESUME                   0
+                36           0 RESUME                   0
                
-                43           2 LOAD_FAST                0 (self)
+                38           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (abi)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'abi')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'abi'
-               firstlineno 41
+               firstlineno 36
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                45           0 RESUME                   0
+                40           0 RESUME                   0
                
-                47           2 LOAD_FAST                0 (self)
+                42           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (functions)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'functions')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'functions'
-               firstlineno 45
+               firstlineno 40
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                49           0 RESUME                   0
+                44           0 RESUME                   0
                
-                51           2 LOAD_FAST                0 (self)
+                46           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_contract)
                             14 LOAD_ATTR                1 (events)
                             24 RETURN_VALUE
                consts
                   None
                names      ('_contract', 'events')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
                name       'events'
-               firstlineno 49
+               firstlineno 44
                lnotab 0x0202
             None
             ('return', 'Chain')
-            ('return', 'Explorer')
-         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'property', 'Web3', 'w3', 'chain', 'explorer', 'Web3Contract', 'contract', 'address', 'abi', 'ContractFunctions', 'functions', 'ContractEvents', 'events')
+         names      ('__name__', '__module__', '__qualname__', 'ChecksumAddress', 'str', '__init__', 'property', 'Web3', 'w3', 'chain', 'Web3Contract', 'contract', 'address', 'abi', 'ContractFunctions', 'functions', 'ContractEvents', 'events')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
          name       'Contract'
-         firstlineno 14
+         firstlineno 13
          lnotab
-            0x0a01160602010aff0e010203020106ff0e010203020106ff0e01020302
-            010aff0e01020302010aff0e010203020104ff0e01020302010aff0e0102
-            0302010aff0e01
+            0x0a01160602010aff0e010203020106ff0e01020302010aff0e01020302
+            010aff0e010203020104ff0e01020302010aff0e01020302010aff0e01
       'Contract'
       None
-   names      ('typing', 'TYPE_CHECKING', 'eth_typing', 'ChecksumAddress', 'eth_utils', 'to_checksum_address', 'web3', 'Web3', 'web3.contract.contract', 'Contract', 'Web3Contract', 'ContractEvents', 'ContractFunctions', 'chain', 'Chain', 'explorer', 'Explorer')
+   names      ('typing', 'TYPE_CHECKING', 'eth_typing', 'ChecksumAddress', 'eth_utils', 'to_checksum_address', 'web3', 'Web3', 'web3.contract.contract', 'Contract', 'Web3Contract', 'ContractEvents', 'ContractFunctions', 'chain', 'Chain')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\contract\\contract.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c020c010c010c010c01100204010c010c03
+   lnotab 0x00ff02010c020c010c010c010c01100204010c03
```

### Comparing `better_web3-1.1.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-1.2.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-1.2.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.2.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/abi/erc1155.json` & `better_web3-1.2.0/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/abi/erc20.json` & `better_web3-1.2.0/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/abi/erc721.json` & `better_web3-1.2.0/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.2.0/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/contract.py` & `better_web3-1.2.0/better_web3/contract/contract.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from eth_utils import to_checksum_address
 from web3 import Web3
 from web3.contract.contract import Contract as Web3Contract
 from web3.contract.contract import ContractEvents, ContractFunctions
 
 if TYPE_CHECKING:
     from ..chain import Chain
-    from ..explorer import Explorer
 
 
 class Contract:
     def __init__(self, chain: "Chain", address: ChecksumAddress | str, abi):
         if isinstance(address, str):
             address = to_checksum_address(address)
         self._chain = chain
@@ -23,18 +22,14 @@
         return self._chain.w3
 
     @property
     def chain(self) -> "Chain":
         return self._chain
 
     @property
-    def explorer(self) -> "Explorer":
-        return self._chain.explorer
-
-    @property
     def contract(self) -> Web3Contract:
         return self._contract
 
     @property
     def address(self) -> str:
         return self._contract.address
```

### Comparing `better_web3-1.1.0/better_web3/contract/erc20.py` & `better_web3-1.2.0/better_web3/contract/erc20.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/erc721.py` & `better_web3-1.2.0/better_web3/contract/erc721.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/contract/multicall.py` & `better_web3-1.2.0/better_web3/contract/multicall.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.2.0/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-1.2.0/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files 19% similar despite different names*

#### Python bytecode

```diff
@@ -1,143 +1,175 @@
 magic:    0xa70d0d0a
-moddate:  0x3a679564 (Fri Jun 23 09:34:50 2023 UTC)
-files sz: 550
+moddate:  0x971c9c64 (Wed Jun 28 11:42:15 2023 UTC)
+files sz: 733
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a050100640465016405650664066501650719000000000000
-      0000006606640784045a08640865096409650565097a0700006604640a84
-      045a0a640b5300
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a040100640064046c056d065a060100640064056c076d085a08010002
+      0065066401ac06a6010000ab0100000000000000005a0964076502640865
+      0a64096502650b190000000000000000006606640a84045a0c640b650d64
+      0c6508650d7a0700006604640d84045a0e6409650d6602640e84045a0f64
+      015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Iterable',))
-                 6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (Iterable)
-                10 STORE_NAME               1 (Iterable)
-                12 POP_TOP
-   
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('islice',))
-                18 IMPORT_NAME              2 (itertools)
-                20 IMPORT_FROM              3 (islice)
-                22 STORE_NAME               3 (islice)
-                24 POP_TOP
-   
-     4          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('HexStr',))
-                30 IMPORT_NAME              4 (eth_typing)
-                32 IMPORT_FROM              5 (HexStr)
-                34 STORE_NAME               5 (HexStr)
-                36 POP_TOP
-   
-     7          38 LOAD_CONST               4 ('elements')
-                40 LOAD_NAME                1 (Iterable)
-                42 LOAD_CONST               5 ('n')
-                44 LOAD_NAME                6 (int)
-                46 LOAD_CONST               6 ('return')
-                48 LOAD_NAME                1 (Iterable)
-                50 LOAD_NAME                7 (list)
-                52 BINARY_SUBSCR
-                62 BUILD_TUPLE              6
-                64 LOAD_CONST               7 (<code object chunks, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 7>)
-                66 MAKE_FUNCTION            4 (annotations)
-                68 STORE_NAME               8 (chunks)
-   
-    21          70 LOAD_CONST               8 ('explorer_url')
-                72 LOAD_NAME                9 (str)
-                74 LOAD_CONST               9 ('tx_hash')
-                76 LOAD_NAME                5 (HexStr)
-                78 LOAD_NAME                9 (str)
-                80 BINARY_OP                7 (|)
-                84 BUILD_TUPLE              4
-                86 LOAD_CONST              10 (<code object link_by_tx_hash, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 21>)
-                88 MAKE_FUNCTION            4 (annotations)
-                90 STORE_NAME              10 (link_by_tx_hash)
-                92 LOAD_CONST              11 (None)
-                94 RETURN_VALUE
+                 4 LOAD_CONST               1 (None)
+                 6 IMPORT_NAME              0 (json)
+                 8 STORE_NAME               0 (json)
+   
+     2          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               2 (('Iterable',))
+                14 IMPORT_NAME              1 (typing)
+                16 IMPORT_FROM              2 (Iterable)
+                18 STORE_NAME               2 (Iterable)
+                20 POP_TOP
+   
+     3          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('islice',))
+                26 IMPORT_NAME              3 (itertools)
+                28 IMPORT_FROM              4 (islice)
+                30 STORE_NAME               4 (islice)
+                32 POP_TOP
+   
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               4 (('lru_cache',))
+                38 IMPORT_NAME              5 (functools)
+                40 IMPORT_FROM              6 (lru_cache)
+                42 STORE_NAME               6 (lru_cache)
+                44 POP_TOP
+   
+     6          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               5 (('HexStr',))
+                50 IMPORT_NAME              7 (eth_typing)
+                52 IMPORT_FROM              8 (HexStr)
+                54 STORE_NAME               8 (HexStr)
+                56 POP_TOP
+   
+     9          58 PUSH_NULL
+                60 LOAD_NAME                6 (lru_cache)
+                62 LOAD_CONST               1 (None)
+                64 KW_NAMES                 6
+                66 PRECALL                  1
+                70 CALL                     1
+                80 STORE_NAME               9 (cache)
+   
+    12          82 LOAD_CONST               7 ('elements')
+                84 LOAD_NAME                2 (Iterable)
+                86 LOAD_CONST               8 ('n')
+                88 LOAD_NAME               10 (int)
+                90 LOAD_CONST               9 ('return')
+                92 LOAD_NAME                2 (Iterable)
+                94 LOAD_NAME               11 (list)
+                96 BINARY_SUBSCR
+               106 BUILD_TUPLE              6
+               108 LOAD_CONST              10 (<code object chunks, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 12>)
+               110 MAKE_FUNCTION            4 (annotations)
+               112 STORE_NAME              12 (chunks)
+   
+    26         114 LOAD_CONST              11 ('explorer_url')
+               116 LOAD_NAME               13 (str)
+               118 LOAD_CONST              12 ('tx_hash')
+               120 LOAD_NAME                8 (HexStr)
+               122 LOAD_NAME               13 (str)
+               124 BINARY_OP                7 (|)
+               128 BUILD_TUPLE              4
+               130 LOAD_CONST              13 (<code object link_by_tx_hash, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 26>)
+               132 MAKE_FUNCTION            4 (annotations)
+               134 STORE_NAME              14 (link_by_tx_hash)
+   
+    30         136 LOAD_CONST               9 ('return')
+               138 LOAD_NAME               13 (str)
+               140 BUILD_TUPLE              2
+               142 LOAD_CONST              14 (<code object to_json, file "H:\Мой диск\Projects\Python\better_web3\better_web3\utils\other.py", line 30>)
+               144 MAKE_FUNCTION            4 (annotations)
+               146 STORE_NAME              15 (to_json)
+               148 LOAD_CONST               1 (None)
+               150 RETURN_VALUE
    consts
       0
+      None
       ('Iterable',)
       ('islice',)
+      ('lru_cache',)
       ('HexStr',)
+      ('maxsize',)
       'elements'
       'n'
       'return'
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 6
          flags     : 35
          code
             0x4b00010097007401000000000000000000007c00a6010000ab01000000
             00000000007d020900740300000000000000000000740500000000000000
             0000007c027c01a6020000ab020000000000000000a6010000ab01000000
             00000000007d037c037302640253007c035600970101008c26
-           7           0 RETURN_GENERATOR
+          12           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-          13           6 LOAD_GLOBAL              1 (NULL + iter)
+          18           6 LOAD_GLOBAL              1 (NULL + iter)
                       18 LOAD_FAST                0 (elements)
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_FAST               2 (it)
          
-          14          36 NOP
+          19          36 NOP
          
-          15     >>   38 LOAD_GLOBAL              3 (NULL + list)
+          20     >>   38 LOAD_GLOBAL              3 (NULL + list)
                       50 LOAD_GLOBAL              5 (NULL + islice)
                       62 LOAD_FAST                2 (it)
                       64 LOAD_FAST                1 (n)
                       66 PRECALL                  2
                       70 CALL                     2
                       80 PRECALL                  1
                       84 CALL                     1
                       94 STORE_FAST               3 (chunk)
          
-          16          96 LOAD_FAST                3 (chunk)
+          21          96 LOAD_FAST                3 (chunk)
                       98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
          
-          17         100 LOAD_CONST               2 (None)
+          22         100 LOAD_CONST               2 (None)
                      102 RETURN_VALUE
          
-          18     >>  104 LOAD_FAST                3 (chunk)
+          23     >>  104 LOAD_FAST                3 (chunk)
                      106 YIELD_VALUE
                      108 RESUME                   1
                      110 POP_TOP
          
-          14         112 JUMP_BACKWARD           38 (to 38)
+          19         112 JUMP_BACKWARD           38 (to 38)
          consts
             '\n    :param elements: Iterable\n    :param n: Number per chunk\n    :return: Yield successive n-sized chunks from elements\n    '
             True
             None
          names      ('iter', 'list', 'islice')
          varnames   ('elements', 'n', 'it', 'chunk')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
          name       'chunks'
-         firstlineno 7
+         firstlineno 12
          lnotab 0x06061e0102013a010401040108fc
       'explorer_url'
       'tx_hash'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code 0x97007c009b0064017c019b009d035300
-          21           0 RESUME                   0
+          26           0 RESUME                   0
          
-          22           2 LOAD_FAST                0 (explorer_url)
+          27           2 LOAD_FAST                0 (explorer_url)
                        4 FORMAT_VALUE             0
                        6 LOAD_CONST               1 ('/tx/')
                        8 LOAD_FAST                1 (tx_hash)
                       10 FORMAT_VALUE             0
                       12 BUILD_STRING             3
                       14 RETURN_VALUE
          consts
@@ -145,18 +177,49 @@
             '/tx/'
          names      ()
          varnames   ('explorer_url', 'tx_hash')
          freevars   ()
          cellvars   ()
          filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
          name       'link_by_tx_hash'
-         firstlineno 21
+         firstlineno 26
          lnotab 0x0201
-      None
-   names      ('typing', 'Iterable', 'itertools', 'islice', 'eth_typing', 'HexStr', 'int', 'list', 'chunks', 'str', 'link_by_tx_hash')
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 5
+         flags     : 3
+         code
+            0x97007401000000000000000000006a0100000000000000007c00640164
+            02ac03a6030000ab0300000000000000005300
+          30           0 RESUME                   0
+         
+          31           2 LOAD_GLOBAL              1 (NULL + json)
+                      14 LOAD_ATTR                1 (dumps)
+                      24 LOAD_FAST                0 (obj)
+                      26 LOAD_CONST               1 ((',', ':'))
+                      28 LOAD_CONST               2 (True)
+                      30 KW_NAMES                 3
+                      32 PRECALL                  3
+                      36 CALL                     3
+                      46 RETURN_VALUE
+         consts
+            None
+            (',', ':')
+            True
+            ('separators', 'ensure_ascii')
+         names      ('json', 'dumps')
+         varnames   ('obj',)
+         freevars   ()
+         cellvars   ()
+         filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
+         name       'to_json'
+         firstlineno 30
+         lnotab 0x0201
+   names      ('json', 'typing', 'Iterable', 'itertools', 'islice', 'functools', 'lru_cache', 'eth_typing', 'HexStr', 'cache', 'int', 'list', 'chunks', 'str', 'link_by_tx_hash', 'to_json')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'H:\\Мой диск\\Projects\\Python\\better_web3\\better_web3\\utils\\other.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c020c03200e
+   lnotab 0x00ff020108010c010c010c020c031803200e1604
```

### Comparing `better_web3-1.1.0/better_web3/utils/eth.py` & `better_web3-1.2.0/better_web3/utils/eth.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.1.0/better_web3/utils/other.py` & `better_web3-1.2.0/better_web3/utils/other.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import json
 from typing import Iterable
 from itertools import islice
+from functools import lru_cache
 
 from eth_typing import HexStr
 
 
+cache = lru_cache(maxsize=None)
+
+
 def chunks(elements: Iterable, n: int) -> Iterable[list]:
     """
     :param elements: Iterable
     :param n: Number per chunk
     :return: Yield successive n-sized chunks from elements
     """
     it = iter(elements)
@@ -16,7 +21,11 @@
         if not chunk:
             return
         yield chunk
 
 
 def link_by_tx_hash(explorer_url: str, tx_hash: HexStr | str):
     return f"{explorer_url}/tx/{tx_hash}"
+
+
+def to_json(obj) -> str:
+    return json.dumps(obj, separators=(',', ':'), ensure_ascii=True)
```

### Comparing `better_web3-1.1.0/PKG-INFO` & `better_web3-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.1.0
+Version: 1.2.0
 Summary: Chain, Explorer, Contracts(Multicall, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
```

