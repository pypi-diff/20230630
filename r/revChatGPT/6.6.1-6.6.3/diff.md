# Comparing `tmp/revChatGPT-6.6.1.tar.gz` & `tmp/revChatGPT-6.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.6.1.tar", last modified: Thu Jun 29 14:53:21 2023, max compression
+gzip compressed data, was "revChatGPT-6.6.3.tar", last modified: Fri Jun 30 10:11:48 2023, max compression
```

## Comparing `revChatGPT-6.6.1.tar` & `revChatGPT-6.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.539480 revChatGPT-6.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58486 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:11:48.464719 revChatGPT-6.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 10:11:48.464719 revChatGPT-6.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 10:11:48.000000 revChatGPT-6.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 10:11:48.464719 revChatGPT-6.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:11:48.456719 revChatGPT-6.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:11:48.460719 revChatGPT-6.6.3/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58651 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:11:48.464719 revChatGPT-6.6.3/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:11:48.464719 revChatGPT-6.6.3/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 10:11:48.000000 revChatGPT-6.6.3/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 10:11:48.000000 revChatGPT-6.6.3/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 10:11:48.000000 revChatGPT-6.6.3/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 10:11:48.000000 revChatGPT-6.6.3/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 10:11:48.000000 revChatGPT-6.6.3/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 10:11:48.464719 revChatGPT-6.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 10:11:18.000000 revChatGPT-6.6.3/tests/test_recipient.py
```

### Comparing `revChatGPT-6.6.1/LICENSE` & `revChatGPT-6.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/PKG-INFO` & `revChatGPT-6.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.6.1
+Version: 6.6.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.6.1/README.md` & `revChatGPT-6.6.3/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/setup.py` & `revChatGPT-6.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/src/revChatGPT/V1.py` & `revChatGPT-6.6.3/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,36 +112,41 @@
 
 session = tls_client.Session(
     client_identifier="firefox110", random_tls_extension_order=True
 )
 
 
 def get_arkose_token() -> str:
-    form_data = session.get(BASE_URL + "arkose").json().get("form")
+    resp = session.get(BASE_URL + "arkose").json()
+    form_data = resp.get("form")
+    referrer_hex = resp.get("hex")
     resp: dict = session.post(
         "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147",
         data=form_data,
         headers={
             "Host": "tcr9i.chat.openai.com",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:114.0) Gecko/20100101 Firefox/114.0",
             "Accept": "*/*",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept-Encoding": "gzip, deflate, br",
             "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
             "Origin": "https://tcr9i.chat.openai.com",
             "DNT": "1",
             "Connection": "keep-alive",
-            "Referer": "https://tcr9i.chat.openai.com/v2/1.5.2/enforcement.64b3a4e29686f93d52816249ecbf9857.html",
+            "Referer": f"https://tcr9i.chat.openai.com/v2/1.5.2/enforcement.{referrer_hex}.html",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "TE": "trailers",
         },
     ).json()
-    return resp.get("token")
+    token: str = resp.get("token")
+    if "|rid=" not in token or "|sup=" not in token:
+        raise Exception("captcha triggered by arkose")
+    return token
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
     """
```

### Comparing `revChatGPT-6.6.1/src/revChatGPT/V3.py` & `revChatGPT-6.6.3/src/revChatGPT/V3.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,16 @@
                 ),
                 "frequency_penalty": kwargs.get(
                     "frequency_penalty",
                     self.frequency_penalty,
                 ),
                 "n": kwargs.get("n", self.reply_count),
                 "user": role,
-                "max_tokens": self.get_max_tokens(convo_id=convo_id),
+                "max_tokens": min(self.get_max_tokens(convo_id=convo_id)
+                                  , kwargs.get("max_tokens", self.max_tokens)),
             },
             timeout=kwargs.get("timeout", self.timeout),
             stream=True,
         )
         if response.status_code != 200:
             raise t.APIConnectionError(
                 f"{response.status_code} {response.reason} {response.text}",
@@ -299,15 +300,16 @@
                 ),
                 "frequency_penalty": kwargs.get(
                     "frequency_penalty",
                     self.frequency_penalty,
                 ),
                 "n": kwargs.get("n", self.reply_count),
                 "user": role,
-                "max_tokens": self.get_max_tokens(convo_id=convo_id),
+                "max_tokens": min(self.get_max_tokens(convo_id=convo_id)
+                                  , kwargs.get("max_tokens", self.max_tokens)),
             },
             timeout=kwargs.get("timeout", self.timeout),
         ) as response:
             if response.status_code != 200:
                 await response.aread()
                 raise t.APIConnectionError(
                     f"{response.status_code} {response.reason_phrase} {response.text}",
```

### Comparing `revChatGPT-6.6.1/src/revChatGPT/__init__.py` & `revChatGPT-6.6.3/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/src/revChatGPT/__main__.py` & `revChatGPT-6.6.3/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.6.3/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/src/revChatGPT/typings.py` & `revChatGPT-6.6.3/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/src/revChatGPT/utils.py` & `revChatGPT-6.6.3/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.6.3/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.6.1
+Version: 6.6.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.6.1/tests/test_recipient.py` & `revChatGPT-6.6.3/tests/test_recipient.py`

 * *Files identical despite different names*

