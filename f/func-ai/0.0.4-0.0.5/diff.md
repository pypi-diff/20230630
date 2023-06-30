# Comparing `tmp/func_ai-0.0.4.tar.gz` & `tmp/func_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.4.tar", max compression
+gzip compressed data, was "func_ai-0.0.5.tar", max compression
```

## Comparing `func_ai-0.0.4.tar` & `func_ai-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.4/LICENSE
--rw-r--r--   0        0        0     2907 2023-06-30 05:05:30.775581 func_ai-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.4/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.4/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.4/func_ai/utils/__init__.py
--rw-r--r--   0        0        0    10240 2023-06-29 18:00:21.930012 func_ai-0.0.4/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0     5701 2023-06-30 05:04:37.316662 func_ai-0.0.4/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3392 2023-06-29 09:04:33.935006 func_ai-0.0.4/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-06-29 15:06:55.283947 func_ai-0.0.4/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      889 2023-06-30 03:07:29.394998 func_ai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3940 1970-01-01 00:00:00.000000 func_ai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3375 2023-06-30 11:34:34.818711 func_ai-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.5/func_ai/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.5/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.5/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0     4515 2023-06-30 11:28:00.351251 func_ai-0.0.5/func_ai/utils/jinja_template_functions.py
+-rw-r--r--   0        0        0    10241 2023-06-30 09:42:46.148402 func_ai-0.0.5/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0     5701 2023-06-30 06:36:30.640188 func_ai-0.0.5/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3392 2023-06-30 06:36:30.641465 func_ai-0.0.5/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-06-30 06:36:30.641834 func_ai-0.0.5/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      907 2023-06-30 11:32:21.641350 func_ai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 func_ai-0.0.5/PKG-INFO
```

### Comparing `func_ai-0.0.4/LICENSE` & `func_ai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.4/README.md` & `func_ai-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -85,12 +85,30 @@
 2023-06-30 07:57:40,306 - urllib3.connectionpool - DEBUG - https://petstore.swagger.io:443 "GET /v2/pet/10 HTTP/1.1" 200 None
 {"id":10,"category":{"id":10,"name":"sample string"},"name":"doggie","photoUrls":[],"tags":[],"status":"pending"}
 """
 ```
 
 > Note: the above is pretty naive implementation of OpenAPI parsing and calling. It is not production ready.
 
+### Jinja2 Templating
+
+```python
+from dotenv import load_dotenv
+from func_ai.utils.jinja_template_functions import JinjaOpenAITemplateFunction
+from func_ai.utils.llm_tools import OpenAIInterface
+load_dotenv()
+ji = JinjaOpenAITemplateFunction.from_string_template("Name: {{ NAME }} \n Age: {{ AGE }}", OpenAIInterface())
+resp = ji.render_from_prompt("John is 20 years old")
+assert "Name: John" in resp
+assert "Age: 20" in resp
+# prints
+"""
+Name: John 
+Age: 20
+"""
+```
+
 ## Inspiration
 
 - https://github.com/jxnl/openai_function_call
 - https://github.com/rizerphe/openai-functions
 - https://github.com/aurelio-labs/funkagent
```

### Comparing `func_ai-0.0.4/func_ai/function_indexer.py` & `func_ai-0.0.5/func_ai/function_indexer.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.4/func_ai/utils/llm_tools.py` & `func_ai-0.0.5/func_ai/utils/llm_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 class OpenAIConversationStore(ConversationStore):
 
     def add_message(self, message: Any):
         self.conversation.append(message)
 
     def add_system_message(self, message: str):
         # remove any existing system messages
-        self.conversation = [x for x in self.conversation if "system" not in x.keys()]
-        self.conversation.append({"role": "system", "content": message})
+        self.conversation = [x for x in self.conversation if x['role'] != 'system']
+        self.conversation.insert(0, {"role": "system", "content": message})
 
 
 class LLMInterface(BaseModel):
     """
     Interface for interacting with the Language Learning Model
 
     """
@@ -204,14 +204,15 @@
                 "total_tokens": 0
             }
         self.usage[model]["prompt_tokens"] += api_response['usage']['prompt_tokens']
         self.usage[model]["completion_tokens"] += api_response['usage']['completion_tokens']
         self.usage[model]["total_tokens"] += api_response['usage']['total_tokens']
 
 
+
 class OpenAISchema(BaseModel):
     @classmethod
     @property
     def openai_schema(cls):
         schema = cls.schema()
 
         return {
```

### Comparing `func_ai-0.0.4/func_ai/utils/openapi_function_parser.py` & `func_ai-0.0.5/func_ai/utils/openapi_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.4/func_ai/utils/py_function_parser.py` & `func_ai-0.0.5/func_ai/utils/py_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.4/func_ai/workflow_creator.py` & `func_ai-0.0.5/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.4/pyproject.toml` & `func_ai-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.4"
+version = "0.0.5"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
@@ -19,14 +19,15 @@
 chromadb = "^0.3.26"
 python-ulid = "^1.1.0"
 fastapi = "^0.98.0"
 pyyaml = "^6.0"
 jsonschema = "^4.17.3"
 python-dotenv = "^1.0.0"
 tenacity = "^8.2.2"
+jinja2 = "^3.1.2"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-env = "^0.8.2"
 pytest-html = "^3.2.0"
 pytest-metadata = "^3.0.0"
```

### Comparing `func_ai-0.0.4/PKG-INFO` & `func_ai-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: func-ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Functional Catalog - OpenAI functions on steriods
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.26,<0.4.0)
 Requires-Dist: fastapi (>=0.98.0,<0.99.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
@@ -111,12 +112,30 @@
 2023-06-30 07:57:40,306 - urllib3.connectionpool - DEBUG - https://petstore.swagger.io:443 "GET /v2/pet/10 HTTP/1.1" 200 None
 {"id":10,"category":{"id":10,"name":"sample string"},"name":"doggie","photoUrls":[],"tags":[],"status":"pending"}
 """
 ```
 
 > Note: the above is pretty naive implementation of OpenAPI parsing and calling. It is not production ready.
 
+### Jinja2 Templating
+
+```python
+from dotenv import load_dotenv
+from func_ai.utils.jinja_template_functions import JinjaOpenAITemplateFunction
+from func_ai.utils.llm_tools import OpenAIInterface
+load_dotenv()
+ji = JinjaOpenAITemplateFunction.from_string_template("Name: {{ NAME }} \n Age: {{ AGE }}", OpenAIInterface())
+resp = ji.render_from_prompt("John is 20 years old")
+assert "Name: John" in resp
+assert "Age: 20" in resp
+# prints
+"""
+Name: John 
+Age: 20
+"""
+```
+
 ## Inspiration
 
 - https://github.com/jxnl/openai_function_call
 - https://github.com/rizerphe/openai-functions
 - https://github.com/aurelio-labs/funkagent
```

