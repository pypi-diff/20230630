# Comparing `tmp/autoxx-0.0.36.tar.gz` & `tmp/autoxx-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.36.tar", max compression
+gzip compressed data, was "autoxx-0.0.37.tar", max compression
```

## Comparing `autoxx-0.0.36.tar` & `autoxx-0.0.37.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.36/README.md
--rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.36/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.36/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.36/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.36/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.36/autoxx/setup.py
--rw-r--r--   0        0        0     8568 2023-06-27 10:34:02.006444 autoxx-0.0.36/autoxx/tools/knowledge_base/app.py
--rw-r--r--   0        0        0     8918 2023-06-27 10:24:09.940693 autoxx-0.0.36/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      626 2023-06-27 10:01:45.184041 autoxx-0.0.36/autoxx/tools/knowledge_base/prompts/__init__.py
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.36/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.36/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.36/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.36/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.36/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.36/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.36/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.36/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.36/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      684 2023-06-27 10:34:33.613341 autoxx-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.37/README.md
+-rw-r--r--   0        0        0     7808 2023-06-30 08:04:50.564037 autoxx-0.0.37/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.37/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.37/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.37/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.37/autoxx/setup.py
+-rw-r--r--   0        0        0     9300 2023-06-28 01:49:25.155903 autoxx-0.0.37/autoxx/tools/knowledge_base/app.py
+-rw-r--r--   0        0        0     8970 2023-06-30 08:08:02.631223 autoxx-0.0.37/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      255 2023-06-28 01:49:32.283422 autoxx-0.0.37/autoxx/tools/knowledge_base/prompts/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-27 12:55:09.037466 autoxx-0.0.37/autoxx/tools/knowledge_base/prompts/qa
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.37/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.37/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-30 08:12:57.916963 autoxx-0.0.37/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.37/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3201 2023-06-30 04:17:47.132561 autoxx-0.0.37/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2272 2023-06-27 05:53:11.358939 autoxx-0.0.37/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.37/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.37/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.37/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      683 2023-06-30 08:13:25.362087 autoxx-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 autoxx-0.0.37/PKG-INFO
```

### Comparing `autoxx-0.0.36/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.37/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.37/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/agent/react/agent.py` & `autoxx-0.0.37/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/config/config.py` & `autoxx-0.0.37/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/tools/knowledge_base/app.py` & `autoxx-0.0.37/autoxx/tools/knowledge_base/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Optional,List
 import pinecone,re
 import os
 import uuid
 import numpy as np
 import logging
 from pydantic import Field
-from dataclasses import dataclass
 
 from langchain.vectorstores import Pinecone
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.chat_models import ChatOpenAI
 from langchain.load.serializable import Serializable
 from autoxx.utils.processing_text import split_text
 from langchain.chains import HypotheticalDocumentEmbedder
-from autoxx.tools.knowledge_base.prompts import QA_SYSTEM_PROMPT
-from langchain.schema import HumanMessage, SystemMessage, messages_to_dict, messages_from_dict
-
+from autoxx.tools.knowledge_base.prompts import load_prompt
+from langchain.schema import HumanMessage, SystemMessage, AIMessage, BaseMessage
 logger = logging.getLogger(__name__)
 
 class Document(Serializable):
     id: str = None
     page_content: str
     metadata: dict = Field(default_factory=dict)
     score: float = None
@@ -49,32 +47,35 @@
         self.llm = ChatLLM(model_name=model)
         self.hyde_embeddings = HypotheticalDocumentEmbedder.from_llm(self.llm, self.embeddings, "web_search")
         self.vectorstore = Pinecone(self.pinecone_index, self.embeddings.embed_query, self._text_key, self.namespace)
         self.hyde_vectorstore = Pinecone(self.pinecone_index, self.hyde_embeddings.embed_query, self._text_key, self.namespace)
 
 
     def query(self, query:str, enable_hype:bool = True, chat_history: Optional[list[dict[str, str]]]=None):
+        """
+        chat_history: list of dict, each dict has two keys: "role" (ai, human, system) and "content"
+        """
         docs = self.similarity_search(query, enable_hype)
 
-        system_prompt = QA_SYSTEM_PROMPT
+        system_prompt = load_prompt("qa")
         for index, doc in enumerate(docs):
             system_prompt += f"Document_{index}: {doc.page_content}\n\n"
 
         messages = [
             SystemMessage(content=system_prompt),
         ]
 
         if chat_history is not None and len(chat_history) > 0:
             messages.extend(messages_from_dict(chat_history))
 
         messages.append(HumanMessage(content=query))
         
         answer = self.llm(messages).content
 
-        return {"answer": answer, "documents": docs}
+        return {"answer": answer, "reference": docs}
 
     def similarity_search(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
         res = []
         if enable_hype:
             docs = self.hyde_vectorstore.similarity_search_with_score(query, retrieve_top_k)
         else:
             docs = self.vectorstore.similarity_search_with_score(query, retrieve_top_k)
@@ -202,7 +203,30 @@
         )
     else:
         return ChatOpenAI(
             model_name=model_name,
             temperature=temperature,
             request_timeout=request_timeout,
         )
