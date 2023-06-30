# Comparing `tmp/ibis-substrait-2.9.7.tar.gz` & `tmp/ibis-substrait-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis-substrait-2.9.7.tar", max compression
+gzip compressed data, was "ibis-substrait-2.9.8.tar", max compression
```

## Comparing `ibis-substrait-2.9.7.tar` & `ibis-substrait-2.9.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11345 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/LICENSE
--rw-r--r--   0        0        0      171 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/README.md
--rw-r--r--   0        0        0       22 2022-08-09 23:09:36.598341 ibis-substrait-2.9.7/ibis_substrait/__init__.py
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/compiler/__init__.py
--rw-r--r--   0        0        0     5925 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/compiler/core.py
--rw-r--r--   0        0        0    34687 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/compiler/decompile.py
--rw-r--r--   0        0        0     1004 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/compiler/mapping.py
--rw-r--r--   0        0        0    29730 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/compiler/translate.py
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/proto/__init__.py
--rw-r--r--   0        0        0       24 2022-08-09 23:08:12.842040 ibis-substrait-2.9.7/ibis_substrait/proto/__init__.pyi
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/__init__.py
--rw-r--r--   0        0        0       19 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/__init__.pyi
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/__init__.py
--rw-r--r--   0        0        0      228 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/__init__.pyi
--rw-r--r--   0        0        0    42349 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/algebra_pb2.py
--rw-r--r--   0        0        0   127324 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/algebra_pb2.pyi
--rw-r--r--   0        0        0     1596 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/capabilities_pb2.py
--rw-r--r--   0        0        0     3200 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/capabilities_pb2.pyi
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/extensions/__init__.py
--rw-r--r--   0        0        0       29 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/extensions/__init__.pyi
--rw-r--r--   0        0        0     3225 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.py
--rw-r--r--   0        0        0     7467 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.pyi
--rw-r--r--   0        0        0     7968 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/function_pb2.py
--rw-r--r--   0        0        0    20854 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/function_pb2.pyi
--rw-r--r--   0        0        0     8723 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.py
--rw-r--r--   0        0        0    20409 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.pyi
--rw-r--r--   0        0        0     1930 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/plan_pb2.py
--rw-r--r--   0        0        0     4328 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/plan_pb2.pyi
--rw-r--r--   0        0        0    10711 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.py
--rw-r--r--   0        0        0    26952 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.pyi
--rw-r--r--   0        0        0    11524 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_pb2.py
--rw-r--r--   0        0        0    28613 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_pb2.pyi
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/compiler/__init__.py
--rw-r--r--   0        0        0     4478 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/compiler/conftest.py
--rw-r--r--   0        0        0    10441 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_compiler.py
--rw-r--r--   0        0        0     8377 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_decompiler.py
--rw-r--r--   0        0        0    13822 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_literal.py
--rw-r--r--   0        0        0    23097 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_tpch.py
--rw-r--r--   0        0        0      175 2022-08-09 23:08:12.846040 ibis-substrait-2.9.7/ibis_substrait/tests/conftest.py
--rw-r--r--   0        0        0     2690 2022-08-09 23:09:38.574348 ibis-substrait-2.9.7/pyproject.toml
--rw-r--r--   0        0        0     1153 2022-08-09 23:09:39.430075 ibis-substrait-2.9.7/setup.py
--rw-r--r--   0        0        0     1187 2022-08-09 23:09:39.430414 ibis-substrait-2.9.7/PKG-INFO
+-rw-r--r--   0        0        0    11345 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/LICENSE
+-rw-r--r--   0        0        0      171 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/README.md
+-rw-r--r--   0        0        0       22 2022-08-10 19:32:23.579247 ibis-substrait-2.9.8/ibis_substrait/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/__init__.py
+-rw-r--r--   0        0        0     5925 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/core.py
+-rw-r--r--   0        0        0    34687 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/decompile.py
+-rw-r--r--   0        0        0     1004 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/mapping.py
+-rw-r--r--   0        0        0    29928 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/translate.py
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/__init__.py
+-rw-r--r--   0        0        0       24 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/__init__.py
+-rw-r--r--   0        0        0       19 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/__init__.py
+-rw-r--r--   0        0        0      228 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/__init__.pyi
+-rw-r--r--   0        0        0    42349 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/algebra_pb2.py
+-rw-r--r--   0        0        0   127324 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/algebra_pb2.pyi
+-rw-r--r--   0        0        0     1596 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/capabilities_pb2.py
+-rw-r--r--   0        0        0     3200 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/capabilities_pb2.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/__init__.py
+-rw-r--r--   0        0        0       29 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/__init__.pyi
+-rw-r--r--   0        0        0     3225 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.py
+-rw-r--r--   0        0        0     7467 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.pyi
+-rw-r--r--   0        0        0     7968 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/function_pb2.py
+-rw-r--r--   0        0        0    20854 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/function_pb2.pyi
+-rw-r--r--   0        0        0     8723 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.py
+-rw-r--r--   0        0        0    20409 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.pyi
+-rw-r--r--   0        0        0     1930 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/plan_pb2.py
+-rw-r--r--   0        0        0     4328 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/plan_pb2.pyi
+-rw-r--r--   0        0        0    10711 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.py
+-rw-r--r--   0        0        0    26952 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.pyi
+-rw-r--r--   0        0        0    11524 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_pb2.py
+-rw-r--r--   0        0        0    28613 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_pb2.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/__init__.py
+-rw-r--r--   0        0        0     4478 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/conftest.py
+-rw-r--r--   0        0        0    10441 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_compiler.py
+-rw-r--r--   0        0        0     8962 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_decompiler.py
+-rw-r--r--   0        0        0    13822 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_literal.py
+-rw-r--r--   0        0        0    23098 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_tpch.py
+-rw-r--r--   0        0        0      175 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/conftest.py
+-rw-r--r--   0        0        0     2690 2022-08-10 19:32:25.615230 ibis-substrait-2.9.8/pyproject.toml
+-rw-r--r--   0        0        0     1153 2022-08-10 19:32:26.480906 ibis-substrait-2.9.8/setup.py
+-rw-r--r--   0        0        0     1187 2022-08-10 19:32:26.481247 ibis-substrait-2.9.8/PKG-INFO
```

### Comparing `ibis-substrait-2.9.7/LICENSE` & `ibis-substrait-2.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/compiler/core.py` & `ibis-substrait-2.9.8/ibis_substrait/compiler/core.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/compiler/decompile.py` & `ibis-substrait-2.9.8/ibis_substrait/compiler/decompile.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/compiler/mapping.py` & `ibis-substrait-2.9.8/ibis_substrait/compiler/mapping.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/compiler/translate.py` & `ibis-substrait-2.9.8/ibis_substrait/compiler/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -794,21 +794,24 @@
 @translate.register(ops.Join)
 def join(
     op: ops.Join,
     expr: ir.TableExpr,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Rel:
+    child_rel_field_offsets = kwargs.pop("child_rel_field_offsets", None)
     return stalg.Rel(
         join=stalg.JoinRel(
             left=translate(op.left, compiler, **kwargs),
             right=translate(op.right, compiler, **kwargs),
             expression=translate(
                 functools.reduce(operator.and_, op.predicates),
                 compiler,
+                child_rel_field_offsets=child_rel_field_offsets
+                or _get_child_relation_field_offsets(expr),
                 **kwargs,
             ),
             type=_translate_join_type(op),
         )
     )
```

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/algebra_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/algebra_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/algebra_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/algebra_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/capabilities_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/capabilities_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/capabilities_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/function_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/function_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/function_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/plan_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/plan_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/plan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_pb2.py` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_pb2.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/proto/substrait/ibis/type_pb2.pyi` & `ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/tests/compiler/conftest.py` & `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/conftest.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_compiler.py` & `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_decompiler.py` & `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_decompiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,24 @@
 
 
 @pytest.fixture
 def s():
     return ibis.table([("c", "string"), ("d", "int64")], name="s")
 
 
+@pytest.fixture
+def r():
+    return ibis.table([("a", "string"), ("b", "int64")], name="r")
+
+
+@pytest.fixture
+def q():
+    return ibis.table([("e", "string"), ("f", "int64")], name="q")
+
+
 @pytest.mark.parametrize(
     "expr_fn",
     [
         pytest.param(lambda t: t, id="read_rel"),
         pytest.param(
             # TODO: ibis: compare .type() instead of dtype on literals
             lambda t: t[t.d == ibis.literal(1, type="int64")],
@@ -277,7 +287,24 @@
 )
 def test_extract_date(compiler, span):
     t = ibis.table([("o_orderdate", dt.date)], name="t")
     expr = t[getattr(t.o_orderdate, span)()]
     plan = compiler.compile(expr)
     (result,) = decompile(plan)
     assert result.equals(expr)
+
+
+def test_roundtrip_join(compiler, s, r):
+    expr = s.join(r, s.c == r.a)
+
+    plan = compiler.compile(expr)
+    (result,) = decompile(plan)
+    assert result.equals(expr)
+
+
+def test_roundtrip_nested_join(compiler, s, r, q):
+    expr = s.join(r, s.c == r.a)
+    expr = expr.join(q, expr.a == q.e)
+
+    plan = compiler.compile(expr)
+    (result,) = decompile(plan)
+    assert result.equals(expr)
```

### Comparing `ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_literal.py` & `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_literal.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.7/ibis_substrait/tests/compiler/test_tpch.py` & `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_tpch.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,15 +685,15 @@
             raises=TypeError,
             reason="protobuf error resulting subquery (cannot merge Expression and AggregateFunction)",  # noqa
         ),
     ),
     pytest.param(
         lazy_fixture("tpc_h15"),
         marks=pytest.mark.xfail(
-            raises=AssertionError, reason="non-empty child offsets"
+            raises=KeyError, reason="TableArrayView not implemented"
         ),
     ),
     pytest.param(
         lazy_fixture("tpc_h16"),
         marks=pytest.mark.xfail(
             raises=TypeError, reason="IntegerColumn is not iterable"
         ),
```

### Comparing `ibis-substrait-2.9.7/pyproject.toml` & `ibis-substrait-2.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ibis-substrait"
-version = "2.9.7"
+version = "2.9.8"
 packages = [{ include = "ibis_substrait" }]
 homepage = "https://github.com/ibis-project/ibis-substrait"
 repository = "https://github.com/ibis-project/ibis-substrait"
 description = "Subtrait compiler for ibis"
 authors = ["Ibis Contributors"]
 maintainers = ["Ibis Contributors"]
 license = "Apache-2.0"
```

### Comparing `ibis-substrait-2.9.7/setup.py` & `ibis-substrait-2.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['ibis-framework>=2,<4',
  'packaging>=21.3,<22.0',
  'platformdirs<2.5.3',
  'protobuf==3.20.1']
 
 setup_kwargs = {
     'name': 'ibis-substrait',
-    'version': '2.9.7',
+    'version': '2.9.8',
     'description': 'Subtrait compiler for ibis',
     'long_description': "# [Ibis](https://ibis-project.org) + [Substrait](https://substrait.io)\n\nThis repo houses the Substrait compiler for ibis.\n\nWe're just getting started here, so stay tuned!\n",
     'author': 'Ibis Contributors',
     'author_email': None,
     'maintainer': 'Ibis Contributors',
     'maintainer_email': None,
     'url': 'https://github.com/ibis-project/ibis-substrait',
```

### Comparing `ibis-substrait-2.9.7/PKG-INFO` & `ibis-substrait-2.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-substrait
-Version: 2.9.7
+Version: 2.9.8
 Summary: Subtrait compiler for ibis
 Home-page: https://github.com/ibis-project/ibis-substrait
 License: Apache-2.0
 Author: Ibis Contributors
 Maintainer: Ibis Contributors
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

