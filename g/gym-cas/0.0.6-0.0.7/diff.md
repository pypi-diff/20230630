# Comparing `tmp/gym_cas-0.0.6.tar.gz` & `tmp/gym_cas-0.0.7.tar.gz`

## Comparing `gym_cas-0.0.6.tar` & `gym_cas-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gym_cas-0.0.6/bitbucket-pipelines.yml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gym_cas-0.0.6/src/gym_cas/__about__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 gym_cas-0.0.6/src/gym_cas/__init__.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 gym_cas-0.0.6/src/gym_cas/trigonometry.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gym_cas-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 gym_cas-0.0.6/tests/cheatsheet_examples.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 gym_cas-0.0.6/tests/test_abc.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 gym_cas-0.0.6/tests/test_trigonometry.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gym_cas-0.0.6/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gym_cas-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 gym_cas-0.0.6/README.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gym_cas-0.0.6/hatch.toml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 gym_cas-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 gym_cas-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 gym_cas-0.0.7/bitbucket-pipelines.yml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 gym_cas-0.0.7/examples/cheatsheet.ipynb
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/__about__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/__init__.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/plot.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 gym_cas-0.0.7/src/gym_cas/trigonometry.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 gym_cas-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 gym_cas-0.0.7/tests/test_abc.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 gym_cas-0.0.7/tests/test_trigonometry.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 gym_cas-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gym_cas-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 gym_cas-0.0.7/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gym_cas-0.0.7/hatch.toml
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 gym_cas-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 gym_cas-0.0.7/PKG-INFO
```

### Comparing `gym_cas-0.0.6/.pytest_cache/v/cache/nodeids` & `gym_cas-0.0.7/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.6/src/gym_cas/trigonometry.py` & `gym_cas-0.0.7/src/gym_cas/trigonometry.py`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.6/tests/test_trigonometry.py` & `gym_cas-0.0.7/tests/test_trigonometry.py`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.6/LICENSE.txt` & `gym_cas-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.6/README.md` & `gym_cas-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ```console
 pip install gym-cas
 ```
 
 ## Cheatsheet
 
-Alle eksempler antager at `gym_cas` først importeres således:
+I nedenstående afsnit antages det at `gym_cas` først importeres således:
 
 ```py
 from gym_cas import *
 ```
 
 ### B1. Tal- og bogstavregning
 
@@ -31,7 +31,19 @@
 ```py
 solve( udtryk )
 solve( [udtryk1, udtryk2] )
 nsolve( udtryk, start )
 ```
 
 Bemærk at den nemmeste måde at bruge `solve` i `SymPy` er ved at omforme sin ligning så en af siderne er lig 0. Hvis man fx vil løse ligningen `x/2 = 10` så kan det skrives `solve(x/2-10)`.
+
+### B3. Geometri og trigonometri
+
+```py
+Sin( vinkel )
+Cos( vinkel )
+Tan( vinkel )
+aSin( forhold )
+aCos( forhold )
+aTan( forhold )
+```
+
```

### Comparing `gym_cas-0.0.6/hatch.toml` & `gym_cas-0.0.7/hatch.toml`

 * *Files identical despite different names*

### Comparing `gym_cas-0.0.6/pyproject.toml` & `gym_cas-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,36 @@
 [project]
 name = "gym-cas"
 dynamic = ["version"]
 description = "Tools to aid the use of Python as CAS in danish high schools."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["matematik, math, gymnasium, HTX, sympy"]
+keywords = ["CAS, Matematik, Math, Gymnasium, HTX"]
 authors = [
   { name = "JACS", email = "jacs@zbc.dk" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Intended Audience :: Education",
+    "Topic :: Education",
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "Development Status :: 3 - Alpha"
+]
+dependencies = [
+    "sympy>=1.12", 
+    "matplotlib>=3.7.1", 
+    "numpy>=1.25.0",
+    "sympy_plot_backends>=2.3.0"
 ]
-dependencies = ["sympy>=1.12"]
 
 [project.urls]
 "Homepage" = "https://jacs-mat.bitbucket.io/"
 
 [tool.black]
 target-version = ["py37"]
 line-length = 120
```

