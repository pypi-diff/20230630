# Comparing `tmp/pyms-nist-search-0.5.0b3.tar.gz` & `tmp/pyms-nist-search-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyms-nist-search-0.5.0b3.tar", last modified: Thu Jun  9 16:48:25 2022, max compression
+gzip compressed data, was "pyms-nist-search-0.6.0.tar", last modified: Fri Jun 30 11:13:43 2023, max compression
```

## Comparing `pyms-nist-search-0.5.0b3.tar` & `pyms-nist-search-0.6.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.386124 pyms-nist-search-0.5.0b3/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8031 2022-06-09 16:48:25.386124 pyms-nist-search-0.5.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6206 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/THIRD_PARTY_COPYRIGHT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.378124 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8031 2022-06-09 16:48:24.000000 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-06-09 16:48:25.000000 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 16:48:24.000000 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 16:48:24.000000 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-06-09 16:48:25.000000 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 16:48:25.000000 pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5803 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-06-09 16:48:25.386124 pyms-nist-search-0.5.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.378124 pyms-nist-search-0.5.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.382124 pyms-nist-search-0.5.0b3/src/pyms_nist_search/
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/NISTERR.H
--rw-r--r--   0 runner    (1001) docker     (121)    36562 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/NISTMS.H
--rw-r--r--   0 runner    (1001) docker     (121)    20892 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/NISTMS_min.H
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4023 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9684 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/docker_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/mona_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    63776 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/pyms_nist_search.c
--rw-r--r--   0 runner    (1001) docker     (121)    20454 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/pyms_nist_search_min.c
--rw-r--r--   0 runner    (1001) docker     (121)     9652 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/reference_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/search_result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.382124 pyms-nist-search-0.5.0b3/src/pyms_nist_search/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/templates/msp_template
--rw-r--r--   0 runner    (1001) docker     (121)     3359 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5702 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/win_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.382124 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/
--rw-r--r--   0 runner    (1001) docker     (121)   226304 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/ctnt66_64.dll
--rw-r--r--   0 runner    (1001) docker     (121)   761344 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64.dll
--rw-r--r--   0 runner    (1001) docker     (121)     5250 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64.lib
--rw-r--r--   0 runner    (1001) docker     (121)   761856 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64_2gb.dll
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64_2gb.lib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 16:48:25.386124 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/
--rw-r--r--   0 runner    (1001) docker     (121)   187904 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/ctnt66.dll
--rw-r--r--   0 runner    (1001) docker     (121)   634368 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32.dll
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32.lib
--rw-r--r--   0 runner    (1001) docker     (121)   634880 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32_2gb.dll
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-06-09 16:47:47.000000 pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32_2gb.lib
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.547583 pyms-nist-search-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-30 11:12:51.000000 pyms-nist-search-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-30 11:12:51.000000 pyms-nist-search-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8080 2023-06-30 11:13:43.547583 pyms-nist-search-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6206 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/THIRD_PARTY_COPYRIGHT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.539583 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8080 2023-06-30 11:13:42.000000 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-06-30 11:13:43.000000 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 11:13:42.000000 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 11:13:42.000000 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-30 11:13:43.000000 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-30 11:13:43.000000 pyms-nist-search-0.6.0/pyms_nist_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-06-30 11:13:43.547583 pyms-nist-search-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2370 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.535583 pyms-nist-search-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.539583 pyms-nist-search-0.6.0/src/pyms_nist_search/
+-rw-r--r--   0 runner    (1001) docker     (122)     3162 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/NISTERR.H
+-rw-r--r--   0 runner    (1001) docker     (122)    36562 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/NISTMS.H
+-rw-r--r--   0 runner    (1001) docker     (122)    20892 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/NISTMS_min.H
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4172 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10388 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/docker_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6226 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/mona_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    63776 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/pyms_nist_search.c
+-rw-r--r--   0 runner    (1001) docker     (122)    20454 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/pyms_nist_search_min.c
+-rw-r--r--   0 runner    (1001) docker     (122)     9819 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/reference_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/search_result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.539583 pyms-nist-search-0.6.0/src/pyms_nist_search/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/templates/msp_template
+-rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5805 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/win_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.543583 pyms-nist-search-0.6.0/src/pyms_nist_search/x64/
+-rw-r--r--   0 runner    (1001) docker     (122)   226304 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x64/ctnt66_64.dll
+-rw-r--r--   0 runner    (1001) docker     (122)   761344 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5250 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64.lib
+-rw-r--r--   0 runner    (1001) docker     (122)   761856 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64_2gb.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64_2gb.lib
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:13:43.547583 pyms-nist-search-0.6.0/src/pyms_nist_search/x86/
+-rw-r--r--   0 runner    (1001) docker     (122)   187904 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x86/ctnt66.dll
+-rw-r--r--   0 runner    (1001) docker     (122)   634368 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32.lib
+-rw-r--r--   0 runner    (1001) docker     (122)   634880 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32_2gb.dll
+-rw-r--r--   0 runner    (1001) docker     (122)     5616 2023-06-30 11:12:52.000000 pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32_2gb.lib
```

### Comparing `pyms-nist-search-0.5.0b3/LICENSE` & `pyms-nist-search-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/MANIFEST.in` & `pyms-nist-search-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/PKG-INFO` & `pyms-nist-search-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyms-nist-search
-Version: 0.5.0b3
+Version: 0.6.0
 Summary: PyMassSpec extension for searching mass spectra using NIST's Mass Spectrum Search Engine.
 Home-page: https://github.com/domdfcoding/pynist
 Author: Dominic Davis-Foster
 Author-email: dominic@davis-foster.co.uk
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Project-URL: Documentation, https://pynist.readthedocs.io/en/latest
 Project-URL: Issue Tracker, https://github.com/domdfcoding/pynist/issues
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -89,16 +90,16 @@
 	:target: https://github.com/domdfcoding/pynist/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/pynist/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/pynist/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/pynist/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/pynist/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/pynist/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/pynist/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/pynist/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/pynist?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/pynist?logo=codefactor
