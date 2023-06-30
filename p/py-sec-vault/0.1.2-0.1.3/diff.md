# Comparing `tmp/py_sec_vault-0.1.2.tar.gz` & `tmp/py_sec_vault-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.1.2.tar", max compression
+gzip compressed data, was "py_sec_vault-0.1.3.tar", max compression
```

## Comparing `py_sec_vault-0.1.2.tar` & `py_sec_vault-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.2/LICENSE
--rw-r--r--   0        0        0     2257 2023-06-28 21:47:56.574571 py_sec_vault-0.1.2/README.md
--rw-r--r--   0        0        0      916 2023-06-28 21:58:05.586419 py_sec_vault-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      146 2023-06-28 21:28:04.863203 py_sec_vault-0.1.2/vault/__init__.py
--rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.2/vault/client.py
--rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.2/vault/config.py
--rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.2/vault/exceptions.py
--rw-r--r--   0        0        0      818 2023-06-28 21:56:34.160025 py_sec_vault-0.1.2/vault/utils.py
--rw-r--r--   0        0        0     2956 2023-06-28 21:43:57.627214 py_sec_vault-0.1.2/vault/vault.py
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 py_sec_vault-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3141 2023-06-30 07:39:34.665800 py_sec_vault-0.1.3/README.md
+-rw-r--r--   0        0        0      916 2023-06-30 07:58:18.740885 py_sec_vault-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-06-28 21:28:04.863203 py_sec_vault-0.1.3/vault/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-28 21:21:02.453186 py_sec_vault-0.1.3/vault/client.py
+-rw-r--r--   0        0        0      386 2023-06-28 21:44:58.555190 py_sec_vault-0.1.3/vault/config.py
+-rw-r--r--   0        0        0      206 2023-06-15 22:26:13.116181 py_sec_vault-0.1.3/vault/exceptions.py
+-rw-r--r--   0        0        0      814 2023-06-30 07:45:59.221556 py_sec_vault-0.1.3/vault/utils.py
+-rw-r--r--   0        0        0     3615 2023-06-30 07:57:19.660254 py_sec_vault-0.1.3/vault/vault.py
+-rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 py_sec_vault-0.1.3/PKG-INFO
```

### Comparing `py_sec_vault-0.1.2/LICENSE` & `py_sec_vault-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.1.2/README.md` & `py_sec_vault-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -19,52 +19,79 @@
 
 ## Installation
 
 ```bash
 pip install py-sec-vault
 ```
 
-After this you should set environment variables to connect to the vault instance.
-
-```
-export VAULT_HOST=http://localhost:8200/
-export VAULT_AUTH_METHOD=approle|token
-export VAULT_ENGINE_NAME=<my_engine_name>
-export VAULT_ROLE_ID=<my_vault_id>
-export VAULT_SECRET_ID=<my_vauld_secret>
-export VAULT_PATH=<my_vault_path>
-```
-
 ## Usage
 
 ```python
 from vault import Vault
 
-vault = Vault()
+vault = Vault(
+    host="http://localhost:8200/",
+    auth_method="approle",
+    engine_name="my_engine_name",
+    path="my_vault_path",
+    token="my_vault_token",
+)
+
+# Prints the keys in the vault, validating if the vault is initialized;
+print(vault.keys) 
 
 # Retrieving a secret from the vault, or None if not found
 my_optional_secret = vault.get("MY_SECRET")
 
 # Retrieving a secret from the vault (and raising an exception if not found)
 my_secret = vault["MY_SECRET"]
 ```
 
 ## Usage with environment variables
+To make the vault work with environment variables, you can use the following code:
+
+First, you need to set the environment variables for the vault:
+```
+export VAULT_HOST=http://localhost:8200/
+export VAULT_AUTH_METHOD=approle|token
+export VAULT_ENGINE_NAME=<my_engine_name>
+export VAULT_ROLE_ID=<my_vault_id>
+export VAULT_SECRET_ID=<my_vauld_secret>
+export VAULT_PATH=<my_vault_path>
+```
+
+Second, you can use the following code to retrieve the secrets from the vault or environment variables:
 ```python
 from vault import from_env_or_vault, from_vault
 
 # NB: These functions will instantiate a Vault object and retrieve the secret from the vault
-# resulting in a performance penalty if used in a loop; in that case, instantiate a Vault object.
+# resulting in a performance penalty if used in a loop. Alternatively, you can instantiate a Vault object
+# once and use the get method to retrieve the secrets (next example).
 
 # Retrieving a secret from the vault or environment variable or using a default value
 from_env_or_vault("DB_PASSWORD", default="admin")
 
 # Retrieving a secret from the vault (and raising an exception if not found)
 from_vault("API_TOKEN")
 ```
 
+To retrieve all secrets from the vault, you can use the following code:
+```python
+from vault import Vault
+
+# This will connect to the vault based on the environment variables;
+vault = Vault()
+
+# Prints the keys in the vault, validating if the vault is initialized;
+print(vault.keys) 
+
+# Retrieving a secret from the vault, or None if not found
+my_optional_secret = vault.get("MY_SECRET")
+```
+
+
 ## Next steps
