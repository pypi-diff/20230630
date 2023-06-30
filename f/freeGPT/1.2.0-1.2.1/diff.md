# Comparing `tmp/freeGPT-1.2.0.tar.gz` & `tmp/freeGPT-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.0.tar", last modified: Sun Jun 25 19:20:57 2023, max compression
+gzip compressed data, was "freeGPT-1.2.1.tar", last modified: Fri Jun 30 21:36:33 2023, max compression
```

## Comparing `freeGPT-1.2.0.tar` & `freeGPT-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 19:20:57.043224 freeGPT-1.2.0/
--rw-rw-rw-   0        0        0    35149 2023-06-25 19:15:08.000000 freeGPT-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       96 2023-06-25 19:15:08.000000 freeGPT-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4501 2023-06-25 19:20:57.039200 freeGPT-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3326 2023-06-25 19:15:08.000000 freeGPT-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 19:20:56.997200 freeGPT-1.2.0/freeGPT/
--rw-rw-rw-   0        0        0      134 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1632 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     4725 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/c_a_l.py
--rw-rw-rw-   0        0        0     1220 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     2655 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/gpt4.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:20:57.037205 freeGPT-1.2.0/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     4501 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 19:20:57.044215 freeGPT-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1577 2023-06-25 19:15:08.000000 freeGPT-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 21:36:33.056357 freeGPT-1.2.1/
+-rw-rw-rw-   0        0        0    35149 2023-06-30 21:35:53.000000 freeGPT-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3561 2023-06-30 21:36:33.054357 freeGPT-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2273 2023-06-30 21:35:53.000000 freeGPT-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 21:36:33.038357 freeGPT-1.2.1/freeGPT/
+-rw-rw-rw-   0        0        0      120 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1880 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     1955 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     4667 2023-06-30 21:35:53.000000 freeGPT-1.2.1/freeGPT/gpt4.py
+drwxrwxrwx   0        0        0        0 2023-06-30 21:36:33.053357 freeGPT-1.2.1/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3561 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-30 21:36:33.000000 freeGPT-1.2.1/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 21:36:32.000000 freeGPT-1.2.1/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 21:36:33.056357 freeGPT-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-06-30 21:35:53.000000 freeGPT-1.2.1/setup.py
```

### Comparing `freeGPT-1.2.0/LICENSE` & `freeGPT-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.0/README.md` & `freeGPT-1.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,94 @@
-[![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
-[![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
-[![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
-# freeGPT
-freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
-<br>
-Get started by installing the package:
-```
-py -m pip install --upgrade freeGPT
-```
-***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)***
-<br>
-Join my [Discord Server](https://discord.gg/XH6pUGkwRr) for live chat and support or if you have any issues with this package.
-
-## Source:
-*GPT-3 has internet access.*
-<br>
-| Models            | Websites                                             |
-| ----------------- | -----------------------------------------------------|
-| gpt3              | [you.com](https://you.com/)                          |
-| gpt4              | [ava-ai-ef611.web.app](https://ava-ai-ef611.web.app/)|
-| alpaca_7b         | [chatllama.baseten.co](https://chatllama.baseten.co/)|
-
-### TODO-List:
-- [x] Make the library well-documented.
-- [x] Make the over-all library easier to use.
-- [x] Make the over-all library easier to understand.
-- [x] Replace you.com with theb.ai for less failed responses.
-- [x] Make GPT-3 & GPT-4 models with web access.
-- [x] Add a non-GPT model.
-- [x] Make a discord bot.
-- [ ] Add a image generation model.
-
-## Support this repository:
-- Star this repository! :D
-- Add the [Discord Bot](https://dsc.gg/freeGPT) :D
-- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
-
-[![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
-
-## Discord bot:
-- Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
-- This bot has ALL the models in this repository available.
-- Its interactive, fast and overall easy to use.
-- And lastly its [Open Sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!
-
-## Examples:
-
-#### GPT-3:
-```python
-from freeGPT import gpt3
-
-while True:
-    prompt = input("👦 > ")
-    try:
-        # Remove the 'proxy' variable and the 'proxies' parameter if you don't want to use a proxy.
-        proxy = "Your proxies IP"
-        resp = gpt3.Completion.create(prompt=prompt, chat=[], proxies={"https": "http://" + proxy})
-        print(f"🤖 > {str(resp['text'])}")
-    except Exception as e:
-        print(f"🤖 > {str(e)}")
-```
-#### GPT-4:
-```python
-from freeGPT import gpt4
-
-while True:
-    prompt = input("👦 > ")
-    try:
-        resp = gpt4.Completion.create(prompt=prompt)
-        print(f"🤖 > {str(resp)}")
-    except Exception as e:
-        print(f"🤖 > {str(e)}")
-```
-
-#### Alpaca-7b:
-```python
-from freeGPT import alpaca_7b
-
-while True:
-    prompt = input("👦 > ")
-    try:
-        resp = alpaca_7b.Completion.create(prompt=prompt)
-        print(f"🤖 > {str(resp)}")
-    except Exception as e:
-        print(f"🤖 > {str(e)}")
-```
-
-## Star History:
-[![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
-
+Metadata-Version: 2.1
+Name: freeGPT
+Version: 1.2.1
+Summary: freeGPT provides free access to GPT3, GPT4 and more models.
+Home-page: https://github.com/Ruu3f/freeGPT
+Author: Ruu3f
+License: GPLv3
+Project-URL: Source, https://github.com/Ruu3f/freeGPT
+Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
+Project-URL: Discord, https://discord.gg/XH6pUGkwRr
+Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt4,gpt3,gpt,ai
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
+[![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
+[![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
+
+# freeGPT
+
+freeGPT provides free access to GPT3, GPT4 and more models.
+
+## Get started:
+
+```
+py -m pip install --upgrade freeGPT
+```
+
+**Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!**
+
+Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
+
+## Source:
+
+| Models   | Websites                                                |
+| -------- | ------------------------------------------------------- |
+| gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
+| gpt4     | [<you.com>](https://you.com/)       |
+| alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+
+## Support this repository:
+
+- Star this repository :D
+- Add the [freeGPT Discord bot](https://dsc.gg/freeGPT).
+- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
+
+[![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
+
+## TODO List:
+
+- [x] Make the library well-documented.
+- [x] Make the overall library easier to use.
+- [x] Make the overall library easier to understand.
+- [x] Add a non-GPT model.
+- [x] Make a discord bot.
+- [ ] Add an image generation model.
+
+## Discord bot:
+
+- Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
+- This bot has all the models in this repository available.
+- It's interactive, overall fast, and easy to use.
+- And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot).
+
+## Example:
+
+```python
+import freeGPT
+
+while True:
+    prompt = input("👦: ")
+    try:
+        model = getattr(freeGPT, "Model Name here.")
+        resp = model.Completion.create(prompt)
+        print(f"🤖: {resp}")
+    except Exception as e:
+        print(f"🤖: {e}")
+```
+
+## Star History Chart:
+
+[![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.0/freeGPT/alpaca_7b.py` & `freeGPT-1.2.1/freeGPT/alpaca_7b.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import requests
 from fake_useragent import UserAgent
 
 
 class Completion:
+    """
+    A class for generating text completions using an API.
+
+    Attributes:
+        None
+
+    Methods:
+        create(prompt): Generates a text completion for the given prompt using an API.
+    """
+
     @staticmethod
     def create(prompt):
         """
-        Create a completion using a given prompt.
+        Generates a text completion for the given prompt using an API.
 
         Args:
-            prompt (str): The prompt for generating the completion.
+            prompt (str): The prompt for which to generate a text completion.
 
         Returns:
-            str: The generated completion.
+            str: The generated text completion.
 
         Raises:
-            Exception: If there is an error while fetching the response.
-
+            Exception: If there is an error fetching the response from the API.
         """
         try:
             resp = requests.post(
                 "https://us-central1-arched-keyword-306918.cloudfunctions.net/run-inference-1",
                 headers={
                     "Origin": "https://chatllama.baseten.co",
                     "Referer": "https://chatllama.baseten.co/",
```

### Comparing `freeGPT-1.2.0/freeGPT/c_a_l.py` & `freeGPT-1.2.1/freeGPT/gpt4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-import re, json
+import re
+import json
 import subprocess
 from uuid import uuid4
 from typing import Optional, List
 from fake_useragent import UserAgent
 
+try:
+    import tls_client
+except Exception:
+    subprocess.run(["pip", "install", "tls_client", "--no-cache-dir"])
+
 
 class Completion:
     @staticmethod
     def create(
         prompt,
         page: int = 1,
         count: int = 10,
@@ -46,20 +52,14 @@
         Raises:
             Exception: If unable to fetch the response.
         """
 
         if chat is None:
             chat = []
 
-        try:
-            import tls_client
-        except ImportError:
-            subprocess.run(["pip", "install", "tls_client", "--no-cache-dir"])
-            import tls_client
-
         client = tls_client.Session(client_identifier="chrome_108")
         client.headers = {
             "authority": "you.com",
             "accept": "text/event-stream",
             "accept-language": "en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3",
             "cache-control": "no-cache",
             "referer": "https://you.com/search?q=hi&tbm=youchat",
```

### Comparing `freeGPT-1.2.0/freeGPT/gpt4.py` & `freeGPT-1.2.1/freeGPT/gpt3.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 import json
 import requests
 
 
 class Completion:
-    """
-    A class that interacts with the Ava API to generate completions for prompts.
-    """
-
     @staticmethod
     def create(prompt):
         """
-        Generates a completion based on the given prompt.
+        Create a new completion based on the given prompt.
 
         Args:
-            prompt (str): The prompt text to generate a completion for.
+            prompt (str): The prompt to generate a completion for.
 
         Returns:
-            str: The generated completion response.
+            str: The generated completion.
 
         Raises:
-            Exception: If there is an error while fetching the response from the API.
+            Exception: If unable to fetch the response.
         """
         try:
-            resp = ""
-            with requests.post(
+            session = requests.Session()
+            resp_obj = session.post(
                 "https://ava-alpha-api.codelink.io/api/chat",
                 headers={"Content-Type": "application/json"},
-                data=json.dumps(
-                    {
-                        "model": "gpt-4",
-                        "temperature": 0.7,
-                        "stream": True,
-                        "messages": [
-                            {
-                                "role": "system",
-                                "content": "You are Ava, an AI assistant. You are running on GPT-4 by OpenAI.",
-                            },
-                            {"role": "user", "content": prompt},
-                        ],
-                    }
-                ),
-                stream=True,
-            ) as resp_obj:
-                resp_obj.raise_for_status()
-                for line in resp_obj.iter_lines():
-                    line_text = line.decode("utf-8").strip()
-                    if line_text.startswith("data:"):
-                        data = line_text[len("data:") :]
-                        try:
-                            data_json = json.loads(data)
-                            if "choices" in data_json:
-                                choices = data_json["choices"]
-                                for choice in choices:
-                                    if (
-                                        "finish_reason" in choice
-                                        and choice["finish_reason"] == "stop"
-                                    ):
-                                        break
-                                    if (
-                                        "delta" in choice
-                                        and "content" in choice["delta"]
-                                    ):
-                                        resp += choice["delta"]["content"]
-                        except json.JSONDecodeError:
-                            pass
-        except requests.exceptions.RequestException:
+                json={
+                    "model": "gpt-4",
+                    "temperature": 0.6,
+                    "stream": True,
+                    "messages": [
+                        {"role": "system", "content": "You are Ava, an AI assistant."},
+                        {"role": "user", "content": prompt},
+                    ],
+                },
+            )
+        except:
             raise Exception("Unable to fetch the response.")
-
+        resp = ""
+        for line in resp_obj.iter_lines():
+            line_text = line.decode("utf-8").strip()
+            if line_text.startswith("data:"):
+                data = line_text[len("data:") :]
+                try:
+                    data_json = json.loads(data)
+                    if "choices" in data_json:
+                        choices = data_json["choices"]
+                        for choice in choices:
+                            if (
+                                "finish_reason" in choice
+                                and choice["finish_reason"] == "stop"
+                            ):
+                                break
+                            if "delta" in choice and "content" in choice["delta"]:
+                                resp += choice["delta"]["content"]
+                except json.JSONDecodeError:
+                    pass
         return resp
```

### Comparing `freeGPT-1.2.0/setup.py` & `freeGPT-1.2.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.0",
-    description="freeGPT provides access to GPT and other models for free.",
+    version="1.2.1",
+    description="freeGPT provides free access to GPT3, GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
-        "ai-models",
-        "chatbot",
+        "deep-learning",
         "gpt4free",
+        "chatbot",
         "freegpt",
         "chatgpt",
         "python",
-        "alpaca",
         "openai",
-        "model",
-        "c-a-l",
+        "llama",
         "free",
-        "gpt3",
         "gpt4",
+        "gpt3",
         "gpt",
-        "py",
         "ai",
     ],
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
     packages=find_packages(),
     install_requires=[
         "requests",
         "fake-useragent",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
         "Issues": "https://github.com/Ruu3f/freeGPT/issues",
-        "Discord": "https://dsc.gg/ruu3fstudio",
+        "Discord": "https://discord.gg/XH6pUGkwRr",
     },
 )
```

