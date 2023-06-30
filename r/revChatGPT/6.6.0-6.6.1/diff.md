# Comparing `tmp/revChatGPT-6.6.0.tar.gz` & `tmp/revChatGPT-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.6.0.tar", last modified: Thu Jun 29 09:02:39 2023, max compression
+gzip compressed data, was "revChatGPT-6.6.1.tar", last modified: Thu Jun 29 14:53:21 2023, max compression
```

## Comparing `revChatGPT-6.6.0.tar` & `revChatGPT-6.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.598651 revChatGPT-6.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58293 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.539480 revChatGPT-6.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58486 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 14:53:21.000000 revChatGPT-6.6.1/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:21.543480 revChatGPT-6.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-29 14:52:52.000000 revChatGPT-6.6.1/tests/test_recipient.py
```

### Comparing `revChatGPT-6.6.0/LICENSE` & `revChatGPT-6.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/PKG-INFO` & `revChatGPT-6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.6.0
+Version: 6.6.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.6.0/README.md` & `revChatGPT-6.6.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/setup.py` & `revChatGPT-6.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT/V1.py` & `revChatGPT-6.6.1/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,16 +409,23 @@
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> Generator[dict, None, None]:
         log.debug("Sending the payload")
 
-        if data.get("model", "").startswith("gpt-4"):
-            data["arkose_token"] = get_arkose_token()
+        if (
+            data.get("model", "").startswith("gpt-4")
+            and not self.config.get("SERVER_SIDE_ARKOSE")
+            and not getenv("SERVER_SIDE_ARKOSE")
+        ):
+            try:
+                data["arkose_token"] = get_arkose_token()
+            except:
+                pass
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
         message = ""
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         response = self.session.post(
```

### Comparing `revChatGPT-6.6.0/src/revChatGPT/V3.py` & `revChatGPT-6.6.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT/__init__.py` & `revChatGPT-6.6.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT/__main__.py` & `revChatGPT-6.6.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.6.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT/typings.py` & `revChatGPT-6.6.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT/utils.py` & `revChatGPT-6.6.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.6.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.6.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.6.0
+Version: 6.6.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.6.0/tests/test_recipient.py` & `revChatGPT-6.6.1/tests/test_recipient.py`

 * *Files identical despite different names*

