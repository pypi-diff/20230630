# Comparing `tmp/mona-openai-0.0.8.tar.gz` & `tmp/mona-openai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.8.tar", last modified: Thu Jun 29 11:38:06 2023, max compression
+gzip compressed data, was "mona-openai-0.0.9.tar", last modified: Fri Jun 30 06:24:56 2023, max compression
```

## Comparing `mona-openai-0.0.8.tar` & `mona-openai-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.832827 mona-openai-0.0.8/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.8/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-29 11:38:06.832620 mona-openai-0.0.8/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    10208 2023-06-29 11:01:14.000000 mona-openai-0.0.8/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.827551 mona-openai-0.0.8/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      100 2023-06-29 11:01:14.000000 mona-openai-0.0.8/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.829093 mona-openai-0.0.8/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3148 2023-06-29 11:36:56.000000 mona-openai-0.0.8/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.829898 mona-openai-0.0.8/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     7749 2023-06-29 11:07:35.000000 mona-openai-0.0.8/mona_openai/endpoints/chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     5165 2023-06-20 04:36:07.000000 mona-openai-0.0.8/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/endpoints/endpoint_wrapping.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/endpoints/wrapping_getter.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.0.8/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-06-29 11:01:14.000000 mona-openai-0.0.8/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17565 2023-06-29 11:01:14.000000 mona-openai-0.0.8/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.831143 mona-openai-0.0.8/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.0.8/mona_openai/util/async_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.8/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/oop_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/openai_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/stream_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.8/mona_openai/util/tokens_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.8/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.828384 mona-openai-0.0.8/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-06-29 11:38:06.000000 mona-openai-0.0.8/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-06-29 11:37:26.000000 mona-openai-0.0.8/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.8/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-06-29 11:38:06.832862 mona-openai-0.0.8/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-29 11:38:06.832335 mona-openai-0.0.8/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.8/tests/test_chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    20103 2023-06-22 09:34:20.000000 mona-openai-0.0.8/tests/test_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.8/tests/test_privacy_analyzer.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:07:35.000000 mona-openai-0.0.8/tests/test_textual_analyzer.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.189441 mona-openai-0.0.9/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.9/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-30 06:24:56.189265 mona-openai-0.0.9/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    10208 2023-06-30 04:40:35.000000 mona-openai-0.0.9/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.185001 mona-openai-0.0.9/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      100 2023-06-30 04:40:35.000000 mona-openai-0.0.9/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.186280 mona-openai-0.0.9/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3100 2023-06-30 04:45:38.000000 mona-openai-0.0.9/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.187086 mona-openai-0.0.9/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7750 2023-06-30 04:45:19.000000 mona-openai-0.0.9/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5166 2023-06-30 04:45:09.000000 mona-openai-0.0.9/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      225 2023-06-28 08:19:06.000000 mona-openai-0.0.9/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-06-30 04:40:35.000000 mona-openai-0.0.9/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17565 2023-06-30 04:40:35.000000 mona-openai-0.0.9/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.188202 mona-openai-0.0.9/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.0.9/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.9/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.9/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.9/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.185715 mona-openai-0.0.9/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    10802 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-06-30 06:24:56.000000 mona-openai-0.0.9/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-06-30 06:24:43.000000 mona-openai-0.0.9/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.9/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-06-30 06:24:56.189476 mona-openai-0.0.9/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-30 06:24:56.188980 mona-openai-0.0.9/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17356 2023-06-30 04:45:09.000000 mona-openai-0.0.9/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    20107 2023-06-30 04:45:09.000000 mona-openai-0.0.9/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.9/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      975 2023-06-29 11:44:26.000000 mona-openai-0.0.9/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.0.8/LICENSE` & `mona-openai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/PKG-INFO` & `mona-openai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mona-openai Version: 0.0.8 Summary: Integration
+Metadata-Version: 2.1 Name: mona-openai Version: 0.0.9 Summary: Integration
 client for monitoring OpenAI usage with Mona Author-email: Itai Bar Sinai
 monalabs.io> Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE # Mona-OpenAI
```

### Comparing `mona-openai-0.0.8/README.md` & `mona-openai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/analysis/privacy.py` & `mona-openai-0.0.9/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/analysis/textual.py` & `mona-openai-0.0.9/mona_openai/analysis/textual.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,19 +107,15 @@
         return len(self._prepositions)
 
     def get_preposition_ratio(self):
         """
         Returns the ratio of prepositions in the text.
         """
         word_count = self.get_word_count()
