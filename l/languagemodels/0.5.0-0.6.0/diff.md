# Comparing `tmp/languagemodels-0.5.0.tar.gz` & `tmp/languagemodels-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.5.0.tar", last modified: Sat Jun 17 20:35:31 2023, max compression
+gzip compressed data, was "languagemodels-0.6.0.tar", last modified: Fri Jun 30 03:21:39 2023, max compression
```

## Comparing `languagemodels-0.5.0.tar` & `languagemodels-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 20:35:31.764542 languagemodels-0.5.0/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8930 2023-06-17 20:35:31.764542 languagemodels-0.5.0/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 20:35:31.764542 languagemodels-0.5.0/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10532 2023-06-17 20:12:04.000000 languagemodels-0.5.0/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4577 2023-06-17 01:38:19.000000 languagemodels-0.5.0/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7105 2023-06-17 19:46:56.000000 languagemodels-0.5.0/languagemodels/inference.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4078 2023-06-17 01:38:19.000000 languagemodels-0.5.0/languagemodels/models.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-17 20:35:31.764542 languagemodels-0.5.0/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8930 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      306 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       61 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-17 20:35:31.000000 languagemodels-0.5.0/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-17 20:35:31.764542 languagemodels-0.5.0/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      800 2023-06-17 20:06:30.000000 languagemodels-0.5.0/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-30 03:21:39.589745 languagemodels-0.6.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9369 2023-06-30 03:21:39.585744 languagemodels-0.6.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-30 03:21:39.585744 languagemodels-0.6.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10679 2023-06-30 03:08:32.000000 languagemodels-0.6.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     5811 2023-06-28 20:37:56.000000 languagemodels-0.6.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7919 2023-06-30 03:08:32.000000 languagemodels-0.6.0/languagemodels/inference.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8340 2023-06-30 03:08:32.000000 languagemodels-0.6.0/languagemodels/models.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-30 03:21:39.585744 languagemodels-0.6.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9369 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      306 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       61 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-30 03:21:39.589745 languagemodels-0.6.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      800 2023-06-30 03:19:50.000000 languagemodels-0.6.0/setup.py
```

### Comparing `languagemodels-0.5.0/PKG-INFO` & `languagemodels-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -70,15 +70,15 @@
         >>> lm.do("What is the capital of France?")
         'Paris.'
         ```
         
         ### Chat
         
         ```python
