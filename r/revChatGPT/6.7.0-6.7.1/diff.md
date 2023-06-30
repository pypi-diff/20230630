# Comparing `tmp/revChatGPT-6.7.0.tar.gz` & `tmp/revChatGPT-6.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.7.0.tar", last modified: Fri Jun 30 15:24:37 2023, max compression
+gzip compressed data, was "revChatGPT-6.7.1.tar", last modified: Fri Jun 30 15:30:38 2023, max compression
```

## Comparing `revChatGPT-6.7.0.tar` & `revChatGPT-6.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 15:24:37.000000 revChatGPT-6.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:37.313623 revChatGPT-6.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    59454 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:24:37.000000 revChatGPT-6.7.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 15:24:37.000000 revChatGPT-6.7.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:24:37.000000 revChatGPT-6.7.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 15:24:37.000000 revChatGPT-6.7.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 15:24:37.000000 revChatGPT-6.7.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:24:37.317623 revChatGPT-6.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 15:24:04.000000 revChatGPT-6.7.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-30 15:30:37.000000 revChatGPT-6.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.137530 revChatGPT-6.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    59738 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 15:30:38.000000 revChatGPT-6.7.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:30:38.141530 revChatGPT-6.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 15:30:02.000000 revChatGPT-6.7.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.7.0/LICENSE` & `revChatGPT-6.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/PKG-INFO` & `revChatGPT-6.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.0
+Version: 6.7.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.0/README.md` & `revChatGPT-6.7.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/setup.py` & `revChatGPT-6.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT/V1.py` & `revChatGPT-6.7.1/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,32 +113,15 @@
 bcolors = t.Colors()
 
 session = tls_client.Session(
     client_identifier="firefox110", random_tls_extension_order=True
 )
 
 
-def get_arkose_token() -> str:
-    captcha_url = BASE_URL.replace("/api/", "") + "/captcha/"
-    resp = session.get(captcha_url + "start?download_images=true")
-    resp_json: dict = resp.json()
-    if resp_json.get("status") == "success":
-        return resp_json.get("token")
-    if resp.status_code != 511:
-        raise Exception(resp_json.get("error"))
-
-    if resp_json.get("status") != "captcha":
-        raise Exception("unknown error")
-
-    challenge_details: dict = resp_json.get("session", {}).get("concise_challenge")
-    if not challenge_details:
-        raise Exception("missing details")
-
-    images: list[str] = resp_json.get("images")
-
+def captcha_solver(images: list[str], challenge_details: dict) -> int:
     # mkdir captcha
     if not Path("captcha").exists():
         Path("captcha").mkdir()
 
     filenames: list[Path] = []
 
     for image in images:
@@ -162,14 +145,43 @@
     print("Enter the index of the images that matches the captcha instructions:")
     index = int(input())
 
     # Delete the images
     for filename in filenames:
         filename.unlink()
 
+    return index
+
+
+def get_arkose_token(
+    download_images: bool = True, solver: function = captcha_solver
+) -> str:
+    captcha_url = BASE_URL.replace("/api/", "") + "/captcha/"
+    resp = session.get(
+        (captcha_url + "start?download_images=true")
+        if download_images
+        else captcha_url + "start"
+    )
+    resp_json: dict = resp.json()
+    if resp_json.get("status") == "success":
+        return resp_json.get("token")
+    if resp.status_code != 511:
+        raise Exception(resp_json.get("error"))
+
+    if resp_json.get("status") != "captcha":
+        raise Exception("unknown error")
+
+    challenge_details: dict = resp_json.get("session", {}).get("concise_challenge")
+    if not challenge_details:
+        raise Exception("missing details")
+
+    images: list[str] = resp_json.get("images")
+
+    index = solver(images, challenge_details)
+
     resp = session.post(
         captcha_url + "verify",
         json={"session": resp_json.get("session"), "index": index},
     )
     if resp.status_code != 200:
         raise Exception("Failed to verify captcha")
     return resp_json.get("token")
```

### Comparing `revChatGPT-6.7.0/src/revChatGPT/V3.py` & `revChatGPT-6.7.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT/__init__.py` & `revChatGPT-6.7.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT/__main__.py` & `revChatGPT-6.7.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.7.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT/typings.py` & `revChatGPT-6.7.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT/utils.py` & `revChatGPT-6.7.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.7.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.0
+Version: 6.7.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.0/tests/test_recipient.py` & `revChatGPT-6.7.1/tests/test_recipient.py`

 * *Files identical despite different names*

