# Comparing `tmp/villa-0.4.1.tar.gz` & `tmp/villa-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.4.1.tar", max compression
+gzip compressed data, was "villa-0.5.0.tar", max compression
```

## Comparing `villa-0.4.1.tar` & `villa-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-06-26 12:48:39.029785 villa-0.4.1/LICENSE
--rw-r--r--   0        0        0     2844 2023-06-26 12:48:39.029785 villa-0.4.1/README.md
--rw-r--r--   0        0        0     1034 2023-06-26 12:48:39.029785 villa-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      285 2023-06-26 12:48:39.029785 villa-0.4.1/villa/__init__.py
--rw-r--r--   0        0        0    38462 2023-06-26 12:48:39.033785 villa-0.4.1/villa/bot.py
--rw-r--r--   0        0        0    10676 2023-06-26 12:48:39.033785 villa-0.4.1/villa/event.py
--rw-r--r--   0        0        0      473 2023-06-26 12:48:39.033785 villa-0.4.1/villa/exception.py
--rw-r--r--   0        0        0     1504 2023-06-26 12:48:39.033785 villa-0.4.1/villa/log.py
--rw-r--r--   0        0        0    17127 2023-06-26 12:48:39.033785 villa-0.4.1/villa/message.py
--rw-r--r--   0        0        0     8899 2023-06-26 12:48:39.033785 villa-0.4.1/villa/models.py
--rw-r--r--   0        0        0      935 2023-06-26 12:48:39.033785 villa-0.4.1/villa/store.py
--rw-r--r--   0        0        0      822 2023-06-26 12:48:39.033785 villa-0.4.1/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-26 12:48:39.033785 villa-0.4.1/villa/utils.py
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 villa-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-30 14:59:51.787095 villa-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3428 2023-06-30 14:59:51.787095 villa-0.5.0/README.md
+-rw-r--r--   0        0        0     1034 2023-06-30 14:59:51.787095 villa-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-06-30 14:59:51.787095 villa-0.5.0/villa/__init__.py
+-rw-r--r--   0        0        0    36288 2023-06-30 14:59:51.791095 villa-0.5.0/villa/bot.py
+-rw-r--r--   0        0        0    10774 2023-06-30 14:59:51.791095 villa-0.5.0/villa/event.py
+-rw-r--r--   0        0        0      728 2023-06-30 14:59:51.791095 villa-0.5.0/villa/exception.py
+-rw-r--r--   0        0        0     3177 2023-06-30 14:59:51.791095 villa-0.5.0/villa/handle.py
+-rw-r--r--   0        0        0     1524 2023-06-30 14:59:51.791095 villa-0.5.0/villa/log.py
+-rw-r--r--   0        0        0    17127 2023-06-30 14:59:51.791095 villa-0.5.0/villa/message.py
+-rw-r--r--   0        0        0     8899 2023-06-30 14:59:51.791095 villa-0.5.0/villa/models.py
+-rw-r--r--   0        0        0      935 2023-06-30 14:59:51.791095 villa-0.5.0/villa/store.py
+-rw-r--r--   0        0        0      240 2023-06-30 14:59:51.791095 villa-0.5.0/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-06-30 14:59:51.791095 villa-0.5.0/villa/utils.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 villa-0.5.0/PKG-INFO
```

### Comparing `villa-0.4.1/LICENSE` & `villa-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.4.1/README.md` & `villa-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -16,68 +16,67 @@
   <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078.svg" alt="wakatime">
 </a>
 
 </div>
 
 ## 特性
 
-- 基于`FastAPI`和`Pydantic`，异步、快速、高性能！
-- 完整的类型注解支持
-- 便捷的消息构造和发送方法
-- 丰富的消息段和完整的API支持
-- ~~想不出来了~~
+- 基于`FastAPI`和`Pydantic`，异步优先、快速、高性能！
+- 完整的类型注解支持，便于开发。
+- 便捷的消息构造和发送方法。
+- 完整的消息段和API支持。
+- `Serverless`云函数支持。
+- More ~~想不出来了~~
 
 ## 安装
 
