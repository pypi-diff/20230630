# Comparing `tmp/rvtools-0.1.4.tar.gz` & `tmp/rvtools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvtools-0.1.4.tar", max compression
+gzip compressed data, was "rvtools-0.1.5.tar", max compression
```

## Comparing `rvtools-0.1.4.tar` & `rvtools-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,41 @@
--rw-r--r--   0        0        0     5605 2023-06-28 13:10:40.461684 rvtools-0.1.4/README.md
--rw-r--r--   0        0        0      900 2023-06-28 13:11:21.607506 rvtools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      264 2023-06-28 11:35:59.919900 rvtools-0.1.4/rvtools/__init__.py
--rw-r--r--   0        0        0      272 2023-06-28 12:42:43.459690 rvtools-0.1.4/rvtools/construct/__init__.py
--rw-r--r--   0        0        0      584 2023-06-28 12:42:44.064856 rvtools-0.1.4/rvtools/construct/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2573 2023-06-25 22:21:36.090266 rvtools-0.1.4/rvtools/construct/__pycache__/_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     2768 2023-06-26 22:48:02.435671 rvtools-0.1.4/rvtools/construct/__pycache__/beta.cpython-311.pyc
--rw-r--r--   0        0        0     3798 2023-06-26 22:48:02.436259 rvtools-0.1.4/rvtools/construct/__pycache__/lognorm.cpython-311.pyc
--rw-r--r--   0        0        0     2457 2023-06-28 13:08:31.007828 rvtools-0.1.4/rvtools/construct/__pycache__/loguniform.cpython-311.pyc
--rw-r--r--   0        0        0     2764 2023-06-26 22:48:02.436685 rvtools-0.1.4/rvtools/construct/__pycache__/norm.cpython-311.pyc
--rw-r--r--   0        0        0     2641 2023-06-26 22:48:02.437087 rvtools-0.1.4/rvtools/construct/__pycache__/uniform.cpython-311.pyc
--rw-r--r--   0        0        0     1535 2023-06-25 22:20:41.612198 rvtools-0.1.4/rvtools/construct/_helpers.py
--rw-r--r--   0        0        0     1477 2023-06-26 22:48:01.909872 rvtools-0.1.4/rvtools/construct/beta.py
--rw-r--r--   0        0        0     2127 2023-06-26 22:48:01.906834 rvtools-0.1.4/rvtools/construct/lognorm.py
--rw-r--r--   0        0        0     1285 2023-06-28 13:08:30.232208 rvtools-0.1.4/rvtools/construct/loguniform.py
--rw-r--r--   0        0        0     1258 2023-06-26 22:48:01.911084 rvtools-0.1.4/rvtools/construct/norm.py
--rw-r--r--   0        0        0     1437 2023-06-26 22:48:01.914585 rvtools-0.1.4/rvtools/construct/uniform.py
--rw-r--r--   0        0        0      126 2023-06-26 20:21:17.331337 rvtools-0.1.4/rvtools/distributions/__init__.py
--rw-r--r--   0        0        0      358 2023-06-26 20:21:36.589514 rvtools-0.1.4/rvtools/distributions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1726 2023-06-26 18:36:15.269055 rvtools-0.1.4/rvtools/distributions/__pycache__/certainty.cpython-311.pyc
--rw-r--r--   0        0        0     8408 2023-06-26 20:16:33.256135 rvtools-0.1.4/rvtools/distributions/__pycache__/tp_uniform.cpython-311.pyc
--rw-r--r--   0        0        0      854 2023-06-26 18:23:58.213480 rvtools-0.1.4/rvtools/distributions/certainty.py
--rw-r--r--   0        0        0     5151 2023-06-26 20:16:32.712477 rvtools-0.1.4/rvtools/distributions/tp_uniform.py
--rw-r--r--   0        0        0      556 2023-06-26 21:58:51.980313 rvtools-0.1.4/rvtools/types.py
--rw-r--r--   0        0        0        0 2023-06-25 18:12:13.995575 rvtools-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      507 2023-06-26 20:21:17.339335 rvtools-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0      339 2023-06-25 21:11:58.259220 rvtools-0.1.4/tests/test_certainty.py
--rw-r--r--   0        0        0     5679 2023-06-28 13:10:57.477667 rvtools-0.1.4/tests/test_constructors.py
--rw-r--r--   0        0        0      274 2023-06-25 23:03:01.270501 rvtools-0.1.4/tests/test_docs_do_not_raise.py
--rw-r--r--   0        0        0     2159 2023-06-26 22:48:01.912458 rvtools-0.1.4/tests/test_parse_spec.py
--rw-r--r--   0        0        0     4264 2023-06-26 22:48:01.908527 rvtools-0.1.4/tests/test_tp_uniform.py
--rw-r--r--   0        0        0      513 2023-06-26 21:58:51.980481 rvtools-0.1.4/tests/test_types.py
--rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 rvtools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1571 2023-06-30 18:44:54.787213 rvtools-0.1.5/README.md
+-rw-r--r--   0        0        0      950 2023-06-30 18:55:08.005404 rvtools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-30 17:26:45.549942 rvtools-0.1.5/rvtools/__init__.py
+-rw-r--r--   0        0        0      408 2023-06-30 18:31:20.324526 rvtools-0.1.5/rvtools/construct/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-30 18:31:21.355889 rvtools-0.1.5/rvtools/construct/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2573 2023-06-25 22:21:36.090266 rvtools-0.1.5/rvtools/construct/__pycache__/_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     3390 2023-06-30 17:10:00.426276 rvtools-0.1.5/rvtools/construct/__pycache__/beta.cpython-311.pyc
+-rw-r--r--   0        0        0     4740 2023-06-30 18:19:29.450911 rvtools-0.1.5/rvtools/construct/__pycache__/lognorm.cpython-311.pyc
+-rw-r--r--   0        0        0     3133 2023-06-30 17:16:00.201884 rvtools-0.1.5/rvtools/construct/__pycache__/loguniform.cpython-311.pyc
+-rw-r--r--   0        0        0     3376 2023-06-30 17:14:17.612857 rvtools-0.1.5/rvtools/construct/__pycache__/norm.cpython-311.pyc
+-rw-r--r--   0        0        0     1136 2023-06-30 18:49:53.018755 rvtools-0.1.5/rvtools/construct/__pycache__/pert.cpython-311.pyc
+-rw-r--r--   0        0        0     1236 2023-06-30 18:49:53.019105 rvtools-0.1.5/rvtools/construct/__pycache__/tp_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     3424 2023-06-30 17:16:00.201337 rvtools-0.1.5/rvtools/construct/__pycache__/uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     1535 2023-06-25 22:20:41.612198 rvtools-0.1.5/rvtools/construct/_helpers.py
+-rw-r--r--   0        0        0     2103 2023-06-30 17:09:58.826501 rvtools-0.1.5/rvtools/construct/beta.py
+-rw-r--r--   0        0        0     3073 2023-06-30 18:08:07.135992 rvtools-0.1.5/rvtools/construct/lognorm.py
+-rw-r--r--   0        0        0     1965 2023-06-30 17:15:58.797323 rvtools-0.1.5/rvtools/construct/loguniform.py
+-rw-r--r--   0        0        0     1880 2023-06-30 17:13:21.148678 rvtools-0.1.5/rvtools/construct/norm.py
+-rw-r--r--   0        0        0      785 2023-06-30 18:36:45.614328 rvtools-0.1.5/rvtools/construct/pert.py
+-rw-r--r--   0        0        0      837 2023-06-30 18:36:45.610762 rvtools-0.1.5/rvtools/construct/tp_uniform.py
+-rw-r--r--   0        0        0     2224 2023-06-30 17:15:58.794493 rvtools-0.1.5/rvtools/construct/uniform.py
+-rw-r--r--   0        0        0      628 2023-06-30 18:22:52.877475 rvtools-0.1.5/rvtools/dists/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-30 18:24:18.881448 rvtools-0.1.5/rvtools/dists/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-06-30 14:37:51.404420 rvtools-0.1.5/rvtools/dists/gen/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-30 14:37:52.815093 rvtools-0.1.5/rvtools/dists/gen/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2123 2023-06-30 17:34:43.838362 rvtools-0.1.5/rvtools/dists/gen/__pycache__/certainty.cpython-311.pyc
+-rw-r--r--   0        0        0     2766 2023-06-30 17:34:43.837781 rvtools-0.1.5/rvtools/dists/gen/__pycache__/halves_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     7374 2023-06-30 17:34:43.837034 rvtools-0.1.5/rvtools/dists/gen/__pycache__/tp_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2023-06-30 17:26:45.575234 rvtools-0.1.5/rvtools/dists/gen/certainty.py
+-rw-r--r--   0        0        0     1350 2023-06-30 17:26:45.578709 rvtools-0.1.5/rvtools/dists/gen/halves_uniform.py
+-rw-r--r--   0        0        0     5244 2023-06-30 17:26:45.610428 rvtools-0.1.5/rvtools/dists/gen/tp_uniform.py
+-rw-r--r--   0        0        0     1257 2023-06-30 17:26:45.575868 rvtools-0.1.5/rvtools/fam.py
+-rw-r--r--   0        0        0        0 2023-06-25 18:12:13.995575 rvtools-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-30 16:50:57.527151 rvtools-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      345 2023-06-30 17:22:10.404617 rvtools-0.1.5/tests/test_certainty.py
+-rw-r--r--   0        0        0     5745 2023-06-29 15:12:37.194609 rvtools-0.1.5/tests/test_constructors.py
+-rw-r--r--   0        0        0     2159 2023-06-26 22:48:01.912458 rvtools-0.1.5/tests/test_parse_spec.py
+-rw-r--r--   0        0        0      256 2023-06-30 17:25:47.032459 rvtools-0.1.5/tests/test_readme_does_not_raise.py
+-rw-r--r--   0        0        0     4440 2023-06-30 17:21:54.412641 rvtools-0.1.5/tests/test_tp_uniform.py
+-rw-r--r--   0        0        0      943 2023-06-30 17:26:45.583827 rvtools-0.1.5/tests/test_types.py
+-rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 rvtools-0.1.5/PKG-INFO
```

### Comparing `rvtools-0.1.4/pyproject.toml` & `rvtools-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "rvtools"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/tadamcz/rvtools"
 description = "Top-level package for Probability distribution and random variable tools."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
@@ -13,25 +13,27 @@
 packages = [
     { include = "rvtools" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-betapert = "^0.1.2"
-copula-wrapper = "^0.1.1"
+betapert = "^0.1.4"
+copula-wrapper = "^0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "*"
 coverage = "*"
 pytest = ">=7.2.0"
 pytest-pycharm = "*"
 black = {extras = ["d"], version = "*"}
 mkcodes = "^0.1.1"
 matplotlib = "^3.7.1"
+sphinx = "^7.0.1"
+sphinx-autobuild = "^2021.3.14"
 
 
 
 [tool.black]
 line-length = 100
 
 [build-system]
```

### Comparing `rvtools-0.1.4/rvtools/construct/__pycache__/__init__.cpython-311.pyc` & `rvtools-0.1.5/rvtools/construct/__pycache__/__init__.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xc32a9c64 (Wed Jun 28 12:42:43 2023 UTC)
-files sz: 272
+moddate:  0x781f9f64 (Fri Jun 30 18:31:20 2023 UTC)
+files sz: 408
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a070100640064056c086d095a
-      090100640064066c0a6d0b5a0b010064075300
+      090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d0100640064
+      086c0e6d0f5a0f0100640064096c106d115a110100640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('CopulaJoint',))
                  6 IMPORT_NAME              0 (copula_wrapper)
                  8 IMPORT_FROM              1 (CopulaJoint)
                 10 STORE_NAME               1 (CopulaJoint)
@@ -49,26 +50,50 @@
    
      7          62 LOAD_CONST               0 (0)
                 64 LOAD_CONST               6 (('loguniform',))
                 66 IMPORT_NAME             10 (rvtools.construct.loguniform)
                 68 IMPORT_FROM             11 (loguniform)
                 70 STORE_NAME              11 (loguniform)
                 72 POP_TOP
-                74 LOAD_CONST               7 (None)
-                76 RETURN_VALUE
+   
+     8          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               7 (('pert',))
+                78 IMPORT_NAME             12 (rvtools.construct.pert)
+                80 IMPORT_FROM             13 (pert)
+                82 STORE_NAME              13 (pert)
+                84 POP_TOP
+   
+     9          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               8 (('tp_uniform',))
+                90 IMPORT_NAME             14 (rvtools.construct.tp_uniform)
+                92 IMPORT_FROM             15 (tp_uniform)
+                94 STORE_NAME              15 (tp_uniform)
+                96 POP_TOP
+   
+    10          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               9 (('certainty',))
+               102 IMPORT_NAME             16 (rvtools.dists)
+               104 IMPORT_FROM             17 (certainty)
+               106 STORE_NAME              17 (certainty)
+               108 POP_TOP
+               110 LOAD_CONST              10 (None)
+               112 RETURN_VALUE
    consts
       0
       ('CopulaJoint',)
       ('beta',)
       ('lognorm',)
       ('norm',)
       ('uniform',)
       ('loguniform',)
+      ('pert',)
+      ('tp_uniform',)
+      ('certainty',)
       None
-   names      ('copula_wrapper', 'CopulaJoint', 'rvtools.construct.beta', 'beta', 'rvtools.construct.lognorm', 'lognorm', 'rvtools.construct.norm', 'norm', 'rvtools.construct.uniform', 'uniform', 'rvtools.construct.loguniform', 'loguniform')
+   names      ('copula_wrapper', 'CopulaJoint', 'rvtools.construct.beta', 'beta', 'rvtools.construct.lognorm', 'lognorm', 'rvtools.construct.norm', 'norm', 'rvtools.construct.uniform', 'uniform', 'rvtools.construct.loguniform', 'loguniform', 'rvtools.construct.pert', 'pert', 'rvtools.construct.tp_uniform', 'tp_uniform', 'rvtools.dists', 'certainty')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/t/repos/rvtools/rvtools/construct/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c020c010c010c010c01
+   lnotab 0x00ff02010c020c010c010c010c010c010c010c01
```

### Comparing `rvtools-0.1.4/rvtools/construct/__pycache__/_helpers.cpython-311.pyc` & `rvtools-0.1.5/rvtools/construct/__pycache__/_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.4/rvtools/construct/__pycache__/beta.cpython-311.pyc` & `rvtools-0.1.5/rvtools/construct/__pycache__/beta.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
-files sz: 1477
+moddate:  0x660c9f64 (Fri Jun 30 17:09:58 2023 UTC)
+files sz: 2103
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a03640064026c045a
@@ -52,22 +52,22 @@
                 66 BUILD_TUPLE              2
                 68 BINARY_SUBSCR
                 78 BUILD_TUPLE              6
                 80 LOAD_CONST               8 (<code object beta, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 9>)
                 82 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                 84 STORE_NAME               8 (beta)
    
-    19          86 LOAD_CONST               7 ('quantiles')
+    38          86 LOAD_CONST               7 ('quantiles')
                 88 LOAD_NAME                7 (dict)
                 90 LOAD_NAME                1 (Real)
                 92 LOAD_NAME                1 (Real)
                 94 BUILD_TUPLE              2
                 96 BINARY_SUBSCR
                106 BUILD_TUPLE              2
-               108 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 19>)
+               108 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 38>)
                110 MAKE_FUNCTION            4 (annotations)
                112 STORE_NAME               9 (from_quantiles)
                114 LOAD_CONST               2 (None)
                116 RETURN_VALUE
    consts
       0
       ('Real',)
