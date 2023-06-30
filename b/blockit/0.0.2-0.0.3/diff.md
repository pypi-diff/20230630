# Comparing `tmp/blockit-0.0.2.tar.gz` & `tmp/blockit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockit-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "blockit-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `blockit-0.0.2.tar` & `blockit-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.2/.dockerignore
--rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.2/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.2/Dockerfile
--rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.2/Hillciph.pdf
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.2/LICENSE
--rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.2/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.2/README.md
--rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.2/ascii-table.png
--rw-r--r--   0        0        0       22 2023-06-30 03:36:29.437662 blockit-0.0.2/blockit/__init__.py
--rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.2/blockit/__main__.py
--rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.2/blockit/cli.py
--rw-r--r--   0        0        0    23430 2023-06-30 03:33:20.021033 blockit-0.0.2/blockit/crypto_algorithms.py
--rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.2/blockit/reverse_encryption_api.py
--rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.2/docker-compose.yml
--rw-r--r--   0        0        0     2269 2023-06-29 14:06:17.584638 blockit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      194 2023-06-30 02:44:18.097885 blockit-0.0.2/requirements.txt
--rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.2/setup.cfg
--rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.2/test_build.py
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 blockit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.3/.dockerignore
+-rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.3/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.3/Dockerfile
+-rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.3/Hillciph.pdf
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.3/LICENSE
+-rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.3/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.3/README.md
+-rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.3/ascii-table.png
+-rw-r--r--   0        0        0       22 2023-06-30 03:43:22.591335 blockit-0.0.3/blockit/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.3/blockit/__main__.py
+-rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.3/blockit/cli.py
+-rw-r--r--   0        0        0    23430 2023-06-30 03:33:20.021033 blockit-0.0.3/blockit/crypto_algorithms.py
+-rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.3/blockit/reverse_encryption_api.py
+-rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.3/docker-compose.yml
+-rw-r--r--   0        0        0     2292 2023-06-30 03:42:57.591831 blockit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-06-30 02:44:18.097885 blockit-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.3/setup.cfg
+-rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.3/test_build.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 blockit-0.0.3/PKG-INFO
```

### Comparing `blockit-0.0.2/.gitignore` & `blockit-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/Dockerfile` & `blockit-0.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/Hillciph.pdf` & `blockit-0.0.3/Hillciph.pdf`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/LICENSE` & `blockit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/ascii-table.png` & `blockit-0.0.3/ascii-table.png`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/blockit/cli.py` & `blockit-0.0.3/blockit/cli.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/blockit/crypto_algorithms.py` & `blockit-0.0.3/blockit/crypto_algorithms.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/blockit/reverse_encryption_api.py` & `blockit-0.0.3/blockit/reverse_encryption_api.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.2/pyproject.toml` & `blockit-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Security :: Cryptography",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "typer >= 0.9.0",
+    "httpx >= 0.24.1",
 ]
 
 [project.scripts]
 blockit = "blockit.cli:app"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `blockit-0.0.2/PKG-INFO` & `blockit-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: blockit
-Version: 0.0.2
+Version: 0.0.3
 Summary: blockit - cli tool for encrypting and decrypting strings
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: typer >= 0.9.0
+Requires-Dist: httpx >= 0.24.1
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: codecov ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
```

