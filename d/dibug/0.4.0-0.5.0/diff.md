# Comparing `tmp/dibug-0.4.0.tar.gz` & `tmp/dibug-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibug-0.4.0.tar", max compression
+gzip compressed data, was "dibug-0.5.0.tar", max compression
```

## Comparing `dibug-0.4.0.tar` & `dibug-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1076 2023-06-11 04:47:47.416881 dibug-0.4.0/LICENSE
--rw-r--r--   0        0        0     1450 2023-06-11 04:47:47.416881 dibug-0.4.0/README.md
--rw-r--r--   0        0        0       66 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/__init__.py
--rw-r--r--   0        0        0      286 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/abc.py
--rw-r--r--   0        0        0      195 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/__init__.py
--rw-r--r--   0        0        0     1740 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/eval.py
--rw-r--r--   0        0        0     1688 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/info.py
--rw-r--r--   0        0        0      361 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/kill.py
--rw-r--r--   0        0        0     1392 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/commands/shell.py
--rw-r--r--   0        0        0     4206 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/dibugger.py
--rw-r--r--   0        0        0        0 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/py.typed
--rw-r--r--   0        0        0      143 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/__init__.py
--rw-r--r--   0        0        0      470 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/chunk.py
--rw-r--r--   0        0        0      641 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/embed.py
--rw-r--r--   0        0        0      808 2023-06-11 04:47:47.416881 dibug-0.4.0/dibug/utils/object.py
--rw-r--r--   0        0        0      780 2023-06-11 04:47:47.416881 dibug-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 dibug-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-30 02:31:28.764861 dibug-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1353 2023-06-30 02:31:28.764861 dibug-0.5.0/README.md
+-rw-r--r--   0        0        0       66 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/__init__.py
+-rw-r--r--   0        0        0      228 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/abc.py
+-rw-r--r--   0        0        0      195 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/eval.py
+-rw-r--r--   0        0        0     1694 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/info.py
+-rw-r--r--   0        0        0      286 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/kill.py
+-rw-r--r--   0        0        0     1317 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/shell.py
+-rw-r--r--   0        0        0     5350 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/dibugger.py
+-rw-r--r--   0        0        0        0 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/py.typed
+-rw-r--r--   0        0        0      143 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/__init__.py
+-rw-r--r--   0        0        0      470 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/chunk.py
+-rw-r--r--   0        0        0      675 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/embed.py
+-rw-r--r--   0        0        0      808 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/object.py
+-rw-r--r--   0        0        0      780 2023-06-30 02:31:28.768861 dibug-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 dibug-0.5.0/PKG-INFO
```

### Comparing `dibug-0.4.0/LICENSE` & `dibug-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dibug-0.4.0/README.md` & `dibug-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,24 +25,19 @@
 owners = [1234567890]  # owners id
 
 
 async def user_has_perm(msg: Message) -> bool:
     return msg.author.id in owners
 
 
-class Bot(Client):
-    def __init__(self) -> None:
-        intents = Intents.default()
-        intents.message_content = True  # dibug requires message content intent
-        super().__init__(intents=intents)
+intents = Intents.default()
+intents.message_content = True  # dibug requires message content intent
 
-
-bot = Bot()
-
-dibugger = Dibugger(bot, user_has_perm)
+bot = Client(intents=intents)
+Dibugger.attach(bot, user_has_perm)
 
 bot.run("token")
 ```
 
 # Commands
 
 ### Default Prefix: `!dbg`
```

### Comparing `dibug-0.4.0/dibug/commands/eval.py` & `dibug-0.5.0/dibug/commands/eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..abc import DibugCommandABC
 from ..utils import DibugEmbed, inspect
 
 
 class EvalCommand(DibugCommandABC):
     def __init__(self, name: list[str], client: Client) -> None:
-        self.name = name
+        super().__init__(name)
 
         self.__client = client
 
     async def execute(self, msg: Message, args: str) -> None:
         if not args:
             await msg.reply("Missing code")
             return