-- 使用pip: `pip install villa`
-- 使用poetry: `poetry add villa`
-- 使用pdm: `pdm add villa`
+- 使用 pip: `pip install villa`
+- 使用 poetry: `poetry add villa`
+- 使用 pdm: `pdm add villa`
 
 ## 快速开始
 
-首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到[机器人开发者社区](https://dby.miyoushe.com/chat/463/20020)(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
+你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的 Bot，可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)(ID: `OpenVilla`)申请，取得`bot_id`、`bot_secret`。
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
-bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url")
-# 初始化Bot，填写你的bot_id、密钥以及回调地址
+bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url_endpoint")
+# 初始化Bot，填写你的bot_id、密钥以及回调地址endpoint
+# 举例：若申请时提供的回调地址为https://域名/callback，这里的callback_url就填`/callback`
 
 @bot.on_startswith("hello")
 async def handler(event: SendMessageEvent):
     await event.send("world!")
-    # 一个简单的处理函数，向你的Bot发送`@Bot hello`，它将会回复你`world`！
+    # 一个简单的处理函数，向你的Bot发送包含`hello`关键词的消息，它将会回复你`world`！
 
 
 if __name__ == "__main__":
     bot.run(host="127.0.0.1", port=13350)
-    # 启动bot，注意，port端口号要和你的回调地址对上
+    # 启动bot，注意，port端口号要和你的回调地址端口对上
 ```
 
 
-## 使用说明
+## 示例
 
-详见`example`文件夹：
-- `single_bot.py`: 单Bot运行
-- `multiple_bots.py`: 多Bot运行
-- `handle_func.py`: 各种处理器介绍
-- `send_message.py`: 各种消息发送方法介绍
+详见 [example](https://github.com/CMHopeSunshine/villa-py/tree/main/example) 文件夹：
 
+- [单 Bot 运行](https://github.com/CMHopeSunshine/villa-py/blob/main/example/single_bot.py)
+- [多 Bot 运行](https://github.com/CMHopeSunshine/villa-py/blob/main/example/multiple_bots.py)
+- [处理器介绍](https://github.com/CMHopeSunshine/villa-py/blob/main/example/handle_func.py)
+- [消息发送方法](https://github.com/CMHopeSunshine/villa-py/blob/main/example/send_message.py)
+- [vercel serverless 部署](https://github.com/CMHopeSunshine/villa-py/blob/main/example/vercel.py)
 
-## 反馈
+## 交流、建议和反馈
 
-目前无论是大别野Bot还是本SDK都在测试开发中，如遇问题请提出issue，感谢支持！
+> 注意：本SDK并非官方SDK
 
-也欢迎来我的大别野【尘世闲游】进行交流~ 
+大别野 Bot 和本 SDK 均为开发测试中，如遇问题请提出 [issue](https://github.com/CMHopeSunshine/villa-py/issues) ，感谢支持！
 
-- 大别野ID: wgiJNaU
-- [Web端链接](https://dby.miyoushe.com/chat/1047/21652)
+也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~ 
 
 ## 相关项目
 
-- [NoneBot2](https://github.com/nonebot/nonebot2) 非常好用的Python跨平台机器人框架！
-- [nonebot-adapter-villa](https://github.com/CMHopeSunshine/nonebot-adapter-villa) NoneBot2的大别野Bot适配器。
-
-推荐有成熟Python开发经验但对NoneBot2不熟悉的小伙伴选择`本SDK`，
-
-对NoneBot2熟悉或希望接触更成熟的生态的小伙伴选择`NoneBot2+Villa适配器`进行开发。
+- [NoneBot2](https://github.com/nonebot/nonebot2) 非常好用的 Python 跨平台机器人框架！
+- [nonebot-adapter-villa](https://github.com/CMHopeSunshine/nonebot-adapter-villa) NoneBot2 的大别野 Bot 适配器。
+- [Herta-villa-SDK](https://github.com/MingxuanGame/Herta-villa-SDK) 另一个大别野 Python SDK。
```

