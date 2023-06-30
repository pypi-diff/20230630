# Comparing `tmp/openai_api_call-0.5.2.tar.gz` & `tmp/openai_api_call-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.5.2.tar", last modified: Fri Jun 16 08:55:36 2023, max compression
+gzip compressed data, was "openai_api_call-0.5.3.tar", last modified: Fri Jun 30 03:05:04 2023, max compression
```

## Comparing `openai_api_call-0.5.2.tar` & `openai_api_call-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:55:36.340973 openai_api_call-0.5.2/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-16 08:55:36.000000 openai_api_call-0.5.2/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 08:55:35.000000 openai_api_call-0.5.2/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:55:36.344974 openai_api_call-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-16 08:55:25.000000 openai_api_call-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:05:04.856735 openai_api_call-0.5.3/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/setup.py
```

### Comparing `openai_api_call-0.5.2/LICENSE` & `openai_api_call-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.2/PKG-INFO` & `openai_api_call-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.5.2
+Version: 0.5.3
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
```

### Comparing `openai_api_call-0.5.2/README.md` & `openai_api_call-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.2/openai_api_call/__init__.py` & `openai_api_call-0.5.3/openai_api_call/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 
 import os, requests
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 from . import request
 
@@ -41,15 +41,16 @@
     """Show the base url of the API call"""
     print(f"Base url:\t{request.base_url}")
 
 def debug_log( net_url:str="https://www.baidu.com"
              , timeout:int=5
              , message:str="hello world! 你好！"
              , test_usage:bool=True
-             , test_response:bool=True):
+             , test_response:bool=True
+             , test_model:bool=True):
     """Debug the API call
 
     Args:
         net_url (str, optional): The url to test the network. Defaults to "https://www.baidu.com".
         timeout (int, optional): The timeout for the network test. Defaults to 5.
         test_usage (bool, optional): Whether to test the usage status. Defaults to True.
         test_response (bool, optional): Whether to test the hello world. Defaults to True.
@@ -82,15 +83,20 @@
         print("Warning: the `url` parameter is deprecated, please use `base_url` instead.")
 
     # 5. Get usage status
     if test_usage:
         print("\nThe usage status of your API key:")
         Chat().show_usage_status(recent=3)
 
-    # 6. Test hello world
+    # 6. Get model list
+    if test_model:
+        print("\nThe model list:")
+        print(Chat().get_valid_models())
+        
+    # 7. Test hello world
     if test_response:
         print("\nTest message:", message)
         chat = Chat(message)
         chat.getresponse(max_requests=3)
         chat.print_log()
 
     print("\nDebug is finished.")
```

### Comparing `openai_api_call-0.5.2/openai_api_call/chattool.py` & `openai_api_call-0.5.3/openai_api_call/chattool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # The object that stores the chat log
 
 from typing import List, Dict, Union, Callable
 import openai_api_call
 from .response import Resp
-from .request import chat_completion, usage_status
+from .request import chat_completion, usage_status, valid_models
 import signal, time, random
 import datetime
 import json
 import warnings
 
 # timeout handler
 def handler(signum, frame):
     raise Exception("API call timed out!")
 
 class Chat():
     def __init__( self
                 , msg:Union[List[Dict], None, str]=None
-                , api_key:Union[None, str]=None) -> None:
+                , api_key:Union[None, str]=None
+                , chat_url:Union[None, str]=None) -> None:
         """Initialize the chat log
 
         Args:
             msg (Union[List[Dict], None, str], optional): chat log. Defaults to None.
             api_key (Union[None, str], optional): API key. Defaults to None.