@@ -79,95 +79,96 @@
       'quantiles'
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 7
          flags     : 11
          code
-            0x970074010000000000000000000064067c007c017c0264019c037c03a4
+            0x970074010000000000000000000064077c007c017c0264019c037c03a4
             018e017d047c04a0010000000000000000000000000000000000000000a6
             000000ab0000000000000000006402640368026b02000000007220740400
             0000000000000000006a030000000000000000a004000000000000000000
             00000000000000000000007c007c01a6020000ab02000000000000000053
             007c04a0010000000000000000000000000000000000000000a6000000ab
             000000000000000000640468016b02000000007215740b00000000000000
             0000007c04640419000000000000000000a6010000ab0100000000000000
             005300740d000000000000000000006405a6010000ab0100000000000000
             008201
            9           0 RESUME                   0
          
-          10           2 LOAD_GLOBAL              1 (NULL + parse_spec)
-                      14 LOAD_CONST               6 (())
+          29           2 LOAD_GLOBAL              1 (NULL + parse_spec)
+                      14 LOAD_CONST               7 (())
                       16 LOAD_FAST                0 (alpha)
                       18 LOAD_FAST                1 (beta)
                       20 LOAD_FAST                2 (quantiles)
                       22 LOAD_CONST               1 (('alpha', 'beta', 'quantiles'))
                       24 BUILD_CONST_KEY_MAP      3
                       26 LOAD_FAST                3 (kwargs)
                       28 DICT_MERGE               1
                       30 CALL_FUNCTION_EX         1
                       32 STORE_FAST               4 (spec)
          
-          11          34 LOAD_FAST                4 (spec)
+          30          34 LOAD_FAST                4 (spec)
                       36 LOAD_METHOD              1 (keys)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 LOAD_CONST               2 ('alpha')
                       74 LOAD_CONST               3 ('beta')
                       76 BUILD_SET                2
                       78 COMPARE_OP               2 (==)
                       84 POP_JUMP_FORWARD_IF_FALSE    32 (to 150)
          
-          12          86 LOAD_GLOBAL              4 (scipy)
+          31          86 LOAD_GLOBAL              4 (scipy)
                       98 LOAD_ATTR                3 (stats)
                      108 LOAD_METHOD              4 (beta)
                      130 LOAD_FAST                0 (alpha)
                      132 LOAD_FAST                1 (beta)
                      134 PRECALL                  2
                      138 CALL                     2
                      148 RETURN_VALUE
          
-          13     >>  150 LOAD_FAST                4 (spec)
+          32     >>  150 LOAD_FAST                4 (spec)
                      152 LOAD_METHOD              1 (keys)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 LOAD_CONST               4 ('quantiles')
                      190 BUILD_SET                1
                      192 COMPARE_OP               2 (==)
                      198 POP_JUMP_FORWARD_IF_FALSE    21 (to 242)
          
-          14         200 LOAD_GLOBAL             11 (NULL + from_quantiles)
+          33         200 LOAD_GLOBAL             11 (NULL + from_quantiles)
                      212 LOAD_FAST                4 (spec)
                      214 LOAD_CONST               4 ('quantiles')
                      216 BINARY_SUBSCR
                      226 PRECALL                  1
                      230 CALL                     1
                      240 RETURN_VALUE
          
-          16     >>  242 LOAD_GLOBAL             13 (NULL + ValueError)
+          35     >>  242 LOAD_GLOBAL             13 (NULL + ValueError)
                      254 LOAD_CONST               5 ("You must specify either 'alpha' and 'beta', or 'quantiles'.")
                      256 PRECALL                  1
                      260 CALL                     1
                      270 RAISE_VARARGS            1
          consts
-            None
+            '\n    Create a (frozen) SciPy beta distribution.\n\n    You can specify the parameters in one of two ways.\n\n    1. Using ``alpha`` and ``beta``:\n\n    >>> from rvtools.construct import beta\n    >>> beta(1, 2)  # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n\n    2. Using quantiles:\n\n    >>> beta(p5=0.1, p95=0.9) # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n    >>> beta(quantiles={1/1000: 0.1, 999/1000: 0.9})  # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n\n    '
             ('alpha', 'beta', 'quantiles')
             'alpha'
             'beta'
             'quantiles'
             "You must specify either 'alpha' and 'beta', or 'quantiles'."
