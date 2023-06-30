# Comparing `tmp/blockit-0.0.1.tar.gz` & `tmp/blockit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockit-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "blockit-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `blockit-0.0.1.tar` & `blockit-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.1/.dockerignore
--rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.1/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.1/Dockerfile
--rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.1/Hillciph.pdf
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.1/LICENSE
--rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.1/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.1/README.md
--rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.1/ascii-table.png
--rw-r--r--   0        0        0       22 2023-06-29 14:07:35.157325 blockit-0.0.1/blockit/__init__.py
--rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.1/blockit/__main__.py
--rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.1/blockit/cli.py
--rw-r--r--   0        0        0    22306 2023-06-29 13:56:53.891309 blockit-0.0.1/blockit/crypto_algorithms.py
--rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.1/docker-compose.yml
--rw-r--r--   0        0        0     2269 2023-06-29 14:06:17.584638 blockit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      121 2023-06-29 09:17:08.018647 blockit-0.0.1/requirements.txt
--rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.1/setup.cfg
--rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.1/test_build.py
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 blockit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.2/.dockerignore
+-rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.2/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.2/Dockerfile
+-rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.2/Hillciph.pdf
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.2/LICENSE
+-rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.2/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.2/README.md
+-rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.2/ascii-table.png
+-rw-r--r--   0        0        0       22 2023-06-30 03:36:29.437662 blockit-0.0.2/blockit/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.2/blockit/__main__.py
+-rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.2/blockit/cli.py
+-rw-r--r--   0        0        0    23430 2023-06-30 03:33:20.021033 blockit-0.0.2/blockit/crypto_algorithms.py
+-rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.2/blockit/reverse_encryption_api.py
+-rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.2/docker-compose.yml
+-rw-r--r--   0        0        0     2269 2023-06-29 14:06:17.584638 blockit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-06-30 02:44:18.097885 blockit-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.2/setup.cfg
+-rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.2/test_build.py
+-rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 blockit-0.0.2/PKG-INFO
```

### Comparing `blockit-0.0.1/.gitignore` & `blockit-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/Dockerfile` & `blockit-0.0.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/Hillciph.pdf` & `blockit-0.0.2/Hillciph.pdf`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/LICENSE` & `blockit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/ascii-table.png` & `blockit-0.0.2/ascii-table.png`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/blockit/cli.py` & `blockit-0.0.2/blockit/cli.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/blockit/crypto_algorithms.py` & `blockit-0.0.2/blockit/crypto_algorithms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import array
 import string
 from abc import ABC, abstractmethod
 
+import httpx
+
 
 class CryptoAlgorithm(ABC):
     @abstractmethod
     def encrypt(self, text):
         ...
 
     @abstractmethod
@@ -703,14 +705,34 @@
             # Multiply the digraph vector by the inverse key matrix.
             digraph_plaintext: list = self.matrix_multiply(digraph_vector, self.inv_key)
             plain_text[i : i + self.digraph_size] = self.convert_to_block(digraph_plaintext)
 
         return "".join(plain_text)
 
 
+class ReverseEncryption(CryptoAlgorithm):
+    """
+    Reverse Encryption Algorithm.
+    """
+
+    def __init__(self, encrypt_url: str, decrypt_url: str):
+        self.encrypt_url = encrypt_url or "http://backendtask.robustastudio.com/encode"
+        self.decrypt_url = decrypt_url or "http://backendtask.robustastudio.com/decode"
+
+    def encrypt(self, plain_text: str) -> str:
+        headers = {"Content-Type": "application/json"}
+        response = httpx.post(self.encrypt_url, headers=headers, json={"text": plain_text})
+        return response.json().get("encoded_text", "")
+
+    def decrypt(self, cipher_text: str) -> str:
+        headers = {"Content-Type": "application/json"}
+        response = httpx.post(self.encrypt_url, headers=headers, json={"text": cipher_text})
+        return response.json().get("decoded_text", "")
+
+
 class CryptoAlgorithmFactory:
     """
     Factory class for dynamically creating crypto algorithm instances.
 
     This factory class provides a convenient way to create different crypto algorithm instances
     """
 
@@ -722,9 +744,13 @@
         - CryptoAlgorithm: An instance of the specified crypto algorithm.
         """
         if algorithm_name == "shift":
             shift = int(kwargs.get("--shift", 3))
             return ShiftEncryption(shift)
         elif algorithm_name == "matrix":
             return MatrixEncryption()
+        elif algorithm_name == "reverse":
+            encrypt_url = "https://encryption-api-five.vercel.app/encode"
+            decrypt_url = "https://encryption-api-five.vercel.app/decode"
+            return ReverseEncryption(encrypt_url=encrypt_url, decrypt_url=decrypt_url)
         else:
             raise ValueError(f"Invalid algorithm name: {algorithm_name}")
```

### Comparing `blockit-0.0.1/pyproject.toml` & `blockit-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blockit-0.0.1/PKG-INFO` & `blockit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockit
-Version: 0.0.1
+Version: 0.0.2
 Summary: blockit - cli tool for encrypting and decrypting strings
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