@@ -124,23 +125,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pynist
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.5.0b3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.0
 	:target: https://github.com/domdfcoding/pynist/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyms-nist-search
 	:target: https://pypi.org/project/pyms-nist-search/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pyms-nist-search-0.5.0b3/README.rst` & `pyms-nist-search-0.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 	:target: https://github.com/domdfcoding/pynist/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/pynist/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/pynist/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/pynist/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/pynist/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/pynist/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/pynist/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/pynist/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/pynist?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/pynist?logo=codefactor
@@ -86,23 +86,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pynist
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.5.0b3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.0
 	:target: https://github.com/domdfcoding/pynist/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyms-nist-search
 	:target: https://pypi.org/project/pyms-nist-search/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/PKG-INFO` & `pyms-nist-search-0.6.0/pyms_nist_search.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyms-nist-search
-Version: 0.5.0b3
+Version: 0.6.0
 Summary: PyMassSpec extension for searching mass spectra using NIST's Mass Spectrum Search Engine.
 Home-page: https://github.com/domdfcoding/pynist
 Author: Dominic Davis-Foster
 Author-email: dominic@davis-foster.co.uk
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Project-URL: Documentation, https://pynist.readthedocs.io/en/latest
 Project-URL: Issue Tracker, https://github.com/domdfcoding/pynist/issues
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -89,16 +90,16 @@
 	:target: https://github.com/domdfcoding/pynist/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/pynist/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/pynist/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/pynist/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/pynist/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/pynist/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/pynist/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/pynist/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/pynist?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/pynist?logo=codefactor
@@ -124,23 +125,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pynist
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.5.0b3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pynist/v0.6.0
 	:target: https://github.com/domdfcoding/pynist/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pynist
 	:target: https://github.com/domdfcoding/pynist/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pyms-nist-search
 	:target: https://pypi.org/project/pyms-nist-search/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `pyms-nist-search-0.5.0b3/pyms_nist_search.egg-info/SOURCES.txt` & `pyms-nist-search-0.6.0/pyms_nist_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/pyproject.toml` & `pyms-nist-search-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,<61,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyms-nist-search"
-version = "0.5.0b3"
+version = "0.6.0"
 description = "PyMassSpec extension for searching mass spectra using NIST's Mass Spectrum Search Engine."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -23,14 +23,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 dynamic = [ "dependencies",]
 
