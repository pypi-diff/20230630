# Comparing `tmp/openai-pricing-1.1.1.tar.gz` & `tmp/openai-pricing-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Pedro\Documents\Trabalho\alo-mundo\openai-pricing\openai-pricing\dist\.tmp-ys3u3oma\openai-pricing-1.1.1.tar", last modified: Fri Jun 30 01:23:12 2023, max compression
+gzip compressed data, was "C:\Users\Pedro\Documents\Trabalho\alo-mundo\openai-pricing\openai-pricing\dist\.tmp-fdqf0ijv\openai-pricing-1.1.2.tar", last modified: Fri Jun 30 01:37:06 2023, max compression
```

## Comparing `openai-pricing-1.1.1.tar` & `openai-pricing-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:12.227476 openai-pricing-1.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-30 01:07:03.000000 openai-pricing-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6288 2023-06-29 18:49:16.000000 openai-pricing-1.1.1/OpenAIPricing.py
--rw-rw-rw-   0        0        0      561 2023-06-30 01:23:12.227476 openai-pricing-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-29 18:48:25.000000 openai-pricing-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:12.225467 openai-pricing-1.1.1/openai_pricing.egg-info/
--rw-rw-rw-   0        0        0      561 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 01:23:12.000000 openai-pricing-1.1.1/openai_pricing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      786 2023-06-30 01:17:39.000000 openai-pricing-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 01:23:12.227476 openai-pricing-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-30 01:17:53.000000 openai-pricing-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:37:06.243686 openai-pricing-1.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-30 01:07:03.000000 openai-pricing-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6288 2023-06-29 18:49:16.000000 openai-pricing-1.1.2/OpenAIPricing.py
+-rw-rw-rw-   0        0        0     3114 2023-06-30 01:37:06.243686 openai-pricing-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-29 18:48:25.000000 openai-pricing-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 01:37:06.241691 openai-pricing-1.1.2/openai_pricing.egg-info/
+-rw-rw-rw-   0        0        0     3114 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      808 2023-06-30 01:36:55.000000 openai-pricing-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 01:37:06.243686 openai-pricing-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-30 01:17:53.000000 openai-pricing-1.1.2/setup.py
```

### Comparing `openai-pricing-1.1.1/LICENSE` & `openai-pricing-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-pricing-1.1.1/OpenAIPricing.py` & `openai-pricing-1.1.2/OpenAIPricing.py`

 * *Files identical despite different names*

### Comparing `openai-pricing-1.1.1/README.md` & `openai-pricing-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openai-pricing-1.1.1/pyproject.toml` & `openai-pricing-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai-pricing"
-version = "1.1.1"
+version = "1.1.2"
 requires-python = ">=3.8"
 authors = [
   {name = "Pedro Dupim", email = "pedrodupim@icloud.com"},
 ]
 maintainers = [
   {name = "Pedro Dupim", email = "pedrodupim@icloud.com"},
 ]
@@ -16,13 +16,14 @@
 dependencies = [
   "requests",
   "pandas",
   "tabulate",
 ]
 description = "Easily check the current costs of OpenAI's GPT and ChatGPT models."
 dynamic = ["optional-dependencies"]
+readme = "README.md"
 
 [project.urls]
 Homepage = "https://github.com/Alo-mundo/openai-pricing"
 Documentation = "https://github.com/Alo-mundo/openai-pricing/blob/main/README.md"
 Repository = "https://github.com/Alo-mundo/openai-pricing.git"
```

### Comparing `openai-pricing-1.1.1/setup.py` & `openai-pricing-1.1.2/setup.py`

 * *Files identical despite different names*

