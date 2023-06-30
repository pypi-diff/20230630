# Comparing `tmp/revChatGPT-6.7.1.tar.gz` & `tmp/revChatGPT-6.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.7.1.tar", last modified: Fri Jun 30 15:30:38 2023, max compression
+gzip compressed data, was "revChatGPT-6.7.2.tar", last modified: Fri Jun 30 15:37:44 2023, max compression
```

## Comparing `revChatGPT-6.7.1.tar` & `revChatGPT-6.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 15:30:37.000000 revChatGPT-6.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.137530 revChatGPT-6.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    59738 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 15:37:44.000000 revChatGPT-6.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:37:44.483097 revChatGPT-6.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    60766 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:37:44.000000 revChatGPT-6.7.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 15:37:44.000000 revChatGPT-6.7.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:37:44.000000 revChatGPT-6.7.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 15:37:44.000000 revChatGPT-6.7.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 15:37:44.000000 revChatGPT-6.7.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:37:44.479097 revChatGPT-6.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 15:37:10.000000 revChatGPT-6.7.2/tests/test_recipient.py
```

### Comparing `revChatGPT-6.7.1/LICENSE` & `revChatGPT-6.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/PKG-INFO` & `revChatGPT-6.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.1
+Version: 6.7.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.1/README.md` & `revChatGPT-6.7.2/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/setup.py` & `revChatGPT-6.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/src/revChatGPT/V1.py` & `revChatGPT-6.7.2/src/revChatGPT/V1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Standard ChatGPT
 """
 from __future__ import annotations
 
-import sys
-import subprocess
 import base64
 import binascii
 import contextlib
 import json
 import logging
 import secrets
+import subprocess
+import sys
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
 from pathlib import Path
 from typing import AsyncGenerator
@@ -109,61 +109,72 @@
 
 
 BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
 
 bcolors = t.Colors()
 
 session = tls_client.Session(
-    client_identifier="firefox110", random_tls_extension_order=True
+    client_identifier="firefox110",
+    random_tls_extension_order=True,
 )
 
 
 def captcha_solver(images: list[str], challenge_details: dict) -> int:
     # mkdir captcha
     if not Path("captcha").exists():
         Path("captcha").mkdir()
 
     filenames: list[Path] = []
 
     for image in images:
-        filename = Path("captcha", f"{time.time()}.png")
+        filename = Path("captcha", f"{time.time()}.jpeg")
         with open(filename, "wb") as f:
             f.write(base64.b64decode(image))
         print(f"Saved captcha image to {filename}")
         # If MacOS, open the image
         if sys.platform == "darwin":
             subprocess.call(["open", filename])
         if sys.platform == "linux":
             subprocess.call(["xdg-open", filename])
         if sys.platform == "win32":
             subprocess.call(["start", filename])
         filenames.append(filename)
 
     print(f'Captcha instructions: {challenge_details.get("instructions")}')
     print(
-        "Developer instructions: The captcha images have an index starting from 0 from left to right"
+        "Developer instructions: The captcha images have an index starting from 0 from left to right",
     )
     print("Enter the index of the images that matches the captcha instructions:")
     index = int(input())
 
     # Delete the images
     for filename in filenames:
         filename.unlink()
 
     return index
 
 
 def get_arkose_token(
-    download_images: bool = True, solver: function = captcha_solver
+    download_images: bool = True,
+    solver: function = captcha_solver,
 ) -> str:
+    """
+    The solver function should take in a list of images in base64 and a dict of challenge details
+    and return the index of the image that matches the challenge details
+
+    Challenge details:
+        game_type: str - Audio or Image
+        instructions: str - Instructions for the captcha
+        URLs: list[str] - URLs of the images or audio files
+    """
     captcha_url = BASE_URL.replace("/api/", "") + "/captcha/"
     resp = session.get(
         (captcha_url + "start?download_images=true")
         if download_images
-        else captcha_url + "start"
+        else captcha_url + "start",
     )
     resp_json: dict = resp.json()
     if resp_json.get("status") == "success":
         return resp_json.get("token")
     if resp.status_code != 511:
         raise Exception(resp_json.get("error"))
 
@@ -196,29 +207,34 @@
     def __init__(
         self,
         config: dict[str, str],
         conversation_id: str | None = None,
         parent_id: str | None = None,
         lazy_loading: bool = True,
         base_url: str | None = None,
+        captcha_solver: function = captcha_solver,
+        captcha_download_images: bool = True,
     ) -> None:
         """Initialize a chatbot
 
         Args:
             config (dict[str, str]): Login and proxy info. Example:
                 {
                     "access_token": "<access_token>"
                     "proxy": "<proxy_url_string>",
                     "model": "<model_name>",
                     "plugin": "<plugin_id>",
                 }
                 More details on these are available at https://github.com/acheong08/ChatGPT#configuration
             conversation_id (str | None, optional): Id of the conversation to continue on. Defaults to None.
             parent_id (str | None, optional): Id of the previous response message to continue on. Defaults to None.
