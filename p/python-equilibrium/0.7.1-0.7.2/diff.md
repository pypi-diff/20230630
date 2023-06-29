# Comparing `tmp/python_equilibrium-0.7.1.tar.gz` & `tmp/python_equilibrium-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.7.1.tar", max compression
+gzip compressed data, was "python_equilibrium-0.7.2.tar", max compression
```

## Comparing `python_equilibrium-0.7.1.tar` & `python_equilibrium-0.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      988 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/LICENSE
--rw-r--r--   0        0        0     1614 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/README.md
--rw-r--r--   0        0        0     1683 2023-06-29 22:31:00.160302 python_equilibrium-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      449 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0      899 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/BaseController.py
--rw-r--r--   0        0        0     1928 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/ControllerRegistry.py
--rw-r--r--   0        0        0     8949 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8519 2023-06-29 22:28:30.752545 python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      707 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0       58 2023-06-29 22:21:32.536390 python_equilibrium-0.7.1/src/equilibrium/NotSet.py
--rw-r--r--   0        0        0    15755 2023-06-29 22:30:25.377290 python_equilibrium-0.7.1/src/equilibrium/Resource.py
--rw-r--r--   0        0        0     3539 2023-06-29 22:22:52.506125 python_equilibrium-0.7.1/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      258 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     8759 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceRegistry.py
--rw-r--r--   0        0        0     4888 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     1248 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ResourceTypeRegistry.py
--rw-r--r--   0        0        0     4202 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/Service.py
--rw-r--r--   0        0        0     2913 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/ServiceRegistry.py
--rw-r--r--   0        0        0     1261 2023-06-29 22:31:00.160302 python_equilibrium-0.7.1/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/py.typed
--rw-r--r--   0        0        0      313 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/FrozenDict.py
--rw-r--r--   0        0        0      381 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/FrozenList.py
--rw-r--r--   0        0        0      288 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/HashableMapping.py
--rw-r--r--   0        0        0      195 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/HashableSequence.py
--rw-r--r--   0        0        0      309 2023-06-29 22:21:32.540390 python_equilibrium-0.7.1/src/equilibrium/types/__init__.py
--rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 python_equilibrium-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1614 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/README.md
+-rw-r--r--   0        0        0     1683 2023-06-29 22:37:07.857862 python_equilibrium-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0      899 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/BaseController.py
+-rw-r--r--   0        0        0     1928 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/ControllerRegistry.py
+-rw-r--r--   0        0        0     8949 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8519 2023-06-29 22:28:30.752545 python_equilibrium-0.7.2/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      707 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0       58 2023-06-29 22:21:32.536390 python_equilibrium-0.7.2/src/equilibrium/NotSet.py
+-rw-r--r--   0        0        0    16240 2023-06-29 22:35:06.349310 python_equilibrium-0.7.2/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0     3539 2023-06-29 22:22:52.506125 python_equilibrium-0.7.2/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      258 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     8759 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/ResourceRegistry.py
+-rw-r--r--   0        0        0     4888 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     1248 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/ResourceTypeRegistry.py
+-rw-r--r--   0        0        0     4202 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     2913 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/ServiceRegistry.py
+-rw-r--r--   0        0        0     1261 2023-06-29 22:37:07.857862 python_equilibrium-0.7.2/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/py.typed
+-rw-r--r--   0        0        0      313 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/types/FrozenDict.py
+-rw-r--r--   0        0        0      381 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/types/FrozenList.py
+-rw-r--r--   0        0        0      288 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/types/HashableMapping.py
+-rw-r--r--   0        0        0      195 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/types/HashableSequence.py
+-rw-r--r--   0        0        0      309 2023-06-29 22:21:32.540390 python_equilibrium-0.7.2/src/equilibrium/types/__init__.py
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 python_equilibrium-0.7.2/PKG-INFO
```

### Comparing `python_equilibrium-0.7.1/LICENSE` & `python_equilibrium-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/README.md` & `python_equilibrium-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/pyproject.toml` & `python_equilibrium-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.7.1/src/equilibrium/BaseController.py` & `python_equilibrium-0.7.2/src/equilibrium/BaseController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/ControllerRegistry.py` & `python_equilibrium-0.7.2/src/equilibrium/ControllerRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.7.2/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.7.2/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.7.2/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/Namespace.py` & `python_equilibrium-0.7.2/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/Resource.py` & `python_equilibrium-0.7.2/src/equilibrium/Resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,25 +266,31 @@
     @dataclass(frozen=True)
     class Metadata:
         namespace: str | None
         name: str
         labels: HashableMapping[str, str] = field(default_factory=FrozenDict)
         annotations: HashableMapping[str, str] = field(default_factory=FrozenDict)
 
+        #: A string that identifies where the resource originates from.
+        origin: str | None = None
+
         def __post_init__(self) -> None:
             validate_identifier(self.name, "name")
             if self.namespace is not None:
                 validate_identifier(self.namespace, "namespace")
 
         def __repr__(self) -> str:
             return f"Resource.Metadata(namespace={self.namespace!r}, name={self.name!r})"
 
         def with_namespace(self, namespace: str | None) -> Resource.Metadata:
             return replace(self, namespace=namespace)
 