```

### Comparing `dibug-0.4.0/dibug/commands/info.py` & `dibug-0.5.0/dibug/commands/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from psutil import Process
 
 from ..abc import DibugCommandABC
 
 
 class InfoCommand(DibugCommandABC):
     def __init__(self, name: list[str], client: Client) -> None:
-        self.name = name
+        super().__init__(name)
 
         self.__client = client
 
     async def execute(self, msg: Message, args: str) -> None:
         lines: list[str] = []
 
         lines.append(f"Python `{version}` on `{system()} {release()} ({platform})`")
```

### Comparing `dibug-0.4.0/dibug/commands/shell.py` & `dibug-0.5.0/dibug/commands/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from discord import Message
 
 from ..abc import DibugCommandABC
 from ..utils import DibugEmbed
 
 
 class ShellCommand(DibugCommandABC):
-    def __init__(self, name: list[str]) -> None:
-        self.name = name
-
     async def execute(self, msg: Message, args: str) -> None:
         if not args:
             await msg.reply("Missing code")
             return
 
         res = await msg.reply("Running...")
```

### Comparing `dibug-0.4.0/dibug/dibugger.py` & `dibug-0.5.0/dibug/dibugger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Callable, Coroutine, Literal, Type
 
 from discord import Client, Message
 
 from .abc import DibugCommandABC
 from .commands import EvalCommand, InfoCommand, KillCommand, ShellCommand
 
@@ -26,25 +28,37 @@
         Whether to patch the client on init, by default True.
         If False, you will have to manually call :meth:`handle_msg` on every message, and every edited message if you want.
 
     Methods
     -------
     handle_msg(msg: Message)
         Handle a message and execute the command if it exists.
+
+    Class Methods
+    --------------
+    attach(
+        client: Client,
+        user_has_perm: Callable[[Message], Coroutine[Any, Any, bool]],
+        no_perm_msg: str = "No Permission",
+        prefix: str = "!dbg",
+        default: Literal["info", "kill"] = "info",
+        patch_on_init: bool = True,
+    ) -> Dibugger
+        Attach a debugger to a discord.py client.
     """
 
     def __init__(
         self,
         client: Client,
         user_has_perm: Callable[[Message], Coroutine[Any, Any, bool]],
         no_perm_msg: str = "No Permission",
         prefix: str = "!dbg",
         default: Literal["info", "kill"] = "info",
         patch_on_init: bool = True,
-    ):
+    ) -> None:
         self.client = client
         self.user_has_perm = user_has_perm
         self.no_perm_msg = no_perm_msg
         self.prefix = prefix
         self.default = default
         self.patch_on_init = patch_on_init
 
@@ -52,51 +66,70 @@
 
         self._register_command(EvalCommand, ["eval", "e", "python", "py"], self.client)
         self._register_command(InfoCommand, ["info", "i"], self.client)
         self._register_command(KillCommand, ["kill", "k", "shutdown"])
         self._register_command(ShellCommand, ["shell", "sh"])
 
         if self.patch_on_init:
-            if hasattr(self.client, "on_message"):
-                original_func = getattr(self.client, "on_message")
-
-                async def on_message_patch(msg: Message) -> None:
-                    await original_func(msg)
-                    await self.handle_msg(msg)
-
-            else:
-
-                async def on_message_patch(msg: Message) -> None:
-                    await self.handle_msg(msg)
-
-            setattr(self.client, "on_message", on_message_patch)
-
-            if hasattr(self.client, "on_message_edit"):
-                original_func = getattr(self.client, "on_message_edit")
-
-                async def on_message_edit_patch(
-                    before: Message, after: Message
-                ) -> None:
-                    await original_func(before, after)
-                    await self.handle_msg(after)
+            setattr(self.client, "on_message", self.handle_msg)
 
-            else:
+            async def handle_edited_msg(_: Any, after: Message) -> None:
+                await self.handle_msg(after)
 
-                async def on_message_edit_patch(
-                    before: Message, after: Message
-                ) -> None:
-                    await self.handle_msg(after)
-
-            setattr(self.client, "on_message_edit", on_message_edit_patch)
+            setattr(self.client, "on_message_edit", handle_edited_msg)
 
     def _register_command(
         self, command: Type[DibugCommandABC], name: list[str], *args: Any, **kwargs: Any
     ) -> None:
         self._commands.append(command(name, *args, **kwargs))
 
+    @classmethod
+    def attach(
+        cls,
+        client: Client,
+        user_has_perm: Callable[[Message], Coroutine[Any, Any, bool]],
+        no_perm_msg: str = "No Permission",
+        prefix: str = "!dbg",
+        default: Literal["info", "kill"] = "info",
+        patch_on_init: bool = True,
+    ) -> Dibugger:
+        """
+        Attach a debugger to a discord.py client.
+
+        Parameters
+        ----------
+        client : Client
+            The discord.py client to attach the debugger to.
+        user_has_perm : Callable[[Message], Coroutine[Any, Any, bool]]
+            A function that returns whether the user has permission to use the debugger.
+        no_perm_msg : str, optional
+            The message to send when the user doesn't have permission, by default "No Permission".
+        prefix : str, optional
+            The prefix for the debugger, by default "!dbg".
+        default : Literal["info", "kill"], optional
+            The default command to run when no command is specified, command shouldn't have any arguments, by default "info".
+        patch_on_init : bool, optional
+            Whether to patch the client on init, by default True.
+            If False, you will have to manually call :meth:`handle_msg` on every message, and every edited message if you want.
+
+        Returns
+        -------
+        Dibugger
+            The debugger that was attached.
+        """
+
+        return cls(
+            client,
+            user_has_perm,
+            no_perm_msg,
+            prefix,
+            default,
+            patch_on_init,
+        )
+
     async def handle_msg(self, msg: Message) -> None:
         """
         Handle a message and execute the command if it exists.
 
         Parameters
         ----------
         msg : Message
