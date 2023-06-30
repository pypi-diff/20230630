# Comparing `tmp/cachier-2.1.1.tar.gz` & `tmp/cachier-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachier-2.1.1.tar", last modified: Sun Apr  9 05:18:54 2023, max compression
+gzip compressed data, was "cachier-2.2.0.tar", last modified: Fri Jun 30 13:52:05 2023, max compression
```

## Comparing `cachier-2.1.1.tar` & `cachier-2.2.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.179899 cachier-2.1.1/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      447 2021-06-17 12:08:06.000000 cachier-2.1.1/.codecov.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      394 2023-04-09 05:18:24.000000 cachier-2.1.1/.coveragerc
--rw-r--r--   0 shaypalachy   (501) staff       (20)      195 2021-06-17 12:08:06.000000 cachier-2.1.1/.deepsource.toml
--rw-r--r--   0 shaypalachy   (501) staff       (20)       30 2021-10-10 23:14:34.000000 cachier-2.1.1/.fdignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)      202 2022-12-02 11:10:23.000000 cachier-2.1.1/.flake8
--rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2021-06-17 12:08:06.000000 cachier-2.1.1/.gitattributes
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.158541 cachier-2.1.1/.github/
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.170232 cachier-2.1.1/.github/workflows/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      680 2023-03-16 11:40:57.000000 cachier-2.1.1/.github/workflows/checkdocs.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      746 2023-03-16 11:40:57.000000 cachier-2.1.1/.github/workflows/lint.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      982 2023-03-22 22:40:25.000000 cachier-2.1.1/.github/workflows/test.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1249 2021-06-17 12:08:06.000000 cachier-2.1.1/.gitignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2022-12-02 11:08:24.000000 cachier-2.1.1/.ignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8489 2021-10-10 23:14:34.000000 cachier-2.1.1/.pylintrc
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1069 2021-06-17 12:08:06.000000 cachier-2.1.1/LICENSE
--rw-r--r--   0 shaypalachy   (501) staff       (20)       50 2021-06-17 12:08:06.000000 cachier-2.1.1/MANIFEST.in
--rw-r--r--   0 shaypalachy   (501) staff       (20)    17286 2023-04-09 05:18:54.180055 cachier-2.1.1/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)    16242 2023-04-09 05:18:24.000000 cachier-2.1.1/README.rst
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.180849 cachier-2.1.1/cachier/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      232 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      471 2023-04-09 05:18:54.180904 cachier-2.1.1/cachier/_version.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     3062 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/base_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    13492 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2846 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/memory_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     5022 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/mongo_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    10068 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/pickle_core.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.173958 cachier-2.1.1/cachier/scripts/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.1.1/cachier/scripts/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      429 2021-06-17 12:08:06.000000 cachier-2.1.1/cachier/scripts/cli.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.173587 cachier-2.1.1/cachier.egg-info/
--rw-r--r--   0 shaypalachy   (501) staff       (20)    17286 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)      906 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/SOURCES.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/dependency_links.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)       71 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/entry_points.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      185 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/requires.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/top_level.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      308 2023-04-09 05:18:24.000000 cachier-2.1.1/pytest.ini
--rw-r--r--   0 shaypalachy   (501) staff       (20)      269 2023-04-09 05:18:54.180603 cachier-2.1.1/setup.cfg
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2531 2023-03-23 18:10:50.000000 cachier-2.1.1/setup.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.179375 cachier-2.1.1/tests/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.1.1/tests/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1903 2023-03-22 22:40:25.000000 cachier-2.1.1/tests/speed_eval.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      168 2023-03-31 07:33:42.000000 cachier-2.1.1/tests/standalone_script.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1100 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_core_lookup.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     5766 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_defaults.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     6703 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_general.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8879 2023-03-31 07:33:42.000000 cachier-2.1.1/tests/test_memory_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8965 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_mongo_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    18208 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_pickle_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      482 2023-03-22 22:40:25.000000 cachier-2.1.1/tests/test_quality.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      577 2023-03-22 22:40:25.000000 cachier-2.1.1/tests/test_security.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    65747 2021-06-17 12:08:06.000000 cachier-2.1.1/versioneer.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.519251 cachier-2.2.0/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      447 2021-06-17 12:08:06.000000 cachier-2.2.0/.codecov.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      394 2023-04-09 05:18:24.000000 cachier-2.2.0/.coveragerc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      195 2021-06-17 12:08:06.000000 cachier-2.2.0/.deepsource.toml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       30 2021-10-10 23:14:34.000000 cachier-2.2.0/.fdignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      202 2022-12-02 11:10:23.000000 cachier-2.2.0/.flake8
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2021-06-17 12:08:06.000000 cachier-2.2.0/.gitattributes
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.491686 cachier-2.2.0/.github/
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.507514 cachier-2.2.0/.github/workflows/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      680 2023-03-16 11:40:57.000000 cachier-2.2.0/.github/workflows/checkdocs.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      775 2023-06-30 12:48:49.000000 cachier-2.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      981 2023-06-30 12:48:49.000000 cachier-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1249 2021-06-17 12:08:06.000000 cachier-2.2.0/.gitignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2022-12-02 11:08:24.000000 cachier-2.2.0/.ignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8489 2021-10-10 23:14:34.000000 cachier-2.2.0/.pylintrc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1069 2021-06-17 12:08:06.000000 cachier-2.2.0/LICENSE
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       50 2021-06-17 12:08:06.000000 cachier-2.2.0/MANIFEST.in
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    17490 2023-06-30 13:52:05.519438 cachier-2.2.0/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    16447 2023-06-30 12:49:12.000000 cachier-2.2.0/README.rst
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.520260 cachier-2.2.0/cachier/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      232 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      471 2023-06-30 13:52:05.520316 cachier-2.2.0/cachier/_version.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     3062 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/base_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    14505 2023-06-30 12:49:12.000000 cachier-2.2.0/cachier/core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2846 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/memory_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     5022 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/mongo_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    10068 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/pickle_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2023-06-30 12:48:49.000000 cachier-2.2.0/cachier/py.typed
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.513238 cachier-2.2.0/cachier/scripts/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.2.0/cachier/scripts/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      429 2021-06-17 12:08:06.000000 cachier-2.2.0/cachier/scripts/cli.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.512829 cachier-2.2.0/cachier.egg-info/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    17490 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      932 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/SOURCES.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/dependency_links.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       52 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/entry_points.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      220 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/requires.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/top_level.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      227 2023-06-30 12:48:49.000000 cachier-2.2.0/mypy.ini
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      308 2023-04-09 05:18:24.000000 cachier-2.2.0/pytest.ini
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      269 2023-06-30 13:52:05.519994 cachier-2.2.0/setup.cfg
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2615 2023-06-30 12:48:49.000000 cachier-2.2.0/setup.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.518782 cachier-2.2.0/tests/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.2.0/tests/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1903 2023-03-22 22:40:25.000000 cachier-2.2.0/tests/speed_eval.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      168 2023-03-31 07:33:42.000000 cachier-2.2.0/tests/standalone_script.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1122 2023-06-30 12:49:12.000000 cachier-2.2.0/tests/test_core_lookup.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     6545 2023-06-30 12:49:12.000000 cachier-2.2.0/tests/test_defaults.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     7272 2023-06-30 12:49:12.000000 cachier-2.2.0/tests/test_general.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8879 2023-03-31 07:33:42.000000 cachier-2.2.0/tests/test_memory_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8963 2023-06-30 12:48:49.000000 cachier-2.2.0/tests/test_mongo_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    18211 2023-06-30 12:48:49.000000 cachier-2.2.0/tests/test_pickle_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      482 2023-03-22 22:40:25.000000 cachier-2.2.0/tests/test_quality.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      577 2023-03-22 22:40:25.000000 cachier-2.2.0/tests/test_security.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    65788 2023-06-30 12:48:49.000000 cachier-2.2.0/versioneer.py
```

### Comparing `cachier-2.1.1/.github/workflows/checkdocs.yml` & `cachier-2.2.0/.github/workflows/checkdocs.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/.github/workflows/lint.yml` & `cachier-2.2.0/.github/workflows/lint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,31 @@
   build:
     runs-on: ${{ matrix.os }}
     environment:
       name: test
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.10']
+        python-version: ["3.10"]
         os: [ubuntu-latest]
 
     steps:
       - name: Check out Git repository
         uses: actions/checkout@v3.4.0
 
       - name: set up python '3.10'
         uses: actions/setup-python@v4.5.0
         with:
-          python-version: '3.10'
+          python-version: "3.10"
 
       # Install your linters here
-      - name: Install flake8
+      - name: Install linters
         run: |
-          python -m pip install flake8
+          python -m pip install -e ".[test]"
+
       - name: Run linters
         uses: wearerequired/lint-action@v2.3.0
         with:
           flake8: true
+          mypy: true
           continue_on_error: false
           # Enable your linters here
```

### Comparing `cachier-2.1.1/.github/workflows/test.yml` & `cachier-2.2.0/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   build:
     runs-on: ${{ matrix.os }}
     environment:
       name: test
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.8, 3.9, '3.10', '3.11']
         os: [ubuntu-latest, macOS-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3.4.0
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4.5.0
@@ -31,10 +31,10 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e ".[test]"
       - name: Unit tests
         run: |
           pytest
       - name: "Upload coverage to Codecov"
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
```

### Comparing `cachier-2.1.1/.gitignore` & `cachier-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/.pylintrc` & `cachier-2.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/LICENSE` & `cachier-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/PKG-INFO` & `cachier-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cachier
-Version: 2.1.1
+Version: 2.2.0
 Summary: Persistent, stale-free, local and cross-machine caching for Python functions.
 Home-page: https://github.com/python-cachier/cachier
 Author: Shay Palachy
 Author-email: shay.palachy@gmail.com
 License: MIT
 Keywords: cache,persistence,mongo,memoization,decorator
 Platform: linux
 Platform: osx
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Intended Audience :: Developers
 Provides-Extra: test
 License-File: LICENSE
@@ -68,15 +68,15 @@
 
     pip install 'cachier==1.2.8'
 
 Features
 ========
 
 * Pure Python.
-* Compatible with Python 3.5+ (and Python 2.7 up until version 1.2.8).
+* Compatible with Python 3.8+ (Python 2.7 was discontinued in version 1.2.8).
 * Supported and `tested on Linux, OS X and Windows <https://travis-ci.org/shaypal5/cachier>`_.
 * A simple interface.
 * Defining "shelf life" for cached values.
 * Local caching using pickle files.
 * Cross-machine caching using MongoDB.
 * Thread-safety.
 
@@ -163,14 +163,15 @@
 *  `mongetter`
 *  `cache_dir`
 *  `pickle_reload`
 *  `separate_files`
 
 These parameters can be changed at any time and they will apply to all decorators:
 
+*  `allow_none`
 *  `caching_enabled`
 *  `stale_after`
 *  `next_time`
 *  `wait_for_calc_timeout`
 
 The current defaults can be fetched by calling `get_default_params`.
 
@@ -280,14 +281,18 @@
 You can have ``cachier`` overwrite an existing cache entry - if one exists - for a specific function call by passing ``overwrite_cache=True`` to the function call. The cache will not be checked but will be updated with the new return value.
 
 Verbose Cache Call
 ~~~~~~~~~~~~~~~~~~
 
 You can have ``cachier`` print out a detailed explanation of the logic of a specific call by passing ``verbose_cache=True`` to the function call. This can be useful if you are not sure why a certain function result is, or is not, returned.
 
+Cache `None` Values
+~~~~~~~~~~~~~~~~~~~
+
+By default, ``cachier`` does not cache ``None`` values. You can override this behaviour by passing ``allow_none=True`` to the function call.
 
 
 Cachier Cores
 =============
 
 Pickle Core
 -----------
@@ -488,9 +493,7 @@
 .. |Codefactor| image:: https://www.codefactor.io/repository/github/python-cachier/cachier/badge?style=plastic
      :target: https://www.codefactor.io/repository/github/python-cachier/cachier
      :alt: Codefactor code quality
 
 .. links:
 .. _pymongo: https://api.mongodb.com/python/current/
 .. _watchdog: https://github.com/gorakhargosh/watchdog
-
-
```

### Comparing `cachier-2.1.1/README.rst` & `cachier-2.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     pip install 'cachier==1.2.8'
 
 Features
 ========
 
 * Pure Python.
-* Compatible with Python 3.5+ (and Python 2.7 up until version 1.2.8).
+* Compatible with Python 3.8+ (Python 2.7 was discontinued in version 1.2.8).
 * Supported and `tested on Linux, OS X and Windows <https://travis-ci.org/shaypal5/cachier>`_.
 * A simple interface.
 * Defining "shelf life" for cached values.
 * Local caching using pickle files.
 * Cross-machine caching using MongoDB.
 * Thread-safety.
 
@@ -135,14 +135,15 @@
 *  `mongetter`
 *  `cache_dir`
 *  `pickle_reload`
 *  `separate_files`
 
 These parameters can be changed at any time and they will apply to all decorators:
 
+*  `allow_none`
 *  `caching_enabled`
 *  `stale_after`
 *  `next_time`
 *  `wait_for_calc_timeout`
 
 The current defaults can be fetched by calling `get_default_params`.
 
@@ -252,14 +253,18 @@
 You can have ``cachier`` overwrite an existing cache entry - if one exists - for a specific function call by passing ``overwrite_cache=True`` to the function call. The cache will not be checked but will be updated with the new return value.
 
 Verbose Cache Call
 ~~~~~~~~~~~~~~~~~~
 
 You can have ``cachier`` print out a detailed explanation of the logic of a specific call by passing ``verbose_cache=True`` to the function call. This can be useful if you are not sure why a certain function result is, or is not, returned.
 
+Cache `None` Values
+~~~~~~~~~~~~~~~~~~~
+
+By default, ``cachier`` does not cache ``None`` values. You can override this behaviour by passing ``allow_none=True`` to the function call.
 
 
 Cachier Cores
 =============
 
 Pickle Core
 -----------
```

### Comparing `cachier-2.1.1/cachier/base_core.py` & `cachier-2.2.0/cachier/base_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/cachier/core.py` & `cachier-2.2.0/cachier/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,32 @@
 # https://github.com/python-cachier/cachier
 
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/MIT-license
 # Copyright (c) 2016, Shay Palachy <shaypal5@gmail.com>
 
 # python 2 compatibility
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-import os
-from functools import wraps
-from warnings import warn
+from __future__ import absolute_import, division, print_function
 
 import datetime
 import functools
 import hashlib
+import os
 import pickle
 from concurrent.futures import ThreadPoolExecutor
+from functools import wraps
+from typing import Callable, Literal, Optional, TypedDict, Union
+from warnings import warn
 
-from .base_core import RecalculationNeeded
-from .pickle_core import _PickleCore
-from .mongo_core import _MongoCore
-from .memory_core import _MemoryCore
+from pymongo.collection import Collection
 
+from .base_core import RecalculationNeeded, _BaseCore
+from .memory_core import _MemoryCore
+from .mongo_core import _MongoCore
+from .pickle_core import _PickleCore
 
 MAX_WORKERS_ENVAR_NAME = 'CACHIER_MAX_WORKERS'
 DEFAULT_MAX_WORKERS = 8
 
 
 def _max_workers():
     try:
@@ -88,39 +87,60 @@
     return hash.hexdigest()
 
 
 class MissingMongetter(ValueError):
     """Thrown when the mongetter keyword argument is missing."""
 
 
-_default_params = {
+HashFunc = Callable[..., str]
+Mongetter = Callable[[], Collection]
+Backend = Literal["pickle", "mongo", "memory"]
+
+
+class Params(TypedDict):
+    caching_enabled: bool
+    hash_func: HashFunc
+    backend: Backend
+    mongetter: Optional[Mongetter]
+    stale_after: datetime.timedelta
+    next_time: bool
+    cache_dir: Union[str, os.PathLike]
+    pickle_reload: bool
+    separate_files: bool
+    wait_for_calc_timeout: int
+    allow_none: bool
+
+
+_default_params: Params = {
     'caching_enabled': True,
     'hash_func': _default_hash_func,
     'backend': 'pickle',
     'mongetter': None,
     'stale_after': datetime.timedelta.max,
     'next_time': False,
     'cache_dir': '~/.cachier/',
     'pickle_reload': True,
     'separate_files': False,
     'wait_for_calc_timeout': 0,
+    'allow_none': False,
 }
 
 
 def cachier(
-    hash_func=None,
-    hash_params=None,
-    backend=None,
-    mongetter=None,
-    stale_after=None,
-    next_time=None,
-    cache_dir=None,
-    pickle_reload=None,
-    separate_files=None,
-    wait_for_calc_timeout=None,
+    hash_func: Optional[HashFunc] = None,
+    hash_params: Optional[HashFunc] = None,
+    backend: Optional[Backend] = None,
+    mongetter: Optional[Mongetter] = None,
+    stale_after: Optional[datetime.timedelta] = None,
+    next_time: Optional[bool] = None,
+    cache_dir: Optional[Union[str, os.PathLike]] = None,
+    pickle_reload: Optional[bool] = None,
+    separate_files: Optional[bool] = None,
+    wait_for_calc_timeout: Optional[int] = None,
+    allow_none: Optional[bool] = None,
 ):
     """A persistent, stale-free memoization decorator.
 
     The positional and keyword arguments to the wrapped function must be
     hashable (i.e. Python's immutable built-in objects, not mutable
     containers). Also, notice that since objects which are instances of
     user-defined classes are hashable but all compare unequal (their hash
@@ -166,28 +186,32 @@
         if you per-function cache files become too large.
     wait_for_calc_timeout: int, optional, for MongoDB only
         The maximum time to wait for an ongoing calculation. When a
         process started to calculate the value setting being_calculated to
         True, any process trying to read the same entry will wait a maximum of
         seconds specified in this parameter. 0 means wait forever.
         Once the timeout expires the calculation will be triggered.
+    allow_none: bool, optional
+        Allows storing None values in the cache. If False, functions returning
+        None will not be cached and are recalculated every call.
     """
     # Check for deprecated parameters
     if hash_params is not None:
         message = 'hash_params will be removed in a future release, ' \
                   'please use hash_func instead'
         warn(message, DeprecationWarning, stacklevel=2)
         hash_func = hash_params
     # Override the backend parameter if a mongetter is provided.
     if mongetter is None:
         mongetter = _default_params['mongetter']
     if callable(mongetter):
         backend = 'mongo'
     if backend is None:
         backend = _default_params['backend']
+    core: _BaseCore
     if backend == 'pickle':
         core = _PickleCore(  # pylint: disable=R0204
             hash_func=hash_func,
             pickle_reload=pickle_reload,
             cache_dir=cache_dir,
             separate_files=separate_files,
             wait_for_calc_timeout=wait_for_calc_timeout,
@@ -204,27 +228,28 @@
             default_params=_default_params,
         )
     elif backend == 'memory':
         core = _MemoryCore(
             hash_func=hash_func,
             default_params=_default_params,
         )
-    elif backend == 'redis':
-        raise NotImplementedError(
-            'A Redis backend has not yet been implemented. '
-            'Please see https://github.com/python-cachier/cachier/issues/4'
-        )
     else:
         raise ValueError('specified an invalid core: {}'.format(backend))
 
     def _cachier_decorator(func):
         core.set_func(func)
 
         @wraps(func)
         def func_wrapper(*args, **kwds):  # pylint: disable=C0111,R0911
+            nonlocal allow_none
+            _allow_none = (
+                allow_none
+                if allow_none is not None else
+                _default_params['allow_none']
+            )
             # print('Inside general wrapper for {}.'.format(func.__name__))
             ignore_cache = kwds.pop('ignore_cache', False)
             overwrite_cache = kwds.pop('overwrite_cache', False)
             verbose_cache = kwds.pop('verbose_cache', False)
             _print = lambda x: None  # skipcq: FLK-E731  # noqa: E731
             if verbose_cache:
                 _print = print
@@ -234,15 +259,15 @@
                 key, entry = core.get_entry(args[1:], kwds)
             else:
                 key, entry = core.get_entry(args, kwds)
             if overwrite_cache:
                 return _calc_entry(core, key, func, args, kwds)
             if entry is not None:  # pylint: disable=R0101
                 _print('Entry found.')
-                if entry.get('value', None) is not None:
+                if (_allow_none or entry.get('value', None) is not None):
                     _print('Cached result found.')
                     local_stale_after = stale_after if stale_after is not None else _default_params['stale_after']  # noqa: E501
                     local_next_time = next_time if next_time is not None else _default_params['next_time']  # noqa: E501
                     now = datetime.datetime.now()
                     if now - entry['time'] > local_stale_after:
                         _print('But it is stale... :(')
                         if entry['being_calculated']:
```

### Comparing `cachier-2.1.1/cachier/memory_core.py` & `cachier-2.2.0/cachier/memory_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/cachier/mongo_core.py` & `cachier-2.2.0/cachier/mongo_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/cachier/pickle_core.py` & `cachier-2.2.0/cachier/pickle_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/cachier.egg-info/PKG-INFO` & `cachier-2.2.0/cachier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: cachier
-Version: 2.1.1
+Version: 2.2.0
 Summary: Persistent, stale-free, local and cross-machine caching for Python functions.
 Home-page: https://github.com/python-cachier/cachier
 Author: Shay Palachy
 Author-email: shay.palachy@gmail.com
 License: MIT
 Keywords: cache,persistence,mongo,memoization,decorator
 Platform: linux
 Platform: osx
 Platform: windows
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Other/Nonlisted Topic
 Classifier: Intended Audience :: Developers
 Provides-Extra: test
 License-File: LICENSE
@@ -68,15 +68,15 @@
 
     pip install 'cachier==1.2.8'
 
 Features
 ========
 
 * Pure Python.
-* Compatible with Python 3.5+ (and Python 2.7 up until version 1.2.8).
+* Compatible with Python 3.8+ (Python 2.7 was discontinued in version 1.2.8).
 * Supported and `tested on Linux, OS X and Windows <https://travis-ci.org/shaypal5/cachier>`_.
 * A simple interface.
 * Defining "shelf life" for cached values.
 * Local caching using pickle files.
 * Cross-machine caching using MongoDB.
 * Thread-safety.
 
@@ -163,14 +163,15 @@
 *  `mongetter`
 *  `cache_dir`
 *  `pickle_reload`
 *  `separate_files`
 
 These parameters can be changed at any time and they will apply to all decorators:
 
+*  `allow_none`
 *  `caching_enabled`
 *  `stale_after`
 *  `next_time`
 *  `wait_for_calc_timeout`
 
 The current defaults can be fetched by calling `get_default_params`.
 
@@ -280,14 +281,18 @@
 You can have ``cachier`` overwrite an existing cache entry - if one exists - for a specific function call by passing ``overwrite_cache=True`` to the function call. The cache will not be checked but will be updated with the new return value.
 
 Verbose Cache Call
 ~~~~~~~~~~~~~~~~~~
 
 You can have ``cachier`` print out a detailed explanation of the logic of a specific call by passing ``verbose_cache=True`` to the function call. This can be useful if you are not sure why a certain function result is, or is not, returned.
 
+Cache `None` Values
+~~~~~~~~~~~~~~~~~~~
+
+By default, ``cachier`` does not cache ``None`` values. You can override this behaviour by passing ``allow_none=True`` to the function call.
 
 
 Cachier Cores
 =============
 
 Pickle Core
 -----------
@@ -488,9 +493,7 @@
 .. |Codefactor| image:: https://www.codefactor.io/repository/github/python-cachier/cachier/badge?style=plastic
      :target: https://www.codefactor.io/repository/github/python-cachier/cachier
      :alt: Codefactor code quality
 
 .. links:
 .. _pymongo: https://api.mongodb.com/python/current/
 .. _watchdog: https://github.com/gorakhargosh/watchdog
-
-
```

### Comparing `cachier-2.1.1/cachier.egg-info/SOURCES.txt` & `cachier-2.2.0/cachier.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 .gitattributes
 .gitignore
 .ignore
 .pylintrc
 LICENSE
 MANIFEST.in
 README.rst
+mypy.ini
 pytest.ini
 setup.cfg
 setup.py
 versioneer.py
 .github/workflows/checkdocs.yml
 .github/workflows/lint.yml
 .github/workflows/test.yml
 cachier/__init__.py
 cachier/_version.py
 cachier/base_core.py
 cachier/core.py
 cachier/memory_core.py
 cachier/mongo_core.py
 cachier/pickle_core.py
+cachier/py.typed
 cachier.egg-info/PKG-INFO
 cachier.egg-info/SOURCES.txt
 cachier.egg-info/dependency_links.txt
 cachier.egg-info/entry_points.txt
 cachier.egg-info/requires.txt
 cachier.egg-info/top_level.txt
 cachier/scripts/__init__.py
```

### Comparing `cachier-2.1.1/setup.py` & `cachier-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/MIT-license
 # Copyright (c) 2016, Shay Palachy <shaypal5@gmail.com>
 
 try:
     from setuptools import setup
 except ImportError:
-    from distutils.core import setup
+    from distutils.core import setup  # type: ignore
 
 import versioneer
 
-
 TEST_REQUIRES = [
     # tests and coverages
     'pytest', 'coverage', 'pytest-cov',
     # linting and code quality
     'bandit', 'flake8', 'pylint', 'safety',
+    # type checking
+    'mypy', 'types-setuptools', 'pandas-stubs',
     # to connect to the test mongodb server
     'pymongo', 'dnspython', 'pymongo-inmemory',
     # to test pandas dataframe as-param hashing with mongodb core
     'pandas',
     # to be able to run `python setup.py checkdocs`
     'collective.checkdocs', 'pygments',
 ]
@@ -62,18 +63,18 @@
     classifiers=[
         # Trove classifiers
         # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Utilities',
         'Topic :: Other/Nonlisted Topic',
         'Intended Audience :: Developers',
     ],
 )
```

### Comparing `cachier-2.1.1/tests/speed_eval.py` & `cachier-2.2.0/tests/speed_eval.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/tests/test_core_lookup.py` & `cachier-2.2.0/tests/test_core_lookup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from cachier import cachier, get_default_params
 from cachier.core import MissingMongetter
 
 
 def test_get_default_params():
     params = get_default_params()
     assert tuple(sorted(params)) == (
+        'allow_none',
         'backend',
         'cache_dir',
         'caching_enabled',
         'hash_func',
         'mongetter',
         'next_time',
         'pickle_reload',
```

### Comparing `cachier-2.1.1/tests/test_defaults.py` & `cachier-2.2.0/tests/test_defaults.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
 import os
-import pytest
 import queue
 import random
 import tempfile
 import threading
 import time
 
-import cachier
-
-from tests.test_mongo_core import _test_mongetter, MONGO_DELTA
+import pytest
 
+import cachier
+from tests.test_mongo_core import MONGO_DELTA, _test_mongetter
 
 _default_params = cachier.get_default_params().copy()
 
 
 def setup_function():
     cachier.set_default_params(**_default_params)
 
@@ -121,14 +120,48 @@
 
     cache_dir_1 = global_test_1.cache_dpath()
     cache_dir_2 = global_test_2.cache_dpath()
     assert len(os.listdir(cache_dir_1)) == 2
     assert len(os.listdir(cache_dir_2)) == 1
 
 
+def test_allow_none_default_param():
+    cachier.set_default_params(
+        allow_none=True,
+        separate_files=True,
+        verbose_cache=True,
+    )
+    allow_count = 0
+    disallow_count = 0
+
+    @cachier.cachier(cache_dir=tempfile.mkdtemp())
+    def allow_none():
+        nonlocal allow_count
+        allow_count += 1
+        return None
+
+    @cachier.cachier(cache_dir=tempfile.mkdtemp(), allow_none=False)
+    def disallow_none():
+        nonlocal disallow_count
+        disallow_count += 1
+        return None
+
+    allow_none.clear_cache()
+    assert allow_count == 0
+    allow_none()
+    allow_none()
+    assert allow_count == 1
+
+    disallow_none.clear_cache()
+    assert disallow_count == 0
+    disallow_none()
+    disallow_none()
+    assert disallow_count == 2
+
+
 parametrize_keys = 'backend,mongetter'
 parametrize_values = [
     pytest.param('pickle', None, marks=pytest.mark.pickle),
     pytest.param('mongo', _test_mongetter, marks=pytest.mark.mongo),
 ]
```

### Comparing `cachier-2.1.1/tests/test_general.py` & `cachier-2.2.0/tests/test_general.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """Non-core-specific tests for cachier."""
 
 from __future__ import print_function
+
 import functools
 import os
 import queue
 import subprocess  # nosec: B404
 import threading
 from random import random
 from time import sleep, time
+
 import pytest
+
 import cachier
 from cachier.core import (
-    MAX_WORKERS_ENVAR_NAME,
     DEFAULT_MAX_WORKERS,
+    MAX_WORKERS_ENVAR_NAME,
+    _get_executor,
     _max_workers,
     _set_max_workers,
-    _get_executor
 )
 from tests.test_mongo_core import (
-    _test_mongetter,
     MONGO_DELTA_LONG,
+    _test_mongetter,
 )
 
 
 def test_information():
     print("\ncachier version: ", end="")
     print(cachier.__version__)
 
@@ -236,7 +239,39 @@
     result_2 = get_random()
     cachier.disable_caching()
     result_3 = get_random()
     cachier.enable_caching()
     result_4 = get_random()
     assert result_1 == result_2 == result_4
     assert result_1 != result_3
+
+
+def test_none_not_cached_by_default():
+    count = 0
+
+    @cachier.cachier()
+    def do_operation():
+        nonlocal count
+        count += 1
+        return None
+
+    do_operation.clear_cache()
+    assert count == 0
+    do_operation()
+    do_operation()
+    assert count == 2
+
+
+def test_allow_caching_none():
+    count = 0
+
+    @cachier.cachier(allow_none=True)
+    def do_operation():
+        nonlocal count
+        count += 1
+        return None
+
+    do_operation.clear_cache()
+    assert count == 0
+    do_operation()
+    do_operation()
+    assert count == 1
```

### Comparing `cachier-2.1.1/tests/test_memory_core.py` & `cachier-2.2.0/tests/test_memory_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/tests/test_mongo_core.py` & `cachier-2.2.0/tests/test_mongo_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """Testing the MongoDB core of cachier."""
 
-import sys
-import platform
 import datetime
+import hashlib
+import platform
+import queue
+import sys
+import threading
 from datetime import timedelta
 from random import random
 from time import sleep
-import threading
-import queue
 
-import pytest
-import pymongo
-import hashlib
 import pandas as pd
+import pymongo
+import pytest
 from pymongo.errors import OperationFailure
+from pymongo_inmemory import MongoClient
 
 from cachier import cachier
 from cachier.base_core import RecalculationNeeded
 from cachier.mongo_core import _MongoCore
 
-from pymongo_inmemory import MongoClient
-
-
 _COLLECTION_NAME = 'cachier_test_{}_{}.{}.{}'.format(
     platform.system(), sys.version_info[0], sys.version_info[1],
     sys.version_info[2])
 
 
 def _test_mongetter():
     if not hasattr(_test_mongetter, 'client'):
```

### Comparing `cachier-2.1.1/tests/test_pickle_core.py` & `cachier-2.2.0/tests/test_pickle_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 
 # from os.path import (
 #     realpath,
 #     dirname
 # )
 import os
 import pickle
-from time import (
-    time,
-    sleep
-)
+import threading
 from datetime import timedelta
 from random import random
-import threading
+from time import sleep, time
 
 import pytest
 
 try:
     import queue
 except ImportError:  # python 2
-    import Queue as queue
+    import Queue as queue  # type: ignore
 
 import hashlib
+
 import pandas as pd
 
 from cachier import cachier
 from cachier.core import _default_params
 
 
 def _get_decorated_func(func, **kwargs):
@@ -372,15 +370,15 @@
     thread2.join(timeout=2)
     if not res_queue.qsize() == 2:
         return False
     res1 = res_queue.get()
     if not isinstance(res1, float):
         return False
     res2 = res_queue.get()
-    if not (res2 is None) or isinstance(res2, KeyError):
+    if res2 is not None or isinstance(res2, KeyError):
         return False
     return True
 
 
 # we want this to succeed at leat once
 @pytest.mark.pickle
 @pytest.mark.xfail
```

### Comparing `cachier-2.1.1/tests/test_security.py` & `cachier-2.2.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.1/versioneer.py` & `cachier-2.2.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,18 +345,19 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
-    import ConfigParser as configparser
+    import ConfigParser as configparser  # type: ignore
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
 
@@ -1543,15 +1544,15 @@
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore[import]
 
         class cmd_build_exe(_build_exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
```

