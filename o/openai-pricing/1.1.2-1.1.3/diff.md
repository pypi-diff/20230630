# Comparing `tmp/openai-pricing-1.1.2.tar.gz` & `tmp/openai-pricing-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Pedro\Documents\Trabalho\alo-mundo\openai-pricing\openai-pricing\dist\.tmp-fdqf0ijv\openai-pricing-1.1.2.tar", last modified: Fri Jun 30 01:37:06 2023, max compression
+gzip compressed data, was "C:\Users\Pedro\Documents\Trabalho\alo-mundo\openai-pricing\openai-pricing\dist\.tmp-oraafvp3\openai-pricing-1.1.3.tar", last modified: Fri Jun 30 01:42:00 2023, max compression
```

## Comparing `openai-pricing-1.1.2.tar` & `openai-pricing-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:37:06.243686 openai-pricing-1.1.2/
--rw-rw-rw-   0        0        0     1091 2023-06-30 01:07:03.000000 openai-pricing-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     6288 2023-06-29 18:49:16.000000 openai-pricing-1.1.2/OpenAIPricing.py
--rw-rw-rw-   0        0        0     3114 2023-06-30 01:37:06.243686 openai-pricing-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-29 18:48:25.000000 openai-pricing-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 01:37:06.241691 openai-pricing-1.1.2/openai_pricing.egg-info/
--rw-rw-rw-   0        0        0     3114 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 01:37:06.000000 openai-pricing-1.1.2/openai_pricing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      808 2023-06-30 01:36:55.000000 openai-pricing-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 01:37:06.243686 openai-pricing-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-30 01:17:53.000000 openai-pricing-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:42:00.802111 openai-pricing-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-30 01:07:03.000000 openai-pricing-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3195 2023-06-30 01:42:00.802111 openai-pricing-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2591 2023-06-30 01:41:44.000000 openai-pricing-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 01:42:00.800117 openai-pricing-1.1.3/openai_pricing.egg-info/
+-rw-rw-rw-   0        0        0     3195 2023-06-30 01:42:00.000000 openai-pricing-1.1.3/openai_pricing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-30 01:42:00.000000 openai-pricing-1.1.3/openai_pricing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:42:00.000000 openai-pricing-1.1.3/openai_pricing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-30 01:42:00.000000 openai-pricing-1.1.3/openai_pricing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-30 01:42:00.000000 openai-pricing-1.1.3/openai_pricing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      808 2023-06-30 01:40:26.000000 openai-pricing-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 01:42:00.803109 openai-pricing-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-06-30 01:39:52.000000 openai-pricing-1.1.3/setup.py
```

### Comparing `openai-pricing-1.1.2/LICENSE` & `openai-pricing-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-pricing-1.1.2/PKG-INFO` & `openai-pricing-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: openai-pricing
-Version: 1.1.2
+Version: 1.1.3
 Summary: Easily check the current costs of OpenAI's GPT and ChatGPT models.
 Author-email: Pedro Dupim <pedrodupim@icloud.com>
 Maintainer-email: Pedro Dupim <pedrodupim@icloud.com>
 Project-URL: Homepage, https://github.com/Alo-mundo/openai-pricing
 Project-URL: Documentation, https://github.com/Alo-mundo/openai-pricing/blob/main/README.md
 Project-URL: Repository, https://github.com/Alo-mundo/openai-pricing.git
 Keywords: openai,chat gpt,pricing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openai-pricing
+================
 
 This repository hosts an unofficial library for OpenAI pricing calculations. Its purpose is to simplify the prediction of costs when using GPT models. The data is obtained from https://gptforwork.com/tools/openai-chatgpt-api-pricing-calculator.
 
 ##  Library usage
+-----------------
 
 The module provides just one class, `OpneAIPricing`, which loads the pricing data when instanced and answers about max tokens and costs per tokens (prompt and completion tokens).
 
 Currently, it supports the following models:
 
 - GPT-4 32k
 - GPT-4
