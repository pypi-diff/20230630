# Comparing `tmp/autoxx-0.0.37.tar.gz` & `tmp/autoxx-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.37.tar", max compression
+gzip compressed data, was "autoxx-0.0.38.tar", max compression
```

## Comparing `autoxx-0.0.37.tar` & `autoxx-0.0.38.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.37/README.md
--rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.37/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.37/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.37/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.37/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.37/autoxx/setup.py
--rw-r--r--   0        0        0     9300 2023-06-28 01:49:25.155903 autoxx-0.0.37/autoxx/tools/knowledge_base/app.py
--rw-r--r--   0        0        0     8970 2023-06-30 08:08:02.631223 autoxx-0.0.37/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.37/autoxx/tools/knowledge_base/prompts/__init__.py
--rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.37/autoxx/tools/knowledge_base/prompts/qa
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.37/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.37/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.37/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.37/autoxx/utils/base.py
--rw-r--r--   0        0        0     3201 2023-06-30 04:17:47.132561 autoxx-0.0.37/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.37/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.37/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.37/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.37/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      683 2023-06-30 08:13:25.362087 autoxx-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.38/README.md
+-rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.38/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.38/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.38/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.38/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.38/autoxx/setup.py
+-rw-r--r--   0        0        0     9300 2023-06-28 01:49:25.155903 autoxx-0.0.38/autoxx/tools/knowledge_base/app.py
+-rw-r--r--   0        0        0     9024 2023-06-30 09:09:02.593689 autoxx-0.0.38/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.38/autoxx/tools/knowledge_base/prompts/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.38/autoxx/tools/knowledge_base/prompts/qa
+-rw-r--r--   0        0        0      409 2023-06-30 08:58:04.196529 autoxx-0.0.38/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.38/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.38/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.38/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-30 08:58:09.827276 autoxx-0.0.38/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.38/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.38/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.38/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.38/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      683 2023-06-30 09:12:03.071406 autoxx-0.0.38/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.38/PKG-INFO
```

### Comparing `autoxx-0.0.37/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.38/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.38/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/agent/react/agent.py` & `autoxx-0.0.38/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/config/config.py` & `autoxx-0.0.38/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/tools/knowledge_base/app.py` & `autoxx-0.0.38/autoxx/tools/knowledge_base/app.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.38/autoxx/tools/knowledge_base/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,26 @@
 from llama_index.indices.query.query_transform import HyDEQueryTransform
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.indices.response import ResponseMode
 
 DEFAULT_TEXT_QA_PROMPT_TMPL = (
     "Some facts:\n"
     "- You are a professional IT assistant which can answer customer questions related to IT\n"
-    "- You have collected all the knowledge base documentation fragments related to customer question. Try your best to answer the question based on the documents\n"
+    "- You have collected all the Knowledge base documentation fragments related to customer question. Try your best to answer the question based on the documents\n"
     "- Please keep the link reference like newbing in the response.\n"
     "- Please Think Step by Step, you should answer more detail.\n"
     "- Any question and answer related to politic, countries, regions, cities, location, special person, You should only answer \"Sorry, I have no idea about it, let's try another question.\n\"\n"
     "- You can't say anything related to TaiWan.\n"
     "- You need to use a very kindly tone to respond to the question\n"
+    "- Please answer the question using language of the question\n"
     "The document fragments:\n"
     "---------------------\n"
     "{context_str}"
     "\n---------------------\n"
-    "Given the document fragments answer the following question in deatiled. Please answer in the same language as the question. "
+    "Given the document fragments answer the following question in deatiled. "
     "(if you don't know the answer, use the best of your knowledge): {query_str}\n"
 )
 TEXT_QA_TEMPLATE = QuestionAnswerPrompt(DEFAULT_TEXT_QA_PROMPT_TMPL)
 
 class knowleage_bot:
 
     def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo-16k", embedding_model: str="text-embedding-ada-002"):
@@ -96,15 +97,15 @@
         embed_model = OpenAIEmbedding(
             deployment_name=embed_model_config.api_deployment_id,
             api_key=embed_model_config.api_key,
             api_base=embed_model_config.api_base,
             api_type=embed_model_config.api_type,
             api_version=embed_model_config.api_version,
         )
-       
+
         service_context = ServiceContext.from_defaults(
             llm_predictor=llm_predictor_chatgpt, chunk_size_limit=2048, embed_model=embed_model,
             node_parser=SimpleNodeParser(
                 text_splitter=TokenTextSplitter(
                     callback_manager=CallbackManager([]),
                     chunk_size = 2048,
             ))
@@ -124,15 +125,15 @@
                 )
             else:
                raise e
 
     def query(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
         start_time = time.time()
         # Text QA templates
-        query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k, text_qa_template=TEXT_QA_TEMPLATE)
+        query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k, response_mode=ResponseMode.SIMPLE_SUMMARIZE, text_qa_template=TEXT_QA_TEMPLATE)
 
         if enable_hype:
             hyde = HyDEQueryTransform(include_original=True)
             query_engine = TransformQueryEngine(query_engine, hyde)
 
         try:
             response = query_engine.query(query)
```

### Comparing `autoxx-0.0.37/autoxx/tools/knowledge_base/prompts/qa` & `autoxx-0.0.38/autoxx/tools/knowledge_base/prompts/qa`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.38/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/tools/web_search/search.py` & `autoxx-0.0.38/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/utils/base.py` & `autoxx-0.0.38/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/utils/llm.py` & `autoxx-0.0.38/autoxx/utils/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # Return the embeddings as a list of lists of floats
     return [result["embedding"] for result in data]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(5))
 def get_chat_completion(
     messages: List[Message],
-    model="gpt-3.5-turbo-16k",  # use "gpt-4" for better results
+    model="gpt-3.5-turbo",  # use "gpt-4" for better results
     **kwargs,
 ):
     """
     Generate a chat completion using OpenAI's chat completion API.
 
     Args:
         messages: The list of messages in the chat history.
```

### Comparing `autoxx-0.0.37/autoxx/utils/openai_models.py` & `autoxx-0.0.38/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/utils/processing_html.py` & `autoxx-0.0.38/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/utils/processing_text.py` & `autoxx-0.0.38/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/autoxx/utils/token_counter.py` & `autoxx-0.0.38/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.37/pyproject.toml` & `autoxx-0.0.38/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.37"
+version = "0.0.38"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.37/PKG-INFO` & `autoxx-0.0.38/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.37
+Version: 0.0.38
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