+            None
             ()
          names      ('parse_spec', 'keys', 'scipy', 'stats', 'beta', 'from_quantiles', 'ValueError')
          varnames   ('alpha', 'beta', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
          filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
          name       'beta'
          firstlineno 9
-         lnotab 0x020120013401400132012a02
+         lnotab 0x021420013401400132012a02
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
@@ -186,126 +187,126 @@
             0000000000000000007c027c067c07a6030000ab0300000000000000007d
             087417000000000000000000006a0c00000000000000007c087c01a60200
             00ab020000000000000000731674030000000000000000000064087c019b
             0064097c089b0064039d05a6010000ab0100000000000000008201740a00
             0000000000000000006a080000000000000000a009000000000000000000
             00000000000000000000007c067c07a6020000ab02000000000000000053
             00
-          19           0 RESUME                   0
+          38           0 RESUME                   0
          
-          20           2 LOAD_GLOBAL              1 (NULL + len)
+          39           2 LOAD_GLOBAL              1 (NULL + len)
                       14 LOAD_FAST                0 (quantiles)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_CONST               1 (2)
                       32 COMPARE_OP               3 (!=)
                       38 POP_JUMP_FORWARD_IF_FALSE    32 (to 104)
          
-          21          40 LOAD_GLOBAL              3 (NULL + ValueError)
+          40          40 LOAD_GLOBAL              3 (NULL + ValueError)
                       52 LOAD_CONST               2 ('Expected exactly two quantiles, got ')
                       54 LOAD_GLOBAL              1 (NULL + len)
                       66 LOAD_FAST                0 (quantiles)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 FORMAT_VALUE             0
                       84 LOAD_CONST               3 ('.')
                       86 BUILD_STRING             3
                       88 PRECALL                  1
                       92 CALL                     1
                      102 RAISE_VARARGS            1
          
-          23     >>  104 LOAD_GLOBAL              5 (NULL + list)
+          42     >>  104 LOAD_GLOBAL              5 (NULL + list)
                      116 LOAD_FAST                0 (quantiles)
                      118 LOAD_METHOD              3 (keys)
                      140 PRECALL                  0
                      144 CALL                     0
                      154 PRECALL                  1
                      158 CALL                     1
                      168 STORE_FAST               1 (ps)
          
-          24         170 LOAD_GLOBAL              5 (NULL + list)
+          43         170 LOAD_GLOBAL              5 (NULL + list)
                      182 LOAD_FAST                0 (quantiles)
                      184 LOAD_METHOD              4 (values)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 PRECALL                  1
                      224 CALL                     1
                      234 STORE_FAST               2 (qs)
          
-          26         236 LOAD_CONST               4 ((1, 1))
+          45         236 LOAD_CONST               4 ((1, 1))
                      238 UNPACK_SEQUENCE          2
                      242 STORE_FAST               3 (alpha_init)
                      244 STORE_FAST               4 (beta_init)
          
-          27         246 LOAD_GLOBAL             10 (scipy)
+          46         246 LOAD_GLOBAL             10 (scipy)
                      258 LOAD_ATTR                6 (optimize)
                      268 LOAD_METHOD              7 (curve_fit)
          
-          28         290 LOAD_CONST               5 (<code object <lambda>, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 28>)
+          47         290 LOAD_CONST               5 (<code object <lambda>, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 47>)
                      292 MAKE_FUNCTION            0
          
-          29         294 LOAD_FAST                2 (qs)
+          48         294 LOAD_FAST                2 (qs)
          
-          30         296 LOAD_FAST                1 (ps)
+          49         296 LOAD_FAST                1 (ps)
          
-          31         298 LOAD_FAST                3 (alpha_init)
+          50         298 LOAD_FAST                3 (alpha_init)
                      300 LOAD_FAST                4 (beta_init)
                      302 BUILD_LIST               2
          
-          27         304 KW_NAMES                 6
+          46         304 KW_NAMES                 6
                      306 PRECALL                  4
                      310 CALL                     4
                      320 STORE_FAST               5 (fit)
          
-          35         322 LOAD_FAST                5 (fit)
+          54         322 LOAD_FAST                5 (fit)
                      324 LOAD_CONST               7 (0)
                      326 BINARY_SUBSCR
                      336 UNPACK_SEQUENCE          2
                      340 STORE_FAST               6 (alpha)
                      342 STORE_FAST               7 (beta)
          
-          36         344 LOAD_GLOBAL             10 (scipy)
+          55         344 LOAD_GLOBAL             10 (scipy)
                      356 LOAD_ATTR                8 (stats)
                      366 LOAD_ATTR                9 (beta)
                      376 LOAD_METHOD             10 (cdf)
                      398 LOAD_FAST                2 (qs)
                      400 LOAD_FAST                6 (alpha)
                      402 LOAD_FAST                7 (beta)
                      404 PRECALL                  3
                      408 CALL                     3
                      418 STORE_FAST               8 (fitted_ps)
          
-          37         420 LOAD_GLOBAL             23 (NULL + np)
+          56         420 LOAD_GLOBAL             23 (NULL + np)
                      432 LOAD_ATTR               12 (allclose)
                      442 LOAD_FAST                8 (fitted_ps)
                      444 LOAD_FAST                1 (ps)
                      446 PRECALL                  2
                      450 CALL                     2
                      460 POP_JUMP_FORWARD_IF_TRUE    22 (to 506)
          
-          38         462 LOAD_GLOBAL              3 (NULL + ValueError)
+          57         462 LOAD_GLOBAL              3 (NULL + ValueError)
          
-          39         474 LOAD_CONST               8 ('Could not fit beta distribution to quantiles. Expected probabilities ')
+          58         474 LOAD_CONST               8 ('Could not fit beta distribution to quantiles. Expected probabilities ')
          
-          40         476 LOAD_FAST                1 (ps)
+          59         476 LOAD_FAST                1 (ps)
          
-          39         478 FORMAT_VALUE             0
+          58         478 FORMAT_VALUE             0
                      480 LOAD_CONST               9 (', got fitted values ')
          
-          40         482 LOAD_FAST                8 (fitted_ps)
+          59         482 LOAD_FAST                8 (fitted_ps)
          
-          39         484 FORMAT_VALUE             0
+          58         484 FORMAT_VALUE             0
                      486 LOAD_CONST               3 ('.')
                      488 BUILD_STRING             5
          
-          38         490 PRECALL                  1
+          57         490 PRECALL                  1
                      494 CALL                     1
                      504 RAISE_VARARGS            1
          
-          43     >>  506 LOAD_GLOBAL             10 (scipy)
+          62     >>  506 LOAD_GLOBAL             10 (scipy)
                      518 LOAD_ATTR                8 (stats)
                      528 LOAD_METHOD              9 (beta)
                      550 LOAD_FAST                6 (alpha)
                      552 LOAD_FAST                7 (beta)
                      554 PRECALL                  2
                      558 CALL                     2
                      568 RETURN_VALUE
@@ -320,15 +321,15 @@
                nlocals   : 3
                stacksize : 5
                flags     : 19
                code
                   0x97007400000000000000000000006a0100000000000000006a02000000
                   0000000000a00300000000000000000000000000000000000000007c007c
                   017c02a6030000ab0300000000000000005300
-                28           0 RESUME                   0
+                47           0 RESUME                   0
                              2 LOAD_GLOBAL              0 (scipy)
                             14 LOAD_ATTR                1 (stats)
                             24 LOAD_ATTR                2 (beta)
                             34 LOAD_METHOD              3 (cdf)
                             56 LOAD_FAST                0 (x)
                             58 LOAD_FAST                1 (alpha)
                             60 LOAD_FAST                2 (beta)
@@ -339,32 +340,32 @@
                   None
                names      ('scipy', 'stats', 'beta', 'cdf')
                varnames   ('x', 'alpha', 'beta')
                freevars   ()
                cellvars   ()
                filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
                name       '<lambda>'
-               firstlineno 28
+               firstlineno 47
                lnotab 0x
             ('xdata', 'ydata', 'p0')
             0
             'Could not fit beta distribution to quantiles. Expected probabilities '
             ', got fitted values '
          names      ('len', 'ValueError', 'list', 'keys', 'values', 'scipy', 'optimize', 'curve_fit', 'stats', 'beta', 'cdf', 'np', 'allclose')
          varnames   ('quantiles', 'ps', 'qs', 'alpha_init', 'beta_init', 'fit', 'alpha', 'beta', 'fitted_ps')
          freevars   ()
          cellvars   ()
          filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
          name       'from_quantiles'
-         firstlineno 19
+         firstlineno 38
          lnotab
             0x020126014002420142020a012c0104010201020106fc120816014c012a
             010c01020102ff040102ff06ff1005
       (None, None)
    names      ('numbers', 'Real', 'numpy', 'np', 'scipy', 'rvtools.construct._helpers', 'parse_spec', 'dict', 'beta', 'from_quantiles')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c02080108020c032c0a
+   lnotab 0x00ff02010c02080108020c032c1d
```

### Comparing `rvtools-0.1.4/rvtools/construct/__pycache__/lognorm.cpython-311.pyc` & `rvtools-0.1.5/rvtools/construct/__pycache__/norm.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,508 +1,368 @@
 magic:    0xa70d0d0a
-moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
-files sz: 2127
+moddate:  0x310d9f64 (Fri Jun 30 17:13:21 2023 UTC)
+files sz: 1880
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 14
+   stacksize : 10
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c025a03640064026c045a
-      04640064036c056d065a060100640064046c076d085a0901000900090064
-      1064026402640264059c0364066501640765016408650164096501640a65
-      0a65016501660219000000000000000000660a640b84075a0b640a650a65
-      0165016602190000000000000000006602640c84045a0c64066501640765
-      016604640d84045a0d640e84005a0e640f84005a0f64025300
+      0x9700640064016c006d015a010100640064026c025a02640064036c036d
+      045a040100640c640264049c016405650164066501640765056501650166
+      02190000000000000000006606640884075a066407650565016501660219
+      0000000000000000006602640984045a07640a6508650165016602190000
+      000000000000006602640b84045a0964025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Real',))
                  6 IMPORT_NAME              0 (numbers)
                  8 IMPORT_FROM              1 (Real)
                 10 STORE_NAME               1 (Real)
                 12 POP_TOP
    
      3          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (None)
-                18 IMPORT_NAME              2 (numpy)
-                20 STORE_NAME               3 (np)
+                18 IMPORT_NAME              2 (scipy)
+                20 STORE_NAME               2 (scipy)
    
-     4          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (None)
-                26 IMPORT_NAME              4 (scipy)
-                28 STORE_NAME               4 (scipy)
-   
-     6          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('parse_spec',))
-                34 IMPORT_NAME              5 (rvtools.construct._helpers)
-                36 IMPORT_FROM              6 (parse_spec)
-                38 STORE_NAME               6 (parse_spec)
-                40 POP_TOP
-   
-     7          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('params_from_quantiles',))
-                46 IMPORT_NAME              7 (rvtools.construct.norm)
-                48 IMPORT_FROM              8 (params_from_quantiles)
-                50 STORE_NAME               9 (norm_params_from_quantiles)
-                52 POP_TOP
-   
-    11          54 NOP
-   
-    12          56 NOP
-   
-    10          58 LOAD_CONST              16 ((None, None))
-   
-    14          60 LOAD_CONST               2 (None)
-   
-    15          62 LOAD_CONST               2 (None)
-   
-    16          64 LOAD_CONST               2 (None)
-   
-    10          66 LOAD_CONST               5 (('mean', 'sd', 'quantiles'))
-                68 BUILD_CONST_KEY_MAP      3
-                70 LOAD_CONST               6 ('mu')
-   
-    11          72 LOAD_NAME                1 (Real)
-   
-    10          74 LOAD_CONST               7 ('sigma')
-   
-    12          76 LOAD_NAME                1 (Real)
-   
-    10          78 LOAD_CONST               8 ('mean')
-   
-    14          80 LOAD_NAME                1 (Real)
-   
-    10          82 LOAD_CONST               9 ('sd')
-   
-    15          84 LOAD_NAME                1 (Real)
-   
-    10          86 LOAD_CONST              10 ('quantiles')
-   
-    16          88 LOAD_NAME               10 (dict)
-                90 LOAD_NAME                1 (Real)
-                92 LOAD_NAME                1 (Real)
-                94 BUILD_TUPLE              2
-                96 BINARY_SUBSCR
-   
-    10         106 BUILD_TUPLE             10
-               108 LOAD_CONST              11 (<code object lognorm, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 10>)
-               110 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
-               112 STORE_NAME              11 (lognorm)
-   
-    32         114 LOAD_CONST              10 ('quantiles')
-               116 LOAD_NAME               10 (dict)
-               118 LOAD_NAME                1 (Real)
-               120 LOAD_NAME                1 (Real)
-               122 BUILD_TUPLE              2
-               124 BINARY_SUBSCR
-               134 BUILD_TUPLE              2
-               136 LOAD_CONST              12 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 32>)
-               138 MAKE_FUNCTION            4 (annotations)
-               140 STORE_NAME              12 (from_quantiles)
-   
-    46         142 LOAD_CONST               6 ('mu')
-               144 LOAD_NAME                1 (Real)
-               146 LOAD_CONST               7 ('sigma')
-               148 LOAD_NAME                1 (Real)
-               150 BUILD_TUPLE              4
-               152 LOAD_CONST              13 (<code object from_params, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 46>)
-               154 MAKE_FUNCTION            4 (annotations)
-               156 STORE_NAME              13 (from_params)
-   
-    57         158 LOAD_CONST              14 (<code object from_mean_sd, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 57>)
-               160 MAKE_FUNCTION            0
-               162 STORE_NAME              14 (from_mean_sd)
-   
-    62         164 LOAD_CONST              15 (<code object to_mu_sigma, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 62>)
-               166 MAKE_FUNCTION            0
-               168 STORE_NAME              15 (to_mu_sigma)
-               170 LOAD_CONST               2 (None)
-               172 RETURN_VALUE
+     5          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('parse_spec',))
+                26 IMPORT_NAME              3 (rvtools.construct._helpers)
+                28 IMPORT_FROM              4 (parse_spec)
+                30 STORE_NAME               4 (parse_spec)
+                32 POP_TOP
+   
+     8          34 LOAD_CONST              12 ((None, None))
+                36 LOAD_CONST               2 (None)
+                38 LOAD_CONST               4 (('quantiles',))
+                40 BUILD_CONST_KEY_MAP      1
+                42 LOAD_CONST               5 ('mean')
+                44 LOAD_NAME                1 (Real)
+                46 LOAD_CONST               6 ('sd')
+                48 LOAD_NAME                1 (Real)
+                50 LOAD_CONST               7 ('quantiles')
+                52 LOAD_NAME                5 (dict)
+                54 LOAD_NAME                1 (Real)
+                56 LOAD_NAME                1 (Real)
+                58 BUILD_TUPLE              2
+                60 BINARY_SUBSCR
+                70 BUILD_TUPLE              6
+                72 LOAD_CONST               8 (<code object norm, file "/Users/t/repos/rvtools/rvtools/construct/norm.py", line 8>)
+                74 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
+                76 STORE_NAME               6 (norm)
+   
+    36          78 LOAD_CONST               7 ('quantiles')
+                80 LOAD_NAME                5 (dict)
+                82 LOAD_NAME                1 (Real)
+                84 LOAD_NAME                1 (Real)
+                86 BUILD_TUPLE              2
+                88 BINARY_SUBSCR
+                98 BUILD_TUPLE              2
+               100 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/norm.py", line 36>)
+               102 MAKE_FUNCTION            4 (annotations)
+               104 STORE_NAME               7 (from_quantiles)
+   
+    48         106 LOAD_CONST              10 ('return')
+               108 LOAD_NAME                8 (tuple)
+               110 LOAD_NAME                1 (Real)
+               112 LOAD_NAME                1 (Real)
+               114 BUILD_TUPLE              2
+               116 BINARY_SUBSCR
+               126 BUILD_TUPLE              2
+               128 LOAD_CONST              11 (<code object params_from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/norm.py", line 48>)
+               130 MAKE_FUNCTION            4 (annotations)
+               132 STORE_NAME               9 (params_from_quantiles)
+               134 LOAD_CONST               2 (None)
+               136 RETURN_VALUE
    consts
       0
       ('Real',)
       None
       ('parse_spec',)
-      ('params_from_quantiles',)
-      ('mean', 'sd', 'quantiles')
-      'mu'
-      'sigma'
+      ('quantiles',)
       'mean'
       'sd'
       'quantiles'
       code
          argcount  : 2
-         nlocals   : 7
-         stacksize : 9
+         nlocals   : 5
+         stacksize : 7
          flags     : 11
          code
-            0x970074010000000000000000000064087c007c017c027c037c0464019c
-            057c05a4018e017d067c06a0010000000000000000000000000000000000
-            000000a6000000ab0000000000000000006402640368026b020000000072
-            107405000000000000000000007c007c01a6020000ab0200000000000000
-            0053007c06a0010000000000000000000000000000000000000000a60000
-            00ab0000000000000000006404640568026b020000000072107407000000
-            000000000000007c027c03a6020000ab02000000000000000053007c06a0
-            010000000000000000000000000000000000000000a6000000ab00000000
-            0000000000640668016b020000000072157409000000000000000000007c
-            06640619000000000000000000a6010000ab010000000000000000530074
-            0b000000000000000000006407a6010000ab0100000000000000008201
-          10           0 RESUME                   0
-         
-          19           2 LOAD_GLOBAL              1 (NULL + parse_spec)
-                      14 LOAD_CONST               8 (())
-                      16 LOAD_FAST                0 (mu)
-                      18 LOAD_FAST                1 (sigma)
-                      20 LOAD_FAST                2 (mean)
-                      22 LOAD_FAST                3 (sd)
-                      24 LOAD_FAST                4 (quantiles)
-                      26 LOAD_CONST               1 (('mu', 'sigma', 'mean', 'sd', 'quantiles'))
-                      28 BUILD_CONST_KEY_MAP      5
-                      30 LOAD_FAST                5 (kwargs)
-                      32 DICT_MERGE               1
-                      34 CALL_FUNCTION_EX         1
-                      36 STORE_FAST               6 (spec)
-         
-          20          38 LOAD_FAST                6 (spec)
-                      40 LOAD_METHOD              1 (keys)
-                      62 PRECALL                  0
-                      66 CALL                     0
-                      76 LOAD_CONST               2 ('mu')
-                      78 LOAD_CONST               3 ('sigma')
-                      80 BUILD_SET                2
-                      82 COMPARE_OP               2 (==)
-                      88 POP_JUMP_FORWARD_IF_FALSE    16 (to 122)
-         
-          21          90 LOAD_GLOBAL              5 (NULL + from_params)
-                     102 LOAD_FAST                0 (mu)
-                     104 LOAD_FAST                1 (sigma)
-                     106 PRECALL                  2
-                     110 CALL                     2
-                     120 RETURN_VALUE
-         
-          22     >>  122 LOAD_FAST                6 (spec)
-                     124 LOAD_METHOD              1 (keys)
-                     146 PRECALL                  0
-                     150 CALL                     0
-                     160 LOAD_CONST               4 ('mean')
-                     162 LOAD_CONST               5 ('sd')
-                     164 BUILD_SET                2
-                     166 COMPARE_OP               2 (==)
-                     172 POP_JUMP_FORWARD_IF_FALSE    16 (to 206)
-         
-          23         174 LOAD_GLOBAL              7 (NULL + from_mean_sd)
-                     186 LOAD_FAST                2 (mean)
-                     188 LOAD_FAST                3 (sd)
-                     190 PRECALL                  2
-                     194 CALL                     2
-                     204 RETURN_VALUE
-         
-          24     >>  206 LOAD_FAST                6 (spec)
-                     208 LOAD_METHOD              1 (keys)
-                     230 PRECALL                  0
-                     234 CALL                     0
-                     244 LOAD_CONST               6 ('quantiles')
-                     246 BUILD_SET                1
-                     248 COMPARE_OP               2 (==)
-                     254 POP_JUMP_FORWARD_IF_FALSE    21 (to 298)
-         
-          25         256 LOAD_GLOBAL              9 (NULL + from_quantiles)
-                     268 LOAD_FAST                6 (spec)
-                     270 LOAD_CONST               6 ('quantiles')
-                     272 BINARY_SUBSCR
-                     282 PRECALL                  1
-                     286 CALL                     1
-                     296 RETURN_VALUE
-         
-          27     >>  298 LOAD_GLOBAL             11 (NULL + ValueError)
-         
-          28         310 LOAD_CONST               7 ("You must specify either 'mu' and 'sigma', 'mean' and 'sd', or 'quantiles'.")
-         
-          27         312 PRECALL                  1
-                     316 CALL                     1
-                     326 RAISE_VARARGS            1
+            0x970074010000000000000000000064077c007c017c0264019c037c03a4
+            018e017d047c04a0010000000000000000000000000000000000000000a6
+            000000ab0000000000000000006402640368026b02000000007220740400
+            0000000000000000006a030000000000000000a004000000000000000000
+            00000000000000000000007c007c01a6020000ab02000000000000000053
+            007c04a0010000000000000000000000000000000000000000a6000000ab
+            000000000000000000640468016b02000000007215740b00000000000000
+            0000007c04640419000000000000000000a6010000ab0100000000000000
+            005300740d000000000000000000006405a6010000ab0100000000000000
+            008201
+           8           0 RESUME                   0
+         
+          27           2 LOAD_GLOBAL              1 (NULL + parse_spec)
+                      14 LOAD_CONST               7 (())
+                      16 LOAD_FAST                0 (mean)
+                      18 LOAD_FAST                1 (sd)
+                      20 LOAD_FAST                2 (quantiles)
+                      22 LOAD_CONST               1 (('mean', 'sd', 'quantiles'))
+                      24 BUILD_CONST_KEY_MAP      3
+                      26 LOAD_FAST                3 (kwargs)
+                      28 DICT_MERGE               1
+                      30 CALL_FUNCTION_EX         1
+                      32 STORE_FAST               4 (spec)
+         
+          28          34 LOAD_FAST                4 (spec)
+                      36 LOAD_METHOD              1 (keys)
+                      58 PRECALL                  0
+                      62 CALL                     0
+                      72 LOAD_CONST               2 ('mean')
+                      74 LOAD_CONST               3 ('sd')
+                      76 BUILD_SET                2
+                      78 COMPARE_OP               2 (==)
+                      84 POP_JUMP_FORWARD_IF_FALSE    32 (to 150)
+         
+          29          86 LOAD_GLOBAL              4 (scipy)
+                      98 LOAD_ATTR                3 (stats)
+                     108 LOAD_METHOD              4 (norm)
+                     130 LOAD_FAST                0 (mean)
+                     132 LOAD_FAST                1 (sd)
+                     134 PRECALL                  2
+                     138 CALL                     2
+                     148 RETURN_VALUE
+         
+          30     >>  150 LOAD_FAST                4 (spec)
+                     152 LOAD_METHOD              1 (keys)
+                     174 PRECALL                  0
+                     178 CALL                     0
+                     188 LOAD_CONST               4 ('quantiles')
+                     190 BUILD_SET                1
+                     192 COMPARE_OP               2 (==)
+                     198 POP_JUMP_FORWARD_IF_FALSE    21 (to 242)
+         
+          31         200 LOAD_GLOBAL             11 (NULL + from_quantiles)
+                     212 LOAD_FAST                4 (spec)
+                     214 LOAD_CONST               4 ('quantiles')
+                     216 BINARY_SUBSCR
+                     226 PRECALL                  1
+                     230 CALL                     1
+                     240 RETURN_VALUE
+         
+          33     >>  242 LOAD_GLOBAL             13 (NULL + ValueError)
+                     254 LOAD_CONST               5 ("You must specify either 'mean' and 'sd', or 'quantiles'.")
+                     256 PRECALL                  1
+                     260 CALL                     1
+                     270 RAISE_VARARGS            1
          consts
-            None
-            ('mu', 'sigma', 'mean', 'sd', 'quantiles')
-            'mu'
-            'sigma'
+            '\n    Create a (frozen) SciPy normal distribution.\n\n    You can specify the parameters in one of two ways.\n\n    1. Using ``mean`` and ``sd``:\n\n    >>> from rvtools.construct import norm\n    >>> norm(1, 2)  # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n\n    2. Using quantiles:\n\n    >>> norm(p5=0.1, p95=0.9) # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n    >>> norm(quantiles={1/1000: 0.1, 999/1000: 0.9})  # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n    '
+            ('mean', 'sd', 'quantiles')
             'mean'
             'sd'
             'quantiles'
-            "You must specify either 'mu' and 'sigma', 'mean' and 'sd', or 'quantiles'."
+            "You must specify either 'mean' and 'sd', or 'quantiles'."
+            None
             ()
-         names      ('parse_spec', 'keys', 'from_params', 'from_mean_sd', 'from_quantiles', 'ValueError')
-         varnames   ('mu', 'sigma', 'mean', 'sd', 'quantiles', 'kwargs', 'spec')
+         names      ('parse_spec', 'keys', 'scipy', 'stats', 'norm', 'from_quantiles', 'ValueError')
+         varnames   ('mean', 'sd', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
-         name       'lognorm'
-         firstlineno 10
-         lnotab 0x02092401340120013401200132012a020c0102ff
+         filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
+         name       'norm'
+         firstlineno 8
+         lnotab 0x021320013401400132012a02
       code
          argcount  : 1
-         nlocals   : 6
+         nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             0064016b0300000000722074030000000000000000000064027401000000
             000000000000007c00a6010000ab0100000000000000009b0064039d03a6
             010000ab01000000000000000082017405000000000000000000007c00a0
             030000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6010000ab0100000000000000007d01740500000000000000
             0000007c00a0040000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab0100000000000000007d02740b00
-            0000000000000000006a0600000000000000007c02a6010000ab01000000
-            00000000007d03740f000000000000000000007c01640419000000000000
-            0000007c036404190000000000000000007c016405190000000000000000
-            007c03640519000000000000000000a6040000ab0400000000000000005c
-            0200007d047d057411000000000000000000007c047c05a6020000ab0200
-            000000000000005300
-          32           0 RESUME                   0
+            0000000000000000007c016404190000000000000000007c026404190000
+            000000000000007c016405190000000000000000007c0264051900000000
+            0000000000a6040000ab0400000000000000005c0200007d037d04740c00
+            0000000000000000006a070000000000000000a008000000000000000000
+            00000000000000000000007c037c04a6020000ab02000000000000000053
+            00
+          36           0 RESUME                   0
          
-          33           2 LOAD_GLOBAL              1 (NULL + len)
+          37           2 LOAD_GLOBAL              1 (NULL + len)
                       14 LOAD_FAST                0 (quantiles)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_CONST               1 (2)
                       32 COMPARE_OP               3 (!=)
                       38 POP_JUMP_FORWARD_IF_FALSE    32 (to 104)
          
-          34          40 LOAD_GLOBAL              3 (NULL + ValueError)
+          38          40 LOAD_GLOBAL              3 (NULL + ValueError)
                       52 LOAD_CONST               2 ('Expected exactly two quantiles, got ')
                       54 LOAD_GLOBAL              1 (NULL + len)
                       66 LOAD_FAST                0 (quantiles)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 FORMAT_VALUE             0
                       84 LOAD_CONST               3 ('.')
                       86 BUILD_STRING             3
                       88 PRECALL                  1
                       92 CALL                     1
                      102 RAISE_VARARGS            1
          
-          36     >>  104 LOAD_GLOBAL              5 (NULL + list)
+          40     >>  104 LOAD_GLOBAL              5 (NULL + list)
                      116 LOAD_FAST                0 (quantiles)
                      118 LOAD_METHOD              3 (keys)
                      140 PRECALL                  0
                      144 CALL                     0
                      154 PRECALL                  1
                      158 CALL                     1
                      168 STORE_FAST               1 (ps)
          
-          37         170 LOAD_GLOBAL              5 (NULL + list)
+          41         170 LOAD_GLOBAL              5 (NULL + list)
                      182 LOAD_FAST                0 (quantiles)
                      184 LOAD_METHOD              4 (values)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 PRECALL                  1
                      224 CALL                     1
                      234 STORE_FAST               2 (qs)
          
-          40         236 LOAD_GLOBAL             11 (NULL + np)
-                     248 LOAD_ATTR                6 (log)
-                     258 LOAD_FAST                2 (qs)
-                     260 PRECALL                  1
-                     264 CALL                     1
-                     274 STORE_FAST               3 (log_qs)
-         
-          41         276 LOAD_GLOBAL             15 (NULL + norm_params_from_quantiles)
-                     288 LOAD_FAST                1 (ps)
-                     290 LOAD_CONST               4 (0)
-                     292 BINARY_SUBSCR
-                     302 LOAD_FAST                3 (log_qs)
-                     304 LOAD_CONST               4 (0)
-                     306 BINARY_SUBSCR
-                     316 LOAD_FAST                1 (ps)
-                     318 LOAD_CONST               5 (1)
-                     320 BINARY_SUBSCR
-                     330 LOAD_FAST                3 (log_qs)
-                     332 LOAD_CONST               5 (1)
-                     334 BINARY_SUBSCR
-                     344 PRECALL                  4
-                     348 CALL                     4
-                     358 UNPACK_SEQUENCE          2
-                     362 STORE_FAST               4 (mu)
-                     364 STORE_FAST               5 (sigma)
-         
-          43         366 LOAD_GLOBAL             17 (NULL + from_params)
-                     378 LOAD_FAST                4 (mu)
-                     380 LOAD_FAST                5 (sigma)
-                     382 PRECALL                  2
-                     386 CALL                     2
-                     396 RETURN_VALUE
+          43         236 LOAD_GLOBAL             11 (NULL + params_from_quantiles)
+                     248 LOAD_FAST                1 (ps)
+                     250 LOAD_CONST               4 (0)
+                     252 BINARY_SUBSCR
+                     262 LOAD_FAST                2 (qs)
+                     264 LOAD_CONST               4 (0)
+                     266 BINARY_SUBSCR
+                     276 LOAD_FAST                1 (ps)
+                     278 LOAD_CONST               5 (1)
+                     280 BINARY_SUBSCR
+                     290 LOAD_FAST                2 (qs)
+                     292 LOAD_CONST               5 (1)
+                     294 BINARY_SUBSCR
+                     304 PRECALL                  4
+                     308 CALL                     4
+                     318 UNPACK_SEQUENCE          2
+                     322 STORE_FAST               3 (mu)
+                     324 STORE_FAST               4 (sigma)
+         
+          45         326 LOAD_GLOBAL             12 (scipy)
+                     338 LOAD_ATTR                7 (stats)
+                     348 LOAD_METHOD              8 (norm)
+                     370 LOAD_FAST                3 (mu)
+                     372 LOAD_FAST                4 (sigma)
+                     374 PRECALL                  2
+                     378 CALL                     2
+                     388 RETURN_VALUE
          consts
             None
             2
             'Expected exactly two quantiles, got '
             '.'
             0
             1
-         names      ('len', 'ValueError', 'list', 'keys', 'values', 'np', 'log', 'norm_params_from_quantiles', 'from_params')
-         varnames   ('quantiles', 'ps', 'qs', 'log_qs', 'mu', 'sigma')
+         names      ('len', 'ValueError', 'list', 'keys', 'values', 'params_from_quantiles', 'scipy', 'stats', 'norm')
+         varnames   ('quantiles', 'ps', 'qs', 'mu', 'sigma')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
          name       'from_quantiles'
-         firstlineno 32
-         lnotab 0x0201260140024201420328015a02
+         firstlineno 36
+         lnotab 0x020126014002420142025a02
+      'return'
       code
-         argcount  : 2
-         nlocals   : 2
+         argcount  : 4
+         nlocals   : 7
          stacksize : 5
          flags     : 3
          code
-            0x97007400000000000000000000006a010000000000000000a002000000
-            00000000000000000000000000000000007407000000000000000000006a
-            0400000000000000007c00a6010000ab0100000000000000007c01ac01a6
-            020000ab0200000000000000005300
-          46           0 RESUME                   0
+            0x97007400000000000000000000006a0100000000000000006a02000000
+            0000000000a00300000000000000000000000000000000000000007c02a6
+            010000ab0100000000000000007400000000000000000000006a01000000
+            00000000006a020000000000000000a00300000000000000000000000000
+            000000000000007c00a6010000ab0100000000000000007a0a00007d047c
+            037c017a0a00007c047a0b00007d057c017400000000000000000000006a
+            0100000000000000006a020000000000000000a003000000000000000000
+            00000000000000000000007c02a6010000ab0100000000000000007a0500
+            007c037400000000000000000000006a0100000000000000006a02000000
+            0000000000a00300000000000000000000000000000000000000007c00a6
+            010000ab0100000000000000007a0500007a0a00007c047a0b00007d067c
+            067c0566025300
+          48           0 RESUME                   0
          
-          54           2 LOAD_GLOBAL              0 (scipy)
+          50           2 LOAD_GLOBAL              0 (scipy)
                       14 LOAD_ATTR                1 (stats)
-                      24 LOAD_METHOD              2 (lognorm)
-                      46 LOAD_GLOBAL              7 (NULL + np)
-                      58 LOAD_ATTR                4 (exp)
-                      68 LOAD_FAST                0 (mu)
-                      70 PRECALL                  1
-                      74 CALL                     1
-                      84 LOAD_FAST                1 (sigma)
-                      86 KW_NAMES                 1
-                      88 PRECALL                  2
-                      92 CALL                     2
-                     102 RETURN_VALUE
-         consts
-            "\n    SciPy's ``lognorm`` does not take the ``mu`` and ``sigma`` parameters (it takes its own\n    ``scale`` and ``s`` parameters).\n\n    This is a convenience wrapper that allows you to create a (frozen) SciPy log-normal distribution using ``mu`` and\n    ``sigma``.\n    "
-            ('scale', 's')
-         names      ('scipy', 'stats', 'lognorm', 'np', 'exp')
-         varnames   ('mu', 'sigma')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
-         name       'from_params'
-         firstlineno 46
-         lnotab 0x0208
-      code
-         argcount  : 2
-         nlocals   : 4
-         stacksize : 4
-         flags     : 3
-         code
-            0x97007401000000000000000000007c007c01a6020000ab020000000000
-            0000005c0200007d027d037403000000000000000000007c027c03a60200
-            00ab0200000000000000005300
-          57           0 RESUME                   0
-         
-          58           2 LOAD_GLOBAL              1 (NULL + to_mu_sigma)
-                      14 LOAD_FAST                0 (mean)
-                      16 LOAD_FAST                1 (sd)
-                      18 PRECALL                  2
-                      22 CALL                     2
-                      32 UNPACK_SEQUENCE          2
-                      36 STORE_FAST               2 (mu)
-                      38 STORE_FAST               3 (sigma)
-         
-          59          40 LOAD_GLOBAL              3 (NULL + from_params)
-                      52 LOAD_FAST                2 (mu)
-                      54 LOAD_FAST                3 (sigma)
-                      56 PRECALL                  2
-                      60 CALL                     2
-                      70 RETURN_VALUE
+                      24 LOAD_ATTR                2 (norm)
+                      34 LOAD_METHOD              3 (ppf)
+                      56 LOAD_FAST                2 (p2)
+                      58 PRECALL                  1
+                      62 CALL                     1
+                      72 LOAD_GLOBAL              0 (scipy)
+                      84 LOAD_ATTR                1 (stats)
+                      94 LOAD_ATTR                2 (norm)
+                     104 LOAD_METHOD              3 (ppf)
+                     126 LOAD_FAST                0 (p1)
+                     128 PRECALL                  1
+                     132 CALL                     1
+                     142 BINARY_OP               10 (-)
+                     146 STORE_FAST               4 (denom)
+         
+          51         148 LOAD_FAST                3 (x2)
+                     150 LOAD_FAST                1 (x1)
+                     152 BINARY_OP               10 (-)
+                     156 LOAD_FAST                4 (denom)
+                     158 BINARY_OP               11 (/)
+                     162 STORE_FAST               5 (sigma)
+         
+          52         164 LOAD_FAST                1 (x1)
+                     166 LOAD_GLOBAL              0 (scipy)
+                     178 LOAD_ATTR                1 (stats)
+                     188 LOAD_ATTR                2 (norm)
+                     198 LOAD_METHOD              3 (ppf)
+                     220 LOAD_FAST                2 (p2)
+                     222 PRECALL                  1
+                     226 CALL                     1
+                     236 BINARY_OP                5 (*)
+                     240 LOAD_FAST                3 (x2)
+                     242 LOAD_GLOBAL              0 (scipy)
+                     254 LOAD_ATTR                1 (stats)
+                     264 LOAD_ATTR                2 (norm)
+                     274 LOAD_METHOD              3 (ppf)
+                     296 LOAD_FAST                0 (p1)
+                     298 PRECALL                  1
+                     302 CALL                     1
+                     312 BINARY_OP                5 (*)
+                     316 BINARY_OP               10 (-)
+                     320 LOAD_FAST                4 (denom)
+                     322 BINARY_OP               11 (/)
+                     326 STORE_FAST               6 (mu)
+         
+          53         328 LOAD_FAST                6 (mu)
+                     330 LOAD_FAST                5 (sigma)
+                     332 BUILD_TUPLE              2
+                     334 RETURN_VALUE
          consts
-            None
-         names      ('to_mu_sigma', 'from_params')
-         varnames   ('mean', 'sd', 'mu', 'sigma')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
-         name       'from_mean_sd'
-         firstlineno 57
-         lnotab 0x02012601
-      code
-         argcount  : 2
-         nlocals   : 5
-         stacksize : 7
-         flags     : 3
-         code
-            0x97007c0164017a0800007d027401000000000000000000006a01000000
-            00000000007401000000000000000000006a0200000000000000007c027c
-            0064017a0800007a0b000064027a000000a6010000ab0100000000000000
-            00a6010000ab0100000000000000007d037401000000000000000000006a
-            0200000000000000007c00a6010000ab0100000000000000006403740100
-            0000000000000000006a0200000000000000007c027c0064017a0800007a
-            0b000064027a000000a6010000ab0100000000000000007a0500007a0a00
-            007d047c047c0366025300
-          62           0 RESUME                   0
-         
-          66           2 LOAD_FAST                1 (sd)
-                       4 LOAD_CONST               1 (2)
-                       6 BINARY_OP                8 (**)
-                      10 STORE_FAST               2 (var)
-         
-          67          12 LOAD_GLOBAL              1 (NULL + np)
-                      24 LOAD_ATTR                1 (sqrt)
-                      34 LOAD_GLOBAL              1 (NULL + np)
-                      46 LOAD_ATTR                2 (log)
-                      56 LOAD_FAST                2 (var)
-                      58 LOAD_FAST                0 (mean)
-                      60 LOAD_CONST               1 (2)
-                      62 BINARY_OP                8 (**)
-                      66 BINARY_OP               11 (/)
-                      70 LOAD_CONST               2 (1)
-                      72 BINARY_OP                0 (+)
-                      76 PRECALL                  1
-                      80 CALL                     1
-                      90 PRECALL                  1
-                      94 CALL                     1
-                     104 STORE_FAST               3 (sigma)
-         
-          69         106 LOAD_GLOBAL              1 (NULL + np)
-                     118 LOAD_ATTR                2 (log)
-                     128 LOAD_FAST                0 (mean)
-                     130 PRECALL                  1
-                     134 CALL                     1
-                     144 LOAD_CONST               3 (0.5)
-                     146 LOAD_GLOBAL              1 (NULL + np)
-                     158 LOAD_ATTR                2 (log)
-                     168 LOAD_FAST                2 (var)
-                     170 LOAD_FAST                0 (mean)
-                     172 LOAD_CONST               1 (2)
-                     174 BINARY_OP                8 (**)
-                     178 BINARY_OP               11 (/)
-                     182 LOAD_CONST               2 (1)
-                     184 BINARY_OP                0 (+)
-                     188 PRECALL                  1
-                     192 CALL                     1
-                     202 BINARY_OP                5 (*)
-                     206 BINARY_OP               10 (-)
-                     210 STORE_FAST               4 (mu)
-         
-          71         212 LOAD_FAST                4 (mu)
-                     214 LOAD_FAST                3 (sigma)
-                     216 BUILD_TUPLE              2
-                     218 RETURN_VALUE
-         consts
-            '\n    Get the ``mu`` and ``sigma`` parameters for a log-normal distribution with the given ``mean`` and ``sd``.\n    '
-            2
-            1
-            0.5
-         names      ('np', 'sqrt', 'log')
-         varnames   ('mean', 'sd', 'var', 'sigma', 'mu')
+            'Find parameters for a normal random variable X so that P(X < x1) = p1 and P(X < x2) = p2.'
+         names      ('scipy', 'stats', 'norm', 'ppf')
+         varnames   ('p1', 'x1', 'p2', 'x2', 'denom', 'sigma', 'mu')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
-         name       'to_mu_sigma'
-         firstlineno 62
-         lnotab 0x02040a015e026a02
+         filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
+         name       'params_from_quantiles'
+         firstlineno 48
+         lnotab 0x020292011001a401
       (None, None)
-   names      ('numbers', 'Real', 'numpy', 'np', 'scipy', 'rvtools.construct._helpers', 'parse_spec', 'rvtools.construct.norm', 'params_from_quantiles', 'norm_params_from_quantiles', 'dict', 'lognorm', 'from_quantiles', 'from_params', 'from_mean_sd', 'to_mu_sigma')
+   names      ('numbers', 'Real', 'scipy', 'rvtools.construct._helpers', 'parse_spec', 'dict', 'norm', 'from_quantiles', 'tuple', 'params_from_quantiles')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
+   filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
    name       '<module>'
    firstlineno 1
-   lnotab
-      0x00ff02010c02080108020c010c04020102fe02040201020102fa060102
-      ff020202fe020402fc020502fb020612fa08161c0e100b0605
+   lnotab 0x00ff02010c0208020c032c1c1c0c
```

### Comparing `rvtools-0.1.4/rvtools/construct/__pycache__/uniform.cpython-311.pyc` & `rvtools-0.1.5/rvtools/construct/__pycache__/uniform.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
-files sz: 1437
+moddate:  0xce0d9f64 (Fri Jun 30 17:15:58 2023 UTC)
+files sz: 2224
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -55,26 +55,26 @@
                 70 BUILD_TUPLE              2
                 72 BINARY_SUBSCR
                 82 BUILD_TUPLE              6
                 84 LOAD_CONST               9 (<code object uniform, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 9>)
                 86 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                 88 STORE_NAME               8 (uniform)
    
-    19          90 LOAD_CONST               8 ('quantiles')
+    40          90 LOAD_CONST               8 ('quantiles')
                 92 LOAD_NAME                7 (dict)
                 94 LOAD_NAME                1 (Real)
                 96 LOAD_NAME                1 (Real)
                 98 BUILD_TUPLE              2
                100 BINARY_SUBSCR
                110 BUILD_TUPLE              2
-               112 LOAD_CONST              10 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 19>)
+               112 LOAD_CONST              10 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 40>)
                114 MAKE_FUNCTION            4 (annotations)
                116 STORE_NAME               9 (from_quantiles)
    