-- [ ] Make sure the vault is not initialized every time, but only when needed
+- [X] Make sure the vault is not initialized every time, but only when needed
 - [ ] On init load multiple paths/engines
 - [ ] Add support for other auth methods
 - [ ] Phase out the use of hvac and use requests instead
 - [ ] Implementation of from_vault_or_env
```

### Comparing `py_sec_vault-0.1.2/pyproject.toml` & `py_sec_vault-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-sec-vault"
-version = "0.1.2"
+version = "0.1.3"
 description = "Vault implementation in python software (Hashicorp)"
 authors = ["CISolutions B.V. <info@cisolutions.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vault"}]
 homepage = "https://github.com/cisolutions-nl/py-sec-vault"
 repository = "https://github.com/cisolutions-nl/py-sec-vault"
```

### Comparing `py_sec_vault-0.1.2/vault/utils.py` & `py_sec_vault-0.1.3/vault/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Optional
 
-from vault import Vault
+from . import Vault
 
 
 def from_env_or_vault(
     key: str,
     default: Optional[str] = None,
 ) -> Optional[str]:
     """
```

### Comparing `py_sec_vault-0.1.2/vault/vault.py` & `py_sec_vault-0.1.3/vault/vault.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from functools import lru_cache
-from typing import Mapping, Optional
+from typing import Mapping, Optional, Tuple
 
+from hvac import Client
 from hvac.exceptions import InvalidPath, Forbidden
 
-from vault import config
-from vault.client import get_client
-from vault.exceptions import VaultClientImproperlyConfiguredError
+from . import config
+from .client import get_client
+from .exceptions import VaultClientImproperlyConfiguredError
 
 logger = logging.getLogger(__name__)
 
 
 def _validate_vault_config(
     auth_method: str,
     token: Optional[str] = None,
@@ -28,71 +29,86 @@
     if auth_method == "approle":
         if not role_id or not secret_id:
             raise VaultClientImproperlyConfiguredError(
                 "Missing variables VAULT_ROLE_ID and/or VAULT_SECRET_ID. "
                 "Cannot authenticate with vault using approle."
             )
         return True
-    return False
-
-
-@lru_cache
-def _fetch_variables() -> Mapping[str, str]:
-    try:
-        _validate_vault_config(
-            auth_method=config.VAULT_AUTH_METHOD,
-            token=config.VAULT_TOKEN,
-            role_id=config.VAULT_ROLE_ID,
-            secret_id=config.VAULT_SECRET_ID,
-        )
-    except VaultClientImproperlyConfiguredError as e:
-        logger.exception(e, exc_info=True)
-        return dict()
-
-    logger.debug("About to fetch credentials from vault.")
-    if not (
-        client := get_client(
-            auth_method=config.VAULT_AUTH_METHOD,
-            host=config.VAULT_HOST,
-            token=config.VAULT_TOKEN,
-            role_id=config.VAULT_ROLE_ID,
-            secret_id=config.VAULT_SECRET_ID,
-        )
-    ):
-        raise ConnectionError("Could not connect to vault.")
-
-    logger.debug(f"Connected to vault with auth method {config.VAULT_AUTH_METHOD}.")
-    try:
-        response = client.secrets.kv.v2.read_secret(
-            mount_point=config.VAULT_ENGINE_NAME,
-            path=config.VAULT_PATH,
-        )
-    except InvalidPath:
-        raise Exception(
-            f"Your path ({config.VAULT_PATH}) has not been created yet "
-            f"or there are no credentials in it."
-        )
-    except Forbidden:
-        raise Exception(
-            f"Your {config.VAULT_AUTH_METHOD} does not have access to the path "
-            f"'{config.VAULT_PATH}'."
-        )
-
-    secrets = response["data"]["data"]
-    logger.info(f"Fetched {len(secrets.keys())} secret(s) from vault.")
-    return secrets
+    raise VaultClientImproperlyConfiguredError("Missing variable VAULT_AUTH_METHOD.")
 
 
 class Vault:
     _variables: Mapping[str, str] = dict()
+    _client: Optional[Client] = None
+
+    def __init__(
+        self,
+        host: str = config.VAULT_HOST,
+        engine_name: str = config.VAULT_ENGINE_NAME,
+        path: str = config.VAULT_PATH,
+        auth_method: str = config.VAULT_AUTH_METHOD,
+        token: Optional[str] = config.VAULT_TOKEN,
+        role_id: Optional[str] = config.VAULT_ROLE_ID,
+        secret_id: Optional[str] = config.VAULT_SECRET_ID,
+    ) -> None:
+        try:
+            _validate_vault_config(
+                auth_method=auth_method,
+                token=token,
+                role_id=role_id,
+                secret_id=secret_id,
+            )
+        except VaultClientImproperlyConfiguredError as e:
+            logger.exception(e, exc_info=True)
+            return
+
+        self._client = get_client(
+            auth_method=auth_method,
+            host=host,
+            token=token,
+            role_id=role_id,
+            secret_id=secret_id,
+        )
+        if not self._client:
+            raise ConnectionError(
+                "Could not connect to vault. Check your vault configuration."
+            )
 
-    def __init__(self):
-        self._variables = _fetch_variables()
+        logger.debug(f"Connected to vault with auth method {auth_method}.")
+        self._variables = self._fetch_variables(
+            engine_name=engine_name,
+            vault_path=path,
+        )
 
     def __getitem__(self, key: str) -> Optional[str]:
         return self._variables[key]
 
+    @lru_cache
+    def _fetch_variables(self, engine_name: str, vault_path: str) -> Mapping[str, str]:
+        try:
+            response = self._client.secrets.kv.v2.read_secret(
+                mount_point=engine_name,
+                path=vault_path,
+            )
+        except InvalidPath:
+            raise Exception(
+                f"Your path ({vault_path}) has not been created yet "
+                f"or there are no credentials in it."
+            )
+        except Forbidden:
+            raise Exception(
+                f"Your client does not have access to the path '{vault_path}'."
+            )
+
+        variables = response["data"]["data"]
+        logger.info(f"Fetched {len(self._variables.keys())} secret(s) from vault.")
+        return variables
+
     def get(self, key: str, default: str = None) -> Optional[str]:
         try:
             return self[key]
         except KeyError:
             return default
+
+    @property
+    def keys(self) -> Tuple[str]:
+        return tuple(self._variables.keys())
```

### Comparing `py_sec_vault-0.1.2/PKG-INFO` & `py_sec_vault-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sec-vault
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vault implementation in python software (Hashicorp)
 Home-page: https://github.com/cisolutions-nl/py-sec-vault
 License: MIT
 Keywords: vault,hashicorp,security
 Author: CISolutions B.V.
 Author-email: info@cisolutions.nl
 Requires-Python: >=3.9
@@ -43,53 +43,80 @@
 
 ## Installation
 
 ```bash
 pip install py-sec-vault
 ```
 
-After this you should set environment variables to connect to the vault instance.
-
-```
-export VAULT_HOST=http://localhost:8200/
-export VAULT_AUTH_METHOD=approle|token
-export VAULT_ENGINE_NAME=<my_engine_name>
-export VAULT_ROLE_ID=<my_vault_id>
-export VAULT_SECRET_ID=<my_vauld_secret>
-export VAULT_PATH=<my_vault_path>
-```
-
 ## Usage
 
 ```python
 from vault import Vault
 
-vault = Vault()
+vault = Vault(
+    host="http://localhost:8200/",
+    auth_method="approle",
+    engine_name="my_engine_name",
+    path="my_vault_path",
+    token="my_vault_token",
+)
+
+# Prints the keys in the vault, validating if the vault is initialized;
+print(vault.keys) 
 
 # Retrieving a secret from the vault, or None if not found
 my_optional_secret = vault.get("MY_SECRET")
 
 # Retrieving a secret from the vault (and raising an exception if not found)
 my_secret = vault["MY_SECRET"]
 ```
 
 ## Usage with environment variables
+To make the vault work with environment variables, you can use the following code:
+
+First, you need to set the environment variables for the vault:
+```
+export VAULT_HOST=http://localhost:8200/
+export VAULT_AUTH_METHOD=approle|token
+export VAULT_ENGINE_NAME=<my_engine_name>
+export VAULT_ROLE_ID=<my_vault_id>
+export VAULT_SECRET_ID=<my_vauld_secret>
+export VAULT_PATH=<my_vault_path>
+```
+
+Second, you can use the following code to retrieve the secrets from the vault or environment variables:
 ```python
 from vault import from_env_or_vault, from_vault
 
 # NB: These functions will instantiate a Vault object and retrieve the secret from the vault
-# resulting in a performance penalty if used in a loop; in that case, instantiate a Vault object.
+# resulting in a performance penalty if used in a loop. Alternatively, you can instantiate a Vault object
+# once and use the get method to retrieve the secrets (next example).
 
 # Retrieving a secret from the vault or environment variable or using a default value
 from_env_or_vault("DB_PASSWORD", default="admin")
 
 # Retrieving a secret from the vault (and raising an exception if not found)
 from_vault("API_TOKEN")
 ```
 
+To retrieve all secrets from the vault, you can use the following code:
+```python
+from vault import Vault
+
+# This will connect to the vault based on the environment variables;
+vault = Vault()
+
+# Prints the keys in the vault, validating if the vault is initialized;
+print(vault.keys) 
+
+# Retrieving a secret from the vault, or None if not found
+my_optional_secret = vault.get("MY_SECRET")
+```
+
+
 ## Next steps
-- [ ] Make sure the vault is not initialized every time, but only when needed
+- [X] Make sure the vault is not initialized every time, but only when needed
 - [ ] On init load multiple paths/engines
 - [ ] Add support for other auth methods
 - [ ] Phase out the use of hvac and use requests instead
 - [ ] Implementation of from_vault_or_env
```

