# Comparing `tmp/python_equilibrium-0.7.0.tar.gz` & `tmp/python_equilibrium-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.7.0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.7.1.tar", max compression
```

## Comparing `python_equilibrium-0.7.0.tar` & `python_equilibrium-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.7.0/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.7.0/README.md
--rw-r--r--   0        0        0     1683 2023-06-02 14:27:10.841786 python_equilibrium-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      449 2023-06-02 09:59:54.391350 python_equilibrium-0.7.0/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0      899 2023-06-02 09:59:54.391350 python_equilibrium-0.7.0/src/equilibrium/BaseController.py
--rw-r--r--   0        0        0     1928 2023-06-02 09:59:54.391350 python_equilibrium-0.7.0/src/equilibrium/ControllerRegistry.py
--rw-r--r--   0        0        0     8949 2023-06-02 09:59:54.395350 python_equilibrium-0.7.0/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.7.0/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8519 2023-06-02 14:23:07.934769 python_equilibrium-0.7.0/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      707 2023-06-02 14:23:07.914769 python_equilibrium-0.7.0/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0       58 2023-06-02 09:59:54.395350 python_equilibrium-0.7.0/src/equilibrium/NotSet.py
--rw-r--r--   0        0        0    15629 2023-06-02 14:20:53.771254 python_equilibrium-0.7.0/src/equilibrium/Resource.py
--rw-r--r--   0        0        0     3474 2023-06-02 09:59:54.395350 python_equilibrium-0.7.0/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      258 2023-06-02 09:59:54.395350 python_equilibrium-0.7.0/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     8759 2023-06-02 14:23:07.930769 python_equilibrium-0.7.0/src/equilibrium/ResourceRegistry.py
--rw-r--r--   0        0        0     4888 2023-06-02 14:23:07.910769 python_equilibrium-0.7.0/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     1248 2023-06-02 14:22:08.290912 python_equilibrium-0.7.0/src/equilibrium/ResourceTypeRegistry.py
--rw-r--r--   0        0        0     4202 2023-06-02 14:19:57.779444 python_equilibrium-0.7.0/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.7.0/src/equilibrium/Service.py
--rw-r--r--   0        0        0     2913 2023-06-02 09:59:54.395350 python_equilibrium-0.7.0/src/equilibrium/ServiceRegistry.py
--rw-r--r--   0        0        0     1261 2023-06-02 14:27:10.841786 python_equilibrium-0.7.0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.7.0/src/equilibrium/py.typed
--rw-r--r--   0        0        0      313 2023-06-02 14:10:56.761492 python_equilibrium-0.7.0/src/equilibrium/types/FrozenDict.py
--rw-r--r--   0        0        0      381 2023-06-02 14:23:07.946769 python_equilibrium-0.7.0/src/equilibrium/types/FrozenList.py
--rw-r--r--   0        0        0      288 2023-06-02 14:10:32.261556 python_equilibrium-0.7.0/src/equilibrium/types/HashableMapping.py
--rw-r--r--   0        0        0      195 2023-06-02 14:10:32.513556 python_equilibrium-0.7.0/src/equilibrium/types/HashableSequence.py
--rw-r--r--   0        0        0      309 2023-06-02 14:10:32.509556 python_equilibrium-0.7.0/src/equilibrium/types/__init__.py
--rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 python_equilibrium-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1614 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/README.md
+-rw-r--r--   0        0        0     1683 2023-06-29 22:31:00.160302 python_equilibrium-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0      899 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/BaseController.py
+-rw-r--r--   0        0        0     1928 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/ControllerRegistry.py
+-rw-r--r--   0        0        0     8949 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8519 2023-06-29 22:28:30.752545 python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      707 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0       58 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/NotSet.py
+-rw-r--r--   0        0        0    15755 2023-06-29 22:30:25.377290 python_equilibrium-0.7.1/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0     3539 2023-06-29 22:22:52.506125 python_equilibrium-0.7.1/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      258 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     8759 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceRegistry.py
+-rw-r--r--   0        0        0     4888 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     1248 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceTypeRegistry.py
+-rw-r--r--   0        0        0     4202 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     2913 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ServiceRegistry.py
+-rw-r--r--   0        0        0     1261 2023-06-29 22:31:00.160302 python_equilibrium-0.7.1/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/py.typed
+-rw-r--r--   0        0        0      313 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/FrozenDict.py
+-rw-r--r--   0        0        0      381 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/FrozenList.py
+-rw-r--r--   0        0        0      288 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/HashableMapping.py
+-rw-r--r--   0        0        0      195 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/HashableSequence.py
+-rw-r--r--   0        0        0      309 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/__init__.py
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 python_equilibrium-0.7.1/PKG-INFO
```

### Comparing `python_equilibrium-0.7.0/LICENSE` & `python_equilibrium-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/README.md` & `python_equilibrium-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/pyproject.toml` & `python_equilibrium-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.7.0/src/equilibrium/BaseController.py` & `python_equilibrium-0.7.1/src/equilibrium/BaseController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/ControllerRegistry.py` & `python_equilibrium-0.7.1/src/equilibrium/ControllerRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.7.1/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/Namespace.py` & `python_equilibrium-0.7.1/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/Resource.py` & `python_equilibrium-0.7.1/src/equilibrium/Resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         return Resource.Locator(self.metadata.namespace, self.metadata.name)
 
     @property
     def uri(self) -> URI:
         return Resource.URI(self.apiVersion, self.kind, self.metadata.namespace, self.metadata.name)
 
     def into_generic(self) -> GenericResource:
