# Comparing `tmp/bump_pydantic-0.0.1.tar.gz` & `tmp/bump_pydantic-0.1.0.tar.gz`

## Comparing `bump_pydantic-0.0.1.tar` & `bump_pydantic-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,34 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/__main__.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/py.typed
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/add_default_none.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/class_def_visitor.py
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/field.py
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/replace_config.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/replace_generic_model.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/replace_imports.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/codemods/root_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/markers/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/bump_pydantic/markers/find_base_model.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/Activate.ps1
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/activate
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/activate.csh
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/activate.fish
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/docutils
--rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/keyring
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/markdown-it
--rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/normalizer
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/pip
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/pip3
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/pip3.10
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/pkginfo
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/pygmentize
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/python -> python3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/python3 -> python3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/python3.10 -> /Users/samuel/.pyenv/versions/3.10.5/bin/python3.10
--rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2html.py
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2html5.py
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2latex.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2man.py
--rwxr-xr-x   0        0        0      828 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2odt.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      683 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2s5.py
--rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rst2xml.py
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/env310/bin/twine
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/integration/__init__.py
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/integration/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_add_default_none.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_class_def_visitor.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_field.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_generic_model.py
--rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_replace_config.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_replace_imports.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/tests/unit/test_root_model.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/README.md
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 bump_pydantic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/__main__.py
+-rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/py.typed
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/__init__.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/add_default_none.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/class_def_visitor.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/field.py
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/replace_config.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/replace_generic_model.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/replace_imports.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/root_model.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/markers/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/markers/find_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_add_default_none.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_class_def_visitor.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_field.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_generic_model.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_replace_config.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_replace_imports.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_root_model.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_validator.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/README.md
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/PKG-INFO
```

### Comparing `bump_pydantic-0.0.1/.github/workflows/main.yml` & `bump_pydantic-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/main.py` & `bump_pydantic-0.1.0/bump_pydantic/main.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/.github/workflows/ci.yml` & `bump_pydantic-0.1.0/bump_pydantic/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/__init__.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from bump_pydantic.codemods.add_default_none import AddDefaultNoneCommand
 from bump_pydantic.codemods.field import FieldCodemod
 from bump_pydantic.codemods.replace_config import ReplaceConfigCodemod
 from bump_pydantic.codemods.replace_generic_model import ReplaceGenericModelCommand
 from bump_pydantic.codemods.replace_imports import ReplaceImportsCodemod
 from bump_pydantic.codemods.root_model import RootModelCommand
+from bump_pydantic.codemods.validator import ValidatorCodemod
 
 
 class Rule(str, Enum):
     BP001 = "BP001"
     """Add default `None` to `Optional[T]`, `Union[T, None]` and `Any` fields"""
     BP002 = "BP002"
     """Replace `Config` class with `model_config` attribute."""
@@ -21,14 +22,16 @@
     """Replace `Field` old parameters with new ones."""
     BP004 = "BP004"
     """Replace imports that have been moved."""
     BP005 = "BP005"
     """Replace `GenericModel` with `BaseModel`."""
     BP006 = "BP006"
     """Replace `BaseModel.__root__ = T` with `RootModel[T]`."""
+    BP007 = "BP007"
+    """Replace `@validator` with `@field_validator`."""
 
 
 def gather_codemods(disabled: List[Rule]) -> List[Type[ContextAwareTransformer]]:
     codemods: List[Type[ContextAwareTransformer]] = []
 
     if Rule.BP001 not in disabled:
         codemods.append(AddDefaultNoneCommand)
@@ -44,10 +47,13 @@
 
     if Rule.BP005 not in disabled:
         codemods.append(ReplaceGenericModelCommand)
 
     if Rule.BP006 not in disabled:
         codemods.append(RootModelCommand)
 
+    if Rule.BP007 not in disabled:
+        codemods.append(ValidatorCodemod)
+
     # Those codemods need to be the last ones.
     codemods.extend([RemoveImportsVisitor, AddImportsVisitor])
     return codemods