### Comparing `villa-0.4.1/pyproject.toml` & `villa-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.4.1"
+version = "0.5.0"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.4.1/villa/bot.py` & `villa-0.5.0/villa/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 import re
 import asyncio
 from itertools import product
-from typing import Any, Set, Dict, List, Type, Union, Literal, Optional
+from collections import defaultdict
+from typing import Any, Set, Dict, List, Type, Union, Literal, Optional, DefaultDict
 
 import httpx
 import uvicorn
 from pydantic import parse_obj_as
 from fastapi.responses import JSONResponse
 from fastapi import FastAPI, BackgroundTasks
 
 from .models import *
 from .message import Message
-from .exception import ActionFailed
+from .utils import escape_tag
+from .handle import EventHandler
 from .message import MessageSegment
 from .log import logger, _log_patcher
-from .utils import run_sync, escape_tag
+from .typing import T_Func, T_Handler
 from .message import Link as LinkSegment
 from .message import Post as PostSegment
 from .message import Text as TextSegment
 from .message import Image as ImageSegment
 from .store import get_app, get_bot, store_bot
 from .message import RoomLink as RoomLinkSegment
-from .typing import T_Func, T_Handler, EventHandler
+from .exception import ActionFailed, StopPropagation
 from .message import MentionAll as MentionAllSegment
 from .message import MentionUser as MentionUserSegment
 from .message import MentionRobot as MentionRobotSegment
 from .event import Event, SendMessageEvent, event_classes, pre_handle_event
 
 
 class Bot:
     """Villa Bot"""
 
-    _event_handlers: List[EventHandler] = []
+    _event_handlers: DefaultDict[int, List[EventHandler]] = defaultdict(list)
+    """事件处理函数"""
     _client: httpx.AsyncClient
     bot_id: str
     """机器人 Id"""
     bot_secret: str
     """机器人密钥"""
     callback_url: str
     """事件回调地址"""
+    wait_util_complete: bool = False
+    """是否等待事件处理全部完成后再响应"""
     _bot_info: Optional[Robot] = None
     """机器人信息"""
 
-    def __init__(self, bot_id: str, bot_secret: str, callback_url: str):
+    def __init__(
+        self,
+        bot_id: str,
+        bot_secret: str,
+        callback_url: str,
+        wait_util_complete: bool = False,
+    ):
         """初始化一个 Bot 实例
 
         参数:
             bot_id: 机器人 ID
             bot_secret: 机器人密钥
             callback_url: 事件回调地址
         """
-        self.bot_id: str = bot_id
-        self.bot_secret: str = bot_secret
-        self.callback_url: str = callback_url
+        self.bot_id = bot_id
+        self.bot_secret = bot_secret
+        self.callback_url = callback_url
+        self.wait_util_complete = wait_util_complete
         self._client = httpx.AsyncClient(
             base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/"
         )
         store_bot(self)
 
     @property
     def nickname(self) -> str:
@@ -103,20 +115,19 @@
         参数:
             *event_type: 事件类型列表.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
         def _decorator(func: T_Handler) -> T_Handler:
-            self._event_handlers.append(
+            self._event_handlers[priority].append(
                 EventHandler(
                     event_type=event_type, func=func, block=block, priority=priority
                 )
             )
-            self._event_handlers.sort(key=lambda x: x.priority)
             return func
 
         return _decorator
 
     def on_message(self, block: bool = False, priority: int = 1):
         """注册一个消息事件处理函数
 
@@ -124,23 +135,22 @@
 
         参数:
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
         def _decorator(func: T_Handler) -> T_Handler:
-            self._event_handlers.append(
+            self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                 )
             )
-            self._event_handlers.sort(key=lambda x: x.priority)
             return func
 
         return _decorator
 
     def on_startswith(
         self,
         *startswith: str,
@@ -159,24 +169,23 @@
             priority: 优先级. 默认为 1.
         """
         if isinstance(prefix, str):
             prefix = {prefix}
         startswith = tuple(set(p + s for p, s in list(product(prefix, startswith))))
 
         def _decorator(func: T_Handler) -> T_Handler:
-            self._event_handlers.append(
+            self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     startswith=startswith or None,
                 )
             )
