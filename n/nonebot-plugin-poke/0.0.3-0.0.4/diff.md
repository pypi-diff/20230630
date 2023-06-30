# Comparing `tmp/nonebot_plugin_poke-0.0.3.tar.gz` & `tmp/nonebot_plugin_poke-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_poke-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_poke-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_poke-0.0.3.tar` & `nonebot_plugin_poke-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/LICENSE
--rw-r--r--   0        0        0     2923 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/README.md
--rw-r--r--   0        0        0     3441 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/__init__.py
--rw-r--r--   0        0        0      753 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/config.py
--rw-r--r--   0        0        0     3895 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/utils.py
--rw-r--r--   0        0        0      922 2023-06-30 07:59:40.720669 nonebot_plugin_poke-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2923 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/README.md
+-rw-r--r--   0        0        0     3441 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/config.py
+-rw-r--r--   0        0        0     3895 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/utils.py
+-rw-r--r--   0        0        0      922 2023-06-30 08:05:20.938097 nonebot_plugin_poke-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 nonebot_plugin_poke-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_poke-0.0.3/LICENSE` & `nonebot_plugin_poke-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.3/README.md` & `nonebot_plugin_poke-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/__init__.py` & `nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 poke_ = on_notice(block=config.poke_block, 
-                  priority=config.poke_priority, rlue=poke_rule)
+                  priority=config.poke_priority, rule=poke_rule)
 
 
 
 @poke_.handle()
 async def _(event: PokeNotifyEvent,matcher:Matcher):
     await poke_send(event,matcher)
     await acc_send(matcher)
```

### Comparing `nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/config.py` & `nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.3/nonebot_plugin_poke/utils.py` & `nonebot_plugin_poke-0.0.4/nonebot_plugin_poke/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_poke-0.0.3/pyproject.toml` & `nonebot_plugin_poke-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_poke"
-version = "0.0.3"
+version = "0.0.4"
 description = "群聊戳戳事件 plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_poke"
 repository = "https://github.com/Agnes4m/nonebot_plugin_poke"
 keywords = ["nonebot2", "plugin","event"]
```

### Comparing `nonebot_plugin_poke-0.0.3/PKG-INFO` & `nonebot_plugin_poke-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-poke
-Version: 0.0.3
+Version: 0.0.4
 Summary: 群聊戳戳事件 plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_poke
 License: MIT
 Keywords: nonebot2,plugin,event
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-poke Version: 0.0.4 Summary:
 ç¾¤èæ³æ³äºä»¶ plugin for NoneBot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_poke License: MIT Keywords: nonebot2,plugin,event Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

