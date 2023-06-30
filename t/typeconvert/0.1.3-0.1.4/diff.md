# Comparing `tmp/typeconvert-0.1.3.tar.gz` & `tmp/typeconvert-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeconvert-0.1.3.tar", last modified: Wed Jan 25 01:57:31 2023, max compression
+gzip compressed data, was "typeconvert-0.1.4.tar", last modified: Fri Jun 30 13:07:46 2023, max compression
```

## Comparing `typeconvert-0.1.3.tar` & `typeconvert-0.1.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.599589 typeconvert-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.575589 typeconvert-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.579589 typeconvert-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-01-25 01:57:20.000000 typeconvert-0.1.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-25 01:57:20.000000 typeconvert-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-25 01:57:20.000000 typeconvert-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-25 01:57:20.000000 typeconvert-0.1.3/.github/workflows/python-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-25 01:57:20.000000 typeconvert-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-25 01:57:20.000000 typeconvert-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-01-25 01:57:31.595589 typeconvert-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-01-25 01:57:20.000000 typeconvert-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-25 01:57:20.000000 typeconvert-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.579589 typeconvert-0.1.3/references/
--rw-r--r--   0 runner    (1001) docker     (123)   103934 2023-01-25 01:57:20.000000 typeconvert-0.1.3/references/IRIG106-20_Appendix9D.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.579589 typeconvert-0.1.3/references/dec/
--rw-r--r--   0 runner    (1001) docker     (123)    25034 2023-01-25 01:57:20.000000 typeconvert-0.1.3/references/dec/libvaxdata.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)   217094 2023-01-25 01:57:20.000000 typeconvert-0.1.3/references/dec/of2005-1424_v1.2.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.583589 typeconvert-0.1.3/references/milstd1750a/
--rw-r--r--   0 runner    (1001) docker     (123)   420119 2023-01-25 01:57:20.000000 typeconvert-0.1.3/references/milstd1750a/milstd1750a.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.583589 typeconvert-0.1.3/references/ti/
--rw-r--r--   0 runner    (1001) docker     (123)  4421260 2023-01-25 01:57:20.000000 typeconvert-0.1.3/references/ti/spra400.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 01:57:31.599589 typeconvert-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.579589 typeconvert-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.587589 typeconvert-0.1.3/src/typeconvert/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/njit.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/pyfunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.595589 typeconvert-0.1.3/src/typeconvert/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/bcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/dec32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/dec64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/dec64g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/ibm32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/ibm64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/milstd1750a32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/milstd1750a48.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/onescomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/ti32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/ti40.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/types/twoscomp.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/ufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-25 01:57:20.000000 typeconvert-0.1.3/src/typeconvert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.591589 typeconvert-0.1.3/src/typeconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-01-25 01:57:31.000000 typeconvert-0.1.3/src/typeconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-01-25 01:57:31.000000 typeconvert-0.1.3/src/typeconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 01:57:31.000000 typeconvert-0.1.3/src/typeconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-25 01:57:31.000000 typeconvert-0.1.3/src/typeconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-25 01:57:31.000000 typeconvert-0.1.3/src/typeconvert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:57:31.595589 typeconvert-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_1750a32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_1750a48.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_bcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_dec32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_dec64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_dec64g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_ibm32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_ibm64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_onescomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_ti32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_ti40.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-01-25 01:57:20.000000 typeconvert-0.1.3/tests/test_twoscomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.544947 typeconvert-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.532947 typeconvert-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.532947 typeconvert-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-30 13:07:36.000000 typeconvert-0.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-30 13:07:36.000000 typeconvert-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 13:07:36.000000 typeconvert-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-30 13:07:36.000000 typeconvert-0.1.4/.github/workflows/python-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 13:07:36.000000 typeconvert-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 13:07:36.000000 typeconvert-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-30 13:07:46.544947 typeconvert-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-30 13:07:36.000000 typeconvert-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-30 13:07:36.000000 typeconvert-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.532947 typeconvert-0.1.4/references/
+-rw-r--r--   0 runner    (1001) docker     (123)   103934 2023-06-30 13:07:36.000000 typeconvert-0.1.4/references/IRIG106-20_Appendix9D.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.532947 typeconvert-0.1.4/references/dec/
+-rw-r--r--   0 runner    (1001) docker     (123)    25034 2023-06-30 13:07:36.000000 typeconvert-0.1.4/references/dec/libvaxdata.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   217094 2023-06-30 13:07:36.000000 typeconvert-0.1.4/references/dec/of2005-1424_v1.2.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.532947 typeconvert-0.1.4/references/milstd1750a/
+-rw-r--r--   0 runner    (1001) docker     (123)   420119 2023-06-30 13:07:36.000000 typeconvert-0.1.4/references/milstd1750a/milstd1750a.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.536947 typeconvert-0.1.4/references/ti/
+-rw-r--r--   0 runner    (1001) docker     (123)  4421260 2023-06-30 13:07:36.000000 typeconvert-0.1.4/references/ti/spra400.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:07:46.544947 typeconvert-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.532947 typeconvert-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.540947 typeconvert-0.1.4/src/typeconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/njit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/pyfunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.540947 typeconvert-0.1.4/src/typeconvert/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/bcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/dec32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/dec64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/dec64g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/ibm32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/ibm64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/milstd1750a32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/milstd1750a48.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/onescomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/ti32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/ti40.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/types/twoscomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/ufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-30 13:07:36.000000 typeconvert-0.1.4/src/typeconvert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.540947 typeconvert-0.1.4/src/typeconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-30 13:07:46.000000 typeconvert-0.1.4/src/typeconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-30 13:07:46.000000 typeconvert-0.1.4/src/typeconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:07:46.000000 typeconvert-0.1.4/src/typeconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 13:07:46.000000 typeconvert-0.1.4/src/typeconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 13:07:46.000000 typeconvert-0.1.4/src/typeconvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:07:46.544947 typeconvert-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_1750a32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_1750a48.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_bcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_dec32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_dec64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_dec64g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_ibm32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_ibm64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_onescomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_ti32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_ti40.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-30 13:07:36.000000 typeconvert-0.1.4/tests/test_twoscomp.py
```

### Comparing `typeconvert-0.1.3/.github/workflows/codeql-analysis.yml` & `typeconvert-0.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/.github/workflows/python-package.yml` & `typeconvert-0.1.4/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `typeconvert-0.1.3/.github/workflows/python-publish.yml` & `typeconvert-0.1.4/.github/workflows/python-publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
+
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
         python-version: '3.x'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build wheel setuptools
 
     - name: Build package
       run: python -m build
 
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `typeconvert-0.1.3/.gitignore` & `typeconvert-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/LICENSE.md` & `typeconvert-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/PKG-INFO` & `typeconvert-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeconvert
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert various unusual data types into integers and floats
 License: # MIT License
         
         Copyright (c) 2022 Jonathan Olsten
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `typeconvert-0.1.3/README.md` & `typeconvert-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/pyproject.toml` & `typeconvert-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,40 @@
 name = "typeconvert"
 description = "Convert various unusual data types into integers and floats"
 readme = {file = "README.md", content-type = "text/markdown"}
 dynamic = ["version"]
 requires-python = ">= 3.7"
 license = {file = "LICENSE.md"}
 dependencies = [
-    "numba",
-    "numpy",
+    "numba>=0.53",
+    "numpy>=1.19,<1.24",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
 ]
 
 [project.urls]
 repository = "https://github.com/jolsten/type-convert"
 
 [project.optional-dependencies]
 dev = [
+  "build",
+  "setuptools>=45",
+  "setuptools_scm[toml]>=6.2",
+  "wheel",
   "pytest",
   "pytest-cov",
 ]
 
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["typeconvert"]
+
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov=typeconvert --cov-report html"
 testpaths = [
     "tests",
```