-    34         118 LOAD_CONST              11 (<code object from_extrema, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 34>)
+    55         118 LOAD_CONST              11 (<code object from_extrema, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 55>)
                120 MAKE_FUNCTION            0
                122 STORE_NAME              10 (from_extrema)
                124 LOAD_CONST               2 (None)
                126 RETURN_VALUE
    consts
       0
       ('Real',)
@@ -87,92 +87,93 @@
       'quantiles'
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 7
          flags     : 11
          code
-            0x970074010000000000000000000064067c007c017c0264019c037c03a4
+            0x970074010000000000000000000064077c007c017c0264019c037c03a4
             018e017d047c04a0010000000000000000000000000000000000000000a6
             000000ab0000000000000000006402640368026b02000000007210740500
             0000000000000000007c007c01a6020000ab02000000000000000053007c
             04a0010000000000000000000000000000000000000000a6000000ab0000
             00000000000000640468016b020000000072157407000000000000000000
             007c04640419000000000000000000a6010000ab01000000000000000053
             007409000000000000000000006405a6010000ab01000000000000000082
             01
            9           0 RESUME                   0
          
-          10           2 LOAD_GLOBAL              1 (NULL + parse_spec)
-                      14 LOAD_CONST               6 (())
+          31           2 LOAD_GLOBAL              1 (NULL + parse_spec)
+                      14 LOAD_CONST               7 (())
                       16 LOAD_FAST                0 (a)
                       18 LOAD_FAST                1 (b)
                       20 LOAD_FAST                2 (quantiles)
                       22 LOAD_CONST               1 (('a', 'b', 'quantiles'))
                       24 BUILD_CONST_KEY_MAP      3
                       26 LOAD_FAST                3 (kwargs)
                       28 DICT_MERGE               1
                       30 CALL_FUNCTION_EX         1
                       32 STORE_FAST               4 (spec)
          
