# Comparing `tmp/llmreflect-0.1.2.tar.gz` & `tmp/llmreflect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.1.2.tar", max compression
+gzip compressed data, was "llmreflect-0.1.3.tar", max compression
```

## Comparing `llmreflect-0.1.2.tar` & `llmreflect-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       14 2023-06-29 15:41:31.549916 llmreflect-0.1.2/README.md
--rw-r--r--   0        0        0     1278 2023-06-29 23:26:08.859984 llmreflect-0.1.2/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     1970 2023-06-29 23:24:38.298808 llmreflect-0.1.2/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3658 2023-06-29 23:24:40.358744 llmreflect-0.1.2/llmreflect/Agents/PostgressqlAgent.py
--rw-r--r--   0        0        0     1807 2023-06-29 23:26:20.583618 llmreflect-0.1.2/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-06-29 23:26:07.928012 llmreflect-0.1.2/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     5547 2023-06-29 23:26:59.422407 llmreflect-0.1.2/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0     1252 2023-06-29 23:24:42.494677 llmreflect-0.1.2/llmreflect/Prompt/GradingPrompt.py
--rw-r--r--   0        0        0     1268 2023-06-29 23:24:44.234623 llmreflect-0.1.2/llmreflect/Prompt/QuestionPrompt.py
--rw-r--r--   0        0        0        0 2023-06-09 21:36:11.820430 llmreflect-0.1.2/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-28 19:50:41.640334 llmreflect-0.1.2/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     4749 2023-06-16 20:16:52.801762 llmreflect-0.1.2/llmreflect/Prompt/promptbase/postgressql.json
--rw-r--r--   0        0        0     3632 2023-06-23 14:57:20.254338 llmreflect-0.1.2/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0      743 2023-06-28 21:41:26.342726 llmreflect-0.1.2/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4064 2023-06-29 23:24:45.810573 llmreflect-0.1.2/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-06-13 18:20:17.809156 llmreflect-0.1.2/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 18:20:19.397105 llmreflect-0.1.2/llmreflect/Scripts/__init__.py
--rw-r--r--   0        0        0      777 2023-06-29 23:24:47.246529 llmreflect-0.1.2/llmreflect/Scripts/database_answer_example.py
--rw-r--r--   0        0        0      777 2023-06-29 23:24:50.606424 llmreflect-0.1.2/llmreflect/Scripts/database_question_example.py
--rw-r--r--   0        0        0      875 2023-06-29 23:24:48.966475 llmreflect-0.1.2/llmreflect/Scripts/database_sql_grading_example.py
--rw-r--r--   0        0        0        0 2023-06-09 21:36:11.820430 llmreflect-0.1.2/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-06-29 14:41:23.216485 llmreflect-0.1.2/llmreflect/Utils/database.py
--rw-r--r--   0        0        0      305 2023-06-28 20:22:46.484992 llmreflect-0.1.2/llmreflect/Utils/message.py
--rw-r--r--   0        0        0        0 2023-06-09 21:36:11.820430 llmreflect-0.1.2/llmreflect/__init__.py
--rw-r--r--   0        0        0      443 2023-06-29 23:25:41.656832 llmreflect-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 llmreflect-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-06-30 19:23:10.035312 llmreflect-0.1.3/README.md
+-rw-r--r--   0        0        0     1278 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     1970 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3658 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Agents/PostgressqlAgent.py
+-rw-r--r--   0        0        0     1807 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     5547 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0     1252 2023-06-30 19:23:10.035312 llmreflect-0.1.3/llmreflect/Prompt/GradingPrompt.py
+-rw-r--r--   0        0        0     1268 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Prompt/QuestionPrompt.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Prompt/promptbase/gradingpostgresql.json
+-rw-r--r--   0        0        0     4749 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Prompt/promptbase/postgressql.json
+-rw-r--r--   0        0        0     3632 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Prompt/promptbase/questionpostgresql.json
+-rw-r--r--   0        0        0      743 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     4064 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Scripts/__init__.py
+-rw-r--r--   0        0        0      777 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Scripts/database_answer_example.py
+-rw-r--r--   0        0        0      777 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Scripts/database_question_example.py
+-rw-r--r--   0        0        0      884 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Scripts/database_sql_grading_example.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Tests/test_1.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      690 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0      305 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/Utils/message.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:23:10.039312 llmreflect-0.1.3/llmreflect/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-30 19:23:10.039312 llmreflect-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 llmreflect-0.1.3/PKG-INFO
```

### Comparing `llmreflect-0.1.2/llmreflect/Agents/BasicAgent.py` & `llmreflect-0.1.3/llmreflect/Agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.1.3/llmreflect/Agents/EvaluationAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Agents/PostgressqlAgent.py` & `llmreflect-0.1.3/llmreflect/Agents/PostgressqlAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.1.3/llmreflect/Agents/QuestionAgent.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.1.3/llmreflect/Prompt/BasicPrompt.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Prompt/GradingPrompt.py` & `llmreflect-0.1.3/llmreflect/Prompt/GradingPrompt.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Prompt/QuestionPrompt.py` & `llmreflect-0.1.3/llmreflect/Prompt/QuestionPrompt.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.1.3/llmreflect/Prompt/promptbase/gradingpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Prompt/promptbase/postgressql.json` & `llmreflect-0.1.3/llmreflect/Prompt/promptbase/postgressql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.1.3/llmreflect/Prompt/promptbase/questionpostgresql.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.1.3/llmreflect/Retriever/BasicRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Retriever/DatabaseRetriever.py` & `llmreflect-0.1.3/llmreflect/Retriever/DatabaseRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Scripts/database_answer_example.py` & `llmreflect-0.1.3/llmreflect/Scripts/database_answer_example.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Scripts/database_question_example.py` & `llmreflect-0.1.3/llmreflect/Scripts/database_question_example.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/llmreflect/Scripts/database_sql_grading_example.py` & `llmreflect-0.1.3/llmreflect/Scripts/database_sql_grading_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,7 +22,10 @@
             db_summary=summary
         )
         print(q)
         print(result['cmd'])
         print(result['summary'])
         print(grading)
         print("=============================")
+
+
+run(5)
```

### Comparing `llmreflect-0.1.2/llmreflect/Utils/database.py` & `llmreflect-0.1.3/llmreflect/Utils/database.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.1.2/PKG-INFO` & `llmreflect-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.1.2
+Version: 0.1.3
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=2.0.17,<3.0.0)
+Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: langchain (>=0.0.219,<0.0.220)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Description-Content-Type: text/markdown
 
 # llm-reflect
```

