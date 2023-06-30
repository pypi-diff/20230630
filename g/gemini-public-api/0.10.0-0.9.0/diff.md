# Comparing `tmp/gemini_public_api-0.10.0.tar.gz` & `tmp/gemini_public_api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_public_api-0.10.0.tar", max compression
+gzip compressed data, was "gemini_public_api-0.9.0.tar", max compression
```

## Comparing `gemini_public_api-0.10.0.tar` & `gemini_public_api-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/LICENSE
--rw-r--r--   0        0        0     2523 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/aiohttp/__init__.py
--rw-r--r--   0        0        0     6593 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/aiohttp/api.py
--rw-r--r--   0        0        0     1078 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/aiohttp/session_context_manager.py
--rw-r--r--   0        0        0     5439 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/api.py
--rw-r--r--   0        0        0      640 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/public_endpoints.py
--rw-r--r--   0        0        0      720 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/gemini_public_api/public_sandbox_endpoints.py
--rw-r--r--   0        0        0      506 2023-06-30 21:19:23.462152 gemini_public_api-0.10.0/pyproject.toml
--rw-r--r--   0        0        0     3004 1970-01-01 00:00:00.000000 gemini_public_api-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1468 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/gemini_public_api/__init__.py
+-rw-r--r--   0        0        0    10543 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/gemini_public_api/api.py
+-rw-r--r--   0        0        0      490 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/gemini_public_api/exceptions.py
+-rw-r--r--   0        0        0      746 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/gemini_public_api/public_endpoints.py
+-rw-r--r--   0        0        0      826 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/gemini_public_api/public_sandbox_endpoints.py
+-rw-r--r--   0        0        0      439 2023-03-12 22:16:54.029631 gemini_public_api-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1908 1970-01-01 00:00:00.000000 gemini_public_api-0.9.0/PKG-INFO
```

### Comparing `gemini_public_api-0.10.0/LICENSE` & `gemini_public_api-0.9.0/LICENSE`

 * *Files identical despite different names*