-          11          34 LOAD_FAST                4 (spec)
+          32          34 LOAD_FAST                4 (spec)
                       36 LOAD_METHOD              1 (keys)
                       58 PRECALL                  0
                       62 CALL                     0
                       72 LOAD_CONST               2 ('a')
                       74 LOAD_CONST               3 ('b')
                       76 BUILD_SET                2
                       78 COMPARE_OP               2 (==)
                       84 POP_JUMP_FORWARD_IF_FALSE    16 (to 118)
          
-          12          86 LOAD_GLOBAL              5 (NULL + from_extrema)
+          33          86 LOAD_GLOBAL              5 (NULL + from_extrema)
                       98 LOAD_FAST                0 (a)
                      100 LOAD_FAST                1 (b)
                      102 PRECALL                  2
                      106 CALL                     2
                      116 RETURN_VALUE
          
-          13     >>  118 LOAD_FAST                4 (spec)
+          34     >>  118 LOAD_FAST                4 (spec)
                      120 LOAD_METHOD              1 (keys)
                      142 PRECALL                  0
                      146 CALL                     0
                      156 LOAD_CONST               4 ('quantiles')
                      158 BUILD_SET                1
                      160 COMPARE_OP               2 (==)
                      166 POP_JUMP_FORWARD_IF_FALSE    21 (to 210)
          
-          14         168 LOAD_GLOBAL              7 (NULL + from_quantiles)
+          35         168 LOAD_GLOBAL              7 (NULL + from_quantiles)
                      180 LOAD_FAST                4 (spec)
                      182 LOAD_CONST               4 ('quantiles')
                      184 BINARY_SUBSCR
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RETURN_VALUE
          
