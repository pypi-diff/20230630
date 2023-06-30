# Comparing `tmp/talk_codebase-0.1.36.tar.gz` & `tmp/talk_codebase-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.36.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.37.tar", max compression
```

## Comparing `talk_codebase-0.1.36.tar` & `talk_codebase-0.1.37.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2874 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/README.md
--rw-r--r--   0        0        0      957 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/talk_codebase/__init__.py
--rw-r--r--   0        0        0     2898 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/talk_codebase/cli.py
--rw-r--r--   0        0        0     1702 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/talk_codebase/consts.py
--rw-r--r--   0        0        0     5492 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/talk_codebase/llm.py
--rw-r--r--   0        0        0     2256 2023-06-30 14:51:52.703908 talk_codebase-0.1.36/talk_codebase/utils.py
--rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0     2874 2023-06-30 15:05:43.638540 talk_codebase-0.1.37/README.md
+-rw-r--r--   0        0        0      957 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/cli.py
+-rw-r--r--   0        0        0     1702 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/consts.py
+-rw-r--r--   0        0        0     5455 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/llm.py
+-rw-r--r--   0        0        0     2256 2023-06-30 15:05:43.642541 talk_codebase-0.1.37/talk_codebase/utils.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 talk_codebase-0.1.37/PKG-INFO
```

### Comparing `talk_codebase-0.1.36/README.md` & `talk_codebase-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.36/pyproject.toml` & `talk_codebase-0.1.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.36"
+version = "0.1.37"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.36/talk_codebase/cli.py` & `talk_codebase-0.1.37/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.36/talk_codebase/consts.py` & `talk_codebase-0.1.37/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.36/talk_codebase/llm.py` & `talk_codebase-0.1.37/talk_codebase/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,18 +85,15 @@
         return llm
 
     def send_query(self, query):
         k = self.config.get("k")
         docs = self.embedding_search(query, k=int(k))
 
         content = "\n".join([f"content: \n```{s.page_content}```" for s in docs])
-        template = """Given the following content, your task is to answer the question. 
-        Content: {content}
-        Question: {question}
-        """
+        template = "Given the following content, your task is to answer the question.\nQuestion: {question}\n{content}"
 
         prompt = PromptTemplate(template=template, input_variables=["content", "question"]).partial(content=content)
         llm_chain = LLMChain(prompt=prompt, llm=self.llm)
 
         llm_chain.run(query)
 
         file_paths = [os.path.abspath(s.metadata["source"]) for s in docs]
```

### Comparing `talk_codebase-0.1.36/talk_codebase/utils.py` & `talk_codebase-0.1.37/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.36/PKG-INFO` & `talk_codebase-0.1.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.36
+Version: 0.1.37
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