### Comparing `typeconvert-0.1.3/references/IRIG106-20_Appendix9D.pdf` & `typeconvert-0.1.4/references/IRIG106-20_Appendix9D.pdf`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/references/dec/libvaxdata.tar.gz` & `typeconvert-0.1.4/references/dec/libvaxdata.tar.gz`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/references/dec/of2005-1424_v1.2.pdf` & `typeconvert-0.1.4/references/dec/of2005-1424_v1.2.pdf`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/references/milstd1750a/milstd1750a.pdf` & `typeconvert-0.1.4/references/milstd1750a/milstd1750a.pdf`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/references/ti/spra400.pdf` & `typeconvert-0.1.4/references/ti/spra400.pdf`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/njit.py` & `typeconvert-0.1.4/src/typeconvert/njit.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/pyfunc.py` & `typeconvert-0.1.4/src/typeconvert/pyfunc.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/bcd.py` & `typeconvert-0.1.4/src/typeconvert/types/bcd.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/dec32.py` & `typeconvert-0.1.4/src/typeconvert/types/dec32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/dec64.py` & `typeconvert-0.1.4/src/typeconvert/types/dec64.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/dec64g.py` & `typeconvert-0.1.4/src/typeconvert/types/dec64g.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/ibm32.py` & `typeconvert-0.1.4/src/typeconvert/types/ibm32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/ibm64.py` & `typeconvert-0.1.4/src/typeconvert/types/ibm64.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/milstd1750a32.py` & `typeconvert-0.1.4/src/typeconvert/types/milstd1750a32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/milstd1750a48.py` & `typeconvert-0.1.4/src/typeconvert/types/milstd1750a48.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 
 # Reference(s):
 # http://www.xgc-tek.com/manuals/mil-std-1750a/c191.html
 
 
 def func(value: np.uint64) -> np.float64:
-    r"""Convert uint to 1750A32
+    r"""Convert uint to 1750A48
 
     Interprets an unsigned integer as a MIL-STD-1750A 48-bit Float and returns
     an IEEE 64-bit Float.
 
     Parameters
     ----------
     value : unsigned integer
```

### Comparing `typeconvert-0.1.3/src/typeconvert/types/onescomp.py` & `typeconvert-0.1.4/src/typeconvert/types/onescomp.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     >>> type(out), out
     (<class 'numpy.int64'>, -1)
     """
     value = np.uint64(value)
     pad_bits = np.uint8(64-size)
     if value & (np.uint64(1) << np.uint8(size-1)) != 0:
         return -np.int64((~(value << pad_bits)) >> pad_bits)
-    return value
+    return np.int64(value)
 
 
 jfunc = njit(signatures)(func)
 ufunc = vectorize(signatures)(func)
```

### Comparing `typeconvert-0.1.3/src/typeconvert/types/ti32.py` & `typeconvert-0.1.4/src/typeconvert/types/ti32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/ti40.py` & `typeconvert-0.1.4/src/typeconvert/types/ti40.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert/types/twoscomp.py` & `typeconvert-0.1.4/src/typeconvert/types/twoscomp.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,12 +33,14 @@
     >>> type(out), out
     (<class 'numpy.int64'>, -1)
     """
     value = np.uint64(value)
     if value >= 2**(size-1):
         pad_bits = np.uint8(64 - size)
         value = np.int64(np.uint64(value) << pad_bits) >> pad_bits
-    return value
+        return value
+    else:
+        return np.int64(value)
 
 
 jfunc = njit(signatures)(func)
 ufunc = vectorize(signatures)(func)