-          16     >>  210 LOAD_GLOBAL              9 (NULL + ValueError)
+          37     >>  210 LOAD_GLOBAL              9 (NULL + ValueError)
                      222 LOAD_CONST               5 ("You must specify either the extrema 'a' and 'b', or 'quantiles'.")
                      224 PRECALL                  1
                      228 CALL                     1
                      238 RAISE_VARARGS            1
          consts
-            None
+            '\n    Create a (frozen) SciPy uniform distribution.\n\n    You can specify the parameters in one of two ways.\n\n    1. Using the bounds ``a`` and ``b`` of the distribution:\n\n    >>> from rvtools.construct import uniform\n    >>> uniform(1, 2)  # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n\n    If two positional arguments are given, they are interpreted as ``a`` and ``b``. **This is\n    different from SciPy.**\n\n    2. Using quantiles:\n\n    >>> uniform(p5=0.1, p95=0.9) # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n    >>> uniform(quantiles={1/1000: 0.1, 999/1000: 0.9})  # doctest: +ELLIPSIS\n    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>\n    '
             ('a', 'b', 'quantiles')
             'a'
             'b'
             'quantiles'
             "You must specify either the extrema 'a' and 'b', or 'quantiles'."
+            None
             ()
          names      ('parse_spec', 'keys', 'from_extrema', 'from_quantiles', 'ValueError')
          varnames   ('a', 'b', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
          filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
          name       'uniform'
          firstlineno 9
-         lnotab 0x020120013401200132012a02
+         lnotab 0x021620013401200132012a02
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
@@ -183,81 +184,81 @@
             0000000000a6010000ab0100000000000000007d01740500000000000000
             0000007c00a0040000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab0100000000000000007d02740b00
             0000000000000000007c017c02640464056406ac07a6050000ab05000000
             00000000007d0302007c036408a6010000ab0100000000000000007d0402
             007c036409a6010000ab0100000000000000007d05740d00000000000000
             0000007c047c05a6020000ab0200000000000000005300
-          19           0 RESUME                   0
+          40           0 RESUME                   0
          
-          20           2 LOAD_GLOBAL              1 (NULL + len)
+          41           2 LOAD_GLOBAL              1 (NULL + len)
                       14 LOAD_FAST                0 (quantiles)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_CONST               1 (2)
                       32 COMPARE_OP               3 (!=)
                       38 POP_JUMP_FORWARD_IF_FALSE    32 (to 104)
          
-          21          40 LOAD_GLOBAL              3 (NULL + ValueError)
+          42          40 LOAD_GLOBAL              3 (NULL + ValueError)
                       52 LOAD_CONST               2 ('Expected exactly two quantiles, got ')
                       54 LOAD_GLOBAL              1 (NULL + len)
                       66 LOAD_FAST                0 (quantiles)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 FORMAT_VALUE             0
                       84 LOAD_CONST               3 ('.')
                       86 BUILD_STRING             3
                       88 PRECALL                  1
                       92 CALL                     1
                      102 RAISE_VARARGS            1
          
-          23     >>  104 LOAD_GLOBAL              5 (NULL + list)
+          44     >>  104 LOAD_GLOBAL              5 (NULL + list)
                      116 LOAD_FAST                0 (quantiles)
                      118 LOAD_METHOD              3 (keys)
                      140 PRECALL                  0
                      144 CALL                     0
                      154 PRECALL                  1
                      158 CALL                     1
                      168 STORE_FAST               1 (ps)
          
-          24         170 LOAD_GLOBAL              5 (NULL + list)
+          45         170 LOAD_GLOBAL              5 (NULL + list)
                      182 LOAD_FAST                0 (quantiles)
                      184 LOAD_METHOD              4 (values)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 PRECALL                  1
                      224 CALL                     1
                      234 STORE_FAST               2 (qs)
          
-          27         236 LOAD_GLOBAL             11 (NULL + interp1d)
+          48         236 LOAD_GLOBAL             11 (NULL + interp1d)
                      248 LOAD_FAST                1 (ps)
                      250 LOAD_FAST                2 (qs)
                      252 LOAD_CONST               4 ('linear')
                      254 LOAD_CONST               5 ('extrapolate')
                      256 LOAD_CONST               6 (True)
                      258 KW_NAMES                 7
                      260 PRECALL                  5
                      264 CALL                     5
                      274 STORE_FAST               3 (f)
          
-          28         276 PUSH_NULL
+          49         276 PUSH_NULL
                      278 LOAD_FAST                3 (f)
                      280 LOAD_CONST               8 (0)
                      282 PRECALL                  1
                      286 CALL                     1
                      296 STORE_FAST               4 (min_val)
          
-          29         298 PUSH_NULL
+          50         298 PUSH_NULL
                      300 LOAD_FAST                3 (f)
                      302 LOAD_CONST               9 (1)
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               5 (max_val)
          
-          31         320 LOAD_GLOBAL             13 (NULL + uniform)
+          52         320 LOAD_GLOBAL             13 (NULL + uniform)
                      332 LOAD_FAST                4 (min_val)
                      334 LOAD_FAST                5 (max_val)
                      336 PRECALL                  2
                      340 CALL                     2
                      350 RETURN_VALUE
          consts
             None
@@ -272,39 +273,39 @@
             1
          names      ('len', 'ValueError', 'list', 'keys', 'values', 'interp1d', 'uniform')
          varnames   ('quantiles', 'ps', 'qs', 'f', 'min_val', 'max_val')
          freevars   ()
          cellvars   ()
          filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
          name       'from_quantiles'
-         firstlineno 19
+         firstlineno 40
          lnotab 0x02012601400242014203280116011602
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007c007c016702a6010000ab01000000
             00000000005c0200007d027d037402000000000000000000006a02000000
             0000000000a00300000000000000000000000000000000000000007c027c
             037c027a0a0000ac01a6020000ab0200000000000000005300
-          34           0 RESUME                   0
+          55           0 RESUME                   0
          
-          41           2 LOAD_GLOBAL              1 (NULL + sorted)
+          62           2 LOAD_GLOBAL              1 (NULL + sorted)
                       14 LOAD_FAST                0 (a)
                       16 LOAD_FAST                1 (b)
                       18 BUILD_LIST               2
                       20 PRECALL                  1
                       24 CALL                     1
                       34 UNPACK_SEQUENCE          2
                       38 STORE_FAST               2 (min)
                       40 STORE_FAST               3 (max)
          
-          42          42 LOAD_GLOBAL              2 (scipy)
+          63          42 LOAD_GLOBAL              2 (scipy)
                       54 LOAD_ATTR                2 (stats)
                       64 LOAD_METHOD              3 (uniform)
                       86 LOAD_FAST                2 (min)
                       88 LOAD_FAST                3 (max)
                       90 LOAD_FAST                2 (min)
                       92 BINARY_OP               10 (-)
                       96 KW_NAMES                 1
@@ -316,18 +317,18 @@
             ('loc', 'scale')
          names      ('sorted', 'scipy', 'stats', 'uniform')
          varnames   ('a', 'b', 'min', 'max')
          freevars   ()
          cellvars   ()
          filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
          name       'from_extrema'
-         firstlineno 34
+         firstlineno 55
          lnotab 0x02072801
       (None, None)
    names      ('numbers', 'Real', 'scipy', 'scipy.interpolate', 'interp1d', 'rvtools.construct._helpers', 'parse_spec', 'dict', 'uniform', 'from_quantiles', 'from_extrema')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c0208010c020c032c0a1c0f
+   lnotab 0x00ff02010c0208010c020c032c1f1c0f
```

### Comparing `rvtools-0.1.4/rvtools/construct/_helpers.py` & `rvtools-0.1.5/rvtools/construct/_helpers.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.4/rvtools/construct/beta.py` & `rvtools-0.1.5/rvtools/construct/beta.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,33 @@
 import numpy as np
 import scipy
 
 from rvtools.construct._helpers import parse_spec
 
 
 def beta(alpha: Real = None, beta: Real = None, *, quantiles: dict[Real, Real] = None, **kwargs):
+    """
+    Create a (frozen) SciPy beta distribution.
+
+    You can specify the parameters in one of two ways.
+
+    1. Using ``alpha`` and ``beta``:
+
+    >>> from rvtools.construct import beta
+    >>> beta(1, 2)  # doctest: +ELLIPSIS
+    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>
+
+    2. Using quantiles:
+
+    >>> beta(p5=0.1, p95=0.9) # doctest: +ELLIPSIS
+    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>
+    >>> beta(quantiles={1/1000: 0.1, 999/1000: 0.9})  # doctest: +ELLIPSIS
+    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>
+
+    """
     spec = parse_spec(alpha=alpha, beta=beta, quantiles=quantiles, **kwargs)
     if spec.keys() == {"alpha", "beta"}:
         return scipy.stats.beta(alpha, beta)
     elif spec.keys() == {"quantiles"}:
         return from_quantiles(spec["quantiles"])
     else:
         raise ValueError("You must specify either 'alpha' and 'beta', or 'quantiles'.")
```

### Comparing `rvtools-0.1.4/rvtools/construct/uniform.py` & `rvtools-0.1.5/rvtools/construct/uniform.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,35 @@
 import scipy
 from scipy.interpolate import interp1d
 
 from rvtools.construct._helpers import parse_spec
 
 
 def uniform(a: Real = None, b: Real = None, *, quantiles: dict[Real, Real] = None, **kwargs):
+    """
+    Create a (frozen) SciPy uniform distribution.
+
+    You can specify the parameters in one of two ways.
+
+    1. Using the bounds ``a`` and ``b`` of the distribution:
+
+    >>> from rvtools.construct import uniform
+    >>> uniform(1, 2)  # doctest: +ELLIPSIS
+    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>
+
+    If two positional arguments are given, they are interpreted as ``a`` and ``b``. **This is
+    different from SciPy.**
+
+    2. Using quantiles:
+
+    >>> uniform(p5=0.1, p95=0.9) # doctest: +ELLIPSIS
+    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>
+    >>> uniform(quantiles={1/1000: 0.1, 999/1000: 0.9})  # doctest: +ELLIPSIS
+    <scipy.stats._distn_infrastructure.rv_continuous_frozen object at 0x...>
+    """
     spec = parse_spec(a=a, b=b, quantiles=quantiles, **kwargs)
     if spec.keys() == {"a", "b"}:
         return from_extrema(a, b)
     elif spec.keys() == {"quantiles"}:
         return from_quantiles(spec["quantiles"])
     else:
         raise ValueError("You must specify either the extrema 'a' and 'b', or 'quantiles'.")
```

### Comparing `rvtools-0.1.4/rvtools/distributions/__pycache__/certainty.cpython-311.pyc` & `rvtools-0.1.5/rvtools/dists/gen/__pycache__/certainty.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xbed79964 (Mon Jun 26 18:23:58 2023 UTC)
-files sz: 854
+moddate:  0x55109f64 (Fri Jun 30 17:26:45 2023 UTC)
+files sz: 1243
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064016c025a030200470064028400640365
@@ -21,25 +21,25 @@
      2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              2 (scipy.stats)
                 16 STORE_NAME               3 (scipy)
    
      5          18 PUSH_NULL
                 20 LOAD_BUILD_CLASS
-                22 LOAD_CONST               2 (<code object Certainty, file "/Users/t/repos/rvtools/rvtools/distributions/certainty.py", line 5>)
+                22 LOAD_CONST               2 (<code object Certainty, file "/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py", line 5>)
                 24 MAKE_FUNCTION            0
                 26 LOAD_CONST               3 ('Certainty')
                 28 LOAD_NAME                3 (scipy)
                 30 LOAD_ATTR                4 (stats)
                 40 LOAD_ATTR                5 (rv_continuous)
                 50 PRECALL                  3
                 54 CALL                     3
                 64 STORE_NAME               6 (Certainty)
    
-    31          66 PUSH_NULL
+    47          66 PUSH_NULL
                 68 LOAD_NAME                6 (Certainty)
                 70 PRECALL                  0
                 74 CALL                     0
                 84 STORE_NAME               7 (certainty)
                 86 LOAD_CONST               1 (None)
                 88 RETURN_VALUE
    consts
@@ -55,80 +55,80 @@
             005a06640584005a076408640784015a0864065300
            5           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Certainty')
                        8 STORE_NAME               2 (__qualname__)
          
-           6          10 LOAD_CONST               1 ('\n    The Dirac delta distribution, but at ``value`` instead of 0.\n\n    Represents certainty, but as a continuous distribution.\n    ')
+           6          10 LOAD_CONST               1 ('\n    Represents certainty, but as a continuous distribution, i.e. a subclass of\n    ``scipy.stats.rv_continuous``.\n\n    Like the Dirac delta distribution, but at ``value`` instead of 0.\n\n    :param value: The value where all the probability density is located.\n\n    Examples\n    --------\n    >>> import scipy\n    >>> from rvtools.dists import certainty\n    >>> dist = certainty(42)\n    >>> dist.rvs(3)\n    array([42, 42, 42])\n\n    Has ``pdf`` and all other methods of a continuous distribution:\n\n    >>> dist.pdf(0)\n    0.0\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          12          14 LOAD_CONST               2 (<code object _argcheck, file "/Users/t/repos/rvtools/rvtools/distributions/certainty.py", line 12>)
+          28          14 LOAD_CONST               2 (<code object _argcheck, file "/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py", line 28>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (_argcheck)
          
-          15          20 LOAD_CONST               3 (<code object _pdf, file "/Users/t/repos/rvtools/rvtools/distributions/certainty.py", line 15>)
+          31          20 LOAD_CONST               3 (<code object _pdf, file "/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py", line 31>)
                       22 MAKE_FUNCTION            0
                       24 STORE_NAME               5 (_pdf)
          
-          18          26 LOAD_CONST               4 (<code object _cdf, file "/Users/t/repos/rvtools/rvtools/distributions/certainty.py", line 18>)
+          34          26 LOAD_CONST               4 (<code object _cdf, file "/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py", line 34>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               6 (_cdf)
          
-          21          32 LOAD_CONST               5 (<code object _ppf, file "/Users/t/repos/rvtools/rvtools/distributions/certainty.py", line 21>)
+          37          32 LOAD_CONST               5 (<code object _ppf, file "/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py", line 37>)
                       34 MAKE_FUNCTION            0
                       36 STORE_NAME               7 (_ppf)
          
-          24          38 LOAD_CONST               8 ((None, None))
-                      40 LOAD_CONST               7 (<code object _rvs, file "/Users/t/repos/rvtools/rvtools/distributions/certainty.py", line 24>)
+          40          38 LOAD_CONST               8 ((None, None))
+                      40 LOAD_CONST               7 (<code object _rvs, file "/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py", line 40>)
                       42 MAKE_FUNCTION            1 (defaults)
                       44 STORE_NAME               8 (_rvs)
                       46 LOAD_CONST               6 (None)
                       48 RETURN_VALUE
          consts
             'Certainty'
-            '\n    The Dirac delta distribution, but at ``value`` instead of 0.\n\n    Represents certainty, but as a continuous distribution.\n    '
+            '\n    Represents certainty, but as a continuous distribution, i.e. a subclass of\n    ``scipy.stats.rv_continuous``.\n\n    Like the Dirac delta distribution, but at ``value`` instead of 0.\n\n    :param value: The value where all the probability density is located.\n\n    Examples\n    --------\n    >>> import scipy\n    >>> from rvtools.dists import certainty\n    >>> dist = certainty(42)\n    >>> dist.rvs(3)\n    array([42, 42, 42])\n\n    Has ``pdf`` and all other methods of a continuous distribution:\n\n    >>> dist.pdf(0)\n    0.0\n    '
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c01a60100
                   00ab0100000000000000005300
-                12           0 RESUME                   0
+                28           0 RESUME                   0
                
-                13           2 LOAD_GLOBAL              1 (NULL + np)
+                29           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (isreal)
                             24 LOAD_FAST                1 (value)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('np', 'isreal')
                varnames   ('self', 'value')
                freevars   ()
                cellvars   ()
-               filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+               filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
                name       '_argcheck'
-               firstlineno 12
+               firstlineno 28
                lnotab 0x0201
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c017c026b
                   02000000007400000000000000000000006a0200000000000000006401a6
                   030000ab0300000000000000005300
-                15           0 RESUME                   0
+                31           0 RESUME                   0
                
-                16           2 LOAD_GLOBAL              1 (NULL + np)
+                32           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (where)
                             24 LOAD_FAST                1 (x)
                             26 LOAD_FAST                2 (value)
                             28 COMPARE_OP               2 (==)
                             34 LOAD_GLOBAL              0 (np)
                             46 LOAD_ATTR                2 (inf)
                             56 LOAD_CONST               1 (0)
@@ -138,29 +138,29 @@
                consts
                   None
                   0
                names      ('np', 'where', 'inf')
                varnames   ('self', 'x', 'value')
                freevars   ()
                cellvars   ()
-               filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+               filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
                name       '_pdf'
-               firstlineno 15
+               firstlineno 31
                lnotab 0x0201
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c017c026b
                   000000000064016402a6030000ab0300000000000000005300
-                18           0 RESUME                   0
+                34           0 RESUME                   0
                
-                19           2 LOAD_GLOBAL              1 (NULL + np)
+                35           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (where)
                             24 LOAD_FAST                1 (x)
                             26 LOAD_FAST                2 (value)
                             28 COMPARE_OP               0 (<)
                             34 LOAD_CONST               1 (0)
                             36 LOAD_CONST               2 (1)
                             38 PRECALL                  3
@@ -170,77 +170,77 @@
                   None
                   0
                   1
                names      ('np', 'where')
                varnames   ('self', 'x', 'value')
                freevars   ()
                cellvars   ()
-               filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+               filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
                name       '_cdf'
-               firstlineno 18
+               firstlineno 34
                lnotab 0x0201
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x97007c025300
-                21           0 RESUME                   0
+                37           0 RESUME                   0
                
-                22           2 LOAD_FAST                2 (value)
+                38           2 LOAD_FAST                2 (value)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'x', 'value')
                freevars   ()
                cellvars   ()
-               filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+               filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
                name       '_ppf'
-               firstlineno 21
+               firstlineno 37
                lnotab 0x0201
             None
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c027c01a6
                   020000ab0200000000000000005300
-                24           0 RESUME                   0
+                40           0 RESUME                   0
                
-                25           2 LOAD_GLOBAL              1 (NULL + np)
+                41           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (full)
                             24 LOAD_FAST                2 (size)
                             26 LOAD_FAST                1 (value)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 RETURN_VALUE
                consts
                   None
                names      ('np', 'full')
                varnames   ('self', 'value', 'size', 'random_state')
                freevars   ()
                cellvars   ()
-               filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+               filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
                name       '_rvs'
-               firstlineno 24
+               firstlineno 40
                lnotab 0x0201
             (None, None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', '_argcheck', '_pdf', '_cdf', '_ppf', '_rvs')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+         filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
          name       'Certainty'
          firstlineno 5
-         lnotab 0x0a0104060603060306030603
+         lnotab 0x0a0104160603060306030603
       'Certainty'
    names      ('numpy', 'np', 'scipy.stats', 'scipy', 'stats', 'rv_continuous', 'Certainty', 'certainty')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/t/repos/rvtools/rvtools/distributions/certainty.py'
+   filename   '/Users/t/repos/rvtools/rvtools/dists/gen/certainty.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010803301a
+   lnotab 0x00ff020108010803302a
```

### Comparing `rvtools-0.1.4/rvtools/distributions/tp_uniform.py` & `rvtools-0.1.5/rvtools/dists/gen/tp_uniform.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,148 +6,137 @@
 """
 
 import numpy as np
 import scipy
 
 
 class TwoPieceUniform(scipy.stats.rv_continuous):
-    def _argcheck(self, mini, q, maxi, p):
-        return argcheck(mini, q, maxi, p)
-
-    def _get_support(self, mini, q, maxi, p):
-        return get_support(mini, q, maxi, p)
-
-    def _rvs(self, mini, q, maxi, p, size=None, random_state=None):
-        return rvs(mini, q, maxi, p, size, random_state)
-
-    def _pdf(self, x, mini, q, maxi, p):
-        return np.vectorize(pdf_single)(x, mini, q, maxi, p)
-
-    def _cdf(self, x, mini, q, maxi, p):
-        return np.vectorize(cdf_single)(x, mini, q, maxi, p)
-
-    def _ppf(self, p_caller, mini, q, maxi, p):
-        return np.vectorize(ppf_single)(p_caller, mini, q, maxi, p)
-
-    def _stats(self, mini, q, maxi, p):
-        return stats(mini, q, maxi, p)
-
-
-class HalvesUniform(scipy.stats.rv_continuous):
-    def _argcheck(self, mini, q, maxi):
-        return argcheck(mini, q, maxi)
+    """
+    A piecewise uniform distribution with two pieces.
 
-    def _get_support(self, mini, q, maxi):
-        return get_support(mini, q, maxi)
+    :param mini: The left bound of the distribution.
+    :param sep: The boundary between the left and right pieces.
+    :param maxi: The right bound of the distribution.
+    :param psep: The probability at ``sep``, i.e. the probability of the left piece, i.e. ``P(X < sep) = psep``.
+
+    Examples
+    --------
+    >>> from rvtools.dists import tp_uniform
+    >>> dist = tp_uniform(0, 3, 10, psep=0.1)
+    """
 
-    def _rvs(self, mini, q, maxi, size=None, random_state=None):
-        return rvs(mini, q, maxi, size, random_state)
+    def _argcheck(self, mini, sep, maxi, psep):
+        return argcheck(mini, sep, maxi, psep)
 
-    def _pdf(self, x, mini, q, maxi):
-        return np.vectorize(pdf_single)(x, mini, q, maxi)
+    def _get_support(self, mini, sep, maxi, psep):
+        return get_support(mini, sep, maxi, psep)
 
-    def _cdf(self, x, mini, q, maxi):
-        return np.vectorize(cdf_single)(x, mini, q, maxi)
+    def _rvs(self, mini, sep, maxi, psep, size=None, random_state=None):
+        return rvs(mini, sep, maxi, psep, size=size, random_state=random_state)
 
-    def _ppf(self, p_caller, mini, q, maxi):
-        return np.vectorize(ppf_single)(p_caller, mini, q, maxi)
+    def _pdf(self, x, mini, sep, maxi, psep):
+        return np.vectorize(pdf_single)(x, mini, sep, maxi, psep)
 
-    def _stats(self, mini, q, maxi):
-        return stats(mini, q, maxi)
+    def _cdf(self, x, mini, sep, maxi, psep):
+        return np.vectorize(cdf_single)(x, mini, sep, maxi, psep)
 
+    def _ppf(self, p, mini, sep, maxi, psep):
+        return np.vectorize(ppf_single)(p, mini, sep, maxi, psep)
 
-# ``tp_uniform`` and ``halves_uniform`` being instances, not a classes, is not IMO idiomatic Python, but it's core to
-# the way SciPy's ``rv_continuous`` class works. See examples of how SciPy defines their distributions in
-# ``scipy/stats/_continuous_distns.py``.
-tp_uniform = TwoPieceUniform()
-halves_uniform = HalvesUniform()
+    def _stats(self, mini, sep, maxi, psep):
+        return stats(mini, sep, maxi, psep)
 
 
-def argcheck(mini, q, maxi, p=0.5):
-    return mini <= q <= maxi and 0 <= p <= 1
+def argcheck(mini, sep, maxi, psep=0.5):
+    return mini <= sep <= maxi and 0 <= psep <= 1
 
 
-def get_support(mini, q, maxi, p=0.5):
+def get_support(mini, sep, maxi, psep=0.5):
     return mini, maxi
 
 
-def rvs(mini, q, maxi, p=0.5, size=None, random_state=None):
+def rvs(mini, sep, maxi, psep=0.5, size=None, random_state=None):
     """
     With size proportional to p, sample from a uniform distribution on [mini, q]. With
     size propotional to 1-p, sample from a uniform distribution on [q, maxi].
     """
-    size_left = np.ceil(size * p).astype(int)
+    if size is not None:
+        if len(size) == 1:  # Caller will give this as (size,)
+            size = size[0]
+        else:
+            raise NotImplementedError("size must be a scalar for TwoPieceUniform")
+    size_left = np.ceil(size * psep).astype(int)
     size_right = size - size_left
 
-    samples_left = np.random.uniform(mini, q, size_left)
-    samples_right = np.random.uniform(q, maxi, size_right)
+    samples_left = np.random.uniform(mini, sep, size_left)
+    samples_right = np.random.uniform(sep, maxi, size_right)
     return np.concatenate([samples_left, samples_right])
 
 
-def pdf_single(x, mini, q, maxi, p=0.5):
-    if mini <= x <= q:
-        return p * _uniform_pdf(x, mini, q)
-    elif q <= x <= maxi:
-        return (1 - p) * _uniform_pdf(x, q, maxi)
+def pdf_single(x, mini, sep, maxi, psep=0.5):
+    if mini <= x <= sep:
+        return psep * _uniform_pdf(x, mini, sep)
+    elif sep <= x <= maxi:
+        return (1 - psep) * _uniform_pdf(x, sep, maxi)
     else:
         return 0
 
 
-def cdf_single(x, mini, q, maxi, p=0.5):
+def cdf_single(x, mini, sep, maxi, psep=0.5):
     if x < mini:
         return 0
-    elif mini <= x < q:
-        return p * ((x - mini) / (q - mini))
-    elif q <= x < maxi:
-        return p + (1 - p) * ((x - q) / (maxi - q))
+    elif mini <= x < sep:
+        return psep * ((x - mini) / (sep - mini))
+    elif sep <= x < maxi:
+        return psep + (1 - psep) * ((x - sep) / (maxi - sep))
     else:  # x >= maxi
         return 1
 
 
-def ppf_single(p_caller, mini, q, maxi, p=0.5):
-    if 0 <= p_caller < p:
-        return mini + p_caller / p * (q - mini)
-    elif p <= p_caller <= 1:
-        return q + (p_caller - p) / (1 - p) * (maxi - q)
+def ppf_single(p, mini, sep, maxi, psep=0.5):
+    if 0 <= p < psep:
+        return mini + p / psep * (sep - mini)
+    elif psep <= p <= 1:
+        return sep + (p - psep) / (1 - psep) * (maxi - sep)
     else:
         return np.nan
 
 
-def stats(mini, q, maxi, p=0.5):
-    mean_left = (mini + q) / 2
-    mean_right = (q + maxi) / 2
-    mean = p * mean_left + (1 - p) * mean_right
+def stats(mini, sep, maxi, psep=0.5):
+    mean_left = (mini + sep) / 2
+    mean_right = (sep + maxi) / 2
+    mean = psep * mean_left + (1 - psep) * mean_right
 
-    var = _var(mini, q, maxi, p)
+    var = _var(mini, sep, maxi, psep)
 
     # These will be calculated (inefficiently) by SciPy's generic methods
     skew = None
     kurt = None
 
     return mean, var, skew, kurt
 
 
-def _var(mini, q, maxi, p):
+def _var(mini, sep, maxi, psep):
     # Calculate variance within each piece
-    var1 = p * (q - mini) ** 2 / 12
-    var2 = (1 - p) * (maxi - q) ** 2 / 12
+    var1 = psep * (sep - mini) ** 2 / 12
+    var2 = (1 - psep) * (maxi - sep) ** 2 / 12
 
     # Calculate the means of each piece
-    mean1 = (mini + q) / 2
-    mean2 = (maxi + q) / 2
+    mean1 = (mini + sep) / 2
+    mean2 = (maxi + sep) / 2
 
     # Calculate the overall mean of the piecewise distribution
-    overall_mean = p * mean1 + (1 - p) * mean2
+    overall_mean = psep * mean1 + (1 - psep) * mean2
 
     # Calculate the additional contribution to the due to the difference between the mean of each piece and the
     # overall mean. Each piece's mean contributes to the total variance in proportion to the square of its distance
     # from the overall mean, and the contribution is also weighted by the probability of the piece (since this is how
     # often we'd expect to be in this piece).
-    var_mean_diff1 = p * (mean1 - overall_mean) ** 2
-    var_mean_diff2 = (1 - p) * (mean2 - overall_mean) ** 2
+    var_mean_diff1 = psep * (mean1 - overall_mean) ** 2
+    var_mean_diff2 = (1 - psep) * (mean2 - overall_mean) ** 2
 
     # Total variance
     variance = var1 + var2 + var_mean_diff1 + var_mean_diff2
 
     return variance
 
 
@@ -155,7 +144,13 @@
     """
     Helper. Using `scipy.stats.uniform`, would require converting to (loc, scale) form and make the code more confusing.
     """
     if mini <= x <= maxi:
         return 1 / (maxi - mini)
     else:
         return 0
+
+
+# These being instances, not a classes, is not IMO idiomatic Python, but it's core to the way SciPy's
+# ``rv_continuous`` class works. See examples of how SciPy defines their distributions in
+# ``scipy/stats/_continuous_distns.py``.
+tp_uniform = TwoPieceUniform()
```

### Comparing `rvtools-0.1.4/tests/test_constructors.py` & `rvtools-0.1.5/tests/test_constructors.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,60 +11,60 @@
     Assert that a (frozen) distribution has the given quantiles.
     """
     for p, q in quantiles.items():
         assert d.cdf(q) == pytest.approx(p)
 
 
 class TestBeta:
-    @pytest.fixture(params=[0.5, 3], ids=lambda p: f"alpha={p}")
+    @pytest.fixture(params=[0.5, 3], ids=lambda psep: f"alpha={psep}")
     def alpha(self, request):
         return request.param
 
-    @pytest.fixture(params=[1, 5], ids=lambda p: f"beta={p}")
+    @pytest.fixture(params=[1, 5], ids=lambda psep: f"beta={psep}")
     def beta(self, request):
         return request.param
 
     @pytest.mark.parametrize("as_kwargs", [True, False], ids=lambda x: "kwargs" if x else "args")
     def test_from_alpha_beta(self, alpha, beta, as_kwargs):
         if as_kwargs:
             our_d = construct.beta(alpha=alpha, beta=beta)
         else:
             our_d = construct.beta(alpha, beta)
         scipy_d = scipy.stats.beta(alpha, beta)
         assert_same_distribution(our_d, scipy_d)
 
     @pytest.fixture(
         params=[{0.1: 0.2, 0.5: 0.85}, {0.1: 0.5, 0.5: 0.99}, {0.001: 0.5, 0.5: 0.99}],  # #  #
-        ids=lambda p: f"quantiles={p}",
+        ids=lambda psep: f"quantiles={psep}",
     )
     def quantiles(self, request):
         return request.param
 
     def test_from_quantiles(self, quantiles):
         assert_has_quantiles(construct.beta(quantiles=quantiles), quantiles)
 
     def test_too_many_args(self):
         with pytest.raises(ValueError, match="You must specify"):
             construct.beta(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
 
 
 class TestLognorm:
-    @pytest.fixture(params=[0.5, 3], ids=lambda p: f"mean={p}")
+    @pytest.fixture(params=[0.5, 3], ids=lambda psep: f"mean={psep}")
     def mean(self, request):
         return request.param
 
-    @pytest.fixture(params=[1, 5], ids=lambda p: f"sd={p}")
+    @pytest.fixture(params=[1, 5], ids=lambda psep: f"sd={psep}")
     def sd(self, request):
         return request.param
 
-    @pytest.fixture(params=[0.5, 3], ids=lambda p: f"mu={p}")
+    @pytest.fixture(params=[0.5, 3], ids=lambda psep: f"mu={psep}")
     def mu(self, request):
         return request.param
 
-    @pytest.fixture(params=[1, 5], ids=lambda p: f"sigma={p}")
+    @pytest.fixture(params=[1, 5], ids=lambda psep: f"sigma={psep}")
     def sigma(self, request):
         return request.param
 
     @pytest.fixture
     def quantiles(self):
         return {0.1: 1, 0.9: 10}
 
@@ -96,19 +96,19 @@
         with pytest.raises(ValueError, match="You must specify"):
             construct.lognorm(1, 1, mean=1)
         with pytest.raises(ValueError, match="You must specify"):
             construct.lognorm(mean=1, sd=1, mu=1)
 
 
 class TestNorm:
-    @pytest.fixture(params=[0.5, 3], ids=lambda p: f"mean={p}")
+    @pytest.fixture(params=[0.5, 3], ids=lambda psep: f"mean={psep}")
     def mean(self, request):
         return request.param
 
-    @pytest.fixture(params=[1, 5], ids=lambda p: f"sd={p}")
+    @pytest.fixture(params=[1, 5], ids=lambda psep: f"sd={psep}")
     def sd(self, request):
         return request.param
 
     @pytest.fixture
     def quantiles(self):
         return {0.1: -1, 0.9: 1}
 
@@ -136,15 +136,15 @@
             # Small numbers
             (1e-10, 1e-9),
         ]
     )
     def pair(self, request):
         return request.param
 
-    @pytest.fixture(params=[{0.1: 1, 0.9: 2}], ids=lambda p: f"quantiles={p}")
+    @pytest.fixture(params=[{0.1: 1, 0.9: 2}], ids=lambda psep: f"quantiles={psep}")
     def quantiles(self, request):
         return request.param
 
     def test_from_pair(self, pair):
         dist = construct.uniform(*pair)
         assert dist.ppf(0.5) == pytest.approx(np.mean(pair))
         assert dist.support() == pytest.approx(sorted(pair))
@@ -162,15 +162,15 @@
     @pytest.fixture(
         params=[
             # A simple case
             {0.1: 1, 0.9: 10_000},
             # Small numbers
             {0.1: 1e-6, 0.9: 1e-5},
         ],
-        ids=lambda p: f"quantiles={p}",
+        ids=lambda psep: f"quantiles={psep}",
     )
     def quantiles(self, request):
         return request.param
 
     def test_from_quantiles(self, quantiles):
         dist = construct.loguniform(quantiles=quantiles)
         assert_has_quantiles(dist, quantiles)
```

### Comparing `rvtools-0.1.4/tests/test_parse_spec.py` & `rvtools-0.1.5/tests/test_parse_spec.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.4/tests/test_tp_uniform.py` & `rvtools-0.1.5/tests/test_tp_uniform.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import pytest
 import scipy
 
-from rvtools import tp_uniform
+from rvtools.dists import tp_uniform
 from rvtools.construct import uniform
-from rvtools.distributions.tp_uniform import TwoPieceUniform, halves_uniform
+from rvtools.dists import halves_uniform
+from rvtools.dists.gen.tp_uniform import TwoPieceUniform
 from tests.conftest import assert_same_distribution
 
 
 @pytest.fixture(
     params=[
         # A simple case
         (0, 1, 3),
@@ -26,40 +27,40 @@
     ids=lambda param: f"mini={param[0]}, q={param[1]}, maxi={param[2]}",
 )
 def param_triple(request):
     return request.param
 
 
 @pytest.fixture(params=[0.90, 0.05, 1 / 3], ids=lambda p: f"p={p}")
-def p_param(request):
+def psep(request):
     return request.param
 
 
-def test_rvs(param_triple, p_param):
-    mini, q, maxi = param_triple
-    dist = tp_uniform(mini=mini, q=q, maxi=maxi, p=p_param)
+def test_rvs(param_triple, psep):
+    mini, sep, maxi = param_triple
+    dist = tp_uniform(mini=mini, sep=sep, maxi=maxi, psep=psep)
 
     # When size=1, deterministically only 1 sample from the left side is returned
-    assert mini <= dist.rvs(size=1, random_state=0) <= q
+    assert mini <= dist.rvs(size=1, random_state=0) <= sep
 
 
-def test_pdf_any(param_triple, p_param):
-    mini, q, maxi = param_triple
-    dist = tp_uniform(mini=mini, q=q, maxi=maxi, p=p_param)
+def test_pdf_any(param_triple, psep):
+    mini, sep, maxi = param_triple
+    dist = tp_uniform(mini=mini, sep=sep, maxi=maxi, psep=psep)
 
     assert dist.pdf(mini - 1) == pytest.approx(0)
     assert dist.pdf(maxi + 1) == pytest.approx(0)
 
 
-def test_cdf_any(param_triple, p_param):
-    mini, q, maxi = param_triple
-    dist = tp_uniform(mini=mini, q=q, maxi=maxi, p=p_param)
+def test_cdf_any(param_triple, psep):
+    mini, sep, maxi = param_triple
+    dist = tp_uniform(mini=mini, sep=sep, maxi=maxi, psep=psep)
 
     assert dist.cdf(mini - 1e-6) == pytest.approx(0)
-    assert dist.cdf(q) == pytest.approx(p_param)
+    assert dist.cdf(sep) == pytest.approx(psep)
     assert dist.cdf(maxi + 1e-6) == pytest.approx(1)
 
 
 def test_pdf_case_1():
     # Same width, pi=(0.5, 0.5)
     dist = tp_uniform(0, 1, 2, 0.5)
     assert dist.pdf(0.1) == pytest.approx(0.5)
@@ -93,48 +94,54 @@
     assert_same_distribution(dist, uniform(mini, maxi))
 
     dist = tp_uniform(mini, maxi, maxi, 1)
     assert_same_distribution(dist, uniform(mini, maxi))
 
 
 @pytest.fixture()
-def numerical_cdf_dist(param_triple, p_param):
+def numerical_cdf_dist(param_triple, psep):
     class NumericalCDFTwoPieceUniform(TwoPieceUniform):
         def _cdf(self, x, *args, **kwargs):
             return scipy.stats.rv_continuous._cdf(self, x, *args, **kwargs)
 
     # Follow SciPy pattern
     numerical_cdf_tp_uniform = NumericalCDFTwoPieceUniform()
 
-    return numerical_cdf_tp_uniform(*param_triple, p_param)
+    return numerical_cdf_tp_uniform(*param_triple, psep)
 
 
-def test_cdf_matches_numerical(param_triple, p_param, numerical_cdf_dist):
+def test_cdf_matches_numerical(param_triple, psep, numerical_cdf_dist):
     """
     The CDF (which we have in closed form) matches the CDF obtained by numerically integrating the PDF.
     """
-    mini, q, maxi = param_triple
+    mini, sep, maxi = param_triple
     x = np.linspace(mini, maxi, 10)
 
     numerical = numerical_cdf_dist.cdf(x)
-    closed_form = tp_uniform.cdf(x, mini, q, maxi, p_param)
+    closed_form = tp_uniform.cdf(x, mini, sep, maxi, psep)
 
     assert numerical == pytest.approx(closed_form)
 
 
-def test_mean_var(param_triple, p_param, random_seed):
+def test_mean_var(param_triple, psep, random_seed):
     """
     mean() and var() (closed form) matches empirical mean and variance from sampling
 
     Not using expect() here because the kinks in the distribution make it hard for numerical integration to be accurate.
     """
-    mini, q, maxi = param_triple
-    dist = tp_uniform(mini, q, maxi, p_param)
+    mini, sep, maxi = param_triple
+    dist = tp_uniform(mini, sep, maxi, psep)
     samples = dist.rvs(size=int(1e7))
 
     assert dist.mean() == pytest.approx(np.mean(samples), rel=1 / 1000)
     assert dist.var() == pytest.approx(np.var(samples), rel=1 / 1000)
 
 
 def test_generalization(param_triple):
-    mini, q, maxi = param_triple
-    assert_same_distribution(tp_uniform(mini, q, maxi, 0.5), halves_uniform(mini, q, maxi))
+    mini, sep, maxi = param_triple
+    assert_same_distribution(tp_uniform(mini, sep, maxi, 0.5), halves_uniform(mini, sep, maxi))
+
+
+def test_rvs_does_not_raise(param_triple):
+    mini, sep, maxi = param_triple
+    dist = tp_uniform(mini, sep, maxi, 0.5)
+    dist.rvs(size=10)
```

