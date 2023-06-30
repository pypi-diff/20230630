# Comparing `tmp/nonebot-adapter-telegram-0.1.0b8.tar.gz` & `tmp/nonebot-adapter-telegram-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-adapter-telegram-0.1.0b8.tar", last modified: Fri Feb 10 07:13:24 2023, max compression
+gzip compressed data, was "nonebot-adapter-telegram-0.1.0b9.tar", last modified: Sun Mar 19 10:53:32 2023, max compression
```

## Comparing `nonebot-adapter-telegram-0.1.0b8.tar` & `nonebot-adapter-telegram-0.1.0b9.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-01-09 12:05:37.018804 nonebot-adapter-telegram-0.1.0b8/LICENSE
--rw-r--r--   0        0        0      304 2023-02-07 13:34:51.963072 nonebot-adapter-telegram-0.1.0b8/README.md
--rw-r--r--   0        0        0      196 2023-01-09 12:05:37.018804 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/__init__.py
--rw-r--r--   0        0        0     9083 2023-02-10 06:39:25.650289 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/adapter.py
--rw-r--r--   0        0        0    32256 2023-02-07 13:27:15.778223 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/api.py
--rw-r--r--   0        0        0     9726 2023-02-10 06:40:39.490852 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/bot.py
--rw-r--r--   0        0        0      969 2023-02-10 04:27:44.214856 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/config.py
--rw-r--r--   0        0        0    19265 2023-02-10 06:41:37.659294 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/event.py
--rw-r--r--   0        0        0     1353 2023-01-09 12:05:37.018804 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/exception.py
--rw-r--r--   0        0        0     9841 2023-02-10 06:40:39.490852 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/message.py
--rw-r--r--   0        0        0    36900 2023-02-07 11:29:54.715660 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/model.py
--rw-r--r--   0        0        0     1381 2023-01-14 08:49:08.158418 nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/permission.py
--rw-r--r--   0        0        0     1741 2023-02-10 06:58:39.891392 nonebot-adapter-telegram-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 nonebot-adapter-telegram-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-09-04 15:32:00.491246 nonebot-adapter-telegram-0.1.0b9/LICENSE
+-rw-r--r--   0        0        0      304 2023-02-20 12:39:16.061634 nonebot-adapter-telegram-0.1.0b9/README.md
+-rw-r--r--   0        0        0      196 2022-09-04 15:32:00.491246 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/__init__.py
+-rw-r--r--   0        0        0     8247 2023-03-15 11:28:00.330230 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/adapter.py
+-rw-r--r--   0        0        0    33433 2023-03-16 07:16:39.630986 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/api.py
+-rw-r--r--   0        0        0    11037 2023-03-19 10:37:55.712643 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/bot.py
+-rw-r--r--   0        0        0      969 2023-02-20 12:39:16.064967 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/config.py
+-rw-r--r--   0        0        0    19173 2023-03-15 13:08:35.241478 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/event.py
+-rw-r--r--   0        0        0     1353 2023-02-20 12:39:16.064967 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/exception.py
+-rw-r--r--   0        0        0     9946 2023-03-16 07:12:59.348152 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/message.py
+-rw-r--r--   0        0        0    37388 2023-03-16 06:08:33.255540 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/model.py
+-rw-r--r--   0        0        0     1381 2023-02-20 12:39:16.064967 nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/permission.py
+-rw-r--r--   0        0        0     2266 2023-03-19 10:43:27.625331 nonebot-adapter-telegram-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0    53248 2023-03-03 14:18:14.784727 nonebot-adapter-telegram-0.1.0b9/tests/.coverage
+-rw-r--r--   0        0        0      521 2023-03-03 13:25:16.142170 nonebot-adapter-telegram-0.1.0b9/tests/conftest.py
+-rw-r--r--   0        0        0    78913 2023-03-03 14:18:14.924726 nonebot-adapter-telegram-0.1.0b9/tests/coverage.xml
+-rw-r--r--   0        0        0     1061 2023-03-15 13:12:04.622147 nonebot-adapter-telegram-0.1.0b9/tests/test_bot.py
+-rw-r--r--   0        0        0     1506 2023-03-15 12:30:18.451648 nonebot-adapter-telegram-0.1.0b9/tests/test_event.py
+-rw-r--r--   0        0        0     1080 2023-03-15 12:30:11.314884 nonebot-adapter-telegram-0.1.0b9/tests/test_message.py
+-rw-r--r--   0        0        0     7357 2023-03-15 13:01:53.431936 nonebot-adapter-telegram-0.1.0b9/tests/updates.json
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 nonebot-adapter-telegram-0.1.0b9/PKG-INFO
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/LICENSE` & `nonebot-adapter-telegram-0.1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/adapter.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,26 +2,17 @@
 import asyncio
 import pathlib
 from typing import Any, Dict, List, cast
 
 from anyio import open_file
 from pydantic.main import BaseModel
 from nonebot.typing import overrides
-from nonebot.message import handle_event
 from pydantic.json import pydantic_encoder
 from nonebot.utils import escape_tag, logger_wrapper
