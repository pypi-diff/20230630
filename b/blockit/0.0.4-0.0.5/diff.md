# Comparing `tmp/blockit-0.0.4.tar.gz` & `tmp/blockit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockit-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "blockit-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `blockit-0.0.4.tar` & `blockit-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.4/.dockerignore
--rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.4/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.4/Dockerfile
--rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.4/Hillciph.pdf
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.4/LICENSE
--rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.4/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.4/README.md
--rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.4/ascii-table.png
--rw-r--r--   0        0        0       22 2023-06-30 03:51:35.013167 blockit-0.0.4/blockit/__init__.py
--rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.4/blockit/__main__.py
--rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.4/blockit/cli.py
--rw-r--r--   0        0        0    23430 2023-06-30 03:50:59.577444 blockit-0.0.4/blockit/crypto_algorithms.py
--rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.4/blockit/reverse_encryption_api.py
--rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.4/docker-compose.yml
--rw-r--r--   0        0        0     2292 2023-06-30 03:42:57.591831 blockit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      194 2023-06-30 02:44:18.097885 blockit-0.0.4/requirements.txt
--rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.4/setup.cfg
--rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.4/test_build.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 blockit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.5/.dockerignore
+-rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.5/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      929 2023-06-30 03:57:14.759274 blockit-0.0.5/Dockerfile
+-rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.5/Hillciph.pdf
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.5/LICENSE
+-rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.5/Makefile
+-rw-r--r--   0        0        0     6246 2023-06-30 06:41:56.563735 blockit-0.0.5/README.md
+-rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.5/ascii-table.png
+-rw-r--r--   0        0        0       22 2023-06-30 06:42:55.880671 blockit-0.0.5/blockit/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.5/blockit/__main__.py
+-rw-r--r--   0        0        0      947 2023-06-30 06:29:05.886752 blockit-0.0.5/blockit/cli.py
+-rw-r--r--   0        0        0    23428 2023-06-30 06:28:32.414492 blockit-0.0.5/blockit/crypto_algorithms.py
+-rw-r--r--   0        0        0      684 2023-06-30 02:43:18.583682 blockit-0.0.5/blockit/reverse_encryption_api.py
+-rw-r--r--   0        0        0      261 2023-06-30 04:08:43.093692 blockit-0.0.5/docker-compose.yml
+-rw-r--r--   0        0        0     2292 2023-06-30 03:42:57.591831 blockit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-06-30 04:17:36.618679 blockit-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.5/setup.cfg
+-rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.5/test_build.py
+-rw-r--r--   0        0        0     7373 1970-01-01 00:00:00.000000 blockit-0.0.5/PKG-INFO
```

### Comparing `blockit-0.0.4/.gitignore` & `blockit-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `blockit-0.0.4/Dockerfile` & `blockit-0.0.5/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # new caching mechanism that can cache these dependencies download, instead of downloading them each time.
 RUN --mount=type=cache,target=/root/.cache \
     pip install -r requirements.txt
 
 # Add app
 COPY . .
 
-CMD uvicorn blockit.api:app --reload --workers 1 --host 0.0.0.0 --port 8000
+CMD uvicorn blockit.reverse_encryption_api:app --reload --workers 1 --host 0.0.0.0 --port 8000
```

### Comparing `blockit-0.0.4/Hillciph.pdf` & `blockit-0.0.5/Hillciph.pdf`

 * *Files identical despite different names*

### Comparing `blockit-0.0.4/LICENSE` & `blockit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `blockit-0.0.4/ascii-table.png` & `blockit-0.0.5/ascii-table.png`

 * *Files identical despite different names*

### Comparing `blockit-0.0.4/blockit/cli.py` & `blockit-0.0.5/blockit/cli.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.4/blockit/crypto_algorithms.py` & `blockit-0.0.5/blockit/crypto_algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,15 +740,15 @@
     def create_algorithm(algorithm_name: str, **kwargs):
         """
         Create a crypto algorithm instance based on the specified algorithm name and optional arguments.
         Returns:
         - CryptoAlgorithm: An instance of the specified crypto algorithm.
         """
         if algorithm_name == "shift":
-            shift = int(kwargs.get("--shift", 3))
+            shift = int(kwargs.get("shift", 3))
             return ShiftEncryption(shift)
         elif algorithm_name == "matrix":
             return MatrixEncryption()
         elif algorithm_name == "reverse":
             encrypt_url = "https://encryption-api-five.vercel.app/encode"
             decrypt_url = "https://encryption-api-five.vercel.app/decode"
             return ReverseEncryption(encrypt_url=encrypt_url, decrypt_url=decrypt_url)
```

### Comparing `blockit-0.0.4/blockit/reverse_encryption_api.py` & `blockit-0.0.5/blockit/reverse_encryption_api.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.4/pyproject.toml` & `blockit-0.0.5/pyproject.toml`

 * *Files identical despite different names*