-        return (
-            self.get_preposition_count() / word_count
-            if word_count
-            else 0
-        )
+        return self.get_preposition_count() / word_count if word_count else 0
 
     def get_words_not_in_others_count(
         self, others: Iterable["TextualAnalyzer"]
     ):
         """
         Returns the number of the words in the text that do not appear in the
         given other texts.
```

### Comparing `mona-openai-0.0.8/mona_openai/endpoints/chat_completion.py` & `mona-openai-0.0.9/mona_openai/endpoints/chat_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 combined_answers.get_previously_unseen_phone_numbers_count(
                     messages_privacy_analyzers
                 )
             ),
             "total_prompt_email_count": sum(
                 combined_messages.get_emails_count()
             ),
-            "answer_unkown_email_count": (
+            "answer_unknown_email_count": (
                 combined_answers.get_previously_unseen_emails_count(
                     messages_privacy_analyzers
                 )
             ),
         }
         if last_user_message_analyzer is not None:
             ret.update(
```

### Comparing `mona-openai-0.0.8/mona_openai/endpoints/completion.py` & `mona-openai-0.0.9/mona_openai/endpoints/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             ),
             "answer_unknown_phone_number_count": (
                 combined_answers.get_previously_unseen_phone_numbers_count(
                     prompts_privacy_analyzers
                 )
             ),
             "prompt_email_count": combined_prompts.get_emails_count(),
-            "answer_unkown_email_count": (
+            "answer_unknown_email_count": (
                 combined_answers.get_previously_unseen_emails_count(
                     prompts_privacy_analyzers
                 )
             ),
         }
 
     @_get_texts
```

### Comparing `mona-openai-0.0.8/mona_openai/endpoints/endpoint_wrapping.py` & `mona-openai-0.0.9/mona_openai/endpoints/endpoint_wrapping.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/endpoints/wrapping_getter.py` & `mona-openai-0.0.9/mona_openai/endpoints/wrapping_getter.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/mona_client.py` & `mona-openai-0.0.9/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/mona_openai.py` & `mona-openai-0.0.9/mona_openai/mona_openai.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/util/async_util.py` & `mona-openai-0.0.9/mona_openai/util/async_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/util/func_util.py` & `mona-openai-0.0.9/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/util/oop_util.py` & `mona-openai-0.0.9/mona_openai/util/oop_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/util/stream_util.py` & `mona-openai-0.0.9/mona_openai/util/stream_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/util/tokens_util.py` & `mona-openai-0.0.9/mona_openai/util/tokens_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai/util/validation_util.py` & `mona-openai-0.0.9/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.0.9/mona_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mona-openai Version: 0.0.8 Summary: Integration
+Metadata-Version: 2.1 Name: mona-openai Version: 0.0.9 Summary: Integration
 client for monitoring OpenAI usage with Mona Author-email: Itai Bar Sinai
 monalabs.io> Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE # Mona-OpenAI
```

### Comparing `mona-openai-0.0.8/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.0.9/mona_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/pyproject.toml` & `mona-openai-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mona-openai-0.0.8/tests/test_chat_completion.py` & `mona-openai-0.0.9/tests/test_chat_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 _DEFAULT_EXPORTED_INPUT = _remove_text_content_from_input(_DEFAULT_INPUT)
 
 _DEFAULT_ANALYSIS = {
     "privacy": {
         "total_prompt_phone_number_count": 0,
         "answer_unknown_phone_number_count": (0,),
         "total_prompt_email_count": 0,
-        "answer_unkown_email_count": (0,),
+        "answer_unknown_email_count": (0,),
         "last_user_message_phone_number_count": 0,
         "last_user_message_emails_count": 0,
     },
     "textual": {
         "total_prompt_length": 35,
         "answer_length": (12,),
         "total_prompt_word_count": 7,
@@ -172,15 +172,15 @@
     expected_input = _remove_text_content_from_input(new_input)
 
     new_analysis = {
         "privacy": {
             "total_prompt_phone_number_count": 0,
             "answer_unknown_phone_number_count": (0,),
             "total_prompt_email_count": 0,
-            "answer_unkown_email_count": (0,),
+            "answer_unknown_email_count": (0,),
         },
         "textual": {
             "total_prompt_length": 74,
             "answer_length": (12,),
             "total_prompt_word_count": 14,
             "answer_word_count": (3,),
             "total_prompt_preposition_count": 2,
@@ -228,15 +228,15 @@
     expected_input = _remove_text_content_from_input(new_input)
 
     new_analysis = {
         "privacy": {
             "total_prompt_phone_number_count": 0,
             "answer_unknown_phone_number_count": (0,),
             "total_prompt_email_count": 0,
-            "answer_unkown_email_count": (0,),
+            "answer_unknown_email_count": (0,),
             "last_user_message_phone_number_count": 0,
             "last_user_message_emails_count": 0,
         },
         "textual": {
             "total_prompt_length": 94,
             "answer_length": (12,),
             "total_prompt_word_count": 18,
@@ -368,15 +368,15 @@
     new_expected_response = _get_response_without_texts(new_response)
 
     new_analysis = {
         "privacy": {
             "total_prompt_phone_number_count": 0,
             "answer_unknown_phone_number_count": (0, 0, 0),
             "total_prompt_email_count": 0,
-            "answer_unkown_email_count": (0, 0, 0),
+            "answer_unknown_email_count": (0, 0, 0),
             "last_user_message_phone_number_count": 0,
             "last_user_message_emails_count": 0,
         },
         "textual": {
             "total_prompt_length": 35,
             "answer_length": (12, 13, 7),
             "total_prompt_word_count": 7,
@@ -501,15 +501,15 @@
     }
 
     new_analysis = {
         "privacy": {
             "total_prompt_phone_number_count": 0,
             "answer_unknown_phone_number_count": (0, 0),
             "total_prompt_email_count": 0,
-            "answer_unkown_email_count": (0, 0),
+            "answer_unknown_email_count": (0, 0),
             "last_user_message_phone_number_count": 0,
             "last_user_message_emails_count": 0,
         },
         "textual": {
             "total_prompt_length": 35,
             "answer_length": (12, 12),
             "total_prompt_word_count": 7,
```

### Comparing `mona-openai-0.0.8/tests/test_completion.py` & `mona-openai-0.0.9/tests/test_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 }
 
 _DEFAULT_ANALYSIS = {
     "privacy": {
         "prompt_phone_number_count": (0,),
         "answer_unknown_phone_number_count": (0,),
         "prompt_email_count": (0,),
-        "answer_unkown_email_count": (0,),
+        "answer_unknown_email_count": (0,),
     },
     "textual": {
         "prompt_length": (35,),
         "answer_length": (12,),
         "prompt_word_count": (7,),
         "answer_word_count": (3,),
         "prompt_preposition_count": (2,),
@@ -177,15 +177,15 @@
     new_expected_response = _get_response_without_texts(new_response)
 
     new_analysis = {
         "privacy": {
             "prompt_phone_number_count": (0, 0),
             "answer_unknown_phone_number_count": (0, 0),
             "prompt_email_count": (0, 0),
-            "answer_unkown_email_count": (0, 0),
+            "answer_unknown_email_count": (0, 0),
         },
         "textual": {
             "prompt_length": (35, 40),
             "answer_length": (12, 13),
             "prompt_word_count": (7, 8),
             "answer_word_count": (3, 3),
             "prompt_preposition_count": (2, 2),
@@ -455,15 +455,15 @@
     new_expected_response = _get_response_without_texts(new_response)
 
     new_analysis = {
         "privacy": {
             "prompt_phone_number_count": (0,),
             "answer_unknown_phone_number_count": (0, 0, 0),
             "prompt_email_count": (0,),
-            "answer_unkown_email_count": (0, 0, 0),
+            "answer_unknown_email_count": (0, 0, 0),
         },
         "textual": {
             "prompt_length": (35,),
             "answer_length": (12, 13, 7),
             "prompt_word_count": (7,),
             "answer_word_count": (3, 3, 1),
             "prompt_preposition_count": (2,),
@@ -589,15 +589,15 @@
     }
 
     new_analysis = {
         "privacy": {
             "prompt_phone_number_count": (0,),
             "answer_unknown_phone_number_count": (0, 0),
             "prompt_email_count": (0,),
-            "answer_unkown_email_count": (0, 0),
+            "answer_unknown_email_count": (0, 0),
         },
         "textual": {
             "prompt_length": (35,),
             "answer_length": (12, 12),
             "prompt_word_count": (7,),
             "answer_word_count": (3, 3),
             "prompt_preposition_count": (2,),
```

### Comparing `mona-openai-0.0.8/tests/test_privacy_analyzer.py` & `mona-openai-0.0.9/tests/test_privacy_analyzer.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.8/tests/test_textual_analyzer.py` & `mona-openai-0.0.9/tests/test_textual_analyzer.py`

 * *Files identical despite different names*

