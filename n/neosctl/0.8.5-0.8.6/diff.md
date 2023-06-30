# Comparing `tmp/neosctl-0.8.5.tar.gz` & `tmp/neosctl-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.5.tar", max compression
+gzip compressed data, was "neosctl-0.8.6.tar", max compression
```

## Comparing `neosctl-0.8.5.tar` & `neosctl-0.8.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-06-21 14:04:03.367848 neosctl-0.8.5/README.md
--rw-r--r--   0        0        0       22 2023-06-21 14:04:03.367848 neosctl-0.8.5/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5491 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-06-21 14:04:03.368847 neosctl-0.8.5/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3564 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     3764 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3067 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      141 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8556 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12292 2023-06-21 14:04:03.369848 neosctl-0.8.5/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-06-21 14:04:03.370848 neosctl-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-06-30 08:38:12.975171 neosctl-0.8.6/README.md
+-rw-r--r--   0        0        0       22 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3564 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     5472 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3216 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      141 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8649 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12292 2023-06-30 08:38:12.978171 neosctl-0.8.6/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-06-30 08:38:12.978171 neosctl-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.6/PKG-INFO
```

### Comparing `neosctl-0.8.5/README.md` & `neosctl-0.8.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.5
+# Core CLI v0.8.6
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.5/neosctl/auth.py` & `neosctl-0.8.6/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/cli.py` & `neosctl-0.8.6/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/profile.py` & `neosctl-0.8.6/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/schema.py` & `neosctl-0.8.6/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/__init__.py` & `neosctl-0.8.6/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/data_product.py` & `neosctl-0.8.6/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/data_source.py` & `neosctl-0.8.6/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/data_system.py` & `neosctl-0.8.6/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.6/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/entity.py` & `neosctl-0.8.6/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/link.py` & `neosctl-0.8.6/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/output.py` & `neosctl-0.8.6/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/schema.py` & `neosctl-0.8.6/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/secret.py` & `neosctl-0.8.6/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/spark.py` & `neosctl-0.8.6/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/gateway/tag.py` & `neosctl-0.8.6/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/iam/iam.py` & `neosctl-0.8.6/neosctl/services/iam/iam.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 import httpx
 import typer
 
-from neosctl import util
+from neosctl import constant, util
 from neosctl.services.iam import schema
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _iam_url(iam_api_url: str, postfix: str = "") -> str:
@@ -121,7 +121,64 @@
             ctx,
             "{iam_url}".format(iam_url=_iam_url(ctx.obj.get_iam_api_url(), "policy/user")),
             params={"user_nrn": user_nrn},
         )
 
     r = _request(ctx)
     process_response(r)
+
+
+@app.command(name="list-users")
+def list_users(
+    ctx: typer.Context,
+    search: str = typer.Option(None, help="Search term", callback=util.sanitize),
+) -> None:
+    """List existing keycloak users.
+
+    Filter by search term on username, first_name, last_name, or email.
+    """
+
+    @util.ensure_login
+    def _request(ctx: typer.Context) -> httpx.Response:
+        return util.get(
+            ctx,
+            _iam_url(ctx.obj.get_iam_api_url(), "users"),
+            params={"search": search} if search else None,
+        )
+
+    r = _request(ctx)
+    process_response(r)
+
+
+@app.command(name="user-permissions")
+def user_permissions(
+    ctx: typer.Context,
+    username: str = typer.Argument(..., help="Keycloak username", callback=util.sanitize),
+) -> None:
+    """List existing keycloak user permissions."""
+
+    @util.ensure_login
+    def _request(ctx: typer.Context) -> httpx.Response:
+        r = util.get(
+            ctx,
+            _iam_url(ctx.obj.get_iam_api_url(), "users"),
+            params={"search": username},
+        )
+        if r.status_code >= constant.BAD_REQUEST_CODE:
+            process_response(r)
+
+        data = r.json()
+        # In case search term matches email/name of another user, filter for specific username
+        user_id = next((user["id"] for user in data["users"] if user["username"] == username), None)
+
+        if user_id is None:
+            typer.echo("User not found.")
+            raise typer.Exit(code=1)
+
+        return util.get(
+            ctx,
+            "{iam_url}".format(iam_url=_iam_url(ctx.obj.get_iam_api_url(), "policy/user")),
+            params={"user_nrn": user_id},
+        )
+
+    r = _request(ctx)
+    process_response(r)
```

### Comparing `neosctl-0.8.5/neosctl/services/iam/schema.py` & `neosctl-0.8.6/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/neosctl/services/registry/registry.py` & `neosctl-0.8.6/neosctl/services/registry/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,24 @@
     r = _request(ctx, rc)
     process_response(r)
 
 
 @app.command(name="list-cores")
 def list_cores(
     ctx: typer.Context,
+    search: str = typer.Option(None, help="Search core name(s)", callback=util.sanitize),
 ) -> None:
     """List existing registered cores."""
 
     @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
         return util.get(
             ctx,
             _core_url(ctx.obj.get_registry_api_url()),
+            params={"search": search} if search else None,
         )
 
     r = _request(ctx)
     process_response(r)
 
 
 @app.command(name="remove-core")
```

### Comparing `neosctl-0.8.5/neosctl/services/storage/storage.py` & `neosctl-0.8.6/neosctl/services/storage/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,27 +119,28 @@
 def list_objects(
     ctx: typer.Context,
     bucket_name: str = typer.Argument(
         ...,
         help="Bucket name",
         callback=util.validate_string_not_empty,
     ),
+    prefix: typing.Union[str, None] = typer.Option(None, help="Path prefix"),
 ) -> None:
     """List objects."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
 
     client = minio.Minio(  # nosec: B106
         host,
         access_key=ctx.obj.profile.access_token,
         secret_key="random-secret",
         secure=secure,
     )
 
-    print([obj._object_name for obj in client.list_objects(bucket_name)])  # noqa: SLF001, T201
+    print([obj._object_name for obj in client.list_objects(bucket_name, prefix=prefix)])  # noqa: SLF001, T201
 
 
 @object_app.command(name="get")
 def get_object(
     ctx: typer.Context,
     bucket_name: str = typer.Argument(
         ...,
```

### Comparing `neosctl-0.8.5/neosctl/util.py` & `neosctl-0.8.6/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.5/pyproject.toml` & `neosctl-0.8.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.5"
+version = "0.8.6"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.5/PKG-INFO` & `neosctl-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.5
+Version: 0.8.6
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.5
+# Core CLI v0.8.6
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

