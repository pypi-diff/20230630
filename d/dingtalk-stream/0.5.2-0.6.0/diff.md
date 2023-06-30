# Comparing `tmp/dingtalk-stream-0.5.2.tar.gz` & `tmp/dingtalk-stream-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.5.2.tar", last modified: Wed Jun 21 07:51:47 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.6.0.tar", last modified: Fri Jun 30 03:44:34 2023, max compression
```

## Comparing `dingtalk-stream-0.5.2.tar` & `dingtalk-stream-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:51:47.826393 dingtalk-stream-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:51:47.826393 dingtalk-stream-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:51:47.826393 dingtalk-stream-0.5.2/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:51:47.826393 dingtalk-stream-0.5.2/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-21 07:51:47.000000 dingtalk-stream-0.5.2/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 07:51:47.000000 dingtalk-stream-0.5.2/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:51:47.000000 dingtalk-stream-0.5.2/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 07:51:47.000000 dingtalk-stream-0.5.2/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 07:51:47.000000 dingtalk-stream-0.5.2/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:51:47.826393 dingtalk-stream-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-21 07:51:46.000000 dingtalk-stream-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:44:34.856657 dingtalk-stream-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-30 03:44:34.852657 dingtalk-stream-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:44:34.852657 dingtalk-stream-0.6.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:44:34.852657 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 03:44:34.000000 dingtalk-stream-0.6.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:44:34.856657 dingtalk-stream-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-30 03:44:33.000000 dingtalk-stream-0.6.0/setup.py
```

### Comparing `dingtalk-stream-0.5.2/LICENSE` & `dingtalk-stream-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.2/PKG-INFO` & `dingtalk-stream-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.5.2/README.md` & `dingtalk-stream-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.2/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.6.0/dingtalk_stream/chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import hashlib
 from .stream import CallbackHandler, CallbackMessage
 from .frames import AckMessage, Headers
 from .interactive_card import generate_multi_text_line_card_data
 from .utils import DINGTALK_OPENAPI_ENDPOINT
 from concurrent.futures import ThreadPoolExecutor
 import uuid
+from .card_instance import MarkdownCardInstance, AIMarkdownCardInstance
 
 
 class AtUser(object):
     def __init__(self):
         self.dingtalk_id = None
         self.staff_id = None
         self.extensions = {}
@@ -191,14 +192,51 @@
             self.sender_nick,
             self.conversation_title,
         )
 
 
 class ChatbotHandler(CallbackHandler):
 
+    def __init__(self):
+        super(ChatbotHandler, self).__init__()
+
+    def reply_markdown_card(self, markdown: str, incoming_message: ChatbotMessage, title: str = "", logo: str = "",
+                            at_sender: bool = False, at_all: bool = False) -> MarkdownCardInstance:
+        """
+        回复一个markdown卡片
+        :param markdown:
+        :param incoming_message:
+        :param title:
+        :param logo:
+        :param at_sender:
+        :param at_all:
+        :return:
+        """
+        markdown_card_instance = MarkdownCardInstance(self.dingtalk_client, incoming_message)
+        markdown_card_instance.set_title_and_logo(title, logo)
+
+        markdown_card_instance.reply(markdown, at_sender, at_all)
+
+        return markdown_card_instance
+
+    def ai_markdown_card_start(self, incoming_message: ChatbotMessage, title: str = "",
+                               logo: str = "") -> AIMarkdownCardInstance:
+        """
+        发起一个AI卡片
+        :param incoming_message:
+        :param title:
+        :param logo:
+        :return:
+        """
+        ai_markdown_card_instance = AIMarkdownCardInstance(self.dingtalk_client, incoming_message)
+        ai_markdown_card_instance.set_title_and_logo(title, logo)
+
+        ai_markdown_card_instance.ai_start()
+        return ai_markdown_card_instance
+
     def set_off_duty_prompt(self, text: str, title: str = "", logo: str = ""):
         """
         设置离线提示词，需要使用OpenAPI，当前仅支持自建应用。
         :param text: 离线提示词，支持markdown
         :param title: 机器人名称，默认："钉钉Stream机器人"
         :param logo: 机器人logo，默认："@lALPDfJ6V_FPDmvNAfTNAfQ"
         :return:
```

### Comparing `dingtalk-stream-0.5.2/dingtalk_stream/frames.py` & `dingtalk-stream-0.6.0/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.2/dingtalk_stream/handlers.py` & `dingtalk-stream-0.6.0/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.2/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.6.0/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.2/dingtalk_stream/stream.py` & `dingtalk-stream-0.6.0/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.5.2/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.6.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.5.2/setup.py` & `dingtalk-stream-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.5.2',
+    version='0.6.0',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

