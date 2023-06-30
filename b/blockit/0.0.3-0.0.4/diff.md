# Comparing `tmp/blockit-0.0.3.tar.gz` & `tmp/blockit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockit-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "blockit-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `blockit-0.0.3.tar` & `blockit-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.3/.dockerignore
--rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.3/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.3/Dockerfile
--rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.3/Hillciph.pdf
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.3/LICENSE
--rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.3/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.3/README.md
--rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.3/ascii-table.png
--rw-r--r--   0        0        0       22 2023-06-30 03:43:22.591335 blockit-0.0.3/blockit/__init__.py
--rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.3/blockit/__main__.py
--rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.3/blockit/cli.py
--rw-r--r--   0        0        0    23430 2023-06-30 03:33:20.021033 blockit-0.0.3/blockit/crypto_algorithms.py
--rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.3/blockit/reverse_encryption_api.py
--rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.3/docker-compose.yml
--rw-r--r--   0        0        0     2292 2023-06-30 03:42:57.591831 blockit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      194 2023-06-30 02:44:18.097885 blockit-0.0.3/requirements.txt
--rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.3/setup.cfg
--rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.3/test_build.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 blockit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.4/.dockerignore
+-rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.4/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.4/Dockerfile
+-rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.4/Hillciph.pdf
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.4/LICENSE
+-rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.4/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.4/README.md
+-rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.4/ascii-table.png
+-rw-r--r--   0        0        0       22 2023-06-30 03:51:35.013167 blockit-0.0.4/blockit/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.4/blockit/__main__.py
+-rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.4/blockit/cli.py
+-rw-r--r--   0        0        0    23430 2023-06-30 03:50:59.577444 blockit-0.0.4/blockit/crypto_algorithms.py
+-rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.4/blockit/reverse_encryption_api.py
+-rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.4/docker-compose.yml
+-rw-r--r--   0        0        0     2292 2023-06-30 03:42:57.591831 blockit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-06-30 02:44:18.097885 blockit-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.4/setup.cfg
+-rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.4/test_build.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 blockit-0.0.4/PKG-INFO
```

### Comparing `blockit-0.0.3/.gitignore` & `blockit-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/Dockerfile` & `blockit-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/Hillciph.pdf` & `blockit-0.0.4/Hillciph.pdf`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/LICENSE` & `blockit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/ascii-table.png` & `blockit-0.0.4/ascii-table.png`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/blockit/cli.py` & `blockit-0.0.4/blockit/cli.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/blockit/crypto_algorithms.py` & `blockit-0.0.4/blockit/crypto_algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,15 +721,15 @@
     def encrypt(self, plain_text: str) -> str:
         headers = {"Content-Type": "application/json"}
         response = httpx.post(self.encrypt_url, headers=headers, json={"text": plain_text})
         return response.json().get("encoded_text", "")
 
     def decrypt(self, cipher_text: str) -> str:
         headers = {"Content-Type": "application/json"}
-        response = httpx.post(self.encrypt_url, headers=headers, json={"text": cipher_text})
+        response = httpx.post(self.decrypt_url, headers=headers, json={"text": cipher_text})
         return response.json().get("decoded_text", "")
 
 
 class CryptoAlgorithmFactory:
     """
     Factory class for dynamically creating crypto algorithm instances.
```

### Comparing `blockit-0.0.3/blockit/reverse_encryption_api.py` & `blockit-0.0.4/blockit/reverse_encryption_api.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/pyproject.toml` & `blockit-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blockit-0.0.3/PKG-INFO` & `blockit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockit
-Version: 0.0.3
+Version: 0.0.4
 Summary: blockit - cli tool for encrypting and decrypting strings
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