```

### Comparing `dibug-0.4.0/dibug/utils/embed.py` & `dibug-0.5.0/dibug/utils/embed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 from discord import Embed
 
 from .chunk import chunk_string
 
 
 class DibugEmbed(Embed):
     def __init__(
         self,
         title: str,
         error: bool = False,
     ):
         super().__init__(title=title, color=0xFF0000 if error else 0x2B2D31)
 
-    def chunked_fields(self, name: str, value: str, lang: str) -> "DibugEmbed":
+    def chunked_fields(self, name: str, value: str, lang: str) -> DibugEmbed:
         chunked = chunk_string(value, 1024 - (8 + len(lang)))
         for idx in range(len(chunked)):
             self.add_field(
                 name=f"{name} ({idx + 1}/{len(chunked)})",
                 value=f"```{lang}\n{chunked[idx]}```",
                 inline=False,
             )
```

### Comparing `dibug-0.4.0/dibug/utils/object.py` & `dibug-0.5.0/dibug/utils/object.py`

 * *Files identical despite different names*

### Comparing `dibug-0.4.0/pyproject.toml` & `dibug-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dibug"
-version = "0.4.0"
+version = "0.5.0"
 description = "Debugging Tool for discord.py"
 authors = ["Starcea <stardev.uwu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/star0202/dibug"
 
 [tool.poetry.dependencies]
```

### Comparing `dibug-0.4.0/PKG-INFO` & `dibug-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dibug
-Version: 0.4.0
+Version: 0.5.0
 Summary: Debugging Tool for discord.py
 Home-page: https://github.com/star0202/dibug
 License: MIT
 Author: Starcea
 Author-email: stardev.uwu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,24 +44,19 @@
 owners = [1234567890]  # owners id
 
 
 async def user_has_perm(msg: Message) -> bool:
     return msg.author.id in owners
 
 
-class Bot(Client):
-    def __init__(self) -> None:
-        intents = Intents.default()
-        intents.message_content = True  # dibug requires message content intent
-        super().__init__(intents=intents)
+intents = Intents.default()
+intents.message_content = True  # dibug requires message content intent
 
-
-bot = Bot()
-
-dibugger = Dibugger(bot, user_has_perm)
+bot = Client(intents=intents)
+Dibugger.attach(bot, user_has_perm)
 
 bot.run("token")
 ```
 
 # Commands
 
 ### Default Prefix: `!dbg`
```

