# Comparing `tmp/quiltcore-0.1.1.tar.gz` & `tmp/quiltcore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltcore-0.1.1.tar", max compression
+gzip compressed data, was "quiltcore-0.1.2.tar", max compression
```

## Comparing `quiltcore-0.1.1.tar` & `quiltcore-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.1.1/LICENSE
--rw-r--r--   0        0        0     1547 2023-06-28 18:42:45.780392 quiltcore-0.1.1/README.md
--rw-r--r--   0        0        0      834 2023-06-29 00:46:44.318863 quiltcore-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      319 2023-06-28 04:19:14.927986 quiltcore-0.1.1/quiltcore/__init__.py
--rw-r--r--   0        0        0     2124 2023-06-29 07:49:44.000000 quiltcore-0.1.1/quiltcore/blob.py
--rw-r--r--   0        0        0      698 2023-06-29 07:49:44.000000 quiltcore-0.1.1/quiltcore/config.py
--rw-r--r--   0        0        0      625 2023-06-28 17:38:51.469138 quiltcore-0.1.1/quiltcore/config.yaml
--rw-r--r--   0        0        0     2040 2023-06-29 07:49:44.000000 quiltcore-0.1.1/quiltcore/manifest.py
--rw-r--r--   0        0        0      549 2023-06-29 07:49:44.000000 quiltcore-0.1.1/quiltcore/name.py
--rw-r--r--   0        0        0      637 2023-06-28 18:05:56.516749 quiltcore-0.1.1/quiltcore/registry.py
--rw-r--r--   0        0        0     2001 2023-06-29 07:49:44.000000 quiltcore-0.1.1/quiltcore/resource.py
--rw-r--r--   0        0        0      160 2023-06-27 22:10:43.161786 quiltcore-0.1.1/quiltcore/schema.yaml
--rw-r--r--   0        0        0      231 2023-06-28 02:38:30.000000 quiltcore-0.1.1/quiltcore/values.py
--rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 quiltcore-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 04:58:49.699035 quiltcore-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1551 2023-06-29 23:49:03.946275 quiltcore-0.1.2/README.md
+-rw-r--r--   0        0        0      831 2023-06-29 23:54:09.916620 quiltcore-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      930 2023-06-30 00:35:03.061872 quiltcore-0.1.2/quiltcore/__init__.py
+-rw-r--r--   0        0        0     1771 2023-06-30 07:59:56.000000 quiltcore-0.1.2/quiltcore/blob.py
+-rw-r--r--   0        0        0      698 2023-06-30 00:30:52.256979 quiltcore-0.1.2/quiltcore/config.py
+-rw-r--r--   0        0        0     2175 2023-06-30 07:59:56.000000 quiltcore-0.1.2/quiltcore/manifest.py
+-rw-r--r--   0        0        0      599 2023-06-30 00:34:19.012973 quiltcore-0.1.2/quiltcore/namespace.py
+-rw-r--r--   0        0        0      615 2023-06-30 00:34:48.607108 quiltcore-0.1.2/quiltcore/registry.py
+-rw-r--r--   0        0        0     2457 2023-06-30 07:59:56.000000 quiltcore-0.1.2/quiltcore/resource.py
+-rw-r--r--   0        0        0      610 2023-06-30 00:42:57.086957 quiltcore-0.1.2/quiltcore/yaml/quiltcore.yaml
+-rw-r--r--   0        0        0      160 2023-06-27 22:10:43.161786 quiltcore-0.1.2/quiltcore/yaml/schema.yaml
+-rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 quiltcore-0.1.2/PKG-INFO
```

### Comparing `quiltcore-0.1.1/LICENSE` & `quiltcore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quiltcore-0.1.1/README.md` & `quiltcore-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,30 +17,31 @@
 ## Example
 
 ```bash
 poetry install
 ```
 
 ```python
-from quiltcore import CoreRegistry
+from quiltcore import Registry
 from tempfile import TemporaryDirectory
 from upath import UPath
 
 TEST_BKT = "s3://quilt-example"
 TEST_PKG = "akarve/amazon-reviews"
 TEST_TAG = "1570503102"
 TEST_HASH = "ffe323137d0a84a9d1d6f200cecd616f434e121b3f53a8891a5c8d70f82244c2"
 TEST_KEY = "camera-reviews"
 ```
 
 ### Get Manifest
 
 <!--pytest-codeblocks:cont-->
 ```python
-registry = CoreRegistry(UPath(TEST_BKT))
+path = UPath(TEST_BKT)
+registry = Registry(path)
 named_package = registry.get(TEST_PKG)
 manifest = named_package.get(TEST_TAG)
 blob = manifest.get(TEST_KEY)
 ```
 
 ### Get Object