```

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/add_default_none.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/add_default_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/class_def_visitor.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/class_def_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/replace_config.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/replace_generic_model.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/replace_generic_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     @m.leave(m.ClassDef(bases=[m.ZeroOrMore(), GENERIC_MODEL_ARG, m.ZeroOrMore()]))
     def leave_generic_model(self, original_node: cst.ClassDef, updated_node: cst.ClassDef) -> cst.ClassDef:
         RemoveImportsVisitor.remove_unused_import(context=self.context, module="pydantic.generics", obj="GenericModel")
         RemoveImportsVisitor.remove_unused_import(context=self.context, module="pydantic", obj="generics")
         AddImportsVisitor.add_needed_import(context=self.context, module="pydantic", obj="BaseModel")
         return updated_node.with_changes(
             bases=[
-                base if not m.matches(base, GENERIC_MODEL_ARG) else cst.Arg(value=cst.Name("BaseModel"))
+                cst.Arg(value=cst.Name("BaseModel")) if m.matches(base, GENERIC_MODEL_ARG) else base
                 for base in updated_node.bases
             ]
         )
 
 
 if __name__ == "__main__":
     import textwrap
```

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/replace_imports.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/replace_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             if m.matches(updated_node, import_info.import_from):
                 aliases: Sequence[cst.ImportAlias] = updated_node.names  # type: ignore
                 # If multiple objects are imported in a single import statement,
                 # we need to remove only the one we're replacing.
                 AddImportsVisitor.add_needed_import(self.context, *import_info.to_import_str)
                 if len(updated_node.names) > 1:  # type: ignore
                     names = [alias for alias in aliases if alias.name.value != import_info.to_import_str[-1]]
+                    names[-1] = names[-1].with_changes(comma=cst.MaybeSentinel.DEFAULT)
                     updated_node = updated_node.with_changes(names=names)
                 else:
                     return cst.RemoveFromParent()  # type: ignore[return-value]
         return updated_node
 
 
 if __name__ == "__main__":
```

### Comparing `bump_pydantic-0.0.1/bump_pydantic/codemods/root_model.py` & `bump_pydantic-0.1.0/bump_pydantic/codemods/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/bump_pydantic/markers/find_base_model.py` & `bump_pydantic-0.1.0/bump_pydantic/markers/find_base_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/tests/integration/test_cli.py` & `bump_pydantic-0.1.0/tests/integration/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -125,23 +125,14 @@
                 "",
                 "",
                 "class B(BaseModel):",
                 "    class Config(BaseConfig):",
                 "        ...",
             ],
         ),