-        >>> chat('''
+        >>> lm.chat('''
         ...      System: Respond as a helpful assistant.
         ...
         ...      User: What time is it?
         ...
         ...      Assistant:
         ...      ''')
         'I'm sorry, but as an AI language model, I don't have access to real-time information. Please provide me with the specific time you are asking for so that I can assist you better.'
@@ -100,15 +100,15 @@
         >>> lm.get_date()
         'Friday, May 12, 2023 at 09:27AM'
         ```
         
         Here's an example showing how this can be used (compare to previous chat example):
         
         ```python
-        >>> chat(f'''
+        >>> lm.chat(f'''
         ...      System: Respond as a helpful assistant. It is {lm.get_date()}
         ...
         ...      User: What time is it?
         ...
         ...      Assistant:
         ...      ''')
         'It is currently Wednesday, June 07, 2023 at 12:53PM.'
@@ -127,23 +127,23 @@
         'Mars is a planet'
         ```
         
         This can also be used to get a blend of context from stored documents:
         
         ```python
         >>> import languagemodels as lm
-        
-        >>> lm.store_doc(lm.get_wiki("Python"))
-        >>> lm.store_doc(lm.get_wiki("C language"))
-        >>> lm.store_doc(lm.get_wiki("Javascript"))
-        >>> lm.store_doc(lm.get_wiki("Fortran"))
+        >>> lm.store_doc(lm.get_wiki("Python"), "Python")
+        >>> lm.store_doc(lm.get_wiki("C language"), "C")
+        >>> lm.store_doc(lm.get_wiki("Javascript"), "Javascript")
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
-        'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
+        'Python: It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.
+        
+        C: It was designed to be compiled to provide low-level access to memory and language constructs that map efficiently to machine instructions, all with minimal runtime support.
         
-        often incorporating third-party libraries. All major web browsers have a dedicated JavaScript engine to execute the code on users\' devices. JavaScript is a high-level, often just-in-time compiled language that conforms to the ECMAScript standard. It has dynamic typing, prototype'
+        C: The book The C Programming Language, co-authored by the original language designer, served for many years as the de facto standard for the language.'
         ```
         
         ### Performance
         
         The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
         
         The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
@@ -156,26 +156,37 @@
         4.0
         >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
         'I have 2 apples left.'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
-        Advanced Usage
+        Commercial Use
         --------------
         
-        This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face. For integrating language models in more complex ways, [LangChain](https://github.com/hwchase17/langchain) or [guidance](https://github.com/microsoft/guidance) may be helpful.
+        This package itself is licensed for commerical use, but the models used may not be compatible with commercial use. In order to use this package commercially, you may want to filter models by their license type using the `require_model_license` function.
+        
+        ```python
+        >>> import languagemodels as lm
+        >>> lm.do("What is your favorite animal.")
+        >>> "As an AI language model, I don't have preferences or emotions."
+        >>> lm.require_model_license("apache.*|mit")
+        >>> lm.do("What is your favorite animal.")
+        'Lion.'
+        ```
+        
+        The commercially-licensed models may not perform as well as the default models. It is recommended to confirm that the models used do meet the licensing requirements for your software.
         
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
-        - CLI Chatbot (see examples/chat.py)
-        - Streamlit chatbot (see examples/streamlitchat.py)
+        - CLI Chatbot (see [examples/chat.py](examples/chat.py))
+        - Streamlit chatbot (see [examples/streamlitchat.py](examples/streamlitchat.py))
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search over documents
         - Document question answering
```

### Comparing `languagemodels-0.5.0/languagemodels/__init__.py` & `languagemodels-0.6.0/languagemodels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import requests
 import datetime
 import json
 
-from languagemodels.models import set_max_ram
-from languagemodels.inference import generate_instruct, parse_chat, list_tokens
+from languagemodels.models import set_max_ram, require_model_license
+from languagemodels.inference import (
+    generate_instruct,
+    rank_instruct,
+    parse_chat,
+    list_tokens,
+)
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
 
 
 def complete(prompt: str) -> str:
     """Provide one completion for a given open-ended prompt
@@ -201,31 +206,32 @@
     'positive'
     >>> classify("That movie was terrible.","positive","negative")
     'negative'
     >>> classify("The submarine is diving", "ocean", "land")
     'ocean'
     """
 
-    result = generate_instruct(
-        f"Classify as {label1} or {label2}: {doc}\n\nClassification:", max_tokens=5
+    results = rank_instruct(
+        f"Classify as {label1} or {label2}: {doc}\n\nClassification:", [label1, label2]
     )
 
-    return result.lower().rstrip(".")
+    return results[0]
 
 
-def store_doc(doc: str) -> None:
+def store_doc(doc: str, name: str = "") -> None:
     """Store document for later retrieval
 
     :param doc: A plain text document to store.
+    :param name: Optional name for the document. This is used as a chunk prefix.
 
     Examples:
 
     >>> store_doc("The sky is blue.")
     """
-    docs.store(doc)
+    docs.store(doc, name)
 
 
 def load_doc(query: str) -> str:
     """Load a matching document
 
     A single document that best matches `query` will be returned.
```

### Comparing `languagemodels-0.5.0/languagemodels/inference.py` & `languagemodels-0.6.0/languagemodels/inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,42 @@
     )
 
     output_tokens = results[0].hypotheses[0]
 
     return tokenizer.DecodePieces(output_tokens)
 
 
+def rank_instruct(input, targets):
+    """Sorts a list of targets by their probabilities
+
+    >>> rank_instruct("I love python", ['positive', 'negative'])
+    ['positive', 'negative']
+
+    >>> rank_instruct("Homework is the worst", ['positive', 'negative', 'neutral'])[0]
+    'negative'
+
+    >>> rank_instruct("The wizard raised their wand", ['fantasy', 'documentary'])
+    ['fantasy', 'documentary']
+    """
+    tokenizer, model = get_model("instruct")
+
+    input_tokens = tokenizer.EncodeAsPieces(input) + ["</s>"]
+
+    scores = model.score_batch(
+        [input_tokens] * len(targets),
+        target=[tokenizer.EncodeAsPieces(t) for t in targets],
+    )
+
+    logprobs = [sum(r.log_probs) for r in scores]
+
+    results = sorted(zip(targets, logprobs), key=lambda r: -r[1])
+
+    return [r[0] for r in results]
+
+
 def parse_chat(prompt):
     """Converts a chat prompt using special tokens to a plain-text prompt
 
     This is useful for prompting generic models that have not been fine-tuned
     for chat using specialized tokens.
 
     >>> parse_chat('User: What time is it?')
```

### Comparing `languagemodels-0.5.0/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.6.0/languagemodels.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -70,15 +70,15 @@
         >>> lm.do("What is the capital of France?")
         'Paris.'
         ```
         
         ### Chat
         
         ```python
-        >>> chat('''
+        >>> lm.chat('''
         ...      System: Respond as a helpful assistant.
         ...
         ...      User: What time is it?
         ...
         ...      Assistant:
         ...      ''')
         'I'm sorry, but as an AI language model, I don't have access to real-time information. Please provide me with the specific time you are asking for so that I can assist you better.'
@@ -100,15 +100,15 @@
         >>> lm.get_date()
         'Friday, May 12, 2023 at 09:27AM'
         ```
         
         Here's an example showing how this can be used (compare to previous chat example):
         
         ```python
-        >>> chat(f'''
+        >>> lm.chat(f'''
         ...      System: Respond as a helpful assistant. It is {lm.get_date()}
         ...
         ...      User: What time is it?
         ...
         ...      Assistant:
         ...      ''')
         'It is currently Wednesday, June 07, 2023 at 12:53PM.'
@@ -127,23 +127,23 @@
         'Mars is a planet'
         ```
         
         This can also be used to get a blend of context from stored documents:
         
         ```python
         >>> import languagemodels as lm
-        
-        >>> lm.store_doc(lm.get_wiki("Python"))
-        >>> lm.store_doc(lm.get_wiki("C language"))
-        >>> lm.store_doc(lm.get_wiki("Javascript"))
-        >>> lm.store_doc(lm.get_wiki("Fortran"))
+        >>> lm.store_doc(lm.get_wiki("Python"), "Python")
+        >>> lm.store_doc(lm.get_wiki("C language"), "C")
+        >>> lm.store_doc(lm.get_wiki("Javascript"), "Javascript")
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
-        'multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language
+        'Python: It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.
+        
+        C: It was designed to be compiled to provide low-level access to memory and language constructs that map efficiently to machine instructions, all with minimal runtime support.
         
-        often incorporating third-party libraries. All major web browsers have a dedicated JavaScript engine to execute the code on users\' devices. JavaScript is a high-level, often just-in-time compiled language that conforms to the ECMAScript standard. It has dynamic typing, prototype'
+        C: The book The C Programming Language, co-authored by the original language designer, served for many years as the de facto standard for the language.'
         ```
         
         ### Performance
         
         The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
         
         The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
@@ -156,26 +156,37 @@
         4.0
         >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
         'I have 2 apples left.'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
-        Advanced Usage
+        Commercial Use
         --------------
         
-        This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face. For integrating language models in more complex ways, [LangChain](https://github.com/hwchase17/langchain) or [guidance](https://github.com/microsoft/guidance) may be helpful.
+        This package itself is licensed for commerical use, but the models used may not be compatible with commercial use. In order to use this package commercially, you may want to filter models by their license type using the `require_model_license` function.
+        
+        ```python
+        >>> import languagemodels as lm
+        >>> lm.do("What is your favorite animal.")
+        >>> "As an AI language model, I don't have preferences or emotions."
+        >>> lm.require_model_license("apache.*|mit")
+        >>> lm.do("What is your favorite animal.")
+        'Lion.'
+        ```
+        
+        The commercially-licensed models may not perform as well as the default models. It is recommended to confirm that the models used do meet the licensing requirements for your software.
         
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
-        - CLI Chatbot (see examples/chat.py)
-        - Streamlit chatbot (see examples/streamlitchat.py)
+        - CLI Chatbot (see [examples/chat.py](examples/chat.py))
+        - Streamlit chatbot (see [examples/streamlitchat.py](examples/streamlitchat.py))
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search over documents
         - Document question answering
```

### Comparing `languagemodels-0.5.0/setup.py` & `languagemodels-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.5.0",
+    version="0.6.0",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