-            self._event_handlers.sort(key=lambda x: x.priority)
             return func
 
         return _decorator
 
     def on_endswith(self, *endswith: str, block: bool = False, priority: int = 1):
         """注册一个消息事件处理函数
 
@@ -185,24 +194,23 @@
         参数:
             *endswith: 字符串列表.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
         def _decorator(func: T_Handler) -> T_Handler:
-            self._event_handlers.append(
+            self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     endswith=endswith or None,
                 )
             )
-            self._event_handlers.sort(key=lambda x: x.priority)
             return func
 
         return _decorator
 
     def on_keyword(self, *keywords: str, block: bool = False, priority: int = 1):
         """注册一个消息事件处理函数
 
@@ -211,24 +219,23 @@
         参数:
             *keywords: 关键词列表.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
         def _decorator(func: T_Handler) -> T_Handler:
-            self._event_handlers.append(
+            self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     keywords=keywords or None,
                 )
             )
-            self._event_handlers.sort(key=lambda x: x.priority)
             return func
 
         return _decorator
 
     def on_regex(
         self, pattern: Union[str, re.Pattern], block: bool = False, priority: int = 1
     ):
@@ -241,24 +248,23 @@
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
         if isinstance(pattern, str):
             pattern = re.compile(pattern)
 
         def _decorator(func: T_Handler) -> T_Handler:
-            self._event_handlers.append(
+            self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     regex=pattern,
                 )
             )
-            self._event_handlers.sort(key=lambda x: x.priority)
             return func
 
         return _decorator
 
     async def send(
         self, villa_id: int, room_id: int, message: Union[str, Message, MessageSegment]
     ) -> str:
@@ -872,60 +878,28 @@
     async def _handle_event(self, event: Event):
         """处理事件
 
         参数:
             event: 事件
         """
         is_handled = False