+            chat_url (Union[None, str], optional): base url. Defaults to None. Example: "https://api.openai.com/v1/chat/completions"
         
         Raises:
             ValueError: msg should be a list of dict, a string or None
         """
         if msg is None:
             self._chat_log = []
         elif isinstance(msg, str):
@@ -34,25 +36,41 @@
             else:
                 self._chat_log = openai_api_call.default_prompt(msg)
         elif isinstance(msg, list):
             self._chat_log = msg.copy() # avoid changing the original list
         else:
             raise ValueError("msg should be a list of dict, a string or None")
         self._api_key = openai_api_call.api_key if api_key is None else api_key
+        self._chat_url = chat_url
     
     @property
     def api_key(self):
         """Get API key"""
         return self._api_key
     
+    @property
+    def chat_url(self):
+        """Get base url"""
+        return self._chat_url
+    
     @api_key.setter
     def api_key(self, api_key:str):
         """Set API key"""
         self._api_key = api_key
     
+    @chat_url.setter
+    def chat_url(self, chat_url:str):
+        """Set base url"""
+        self._chat_url = chat_url
+
+    @property
+    def chat_log(self):
+        """Chat history"""
+        return self._chat_log
+    
     def getresponse( self
                    , max_requests:int=1
                    , strip:bool=True
                    , update:bool = True
                    , timeout:int = 0
                    , timeinterval:int = 0
                    , api_key:Union[str, None]=None
@@ -87,15 +105,15 @@
         signal.signal(signal.SIGALRM, handler)
         while max_requests:
             try:
                 # Set the alarm to trigger after `timeout` seconds
                 signal.alarm(timeout)
                 # Make the API call
                 response = chat_completion(
-                    api_key=api_key, messages=msg, model=model, **options)
+                    api_key=api_key, messages=msg, model=model, chat_url=self.chat_url, **options)
                 time.sleep(random.random() * timeinterval)
                 resp = Resp(response, strip=strip)
                 assert resp.is_valid(), "Invalid response with message: " + resp.error_message
                 break
             except Exception as e:
                 max_requests -= 1
                 numoftries += 1
@@ -150,14 +168,25 @@
             print(f"Remaining(this month): {rem:.4f}$")
         if len(recent_usage) > 0:
             usage = sum(recent_usage.values())
             print(f"Usage(the last {len(recent_usage)} days): {usage:.4f}$")
         for date, cost in recent_usage.items():
             print(f"{date}: {cost:.4f}$")
 
+    def get_valid_models(self, gpt_only:bool=True)->List[str]:
+        """Get the valid models
+
+        Args:
+            gpt_only (bool, optional): whether to only show the GPT models. Defaults to True.
+
+        Returns:
+            List[str]: valid models
+        """
+        return valid_models(self.api_key, gpt_only=gpt_only)
+
     def add(self, role:str, msg:str):
         """Add a message to the chat log"""
         assert role in ['user', 'assistant', 'system'], "role should be 'user', 'assistant' or 'system'"
         self._chat_log.append({"role": role, "content": msg})
         return self
 
     def user(self, msg:str):
@@ -201,19 +230,14 @@
     def print_log(self, sep: Union[str, None]=None):
         """Print the chat log"""
         if sep is None:
             sep = '\n' + '-'*15 + '\n'
         for d in self._chat_log:
             print(sep, d['role'], sep, d['content'])
     
-    @property
-    def chat_log(self):
-        """Chat history"""
-        return self._chat_log
-    
     def pop(self, ind:int=-1):
         """Pop the last message"""
         return self._chat_log.pop(ind)
 
     def __len__(self):
         """Length of the chat log"""
         return len(self._chat_log)
```

### Comparing `openai_api_call-0.5.2/openai_api_call/checkpoint.py` & `openai_api_call-0.5.3/openai_api_call/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json, warnings, os
 from typing import List, Dict, Union, Callable, Any
 from .chattool import Chat
-from tqdm import tqdm
+import tqdm
 
 def load_chats( checkpoint:str
               , sep:str='\n'
               , last_message_only:bool=False
               , chat_log_only:bool=False):
     """Load chats from a checkpoint file
     
@@ -51,24 +51,26 @@
     return [Chat(chatlog) if chatlog is not None else None for chatlog in chatlogs]
 
 def process_chats( data:List[Any]
                  , data2chat:Callable[[Any], Chat]
                  , checkpoint:str
                  , sep:str='\n'
                  , last_message_only:bool=False
-                 , clearfile:bool=False):
+                 , clearfile:bool=False
+                 , notebook:bool=False):
     """Process chats and save to a checkpoint file
     
     Args:
         data (List[Any]): data to be processed
         data2chat (Callable[[Any], Chat]): function to convert data to Chat
         checkpoint (str): path to the checkpoint file
         sep (str, optional): separator of chats. Defaults to '\n'.
         last_message_only (bool, optional): whether to return the last message of each chat. Defaults to False.
         clearfile (bool, optional): whether to clear the checkpoint file. Defaults to False.
+        notebook (bool, optional): whether to use tqdm in Jupiter Notebook. Defaults to False.
 
     Returns:
         list: chats or last messages of chats
     """
     if clearfile and os.path.exists(checkpoint):
         # Warning: You are about to delete the checkpoint file
         os.system(f"rm {checkpoint}")
@@ -77,15 +79,16 @@
     if len(chats) > len(data):
         warnings.warn(f"checkpoint file {checkpoint} has more chats than the messages")
         chats = chats[:len(data)]
         return [chat[-1] for chat in chats] if last_message_only else chats
         
     chats.extend([None] * (len(data) - len(chats)))
     ## process chats
-    for i in tqdm(range(len(data))):
+    tq = tqdm.tqdm if not notebook else tqdm.notebook.tqdm
+    for i in tq(range(len(data))):
         if chats[i] is not None: continue
         chat = data2chat(data[i])
         chat.save(checkpoint, mode='a', end=sep)
         chats[i] = chat
     if last_message_only:
         return [chat[-1] for chat in chats]
     return chats
```

### Comparing `openai_api_call-0.5.2/openai_api_call/proxy.py` & `openai_api_call-0.5.3/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.2/openai_api_call/response.py` & `openai_api_call-0.5.3/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.2/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.5.3/openai_api_call.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.5.2
+Version: 0.5.3
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
```

### Comparing `openai_api_call-0.5.2/setup.py` & `openai_api_call-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.5.2'
+VERSION = '0.5.3'
 
 requirements = ['Click>=7.0', 'requests>=2.20', 'tqdm>=4.60']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