```

### Comparing `typeconvert-0.1.3/src/typeconvert/ufunc.py` & `typeconvert-0.1.4/src/typeconvert/ufunc.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/src/typeconvert.egg-info/PKG-INFO` & `typeconvert-0.1.4/src/typeconvert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeconvert
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert various unusual data types into integers and floats
 License: # MIT License
         
         Copyright (c) 2022 Jonathan Olsten
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `typeconvert-0.1.3/src/typeconvert.egg-info/SOURCES.txt` & `typeconvert-0.1.4/src/typeconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_1750a32.py` & `typeconvert-0.1.4/tests/test_1750a32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_1750a48.py` & `typeconvert-0.1.4/tests/test_1750a48.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_bcd.py` & `typeconvert-0.1.4/tests/test_bcd.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_dec32.py` & `typeconvert-0.1.4/tests/test_dec32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_dec64.py` & `typeconvert-0.1.4/tests/test_dec64.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_dec64g.py` & `typeconvert-0.1.4/tests/test_dec64g.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_ibm32.py` & `typeconvert-0.1.4/tests/test_ibm32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_ibm64.py` & `typeconvert-0.1.4/tests/test_ibm64.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_onescomp.py` & `typeconvert-0.1.4/tests/test_twoscomp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,103 @@
 import pytest
 import numpy as np
 from itertools import zip_longest
 from typeconvert.utils import bits_to_wordsize, mask
-from typeconvert.types.onescomp import func, jfunc, ufunc
+from typeconvert.types.twoscomp import func, jfunc, ufunc
+
+def size_hex(size: int) -> int:
+    return int(bits_to_wordsize(size) / 4)
 
 TEST_ARRAY_SIZE = 100
 TEST_CASES = {
     3: [
         (0b000,  0),
         (0b001,  1),
         (0b010,  2),
         (0b011,  3),
-        (0b100, -3),
-        (0b101, -2),
-        (0b110, -1),
-        (0b111, -0),
+        (0b100, -4),
+        (0b101, -3),
+        (0b110, -2),
+        (0b111, -1),
     ],
     8: [
         (0b00000000,    0),
         (0b00000001,    1),
         (0b00000010,    2),
         (0b01111110,  126),
         (0b01111111,  127),
-        (0b10000000, -127),
-        (0b10000001, -126),
-        (0b10000010, -125),
-        (0b11111110,   -1),
-        (0b11111111,   -0),
+        (0b10000000, -128),
+        (0b10000001, -127),
+        (0b10000010, -126),
+        (0b11111110,   -2),
+        (0b11111111,   -1),
     ],
     16: [
         (0x0000,  0),
-        (0xFFFF,  0),
+        (0x7FFF, 2**15-1),
+        (0x8000, -2**15),
+        (0xFFFF, -1),
     ],
     24: [
         (0x000000,  0),
-        (0xFFFFFF,  0),
+        (0x7FFFFF, 2**23-1),
+        (0x800000, -2**23),
+        (0xFFFFFF, -1),
     ],
     32: [
         (0x00000000,  0),
-        (0xFFFFFFFF,  0),
+        (0x7FFFFFFF, 2**31-1),
+        (0x80000000, -2**31),
+        (0xFFFFFFFF, -1),
     ],
     48: [
         (0x000000000000,  0),
-        (0xFFFFFFFFFFFF,  0),
+        (0x7FFFFFFFFFFF, 2**47-1),
+        (0x800000000000, -2**47),
+        (0xFFFFFFFFFFFF, -1),
     ],
     64: [
         (0x0000000000000000,  0),
-        (0xFFFFFFFFFFFFFFFF,  0),
+        (0x7FFFFFFFFFFFFFFF, 2**63-1),
+        (0x8000000000000000, -2**63),
+        (0xFFFFFFFFFFFFFFFF, -1),
     ],
 }
 
 tests = []
 for size in TEST_CASES:
     for val_in, val_out in TEST_CASES[size]:
         tests.append((size, val_in, val_out))
 tests += [(size, 0, 0) for size in np.arange(64)+1]
-tests += [(size, mask(size), -0) for size in np.arange(64)+1]
+tests += [(size, mask(size), -1) for size in np.arange(64)+1]
 
 
 @pytest.mark.parametrize('size, val_in, val_out', tests)
 def test_func(size, val_in, val_out):
-    print('zzz', val_in, size, val_out)
-    size = np.uint8(size)
+    print('func')
+    print(f'check {val_in:0{size_hex(size)}X}')
     assert func(val_in, size) == val_out
 
 
 @pytest.mark.parametrize('size, val_in, val_out', tests)
 def test_njit(size, val_in, val_out):
+    print('jfunc')
+    print(f'check {val_in:0{size_hex(size)}X}')
     size = np.uint8(size)
     iter = {8: np.uint8, 16: np.uint16, 32: np.uint32, 64: np.uint64}
     for bits, dtype in iter.items():
         if size <= bits:
             break
     val_in = dtype(val_in)
-    print(val_in, val_in.dtype, size, size.dtype)
+    print('C', val_in, val_in.dtype, size, size.dtype)
     assert jfunc(val_in, size) == val_out
 
 
 @pytest.mark.parametrize('size, val_in, val_out', tests)
 def test_vectorize(size, val_in, val_out):
-    size = np.uint8(size)
+    print('ufunc')
+    print(f'check {val_in:0{size_hex(size)}X}')
     data = np.array(
         [val_in] * TEST_ARRAY_SIZE, dtype=f'uint{bits_to_wordsize(size)}'
     )
     expected = [val_out] * TEST_ARRAY_SIZE
     assert all([a == b for a, b in zip_longest(ufunc(data, size), expected)])
```

### Comparing `typeconvert-0.1.3/tests/test_ti32.py` & `typeconvert-0.1.4/tests/test_ti32.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_ti40.py` & `typeconvert-0.1.4/tests/test_ti40.py`

 * *Files identical despite different names*