-from nonebot.drivers import (
-    URL,
-    Driver,
-    Request,
-    Response,
-    ForwardDriver,
-    ReverseDriver,
-    HTTPServerSetup,
-)
+from nonebot.drivers import URL, Driver, Request, Response, HTTPServerSetup
 
 from nonebot.adapters import Adapter as BaseAdapter
 
 from .bot import Bot
 from .event import Event
 from .model import InputMedia
 from .config import BotConfig, AdapterConfig
@@ -49,116 +40,105 @@
         self.setup()
 
     @classmethod
     @overrides(BaseAdapter)
     def get_name(cls) -> str:
         return "Telegram"
 
-    def setup_webhook(self, bot_configs: List[BotConfig]):
+    def setup_webhook(self, bot: Bot):
         @self.driver.on_startup
         async def _():
-            async def handle_http(request: Request) -> Response:
-                token = request.headers.get("X-Telegram-Bot-Api-Secret-Token")
-                for bot in self.bots.values():
-                    bot = cast(Bot, bot)
-                    if bot.secret_token == token:
-                        if request.content:
-                            message: dict = json.loads(request.content)
-                            asyncio.create_task(
-                                handle_event(bot, Event.parse_event(message))
-                            )
-                        return Response(204)
-                return Response(401)
-
-            setup = HTTPServerSetup(
-                URL(f"/telegram"),
-                "POST",
-                self.get_name(),
-                handle_http,
-            )
-            self.setup_http_server(setup)
+            try:
+                bot.username = (await bot.get_me()).username
+                log("INFO", "Delete old webhook")
+                await bot.delete_webhook()
+                log("INFO", "Set new webhook")
+                await bot.set_webhook(
+                    url=f"{self.adapter_config.telegram_webhook_url}/telegram",
+                    secret_token=bot.secret_token,
+                )
+                self.bot_connect(bot)
+            except Exception as e:
+                log("ERROR", f"Setup for bot {bot.self_id} failed", e)
+
+    async def poll(self, bot: Bot):
+        try:
+            bot.username = (await bot.get_me()).username
+            log("INFO", "Delete old webhook")
+            await bot.delete_webhook()
+            log("INFO", "Start poll")
+            self.bot_connect(bot)
 
-            for bot_config in bot_configs:
-                bot = Bot(self, bot_config)
-                try:
-                    log("INFO", "Delete old webhook")
-                    await bot.delete_webhook()
-                    log("INFO", "Set new webhook")
-                    await bot.set_webhook(
-                        url=f"{self.adapter_config.telegram_webhook_url}/telegram",
-                        secret_token=bot.secret_token,
-                    )
-                    self.bot_connect(bot)
-
-                except Exception as e:
-                    log("ERROR", f"Setup for bot {bot.self_id} failed", e)
-
-    def setup_polling(self, bot_configs: List[BotConfig]):
-        @self.driver.on_startup
-        async def _():
-            async def poll(bot: Bot):
+            update_offset = None
+            while True:
                 try:
-                    log("INFO", "Delete old webhook")
-                    await bot.delete_webhook()
-                    log("INFO", "Start poll")
-                    self.bot_connect(bot)
-
-                    update_offset = None
-                    while True:
-                        try:
-                            message = await bot.get_updates(
-                                offset=update_offset, timeout=30
+                    updates = await bot.get_updates(offset=update_offset, timeout=30)
+                    if update_offset is not None:
+                        for update in updates:
+                            update_offset = update.update_id + 1
+                            event = Event.parse_event(
+                                update.dict(by_alias=True, exclude_none=True)
                             )
-                            if update_offset is not None:
-                                for msg in message:
-                                    update_offset = msg.update_id + 1
-                                    event = Event.parse_event(
-                                        msg.dict(by_alias=True, exclude_none=True)
+                            log(
+                                "DEBUG",
+                                escape_tag(
+                                    str(
+                                        event.dict(
+                                            exclude_none=True,
+                                            exclude={"telegram_model"},
+                                        )
                                     )
-                                    log(
-                                        "DEBUG",
-                                        escape_tag(
-                                            str(
-                                                event.dict(
-                                                    exclude_none=True,
-                                                    exclude={"telegram_model"},
-                                                )
-                                            )
-                                        ),
-                                    )
-                                    await handle_event(bot, event)
-                            elif message:
-                                update_offset = message[0].update_id
-                        except Exception as e:
-                            log("ERROR", f"Get updates for bot {bot.self_id} failed", e)
+                                ),
+                            )
+                            await bot.handle_event(event)
+                    elif updates:
+                        update_offset = updates[0].update_id
                 except Exception as e:
-                    log("ERROR", f"Setup for bot {bot.self_id} failed", e)
+                    log("ERROR", f"Get updates for bot {bot.self_id} failed", e)
+        except Exception as e:
+            log("ERROR", f"Setup for bot {bot.self_id} failed", e)
 
-            for bot_config in bot_configs:
-                self.tasks.append(asyncio.create_task(poll(Bot(self, bot_config))))
+    def setup_polling(self, bot: Bot):
+        @self.driver.on_startup
+        async def _():
+            self.tasks.append(asyncio.create_task(self.poll(bot)))
 
         @self.driver.on_shutdown
         async def _():
             for task in self.tasks:
                 if not task.done():
                     task.cancel()
             await asyncio.gather(*self.tasks, return_exceptions=True)
 
-    def setup(self) -> None:
-        polling_bot_configs = []
-        webhook_bot_configs = []
+    async def handle_http(self, request: Request) -> Response:
+        token = request.headers.get("X-Telegram-Bot-Api-Secret-Token")
+        for bot in self.bots.values():
+            bot = cast(Bot, bot)
+            if bot.secret_token == token:
+                if request.content:
+                    update: dict = json.loads(request.content)
+                    asyncio.create_task(bot.handle_event(Event.parse_event(update)))
+                return Response(204)
+        return Response(401)
 
+    def setup(self) -> None:
+        self.setup_http_server(
+            HTTPServerSetup(
+                URL("/telegram"),
+                "POST",
+                self.get_name(),
+                self.handle_http,
+            )
+        )
         for bot_config in self.adapter_config.telegram_bots:
+            bot = Bot(self, bot_config)
             if bot_config.is_webhook:
-                webhook_bot_configs.append(bot_config)
+                self.setup_webhook(bot)
             else:
-                polling_bot_configs.append(bot_config)
-
-        self.setup_webhook(webhook_bot_configs)
-        self.setup_polling(polling_bot_configs)
+                self.setup_polling(bot)
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data) -> Any:
         # 将方法名称改为驼峰式
         api = api.split("_", maxsplit=1)[0] + "".join(
             s.capitalize() for s in api.split("_")[1:]
         )
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/api.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,29 +14,32 @@
     ChatMember,
     ForceReply,
     ForumTopic,
     InputMedia,
     MenuButton,
     StickerSet,
     WebhookInfo,
+    InputSticker,
     LabeledPrice,
     MaskPosition,
     GameHighScore,
     MessageEntity,
+    BotDescription,
     ChatInviteLink,
     ShippingOption,
     BotCommandScope,
     ChatPermissions,
     InputMediaAudio,
     InputMediaPhoto,
     InputMediaVideo,
     InlineQueryResult,
     SentWebAppMessage,
     UserProfilePhotos,
     InputMediaDocument,
+    BotShortDescription,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
     InlineKeyboardMarkup,
     PassportElementError,
     ChatAdministratorRights,
 )
 
@@ -175,15 +178,15 @@
         message_thread_id: Optional[int] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[List[MessageEntity]] = None,
         duration: Optional[int] = None,
         performer: Optional[str] = None,
         title: Optional[str] = None,
