# Comparing `tmp/nonebot_plugin_poke-0.0.1.tar.gz` & `tmp/nonebot_plugin_poke-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.0.1.tar` & `nonebot_plugin_poke-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1091 2023-06-02 08:35:26.135574 nonebot_plugin_poke-0.0.1/LICENSE
--rw-r--r--   0        0        0     1066 2023-06-29 10:13:30.511526 nonebot_plugin_poke-0.0.1/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      793 2023-06-29 09:58:33.763718 nonebot_plugin_poke-0.0.1/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     1572 2023-06-29 10:13:16.973289 nonebot_plugin_poke-0.0.1/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      951 2023-06-29 10:14:13.075264 nonebot_plugin_poke-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-06-02 10:18:20.539396 nonebot_plugin_poke-0.0.1/README.md
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2923 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/README.md
+-rw-r--r--   0        0        0     3455 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     3786 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0      922 2023-06-30 07:50:04.957599 nonebot_plugin_poke-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.0.1/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.0.2/nonebot_plugin_poke/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from pathlib import Path
-from typing import Optional, Sequence,List
-
-from nonebot import get_driver
-from nonebot.log import logger
-from pydantic import BaseSettings, validator,Field
-
-
-class Config(BaseSettings):
-    bot_nickname: str = list[get_driver().config.nickname][0]
-    poke_black: bool = True
-    poke_ban_group:List[str] = []
-    poke_allow_group:List[str] = []
-    poke_send_pic: bool = False
-    poke_send_poke: bool = True
-    poke_send_text: bool = False
-    poke_send_acc: bool = False
-    poke_path:Path = Path('data/poke')
-
-
-    class Config:
-        extra = "ignore"
-
-
-config = Config.parse_obj(get_driver().config)
-
-
-if not config.poke_path.exists() or not config.poke_path.is_dir():
+from pathlib import Path
+from typing import List
+
+from nonebot import get_driver
+from nonebot.log import logger
+from pydantic import BaseSettings
+
+
+class Config(BaseSettings):
+    bot_nickname: str = '宁宁'
+    poke_black: bool = True
+    poke_ban_group:List[str] = []
+    poke_allow_group:List[str] = []
+    poke_send_pic: bool = False
+    poke_send_poke: bool = True
+    poke_send_text: bool = False
+    poke_send_acc: bool = False
+    poke_path:Path = Path('data/poke')
+    poke_priority:int = 1
+    poke_block:bool = True
+
+
+    class Config:
+        extra = "ignore"
+
+
+config = Config.parse_obj(get_driver().config)
+
+
+if not config.poke_path.exists() or not config.poke_path.is_dir():
     config.poke_path.mkdir(0o755, parents=True, exist_ok=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_poke-0.0.1/pyproject.toml` & `nonebot_plugin_poke-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-[tool.poetry]
-name = "nonebot_plugin_poke"
-version = "0.0.1"
-description = "nonebot_plugin_poke plugin for NoneBot2"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
-repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
-keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
-classifiers = [
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Operating System :: OS Independent",
-]
-include = [
-    "LICENSE","README.md"
-]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-nonebot2 = "^2.0.0"
-nonebot-adapter-onebot = ">=2.1.5"
-
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot_plugin_poke"
+version = "0.0.2"
+description = "群聊戳戳事件 plugin for NoneBot2"
+authors = ["Agnes_Digital <Z735803792@163.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
+repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
+keywords = ["nonebot2", "plugin","event"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+]
+include = [
+    "LICENSE","README.md"
+]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+nonebot2 = "^2.0.0"
+nonebot-adapter-onebot = ">=2.1.5"
+
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