@@ -33,14 +35,16 @@
 
 This list can be obtained by calling `OpenAIPricing.list_available_models()`.
 
 ### Example
 -----------
 
 ```shell
+from openai_pricing import OpenAIPricing
+
 p = OpenAIPricing()
 
 p.list_available_models()
 
 
 model = 'gpt-4-32k'
 tokens = 1000 # default value for tokens is 1000
```

### Comparing `openai-pricing-1.1.2/README.md` & `openai-pricing-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # openai-pricing
+================
 
 This repository hosts an unofficial library for OpenAI pricing calculations. Its purpose is to simplify the prediction of costs when using GPT models. The data is obtained from https://gptforwork.com/tools/openai-chatgpt-api-pricing-calculator.
 
 ##  Library usage
+-----------------
 
 The module provides just one class, `OpneAIPricing`, which loads the pricing data when instanced and answers about max tokens and costs per tokens (prompt and completion tokens).
 
 Currently, it supports the following models:
 
 - GPT-4 32k
 - GPT-4
@@ -19,14 +21,16 @@
 
 This list can be obtained by calling `OpenAIPricing.list_available_models()`.
 
 ### Example
 -----------
 
 ```shell
+from openai_pricing import OpenAIPricing
+
 p = OpenAIPricing()
 
 p.list_available_models()
 
 
 model = 'gpt-4-32k'
 tokens = 1000 # default value for tokens is 1000
```

### Comparing `openai-pricing-1.1.2/openai_pricing.egg-info/PKG-INFO` & `openai-pricing-1.1.3/openai_pricing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: openai-pricing
-Version: 1.1.2
+Version: 1.1.3
 Summary: Easily check the current costs of OpenAI's GPT and ChatGPT models.
 Author-email: Pedro Dupim <pedrodupim@icloud.com>
 Maintainer-email: Pedro Dupim <pedrodupim@icloud.com>
 Project-URL: Homepage, https://github.com/Alo-mundo/openai-pricing
 Project-URL: Documentation, https://github.com/Alo-mundo/openai-pricing/blob/main/README.md
 Project-URL: Repository, https://github.com/Alo-mundo/openai-pricing.git
 Keywords: openai,chat gpt,pricing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openai-pricing
+================
 
 This repository hosts an unofficial library for OpenAI pricing calculations. Its purpose is to simplify the prediction of costs when using GPT models. The data is obtained from https://gptforwork.com/tools/openai-chatgpt-api-pricing-calculator.
 
 ##  Library usage
+-----------------
 
 The module provides just one class, `OpneAIPricing`, which loads the pricing data when instanced and answers about max tokens and costs per tokens (prompt and completion tokens).
 
 Currently, it supports the following models:
 
 - GPT-4 32k
 - GPT-4
@@ -33,14 +35,16 @@
 
 This list can be obtained by calling `OpenAIPricing.list_available_models()`.
 
 ### Example
 -----------
 
 ```shell
+from openai_pricing import OpenAIPricing
+
 p = OpenAIPricing()
 
 p.list_available_models()
 
 
 model = 'gpt-4-32k'
 tokens = 1000 # default value for tokens is 1000
```

### Comparing `openai-pricing-1.1.2/pyproject.toml` & `openai-pricing-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai-pricing"
-version = "1.1.2"
+version = "1.1.3"
 requires-python = ">=3.8"
 authors = [
   {name = "Pedro Dupim", email = "pedrodupim@icloud.com"},
 ]
 maintainers = [
   {name = "Pedro Dupim", email = "pedrodupim@icloud.com"},
 ]
```

### Comparing `openai-pricing-1.1.2/setup.py` & `openai-pricing-1.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #     packages=[''], #have to import modules directly in code after installing this wheel, like import mod2 (respective file name in this case is mod2.py) - no direct use of distribution name while importing
   
     #can list down each package names - no need to keep __init__.py under packages / directories
 #     packages=['<list of name of packages>'], #importing is like: from package1 import mod2, or import package1.mod2 as m2
   
     #this approach automatically finds out all directories (packages) - those must contain a file named __init__.py (can be empty)
     packages=find_packages(), #include/exclude arguments take * as wildcard, . for any sub-package names
-    py_modules=['OpenAIPricing'],
+    py_modules=['openai_pricing'],
 )
```