@@ -57,15 +58,15 @@
     "Operating System :: Microsoft :: Windows :: Windows 8.1",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Programming Language :: C",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython",]
 platforms = [ "Windows", "Linux",]
 license-key = "LGPL-3.0-or-later"
 package = "pyms_nist_search"
 additional-files = [
     "include THIRD_PARTY_COPYRIGHT",
     "recursive-include src/pyms_nist_search *",
```

### Comparing `pyms-nist-search-0.5.0b3/requirements.txt` & `pyms-nist-search-0.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/setup.cfg` & `pyms-nist-search-0.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyms-nist-search
-version = 0.5.0b3
+version = 0.6.0
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = GNU Lesser General Public License v3 or later (LGPLv3+)
 keywords = 
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, Linux
@@ -27,14 +27,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Chemistry
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 
 [options]
 python_requires = >=3.6.1
```

### Comparing `pyms-nist-search-0.5.0b3/setup.py` & `pyms-nist-search-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/NISTERR.H` & `pyms-nist-search-0.6.0/src/pyms_nist_search/NISTERR.H`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/NISTMS.H` & `pyms-nist-search-0.6.0/src/pyms_nist_search/NISTMS.H`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/NISTMS_min.H` & `pyms-nist-search-0.6.0/src/pyms_nist_search/NISTMS_min.H`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/__init__.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,11 +69,11 @@
 	# this package
 	from pyms_nist_search.docker_engine import Engine  # noqa: F401
 
 name: str = "PyMassSpec NIST Search"
 __author__: str = "Dominic Davis-Foster"
 __license__: str = "LGPLv3+"
 __maintainer_email__: str = "dominic@davis-foster.co.uk"
-__version__: str = "0.5.0b3"
+__version__: str = "0.6.0"
 
 __copyright__: str = "2020 Dominic Davis-Foster"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/base.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,20 +109,32 @@
 		Construct an object from a dictionary.
 
 		:param dictionary:
 		"""
 
 		return cls(**dictionary)
 
+	def to_dict(self) -> Dict[str, Any]:
+		"""
+		Convert the object to a dictionary.
+
+		.. versionadded:: 0.6.0
+		"""
+
+		return dict(
+				name=self._name,
+				cas=self.cas,
+				)
+
 	def to_json(self) -> str:
 		"""
 		Convert the object to json.
 		"""
 
-		return sdjson.dumps(dict(self))
+		return sdjson.dumps(self.to_dict())
 
 	@classmethod
 	def from_pynist(cls, pynist_dict: Dict[str, Any]):
 		"""
 		Create an object from the raw data returned by the C extension.
 
 		:param pynist_dict:
@@ -131,34 +143,31 @@
 		return cls(
 				name=parse_name_chars(pynist_dict["hit_name_chars"]),
 				cas=cas_int_to_string(pynist_dict["cas_no"]),
 				)
 
 	@property
 	def __dict__(self):
-		return dict(
-				name=self._name,
-				cas=self.cas,
-				)
+		return self.to_dict()
 
 	def __getstate__(self) -> Dict[str, Any]:
-		return self.__dict__
+		return self.to_dict()
 
 	def __setstate__(self, state):
 		self.__init__(**state)  # type: ignore
 
 	def __iter__(self):
-		yield from self.__dict__.items()
+		yield from self.to_dict().items()
 
 	def __str__(self) -> str:
 		return self.__repr__()
 
 	def __eq__(self, other) -> bool:
 		if isinstance(other, self.__class__):
-			return self.__dict__ == other.__dict__
+			return self.to_dict() == other.to_dict()
 
 		return NotImplemented
 
 
 @sdjson.register_encoder(int64)
 @sdjson.register_encoder(int32)
 @sdjson.register_encoder(signedinteger)
```

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/docker_engine.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/docker_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,22 +89,36 @@
 
 class Engine:
 	"""
 	Search engine for Linux and other platforms supporting Docker.
 
 	The first time the engine is initialized it will download the latest
 	version of the docker image automatically.
-
-	This can also be done manually, such as to upgrade to the latest version,
+	This can also be performed manually, such as to upgrade to the latest version,
 	with the following command:
 
 	.. prompt:: bash
 
 		docker pull domdfcoding/pywine-pyms-nist
 
+	The engine must be uninitialized when no longer required to shut down the underlying docker container.
+	This is achieved with the :meth:`uninit() <pyms_nist_search.docker_engine.Engine.uninit>` method.
+	Alternatively, this class can be used as a contextmanager to automatically uninitialize the engine
+	upon leaving the :keyword:`with` block:
+
+	.. code-block:: python3
+
+		with pyms_nist_search.Engine(
+				FULL_PATH_TO_MAIN_LIBRARY,
+				pyms_nist_search.NISTMS_MAIN_LIB,
+				FULL_PATH_TO_WORK_DIR,
+				) as search:
+			search.full_spectrum_search(ms, n_hits=5)
+
+	.. versionchanged:: 0.6.0  Added context manager support.
 	"""
 
 	initialised: bool
 
 	def __init__(
 			self,
 			lib_path: PathLike,
@@ -173,14 +187,20 @@
 				# stdout=False,
 				# stderr=False,
 				stdin_open=False,
 				volumes={lib_path: {"bind": "/mainlib", "mode": "ro"}},
 				environment=[f"LIBTYPE={lib_type}"],
 				)
 
+	def __enter__(self):
+		return self
+
+	def __exit__(self, exc_type, exc_val, exc_tb):
+		self.uninit()
+
 	def uninit(self) -> None:
 		"""
 		Uninitialize the Search Engine.
 		"""
 
 		if self.initialised:
 
@@ -272,16 +292,16 @@
 			) -> List[Tuple[SearchResult, ReferenceData]]:
 		"""
 		Perform a Full Spectrum Search of the mass spectral library, including reference data.
 
 		:param mass_spec: The mass spectrum to search against the library.
 		:param n_hits: The number of hits to return.
 
-		:return: List of tuples consisting of the possible identities
-			for the mass spectrum and the reference data from the library.
+		:return: List of tuples containing possible identities
+			for the mass spectrum, and the reference data.
 		"""
 
 		if not isinstance(mass_spec, MassSpectrum):
 			raise TypeError("`mass_spec` must be a pyms.Spectrum.MassSpectrum object.")
 
 		retry_count = 0