-        # File(
-        #     "rename_method.py",
-        #     content=[
-        #         "from project.add_none import A",
-        #         "",
-        #         'a = A(a=1, b=2, c=3, d=4, e={"ha": "ha"})',
-        #         "a.dict()",
-        #     ],
-        # ),
         File(
             "replace_generic.py",
             content=[
                 "from typing import Generic, TypeVar",
                 "",
                 "from pydantic.generics import GenericModel",
                 "",
@@ -167,30 +158,64 @@
             content=[
                 "from pydantic import BaseModel",
                 "",
                 "",
                 "class A(BaseModel):",
                 "    __root__ = int",
             ],
-        )
-        # File(
-        #     "config_dict_and_settings.py",
-        #     content=[
-        #         "from pydantic import BaseModel, BaseSettings",
-        #         "",
-        #         "",
-        #         "class Settings(BaseSettings):",
-        #         "    sentry_dsn: str",
-        #         "",
-        #         "",
-        #         "class A(BaseModel):",
-        #         "    class Config:",
-        #         "        orm_mode = True",
-        #     ]
-        # )
+        ),
+        File(
+            "replace_validator.py",
+            content=[
+                "from pydantic import BaseModel, validator, root_validator",
+                "",
+                "",
+                "class A(BaseModel):",
+                "    a: int",
+                "    b: str",
+                "",
+                "    @validator('a')",
+                "    def validate_a(cls, v):",
+                "        return v + 1",
+                "",
+                "    @root_validator()",
+                "    def validate_b(cls, values):",
+                "        return values",
+            ],
+        ),
+        File(
+            "const_to_literal.py",
+            content=[
+                "from enum import Enum",
+                "from pydantic import BaseModel, Field",
+                "",
+                "",
+                "class A(str, Enum):",
+                "    a = 'a'",
+                "    b = 'b'",
+                "",
+                "class A(BaseModel):",
+                "    a: A = Field(A.a, const=True)",
+            ],
+        ),
+        File(
+            "config_dict_and_settings.py",
+            content=[
+                "from pydantic import BaseModel, BaseSettings",
+                "",
+                "",
+                "class Settings(BaseSettings):",
+                "    sentry_dsn: str",
+                "",
+                "",
+                "class A(BaseModel):",
+                "    class Config:",
+                "        orm_mode = True",
+            ],
+        ),
     )
 
 
 @pytest.fixture()
 def expected() -> Folder:
     return Folder(
         "project",
@@ -239,23 +264,14 @@
                 "class B(BaseModel):",
                 "    # TODO[pydantic]: The `Config` class inherits from another class, please create the `model_config` manually.",  # noqa: E501
                 "    # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.",
                 "    class Config(BaseConfig):",
                 "        ...",
             ],
         ),
-        # File(
-        #     "rename_method.py",
-        #     content=[
-        #         "from project.add_none import A",
-        #         "",
-        #         'a = A(a=1, b=2, c=3, d=4, e={"ha": "ha"})',
-        #         "a.dict()",
-        #     ],
-        # ),
         File(
             "replace_generic.py",
             content=[
                 "from typing import Generic, TypeVar",
                 "from pydantic import BaseModel",
                 "",
                 "T = TypeVar('T')",
@@ -280,30 +296,67 @@
             content=[
                 "from pydantic import RootModel",
                 "",
                 "",
                 "class A(RootModel[int]):",
                 "    pass",
             ],
-        )
-        # File(
-        #     "config_dict_and_settings.py",
-        #     content=[
-        #         "from pydantic import ConfigDict, BaseModel",
-        #         "from pydantic_settings import BaseSettings",
-        #         "",
-        #         "",
-        #         "class Settings(BaseSettings):",
-        #         "    sentry_dsn: str",
-        #         "",
-        #         "",
-        #         "class A(BaseModel):",
-        #         "    model_config = ConfigDict(orm_mode=True)",
-        #     ]
-        # )
+        ),
+        File(
+            "replace_validator.py",
+            content=[
+                "from pydantic import field_validator, model_validator, BaseModel",
+                "",
+                "",
+                "class A(BaseModel):",
+                "    a: int",
+                "    b: str",
+                "",
+                "    @field_validator('a')",
+                "    @classmethod",
+                "    def validate_a(cls, v):",
+                "        return v + 1",
+                "",
+                "    @model_validator()",
+                "    @classmethod",
+                "    def validate_b(cls, values):",
+                "        return values",
+            ],
+        ),
+        File(
+            "const_to_literal.py",
+            content=[
+                "from enum import Enum",
+                "from pydantic import BaseModel",
+                "from typing import Literal",
+                "",
+                "",
+                "class A(str, Enum):",
+                "    a = 'a'",
+                "    b = 'b'",
+                "",
+                "class A(BaseModel):",
+                "    a: Literal[A.a] = A.a",
+            ],
+        ),
+        File(
+            "config_dict_and_settings.py",
+            content=[
+                "from pydantic import ConfigDict, BaseModel",
+                "from pydantic_settings import BaseSettings",
+                "",
+                "",
+                "class Settings(BaseSettings):",
+                "    sentry_dsn: str",
+                "",
+                "",
+                "class A(BaseModel):",
+                "    model_config = ConfigDict(from_attributes=True)",
+            ],
+        ),
     )
 
 
 def find_issue(current: Folder, expected: Folder) -> str:
     for current_file, expected_file in zip(current.files, expected.files):
         if current_file != expected_file:
             if current_file.name != expected_file.name:
```

### Comparing `bump_pydantic-0.0.1/tests/unit/test_add_default_none.py` & `bump_pydantic-0.1.0/tests/unit/test_add_default_none.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/tests/unit/test_class_def_visitor.py` & `bump_pydantic-0.1.0/tests/unit/test_class_def_visitor.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/tests/unit/test_field.py` & `bump_pydantic-0.1.0/tests/unit/test_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from libcst.codemod import CodemodTest
 
 from bump_pydantic.codemods.field import FieldCodemod
 
 
-class TestReplaceConfigCommand(CodemodTest):
+class TestFieldCommand(CodemodTest):
     TRANSFORM = FieldCodemod
 
     maxDiff = None
 
     def test_field_rename(self) -> None:
         before = """
         from pydantic import BaseModel, Field
@@ -70,7 +70,35 @@
         code = """
         from pydantic import BaseModel, Field
 
         class Potato(BaseModel):
             potato: int = Field(..., env="POTATO")
         """
         self.assertCodemod(code, code)
+
+    def test_replace_const_by_literal_type(self) -> None:
+        before = """
+        from enum import Enum
+
+        from pydantic import BaseModel, Field
+
+
+        class MyEnum(Enum):
+            POTATO = "potato"
+
+        class Potato(BaseModel):
+            potato: MyEnum = Field(MyEnum.POTATO, const=True)
+        """
+        after = """
+        from enum import Enum
+
+        from pydantic import BaseModel
+        from typing import Literal
+
+
+        class MyEnum(Enum):
+            POTATO = "potato"
+
+        class Potato(BaseModel):
+            potato: Literal[MyEnum.POTATO] = MyEnum.POTATO
+        """
+        self.assertCodemod(before, after)
```

### Comparing `bump_pydantic-0.0.1/tests/unit/test_generic_model.py` & `bump_pydantic-0.1.0/tests/unit/test_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/tests/unit/test_replace_config.py` & `bump_pydantic-0.1.0/tests/unit/test_replace_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             # TODO[pydantic]: The `Config` class inherits from another class, please create the `model_config` manually.
             # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
             class Config(SuperConfig):
                 allow_arbitrary_types = True
         """
         self.assertCodemod(before, after)
 
-    @pytest.mark.xfail(reason="Not implemented yet")
+    @pytest.mark.xfail(reason="Comments inside Config are swallowed.")
     def test_inner_comments(self) -> None:
         before = """
         from pydantic import BaseModel
 
         class Potato(BaseModel):
             class Config:
                 # This is a comment
@@ -172,25 +172,24 @@
             # TODO[pydantic]: The `Config` class inherits from another class, please create the `model_config` manually.
             # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
             class Config(SuperConfig):
                 allow_arbitrary_types = True
         """
         self.assertCodemod(before, after)
 
-    @pytest.mark.xfail(reason="Not implemented yet")
     def test_extra_enum(self) -> None:
         before = """
         from pydantic import BaseModel, Extra
 
         class Potato(BaseModel):
             class Config:
                 extra = Extra.allow
         """
         after = """
-        from pydantic import BaseModel
+        from pydantic import ConfigDict, BaseModel
 
         class Potato(BaseModel):
             model_config = ConfigDict(extra="allow")
         """
         self.assertCodemod(before, after)
 
     def test_removed_keys(self) -> None:
```

### Comparing `bump_pydantic-0.0.1/tests/unit/test_replace_imports.py` & `bump_pydantic-0.1.0/tests/unit/test_replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/tests/unit/test_root_model.py` & `bump_pydantic-0.1.0/tests/unit/test_root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/.gitignore` & `bump_pydantic-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/LICENSE.txt` & `bump_pydantic-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/pyproject.toml` & `bump_pydantic-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.0.1/PKG-INFO` & `bump_pydantic-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-pydantic
-Version: 0.0.1
+Version: 0.1.0
 Summary: Convert Pydantic from V1 to V2 ♻
 Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
 Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
 Project-URL: Source, https://github.com/pydantic/bump-pydantic
 Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -49,14 +49,16 @@
     - [BP001: Add default `None` to `Optional[T]`, `Union[T, None]` and `Any` fields](#bp001-add-default-none-to-optionalt-uniont-none-and-any-fields)
     - [BP002: Replace `Config` class by `model_config` attribute](#bp002-replace-config-class-by-model_config-attribute)
     - [BP003: Replace `Field` old parameters to new ones](#bp003-replace-field-old-parameters-to-new-ones)
     - [BP004: Replace imports](#bp004-replace-imports)
     - [BP003: Replace `Config` class by `model_config`](#bp003-replace-config-class-by-model_config)
     - [BP005: Replace `GenericModel` by `BaseModel`](#bp005-replace-genericmodel-by-basemodel)
     - [BP006: Replace `__root__` by `RootModel`](#bp006-replace-__root__-by-rootmodel)
+    - [BP007: Replace decorators](#bp007-replace-decorators)
+    - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter)
   - [License](#license)
 
 ---
 
 ## Installation
 
 The installation is as simple as:
@@ -148,14 +150,15 @@
 
     model_config = ConfigDict(extra="forbid")
 ```
 
 ### BP003: Replace `Field` old parameters to new ones
 
 - ✅ Replace `Field` old parameters to new ones.
+- ✅ Replace `field: Enum = Field(Enum.VALUE, const=True)` by `field: Literal[Enum.VALUE] = Enum.VALUE`.
 
 The following code will be transformed:
 
 ```py
 from typing import List
 
 from pydantic import BaseModel, Field
@@ -262,12 +265,96 @@
     age: int
     name: str
 
 class Users(RootModel[List[User]]):
     pass
 ```
 
+### BP007: Replace decorators
+
+- ✅ Replace `@validator` by `@field_validator`.
+- ✅ Replace `@root_validator` by `@model_validator`.
+
+The following code will be transformed:
+
+```py
+from pydantic import BaseModel, validator, root_validator
+
+
+class User(BaseModel):
+    name: str
+
+    @validator('name', pre=True)
+    def validate_name(cls, v):
+        return v
+
+    @root_validator(pre=True)
+    def validate_root(cls, values):
+        return values
+```
+
+Into:
+
+```py
+from pydantic import BaseModel, field_validator, model_validator
+
+
+class User(BaseModel):
+    name: str
+
+    @field_validator('name', mode='before')
+    def validate_name(cls, v):
+        return v
+
+    @model_validator(mode='before')
+    def validate_root(cls, values):
+        return values
+```
+
+### BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
+
+- ✅ Replace `pydantic.parse_obj_as(T, obj)` to `pydantic.TypeAdapter(T).validate_python(obj)`.
+
+
+The following code will be transformed:
+
+```py
+from typing import List
+
+from pydantic import BaseModel, parse_obj_as
+
+
+class User(BaseModel):
+    name: str
+
+
+class Users(BaseModel):
+    users: List[User]
+
+
+users = parse_obj_as(Users, {'users': [{'name': 'John'}]})
+```
+
+Into:
+
+```py
+from typing import List
+
+from pydantic import BaseModel, TypeAdapter
+
+
+class User(BaseModel):
+    name: str
+
+
+class Users(BaseModel):
+    users: List[User]
+
+
+users = TypeAdapter(Users).validate_python({'users': [{'name': 'John'}]})
+```
+
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