```

### Comparing `quiltcore-0.1.1/pyproject.toml` & `quiltcore-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "quiltcore"
-version = "0.1.1"
-description = "next-generation package manager for universal data"
+version = "0.1.2"
+description = "low-level plubming to read/write Quilt packages"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = "^4.6.3"
 tzlocal = "^5.0.1"
```

### Comparing `quiltcore-0.1.1/quiltcore/blob.py` & `quiltcore-0.1.2/quiltcore/blob.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 from pathlib import Path
 
 from multiformats import multihash
 
-from .manifest import CoreManifest
-from .resource import CoreResource
+from .resource import Resource
 
 
-class CoreBlob(CoreResource):
-    """Storage for dereferenced Names"""
+class Blob(Resource):
+    """Represents a single blob of data in a datastore."""
 
-    MH_PREFIX = "1220"
-
-    @staticmethod
-    def FromKeyInManifest(key: str, manifest: CoreManifest) -> "CoreBlob":
-        path = manifest.child_path(key)
-        row = manifest.child_row(key)
-        return CoreBlob(path, parent=manifest, row=row)
+    MH_PREFIX_SHA256 = "1220"
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         self.parent = kwargs["parent"]
         self.row = kwargs["row"]
         if len(self.row) > 0:
             self.setup(self.row)
@@ -33,35 +26,38 @@
                 key = key.rstrip("s")
             if type == "int64":
                 value = int(value)
             setattr(self, key, value)
             if key == "hash":
                 self.setup_hash(value)  # type: ignore
 
+    #
+    # Calculate and verify hash
+    #
+
     def setup_hash(self, opt: dict):
         self.hash_value = opt["value"]
         hash_key = f'multihash/{opt["type"]}'
         self.hash_type = self.cf.get_str(hash_key)
         self.hash_digest = multihash.get(self.hash_type)
 
     def digest(self, bstring: bytes) -> str:
         digest = self.hash_digest.digest(bstring)
         hex = digest.hex()
-        return hex.strip(CoreBlob.MH_PREFIX)
-
-    def name(self):
-        return self.row[self.parent.name_col]  # type: ignore
-
-    def location(self):
-        return self.row[self.parent.loc_col]  # type: ignore
-
-    def put(self, dest: Path) -> Path:
-        """Put a resource into dest. Return the new path"""
-        dest.write_bytes(self.path.read_bytes())  # for binary files
-        return dest
+        return hex.strip(Blob.MH_PREFIX_SHA256)
 
     def verify(self, bstring: bytes) -> bool:
         """Verify that bytes match the hash"""
         digest = self.digest(bstring)
         print(digest)
         print(self.hash_value)
         return digest == self.hash_value
+
+    #
+    # Convenience Methods
+    #
+
+    def name(self):
+        return self.row[self.parent.name_col]  # type: ignore
+
+    def place(self):
+        return self.row[self.parent.place_col]  # type: ignore
```

### Comparing `quiltcore-0.1.1/quiltcore/config.py` & `quiltcore-0.1.2/quiltcore/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 from un_yaml import UnYaml  # type: ignore
 
 
-class CoreConfig(UnYaml):
-    CONFIG_FILE = "config.yaml"
+class Config(UnYaml):
+    CONFIG_FILE = "yaml/quiltcore.yaml"
 
     @classmethod
     def DefaultConfig(cls) -> dict:
         return UnYaml.LoadYaml(cls.CONFIG_FILE, __package__)
 
     def __init__(self, yaml_data: dict = {}) -> None:
-        data = yaml_data if len(yaml_data) > 0 else CoreConfig.DefaultConfig()
+        data = yaml_data if len(yaml_data) > 0 else Config.DefaultConfig()
         super().__init__(data)
 
     def get_str(self, key: str, default="") -> str:
         return super().get(key) or default
 
     def get_path(self, key: str) -> Path:
         str_path = self.get_str(key, ".")
```

### Comparing `quiltcore-0.1.1/quiltcore/config.yaml` & `quiltcore-0.1.2/quiltcore/yaml/quiltcore.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -4,34 +4,34 @@
   app: registry
   app_version: 0.1.0
   doc: quiltcore
   doc_version: 0.1.0
 dirs:
   config: .quilt
   names: named_packages
-  values: packages
+  versions: packages
 multihash:
   SHA256: sha2-256
 resources:
-  CoreRegistry:
-    child: CoreName
+  Registry:
+    child: Namespace
     glob: "*/*"
-  CoreName:
-    child: CoreManifest
+  Namespace:
+    child: Manifest
     glob: "*"
-  CoreManifest:
-    child: CoreBlob
+  Manifest:
+    child: Blob
 schema:
   columns:
     logical_key: string
     physical_keys: [string]
     size: int64
     hash:
       type: string
       value: string
     meta: struct
   headers:
     version: string
     message: string
-  location: physical_keys
+  place: physical_keys
   name: logical_key
 type: application/ld+json
```

### Comparing `quiltcore-0.1.1/quiltcore/manifest.py` & `quiltcore-0.1.2/quiltcore/manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,55 +2,65 @@
 
 import pyarrow as pa  # type: ignore
 import pyarrow.compute as pc  # type: ignore
 import pyarrow.json as pj  # type: ignore
 from typing_extensions import Self
 from upath import UPath
 
-from .resource import CoreResource
+from .resource import Resource
 
 
-class CoreManifest(CoreResource):
-    """In-memory representation of a serialized package manifest."""
+class Manifest(Resource):
+    """
+    In-memory representation of a serialized package manifest.
+    list/get returns Blob with Path to the Place data actually lives
+    """
 
     # TODO: cache Blobs to avoid repeated lookups
-    # TODO: improve/replace child(key) handling
 
     def __init__(self, path: Path, **kwargs):
         super().__init__(path, **kwargs)
         with path.open(mode="rb") as fi:
             self.table = pj.read_json(fi)
-        self.body = self.setup()
+        self.body = self.setup_table()
         self.name_col = self.cf.get_str("schema/name", "logical_key")
-        self.loc_col = self.cf.get_str("schema/location", "physical_keys")
+        self.place_col = self.cf.get_str("schema/place", "physical_keys")
 
-    def setup(self) -> pa.Table:
+    def setup_table(self) -> pa.Table:
         first = self.table.take([0]).to_pydict()
         headers = self.cf.get_dict("schema/headers")
         keys = list(headers.keys())
         for key in keys:
             setattr(self, key, first[key][0])
         return self.table.drop_columns(keys).slice(1)
 
+    #
+    # Private Methods for child resources
+    #
+
     def child_row(self, key: str) -> dict:
         """Return the dict for a child resource."""
         # TODO: cache to avoid continually re-calcluating
         rows = self.body.filter(pc.field(self.name_col) == key)
         if rows.num_rows == 0:
             raise KeyError(f"Key [{key}] not found in {self.name_col} of {self.path}")
         return rows.to_pydict()
 
     def child_path(self, key: str) -> Path:
-        """Return the path for a child resource."""
+        """Return the Path for a child resource."""
         row = self.child_row(key)
-        loc = row[self.loc_col][0][0]
-        return UPath(loc)
+        place = row[self.place_col][0][0]
+        return UPath(place)
 
     def child_args(self, key: str) -> dict:
         """Return the parameters for a child resource."""
         row = self.child_row(key)
         return {"row": row, "parent": self}
 
+    #
+    # Public HTTP-like Methods
+    #
+
     def list(self) -> list[Self]:
         """List all child resources."""
         names = self.body.column(self.name_col).to_pylist()
         return [self.child(self.child_path(x), x) for x in names]
```

### Comparing `quiltcore-0.1.1/PKG-INFO` & `quiltcore-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: quiltcore
-Version: 0.1.1
-Summary: next-generation package manager for universal data
+Version: 0.1.2
+Summary: low-level plubming to read/write Quilt packages
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
@@ -39,30 +39,31 @@
 ## Example
 
 ```bash
 poetry install
 ```
 
 ```python
-from quiltcore import CoreRegistry
+from quiltcore import Registry
 from tempfile import TemporaryDirectory
 from upath import UPath
 
 TEST_BKT = "s3://quilt-example"
 TEST_PKG = "akarve/amazon-reviews"
 TEST_TAG = "1570503102"
 TEST_HASH = "ffe323137d0a84a9d1d6f200cecd616f434e121b3f53a8891a5c8d70f82244c2"
 TEST_KEY = "camera-reviews"
 ```
 
 ### Get Manifest
 
 <!--pytest-codeblocks:cont-->
 ```python
-registry = CoreRegistry(UPath(TEST_BKT))
+path = UPath(TEST_BKT)
+registry = Registry(path)
 named_package = registry.get(TEST_PKG)
 manifest = named_package.get(TEST_TAG)
 blob = manifest.get(TEST_KEY)
 ```
 
 ### Get Object
```