-        thumb: Optional[Union[InputFile, str]] = None,
+        thumbnail: Optional[Union[InputFile, str]] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: Optional[bool] = None,
         reply_markup: Optional[
             Union[
                 InlineKeyboardMarkup,
@@ -196,15 +199,15 @@
         ...
 
     async def send_document(
         self,
         chat_id: Union[int, str],
         document: Union[InputFile, str],
         message_thread_id: Optional[int] = None,
-        thumb: Optional[Union[InputFile, str]] = None,
+        thumbnail: Optional[Union[InputFile, str]] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[List[MessageEntity]] = None,
         disable_content_type_detection: Optional[bool] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_to_message_id: Optional[int] = None,
@@ -224,15 +227,15 @@
         self,
         chat_id: Union[int, str],
         video: Union[InputFile, str],
         message_thread_id: Optional[int] = None,
         duration: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
-        thumb: Optional[Union[InputFile, str]] = None,
+        thumbnail: Optional[Union[InputFile, str]] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[List[MessageEntity]] = None,
         has_spoiler: Optional[bool] = None,
         supports_streaming: Optional[bool] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
@@ -253,15 +256,15 @@
         self,
         chat_id: Union[int, str],
         animation: Union[InputFile, str],
         message_thread_id: Optional[int] = None,
         duration: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
-        thumb: Optional[Union[InputFile, str]] = None,
+        thumbnail: Optional[Union[InputFile, str]] = None,
         caption: Optional[str] = None,
         parse_mode: Optional[str] = None,
         caption_entities: Optional[List[MessageEntity]] = None,
         has_spoiler: Optional[bool] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_to_message_id: Optional[int] = None,
@@ -304,15 +307,15 @@
     async def send_video_note(
         self,
         chat_id: Union[int, str],
         video_note: Union[InputFile, str],
         message_thread_id: Optional[int] = None,
         duration: Optional[int] = None,
         length: Optional[int] = None,
-        thumb: Optional[Union[InputFile, str]] = None,
+        thumbnail: Optional[Union[InputFile, str]] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: Optional[bool] = None,
         reply_markup: Optional[
             Union[
                 InlineKeyboardMarkup,
@@ -764,14 +767,36 @@
     async def get_my_commands(
         self,
         scope: Optional[BotCommandScope] = None,
         language_code: Optional[str] = None,
     ) -> List[BotCommand]:
         ...
 
+    async def set_my_description(
+        self, description: Optional[str] = None, language_code: Optional[str] = None
+    ) -> Literal[True]:
+        ...
+
+    async def get_my_description(
+        self, language_code: Optional[str] = None
+    ) -> BotDescription:
+        ...
+
+    async def set_my_short_description(
+        self,
+        short_description: Optional[str] = None,
+        language_code: Optional[str] = None,
+    ) -> Literal[True]:
+        ...
+
+    async def get_my_short_description(
+        self, language_code: Optional[str] = None
+    ) -> BotShortDescription:
+        ...
+
     async def set_chat_menu_button(
         self, chat_id: Optional[int] = None, menu_button: Optional[MenuButton] = None
     ) -> Literal[True]:
         ...
 
     async def get_chat_menu_button(self, chat_id: Optional[int] = None) -> MenuButton:
         ...
@@ -846,14 +871,15 @@
         ...
 
     async def send_sticker(
         self,
         chat_id: Union[int, str],
         sticker: Union[InputFile, str],
         message_thread_id: Optional[int] = None,
+        emoji: Optional[str] = None,
         disable_notification: Optional[bool] = None,
         protect_content: Optional[bool] = None,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: Optional[bool] = None,
         reply_markup: Optional[
             Union[
                 InlineKeyboardMarkup,
@@ -869,56 +895,78 @@
         ...
 
     async def get_custom_emoji_stickers(
         self, custom_emoji_ids: List[str]
     ) -> List[Sticker]:
         ...
 
-    async def upload_sticker_file(self, user_id: int, png_sticker: InputFile) -> File:
+    async def upload_sticker_file(
+        self, user_id: int, sticker: InputFile, sticker_format: str
+    ) -> File:
         ...
 
     async def create_new_sticker_set(
         self,
         user_id: int,
         name: str,
         title: str,
-        emojis: str,
-        png_sticker: Optional[Union[InputFile, str]] = None,
-        tgs_sticker: Optional[InputFile] = None,
-        webm_sticker: Optional[InputFile] = None,
+        stickers: List[InputSticker],
+        sticker_format: str,
         sticker_type: Optional[str] = None,
-        mask_position: Optional[MaskPosition] = None,
+        needs_repainting: Optional[bool] = None,
     ) -> Literal[True]:
         ...
 
     async def add_sticker_to_set(
         self,
         user_id: int,
         name: str,
-        emojis: str,
-        png_sticker: Optional[Union[InputFile, str]] = None,
-        tgs_sticker: Optional[InputFile] = None,
-        webm_sticker: Optional[InputFile] = None,
-        mask_position: Optional[MaskPosition] = None,
+        sticker: InputSticker,
     ) -> Literal[True]:
         ...
 
     async def set_sticker_position_in_set(
         self, sticker: str, position: int
     ) -> Literal[True]:
         ...
 
     async def delete_sticker_from_set(self, sticker: str) -> Literal[True]:
         ...
 
-    async def set_sticker_set_thumb(
-        self, name: str, user_id: int, thumb: Optional[Union[InputFile, str]] = None
+    async def set_sticker_emoji_list(
+        self, sticker: str, emoji_list: List[str]
     ) -> Literal[True]:
         ...
 
+    async def set_sticker_keywords(
+        self, sticker: str, keywords: Optional[List[str]] = None
+    ) -> Literal[True]:
+        ...
+
+    async def set_sticker_mask_position(
+        self, sticker: str, mask_position: Optional[MaskPosition] = None
+    ) -> Literal[True]:
+        ...
+
+    async def set_sticker_set_title(self, name: str, title: str) -> Literal[True]:
+        ...
+
+    async def set_sticker_set_thumbnail(
+        self, name: str, user_id: int, thumbnail: Optional[Union[InputFile, str]] = None
+    ) -> Literal[True]:
+        ...
+
+    async def set_custom_emoji_sticker_set_thumbnail(
+        self, name: str, custom_emoji_id: Optional[str] = None
+    ) -> Literal[True]:
+        ...
+
+    async def delete_sticker_set(self, name: str) -> Literal[True]:
+        ...
+
     async def answer_inline_query(
         self,
         inline_query_id: str,
         results: List[InlineQueryResult],
         cache_time: Optional[int] = None,
         is_personal: Optional[bool] = None,
         next_offset: Optional[str] = None,
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/bot.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/bot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,69 @@
 import inspect
 from uuid import uuid4
 from functools import partial
 from typing import Any, Union, Optional, cast
 
 from pydantic import parse_obj_as
 from nonebot.typing import overrides
+from nonebot.message import handle_event
 
 from nonebot.adapters import Adapter
 from nonebot.adapters import Bot as BaseBot
 
 from .api import API
 from .config import BotConfig
 from .exception import ApiNotAvailable
-from .event import Event, EventWithChat
 from .model import InputMedia, MessageEntity
+from .event import Event, MessageEvent, EventWithChat
 from .message import File, Entity, Message, UnCombinFile, MessageSegment
 
 
 class Bot(BaseBot, API):
     """
     Telegram Bot 适配。继承属性参考 `BaseBot <./#class-basebot>`_ 。
     """
 
     def __init__(self, adapter: "Adapter", config: BotConfig):
         self.adapter = adapter
         self.self_id = config.token.split(":")[0]
+        self.username: Optional[str] = None
         self.bot_config = config
         self.secret_token = uuid4().hex
 
+    def _check_tome(self, event: MessageEvent):
+        def process_first_segment(message: Message):
+            if not message:
+                message.append(Entity.text(""))
+            elif message[0].is_text():
+                message[0].data["text"] = message[0].data["text"].lstrip()
+                if not str(message[0]):
+                    del message[0]
+                    process_first_segment(message)
+
+        segment = event.message[0]
+        if segment.type == "mention":
+            if segment.data.get("text", "")[1:] == self.username:
+                del event.message[0]
+                process_first_segment(event.message)
+                event._tome = True
+        elif segment.type == "text":
+            text = str(segment)
+            for nickname in self.config.nickname:
+                if nickname in text:
+                    event.message[0].data["text"] = text.replace(nickname, "", 1)
+                    process_first_segment(event.message)
+                    event._tome = True
+                    break
+
+    async def handle_event(self, event: Event):
+        if isinstance(event, MessageEvent):
+            self._check_tome(event)
+        await handle_event(self, event)
+
     async def call_api(self, api: str, *args: Any, **kargs: Any) -> Any:
         if hasattr(API, api):
             sign = inspect.signature(getattr(API, api))
             args_ = list(args)
             for param in sign.parameters.values():
                 if param.name != "self" and param.name not in kargs:
                     try:
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/config.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/event.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     forward_date: Optional[int]
     via_bot: Optional[User]
     has_protected_content: Optional[Literal[True]]
     media_group_id: Optional[str]
     author_signature: Optional[str]
     reply_to_message: Optional["MessageEvent"] = None
     message: Message = Message()
+    _tome: bool = False
 
     @classmethod
     def __parse_event(cls, obj: dict) -> "Event":
         message = Message.parse_obj(obj)
         if not message:
             return NoticeEvent.parse_event(obj)
         else:
@@ -166,18 +167,17 @@
     def get_event_name(self) -> str:
         return "message"
 
     @overrides(Event)
     def get_message(self) -> Message:
         return self.message
 
-    # TODO
     @overrides(Event)
     def is_tome(self) -> bool:
-        return super().is_tome()
+        return self._tome
 
     @overrides(Event)
     def get_event_description(self) -> str:
         return f"Message {self.message_id} @[Chat {self.chat.id}]: {self.get_message_description()}"
 
 
 class PrivateMessageEvent(MessageEvent):
@@ -294,19 +294,14 @@
     def get_message(self) -> Message:
         return self.message
 
     @overrides(Event)
     def get_plaintext(self) -> str:
         return self.message.extract_plain_text()
 
-    # TODO
-    @overrides(Event)
-    def is_tome(self) -> bool:
-        return super().is_tome()
-
     @overrides(Event)
     def get_event_description(self) -> str:
         return f"EditedMessage {self.message_id} @[Chat {self.chat.id}]: {self.get_message_description()}"
 
 
 class PrivateEditedMessageEvent(EditedMessageEvent):
     from_: User = Field(alias="from")
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/exception.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/message.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -195,55 +195,58 @@
         file: Union[str, bytes],
     ) -> "MessageSegment":
         return File("voice", {"file": file})
 
     @staticmethod
     def animation(
         file: Union[str, bytes],
-        thumb: Union[None, str, bytes] = None,
+        thumbnail: Union[None, str, bytes] = None,
         has_spoiler: Optional[bool] = None,
     ) -> "MessageSegment":
         return File(
-            "animation", {"file": file, "thumb": thumb, "has_spoiler": has_spoiler}
+            "animation",
+            {"file": file, "thumbnail": thumbnail, "has_spoiler": has_spoiler},
         )
 
     @staticmethod
     def audio(
         file: Union[str, bytes],
-        thumb: Union[None, str, bytes] = None,
+        thumbnail: Union[None, str, bytes] = None,
     ) -> "MessageSegment":
-        return File("audio", {"file": file, "thumb": thumb})
+        return File("audio", {"file": file, "thumbnail": thumbnail})
 
     @staticmethod
     def document(
         file: Union[str, bytes],
-        thumb: Union[None, str, bytes] = None,
+        thumbnail: Union[None, str, bytes] = None,
     ) -> "MessageSegment":
-        return File("document", {"file": file, "thumb": thumb})
+        return File("document", {"file": file, "thumbnail": thumbnail})
 
     @staticmethod
     def video(
         file: Union[str, bytes],
-        thumb: Union[None, str, bytes] = None,
+        thumbnail: Union[None, str, bytes] = None,
         has_spoiler: Optional[bool] = None,
     ) -> "MessageSegment":
-        return File("video", {"file": file, "thumb": thumb, "has_spoiler": has_spoiler})
+        return File(
+            "video", {"file": file, "thumbnail": thumbnail, "has_spoiler": has_spoiler}
+        )
 
 
 class UnCombinFile(File):
     @staticmethod
     def sticker(file: Union[str, bytes]) -> "MessageSegment":
         return File("sticker", {"file": file})
 
     @staticmethod
     def video_note(
         file: Union[str, bytes],
-        thumb: Union[None, str, bytes] = None,
+        thumbnail: Union[None, str, bytes] = None,
     ) -> "MessageSegment":
-        return File("video_note", {"file": file, "thumb": thumb})
+        return File("video_note", {"file": file, "thumbnail": thumbnail})
 
 
 class Message(BaseMessage[MessageSegment]):
     def __repr__(self) -> str:
         return "".join(repr(seg) for seg in self)
 
     @classmethod
@@ -311,13 +314,13 @@
             elif key == "poll":
                 seg = MessageSegment(
                     key,
                     {"question": obj[key]["question"], "options": obj[key]["options"]},
                 )
             else:
                 continue
-            if isinstance(obj[key], dict) and obj[key].get("thumb", None):
-                kargs["thumb"] = obj["key"]["thumb"]["file_id"]
+            if isinstance(obj[key], dict) and obj[key].get("thumbnail", None):
+                kargs["thumbnail"] = obj[key]["thumbnail"]["file_id"]
             seg.data.update(kargs)
             msg.append(seg)
             del obj[key]
         return cls(msg)
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/model.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,18 +221,18 @@
     chat_shared: Optional["ChatShared"] = None
     connected_website: Optional[str] = None
     write_access_allowed: Optional["WriteAccessAllowed"] = None
     passport_data: Optional["PassportData"] = None
     proximity_alert_triggered: Optional["ProximityAlertTriggered"] = None
     forum_topic_created: Optional["ForumTopicCreated"] = None
     forum_topic_edited: Optional["ForumTopicEdited"] = None
-    general_forum_topic_hidden: Optional["GeneralForumTopicHidden"] = None
-    general_forum_topic_unhidden: Optional["GeneralForumTopicUnhidden"] = None
     forum_topic_closed: Optional["ForumTopicClosed"] = None
     forum_topic_reopened: Optional["ForumTopicReopened"] = None
+    general_forum_topic_hidden: Optional["GeneralForumTopicHidden"] = None
+    general_forum_topic_unhidden: Optional["GeneralForumTopicUnhidden"] = None
     video_chat_scheduled: Optional["VideoChatScheduled"] = None
     video_chat_started: Optional["VideoChatStarted"] = None
     video_chat_ended: Optional["VideoChatEnded"] = None
     video_chat_participants_invited: Optional["VideoChatParticipantsInvited"] = None
     web_app_data: Optional["WebAppData"] = None
     reply_markup: Optional["InlineKeyboardMarkup"] = None
 
@@ -261,59 +261,59 @@
 
 class Animation(BaseModel):
     file_id: str
     file_unique_id: str
     width: int
     height: int
     duration: int
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
     file_size: Optional[int] = None
 
 
 class Audio(BaseModel):
     file_id: str
     file_unique_id: str
     duration: int
     performer: Optional[str] = None
     title: Optional[str] = None
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
     file_size: Optional[int] = None
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
 
 
 class Document(BaseModel):
     file_id: str
     file_unique_id: str
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
     file_size: Optional[int] = None
 
 
 class Video(BaseModel):
     file_id: str
     file_unique_id: str
     width: int
     height: int
     duration: int
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
     file_size: Optional[int] = None
 
 
 class VideoNote(BaseModel):
     file_id: str
     file_unique_id: str
     length: int
     duration: int
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
     file_size: Optional[int] = None
 
 
 class Voice(BaseModel):
     file_id: str
     file_unique_id: str
     duration: int
@@ -732,14 +732,22 @@
 
 class BotCommandScopeChatMember(BotCommandScope):
     type: Literal["chat_member"] = "chat_member"
     chat_id: Union[int, str]
     user_id: int
 
 
+class BotDescription(BaseModel):
+    description: str
+
+
+class BotShortDescription(BaseModel):
+    short_description: str
+
+
 class MenuButton(BaseModel):
     type: str
 
 
 class MenuButtonCommands(MenuButton):
     type: Literal["commmands"] = "commmands"
 
@@ -773,42 +781,42 @@
 class InputMediaPhoto(InputMedia):
     type: Literal["photo"] = "photo"
     has_spoiler: Optional[bool] = None
 
 
 class InputMediaVideo(InputMedia):
     type: Literal["video"] = "video"
-    thumb: Optional[Union[InputFile, str]] = None
+    thumbnail: Optional[Union[InputFile, str]] = None
     width: Optional[int] = None
     height: Optional[int] = None
     duration: Optional[int] = None
     supports_streaming: Optional[bool] = None
     has_spoiler: Optional[bool] = None
 
 
 class InputMediaAnimation(InputMedia):
     type: Literal["animation"] = "animation"
-    thumb: Optional[Union[InputFile, str]] = None
+    thumbnail: Optional[Union[InputFile, str]] = None
     width: Optional[int] = None
     height: Optional[int] = None
     duration: Optional[int] = None
     has_spoiler: Optional[bool] = None
 
 
 class InputMediaAudio(InputMedia):
     type: Literal["audio"] = "audio"
-    thumb: Optional[Union[InputFile, str]] = None
+    thumbnail: Optional[Union[InputFile, str]] = None
     duration: Optional[int] = None
     performer: Optional[str] = None
     title: Optional[str] = None
 
 
 class InputMediaDocument(InputMedia):
     type: Literal["document"] = "document"
-    thumb: Optional[Union[InputFile, str]] = None
+    thumbnail: Optional[Union[InputFile, str]] = None
     disable_content_type_detection: Optional[bool] = None
 
 
 class MaskPosition(BaseModel):
     point: str
     x_shift: float
     y_shift: float
@@ -819,31 +827,39 @@
     file_id: str
     file_unique_id: str
     type: str
     width: int
     height: int
     is_animated: bool
     is_video: bool
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
     emoji: Optional[str] = None
     set_name: Optional[str] = None
     premium_animation: Optional[File] = None
     mask_position: Optional[MaskPosition] = None
     custom_emoji_id: Optional[str] = None
+    needs_repainting: Optional[Literal[True]] = None
     file_size: Optional[int] = None
 
 
 class StickerSet(BaseModel):
     name: str
     title: str
     sticker_type: str
     is_animated: bool
     is_video: bool
     stickers: List[Sticker]
-    thumb: Optional[PhotoSize] = None
+    thumbnail: Optional[PhotoSize] = None
+
+
+class InputSticker(BaseModel):
+    sticker: Union[InputFile, str]
+    emoji_list: List[str]
+    mask_position: Optional[MaskPosition] = None
+    keywords: Optional[List[str]] = None
 
 
 class InlineQuery(BaseModel):
     id: str
     from_: User = Field(alias="from")
     query: str
     offset: str
@@ -921,23 +937,23 @@
 class InlineQueryResultArticle(InlineQueryResult):
     type: Literal["article"] = "article"
     title: str
     input_message_content: InputMessageContent
     url: Optional[str] = None
     hide_url: Optional[bool] = None
     description: Optional[str] = None
-    thumb_url: Optional[str] = None
-    thumb_width: Optional[int] = None
-    thumb_height: Optional[int] = None
+    thumbnail_url: Optional[str] = None
+    thumbnail_width: Optional[int] = None
+    thumbnail_height: Optional[int] = None
 
 
 class InlineQueryResultPhoto(InlineQueryResult):
     type: Literal["photo"] = "photo"
     photo_url: str
-    thumb_url: str
+    thumbnail_url: str
     photo_width: Optional[int] = None
     photo_height: Optional[int] = None
     title: Optional[str] = None
     description: Optional[str] = None
     caption: Optional[str] = None
     parse_mode: Optional[str] = None
     caption_entities: Optional[List[MessageEntity]] = None
@@ -946,43 +962,43 @@
 
 class InlineQueryResultGif(InlineQueryResult):
     type: Literal["gif"] = "gif"
     gif_url: str
     gif_width: Optional[int] = None
     gif_height: Optional[int] = None
     gif_duration: Optional[int] = None
-    thumb_url: str
-    thumb_mime_type: Optional[str] = None
+    thumbnail_url: str
+    thumbnail_mime_type: Optional[str] = None
     title: Optional[str] = None
     caption: Optional[str] = None
     parse_mode: Optional[str] = None
     caption_entities: Optional[List[MessageEntity]] = None
     input_message_content: Optional[InputMessageContent] = None
 
 
 class InlineQueryResultMpeg4Gif(InlineQueryResult):
     type: Literal["mpeg4_gif"] = "mpeg4_gif"
     mpeg4_url: str
     mpeg4_width: Optional[int] = None
     mpeg4_height: Optional[int] = None
     mpeg4_duration: Optional[int] = None
-    thumb_url: str
-    thumb_mime_type: Optional[str] = None
+    thumbnail_url: str
+    thumbnail_mime_type: Optional[str] = None
     title: Optional[str] = None
     caption: Optional[str] = None
     parse_mode: Optional[str] = None
     caption_entities: Optional[List[MessageEntity]] = None
     input_message_content: Optional[InputMessageContent] = None
 
 
 class InlineQueryResultVideo(InlineQueryResult):
     type: Literal["video"] = "video"
     video_url: str
     mime_type: str
-    thumb_url: str
+    thumbnail_url: str
     title: str
     caption: Optional[str] = None
     parse_mode: Optional[str] = None
     caption_entities: Optional[List[MessageEntity]] = None
     video_width: Optional[int] = None
     video_height: Optional[int] = None
     video_duration: Optional[int] = None
@@ -1019,61 +1035,61 @@
     caption: Optional[str] = None
     parse_mode: Optional[str] = None
     caption_entities: Optional[List[MessageEntity]] = None
     document_url: str
     mime_type: str
     description: Optional[str] = None
     input_message_content: Optional[InputMessageContent] = None
-    thumb_url: Optional[str] = None
-    thumb_width: Optional[int] = None
-    thumb_height: Optional[int] = None
+    thumbnail_url: Optional[str] = None
+    thumbnail_width: Optional[int] = None
+    thumbnail_height: Optional[int] = None
 
 
 class InlineQueryResultLocation(InlineQueryResult):
     type: Literal["location"] = "location"
     latitude: float
     longitude: float
     title: str
     horizontal_accuracy: Optional[float] = None
     live_period: Optional[int] = None
     heading: Optional[int] = None
     proximity_alert_radius: Optional[int] = None
     input_message_content: Optional[InputMessageContent] = None
-    thumb_url: Optional[str] = None
-    thumb_width: Optional[int] = None
-    thumb_height: Optional[int] = None
+    thumbnail_url: Optional[str] = None
+    thumbnail_width: Optional[int] = None
+    thumbnail_height: Optional[int] = None
 
 
 class InlineQueryResultVenue(InlineQueryResult):
     type: Literal["venue"] = "venue"
     latitude: float
     longitude: float
     title: str
     address: str
     foursquare_id: Optional[str] = None
     foursquare_type: Optional[str] = None
     google_place_id: Optional[str] = None
     google_place_type: Optional[str] = None
     input_message_content: Optional[InputMessageContent] = None
-    thumb_url: Optional[str] = None
-    thumb_width: Optional[int] = None
-    thumb_height: Optional[int] = None
+    thumbnail_url: Optional[str] = None
+    thumbnail_width: Optional[int] = None
+    thumbnail_height: Optional[int] = None
 
 
 class InlineQueryResultContact(InlineQueryResult):
     type: Literal["contact"] = "contact"
     phone_number: str
     first_name: str
     last_name: Optional[str] = None
     user_id: Optional[int] = None
     vcard: Optional[str] = None
     input_message_content: Optional[InputMessageContent] = None
-    thumb_url: Optional[str] = None
-    thumb_width: Optional[int] = None
-    thumb_height: Optional[int] = None
+    thumbnail_url: Optional[str] = None
+    thumbnail_width: Optional[int] = None
+    thumbnali_height: Optional[int] = None
 
 
 class InlineQueryResultGame(InlineQueryResult):
     type: Literal["game"] = "game"
     game_short_name: str
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/nonebot/adapters/telegram/permission.py` & `nonebot-adapter-telegram-0.1.0b9/nonebot/adapters/telegram/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot-adapter-telegram-0.1.0b8/pyproject.toml` & `nonebot-adapter-telegram-0.1.0b9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-adapter-telegram"
-version = "0.1.0b8"
+version = "0.1.0b9"
 description = "Telegram Adapter for NoneBot2"
 authors = [
     { name = "Jigsaw", email = "j1g5aw@foxmail.com" },
 ]
 dependencies = [
     "nonebot2<3.0.0,>=2.0.0b1",
     "anyio<4.0.0,>=3.6.2",
@@ -33,23 +33,30 @@
 documentation = "https://github.com/nonebot/adapter-telegram/blob/beta/MANUAL.md"
 changelog = "https://github.com/nonebot/adapter-telegram/blob/beta/CHANGELOG.md"
 
 [tool.pdm.dev-dependencies]
 nonebot = [
     "httpx<1.0.0,>=0.23.0",
     "fastapi<1.0.0,>=0.89.0",
+    "uvicorn>=0.12.0,<0.21.0",
     "nonebot2 @ git+https://github.com/nonebot/nonebot2.git",
 ]
 pre-commit = [
     "pycln",
     "isort",
     "black",
     "nonemoji",
     "pre-commit",
 ]
+tests = [
+    "nonebug>=0.3.1",
+    "pytest-asyncio>=0.20.3",
+    "pytest-cov>=4.0.0",
+    "pytest-xdist>=3.2.0",
+]
 
 [tool.pdm.build]
 includes = [
     "nonebot",
 ]
 
 [tool.black]
@@ -73,17 +80,36 @@
     "typing_extensions",
 ]
 
 [tool.pycln]
 path = "."
 all = false
 
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+addopts = "--cov nonebot.adapters.telegram --cov-report term-missing"
+
 [tool.pyright]
+reportShadowedImports = false
+pythonVersion = "3.8"
+pythonPlatform = "All"
+extraPaths = [
+    "__pypackages__/3.10/lib",
+]
 exclude = [
     "__pypackages__",
 ]
 
+[[tool.pyright.executionEnvironments]]
+root = "./tests"
+extraPaths = [
+    "./",
+]
+
+[[tool.pyright.executionEnvironments]]
+root = "./"
+
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `nonebot-adapter-telegram-0.1.0b8/PKG-INFO` & `nonebot-adapter-telegram-0.1.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-telegram
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: Telegram Adapter for NoneBot2
 License: MIT
 Keywords: bot,telegram
 Author-email: Jigsaw <j1g5aw@foxmail.com>
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
```

