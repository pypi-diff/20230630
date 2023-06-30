# Comparing `tmp/openai_pricing-1.1.tar.gz` & `tmp/openai-pricing-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "C:\Users\Pedro\Documents\Trabalho\alo-mundo\openai-pricing\openai-pricing\dist\.tmp-ys3u3oma\openai-pricing-1.1.1.tar", last modified: Fri Jun 30 01:23:12 2023, max compression
```

## Comparing `openai_pricing-1.1.tar` & `openai-pricing-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openai_pricing-1.1/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_pricing-1.1/__init__.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 openai_pricing-1.1/openai_pricing.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 openai_pricing-1.1/setup.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 openai_pricing-1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 openai_pricing-1.1/openai_pricing.egg-info/PKG-INFO
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openai_pricing-1.1/openai_pricing.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 openai_pricing-1.1/openai_pricing.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 openai_pricing-1.1/openai_pricing.egg-info/top_level.txt
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 openai_pricing-1.1/pyproject.toml
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openai_pricing-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 01:23:12.227476 openai-pricing-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-30 01:07:03.000000 openai-pricing-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6288 2023-06-29 18:49:16.000000 openai-pricing-1.1.1/OpenAIPricing.py
+-rw-rw-rw-   0        0        0      561 2023-06-30 01:23:12.227476 openai-pricing-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-29 18:48:25.000000 openai-pricing-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 01:23:12.225467 openai-pricing-1.1.1/openai_pricing.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      786 2023-06-30 01:17:39.000000 openai-pricing-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 01:23:12.227476 openai-pricing-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-30 01:17:53.000000 openai-pricing-1.1.1/setup.py
```

### Comparing `openai_pricing-1.1/README.md` & `openai-pricing-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_pricing-1.1/openai_pricing.py` & `openai-pricing-1.1.1/OpenAIPricing.py`

 * *Files identical despite different names*

### Comparing `openai_pricing-1.1/setup.py` & `openai-pricing-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     #this will be the package name you will see, e.g. the output of 'conda list' in anaconda prompt
     name = 'openai-pricing', 
     #some version number you may wish to add - increment this after every update
-    version='1.0', 
+    version='1.1.1', 
   
     # Use one of the below approach to define package and/or module names:
   
     #if there are only handful of modules placed in root directory, and no packages/directories exist then can use below syntax
 #     packages=[''], #have to import modules directly in code after installing this wheel, like import mod2 (respective file name in this case is mod2.py) - no direct use of distribution name while importing
   
     #can list down each package names - no need to keep __init__.py under packages / directories
```

### Comparing `openai_pricing-1.1/pyproject.toml` & `openai-pricing-1.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai-pricing"
-version = "1.1"
+version = "1.1.1"
 requires-python = ">=3.8"
 authors = [
   {name = "Pedro Dupim", email = "pedrodupim@icloud.com"},
 ]
 maintainers = [
   {name = "Pedro Dupim", email = "pedrodupim@icloud.com"},
 ]
 keywords = ["openai", "chat gpt", "pricing"]
 dependencies = [
   "requests",
   "pandas",
   "tabulate",
 ]
-dynamic = ["description", "optional-dependencies"]
+description = "Easily check the current costs of OpenAI's GPT and ChatGPT models."
+dynamic = ["optional-dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/Alo-mundo/openai-pricing"
 Documentation = "https://github.com/Alo-mundo/openai-pricing/blob/main/README.md"
 Repository = "https://github.com/Alo-mundo/openai-pricing.git"
```