```

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/mona_tools.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/mona_tools.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/pyms_nist_search.c` & `pyms-nist-search-0.6.0/src/pyms_nist_search/pyms_nist_search.c`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/pyms_nist_search_min.c` & `pyms-nist-search-0.6.0/src/pyms_nist_search/pyms_nist_search_min.c`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/reference_data.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/reference_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
 	:param nist_no:
 	:param id:
 	:param mw:
 	:param formula: The formula of the compound.
 	:param contributor: The contributor to the library.
 	:param mass_spec: The reference mass spectrum.
 	:param synonyms: List of synonyms for the compound.
+
+	.. latex:vspace:: 60px
 	"""
 
 	_exact_mass: float
 	_mass_spec: MassSpectrum
 	_synonyms: List[str]
 
 	def __init__(
@@ -202,29 +204,38 @@
 				mass_spec=MassSpectrum(pynist_dict["mass_list"], pynist_dict["intensity_list"]),
 				synonyms=[parse_name_chars(synonym) for synonym in pynist_dict["synonyms_chars"]],
 				)
 
 	def __repr__(self) -> str:
 		return f"Reference Data: {self.name} \t({self.cas})"
 
-	@property
-	def __dict__(self):
+	def to_dict(self) -> Dict[str, Any]:
+		"""
+		Convert the object to a dictionary.
+
+		.. versionadded:: 0.6.0
+		"""
+
 		return dict(
 				name=self.name,
 				cas=self.cas,
 				formula=self.formula,
 				contributor=self.contributor,
 				nist_no=self.nist_no,
 				id=self.id,
 				mw=self.mw,
 				exact_mass=self.exact_mass,
 				synonyms=self.synonyms[:],
 				mass_spec=self.mass_spec,
 				)
 
+	@property
+	def __dict__(self):
+		return self.to_dict()
+
 	@classmethod
 	def from_jcamp(cls, file_name: PathLike, ignore_warnings: bool = True) -> "ReferenceData":
 		"""
 		Create a ReferenceData object from a JCAMP-DX file.
 
 		:param file_name: Path of the file to read.
 		:param ignore_warnings: Whether warnings about invalid tags should be shown.
@@ -287,15 +298,15 @@
 					)
 
 	def to_json(self) -> str:
 		"""
 		Convert the object to JSON.
 		"""
 
-		return sdjson.dumps(self.__dict__)
+		return sdjson.dumps(self.to_dict())
 
 	@classmethod
 	def from_json(cls, json_data: str):
 		"""
 		Construct an object from JSON data.
 
 		:param json_data:
```

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/search_result.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/search_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
 	:param name: The name of the compound
 	:param cas: The CAS number of the compound
 	:param match_factor:
 	:param reverse_match_factor:
 	:param hit_prob:
 	:param spec_loc: The location of the reference spectrum in the library.
