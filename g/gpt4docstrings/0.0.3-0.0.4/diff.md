# Comparing `tmp/gpt4docstrings-0.0.3.tar.gz` & `tmp/gpt4docstrings-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4docstrings-0.0.3.tar", max compression
+gzip compressed data, was "gpt4docstrings-0.0.4.tar", max compression
```

## Comparing `gpt4docstrings-0.0.3.tar` & `gpt4docstrings-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-06-30 08:34:23.906921 gpt4docstrings-0.0.3/LICENSE
--rw-r--r--   0        0        0     2830 2023-06-30 08:34:23.906921 gpt4docstrings-0.0.3/README.md
--rw-r--r--   0        0        0     1987 2023-06-30 08:34:38.246877 gpt4docstrings-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       83 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/__init__.py
--rw-r--r--   0        0        0       75 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/__main__.py
--rw-r--r--   0        0        0     1558 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/cli.py
--rw-r--r--   0        0        0       67 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/docstrings_generators/__init__.py
--rw-r--r--   0        0        0     4877 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
--rw-r--r--   0        0        0     4084 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/generate_docstrings.py
--rw-r--r--   0        0        0     1591 2023-06-30 08:34:23.918921 gpt4docstrings-0.0.3/src/gpt4docstrings/utils.py
--rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-30 14:19:27.830981 gpt4docstrings-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2830 2023-06-30 14:19:27.830981 gpt4docstrings-0.0.4/README.md
+-rw-r--r--   0        0        0     1987 2023-06-30 14:19:43.306952 gpt4docstrings-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/__main__.py
+-rw-r--r--   0        0        0     1558 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/cli.py
+-rw-r--r--   0        0        0       67 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/docstrings_generators/__init__.py
+-rw-r--r--   0        0        0     4718 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py
+-rw-r--r--   0        0        0     4084 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/generate_docstrings.py
+-rw-r--r--   0        0        0     1591 2023-06-30 14:19:27.838981 gpt4docstrings-0.0.4/src/gpt4docstrings/utils.py
+-rw-r--r--   0        0        0     3911 1970-01-01 00:00:00.000000 gpt4docstrings-0.0.4/PKG-INFO
```

### Comparing `gpt4docstrings-0.0.3/LICENSE` & `gpt4docstrings-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.3/README.md` & `gpt4docstrings-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.3/pyproject.toml` & `gpt4docstrings-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt4docstrings"
-version = "0.0.3"
+version = "0.0.4"
 description = "gpt4docstrings"
 authors = ["Miguel Otero Pedrido <miguel.otero.pedrido.1993@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 repository = "https://github.com/MichaelisTrofficus/gpt4docstrings"
 documentation = "https://gpt4docstrings.readthedocs.io"
```

### Comparing `gpt4docstrings-0.0.3/src/gpt4docstrings/cli.py` & `gpt4docstrings-0.0.4/src/gpt4docstrings/cli.py`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.3/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py` & `gpt4docstrings-0.0.4/src/gpt4docstrings/docstrings_generators/openai_chatgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,31 +36,29 @@
 
         Args:
             prompt: ChatGPT prompt
 
         Returns:
             ChatGPT response
         """
-        result = ""
-        for _ in range(0, 5):
-            while True:
-                try:
-                    messages = [{"role": "user", "content": prompt}]
-                    response = openai.ChatCompletion.create(
-                        model=self.model,
-                        messages=messages,
-                        temperature=0,  # TODO: Let user configure temperature??
-                    )
-                    result = response.choices[0].message["content"]
-                except openai.error.APIError as e:
-                    print(f"OpenAI API returned an API Error: {e}")
-                    time.sleep(2)
-                    continue
-                break
-        return result
+        max_retries = 5
+        retries = 0
+        messages = [{"role": "user", "content": prompt}]
+
+        while retries < max_retries:
+            try:
+                response = openai.ChatCompletion.create(
+                    model=self.model,
+                    messages=messages,
+                    temperature=0,  # TODO: Let user configure temperature??
+                )
+                return response.choices[0].message["content"]
+            except openai.error.APIError:
+                time.sleep(5)
+                retries += 1
 
     def generate_function_docstring(self, source: str) -> dict:
         """
         Generates docstring for Python function.
 
         Args:
             source: The source code of the Python method
```

### Comparing `gpt4docstrings-0.0.3/src/gpt4docstrings/generate_docstrings.py` & `gpt4docstrings-0.0.4/src/gpt4docstrings/generate_docstrings.py`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.3/src/gpt4docstrings/utils.py` & `gpt4docstrings-0.0.4/src/gpt4docstrings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt4docstrings-0.0.3/PKG-INFO` & `gpt4docstrings-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4docstrings
-Version: 0.0.3
+Version: 0.0.4
 Summary: gpt4docstrings
 Home-page: https://github.com/MichaelisTrofficus/gpt4docstrings
 License: MIT
 Author: Miguel Otero Pedrido
 Author-email: miguel.otero.pedrido.1993@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 1 - Planning
```