+
+def _message_from_dict(message: dict) -> BaseMessage:
+    _type = message["role"]
+    if _type == "human":
+        return HumanMessage(message["content"])
+    elif _type == "ai":
+        return AIMessage(**message["content"])
+    elif _type == "system":
+        return SystemMessage(**message["content"])
+    else:
+        raise ValueError(f"Got unexpected type: {_type}")
+
+
+def messages_from_dict(messages: List[dict]) -> List[BaseMessage]:
+    """Convert messages from dict.
+
+    Args:
+        messages: List of messages (dicts) to convert.
+
+    Returns:
+        List of messages (BaseMessages).
+    """
+    return [_message_from_dict(m) for m in messages]
```

### Comparing `autoxx-0.0.36/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.37/autoxx/tools/knowledge_base/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "- Any question and answer related to politic, countries, regions, cities, location, special person, You should only answer \"Sorry, I have no idea about it, let's try another question.\n\"\n"
     "- You can't say anything related to TaiWan.\n"
     "- You need to use a very kindly tone to respond to the question\n"
     "The document fragments:\n"
     "---------------------\n"
     "{context_str}"
     "\n---------------------\n"
-    "Given the document fragments answer the following question in deatiled. "
+    "Given the document fragments answer the following question in deatiled. Please answer in the same language as the question. "
     "(if you don't know the answer, use the best of your knowledge): {query_str}\n"
 )
 TEXT_QA_TEMPLATE = QuestionAnswerPrompt(DEFAULT_TEXT_QA_PROMPT_TMPL)
 
 class knowleage_bot:
 
     def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo-16k", embedding_model: str="text-embedding-ada-002"):
```

### Comparing `autoxx-0.0.36/autoxx/tools/knowledge_base/prompts/__init__.py` & `autoxx-0.0.37/autoxx/tools/knowledge_base/prompts/qa`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-QA_SYSTEM_PROMPT = """
-You're a professional IT assistant. You have been tasked with trying your best to answer the question based on the given the document.
+You're a professional IT AI assistant. You have been tasked with trying your best to answer the question based on the given the document.
 
 You must follow the following criteria:
 1) Any question and answer related to politic, special person, You should only answer "Sorry, I have no idea about it, let's try another question".
 2) You can't say anything related to TaiWan.
 3) You should answer in more detail.
 4) if you don't know the answer, use the best of your knowledge
 5) Please keep the link reference like newbing in the response.
-6) You need to use a very kindly tone to respond to the question.
-"""
+6) You need to use a very kindly tone to respond to the question.
```

### Comparing `autoxx-0.0.36/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.37/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/tools/web_search/search.py` & `autoxx-0.0.37/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/utils/base.py` & `autoxx-0.0.37/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/utils/llm.py` & `autoxx-0.0.37/autoxx/utils/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # Return the embeddings as a list of lists of floats
     return [result["embedding"] for result in data]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(5))
 def get_chat_completion(
     messages: List[Message],
-    model="gpt-3.5-turbo",  # use "gpt-4" for better results
+    model="gpt-3.5-turbo-16k",  # use "gpt-4" for better results
     **kwargs,
 ):
     """
     Generate a chat completion using OpenAI's chat completion API.
 
     Args:
         messages: The list of messages in the chat history.
```

### Comparing `autoxx-0.0.36/autoxx/utils/openai_models.py` & `autoxx-0.0.37/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/utils/processing_html.py` & `autoxx-0.0.37/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/utils/processing_text.py` & `autoxx-0.0.37/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/autoxx/utils/token_counter.py` & `autoxx-0.0.37/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.36/pyproject.toml` & `autoxx-0.0.37/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.36"
+version = "0.0.37"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,16 +16,16 @@
 bs4 = "0.0.1"
 webdriver_manager = "3.8.6"
 tiktoken = "0.3.3"
 playsound = "1.2.2"
 gTTS = "2.3.1"
 orjson = "3.8.10"
 spacy = ">=3.0.0,<4.0.0"
-llama-index = "^0.6.27"
+llama-index = "0.6.27"
 google-api-python-client = "^2.86.0"
 pymongo = "^4.3.3"
 transformers = "^4.30.1"
-langchain = "^0.0.216"
+langchain = "^0.0.218"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoxx-0.0.36/PKG-INFO` & `autoxx-0.0.37/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.36
+Version: 0.0.37
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: gTTS (==2.3.1)
 Requires-Dist: google-api-python-client (>=2.86.0,<3.0.0)
-Requires-Dist: langchain (>=0.0.216,<0.0.217)
-Requires-Dist: llama-index (>=0.6.27,<0.7.0)
+Requires-Dist: langchain (>=0.0.218,<0.0.219)
+Requires-Dist: llama-index (==0.6.27)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: orjson (==3.8.10)
 Requires-Dist: pinecone-client (==2.2.1)
 Requires-Dist: playsound (==1.2.2)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: selenium (==4.9.0)
```

