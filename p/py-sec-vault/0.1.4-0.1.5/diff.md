# Comparing `tmp/py_sec_vault-0.1.4.tar.gz` & `tmp/py_sec_vault-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.1.4.tar", max compression
+gzip compressed data, was "py_sec_vault-0.1.5.tar", max compression
```

## Comparing `py_sec_vault-0.1.4.tar` & `py_sec_vault-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.4/LICENSE
--rw-r--r--   0        0        0     3141 2023-06-30 07:39:34.665800 py_sec_vault-0.1.4/README.md
--rw-r--r--   0        0        0      916 2023-06-30 08:14:07.660265 py_sec_vault-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      146 2023-06-28 21:28:04.863203 py_sec_vault-0.1.4/vault/__init__.py
--rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.4/vault/client.py
--rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.4/vault/config.py
--rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.4/vault/exceptions.py
--rw-r--r--   0        0        0      814 2023-06-30 07:45:59.221556 py_sec_vault-0.1.4/vault/utils.py
--rw-r--r--   0        0        0     3609 2023-06-30 08:12:09.227387 py_sec_vault-0.1.4/vault/vault.py
--rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 py_sec_vault-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3347 2023-06-30 08:34:41.532823 py_sec_vault-0.1.5/README.md
+-rw-r--r--   0        0        0      916 2023-06-30 08:28:08.979442 py_sec_vault-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-06-30 08:25:36.575393 py_sec_vault-0.1.5/vault/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.5/vault/client.py
+-rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.5/vault/config.py
+-rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.5/vault/exceptions.py
+-rw-r--r--   0        0        0     1851 2023-06-30 08:32:06.011213 py_sec_vault-0.1.5/vault/utils.py
+-rw-r--r--   0        0        0     3609 2023-06-30 08:12:09.227387 py_sec_vault-0.1.5/vault/vault.py
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 py_sec_vault-0.1.5/PKG-INFO
```

### Comparing `py_sec_vault-0.1.4/LICENSE` & `py_sec_vault-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.4/README.md` & `py_sec_vault-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -72,26 +72,30 @@
 
 # Retrieving a secret from the vault (and raising an exception if not found)
 from_vault("API_TOKEN")
 ```
 
 To retrieve all secrets from the vault, you can use the following code:
 ```python
-from vault import Vault
+from vault import Vault, from_env_or_vault
 
 # This will connect to the vault based on the environment variables;
 vault = Vault()
 
 # Prints the keys in the vault, validating if the vault is initialized;
 print(vault.keys) 
 
 # Retrieving a secret from the vault, or None if not found
-my_optional_secret = vault.get("MY_SECRET")
+my_secret = vault.get("MY_SECRET")
+
+# Passing an instance of Vault to the from_env_or_vault function,
+# so it doesn't need to connect to the vault again;
+my_variable = from_env_or_vault("MY_VARIABLE", default="admin", vault=vault)
 ```
 
 
 ## Next steps
-- [X] Make sure the vault is not initialized every time, but only when needed
 - [ ] On init load multiple paths/engines
 - [ ] Add support for other auth methods
 - [ ] Phase out the use of hvac and use requests instead
-- [ ] Implementation of from_vault_or_env
+- [X] Make sure the vault is not initialized every time, but only when needed
+- [X] Implementation of from_vault_or_env
```

### Comparing `py_sec_vault-0.1.4/pyproject.toml` & `py_sec_vault-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-sec-vault"
-version = "0.1.4"
+version = "0.1.5"
 description = "Vault implementation in python software (Hashicorp)"
 authors = ["CISolutions B.V. <info@cisolutions.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vault"}]
 homepage = "https://github.com/cisolutions-nl/py-sec-vault"
 repository = "https://github.com/cisolutions-nl/py-sec-vault"
```

### Comparing `py_sec_vault-0.1.4/vault/vault.py` & `py_sec_vault-0.1.5/vault/vault.py`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.4/PKG-INFO` & `py_sec_vault-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sec-vault
-Version: 0.1.4
+Version: 0.1.5
 Summary: Vault implementation in python software (Hashicorp)
 Home-page: https://github.com/cisolutions-nl/py-sec-vault
 License: MIT
 Keywords: vault,hashicorp,security
 Author: CISolutions B.V.
 Author-email: info@cisolutions.nl
 Requires-Python: >=3.9
@@ -96,27 +96,31 @@
 
 # Retrieving a secret from the vault (and raising an exception if not found)
 from_vault("API_TOKEN")
 ```
 
 To retrieve all secrets from the vault, you can use the following code:
 ```python
-from vault import Vault
+from vault import Vault, from_env_or_vault
 
 # This will connect to the vault based on the environment variables;
 vault = Vault()
 
 # Prints the keys in the vault, validating if the vault is initialized;
 print(vault.keys) 
 
 # Retrieving a secret from the vault, or None if not found
-my_optional_secret = vault.get("MY_SECRET")
+my_secret = vault.get("MY_SECRET")
+
+# Passing an instance of Vault to the from_env_or_vault function,
+# so it doesn't need to connect to the vault again;
+my_variable = from_env_or_vault("MY_VARIABLE", default="admin", vault=vault)
 ```
 
 
 ## Next steps
-- [X] Make sure the vault is not initialized every time, but only when needed
 - [ ] On init load multiple paths/engines
 - [ ] Add support for other auth methods
 - [ ] Phase out the use of hvac and use requests instead
-- [ ] Implementation of from_vault_or_env
+- [X] Make sure the vault is not initialized every time, but only when needed
+- [X] Implementation of from_vault_or_env
```

