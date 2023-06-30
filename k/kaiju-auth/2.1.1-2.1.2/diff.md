# Comparing `tmp/kaiju_auth-2.1.1-py3-none-any.whl.zip` & `tmp/kaiju_auth-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,16 @@
-Zip file size: 16219 bytes, number of entries: 11
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-29 12:35 kaiju_auth/__init__.py
--rw-r--r--  2.0 unx    39335 b- defN 23-Jun-29 12:35 kaiju_auth/services.py
--rw-r--r--  2.0 unx       55 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/__init__.py
--rw-r--r--  2.0 unx     3228 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/models.py
--rw-r--r--  2.0 unx    18327 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/service.py
--rw-r--r--  2.0 unx     1212 b- defN 23-Jun-29 12:35 kaiju_auth/permissions_gui/validators.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2987 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      935 b- defN 23-Jun-29 12:36 kaiju_auth-2.1.1.dist-info/RECORD
-11 files, 66885 bytes uncompressed, 14623 bytes compressed:  78.1%
+Zip file size: 18870 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-30 16:23 kaiju_auth/__init__.py
+-rw-r--r--  2.0 unx    39376 b- defN 23-Jun-30 16:23 kaiju_auth/services.py
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/__init__.py
+-rw-r--r--  2.0 unx     3228 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/models.py
+-rw-r--r--  2.0 unx    18327 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/service.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-Jun-30 16:23 kaiju_auth/permissions_gui/validators.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-30 16:23 kaiju_auth/tests/__init__.py
+-rw-r--r--  2.0 unx     1516 b- defN 23-Jun-30 16:23 kaiju_auth/tests/fixtures.py
+-rw-r--r--  2.0 unx     7957 b- defN 23-Jun-30 16:23 kaiju_auth/tests/test_auth.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2987 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Jun-30 16:24 kaiju_auth-2.1.2.dist-info/RECORD
+14 files, 76695 bytes uncompressed, 16876 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -12,23 +12,32 @@
 
 Filename: kaiju_auth/permissions_gui/service.py
 Comment: 
 
 Filename: kaiju_auth/permissions_gui/validators.py
 Comment: 
 
-Filename: kaiju_auth-2.1.1.dist-info/LICENSE
+Filename: kaiju_auth/tests/__init__.py
 Comment: 
 
-Filename: kaiju_auth-2.1.1.dist-info/METADATA
+Filename: kaiju_auth/tests/fixtures.py
 Comment: 
 
-Filename: kaiju_auth-2.1.1.dist-info/WHEEL
+Filename: kaiju_auth/tests/test_auth.py
 Comment: 
 
-Filename: kaiju_auth-2.1.1.dist-info/top_level.txt
+Filename: kaiju_auth-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_auth-2.1.1.dist-info/RECORD
+Filename: kaiju_auth-2.1.2.dist-info/METADATA
+Comment: 
+
+Filename: kaiju_auth-2.1.2.dist-info/WHEEL
+Comment: 
+
+Filename: kaiju_auth-2.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: kaiju_auth-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_auth/__init__.py

```diff
@@ -1,4 +1,4 @@
 from kaiju_auth.services import *
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_auth/services.py

```diff
@@ -814,15 +814,15 @@
             interval=self.ttl / 2,
             retries=10,
             name=f'{self.service_name}._generate_encryption_key',
         )
 
     async def close(self):
         self._task_renew_keys.enabled = False
-        await self._cache.delete(self.ns.get_key(self._kid))
+        # await self._cache.delete(self.ns.get_key(self._kid))
 
     @property
     def encryption_key(self) -> (str, jwt.JWK):
         """Get a key pair."""
         return self._kid, self._key
 
     async def get_public_key(self, kid: str = None) -> Optional[jwk.JWK]:
@@ -832,15 +832,15 @@
         pkey = await self._cache.get(self.ns.get_key(kid))
         if pkey:
             return jwk.JWK(**pkey)
 
     async def _generate_encryption_key(self) -> None:
         """Generate and set a new key pair and key deadline and push the public key to the shared store (cache)."""
         kid = uuid.uuid4().hex
-        key = jwk.JWK.generate(kty=self.algorithm, size=self.key_size)
+        key = jwk.JWK.generate(kty=self.algorithm, size=self.key_size, kid=kid)
         pkey = key.export_public(as_dict=True)
         self._pkey = jwk.JWK(**pkey)
         self._kid = kid
         self._key = key
         self._deadline = time() + self.ttl
         await self._cache.set(self.ns.get_key(self._kid), pkey, ttl=self.ttl)
 
@@ -1035,15 +1035,16 @@
                     await service.set_user_groups(user_id, user_groups)
         else:
             self.logger.debug('No user fixtures have been found.')
 
     @staticmethod
     def load_file(path: Path):
         if path.exists():
-            return load(str(path))
+            with open(path) as f:
+                return load(f)
 
 
 service_class_registry.register_class(PermissionService)
 service_class_registry.register_class(GroupService)
 service_class_registry.register_class(UserService)
 service_class_registry.register_class(JWTClientService)
 service_class_registry.register_class(SessionStore)
```

## Comparing `kaiju_auth-2.1.1.dist-info/LICENSE` & `kaiju_auth-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_auth-2.1.1.dist-info/METADATA` & `kaiju_auth-2.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-auth
-Version: 2.1.1
+Version: 2.1.2
 Summary: Authentication services.
 Home-page: https://gitlab.com/kaiju-python/kaiju-auth
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