-        for event_handler in self._event_handlers:
-            if isinstance(event, event_handler.event_type):
-                if isinstance(event, SendMessageEvent):
-                    if (
-                        event_handler.startswith is not None
-                        and not event.message.startswith(event_handler.startswith)
-                    ):
-                        logger.opt(colors=True).trace(
-                            f"<b><y>[{event.__class__.__name__}]</y></b> not startswith \"{'|'.join(event_handler.startswith)}\", pass"
-                        )
-                        continue
-                    if (
-                        event_handler.endswith is not None
-                        and not event.message.endswith(event_handler.endswith)
-                    ):
-                        logger.opt(colors=True).trace(
-                            f"<b><y>[{event.__class__.__name__}]</y></b> not endswith \"{'|'.join(event_handler.endswith)}\", pass"
-                        )
-                        continue
-                    if event_handler.keywords is not None and not any(
-                        keyword in event.message for keyword in event_handler.keywords
-                    ):
-                        logger.opt(colors=True).trace(
-                            f"<b><y>[{event.__class__.__name__}]</y></b> not contains \"{'|'.join(event_handler.keywords)}\", pass"
-                        )
-                        continue
-                    if event_handler.regex is not None and not event.message.match(
-                        event_handler.regex
-                    ):
-                        logger.opt(colors=True).trace(
-                            f'<b><y>[{event.__class__.__name__}]</y></b> not match "{event_handler.regex}", <y>pass</y>'
-                        )
-                        continue
-                logger.opt(colors=True).info(
-                    f"<b><y>[{event.__class__.__name__}]</y></b> will be handled by <y>{event_handler}</y>"
+        for priority in sorted(self._event_handlers.keys()):
+            try:
+                await asyncio.gather(
+                    *[handler._run(event) for handler in self._event_handlers[priority]]
                 )
-                await run_handler(event_handler, event)
                 is_handled = True
-                if event_handler.block:
-                    logger.opt(colors=True).debug(
-                        f"<b><y>[{event.__class__.__name__}]</y></b> stop handled by <y>{event_handler}</y>"
-                    )
-                    break
+            except StopPropagation as e:
+                logger.opt(colors=True).debug(
+                    f"<b><y>[{event.__class__.__name__}]</y></b> stop handled by <y>{e.handler}</y>"
+                )
+                break
         if is_handled:
             logger.opt(colors=True).success(
-                f"<b><y>[{event.__class__.__name__}]</y></b> handle completed"
+                f"{event.get_event_name()} handle completed"
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
         """解析消息内容"""
         if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
 
@@ -1171,29 +1145,19 @@
         logger.opt(exception=e).warning(
             f"Failed to parse payload {escape_tag(str(payload_data))}"
         )
         return JSONResponse(
             status_code=400, content={"retcode": -1, "msg": "Invalid data"}
         )
     else:
-        backgroud_tasks.add_task(bot._handle_event, event=event)
-    return JSONResponse(status_code=200, content={"retcode": 0, "message": "success"})
-
-
-async def run_handler(handler: EventHandler, event: Event):
-    """运行事件处理器"""
-    try:
-        if asyncio.iscoroutinefunction(handler.func):
-            await handler.func(event)
+        if bot.wait_util_complete:
+            await bot._handle_event(event=event)
         else:
-            await run_sync(handler.func)(event)
-    except Exception as e:
-        logger.opt(exception=e).error(
-            f"Error when running {handler} for {event.__class__.__name__}"
-        )
+            backgroud_tasks.add_task(bot._handle_event, event=event)
+    return JSONResponse(status_code=200, content={"retcode": 0, "message": "success"})
 
 
 def on_startup(func: T_Func):
     """让函数在 APP 启动时运行
 
     参数:
         func: 无参函数
```

### Comparing `villa-0.4.1/villa/event.py` & `villa-0.5.0/villa/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     """事件回调时间"""
 
     @property
     def bot_id(self) -> str:
         """机器人ID"""
         return self.robot.template.id
 
+    def get_event_name(self) -> str:
+        return f"<b><y>[{self.__class__.__name__}]</y></b>"
+
     def get_event_description(self) -> str:
         return escape_tag(str(self.dict()))
 
 
 class JoinVillaEvent(Event):
     """新用户加入大别野事件
 
@@ -211,15 +214,15 @@
         """
         if (bot := get_bot(self.bot_id)) is None:
             raise ValueError(f"Bot {self.bot_id} not found. Cannot send message.")
         if isinstance(message, (str, MessageSegment)):
             message = Message(message)
         if mention_sender:
             message.insert(
-                0, MessageSegment.mention_user(self.from_user_id, self.villa_id)
+                0, MessageSegment.mention_user(self.villa_id, self.from_user_id)
             )
         if quote_message:
             message.append(MessageSegment.quote(self.msg_uid, self.send_at))
         return await bot.send(self.villa_id, self.room_id, message)
 
 
 class CreateRobotEvent(Event):
```

### Comparing `villa-0.4.1/villa/log.py` & `villa-0.5.0/villa/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,11 +49,12 @@
     record["name"] = record["name"].split(".")[0]  # type: ignore
 
 
 logger.remove()
 logger_id = logger.add(
     sys.stdout,
     level=0,
-    diagnose=False,
+    diagnose=True,
+    backtrace=False,
     filter=default_filter,
     format=default_format,
 )
```

### Comparing `villa-0.4.1/villa/message.py` & `villa-0.5.0/villa/message.py`

 * *Files identical despite different names*

### Comparing `villa-0.4.1/villa/models.py` & `villa-0.5.0/villa/models.py`

 * *Files identical despite different names*

### Comparing `villa-0.4.1/villa/store.py` & `villa-0.5.0/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.4.1/villa/utils.py` & `villa-0.5.0/villa/utils.py`

 * *Files identical despite different names*

