# Comparing `tmp/py_sec_vault-0.1.3.tar.gz` & `tmp/py_sec_vault-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.1.3.tar", max compression
+gzip compressed data, was "py_sec_vault-0.1.4.tar", max compression
```

## Comparing `py_sec_vault-0.1.3.tar` & `py_sec_vault-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.3/LICENSE
--rw-r--r--   0        0        0     3141 2023-06-30 07:39:34.665800 py_sec_vault-0.1.3/README.md
--rw-r--r--   0        0        0      916 2023-06-30 07:58:18.740885 py_sec_vault-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      146 2023-06-28 21:28:04.863203 py_sec_vault-0.1.3/vault/__init__.py
--rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.3/vault/client.py
--rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.3/vault/config.py
--rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.3/vault/exceptions.py
--rw-r--r--   0        0        0      814 2023-06-30 07:45:59.221556 py_sec_vault-0.1.3/vault/utils.py
--rw-r--r--   0        0        0     3615 2023-06-30 07:57:19.660254 py_sec_vault-0.1.3/vault/vault.py
--rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 py_sec_vault-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3141 2023-06-30 07:39:34.665800 py_sec_vault-0.1.4/README.md
+-rw-r--r--   0        0        0      916 2023-06-30 08:14:07.660265 py_sec_vault-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-06-28 21:28:04.863203 py_sec_vault-0.1.4/vault/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.4/vault/client.py
+-rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.4/vault/config.py
+-rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.4/vault/exceptions.py
+-rw-r--r--   0        0        0      814 2023-06-30 07:45:59.221556 py_sec_vault-0.1.4/vault/utils.py
+-rw-r--r--   0        0        0     3609 2023-06-30 08:12:09.227387 py_sec_vault-0.1.4/vault/vault.py
+-rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 py_sec_vault-0.1.4/PKG-INFO
```

### Comparing `py_sec_vault-0.1.3/LICENSE` & `py_sec_vault-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.3/README.md` & `py_sec_vault-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.3/pyproject.toml` & `py_sec_vault-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-sec-vault"
-version = "0.1.3"
+version = "0.1.4"
 description = "Vault implementation in python software (Hashicorp)"
 authors = ["CISolutions B.V. <info@cisolutions.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vault"}]
 homepage = "https://github.com/cisolutions-nl/py-sec-vault"
 repository = "https://github.com/cisolutions-nl/py-sec-vault"
```

### Comparing `py_sec_vault-0.1.3/vault/utils.py` & `py_sec_vault-0.1.4/vault/utils.py`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.3/vault/vault.py` & `py_sec_vault-0.1.4/vault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             )
         except Forbidden:
             raise Exception(
                 f"Your client does not have access to the path '{vault_path}'."
             )
 
         variables = response["data"]["data"]
-        logger.info(f"Fetched {len(self._variables.keys())} secret(s) from vault.")
+        logger.info(f"Fetched {len(variables.keys())} secret(s) from vault.")
         return variables
 
     def get(self, key: str, default: str = None) -> Optional[str]:
         try:
             return self[key]
         except KeyError:
             return default
```

### Comparing `py_sec_vault-0.1.3/PKG-INFO` & `py_sec_vault-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sec-vault
-Version: 0.1.3
+Version: 0.1.4
 Summary: Vault implementation in python software (Hashicorp)
 Home-page: https://github.com/cisolutions-nl/py-sec-vault
 License: MIT
 Keywords: vault,hashicorp,security
 Author: CISolutions B.V.
 Author-email: info@cisolutions.nl
 Requires-Python: >=3.9
```