-        if isinstance(self.spec, dict):
+        if isinstance(self.spec, Mapping):
             return cast(GenericResource, self)
         return Resource(
             self.apiVersion,
             self.kind,
             self.metadata,
             cast(dict[str, Any], databind.json.dump(self.spec, type(self.spec))),
             self.deletion_marker,
@@ -347,32 +347,34 @@
             raise ValueError(
                 f"{self.apiVersion=!r} does not match {spec_type.__name__}.apiVersion={spec_type.API_VERSION!r}"
             )
         if spec_type.KIND != self.kind:
             raise ValueError(f"{self.kind=!r} does not match {spec_type.__name__}.kind={spec_type.KIND!r}")
         if isinstance(self.spec, spec_type):
             return cast(Resource[U_Spec], self)
-        if not isinstance(self.spec, dict):
+        if not isinstance(self.spec, Mapping):
             raise RuntimeError("Resource.into() can only be used for generic resources")
         spec = databind.json.load(self.spec, spec_type)
         return Resource(self.apiVersion, self.kind, self.metadata, spec, self.deletion_marker, self.state)
 
     @overload
     @staticmethod
-    def of(payload: dict[str, Any]) -> GenericResource:
+    def of(payload: dict[str, Any], *, filename: str | None = None) -> GenericResource:
         ...
 
     @overload
     @staticmethod
-    def of(payload: dict[str, Any], spec_type: _Type[U_Spec]) -> Resource[U_Spec]:
+    def of(payload: dict[str, Any], spec_type: _Type[U_Spec], *, filename: str | None = None) -> Resource[U_Spec]:
         ...
 
     @staticmethod
-    def of(payload: dict[str, Any], spec_type: _Type[U_Spec] | None = None) -> Resource[Any]:
-        return databind.json.load(payload, GenericResource if spec_type is None else Resource[spec_type])  # type: ignore[valid-type]  # noqa: E501
+    def of(
+        payload: dict[str, Any], spec_type: _Type[U_Spec] | None = None, *, filename: str | None = None
+    ) -> Resource[Any]:
+        return databind.json.load(payload, GenericResource if spec_type is None else Resource[spec_type], filename)  # type: ignore[valid-type]  # noqa: E501
 
     @staticmethod
     def create(metadata: Resource.Metadata, spec: U_Spec, state: GenericState | None = None) -> Resource[U_Spec]:
         resource = Resource(spec.API_VERSION, spec.KIND, metadata, spec, None, state)
         spec.check_uri(resource.uri, do_raise=True)
         return resource
```

### Comparing `python_equilibrium-0.7.0/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.7.1/src/equilibrium/ResourceContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,14 @@
     def load_manifest(self, path: PathLike[str] | str) -> list[GenericResource]:
         """
         Loads a YAML file containing resource manifests into the store.
         """
 
         resources = []
         with Path(path).open() as fp:
-            for payload in yaml.safe_load_all(fp):
-                resource = Resource.of(payload)
+            for doc_idx, payload in enumerate(yaml.safe_load_all(fp)):
+                resource = Resource.of(payload, filename=f"{path}#document_index={doc_idx}")
                 resources.append(self.resources.put(resource))
         return resources
 
     def reconcile(self) -> None:
         self.controllers.reconcile(ResourceController.Context(self.resources, self.services))
```

### Comparing `python_equilibrium-0.7.0/src/equilibrium/ResourceRegistry.py` & `python_equilibrium-0.7.1/src/equilibrium/ResourceRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.7.1/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/ResourceTypeRegistry.py` & `python_equilibrium-0.7.1/src/equilibrium/ResourceTypeRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/Resource_test.py` & `python_equilibrium-0.7.1/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/Service.py` & `python_equilibrium-0.7.1/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/ServiceRegistry.py` & `python_equilibrium-0.7.1/src/equilibrium/ServiceRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.0/src/equilibrium/__init__.py` & `python_equilibrium-0.7.1/src/equilibrium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `python_equilibrium-0.7.0/PKG-INFO` & `python_equilibrium-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

