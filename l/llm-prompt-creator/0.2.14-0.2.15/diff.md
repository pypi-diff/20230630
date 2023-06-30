# Comparing `tmp/llm_prompt_creator-0.2.14.tar.gz` & `tmp/llm_prompt_creator-0.2.15.tar.gz`

## Comparing `llm_prompt_creator-0.2.14.tar` & `llm_prompt_creator-0.2.15.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/main.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/prompter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/src/llm_prompt_creator/__init__.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/src/llm_prompt_creator/prompt.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/LICENSE
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/README.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/pyproject.toml
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.14/PKG-INFO
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/main.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/prompter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/src/llm_prompt_creator/__init__.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/src/llm_prompt_creator/prompt.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/LICENSE
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/README.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/pyproject.toml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 llm_prompt_creator-0.2.15/PKG-INFO
```

### Comparing `llm_prompt_creator-0.2.14/main.py` & `llm_prompt_creator-0.2.15/main.py`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.14/prompter.py` & `llm_prompt_creator-0.2.15/prompter.py`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.14/src/llm_prompt_creator/prompt.py` & `llm_prompt_creator-0.2.15/src/llm_prompt_creator/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.14/LICENSE` & `llm_prompt_creator-0.2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_prompt_creator-0.2.14/README.md` & `llm_prompt_creator-0.2.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 To contribute, create a feature or fix branch (prepended with `feature_` or `fix_` respectively), commit your changes there and then create a pull request from your branch into `main`.
 
 We will review & (after approval) merge your git branch and then delete the remote branch on our github repo to limit left-over branches.
 
 ## Set Up
 
+> **Note**
+> Windows users may need to install the Visual Studio C++ Compiler to use this package
+
 Simple example usage:
 ```
 from llm_prompt_creator import prompt as PR
 dir = "<path to your java codebase directory>"
 
 # Chunk & store your codebase as tokenized chunks via javalang.
 # Defaults to store succesfully chunked files in "./chunks.json".
@@ -41,15 +44,15 @@
 """
 # PR.prompt(store, show_context=True)
 ```
 
 Following the example should yield a similar response to the below image 
 (subject to LLM model used and codebase):
 
-![](results/202306091608_fix_readme-and-misc-org.jpeg)]
+![](results/202306091608_fix_readme-and-misc-org.jpeg)
 
 ## TODO
 
 - [x] Refactoring across the board, particularly to reduce the number of called Python scripts.
 - [ ] Optimize chunker to allow larger codebase directories
 - [ ] Establish a standard way of calculating token limits.
 - [ ] Use token limits to dynamically adjust the amount of context and therefore the number of tokens used during a prompt/completion instance with OpenAI.
```

### Comparing `llm_prompt_creator-0.2.14/pyproject.toml` & `llm_prompt_creator-0.2.15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "archive/",
     "venv/",
     "*.json",
 ]
 
 [project]
 name = "llm_prompt_creator"
-version = "0.2.14"
+version = "0.2.15"
 authors = [
     {name="Chris Mills", email="cmills@breakfreesolutions.com"},
     {name="Zak Alford", email="zalford@breakfreesolutions.com"}
 ]
 description = "Takes a given directory and parses its contents to create a text vectorstore to be consumed in prompts for various LLM models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `llm_prompt_creator-0.2.14/PKG-INFO` & `llm_prompt_creator-0.2.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_prompt_creator
-Version: 0.2.14
+Version: 0.2.15
 Summary: Takes a given directory and parses its contents to create a text vectorstore to be consumed in prompts for various LLM models.
 Project-URL: Homepage, https://github.com/break-free/fineract-unit-tests-openai
 Project-URL: Issues, https://github.com/break-free/fineract-unit-tests-openai/issues
 Author-email: Chris Mills <cmills@breakfreesolutions.com>, Zak Alford <zalford@breakfreesolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,17 @@
 
 To contribute, create a feature or fix branch (prepended with `feature_` or `fix_` respectively), commit your changes there and then create a pull request from your branch into `main`.
 
 We will review & (after approval) merge your git branch and then delete the remote branch on our github repo to limit left-over branches.
 
 ## Set Up
 
+> **Note**
+> Windows users may need to install the Visual Studio C++ Compiler to use this package
+
 Simple example usage:
 ```
 from llm_prompt_creator import prompt as PR
 dir = "<path to your java codebase directory>"
 
 # Chunk & store your codebase as tokenized chunks via javalang.
 # Defaults to store succesfully chunked files in "./chunks.json".
@@ -61,15 +64,15 @@
 """
 # PR.prompt(store, show_context=True)
 ```
 
 Following the example should yield a similar response to the below image 
 (subject to LLM model used and codebase):
 
-![](results/202306091608_fix_readme-and-misc-org.jpeg)]
+![](results/202306091608_fix_readme-and-misc-org.jpeg)
 
 ## TODO
 
 - [x] Refactoring across the board, particularly to reduce the number of called Python scripts.
 - [ ] Optimize chunker to allow larger codebase directories
 - [ ] Establish a standard way of calculating token limits.
 - [ ] Use token limits to dynamically adjust the amount of context and therefore the number of tokens used during a prompt/completion instance with OpenAI.
```