### Comparing `typeconvert-0.1.3/tests/test_twoscomp.py` & `typeconvert-0.1.4/tests/test_onescomp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,97 @@
 import pytest
 import numpy as np
 from itertools import zip_longest
 from typeconvert.utils import bits_to_wordsize, mask
-from typeconvert.types.twoscomp import func, jfunc, ufunc
+from typeconvert.types.onescomp import func, jfunc, ufunc
 
 TEST_ARRAY_SIZE = 100
 TEST_CASES = {
     3: [
         (0b000,  0),
         (0b001,  1),
         (0b010,  2),
         (0b011,  3),
-        (0b100, -4),
-        (0b101, -3),
-        (0b110, -2),
-        (0b111, -1),
+        (0b100, -3),
+        (0b101, -2),
+        (0b110, -1),
+        (0b111, -0),
     ],
     8: [
         (0b00000000,    0),
         (0b00000001,    1),
         (0b00000010,    2),
         (0b01111110,  126),
         (0b01111111,  127),
-        (0b10000000, -128),
-        (0b10000001, -127),
-        (0b10000010, -126),
-        (0b11111110,   -2),
-        (0b11111111,   -1),
+        (0b10000000, -127),
+        (0b10000001, -126),
+        (0b10000010, -125),
+        (0b11111110,   -1),
+        (0b11111111,   -0),
     ],
     16: [
         (0x0000,  0),
-        (0xFFFF, -1),
+        (0x7FFF, 2**15-1),
+        (0x8000, -2**15+1),
+        (0xFFFF, 0),
     ],
     24: [
         (0x000000,  0),
-        (0xFFFFFF, -1),
+        (0x7FFFFF, 2**23-1),
+        (0x800000, -2**23+1),
+        (0xFFFFFF, 0),
     ],
     32: [
         (0x00000000,  0),
-        (0xFFFFFFFF, -1),
+        (0x7FFFFFFF, 2**31-1),
+        (0x80000000, -2**31+1),
+        (0xFFFFFFFF, 0),
     ],
     48: [
         (0x000000000000,  0),
-        (0xFFFFFFFFFFFF, -1),
+        (0x7FFFFFFFFFFF, 2**47-1),
+        (0x800000000000, -2**47+1),
+        (0xFFFFFFFFFFFF, 0),
     ],
     64: [
         (0x0000000000000000,  0),
-        (0xFFFFFFFFFFFFFFFF, -1),
+        (0x7FFFFFFFFFFFFFFF, 2**63-1),
+        (0x8000000000000000, -2**63+1),
+        (0xFFFFFFFFFFFFFFFF, 0),
     ],
 }
 
 tests = []
 for size in TEST_CASES:
     for val_in, val_out in TEST_CASES[size]:
         tests.append((size, val_in, val_out))
 tests += [(size, 0, 0) for size in np.arange(64)+1]
-tests += [(size, mask(size), -1) for size in np.arange(64)+1]
+tests += [(size, mask(size), -0) for size in np.arange(64)+1]
 
 
 @pytest.mark.parametrize('size, val_in, val_out', tests)
 def test_func(size, val_in, val_out):
-    print('func')
+    print('zzz', val_in, size, val_out)
+    size = np.uint8(size)
     assert func(val_in, size) == val_out
 
 
 @pytest.mark.parametrize('size, val_in, val_out', tests)
 def test_njit(size, val_in, val_out):
-    print('jfunc')
     size = np.uint8(size)
     iter = {8: np.uint8, 16: np.uint16, 32: np.uint32, 64: np.uint64}
     for bits, dtype in iter.items():
         if size <= bits:
             break
     val_in = dtype(val_in)
-    print('C', val_in, val_in.dtype, size, size.dtype)
+    print(val_in, val_in.dtype, size, size.dtype)
     assert jfunc(val_in, size) == val_out
 
 
 @pytest.mark.parametrize('size, val_in, val_out', tests)
 def test_vectorize(size, val_in, val_out):
-    print('ufunc')
+    size = np.uint8(size)
     data = np.array(
         [val_in] * TEST_ARRAY_SIZE, dtype=f'uint{bits_to_wordsize(size)}'
     )
     expected = [val_out] * TEST_ARRAY_SIZE
     assert all([a == b for a, b in zip_longest(ufunc(data, size), expected)])
```

