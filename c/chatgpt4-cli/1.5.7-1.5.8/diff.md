# Comparing `tmp/chatgpt4-cli-1.5.7.tar.gz` & `tmp/chatgpt4-cli-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.7.tar", last modified: Wed May 24 10:10:20 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.8.tar", last modified: Fri Jun 30 08:32:52 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.7.tar` & `chatgpt4-cli-1.5.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32364 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:10:20.186661 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 10:10:20.000000 chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 10:10:20.190662 chatgpt4-cli-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-24 10:09:54.000000 chatgpt4-cli-1.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:32:52.096710 chatgpt4-cli-1.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:32:52.096710 chatgpt4-cli-1.5.8/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32381 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-06-30 08:32:52.096710 chatgpt4-cli-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:32:52.096710 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-06-30 08:32:52.000000 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-30 08:32:52.000000 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:32:52.000000 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 08:32:52.000000 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-30 08:32:52.000000 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 08:32:52.000000 chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 08:32:52.096710 chatgpt4-cli-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-30 08:32:25.000000 chatgpt4-cli-1.5.8/setup.py
```

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.8/GPTCLI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.7"
+__version__ = "1.5.8"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 __info__ = "Interact with ChatGPT and Bard at the terminal."
 
 import logging
 
 logging.basicConfig(
```

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/addons.py` & `chatgpt4-cli-1.5.8/GPTCLI/addons.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/bard.py` & `chatgpt4-cli-1.5.8/GPTCLI/bard.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/emage.py` & `chatgpt4-cli-1.5.8/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.8/GPTCLI/gptcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python
 from . import __version__, __author__, __repo__, __info__
 from colorama import Fore, Back
-from os import getlogin, getcwd, path
+from os import getcwd, path
+from getpass import getuser
 from rich.console import Console
 from rich.panel import Panel
 from rich.style import Style
 from rich import print as rich_print
 import argparse
 
 
@@ -172,15 +173,15 @@
             default="yellow",
             metavar="[cyan|green|yellow|red]",
             choices=self.colors,
         )
         parser.add_argument(
             "--prompt",
             help="Customizes the prompt display",
-            default=f"┌─[{getlogin().capitalize()}@GPT-CLI]─(%H:%M:%S)",
+            default=f"┌─[{getuser().capitalize()}@GPT-CLI]─(%H:%M:%S)",
             dest="settings",
             nargs="*",
         )
         parser.add_argument(
             "-tm",
             "--timeout",
             help="Request timeout while making request - (Soon)",
```

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/helper.py` & `chatgpt4-cli-1.5.8/GPTCLI/helper.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.7/GPTCLI/image.py` & `chatgpt4-cli-1.5.8/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.7/LICENSE` & `chatgpt4-cli-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.7/PKG-INFO` & `chatgpt4-cli-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.7
+Version: 1.5.8
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.7&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.8&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.7 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.8 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
```

### Comparing `chatgpt4-cli-1.5.7/README.md` & `chatgpt4-cli-1.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.7&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.8&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
```

### Comparing `chatgpt4-cli-1.5.7/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.8/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.7
+Version: 1.5.8
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.7&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.8&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.7 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.8 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
```

### Comparing `chatgpt4-cli-1.5.7/setup.py` & `chatgpt4-cli-1.5.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from setuptools import setup
-from GPTCLI import __version__, __author__, __repo__, __info__
+
+__version__ = "1.5.8"
+__author__ = "Smartwa Caleb"
+__repo__ = "https://github.com/Simatwa/gpt-cli"
+__info__ = "Interact with ChatGPT and Bard at the terminal."
 
 setup(
     name="chatgpt4-cli",
     packages=["GPTCLI"],
     version=__version__,
     license="MIT",
     author=__author__,
@@ -16,15 +20,15 @@
         "numpy>=1.23.4",
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
         "appdirs>=1.4.4",
         "requests>=2.28.2",
         "tabulate>=0.9.0",
-        "GoogleBard==1.0.3",
+        "GoogleBard==1.4.0",
         "fpdf==1.7.2",
     ],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```