+
+	.. latex:vspace:: 20px
 	"""
 
 	def __init__(
 			self,
 			name: str = '',
 			cas: Union[str, int] = "---",
 			match_factor: float = 0,
@@ -131,22 +133,31 @@
 				hit_prob=pynist_dict["hit_prob"] / 100,
 				spec_loc=pynist_dict["spec_loc"],
 				)
 
 	def __repr__(self) -> str:
 		return f"Search Result: {self.name} \t({self.match_factor})"
 
-	@property
-	def __dict__(self):
+	def to_dict(self) -> Dict[str, Any]:
+		"""
+		Convert the object to a dictionary.
+
+		.. versionadded:: 0.6.0
+		"""
+
 		return dict(
 				name=self._name,
 				cas=self.cas,
 				match_factor=self.match_factor,
 				reverse_match_factor=self.reverse_match_factor,
 				spec_loc=self.spec_loc,
 				hit_prob=self.hit_prob,
 				)
 
+	@property
+	def __dict__(self):
+		return self.to_dict()
+
 
 @register_encoder(SearchResult)
 def encode_search_result(obj: SearchResult) -> Dict[str, Any]:
 	return dict(obj)
```

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/templates/__init__.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/utils.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/utils.py`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/win_engine.py` & `pyms-nist-search-0.6.0/src/pyms_nist_search/win_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 
 		Search by Name. See page 13 of the documentation.
 		Would also like to search by CAS number but DLL doesn't seem to support that.
 
 	:param lib_path: The path to the mass spectral library.
 	:param lib_type: The type of library. One of ``NISTMS_MAIN_LIB``, ``NISTMS_USER_LIB``, ``NISTMS_REP_LIB``.
 	:param work_dir: The path to the working directory.
+
+	.. latex:vspace:: 50px
 	"""
 
 	def __init__(
 			self,
 			lib_path: PathLike,
 			lib_type: int = _core.NISTMS_MAIN_LIB,
 			work_dir: Optional[PathLike] = None,
@@ -147,16 +149,16 @@
 			) -> List[Tuple[SearchResult, ReferenceData]]:
 		"""
 		Perform a Full Spectrum Search of the mass spectral library, including reference data.
 
 		:param mass_spec: The mass spectrum to search against the library.
 		:param n_hits: The number of hits to return.
 
-		:return: List of tuples consisting of the possible identities for the
-			mass spectrum and the reference data from the library.
+		:return: List of tuples containing possible identities
+			for the mass spectrum, and the reference data
 		"""
 
 		if not isinstance(mass_spec, MassSpectrum):
 			raise TypeError("`mass_spec` must be a pyms.Spectrum.MassSpectrum object.")
 
 		hit_list = self.full_spectrum_search(mass_spec, n_hits)
 
@@ -175,7 +177,13 @@
 
 		:param spec_loc:
 		"""
 
 		reference_data = _core._get_reference_data(spec_loc)
 
 		return ReferenceData.from_pynist(reference_data)
+
+	def __enter__(self):
+		return self
+
+	def __exit__(self, exc_type, exc_val, exc_tb):
+		self.uninit()
```

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/ctnt66_64.dll` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x64/ctnt66_64.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64.dll` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64.lib` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64.lib`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64_2gb.dll` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64_2gb.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x64/nistdl64_2gb.lib` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x64/nistdl64_2gb.lib`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/ctnt66.dll` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x86/ctnt66.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32.dll` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32.lib` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32.lib`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32_2gb.dll` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32_2gb.dll`

 * *Files identical despite different names*

### Comparing `pyms-nist-search-0.5.0b3/src/pyms_nist_search/x86/nistdl32_2gb.lib` & `pyms-nist-search-0.6.0/src/pyms_nist_search/x86/nistdl32_2gb.lib`

 * *Files identical despite different names*