-            session_client (_type_, optional): _description_. Defaults to None.
+            lazy_loading (bool, optional): Whether to load only the active conversation. Defaults to True.
+            base_url (str | None, optional): Base URL of the ChatGPT server. Defaults to None.
+            captcha_solver (function, optional): Function to solve captcha. Defaults to captcha_solver.
+            captcha_download_images (bool, optional): Whether to download captcha images. Defaults to True.
 
         Raises:
             Exception: _description_
         """
         user_home = getenv("HOME") or getenv("USERPROFILE")
         if user_home is None:
             user_home = Path().cwd()
@@ -291,14 +307,16 @@
             auth = Authenticator("blah", "blah")
             auth.access_token = self.config["access_token"]
             puid = auth.get_puid()
             self.session.headers.update({"PUID": puid})
             print("Setting PUID (You are a Plus user!): " + puid)
         except:
             pass
+        self.captcha_solver = captcha_solver
+        self.captcha_download_images = captcha_download_images
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
             - access_token
@@ -462,15 +480,18 @@
 
         if (
             data.get("model", "").startswith("gpt-4")
             and not self.config.get("SERVER_SIDE_ARKOSE")
             and not getenv("SERVER_SIDE_ARKOSE")
         ):
             try:
-                data["arkose_token"] = get_arkose_token()
+                data["arkose_token"] = get_arkose_token(
+                    self.captcha_download_images,
+                    self.captcha_solver,
+                )
             except Exception as e:
                 print(e)
                 raise e
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         message = ""
```

### Comparing `revChatGPT-6.7.1/src/revChatGPT/V3.py` & `revChatGPT-6.7.2/src/revChatGPT/V3.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
         if self.engine not in ENGINES:
             raise NotImplementedError(
-                f"Engine {self.engine} is not supported. Select from {ENGINES}"
+                f"Engine {self.engine} is not supported. Select from {ENGINES}",
             )
         tiktoken.model.MODEL_TO_ENCODING["gpt-4"] = "cl100k_base"
 
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
@@ -227,16 +227,18 @@
                 ),
                 "frequency_penalty": kwargs.get(
                     "frequency_penalty",
                     self.frequency_penalty,
                 ),
                 "n": kwargs.get("n", self.reply_count),
                 "user": role,
-                "max_tokens": min(self.get_max_tokens(convo_id=convo_id)
-                                  , kwargs.get("max_tokens", self.max_tokens)),
+                "max_tokens": min(
+                    self.get_max_tokens(convo_id=convo_id),
+                    kwargs.get("max_tokens", self.max_tokens),
+                ),
             },
             timeout=kwargs.get("timeout", self.timeout),
             stream=True,
         )
         if response.status_code != 200:
             raise t.APIConnectionError(
                 f"{response.status_code} {response.reason} {response.text}",
@@ -300,16 +302,18 @@
                 ),
                 "frequency_penalty": kwargs.get(
                     "frequency_penalty",
                     self.frequency_penalty,
                 ),
                 "n": kwargs.get("n", self.reply_count),
                 "user": role,
-                "max_tokens": min(self.get_max_tokens(convo_id=convo_id)
-                                  , kwargs.get("max_tokens", self.max_tokens)),
+                "max_tokens": min(
+                    self.get_max_tokens(convo_id=convo_id),
+                    kwargs.get("max_tokens", self.max_tokens),
+                ),
             },
             timeout=kwargs.get("timeout", self.timeout),
         ) as response:
             if response.status_code != 200:
                 await response.aread()
                 raise t.APIConnectionError(
                     f"{response.status_code} {response.reason_phrase} {response.text}",
```

### Comparing `revChatGPT-6.7.1/src/revChatGPT/__init__.py` & `revChatGPT-6.7.2/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/src/revChatGPT/__main__.py` & `revChatGPT-6.7.2/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.7.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/src/revChatGPT/typings.py` & `revChatGPT-6.7.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/src/revChatGPT/utils.py` & `revChatGPT-6.7.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.7.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.1
+Version: 6.7.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.1/tests/test_recipient.py` & `revChatGPT-6.7.2/tests/test_recipient.py`

 * *Files identical despite different names*