+        def with_origin(self, origin: str | None) -> Resource.Metadata:
+            return replace(self, origin=origin)
+
     @dataclass(frozen=True)
     class DeletionMarker:
         timestamp: datetime = field(default_factory=lambda: datetime.now(timezone.utc))
 
     @dataclass(frozen=True)
     class Event:
         Type = Literal["Normal", "Warning", "Error"]
@@ -333,15 +339,15 @@
     def into_generic(self) -> GenericResource:
         if isinstance(self.spec, Mapping):
             return cast(GenericResource, self)
         return Resource(
             self.apiVersion,
             self.kind,
             self.metadata,
-            cast(dict[str, Any], databind.json.dump(self.spec, type(self.spec))),
+            cast(dict[str, Any], databind.json.dump(self.spec, type(self.spec), filename=self.metadata.origin)),
             self.deletion_marker,
             self.state,
         )
 
     def into(self, spec_type: _Type[U_Spec]) -> Resource[U_Spec]:
         if spec_type.API_VERSION != self.apiVersion:
             raise ValueError(
@@ -349,15 +355,15 @@
             )
         if spec_type.KIND != self.kind:
             raise ValueError(f"{self.kind=!r} does not match {spec_type.__name__}.kind={spec_type.KIND!r}")
         if isinstance(self.spec, spec_type):
             return cast(Resource[U_Spec], self)
         if not isinstance(self.spec, Mapping):
             raise RuntimeError("Resource.into() can only be used for generic resources")
-        spec = databind.json.load(self.spec, spec_type)
+        spec = databind.json.load(self.spec, spec_type, filename=self.metadata.origin)
         return Resource(self.apiVersion, self.kind, self.metadata, spec, self.deletion_marker, self.state)
 
     @overload
     @staticmethod
     def of(payload: dict[str, Any], *, filename: str | None = None) -> GenericResource:
         ...
 
@@ -366,15 +372,18 @@
     def of(payload: dict[str, Any], spec_type: _Type[U_Spec], *, filename: str | None = None) -> Resource[U_Spec]:
         ...
 
     @staticmethod
     def of(
         payload: dict[str, Any], spec_type: _Type[U_Spec] | None = None, *, filename: str | None = None
     ) -> Resource[Any]:
-        return databind.json.load(payload, GenericResource if spec_type is None else Resource[spec_type], filename)  # type: ignore[valid-type]  # noqa: E501
+        resource = databind.json.load(payload, GenericResource if spec_type is None else Resource[spec_type], filename)  # type: ignore[valid-type]  # noqa: E501
+        if filename is not None:
+            resource.metadata = resource.metadata.with_origin(filename)
+        return resource
 
     @staticmethod
     def create(metadata: Resource.Metadata, spec: U_Spec, state: GenericState | None = None) -> Resource[U_Spec]:
         resource = Resource(spec.API_VERSION, spec.KIND, metadata, spec, None, state)
         spec.check_uri(resource.uri, do_raise=True)
         return resource
 
@@ -388,18 +397,18 @@
 
     def get_state(self, state_type: _Type[U_State] | _Type[GenericState]) -> U_State | GenericState:
         if self.state is None:
             raise ValueError("resource has no state")
         if state_type == Resource.GenericState or state_type is dict:
             return self.state
         else:
-            return cast(U_State, databind.json.load(self.state, state_type))
+            return cast(U_State, databind.json.load(self.state, state_type, filename=self.metadata.origin))
 
     def set_state(self, state_type: _Type[T_State], state: T_State) -> None:
-        self.state = cast(Resource.GenericState, databind.json.dump(state, state_type))
+        self.state = cast(Resource.GenericState, databind.json.dump(state, state_type, filename=self.metadata.origin))
 
 
 # NOTE(@NiklasRosenstein): We repeat the definition of the type variables here for use inside the Resource class.
 #       Attempting to reference a type variable inside the class definition in which the variable is defined
 #       leads to issues, especially if that type variable needs to be referenced in a cast() inside a method.
 U_Spec = TypeVar("U_Spec", bound="Resource.Spec")
 U_State = TypeVar("U_State", bound="Resource.State")
```

### Comparing `python_equilibrium-0.7.1/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.7.2/src/equilibrium/ResourceContext.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/ResourceRegistry.py` & `python_equilibrium-0.7.2/src/equilibrium/ResourceRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.7.2/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/ResourceTypeRegistry.py` & `python_equilibrium-0.7.2/src/equilibrium/ResourceTypeRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/Resource_test.py` & `python_equilibrium-0.7.2/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/Service.py` & `python_equilibrium-0.7.2/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/ServiceRegistry.py` & `python_equilibrium-0.7.2/src/equilibrium/ServiceRegistry.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.7.1/src/equilibrium/__init__.py` & `python_equilibrium-0.7.2/src/equilibrium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

### Comparing `python_equilibrium-0.7.1/PKG-INFO` & `python_equilibrium-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

