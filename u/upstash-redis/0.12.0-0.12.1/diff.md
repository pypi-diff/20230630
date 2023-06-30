# Comparing `tmp/upstash_redis-0.12.0.tar.gz` & `tmp/upstash_redis-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.12.0.tar", max compression
+gzip compressed data, was "upstash_redis-0.12.1.tar", max compression
```

## Comparing `upstash_redis-0.12.0.tar` & `upstash_redis-0.12.1.tar`

### file list

```diff
@@ -1,20 +1,27 @@
--rw-r--r--   0        0        0     1070 2023-05-24 07:39:12.527702 upstash_redis-0.12.0/LICENSE
--rw-r--r--   0        0        0     7813 2023-05-24 11:55:45.148047 upstash_redis-0.12.0/README.md
--rw-r--r--   0        0        0      386 2023-05-24 11:56:05.200030 upstash_redis-0.12.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 07:40:32.115270 upstash_redis-0.12.0/upstash_redis/__init__.py
--rw-r--r--   0        0        0    84603 2023-05-24 11:50:50.648380 upstash_redis-0.12.0/upstash_redis/client.py
--rw-r--r--   0        0        0      283 2023-05-24 11:43:41.923117 upstash_redis-0.12.0/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-05-24 07:40:32.115728 upstash_redis-0.12.0/upstash_redis/exception.py
--rw-r--r--   0        0        0      764 2023-05-24 07:40:32.115822 upstash_redis-0.12.0/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     2937 2023-05-24 11:51:41.605298 upstash_redis-0.12.0/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      214 2023-05-24 09:14:08.037410 upstash_redis-0.12.0/upstash_redis/play.py
--rw-r--r--   0        0        0        0 2023-05-24 07:40:32.115926 upstash_redis-0.12.0/upstash_redis/py.typed
--rw-r--r--   0        0        0      409 2023-05-24 07:40:32.116182 upstash_redis-0.12.0/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1119 2023-05-24 07:40:32.116295 upstash_redis-0.12.0/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      743 2023-05-24 11:43:31.886615 upstash_redis-0.12.0/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-05-24 07:40:32.116436 upstash_redis-0.12.0/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-05-24 07:40:32.116534 upstash_redis-0.12.0/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-05-24 07:40:32.116604 upstash_redis-0.12.0/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3339 2023-05-24 07:40:32.116678 upstash_redis-0.12.0/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     4133 2023-05-24 07:40:32.116752 upstash_redis-0.12.0/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     8292 1970-01-01 00:00:00.000000 upstash_redis-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis-0.12.1/LICENSE
+-rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis-0.12.1/README.md
+-rw-r--r--   0        0        0      387 2023-06-30 21:00:18.275936 upstash_redis-0.12.1/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-30 10:23:27.543198 upstash_redis-0.12.1/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-29 09:51:44.031185 upstash_redis-0.12.1/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4603 2023-06-30 18:46:43.369679 upstash_redis-0.12.1/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     4790 2023-06-30 18:55:39.814269 upstash_redis-0.12.1/upstash_redis/client.py
+-rw-r--r--   0        0        0       98 2023-06-29 09:49:58.469586 upstash_redis-0.12.1/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-30 14:20:06.203122 upstash_redis-0.12.1/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    22281 2023-06-30 14:06:30.500480 upstash_redis-0.12.1/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    71995 2023-06-30 17:28:46.668722 upstash_redis-0.12.1/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    21313 2023-06-30 14:14:41.609808 upstash_redis-0.12.1/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0    83861 2023-06-30 14:05:28.406050 upstash_redis-0.12.1/upstash_redis/commands-old.py
+-rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis-0.12.1/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis-0.12.1/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-06-22 15:12:55.454825 upstash_redis-0.12.1/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     5478 2023-06-30 18:56:49.908728 upstash_redis-0.12.1/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-06-22 15:12:55.456040 upstash_redis-0.12.1/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1174 2023-06-22 15:12:55.456402 upstash_redis-0.12.1/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-06-22 15:12:55.456727 upstash_redis-0.12.1/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis-0.12.1/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      172 2023-06-29 13:07:48.827924 upstash_redis-0.12.1/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis-0.12.1/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis-0.12.1/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-06-22 15:12:55.457479 upstash_redis-0.12.1/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     8827 2023-06-30 17:25:24.184093 upstash_redis-0.12.1/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9751 1970-01-01 00:00:00.000000 upstash_redis-0.12.1/PKG-INFO
```

### Comparing `upstash_redis-0.12.0/LICENSE` & `upstash_redis-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.0/README.md` & `upstash_redis-0.12.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Upstash Rate Limit - python edition
+# Upstash Redis - python edition
 
 upstash-redis is a connectionless, HTTP-based Redis client for python, designed to be used in serverless and serverful environments such as:
 - AWS Lambda
 - Google Cloud Functions
 - and other environments where HTTP is preferred over TCP.
 
 Inspired by other Redis clients like [@upstash/redis](https://github.com/upstash/upstash-redis) and [redis-py](https://github.com/redis/redis-py),
@@ -14,14 +14,17 @@
 
 <!-- toc -->
 
 - [Quick Start](#quick-start)
   - [Install](#install)
     - [PyPi](#PyPi)
   - [Usage](#usage)
+    - [Command groups](#command-groups)
+    - [BITFIELD and BITFIELD_RO](#bitfield-and-bitfieldro)
+    - [Custom commands](#custom-commands)
   - [Telemetry](#telemetry)
 - [Encoding](#encoding)
 - [Retry mechanism](#retry-mechanism)
 - [Formatting returns](#formatting-returns)
 - [Contributing](#contributing)
   - [Preparing the environment](#preparing-the-environment)
   - [Config](#config)
@@ -87,14 +90,57 @@
         await redis.set("a", "b")
         print(await redis.get("a"))
 
 run(main())
 
 ```
 
+### Command groups
+Most of the command groups, such as `PUBSUB` and `SCRIPT`, are available as an instance attribute of the `Redis` class.
+
+```python
+await redis.pubsub.channels()
+
+await redis.script.flush(mode="ASYNC")
+```
+
+
+### BITFIELD and BITFIELD_RO
+One particular case is represented by these two chained commands, which are available as functions that return an instance of 
+the `BITFIELD` and, respectively, `BITFIELD_RO` classes. Use the `execute` function to run the commands.
+
+```python
+await (
+    redis.bitfield("test_key")
+    .incrby(encoding="i8", offset=100, increment=100)
+    .overflow("SAT")
+    .incrby(encoding="i8", offset=100, increment=100)
+    .execute()
+)
+
+await (
+    redis.bitfield_ro("test_key_2")
+    .get(encoding="u8", offset=0)
+    .get(encoding="u8", offset="#1")
+    .execute()
+)
+```
+
+
+### Custom commands
+If you want to run a command that hasn't been implemented, you can use the `run` function of your client instance
+and pass the command as `list`
+
+```python
+await redis.run(command=["XLEN", "test_stream"])
+```
+
+If you want to have more control over your session management or need to use multiple custom values, use
+the [execute](./upstash_redis/http/execute.py) function directly.
+
 
 # Telemetry
 The SDK can collect the following anonymous telemetry:
   - the runtime (ex: `python@v.3.10.0`)
   - the SDK or SDKs you're using (ex: `upstash-redisy@development, upstash-ratelimit@v.0.1.0`)
   - the platform you're running on (ex: `AWS-lambda`)
```

### Comparing `upstash_redis-0.12.0/upstash_redis/client.py` & `upstash_redis-0.12.1/upstash_redis/commands-old.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,58 +2,62 @@
 from upstash_redis.schema.http import RESTResult, RESTEncoding
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.config import (
     REST_ENCODING,
     REST_RETRIES,
     REST_RETRY_INTERVAL,
     ALLOW_TELEMETRY,
-    FORMAT_RETURN
+    FORMAT_RETURN,
 )
 from upstash_redis.utils.format import (
     format_geo_positions_return,
     format_geo_members_return,
     format_hash_return,
     format_pubsub_numsub_return,
     format_bool_list,
     format_server_time_return,
     format_sorted_set_return,
-    format_float_list
+    format_float_list,
 )
 from upstash_redis.utils.exception import (
     handle_geosearch_exceptions,
     handle_non_deprecated_zrange_exceptions,
     handle_zrangebylex_exceptions,
-    handle_georadius_write_exceptions
+    handle_georadius_write_exceptions,
 )
 from upstash_redis.utils.comparison import number_are_not_none
-from upstash_redis.schema.commands.parameters import BitFieldOffset, GeoMember, FloatMinMax
+from upstash_redis.schema.commands.parameters import (
+    BitFieldOffset,
+    GeoMember,
+    FloatMinMax,
+)
 from upstash_redis.schema.commands.returns import (
     GeoMembersReturn,
     FormattedGeoMembersReturn,
     HashReturn,
     FormattedHashReturn,
     SortedSetReturn,
-    FormattedSortedSetReturn
+    FormattedSortedSetReturn,
 )
 from aiohttp import ClientSession
-from typing import Type, Any, Literal
+from typing import Type, Any, Literal, Union, List, Dict
 from os import environ
 
 
-class Redis:
+class Commands:
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
-        telemetry_data: TelemetryData | None = None
+        telemetry_data: Union[TelemetryData, None] = None,
     ):
         """
         :param url: UPSTASH_REDIS_REST_URL in the console
         :param token: UPSTASH_REDIS_REST_TOKEN in the console
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
@@ -70,23 +74,36 @@
 
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
         self.telemetry_data = telemetry_data
 
+        # See https://redis.io/commands/pubsub/
+        self.pubsub = PubSub(client=self)
+
+        # See https://redis.io/commands/script/
+        self.script = Script(client=self)
+
+        """
+        Need to double-check compatibility with the classic Redis API for this one.
+        
+        See https://redis.io/commands/acl
+        self.acl = ACL(client=self)
+        """
+
     @classmethod
     def from_env(
         cls,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
-        telemetry_data: TelemetryData | None = None
+        telemetry_data: Union[TelemetryData, None] = None,
     ):
         """
         Load the credentials from environment.
 
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
@@ -98,59 +115,66 @@
             environ["UPSTASH_REDIS_REST_URL"],
             environ["UPSTASH_REDIS_REST_TOKEN"],
             rest_encoding,
             rest_retries,
             rest_retry_interval,
             format_return,
             allow_telemetry,
-            telemetry_data
+            telemetry_data,
         )
 
     async def __aenter__(self) -> ClientSession:
         """
         Enter the async context.
         """
 
         self._session: ClientSession = ClientSession()
         # It needs to return the session object because it will be used in "async with" statements.
         return self._session
 
-    async def __aexit__(self, exc_type: Type[BaseException] | None, exc_val: BaseException | None, exc_tb: Any) -> None:
+    async def __aexit__(
+        self,
+        exc_type: Union[Type[BaseException], None],
+        exc_val: Union[BaseException, None],
+        exc_tb: Any,
+    ) -> None:
         """
         Exit the async context.
         """
 
         await self._session.close()
 
-    async def run(self, command: list) -> RESTResult:
+    async def run(self, command: List) -> RESTResult:
         """
         Specify the http options and execute the command.
         """
 
         return await execute(
             session=self._session,
             url=self.url,
             token=self.token,
             encoding=self.rest_encoding,
             retries=self.rest_retries,
             retry_interval=self.rest_retry_interval,
             command=command,
             allow_telemetry=self.allow_telemetry,
-            telemetry_data=self.telemetry_data
+            telemetry_data=self.telemetry_data,
         )
 
-    async def bitcount(self, key: str, start: int | None = None, end: int | None = None) -> int:
+    async def bitcount(
+        self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
+    ) -> int:
         """
         See https://redis.io/commands/bitcount
         """
 
         if number_are_not_none(start, end, number=1):
-            raise Exception("Both \"start\" and \"end\" must be specified.")
+            raise Exception('Both "start" and "end" must be specified.')
 
-        command: list = ["BITCOUNT", key]
+        command: List = ["BITCOUNT", key]
 
         if start is not None:
             command.extend([start, end])
 
         return await self.run(command)
 
     def bitfield(self, key: str) -> "BitFieldCommands":
@@ -164,98 +188,105 @@
         """
         See https://redis.io/commands/bitfield_ro
         """
 
         return BitFieldRO(key=key, client=self)
 
     async def bitop(
-        self,
-        operation: Literal["AND", "OR", "XOR", "NOT"],
-        destination_key: str,
-        *source_keys: str
+        self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *srckeys: str
     ) -> int:
         """
         See https://redis.io/commands/bitop
         """
 
-        if len(source_keys) == 0:
+        if len(srckeys) == 0:
             raise Exception("At least one source key must be specified.")
 
-        if operation == "NOT" and len(source_keys) > 1:
-            raise Exception("The \"NOT \" operation takes only one source key as argument.")
+        if operation == "NOT" and len(srckeys) > 1:
+            raise Exception(
+                'The "NOT " operation takes only one source key as argument.'
+            )
 
-        command: list = ["BITOP", operation, destination_key, *source_keys]
+        command: List = ["BITOP", operation, destkey, *srckeys]
 
         return await self.run(command)
 
-    async def bitpos(self, key: str, bit: Literal[0, 1], start: int | None = None, end: int | None = None) -> int:
+    async def bitpos(
+        self,
+        key: str,
+        bit: Literal[0, 1],
+        start: Union[int, None] = None,
+        end: Union[int, None] = None,
+    ) -> int:
         """
         See https://redis.io/commands/bitpos
         """
 
         if start is None and end is not None:
-            raise Exception("\"end\" is specified, but \"start\" is missing.")
+            raise Exception('"end" is specified, but "start" is missing.')
 
-        command: list = ["BITPOS", key, bit]
+        command: List = ["BITPOS", key, bit]
 
         if start is not None:
             command.append(start)
 
         if end is not None:
             command.append(end)
 
         return await self.run(command)
 
     async def getbit(self, key: str, offset: int) -> int:
         """
         See https://redis.io/commands/getbit
         """
 
-        command: list = ["GETBIT", key, offset]
+        command: List = ["GETBIT", key, offset]
 
         return await self.run(command)
 
     async def setbit(self, key: str, offset: int, value: Literal[0, 1]) -> int:
         """
         See https://redis.io/commands/setbit
         """
 
-        command: list = ["SETBIT", key, offset, value]
+        command: List = ["SETBIT", key, offset, value]
 
         return await self.run(command)
 
-    async def ping(self, message: str | None = None) -> str:
+    async def ping(self, message: Union[str, None] = None) -> str:
         """
         See https://redis.io/commands/ping
         """
 
-        command: list = ["PING"]
+        command: List = ["PING"]
 
         if message is not None:
             command.append(message)
 
         return await self.run(command)
 
     async def echo(self, message: str) -> str:
         """
         See https://redis.io/commands/echo
         """
 
-        command: list = ["ECHO", message]
+        command: List = ["ECHO", message]
 
         return await self.run(command)
 
-    async def copy(self, source: str, destination: str, replace: bool = False) -> Literal[1, 0] | bool:
+    async def copy(
+        self, source: str, destination: str, replace: bool = False
+    ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/copy
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["COPY", source, destination]
+        command: List = ["COPY", source, destination]
 
         if replace:
             command.append("REPLACE")
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
@@ -264,1499 +295,1454 @@
         """
         See https://redis.io/commands/del
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be deleted.")
 
-        command: list = ["DEL", *keys]
+        command: List = ["DEL", *keys]
 
         return await self.run(command)
 
     async def exists(self, *keys: str) -> int:
         """
         See https://redis.io/commands/exists
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be checked.")
 
-        command: list = ["EXISTS", *keys]
+        command: List = ["EXISTS", *keys]
 
         return await self.run(command)
 
-    async def expire(self, key: str, seconds: int) -> Literal[1, 0] | bool:
+    async def expire(self, key: str, seconds: int) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/expire
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["EXPIRE", key, seconds]
+        command: List = ["EXPIRE", key, seconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def expireat(self, key: str, unix_time_seconds: int) -> Literal[1, 0] | bool:
+    async def expireat(
+        self, key: str, unix_time_seconds: int
+    ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/expireat
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["EXPIREAT", key, unix_time_seconds]
+        command: List = ["EXPIREAT", key, unix_time_seconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def keys(self, pattern: str) -> list[str]:
+    async def keys(self, pattern: str) -> List[str]:
         """
         See https://redis.io/commands/keys
         """
 
-        command: list = ["KEYS", pattern]
+        command: List = ["KEYS", pattern]
 
         return await self.run(command)
 
-    async def persist(self, key: str) -> Literal[1, 0] | bool:
+    async def persist(self, key: str) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/persist
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PERSIST", key]
+        command: List = ["PERSIST", key]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def pexpire(self, key: str, milliseconds: int) -> Literal[1, 0] | bool:
+    async def pexpire(self, key: str, milliseconds: int) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/pexpire
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PEXPIRE", key, milliseconds]
+        command: List = ["PEXPIRE", key, milliseconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def pexpireat(self, key: str, unix_time_milliseconds: int) -> Literal[1, 0] | bool:
+    async def pexpireat(
+        self, key: str, unix_time_milliseconds: int
+    ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/pexpireat
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PEXPIREAT", key, unix_time_milliseconds]
+        command: List = ["PEXPIREAT", key, unix_time_milliseconds]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pttl(self, key: str) -> int:
         """
         See https://redis.io/commands/pttl
         """
 
-        command: list = ["PTTL", key]
+        command: List = ["PTTL", key]
 
         return await self.run(command)
 
-    async def randomkey(self) -> str | None:
+    async def randomkey(self) -> Union[str, None]:
         """
         See https://redis.io/commands/randomkey
         """
 
-        command: list = ["RANDOMKEY"]
+        command: List = ["RANDOMKEY"]
 
         return await self.run(command)
 
-    async def rename(self, key: str, new_name: str) -> str:
+    async def rename(self, key: str, newkey: str) -> str:
         """
         See https://redis.io/commands/rename
         """
 
-        command: list = ["RENAME", key, new_name]
+        command: List = ["RENAME", key, newkey]
 
         return await self.run(command)
 
-    async def renamenx(self, key: str, new_name: str) -> Literal[1, 0] | bool:
+    async def renamenx(self, key: str, newkey: str) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/renamenx
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["RENAMENX", key, new_name]
+        command: List = ["RENAMENX", key, newkey]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def scan(
         self,
         cursor: int,
-        pattern: str | None = None,
-        count: int | None = None,
-        scan_type: str | None = None,
-        return_cursor: bool = True
-    ) -> (list[str | list[str]] | list[int | list[str]]) | list[str]:
+        match_pattern: Union[str, None] = None,
+        count: Union[int, None] = None,
+        scan_type: Union[str, None] = None,
+    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]:
         """
         See https://redis.io/commands/scan
 
-        :param pattern: replacement for "MATCH"
-
-        :param count: defaults to 10 on the server side
+        :param return_cursor: if set to False, it won't return the cursor
 
         :param scan_type: replacement for "TYPE"
-
-        :param return_cursor: if set to False, it won't return the cursor
+        :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only the list of elements will be returned if "return_cursor" is False
+        Only the List of elements will be returned if "return_cursor" is False
         """
 
-        command: list = ["SCAN", cursor]
+        command: List = ["SCAN", cursor]
 
-        if pattern is not None:
-            command.extend(["MATCH", pattern])
+        if match_pattern is not None:
+            command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         if scan_type is not None:
             command.extend(["TYPE", scan_type])
 
-        # The raw result is composed of the new cursor and the list of elements.
-        raw: list[str | list[str]] = await self.run(command)
-
-        if return_cursor:
-            return [int(raw[0]), raw[1]] if self.format_return else raw
+        # The raw result is composed of the new cursor and the List of elements.
+        raw: List[Union[str, List[str]]] = await self.run(command)
 
-        return raw[1]
+        return [int(raw[0]), raw[1]] if self.format_return else raw
 
     async def touch(self, *keys: str) -> int:
         """
         See https://redis.io/commands/touch
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["TOUCH", *keys]
+        command: List = ["TOUCH", *keys]
 
         return await self.run(command)
 
     async def ttl(self, key: str) -> int:
         """
         See https://redis.io/commands/ttl
         """
 
-        command: list = ["TTL", key]
+        command: List = ["TTL", key]
 
         return await self.run(command)
 
-    async def type(self, key: str) -> str | None:
+    async def type(self, key: str) -> Union[str, None]:
         """
         See https://redis.io/commands/type
         """
 
-        command: list = ["TYPE", key]
+        command: List = ["TYPE", key]
 
         return await self.run(command)
 
     async def unlink(self, *keys: str) -> int:
         """
         See https://redis.io/commands/unlink
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["UNLINK", *keys]
+        command: List = ["UNLINK", *keys]
 
         return await self.run(command)
 
     async def geoadd(
         self,
         key: str,
         *members: GeoMember,
         nx: bool = False,
         xx: bool = False,
         ch: bool = False,
     ) -> int:
         """
         See https://redis.io/commands/geoadd
 
-        :param members: a sequence of GeoMember dict types (longitude, latitude, name).
+        :param members: a sequence of GeoMember Dict types (longitude, latitude, name).
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
         if nx and xx:
-            raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
+            raise Exception('"nx" and "xx" are mutually exclusive.')
 
-        command: list = ["GEOADD", key]
+        command: List = ["GEOADD", key]
 
         if nx:
             command.append("NX")
 
         if xx:
             command.append("XX")
 
         if ch:
             command.append("CH")
 
         for member in members:
-            command.extend([member["longitude"], member["latitude"], member["name"]])
+            command.extend([member["longitude"], member["latitude"], member["member"]])
 
         return await self.run(command)
 
     async def geodist(
         self,
         key: str,
-        first_member: str,
-        second_member: str,
-        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M"
-    ) -> str | float | None:
+        member1: str,
+        member2: str,
+        unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"] = "M",
+    ) -> Union[str, float, None]:
         """
         See https://redis.io/commands/geodist
 
         :return: A float value if "format_return" is True.
         """
 
-        command: list = ["GEODIST", key, first_member, second_member, unit]
+        command: List = ["GEODIST", key, member1, member2, unit]
 
-        raw: str | None = await self.run(command)
+        raw: Union[str, None] = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
-    async def geohash(self, key: str, *members: str) -> list[str | None]:
+    async def geohash(self, key: str, *members: str) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/geohash
         """
 
-        command: list = ["GEOHASH", key, *members]
+        command: List = ["GEOHASH", key, *members]
 
         return await self.run(command)
 
     async def geopos(
-        self,
-        key: str,
-        *members: str
-    ) -> list[list[str] | None] | list[dict[str, float] | None]:
+        self, key: str, *members: str
+    ) -> Union[List[Union[List[str], None]], List[Union[Dict[str, float], None]]]:
         """
         See https://redis.io/commands/geopos
 
-        :return: A list of dicts with either None or the longitude and latitude if "format_return" is True.
+        :return: A List of Dicts with either None or the longitude and latitude if "format_return" is True.
         """
 
-        command: list = ["GEOPOS", key, *members]
+        command: List = ["GEOPOS", key, *members]
 
-        raw: list[list[str] | None] = await self.run(command)
+        raw: List[Union[List[str], None]] = await self.run(command)
 
         return format_geo_positions_return(raw) if self.format_return else raw
 
     async def georadius(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        with_distance: bool = False,
-        with_hash: bool = False,
-        with_coordinates: bool = False,
-        count: int | None = None,
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
         count_any: bool = False,
-        sort: Literal["ASC", "DESC"] | None = None,
-        store_as: str | None = None,
-        store_distance_as: str | None = None
-    ) -> GeoMembersReturn | FormattedGeoMembersReturn | int:
+        sort: Union[Literal["ASC", "DESC"], None] = None,
+        store: Union[str, None] = None,
+        storedist: Union[str, None] = None,
+    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn, int]:
         """
         See https://redis.io/commands/georadius
 
         :param count_any: replacement for "ANY"
 
-        :param store_as: replacement for "STORE"
-        :param store_distance_as: replacement for "STORE_DIST"
-
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         handle_georadius_write_exceptions(
-            with_distance,
-            with_hash,
-            with_coordinates,
-            count,
-            count_any,
-            store_as,
-            store_distance_as
+            withdist, withhash, withcoord, count, count_any, store, storedist
         )
 
-        command: list = ["GEORADIUS", key, longitude, latitude, radius, unit]
+        command: List = ["GEORADIUS", key, longitude, latitude, radius, unit]
 
-        if with_distance:
+        if withdist:
             command.append("WITHDIST")
 
-        if with_hash:
+        if withhash:
             command.append("WITHHASH")
 
-        if with_coordinates:
+        if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
             if count_any:
                 command.append("ANY")
 
         if sort:
             command.append(sort)
 
-        if store_as:
-            command.extend(["STORE", store_as])
+        if store:
+            command.extend(["STORE", store])
 
-        if store_distance_as:
-            command.extend(["STOREDIST", store_distance_as])
+        if storedist:
+            command.extend(["STOREDIST", storedist])
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
-        if self.format_return and (with_distance or with_hash or with_coordinates):
-            return format_geo_members_return(raw, with_distance, with_hash, with_coordinates)
+        # If none of the additional properties are requested, the result will be "List[str]".
+        if self.format_return and (withdist or withhash or withcoord):
+            return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def georadius_ro(
         self,
         key: str,
         longitude: float,
         latitude: float,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        with_distance: bool = False,
-        with_hash: bool = False,
-        with_coordinates: bool = False,
-        count: int | None = None,
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
         count_any: bool = False,
-        sort: Literal["ASC", "DESC"] | None = None
-    ) -> GeoMembersReturn | FormattedGeoMembersReturn:
+        sort: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/georadius_ro
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         if count_any and count is None:
-            raise Exception("\"count_any\" can only be used together with \"count\".")
+            raise Exception('"count_any" can only be used together with "count".')
 
-        command: list = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
+        command: List = ["GEORADIUS_RO", key, longitude, latitude, radius, unit]
 
-        if with_distance:
+        if withdist:
             command.append("WITHDIST")
 
-        if with_hash:
+        if withhash:
             command.append("WITHHASH")
 
-        if with_coordinates:
+        if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
             if count_any:
                 command.append("ANY")
 
         if sort:
             command.append(sort)
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
-        if self.format_return and (with_distance or with_hash or with_coordinates):
-            return format_geo_members_return(raw, with_distance, with_hash, with_coordinates)
+        # If none of the additional properties are requested, the result will be "List[str]".
+        if self.format_return and (withdist or withhash or withcoord):
+            return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def georadiusbymember(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        with_distance: bool = False,
-        with_hash: bool = False,
-        with_coordinates: bool = False,
-        count: int | None = None,
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
         count_any: bool = False,
-        sort: Literal["ASC", "DESC"] | None = None,
-        store_as: str | None = None,
-        store_distance_as: str | None = None
-    ) -> GeoMembersReturn | FormattedGeoMembersReturn:
+        sort: Union[Literal["ASC", "DESC"], None] = None,
+        store: Union[str, None] = None,
+        storedist: Union[str, None] = None,
+    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/georadiusbymember
 
         :param count_any: replacement for "ANY"
 
-        :param store_as: replacement for "STORE"
-        :param store_distance_as: replacement for "STORE_DIST"
-
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         handle_georadius_write_exceptions(
-            with_distance,
-            with_hash,
-            with_coordinates,
-            count,
-            count_any,
-            store_as,
-            store_distance_as
+            withdist, withhash, withcoord, count, count_any, store, storedist
         )
 
-        command: list = ["GEORADIUSBYMEMBER", key, member, radius, unit]
+        command: List = ["GEORADIUSBYMEMBER", key, member, radius, unit]
 
-        if with_distance:
+        if withdist:
             command.append("WITHDIST")
 
-        if with_hash:
+        if withhash:
             command.append("WITHHASH")
 
-        if with_coordinates:
+        if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
             if count_any:
                 command.append("ANY")
 
         if sort:
             command.append(sort)
 
-        if store_as:
-            command.extend(["STORE", store_as])
+        if store:
+            command.extend(["STORE", store])
 
-        if store_distance_as:
-            command.extend(["STOREDIST", store_distance_as])
+        if storedist:
+            command.extend(["STOREDIST", storedist])
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
-        if self.format_return and (with_distance or with_hash or with_coordinates):
-            return format_geo_members_return(raw, with_distance, with_hash, with_coordinates)
+        # If none of the additional properties are requested, the result will be "List[str]".
+        if self.format_return and (withdist or withhash or withcoord):
+            return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def georadiusbymember_ro(
         self,
         key: str,
         member: str,
         radius: float,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        with_distance: bool = False,
-        with_hash: bool = False,
-        with_coordinates: bool = False,
-        count: int | None = None,
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+        count: Union[int, None] = None,
         count_any: bool = False,
-        sort: Literal["ASC", "DESC"] | None = None
-    ) -> GeoMembersReturn | FormattedGeoMembersReturn:
+        sort: Union[Literal["ASC", "DESC"], None] = None,
+    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
-        See https://redis.io/commands/georadiusbymember
+        See https://redis.io/commands/georadiusbymember_ro
 
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
         if count_any and count is None:
-            raise Exception("\"count_any\" can only be used together with \"count\".")
+            raise Exception('"count_any" can only be used together with "count".')
 
-        command: list = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
+        command: List = ["GEORADIUSBYMEMBER_RO", key, member, radius, unit]
 
-        if with_distance:
+        if withdist:
             command.append("WITHDIST")
 
-        if with_hash:
+        if withhash:
             command.append("WITHHASH")
 
-        if with_coordinates:
+        if withcoord:
             command.append("WITHCOORD")
 
         if count is not None:
             command.extend(["COUNT", count])
             if count_any:
                 command.append("ANY")
 
         if sort:
             command.append(sort)
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
-        if self.format_return and (with_distance or with_hash or with_coordinates):
-            return format_geo_members_return(raw, with_distance, with_hash, with_coordinates)
+        # If none of the additional properties are requested, the result will be "List[str]".
+        if self.format_return and (withdist or withhash or withcoord):
+            return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def geosearch(
         self,
         key: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        member: str | None = None,
-        longitude: float | None = None,
-        latitude: float | None = None,
-        radius: float | None = None,
-        width: float | None = None,
-        height: float | None = None,
-        sort: Literal["ASC", "DESC"] | None = None,
-        count: int | None = None,
+        frommember: Union[str, None] = None,
+        fromlonlat_longitude: Union[float, None] = None,
+        fromlonlat_latitude: Union[float, None] = None,
+        byradius: Union[float, None] = None,
+        bybox_width: Union[float, None] = None,
+        bybox_height: Union[float, None] = None,
+        sort: Union[Literal["ASC", "DESC"], None] = None,
+        count: Union[int, None] = None,
         count_any: bool = False,
-        with_distance: bool = False,
-        with_hash: bool = False,
-        with_coordinates: bool = False
-    ) -> GeoMembersReturn | FormattedGeoMembersReturn:
+        withdist: bool = False,
+        withhash: bool = False,
+        withcoord: bool = False,
+    ) -> Union[GeoMembersReturn, FormattedGeoMembersReturn]:
         """
         See https://redis.io/commands/geosearch
 
-        :param member: replacement for "FROMMEMBER"
-
-        :param longitude: replacement for "FROMLONLAT" together with "latitude"
-        :param latitude: replacement for "FROMLONLAT" together with "longitude"
-
-        :param radius: replacement for "BYRADIUS"
-
-        :param width: replacement for "BYBOX" together with "height"
-        :param height: replacement for "BYBOX" together with "width"
-
         :param count_any: replacement for "ANY"
 
-        :return: A list of dicts with the requested properties if "format_return" is True.
+        :return: A List of Dicts with the requested properties if "format_return" is True.
         """
 
-        handle_geosearch_exceptions(member, longitude, latitude, radius, width, height, count, count_any)
+        handle_geosearch_exceptions(
+            frommember,
+            fromlonlat_longitude,
+            fromlonlat_latitude,
+            byradius,
+            bybox_width,
+            bybox_height,
+            count,
+            count_any,
+        )
 
-        command: list = ["GEOSEARCH", key]
+        command: List = ["GEOSEARCH", key]
 
-        if member is not None:
-            command.extend(["FROMMEMBER", member])
+        if frommember is not None:
+            command.extend(["FROMMEMBER", frommember])
 
-        if longitude is not None:
-            command.extend(["FROMLONLAT", longitude, latitude])
+        if fromlonlat_longitude is not None:
+            command.extend(["FROMLONLAT", fromlonlat_longitude, fromlonlat_latitude])
 
-        if radius is not None:
-            command.extend(["BYRADIUS", radius])
+        if byradius is not None:
+            command.extend(["BYRADIUS", byradius])
 
-        if width is not None:
-            command.extend(["BYBOX", width, height])
+        if bybox_width is not None:
+            command.extend(["BYBOX", bybox_width, bybox_height])
 
         command.append(unit)
 
         if sort:
             command.append(sort)
 
         if count is not None:
             command.extend(["COUNT", count])
             if count_any:
                 command.append("ANY")
 
-        if with_distance:
+        if withdist:
             command.append("WITHDIST")
 
-        if with_hash:
+        if withhash:
             command.append("WITHHASH")
 
-        if with_coordinates:
+        if withcoord:
             command.append("WITHCOORD")
 
         raw: GeoMembersReturn = await self.run(command)
 
-        # If none of the additional properties are requested, the result will be "list[str]".
-        if self.format_return and (with_distance or with_hash or with_coordinates):
-            return format_geo_members_return(raw, with_distance, with_hash, with_coordinates)
+        # If none of the additional properties are requested, the result will be "List[str]".
+        if self.format_return and (withdist or withhash or withcoord):
+            return format_geo_members_return(raw, withdist, withhash, withcoord)
 
         return raw
 
     async def geosearchstore(
         self,
-        destination_key: str,
-        source_key: str,
+        destination: str,
+        source: str,
         unit: Literal["m", "km", "ft", "mi", "M", "KM", "FT", "MI"],
-        member: str | None = None,
-        longitude: float | None = None,
-        latitude: float | None = None,
-        radius: float | None = None,
-        width: float | None = None,
-        height: float | None = None,
-        sort: Literal["ASC", "DESC"] | None = None,
-        count: int | None = None,
+        frommember: Union[str, None] = None,
+        fromlonlat_longitude: Union[float, None] = None,
+        fromlonlat_latitude: Union[float, None] = None,
+        byradius: Union[float, None] = None,
+        bybox_width: Union[float, None] = None,
+        bybox_height: Union[float, None] = None,
+        sort: Union[Literal["ASC", "DESC"], None] = None,
+        count: Union[int, None] = None,
         count_any: bool = False,
-        store_distance: bool = False
+        storedist: bool = False,
     ) -> int:
         """
         See https://redis.io/commands/geosearchstore
 
-        :param member: replacement for "FROMMEMBER"
-
-        :param longitude: replacement for "FROMLONLAT" together with "latitude"
-        :param latitude: replacement for "FROMLONLAT" together with "longitude"
-
-        :param radius: replacement for "BYRADIUS"
-
-        :param width: replacement for "BYBOX" together with "height"
-        :param height: replacement for "BYBOX" together with "width"
-
         :param count_any: replacement for "ANY"
-
-        :param store_distance: replacement for "STOREDIST"
         """
 
-        handle_geosearch_exceptions(member, longitude, latitude, radius, width, height, count, count_any)
+        handle_geosearch_exceptions(
+            frommember,
+            fromlonlat_longitude,
+            fromlonlat_latitude,
+            byradius,
+            bybox_width,
+            bybox_height,
+            count,
+            count_any,
+        )
 
-        command: list = ["GEOSEARCHSTORE", destination_key, source_key]
+        command: List = ["GEOSEARCHSTORE", destination, source]
 
-        if member is not None:
-            command.extend(["FROMMEMBER", member])
+        if frommember is not None:
+            command.extend(["FROMMEMBER", frommember])
 
-        if longitude is not None:
-            command.extend(["FROMLONLAT", longitude, latitude])
+        if fromlonlat_longitude is not None:
+            command.extend(["FROMLONLAT", fromlonlat_longitude, fromlonlat_latitude])
 
-        if radius is not None:
-            command.extend(["BYRADIUS", radius])
+        if byradius is not None:
+            command.extend(["BYRADIUS", byradius])
 
-        if width is not None:
-            command.extend(["BYBOX", width, height])
+        if bybox_width is not None:
+            command.extend(["BYBOX", bybox_width, bybox_height])
 
         command.append(unit)
 
         if sort:
             command.append(sort)
 
         if count is not None:
             command.extend(["COUNT", count])
             if count_any:
                 command.append("ANY")
 
-        if store_distance:
+        if storedist:
             command.append("STOREDIST")
 
         return await self.run(command)
 
     async def hdel(self, key: str, *fields: str) -> int:
         """
         See https://redis.io/commands/hdel
         """
 
         if len(fields) == 0:
             raise Exception("At least one field must be deleted.")
 
-        command: list = ["HDEL", key, *fields]
+        command: List = ["HDEL", key, *fields]
 
         return await self.run(command)
 
-    async def hexists(self, key: str, field: str) -> Literal[1, 0] | bool:
+    async def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/hexists
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["HEXISTS", key, field]
+        command: List = ["HEXISTS", key, field]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def hget(self, key: str, field: str) -> str | None:
+    async def hget(self, key: str, field: str) -> Union[str, None]:
         """
         See https://redis.io/commands/hget
         """
 
-        command: list = ["HGET", key, field]
+        command: List = ["HGET", key, field]
 
         return await self.run(command)
 
-    async def hgetall(self, key: str) -> HashReturn | FormattedHashReturn:
+    async def hgetall(self, key: str) -> Union[HashReturn, FormattedHashReturn]:
         """
         See https://redis.io/commands/hgetall
 
-        :return: A dict of field-value pairs if "format_return" is True.
+        :return: A Dict of field-value pairs if "format_return" is True.
         """
 
-        command: list = ["HGETALL", key]
+        command: List = ["HGETALL", key]
 
         raw: HashReturn = await self.run(command)
 
         return format_hash_return(raw) if self.format_return else raw
 
     async def hincrby(self, key: str, field: str, increment: int) -> int:
         """
         See https://redis.io/commands/hincrby
         """
 
-        command: list = ["HINCRBY", key, field, increment]
+        command: List = ["HINCRBY", key, field, increment]
 
         return await self.run(command)
 
-    async def hincrbyfloat(self, key: str, field: str, increment: float) -> str | float:
+    async def hincrbyfloat(
+        self, key: str, field: str, increment: float
+    ) -> Union[str, float]:
         """
         See https://redis.io/commands/hincrbyfloat
 
         :return: A float if "format_return" is True.
         """
 
-        command: list = ["HINCRBYFLOAT", key, field, increment]
+        command: List = ["HINCRBYFLOAT", key, field, increment]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
-    async def hkeys(self, key: str) -> list[str]:
+    async def hkeys(self, key: str) -> List[str]:
         """
         See https://redis.io/commands/hkeys
         """
 
-        command: list = ["HKEYS", key]
+        command: List = ["HKEYS", key]
 
         return await self.run(command)
 
     async def hlen(self, key: str) -> int:
         """
         See https://redis.io/commands/hlen
         """
 
-        command: list = ["HLEN", key]
+        command: List = ["HLEN", key]
 
         return await self.run(command)
 
-    async def hmget(self, key: str, *fields: str) -> list[str | None]:
+    async def hmget(self, key: str, *fields: str) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/hmget
         """
 
         if len(fields) == 0:
             raise Exception("At least one field must be specified.")
 
-        command: list = ["HMGET", key, *fields]
+        command: List = ["HMGET", key, *fields]
 
         return await self.run(command)
 
-    async def hmset(self, key: str, fields_and_values: dict) -> str:
+    async def hmset(self, key: str, field_value_pairs: Dict) -> str:
         """
         See https://redis.io/commands/hmset
         """
 
-        command: list = ["HMSET", key]
+        command: List = ["HMSET", key]
 
-        for field, value in fields_and_values.items():
+        for field, value in field_value_pairs.items():
             command.extend([field, value])
 
         return await self.run(command)
 
     async def hrandfield(
-        self,
-        key: str,
-        count: int | None = None,
-        with_values: bool = False
-    ) -> (str | None) | (HashReturn | FormattedHashReturn):
+        self, key: str, count: Union[int, None] = None, withvalues: bool = False
+    ) -> Union[(Union[str, None]), Union[HashReturn, FormattedHashReturn]]:
         """
         See https://redis.io/commands/hrandfield
 
-        :param count: defaults to 1 on the server side
-
-        :return: A dict of field-value pairs if "count" and "with_values" are specified and "format_return" is True.
+        :return: A Dict of field-value pairs if "count" and "withvalues" are specified and "format_return" is True.
         """
 
-        if count is None and with_values:
-            raise Exception("\"with_values\" can only be used together with \"count\"")
+        if count is None and withvalues:
+            raise Exception('"withvalues" can only be used together with "count"')
 
-        command: list = ["HRANDFIELD", key]
+        command: List = ["HRANDFIELD", key]
 
         if count is not None:
             command.extend(["COUNT", count])
 
-            if with_values:
+            if withvalues:
                 command.append("WITHVALUES")
 
                 raw: HashReturn = await self.run(command)
 
                 return format_hash_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     async def hscan(
         self,
         key: str,
         cursor: int,
-        pattern: str | None = None,
-        count: int | None = None,
-        return_cursor: bool = True
-    ) -> (list[str | HashReturn] | list[int | FormattedHashReturn]) | (HashReturn | FormattedHashReturn):
+        match_pattern: Union[str, None] = None,
+        count: Union[int, None] = None,
+    ) -> Union[List[Union[str, HashReturn]], List[Union[int, FormattedHashReturn]]]:
         """
         See https://redis.io/commands/hscan
 
-        :param pattern: replacement for "MATCH"
-
-        :param count: defaults to 10 on the server side
-
         :param return_cursor: if set to False, it won't return the cursor
+        :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only a dict of field-value pairs will be returned if "return_cursor" is False and "format_return" is True.
+        Only a Dict of field-value pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
-        command: list = ["HSCAN", key, cursor]
+        command: List = ["HSCAN", key, cursor]
 
-        if pattern is not None:
-            command.extend(["MATCH", pattern])
+        if match_pattern is not None:
+            command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        # The raw result is composed of the new cursor and the list of elements.
-        raw: list[str | HashReturn] | HashReturn = await self.run(command)
+        # The raw result is composed of the new cursor and the List of elements.
+        raw: Union[List[Union[str, HashReturn]], HashReturn] = await self.run(command)
 
-        if return_cursor:
-            return [int(raw[0]), format_hash_return(raw[1])] if self.format_return else raw
+        return [int(raw[0]), format_hash_return(raw[1])] if self.format_return else raw
 
-        return format_hash_return(raw[1]) if self.format_return else raw[1]
 
-    async def hset(self, key: str, fields_and_values: dict) -> int:
+    async def hset(self, key: str, field_value_pairs: Dict) -> int:
         """
         See https://redis.io/commands/hset
         """
 
-        command: list = ["HSET", key]
+        command: List = ["HSET", key]
 
-        for field, value in fields_and_values.items():
+        for field, value in field_value_pairs.items():
             command.extend([field, value])
 
         return await self.run(command)
 
-    async def hsetnx(self, key: str, field: str, value: Any) -> Literal[1, 0] | bool:
+    async def hsetnx(
+        self, key: str, field: str, value: Any
+    ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/hsetnx
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["HSETNX", key, field, value]
+        command: List = ["HSETNX", key, field, value]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def hstrlen(self, key: str, field: str) -> int:
         """
         See https://redis.io/commands/hstrlen
         """
 
-        command: list = ["HSTRLEN", key, field]
+        command: List = ["HSTRLEN", key, field]
 
         return await self.run(command)
 
-    async def hvals(self, key: str) -> list[str]:
+    async def hvals(self, key: str) -> List[str]:
         """
         See https://redis.io/commands/hvals
         """
 
-        command: list = ["HVALS", key]
+        command: List = ["HVALS", key]
 
         return await self.run(command)
 
-    async def pfadd(self, key: str, *elements: Any) -> Literal[1, 0] | bool:
+    async def pfadd(self, key: str, *elements: Any) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/pfadd
 
         :return: A bool if "format_return" is True.
         """
 
-        command: list = ["PFADD", key, *elements]
+        command: List = ["PFADD", key, *elements]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
     async def pfcount(self, *keys: str) -> int:
         """
         See https://redis.io/commands/pfcount
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["PFCOUNT", *keys]
+        command: List = ["PFCOUNT", *keys]
 
         return await self.run(command)
 
-    async def pfmerge(self, destination_key: str, *source_keys: str) -> str:
+    async def pfmerge(self, destkey: str, *sourcekeys: str) -> str:
         """
         See https://redis.io/commands/pfmerge
         """
 
-        command: list = ["PFMERGE", destination_key, *source_keys]
+        command: List = ["PFMERGE", destkey, *sourcekeys]
 
         return await self.run(command)
 
-    async def lindex(self, key: str, index: int) -> str | None:
+    async def lindex(self, key: str, index: int) -> Union[str, None]:
         """
         See https://redis.io/commands/lindex
         """
 
-        command: list = ["LINDEX", key, index]
+        command: List = ["LINDEX", key, index]
 
         return await self.run(command)
 
     async def linsert(
-        self,
-        key: str,
-        position: Literal["BEFORE", "AFTER"],
-        pivot: Any,
-        element: Any
+        self, key: str, position: Literal["BEFORE", "AFTER"], pivot: Any, element: Any
     ) -> int:
         """
         See https://redis.io/commands/linsert
         """
 
-        command: list = ["LINSERT", key, position, pivot, element]
+        command: List = ["LINSERT", key, position, pivot, element]
 
         return await self.run(command)
 
     async def llen(self, key: str) -> int:
         """
         See https://redis.io/commands/llen
         """
 
-        command: list = ["LLEN", key]
+        command: List = ["LLEN", key]
 
         return await self.run(command)
 
     async def lmove(
         self,
-        source_key: str,
-        destination_key: str,
+        source: str,
+        destination: str,
         source_position: Literal["LEFT", "RIGHT"],
-        destination_position: Literal["LEFT", "RIGHT"]
-    ) -> str | None:
+        destination_position: Literal["LEFT", "RIGHT"],
+    ) -> Union[str, None]:
         """
         See https://redis.io/commands/lmove
         """
 
-        command: list = ["LMOVE", source_key, destination_key, source_position, destination_position]
+        command: List = [
+            "LMOVE",
+            source,
+            destination,
+            source_position,
+            destination_position,
+        ]
 
         return await self.run(command)
 
-    async def lpop(self, key: str, count: int | None = None) -> (str | None) | list[str]:
+    async def lpop(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/lpop
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["LPOP", key]
+        command: List = ["LPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def lpos(
         self,
         key: str,
         element: Any,
-        first_return: int | None = None,
-        count: int | None = None,
-        max_number_of_comparisons: int | None = None
-    ) -> (int | None) | list[int]:
+        rank: Union[int, None] = None,
+        count: Union[int, None] = None,
+        maxlen: Union[int, None] = None,
+    ) -> Union[(Union[int, None]), List[int]]:
         """
         See https://redis.io/commands/lpos
-
-        :param first_return: replacement for "RANK"
-
-        :param max_number_of_comparisons: replacement for "MAXLEN"
         """
 
-        command: list = ["LPOS", key, element]
+        command: List = ["LPOS", key, element]
 
-        if first_return is not None:
-            command.extend(["RANK", first_return])
+        if rank is not None:
+            command.extend(["RANK", rank])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        if max_number_of_comparisons is not None:
-            command.extend(["MAXLEN", max_number_of_comparisons])
+        if maxlen is not None:
+            command.extend(["MAXLEN", maxlen])
 
         return await self.run(command)
 
     async def lpush(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/lpush
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["LPUSH", key, *elements]
+        command: List = ["LPUSH", key, *elements]
 
         return await self.run(command)
 
     async def lpushx(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/lpushx
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["LPUSHX", key, *elements]
+        command: List = ["LPUSHX", key, *elements]
 
         return await self.run(command)
 
-    async def lrange(self, key: str, start: int, stop: int) -> list[str]:
+    async def lrange(self, key: str, start: int, stop: int) -> List[str]:
         """
         See https://redis.io/commands/lrange
         """
 
-        command: list = ["LRANGE", key, start, stop]
+        command: List = ["LRANGE", key, start, stop]
 
         return await self.run(command)
 
     async def lrem(self, key: str, count: int, element: Any) -> int:
         """
         See https://redis.io/commands/lrem
         """
 
-        command: list = ["LREM", key, count, element]
+        command: List = ["LREM", key, count, element]
 
         return await self.run(command)
 
     async def lset(self, key: str, index: int, element: Any) -> str:
         """
         See https://redis.io/commands/lset
         """
 
-        command: list = ["LSET", key, index, element]
+        command: List = ["LSET", key, index, element]
 
         return await self.run(command)
 
     async def ltrim(self, key: str, start: int, stop: int) -> str:
         """
         See https://redis.io/commands/ltrim
         """
 
-        command: list = ["LTRIM", key, start, stop]
+        command: List = ["LTRIM", key, start, stop]
 
         return await self.run(command)
 
-    async def rpop(self, key: str, count: int | None = None) -> (str | None) | list[str]:
+    async def rpop(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/rpop
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["RPOP", key]
+        command: List = ["RPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
-    async def rpoplpush(self, source_key: str, destination_key: str) -> str | None:
+    async def rpoplpush(self, source: str, destination: str) -> Union[str, None]:
         """
         See https://redis.io/commands/rpoplpush
         """
 
-        command: list = ["RPOPLPUSH", source_key, destination_key]
+        command: List = ["RPOPLPUSH", source, destination]
 
         return await self.run(command)
 
     async def rpush(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/rpush
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["RPUSH", key, *elements]
+        command: List = ["RPUSH", key, *elements]
 
         return await self.run(command)
 
     async def rpushx(self, key: str, *elements: Any) -> int:
         """
         See https://redis.io/commands/rpushx
         """
 
         if len(elements) == 0:
             raise Exception("At least one element must be added.")
 
-        command: list = ["RPUSHX", key, *elements]
+        command: List = ["RPUSHX", key, *elements]
 
         return await self.run(command)
 
     async def publish(self, channel: str, message: str) -> int:
         """
         See https://redis.io/commands/publish
         """
 
-        command: list = ["PUBLISH", channel, message]
+        command: List = ["PUBLISH", channel, message]
 
         return await self.run(command)
 
-    async def pubsub(self) -> "PubSub":
-        """
-        See https://redis.io/commands/pubsub
-        """
-
-        return PubSub(client=self)
-
-    async def eval(self, script: str, keys: list[str] | None = None, arguments: list | None = None) -> Any:
+    async def eval(
+        self,
+        script: str,
+        keys: Union[List[str], None] = None,
+        args: Union[List, None] = None,
+    ) -> Any:
         """
         See https://redis.io/commands/eval
 
         The number of keys is calculated automatically.
         """
 
-        command: list = ["EVAL", script]
+        command: List = ["EVAL", script]
 
-        if keys:
+        if keys is not None:
             command.extend([len(keys), *keys])
+        else:
+            command.append(0)
 
-        if arguments:
-            command.extend(arguments)
+        if args:
+            command.extend(args)
 
         return await self.run(command)
 
     async def evalsha(
         self,
-        sha1_digest: str,
-        keys: list[str] | None = None,
-        arguments: list | None = None
+        sha1: str,
+        keys: Union[List[str], None] = None,
+        args: Union[List, None] = None,
     ) -> Any:
         """
         See https://redis.io/commands/evalsha
 
         The number of keys is calculated automatically.
         """
 
-        command: list = ["EVALSHA", sha1_digest]
+        command: List = ["EVALSHA", sha1]
 
-        if keys:
+        if keys is not None:
             command.extend([len(keys), *keys])
+        else:
+            command.append(0)
 
-        if arguments:
-            command.extend(arguments)
+        if args:
+            command.extend(args)
 
         return await self.run(command)
 
-    async def script(self) -> "Script":
-        """
-        See https://redis.io/commands/script
-        """
-
-        return Script(client=self)
-
-    """
-    Need to double-check compatibility with the classic Redis API for this one.
-    async def acl(self) -> "ACL":
-        # See https://redis.io/commands/acl
-        
-        return ACL(client=self)
-    """
-
     async def dbsize(self) -> int:
         """
         See https://redis.io/commands/dbsize
         """
 
-        command: list = ["DBSIZE"]
+        command: List = ["DBSIZE"]
 
         return await self.run(command)
 
-    async def flushall(self, mode: Literal["ASYNC", "SYNC"] | None = None) -> str:
+    async def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
         """
         See https://redis.io/commands/flushall
         """
 
-        command: list = ["FLUSHALL"]
+        command: List = ["FLUSHALL"]
 
         if mode:
             command.append(mode)
 
         return await self.run(command)
 
-    async def flushdb(self, mode: Literal["ASYNC", "SYNC"] | None = None) -> str:
+    async def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
         """
         See https://redis.io/commands/flushdb
         """
 
-        command: list = ["FLUSHDB"]
+        command: List = ["FLUSHDB"]
 
         if mode:
             command.append(mode)
 
         return await self.run(command)
 
-    async def time(self) -> list[str] | dict[str, int]:
+    async def time(self) -> Union[List[str], Dict[str, int]]:
         """
         See https://redis.io/commands/time
 
-        :return: A dict with the keys "seconds" and "microseconds" if self.format_return is True.
+        :return: A Dict with the keys "seconds" and "microseconds" if self.format_return is True.
         """
 
-        command: list = ["TIME"]
+        command: List = ["TIME"]
 
-        raw: list[str] = await self.run(command)
+        raw: List[str] = await self.run(command)
 
         return format_server_time_return(raw) if self.format_return else raw
 
     async def sadd(self, key: str, *members: Any) -> int:
         """
         See https://redis.io/commands/sadd
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be added.")
 
-        command: list = ["SADD", key, *members]
+        command: List = ["SADD", key, *members]
 
         return await self.run(command)
 
     async def scard(self, key: str) -> int:
         """
         See https://redis.io/commands/scard
         """
 
-        command: list = ["SCARD", key]
+        command: List = ["SCARD", key]
 
         return await self.run(command)
 
-    async def sdiff(self, *keys: str) -> list[str]:
+    async def sdiff(self, *keys: str) -> List[str]:
         """
         See https://redis.io/commands/sdiff
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SDIFF", *keys]
+        command: List = ["SDIFF", *keys]
 
         return await self.run(command)
 
-    async def sdiffstore(self, destination_key: str, *keys: str) -> int:
+    async def sdiffstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/sdiffstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SDIFFSTORE", destination_key, *keys]
+        command: List = ["SDIFFSTORE", destination, *keys]
 
         return await self.run(command)
 
-    async def sinter(self, *keys: str) -> list[str]:
+    async def sinter(self, *keys: str) -> List[str]:
         """
         See https://redis.io/commands/sinter
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SINTER", *keys]
+        command: List = ["SINTER", *keys]
 
         return await self.run(command)
 
-    async def sinterstore(self, destination_key: str, *keys: str) -> int:
+    async def sinterstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/sinterstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SINTERSTORE", destination_key, *keys]
+        command: List = ["SINTERSTORE", destination, *keys]
 
         return await self.run(command)
 
-    async def sismember(self, key: str, member: Any) -> Literal[1, 0] | bool:
+    async def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/sismember
 
         :return: A bool if self.format_return is True.
         """
 
-        command: list = ["SISMEMBER", key, member]
+        command: List = ["SISMEMBER", key, member]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def smembers(self, key: str) -> list[str]:
+    async def smembers(self, key: str) -> List[str]:
         """
         See https://redis.io/commands/smembers
         """
 
-        command: list = ["SMEMBERS", key]
+        command: List = ["SMEMBERS", key]
 
         return await self.run(command)
 
-    async def smove(self, source_key: str, destination_key: str, member: Any) -> Literal[1, 0] | bool:
+    async def smove(
+        self, source: str, destination: str, member: Any
+    ) -> Union[Literal[1, 0], bool]:
         """
         See https://redis.io/commands/smove
 
         :return: A bool if self.format_return is True.
         """
 
-        command: list = ["SMOVE", source_key, destination_key, member]
+        command: List = ["SMOVE", source, destination, member]
 
         raw: Literal[1, 0] = await self.run(command)
 
         return bool(raw) if self.format_return else raw
 
-    async def spop(self, key: str, count: int | None = None) -> (str | None) | list[str]:
+    async def spop(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/spop
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["SPOP", key]
+        command: List = ["SPOP", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
-    async def srandmember(self, key: str, count: int | None = None) -> (str | None) | list[str]:
+    async def srandmember(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[(Union[str, None]), List[str]]:
         """
         See https://redis.io/commands/srandmember
 
         :param count: defaults to 1 on the server side
         """
 
-        command: list = ["SRANDMEMBER", key]
+        command: List = ["SRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
         return await self.run(command)
 
     async def srem(self, key: str, *members: Any) -> int:
         """
         See https://redis.io/commands/srem
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
-        command: list = ["SREM", key, *members]
+        command: List = ["SREM", key, *members]
 
         return await self.run(command)
 
     async def sscan(
         self,
         key: str,
         cursor: int,
-        pattern: str | None = None,
-        count: int | None = None,
-        return_cursor: bool = True
-    ) -> (list[str | list[str]] | list[int | list[str]]) | list[str]:
+        match_pattern: Union[str, None] = None,
+        count: Union[int, None] = None,
+    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]:
         """
         See https://redis.io/commands/sscan
 
-        :param pattern: replacement for "MATCH"
-
-        :param count: defaults to 10 on the server side
-
         :param return_cursor: if set to False, it won't return the cursor
+        :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only the list of elements will be returned if "return_cursor" is False.
+        Only the List of elements will be returned if "return_cursor" is False.
         """
 
-        command: list = ["SSCAN", key, cursor]
+        command: List = ["SSCAN", key, cursor]
 
-        if pattern is not None:
-            command.extend(["MATCH", pattern])
+        if match_pattern is not None:
+            command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        # The raw result is composed of the new cursor and the list of elements.
-        raw: list[str | list[str]] = await self.run(command)
+        # The raw result is composed of the new cursor and the List of elements.
+        raw: List[Union[str, List[str]]] = await self.run(command)
 
-        if return_cursor:
-            return [int(raw[0]), raw[1]] if self.format_return else raw
+        return [int(raw[0]), raw[1]] if self.format_return else raw
 
-        return raw[1]
 
-    async def sunion(self, *keys: str) -> list[str]:
+    async def sunion(self, *keys: str) -> List[str]:
         """
         See https://redis.io/commands/sunion
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SUNION", *keys]
+        command: List = ["SUNION", *keys]
 
         return await self.run(command)
 
-    async def sunionstore(self, destination_key: str, *keys: str) -> int:
+    async def sunionstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/sunionstore
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["SUNIONSTORE", destination_key, *keys]
+        command: List = ["SUNIONSTORE", destination, *keys]
 
         return await self.run(command)
 
     async def zadd(
         self,
         key: str,
-        sorted_set_members: dict,
+        score_member_pairs: Dict,
         nx: bool = False,
         xx: bool = False,
         gt: bool = False,
         lt: bool = False,
         ch: bool = False,
-        incr: bool = False
-    ) -> int | (str | None | float):
+        incr: bool = False,
+    ) -> Union[int, (Union[str, None, float])]:
         """
         See https://redis.io/commands/zadd
 
-        :param sorted_set_members: a dict containing their names and scores.
+        :param score_member_pairs: a Dict containing members and their scores.
 
         :return: A float representing the number of elements added or None if "incr" is False
         and "format_return" is True.
         """
 
         if nx and xx:
-            raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
+            raise Exception('"nx" and "xx" are mutually exclusive.')
 
         if gt and lt:
-            raise Exception("\"gt\" and \"lt\" are mutually exclusive.")
+            raise Exception('"gt" and "lt" are mutually exclusive.')
 
         if nx and (gt or lt):
-            raise Exception("\"nx\" and \"gt\" or \"lt\" are mutually exclusive.")
+            raise Exception('"nx" and "gt" or "lt" are mutually exclusive.')
 
-        command: list = ["ZADD", key]
+        command: List = ["ZADD", key]
 
         if nx:
             command.append("NX")
 
         if xx:
             command.append("XX")
 
@@ -1768,965 +1754,998 @@
 
         if ch:
             command.append("CH")
 
         if incr:
             command.append("INCR")
 
-            for name, score in sorted_set_members.items():
+            for name, score in score_member_pairs.items():
                 command.extend([score, name])
 
-            raw: (str | None) = await self.run(command)
+            raw: (Union[str, None]) = await self.run(command)
 
             return float(raw) if self.format_return and raw is not None else raw
 
-        for name, score in sorted_set_members.items():
+        for name, score in score_member_pairs.items():
             command.extend([score, name])
 
         return await self.run(command)
 
     async def zcard(self, key: str) -> int:
         """
         See https://redis.io/commands/zcard
         """
 
-        command: list = ["ZCARD", key]
+        command: List = ["ZCARD", key]
 
         return await self.run(command)
 
-    async def zcount(self, key: str, min_score: FloatMinMax, max_score: FloatMinMax) -> int:
+    async def zcount(
+        self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
+    ) -> int:
         """
         See https://redis.io/commands/zcount
 
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
+
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        command: list = ["ZCOUNT", key, min_score, max_score]
+        command: List = ["ZCOUNT", key, min_score, max_score]
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
-    async def zdiff(self, *keys: str, with_scores: bool = False) -> SortedSetReturn | FormattedSortedSetReturn:
+
+    async def zdiff(
+        self, *keys: str, withscores: bool = False
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zdiff
 
         The number of keys is calculated automatically.
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZDIFF", len(keys), *keys]
+        command: List = ["ZDIFF", len(keys), *keys]
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
-    async def zdiffstore(self, destination_key: str, *keys: str) -> int:
+    async def zdiffstore(self, destination: str, *keys: str) -> int:
         """
         See https://redis.io/commands/zdiffstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZDIFFSTORE", destination_key, len(keys), *keys]
+        command: List = ["ZDIFFSTORE", destination, len(keys), *keys]
 
         return await self.run(command)
 
-    async def zincrby(self, key: str, increment: float, member: str) -> str | float:
+    async def zincrby(
+        self, key: str, increment: float, member: str
+    ) -> Union[str, float]:
         """
         See https://redis.io/commands/zincrby
 
         :return: A float if "format_return" is True.
         """
 
-        command: list = ["ZINCRBY", key, increment, member]
+        command: List = ["ZINCRBY", key, increment, member]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
+
     async def zinter(
         self,
         *keys: str,
-        multiplication_factors: list[float] | None = None,
-        aggregate: Literal["SUM", "MIN", "MAX"] | None = None,
-        with_scores: bool = False
-    ) -> SortedSetReturn | FormattedSortedSetReturn:
+        weights: Union[List[float], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
+        withscores: bool = False,
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zinter
 
         The number of keys is calculated automatically.
 
-        :param multiplication_factors: replacement for "WEIGHTS"
-
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZINTER", len(keys), *keys]
+        command: List = ["ZINTER", len(keys), *keys]
 
-        if multiplication_factors:
-            command.extend(["WEIGHTS", *multiplication_factors])
+        if weights:
+            command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     async def zinterstore(
         self,
-        destination_key: str,
+        destination: str,
         *keys: str,
-        multiplication_factors: list[float] | None = None,
-        aggregate: Literal["SUM", "MIN", "MAX"] | None = None
+        weights: Union[List[float], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         """
         See https://redis.io/commands/zinterstore
 
         The number of keys is calculated automatically.
-
-        :param multiplication_factors: replacement for "WEIGHTS"
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZINTERSTORE", destination_key, len(keys), *keys]
+        command: List = ["ZINTERSTORE", destination, len(keys), *keys]
 
-        if multiplication_factors:
-            command.extend(["WEIGHTS", *multiplication_factors])
+        if weights:
+            command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
         return await self.run(command)
 
     async def zlexcount(self, key: str, min_score: str, max_score: str) -> int:
         """
         See https://redis.io/commands/zlexcount
+
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
         """
 
-        if not min_score.startswith(('(', '[', '+', '-')) or not max_score.startswith(('(', '[', '+', '-')):
+        if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
+            ("(", "[", "+", "-")
+        ):
             raise Exception(
                 "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
             )
 
-        command: list = ["ZLEXCOUNT", key, min_score, max_score]
+        command: List = ["ZLEXCOUNT", key, min_score, max_score]
 
         return await self.run(command)
 
-    async def zmscore(self, key: str, *members: str) -> list[str | None] | list[float | None]:
+    async def zmscore(
+        self, key: str, *members: str
+    ) -> Union[List[Union[str, None]], List[Union[float, None]]]:
         """
         See https://redis.io/commands/zmscore
 
-        :return: A list of float or None values if "format_return" is True.
+        :return: A List of float or None values if "format_return" is True.
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be specified.")
 
-        command: list = ["ZMSCORE", key, *members]
+        command: List = ["ZMSCORE", key, *members]
 
-        raw: list[str | None] = await self.run(command)
+        raw: List[Union[str, None]] = await self.run(command)
 
         return format_float_list(raw) if self.format_return else raw
 
-    async def zpopmax(self, key: str, count: int | None = None) -> SortedSetReturn | FormattedSortedSetReturn:
+    async def zpopmax(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zpopmax
 
         :param count: defaults to 1 on the server side
 
-        :return: A dict of member-score pairs if "format_return" is True.
+        :return: A Dict of member-score pairs if "format_return" is True.
         """
 
-        command: list = ["ZPOPMAX", key]
+        command: List = ["ZPOPMAX", key]
 
         if count is not None:
             command.append(count)
 
         raw: SortedSetReturn = await self.run(command)
 
         return format_sorted_set_return(raw) if self.format_return else raw
 
-    async def zpopmin(self, key: str, count: int | None = None) -> SortedSetReturn | FormattedSortedSetReturn:
+    async def zpopmin(
+        self, key: str, count: Union[int, None] = None
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zpopmin
 
         :param count: defaults to 1 on the server side
 
-        :return: A dict of member-score pairs if "format_return" is True.
+        :return: A Dict of member-score pairs if "format_return" is True.
         """
 
-        command: list = ["ZPOPMIN", key]
+        command: List = ["ZPOPMIN", key]
 
         if count is not None:
             command.append(count)
 
         raw: SortedSetReturn = await self.run(command)
 
         return format_sorted_set_return(raw) if self.format_return else raw
 
     async def zrandmember(
-        self,
-        key: str,
-        count: int | None = None,
-        with_scores: bool = False
-    ) -> (str | None) | (SortedSetReturn | FormattedSortedSetReturn):
+        self, key: str, count: Union[int, None] = None, withscores: bool = False
+    ) -> Union[(Union[str, None]), (Union[SortedSetReturn, FormattedSortedSetReturn])]:
         """
         See https://redis.io/commands/zrandmember
 
         :param count: defaults to 1 on the server side
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        if count is None and with_scores:
-            raise Exception("\"with_scores\" can only be used with \"count\".")
+        if count is None and withscores:
+            raise Exception('"withscores" can only be used with "count".')
 
-        command: list = ["ZRANDMEMBER", key]
+        command: List = ["ZRANDMEMBER", key]
 
         if count is not None:
             command.append(count)
 
-            if with_scores:
+            if withscores:
                 command.append("WITHSCORES")
 
                 raw: SortedSetReturn = await self.run(command)
 
                 return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
+
     async def zrange(
         self,
         key: str,
         start: FloatMinMax,
         stop: FloatMinMax,
-        range_method: Literal["BYSCORE", "BYLEX"] | None = None,
+        range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
-        offset: int | None = None,
-        count: int | None = None,
-        with_scores: bool = False
-    ) -> SortedSetReturn | FormattedSortedSetReturn:
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
+        withscores: bool = False,
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zrange
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
         """
 
-        handle_non_deprecated_zrange_exceptions(range_method, start, stop, offset, count)
+        handle_non_deprecated_zrange_exceptions(
+            range_method, start, stop, limit_offset, limit_count
+        )
 
-        command: list = ["ZRANGE", key, start, stop]
+        command: List = ["ZRANGE", key, start, stop]
 
         if range_method:
             command.append(range_method)
 
         if rev:
             command.append("REV")
 
-        if offset is not None:
-            command.extend(["LIMIT", offset, count])
+        if limit_offset is not None:
+            command.extend(["LIMIT", limit_offset, limit_count])
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     async def zrangebylex(
         self,
         key: str,
         min_score: str,
         max_score: str,
-        offset: int | None = None,
-        count: int | None = None
-    ) -> list[str | None]:
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
+    ) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/zrangebylex
+
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
         """
 
-        handle_zrangebylex_exceptions(min_score, max_score, offset, count)
+        handle_zrangebylex_exceptions(min_score, max_score, limit_offset, limit_count)
 
-        command: list = ["ZRANGEBYLEX", key, min_score, max_score]
+        command: List = ["ZRANGEBYLEX", key, min_score, max_score]
 
-        if offset is not None:
-            command.extend(["LIMIT", offset, count])
+        if limit_offset is not None:
+            command.extend(["LIMIT", limit_offset, limit_count])
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but, 
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "withscores" is True or not, its raw return type will be List[str].
     """
+
     async def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
-        with_scores: bool = False,
-        offset: int | None = None,
-        count: int | None = None
-    ) -> SortedSetReturn | FormattedSortedSetReturn:
+        withscores: bool = False,
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
+
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if number_are_not_none(offset, count, number=1):
-            raise Exception("Both \"offset\" and \"count\" must be specified.")
+            raise Exception('Both "offset" and "count" must be specified.')
 
-        command: list = ["ZRANGEBYSCORE", key, min_score, max_score]
+        command: List = ["ZRANGEBYSCORE", key, min_score, max_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     async def zrangestore(
         self,
-        destination_key: str,
-        source_key: str,
-        start: FloatMinMax,
-        stop: FloatMinMax,
-        range_method: Literal["BYSCORE", "BYLEX"] | None = None,
+        dst: str,
+        src: str,
+        min_score: FloatMinMax,
+        max_score: FloatMinMax,
+        range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
-        offset: int | None = None,
-        count: int | None = None
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
     ) -> int:
         """
         See https://redis.io/commands/zrangestore
 
-        If you need to use "-inf" and "+inf", please write them as strings.
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
 
-        :param start: replacement for "min" to match "ZRANGE"
-        :param stop: replacement for "max" to match "ZRANGE"
+        If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        handle_non_deprecated_zrange_exceptions(range_method, start, stop, offset, count)
+        handle_non_deprecated_zrange_exceptions(
+            range_method, min_score, max_score, limit_offset, limit_count
+        )
 
-        command: list = ["ZRANGESTORE", destination_key, source_key, start, stop]
+        command: List = ["ZRANGESTORE", dst, src, min_score, max_score]
 
         if range_method:
             command.append(range_method)
 
         if rev:
             command.append("REV")
 
-        if offset is not None:
-            command.extend(["LIMIT", offset, count])
+        if limit_offset is not None:
+            command.extend(["LIMIT", limit_offset, limit_count])
 
         return await self.run(command)
 
-    async def zrank(self, key: str, member: str) -> int | None:
+    async def zrank(self, key: str, member: str) -> Union[int, None]:
         """
         See https://redis.io/commands/zrank
         """
 
-        command: list = ["ZRANK", key, member]
+        command: List = ["ZRANK", key, member]
 
         return await self.run(command)
 
     async def zrem(self, key: str, *members: str) -> int:
         """
         See https://redis.io/commands/zrem
         """
 
         if len(members) == 0:
             raise Exception("At least one member must be removed.")
 
-        command: list = ["ZREM", key, *members]
+        command: List = ["ZREM", key, *members]
 
         return await self.run(command)
 
     async def zremrangebylex(self, key: str, min_score: str, max_score: str) -> int:
         """
         See https://redis.io/commands/zremrangebylex
+
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
         """
 
-        if not min_score.startswith(('(', '[', '+', '-')) or not max_score.startswith(('(', '[', '+', '-')):
+        if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
+            ("(", "[", "+", "-")
+        ):
             raise Exception(
                 "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
             )
 
-        command: list = ["ZREMRANGEBYLEX", key, min_score, max_score]
+        command: List = ["ZREMRANGEBYLEX", key, min_score, max_score]
 
         return await self.run(command)
 
     async def zremrangebyrank(self, key: str, start: int, stop: int) -> int:
         """
         See https://redis.io/commands/zremrangebyrank
         """
 
-        command: list = ["ZREMRANGEBYRANK", key, start, stop]
+        command: List = ["ZREMRANGEBYRANK", key, start, stop]
 
         return await self.run(command)
 
-    async def zremrangebyscore(self, key: str, min_score: FloatMinMax, max_score: FloatMinMax) -> int:
+    async def zremrangebyscore(
+        self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
+    ) -> int:
         """
-        See https://redis.io/commands/zremrangebyscore
+        See https://redis.io/commands/zremrangebyscore\
+        
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
 
         If you need to use "-inf" and "+inf", please write them as strings.
         """
 
-        command: list = ["ZREMRANGEBYSCORE", key, min_score, max_score]
+        command: List = ["ZREMRANGEBYSCORE", key, min_score, max_score]
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but,
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "with_scores" is True or not, its raw return type will be List[str].
     """
+
     async def zrevrange(
-        self,
-        key: str,
-        start: int,
-        stop: int,
-        with_scores: bool = False
-    ) -> SortedSetReturn | FormattedSortedSetReturn:
+        self, key: str, start: int, stop: int, withscores: bool = False
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zrevrange
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        command: list = ["ZREVRANGE", key, start, stop]
+        command: List = ["ZREVRANGE", key, start, stop]
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     async def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
-        offset: int | None = None,
-        count: int | None = None
-    ) -> list[str]:
+        offset: Union[int, None] = None,
+        count: Union[int, None] = None,
+    ) -> List[str]:
         """
         See https://redis.io/commands/zrevrangebylex
+
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
         """
 
         handle_zrangebylex_exceptions(min_score, max_score, offset, count)
 
-        command: list = ["ZREVRANGEBYLEX", key, max_score, min_score]
+        command: List = ["ZREVRANGEBYLEX", key, max_score, min_score]
 
         if offset is not None:
             command.extend(["LIMIT", offset, count])
 
         return await self.run(command)
 
     """
     This has actually 3 return scenarios, but,
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "withscores" is True or not, its raw return type will be List[str].
     """
+
     async def zrevrangebyscore(
         self,
         key: str,
         max_score: FloatMinMax,
         min_score: FloatMinMax,
-        with_scores: bool = False,
-        offset: int | None = None,
-        count: int | None = None
-    ) -> SortedSetReturn | FormattedSortedSetReturn:
+        withscores: bool = False,
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zrevrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :param min_score: replacement for "MIN"
+        :param max_score: replacement for "MAX"
+
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        if number_are_not_none(offset, count, number=1):
-            raise Exception("Both \"offset\" and \"count\" must be specified.")
+        if number_are_not_none(limit_offset, limit_count, number=1):
+            raise Exception('Both "limit_offset" and "limit_count" must be specified.')
 
-        command: list = ["ZREVRANGEBYSCORE", key, max_score, min_score]
+        command: List = ["ZREVRANGEBYSCORE", key, max_score, min_score]
 
-        if offset is not None:
-            command.extend(["LIMIT", offset, count])
+        if limit_offset is not None:
+            command.extend(["LIMIT", limit_offset, limit_count])
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
-    async def zrevrank(self, key: str, member: str) -> int | None:
+    async def zrevrank(self, key: str, member: str) -> Union[int, None]:
         """
         See https://redis.io/commands/zrevrank
         """
 
-        command: list = ["ZREVRANK", key, member]
+        command: List = ["ZREVRANK", key, member]
 
         return await self.run(command)
 
     async def zscan(
         self,
         key: str,
         cursor: int,
-        pattern: str | None = None,
-        count: int | None = None,
-        return_cursor: bool = True
-    ) -> (
-            list[str | SortedSetReturn] | list[int | FormattedSortedSetReturn]
-         ) | (
-            SortedSetReturn | FormattedSortedSetReturn
-         ):
+        match_pattern: Union[str, None] = None,
+        count: Union[int, None] = None,
+    ) -> Union[List[Union[str, SortedSetReturn]],List[Union[int, FormattedSortedSetReturn]]]:
         """
         See https://redis.io/commands/zscan
 
-        :param pattern: replacement for "MATCH"
-
-        :param count: defaults to 10 on the server side
-
         :param return_cursor: if set to False, it won't return the cursor
+        :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only a dict of member-score pairs will be returned if "return_cursor" is False and "format_return" is True.
+        Only a Dict of member-score pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
-        command: list = ["ZSCAN", key, cursor]
+        command: List = ["ZSCAN", key, cursor]
 
-        if pattern is not None:
-            command.extend(["MATCH", pattern])
+        if match_pattern is not None:
+            command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
-        raw: list[int | SortedSetReturn] = await self.run(command)
+        raw: List[Union[int, SortedSetReturn]] = await self.run(command)
 
-        if return_cursor:
-            return [int(raw[0]), format_sorted_set_return(raw[1])] if self.format_return else raw
+        return [int(raw[0]), format_sorted_set_return(raw[1])] if self.format_return else raw
 
-        # The raw result is composed of the new cursor and the list of elements.
-        return format_sorted_set_return(raw[1]) if self.format_return else raw[1]
 
-    async def zscore(self, key: str, member: str) -> str | None | float:
+    async def zscore(self, key: str, member: str) -> Union[str, None, float]:
         """
         See https://redis.io/commands/zscore
 
         :return: A float or None if "format_return" is True.
         """
 
-        command: list = ["ZSCORE", key, member]
+        command: List = ["ZSCORE", key, member]
 
-        raw: str | None = await self.run(command)
+        raw: Union[str, None] = await self.run(command)
 
         return float(raw) if self.format_return and raw is not None else raw
 
     """
     This has actually 3 return scenarios, but,
-    whether "with_scores" is True or not, its raw return type will be list[str].
+    whether "withscores" is True or not, its raw return type will be List[str].
     """
+
     async def zunion(
         self,
         *keys: str,
-        multiplication_factors: list[float] | None = None,
-        aggregate: Literal["SUM", "MIN", "MAX"] | None = None,
-        with_scores: bool = False
-    ) -> SortedSetReturn | FormattedSortedSetReturn:
+        weights: Union[List[float], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
+        withscores: bool = False,
+    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
         """
         See https://redis.io/commands/zunion
 
         The number of keys is calculated automatically.
 
-        :param multiplication_factors: replacement for "WEIGHTS"
-
-        :return: A dict of member-score pairs if "with_scores" and "format_return" are True.
+        :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZUNION", len(keys), *keys]
+        command: List = ["ZUNION", len(keys), *keys]
 
-        if multiplication_factors:
-            command.extend(["WEIGHTS", *multiplication_factors])
+        if weights:
+            command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
-        if with_scores:
+        if withscores:
             command.append("WITHSCORES")
 
             raw: SortedSetReturn = await self.run(command)
 
             return format_sorted_set_return(raw) if self.format_return else raw
 
         return await self.run(command)
 
     async def zunionstore(
         self,
-        destination_key: str,
+        destination: str,
         *keys: str,
-        multiplication_factors: list[float] | None = None,
-        aggregate: Literal["SUM", "MIN", "MAX"] | None = None
+        weights: Union[List[float], None] = None,
+        aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         """
         See https://redis.io/commands/zunionstore
 
         The number of keys is calculated automatically.
-
-        :param multiplication_factors: replacement for "WEIGHTS"
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["ZUNIONSTORE", destination_key, len(keys), *keys]
+        command: List = ["ZUNIONSTORE", destination, len(keys), *keys]
 
-        if multiplication_factors:
-            command.extend(["WEIGHTS", *multiplication_factors])
+        if weights:
+            command.extend(["WEIGHTS", *weights])
 
         if aggregate:
             command.extend(["AGGREGATE", aggregate])
 
         return await self.run(command)
 
     async def append(self, key: str, value: Any) -> int:
         """
         See https://redis.io/commands/append
         """
 
-        command: list = ["APPEND", key, value]
+        command: List = ["APPEND", key, value]
 
         return await self.run(command)
 
     async def decr(self, key: str) -> int:
         """
         See https://redis.io/commands/decr
         """
 
-        command: list = ["DECR", key]
+        command: List = ["DECR", key]
 
         return await self.run(command)
 
     async def decrby(self, key: str, decrement: int) -> int:
         """
         See https://redis.io/commands/decrby
         """
 
-        command: list = ["DECRBY", key, decrement]
+        command: List = ["DECRBY", key, decrement]
 
         return await self.run(command)
 
-    async def get(self, key: str) -> str | None:
+    async def get(self, key: str) -> Union[str, None]:
         """
         See https://redis.io/commands/get
         """
 
-        command: list = ["GET", key]
+        command: List = ["GET", key]
 
         return await self.run(command)
 
-    async def getdel(self, key: str) -> str | None:
+    async def getdel(self, key: str) -> Union[str, None]:
         """
         See https://redis.io/commands/getdel
         """
 
-        command: list = ["GETDEL", key]
+        command: List = ["GETDEL", key]
 
         return await self.run(command)
 
     async def getex(
         self,
         key: str,
-        seconds: int | None = None,
-        milliseconds: int | None = None,
-        unix_time_seconds: int | None = None,
-        unix_time_milliseconds: int | None = None,
-        persist: bool | None = None
-    ) -> str | None:
+        ex: Union[int, None] = None,
+        px: Union[int, None] = None,
+        exat: Union[int, None] = None,
+        pxat: Union[int, None] = None,
+        persist: Union[bool, None] = None,
+    ) -> Union[str, None]:
         """
         See https://redis.io/commands/getex
         """
 
-        if not number_are_not_none(seconds, milliseconds, unix_time_seconds, unix_time_milliseconds, persist, number=1):
+        if not number_are_not_none(ex, px, exat, pxat, persist, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
-        command: list = ["GETEX", key]
+        command: List = ["GETEX", key]
 
-        if seconds is not None:
-            command.extend(["EX", seconds])
+        if ex is not None:
+            command.extend(["EX", ex])
 
-        if milliseconds is not None:
-            command.extend(["PX", milliseconds])
+        if px is not None:
+            command.extend(["PX", px])
 
-        if unix_time_seconds is not None:
-            command.extend(["EXAT", unix_time_seconds])
+        if exat is not None:
+            command.extend(["EXAT", exat])
 
-        if unix_time_milliseconds is not None:
-            command.extend(["PXAT", unix_time_milliseconds])
+        if pxat is not None:
+            command.extend(["PXAT", pxat])
 
         if persist is not None:
             command.append("PERSIST")
 
         return await self.run(command)
 
     async def getrange(self, key: str, start: int, end: int) -> str:
         """
         See https://redis.io/commands/getrange
         """
 
-        command: list = ["GETRANGE", key, start, end]
+        command: List = ["GETRANGE", key, start, end]
 
         return await self.run(command)
 
-    async def getset(self, key: str, value: Any) -> str | None:
+    async def getset(self, key: str, value: Any) -> Union[str, None]:
         """
         See https://redis.io/commands/getset
         """
 
-        command: list = ["GETSET", key, value]
+        command: List = ["GETSET", key, value]
 
         return await self.run(command)
 
     async def incr(self, key: str) -> int:
         """
         See https://redis.io/commands/incr
         """
 
-        command: list = ["INCR", key]
+        command: List = ["INCR", key]
 
         return await self.run(command)
 
     async def incrby(self, key: str, increment: int) -> int:
         """
         See https://redis.io/commands/incrby
         """
 
-        command: list = ["INCRBY", key, increment]
+        command: List = ["INCRBY", key, increment]
 
         return await self.run(command)
 
-    async def incrbyfloat(self, key: str, increment: float) -> str | float:
+    async def incrbyfloat(self, key: str, increment: float) -> Union[str, float]:
         """
         See https://redis.io/commands/incrbyfloat
 
         :return: A float if "format_return" is True.
         """
 
-        command: list = ["INCRBYFLOAT", key, increment]
+        command: List = ["INCRBYFLOAT", key, increment]
 
         raw: str = await self.run(command)
 
         return float(raw) if self.format_return else raw
 
-    async def mget(self, *keys: str) -> list[str | None]:
+    async def mget(self, *keys: str) -> List[Union[str, None]]:
         """
         See https://redis.io/commands/mget
         """
 
         if len(keys) == 0:
             raise Exception("At least one key must be specified.")
 
-        command: list = ["MGET", *keys]
+        command: List = ["MGET", *keys]
 
         return await self.run(command)
 
-    async def mset(self, keys_and_values: dict) -> Literal["OK"]:
+    async def mset(self, key_value_pairs: Dict) -> Literal["OK"]:
         """
         See https://redis.io/commands/mset
         """
 
-        command: list = ["MSET"]
+        command: List = ["MSET"]
 
-        for key, value in keys_and_values.items():
+        for key, value in key_value_pairs.items():
             command.extend([key, value])
 
         return await self.run(command)
 
-    async def msetnx(self, keys_and_values: dict) -> Literal[1, 0]:
+    async def msetnx(self, key_value_pairs: Dict) -> Literal[1, 0]:
         """
         See https://redis.io/commands/msetnx
         """
 
-        command: list = ["MSETNX"]
+        command: List = ["MSETNX"]
 
-        for key, value in keys_and_values.items():
+        for key, value in key_value_pairs.items():
             command.extend([key, value])
 
         return await self.run(command)
 
     async def psetex(self, key: str, milliseconds: int, value: Any) -> str:
         """
         See https://redis.io/commands/psetex
         """
 
-        command: list = ["PSETEX", key, milliseconds, value]
+        command: List = ["PSETEX", key, milliseconds, value]
 
         return await self.run(command)
 
     async def set(
         self,
         key: str,
         value: Any,
         nx: bool = False,
         xx: bool = False,
         get: bool = False,
-        seconds: int | None = None,
-        milliseconds: int | None = None,
-        unix_time_seconds: int | None = None,
-        unix_time_milliseconds: int | None = None,
-        keep_ttl: bool = False,
-    ) -> str | None:
+        ex: Union[int, None] = None,
+        px: Union[int, None] = None,
+        exat: Union[int, None] = None,
+        pxat: Union[int, None] = None,
+        keepttl: bool = False,
+    ) -> Union[str, None]:
         """
         See https://redis.io/commands/set
         """
 
         if nx and xx:
-            raise Exception("\"nx\" and \"xx\" are mutually exclusive.")
+            raise Exception('"nx" and "xx" are mutually exclusive.')
 
-        if not number_are_not_none(
-            seconds,
-            milliseconds,
-            unix_time_seconds,
-            unix_time_milliseconds,
-            keep_ttl,
-            number=1
-        ):
+        if not number_are_not_none(ex, px, exat, pxat, keepttl, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         if nx and get:
-            raise Exception("\"nx\" and \"get\" are mutually exclusive.")
+            raise Exception('"nx" and "get" are mutually exclusive.')
 
-        command: list = ["SET", key, value]
+        command: List = ["SET", key, value]
 
         if nx:
             command.append("NX")
 
         if xx:
             command.append("XX")
 
         if get:
             command.append("GET")
 
-        if seconds is not None:
-            command.extend(["EX", seconds])
+        if ex is not None:
+            command.extend(["EX", ex])
 
-        if milliseconds is not None:
-            command.extend(["PX", milliseconds])
+        if px is not None:
+            command.extend(["PX", px])
 
-        if unix_time_seconds is not None:
-            command.extend(["EXAT", unix_time_seconds])
+        if exat is not None:
+            command.extend(["EXAT", exat])
 
-        if unix_time_milliseconds is not None:
-            command.extend(["PXAT", unix_time_milliseconds])
+        if pxat is not None:
+            command.extend(["PXAT", pxat])
 
-        if keep_ttl:
+        if keepttl:
             command.append("KEEPTTL")
 
         return await self.run(command)
 
     async def setex(self, key: str, seconds: int, value: Any) -> str:
         """
         See https://redis.io/commands/setex
         """
 
-        command: list = ["SETEX", key, seconds, value]
+        command: List = ["SETEX", key, seconds, value]
 
         return await self.run(command)
 
     async def setnx(self, key: str, value: Any) -> Literal[1, 0]:
         """
         See https://redis.io/commands/setnx
         """
 
-        command: list = ["SETNX", key, value]
+        command: List = ["SETNX", key, value]
 
         return await self.run(command)
 
     async def setrange(self, key: str, offset: int, value: Any) -> int:
         """
         See https://redis.io/commands/setrange
         """
 
-        command: list = ["SETRANGE", key, offset, value]
+        command: List = ["SETRANGE", key, offset, value]
 
         return await self.run(command)
 
     async def strlen(self, key: str) -> int:
         """
         See https://redis.io/commands/strlen
         """
 
-        command: list = ["STRLEN", key]
+        command: List = ["STRLEN", key]
 
         return await self.run(command)
 
     async def substr(self, key: str, start: int, end: int) -> str:
         """
         See https://redis.io/commands/substr
         """
 
-        command: list = ["SUBSTR", key, start, end]
+        command: List = ["SUBSTR", key, start, end]
 
         return await self.run(command)
+    
+    def pubsub(self) -> "PubSub":
+        """
+        See https://redis.io/commands/pubsub
+        """
 
+        return PubSub(client=self)
+    
+    def script(self) -> "Script":
+        """
+        See https://redis.io/commands/script
+        """
 
+        return Script(client=self)
+    
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: Redis, key: str):
+    def __init__(self, client: Commands, key: str):
         self.client = client
-        self.command: list = ["BITFIELD", key]
+        self.command: List = ["BITFIELD", key]
 
     def get(self, encoding: str, offset: BitFieldOffset):
         """
         Returns the specified bit field.
 
         Source: https://redis.io/commands/bitfield
         """
@@ -2773,189 +2792,188 @@
         """
 
         _command = ["OVERFLOW", overflow]
         self.command.extend(_command)
 
         return self
 
-    async def execute(self) -> list:
+    async def execute(self) -> List:
         return await self.client.run(command=self.command)
 
 
 class BitFieldRO:
-    def __init__(self, client: Redis, key: str):
+    def __init__(self, client: Commands, key: str):
         self.client = client
-        self.command: list = ["BITFIELD_RO", key]
+        self.command: List = ["BITFIELD_RO", key]
 
     def get(self, encoding: str, offset: BitFieldOffset):
         """
         Returns the specified bit field.
 
-        Source: https://redis.io/commands/bitfield
+        Source: https://redis.io/commands/bitfield_ro
         """
 
         _command = ["GET", encoding, offset]
         self.command.extend(_command)
 
         return self
 
-    async def execute(self) -> list:
+    async def execute(self) -> List:
         return await self.client.run(command=self.command)
 
 
 class PubSub:
-    def __init__(self, client: Redis):
+    def __init__(self, client: Commands):
         self.client = client
-        self.command: list = ["PUBSUB"]
 
-    async def channels(self, pattern: str | None = None) -> list[str]:
+    async def channels(self, pattern: Union[str, None] = None) -> List[str]:
         """
         See https://redis.io/commands/pubsub-channels
         """
 
-        self.command.append("CHANNELS")
+        command: List = ["PUBSUB", "CHANNELS"]
 
         if pattern is not None:
-            self.command.append(pattern)
+            command.append(pattern)
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
     async def numpat(self) -> int:
         """
         See https://redis.io/commands/pubsub-numpat
         """
 
-        self.command.append("NUMPAT")
+        command: List = ["PUBSUB", "NUMPAT"]
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
-    async def numsub(self, *channels: str) -> list[str | int] | dict[str, int]:
+    async def numsub(
+        self, *channels: str
+    ) -> Union[List[Union[str, int]], Dict[str, int]]:
         """
         See https://redis.io/commands/pubsub-numsub
 
-        :return: A dict with channel-(number-of-subscribers) pairs if "format_return" is True.
+        :return: A Dict with channel-number_of_subscribers pairs if "format_return" is True.
         """
 
-        self.command.extend(["NUMSUB", *channels])
+        command: List = ["PUBSUB", "NUMSUB", *channels]
 
-        raw: list[str | int] = await self.client.run(command=self.command)
+        raw: List[Union[str, int]] = await self.client.run(command)
 
         return format_pubsub_numsub_return(raw) if self.client.format_return else raw
 
 
 class Script:
-    def __init__(self, client: Redis):
+    def __init__(self, client: Commands):
         self.client = client
-        self.command: list = ["SCRIPT"]
 
-    async def exists(self, *sha1_digests: str) -> list[Literal[1, 0]] | list[bool]:
+    async def exists(self, *sha1: str) -> Union[List[Literal[1, 0]], List[bool]]:
         """
         See https://redis.io/commands/script-exists
 
-        :return: A list of bools if "format_return" is True.
+        :return: A List of bools if "format_return" is True.
         """
 
-        if len(sha1_digests) == 0:
-            raise Exception("At least one sha1 digest must be provided.")
+        if len(sha1) == 0:
+            raise Exception("At least one sha1 digests must be provided.")
 
-        self.command.extend(["EXISTS", *sha1_digests])
+        command: List = ["SCRIPT", "EXISTS", *sha1]
 
-        raw: list[Literal[1, 0]] = await self.client.run(command=self.command)
+        raw: List[Literal[1, 0]] = await self.client.run(command=command)
 
         return format_bool_list(raw) if self.client.format_return else raw
 
     async def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
         """
         See https://redis.io/commands/script-flush
         """
 
-        self.command.append("FLUSH")
+        command: List = ["SCRIPT", "FLUSH"]
 
         if mode:
-            self.command.append(mode)
+            command.append(mode)
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
     async def load(self, script: str) -> str:
         """
         See https://redis.io/commands/script-load
         """
 
-        self.command.extend(["LOAD", script])
+        command: List = ["SCRIPT", "LOAD", script]
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
 
 """
 class ACL:
-    def __init__(self, client: Redis):
+    def __init__(self, client: Commands):
         self.client = client
-        self.command: list = ["ACL"]
 
-    async def cat(self, category_name: str | None = None) -> list[str]:
+    async def cat(self, category: Union[str, None] = None) -> List[str]:
         # See https://redis.io/commands/acl-cat
 
-        self.command.append("CAT")
+        command: List = ["ACL", "CAT"]
 
-        if category_name is not None:
-            self.command.append(category_name)
+        if category is not None:
+            command.append(category)
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
     async def deluser(self, *usernames: str) -> int:
         # See https://redis.io/commands/acl-deluser
         
         if len(usernames) == 0:
             raise Exception("At least one username must be provided.")
 
-        self.command.extend(["DELUSER", *usernames])
+        command: List = ["ACL", "DELUSER", *usernames]
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
-    async def genpass(self, bits: int | None = None) -> str:
+    async def genpass(self, bits: Union[int, None] = None) -> str:
         # See https://redis.io/commands/acl-genpass
 
-        self.command.append("GENPASS")
+        command: List = ["ACL", "GENPASS"]
 
         if bits is not None:
-            self.command.append(bits)
+            command.append(bits)
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
     # Is it possible to format this output?
-    async def getuser(self, username: str) -> list[str] | None:
+    async def getuser(self, username: str) -> Union[List[str], None]:
         # See https://redis.io/commands/acl-getuser
 
-        self.command.extend(["GETUSER", username])
+        command: List = ["ACL", "GETUSER", username]
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
-    async def list_rules(self) -> list[str]:
-        # See https://redis.io/commands/acl-list
+    async def List_rules(self) -> List[str]:
+        # See https://redis.io/commands/acl-List
 
-        self.command.append("LIST")
+        command = ["ACL", "LIST"]
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
     async def load(self) -> str:
         # See https://redis.io/commands/acl-load
 
-        self.command.append("LOAD")
+        command = ["ACL", "LOAD"]
 
-        return await self.client.run(command=self.command)
+        return await self.client.run(command=command)
 
-    async def log(self, count: int | None = None, reset: bool = False) -> list[str]:
+    async def log(self, count: Union[int, None] = None, reset: bool = False) -> List[str]:
         # See https://redis.io/commands/acl-log
 
         if count is not None and reset:
             raise Exception("Cannot specify both "count" and "reset".")
 
-        self.command.append("LOG")
+        command: List = ["ACL", "LOG"]
 
         if count is not None:
-            self.command.append(count)
+            command.append(count)
 
         if reset:
-            self.command.append("RESET")
+            command.append("RESET")
 
-        return await self.client.run(command=self.command)
-"""
+        return await self.client.run(command=command)
+"""
```

### Comparing `upstash_redis-0.12.0/upstash_redis/http/decode.py` & `upstash_redis-0.12.1/upstash_redis/http/decode.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from upstash_redis.schema.http import RESTResult
 from upstash_redis.utils.base import base64_to_string
 from upstash_redis.exception import UpstashException
+from typing import List
 
 
 def decode(raw: RESTResult, encoding: str) -> RESTResult:
     """
     Decode the response received from the REST API.
     """
 
     if encoding == "base64":
         if isinstance(raw, str):
             return "OK" if raw == "OK" else base64_to_string(raw)
 
         elif isinstance(raw, int) or raw is None:
             return raw
 
-        elif isinstance(raw, list):
+        elif isinstance(raw, List):
             return [
                 # Decode recursively.
-                decode(element, encoding) for element in raw
+                decode(element, encoding)
+                for element in raw
             ]
         else:
-            raise UpstashException(f'Error decoding data for result type {str(type(raw))}')
+            raise UpstashException(
+                f"Error decoding data for result type {str(type(raw))}"
+            )
```

### Comparing `upstash_redis-0.12.0/upstash_redis/http/execute.py` & `upstash_redis-0.12.1/upstash_redis/http/execute.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,150 @@
+import aiohttp
 from upstash_redis.exception import UpstashException
 from upstash_redis.http.decode import decode
 from upstash_redis.schema.http import RESTResult, RESTResponse, RESTEncoding
 from upstash_redis.schema.telemetry import TelemetryData
 from asyncio import sleep
 from aiohttp import ClientSession
 from json import dumps
 from platform import python_version
+from typing import Union, List, Dict
 
+from requests import Session
+import time
 
-async def execute(
+
+async def async_execute(
     session: ClientSession,
     url: str,
     token: str,
     encoding: RESTEncoding,
     retries: int,
     retry_interval: int,
-    command: list,
+    command: List,
     allow_telemetry: bool,
-    telemetry_data: TelemetryData | None = None
+    telemetry_data: Union[TelemetryData, None] = None,
 ) -> RESTResult:
     """
     Execute the given command over the REST API.
 
     :param encoding: the encoding that can be used by the REST API to parse the response before sending it
     :param retries: how many times an HTTP request will be retried if it fails
     :param retry_interval: how many seconds will be waited between each retry
     :param allow_telemetry: whether anonymous telemetry can be collected
     """
 
     # Serialize the command; more specifically, write string-incompatible types as JSON strings.
     command = [
-        element if isinstance(element, str | int | float)
-
-        else dumps(element)
-
+        element if (isinstance(element, str) or isinstance(element, int) or isinstance(element, float)) else dumps(element)
         for element in command
     ]
 
     for i in range(retries + 1):
         try:
-            headers: dict[str, str] = {"Authorization": f'Bearer {token}'}
+            headers: Dict[str, str] = {"Authorization": f"Bearer {token}"}
 
             if allow_telemetry:
                 if telemetry_data:
                     # Avoid the [] syntax to prevent KeyError from being raised.
                     if telemetry_data.get("runtime"):
                         headers["Upstash-Telemetry-Runtime"] = telemetry_data["runtime"]
                     else:
-                        headers["Upstash-Telemetry-Runtime"] = f'python@v{python_version()}'
+                        headers[
+                            "Upstash-Telemetry-Runtime"
+                        ] = f"python@v{python_version()}"
 
                     if telemetry_data.get("sdk"):
                         headers["Upstash-Telemetry-Sdk"] = telemetry_data["sdk"]
                     else:
                         headers["Upstash-Telemetry-Sdk"] = "upstash_redis@development"
 
                     if telemetry_data.get("platform"):
-                        headers["Upstash-Telemetry-Platform"] = telemetry_data["platform"]
+                        headers["Upstash-Telemetry-Platform"] = telemetry_data[
+                            "platform"
+                        ]
 
             if encoding:
                 headers["Upstash-Encoding"] = encoding
 
             async with session.post(url, headers=headers, json=command) as response:
                 body: RESTResponse = await response.json()
 
                 # Avoid the [] syntax to prevent KeyError from being raised.
                 if body.get("error"):
                     raise UpstashException(body.get("error"))
 
-                return decode(raw=body["result"], encoding=encoding) if encoding else body["result"]
+                return (
+                    decode(raw=body["result"], encoding=encoding)
+                    if encoding
+                    else body["result"]
+                )
             break
         except Exception as exception:
             if i == retries:
                 # If we exhausted all the retries, raise the exception.
                 raise exception
             else:
                 await sleep(retry_interval)
+
+
+def sync_execute(
+    session: Session,
+    url: str,
+    token: str,
+    encoding: RESTEncoding,
+    retries: int,
+    retry_interval: int,
+    command: List,
+    allow_telemetry: bool,
+    telemetry_data: Union[TelemetryData, None] = None,
+) -> RESTResult:
+
+    command = [
+        element if (isinstance(element, str) or isinstance(element, int) or isinstance(element, float)) else dumps(element)
+        for element in command
+    ]
+
+    for i in range(retries + 1):
+        try:
+            headers: Dict[str, str] = {"Authorization": f"Bearer {token}"}
+
+            if allow_telemetry:
+                if telemetry_data:
+                    # Avoid the [] syntax to prevent KeyError from being raised.
+                    if telemetry_data.get("runtime"):
+                        headers["Upstash-Telemetry-Runtime"] = telemetry_data["runtime"]
+                    else:
+                        headers[
+                            "Upstash-Telemetry-Runtime"
+                        ] = f"python@v{python_version()}"
+
+                    if telemetry_data.get("sdk"):
+                        headers["Upstash-Telemetry-Sdk"] = telemetry_data["sdk"]
+                    else:
+                        headers["Upstash-Telemetry-Sdk"] = "upstash_redis@development"
+
+                    if telemetry_data.get("platform"):
+                        headers["Upstash-Telemetry-Platform"] = telemetry_data[
+                            "platform"
+                        ]
+
+            if encoding:
+                headers["Upstash-Encoding"] = encoding
+
+            response = session.post(url, headers=headers, json=command).json()
+
+            # Avoid the [] syntax to prevent KeyError from being raised.
+            if response.get("error"):
+                raise UpstashException(response.get("error"))
+
+            return (
+                decode(raw=response["result"], encoding=encoding)
+                if encoding
+                else response["result"]
+            )
+        except Exception as exception:
+            if i == retries:
+                # If we exhausted all the retries, raise the exception.
+                raise exception
+            else:
+                time.sleep(retry_interval)
```

### Comparing `upstash_redis-0.12.0/upstash_redis/utils/exception.py` & `upstash_redis-0.12.1/upstash_redis/utils/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,114 @@
 from upstash_redis.schema.commands.parameters import FloatMinMax
 from upstash_redis.utils.comparison import number_are_not_none
-from typing import Literal
+from typing import Literal, Union
 
 
 def handle_georadius_write_exceptions(
-    with_distance: bool = False,
-    with_hash: bool = False,
-    with_coordinates: bool = False,
-    count: int | None = None,
+    withdist: bool = False,
+    withhash: bool = False,
+    withcoord: bool = False,
+    count: Union[int, None] = None,
     count_any: bool = False,
-    store_as: str | None = None,
-    store_dist_as: str | None = None,
+    store: Union[str, None] = None,
+    storedist: Union[str, None] = None,
 ) -> None:
     """
     Handle exceptions for "GEORADIUS*" write commands.
     """
 
     if count_any and count is None:
-        raise Exception("\"count_any\" can only be used together with \"count\".")
+        raise Exception('"count_any" can only be used together with "count".')
 
-    if (with_distance or with_hash or with_coordinates) and (store_as or store_dist_as):
-        raise Exception("Cannot use \"store_as\" or \"store_dist_as\" when requesting additional properties.")
+    if (withdist or withhash or withcoord) and (store or storedist):
+        raise Exception(
+            'Cannot use "store" or "storedist" when requesting additional properties.'
+        )
 
 
 def handle_geosearch_exceptions(
-    member: str | None,
-    longitude: float | None,
-    latitude: float | None,
-    radius: float | None,
-    width: float | None,
-    height: float | None,
-    count: int | None,
-    count_any: bool
+    member: Union[str, None],
+    fromlonlat_longitude: Union[float, None],
+    fromlonlat_latitude: Union[float, None],
+    byradius: Union[float, None],
+    bybox_width: Union[float, None],
+    bybox_height: Union[float, None],
+    count: Union[int, None],
+    count_any: bool,
 ) -> None:
     """
     Handle exceptions for "GEOSEARCH*" commands.
     """
 
-    if number_are_not_none(longitude, latitude, number=1):
-        raise Exception("Both \"longitude\" and \"latitude\" must be specified.")
+    if number_are_not_none(fromlonlat_longitude, fromlonlat_latitude, number=1):
+        raise Exception(
+            'Both "fromlonlat_longitude" and "fromlonlat_latitude" must be specified.'
+        )
 
-    if number_are_not_none(width, height, number=1):
-        raise Exception("Both \"width\" and \"height\" must be specified.")
+    if number_are_not_none(bybox_width, bybox_height, number=1):
+        raise Exception('Both "bybox_width" and "bybox_height" must be specified.')
 
-    if not number_are_not_none(member, longitude, number=1):
-        raise Exception("""Specify either the member's name with "member",
-or the longitude and latitude with "longitude" and "latitude", but not both.""")
-
-    if not number_are_not_none(radius, width, number=1):
-        raise Exception("""Specify either the radius with "radius",
-or the width and height with "width" and "height", but not both.""")
+    if not number_are_not_none(member, fromlonlat_longitude, number=1):
+        raise Exception(
+            """Specify either the member's name with "member",
+or the fromlonlat_longitude and fromlonlat_latitude with "fromlonlat_longitude" and "fromlonlat_latitude", but not both."""
+        )
+
+    if not number_are_not_none(byradius, bybox_width, number=1):
+        raise Exception(
+            """Specify either the byradius with "byradius",
+or the bybox_width and bybox_height with "bybox_width" and "bybox_height", but not both."""
+        )
 
     if count_any and count is None:
-        raise Exception("\"count_any\" can only be used together with \"count\".")
+        raise Exception('"count_any" can only be used together with "count".')
 
 
 def handle_non_deprecated_zrange_exceptions(
-    range_method: Literal["BYLEX", "BYSCORE"] | None,
+    range_method: Union[Literal["BYLEX", "BYSCORE"], None],
     start: FloatMinMax,
     stop: FloatMinMax,
-    offset: int | None,
-    count: int | None,
+    offset: Union[int, None],
+    count: Union[int, None],
 ) -> None:
     """
     Handle exceptions for non-deprecated "ZRANGE*" commands.
     """
 
     if range_method == "BYLEX" and (
-        not (
-            isinstance(start, str) and isinstance(stop, str)
-        ) or not (
-            start.startswith(('(', '[', '+', '-'))
-            and stop.startswith(('(', '[', '+', '-'))
+        not (isinstance(start, str) and isinstance(stop, str))
+        or not (
+            start.startswith(("(", "[", "+", "-"))
+            and stop.startswith(("(", "[", "+", "-"))
         )
     ):
-        raise Exception(""""start" and "stop" must either start with '(' or '[' or be '+' or '-' when
-the ranging method is "BYLEX".""")
+        raise Exception(
+            """"start" and "stop" must either start with '(' or '[' or be '+' or '-' when
+the ranging method is "BYLEX"."""
+        )
 
     if number_are_not_none(offset, count, number=1):
-        raise Exception("Both \"offset\" and \"count\" must be specified.")
+        raise Exception('Both "offset" and "count" must be specified.')
 
 
 def handle_zrangebylex_exceptions(
     min_score: str,
     max_score: str,
-    offset: int | None,
-    count: int | None,
+    offset: Union[int, None],
+    count: Union[int, None],
 ) -> None:
     """
     Handle exceptions for "ZRANGEBYLEX" and "ZREVRANGEBYLEX" commands.
+
+    :param min_score: replacement for "MIN"
+    :param max_score: replacement for "MAX"
     """
 
-    if not min_score.startswith(('(', '[', '+', '-')) or not max_score.startswith(('(', '[', '+', '-')):
+    if not min_score.startswith(("(", "[", "+", "-")) or not max_score.startswith(
+        ("(", "[", "+", "-")
+    ):
         raise Exception(
             "\"min_score\" and \"max_score\" must either start with '(' or '[' or be '+' or '-'."
         )
 
     if number_are_not_none(offset, count, number=1):
-        raise Exception("Both \"offset\" and \"count\" must be specified.")
+        raise Exception('Both "offset" and "count" must be specified.')
```

### Comparing `upstash_redis-0.12.0/PKG-INFO` & `upstash_redis-0.12.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.12.0
+Version: 0.12.1
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
-# Upstash Rate Limit - python edition
+# Upstash Redis - python edition
 
 upstash-redis is a connectionless, HTTP-based Redis client for python, designed to be used in serverless and serverful environments such as:
 - AWS Lambda
 - Google Cloud Functions
 - and other environments where HTTP is preferred over TCP.
 
 Inspired by other Redis clients like [@upstash/redis](https://github.com/upstash/upstash-redis) and [redis-py](https://github.com/redis/redis-py),
@@ -29,14 +31,17 @@
 
 <!-- toc -->
 
 - [Quick Start](#quick-start)
   - [Install](#install)
     - [PyPi](#PyPi)
   - [Usage](#usage)
+    - [Command groups](#command-groups)
+    - [BITFIELD and BITFIELD_RO](#bitfield-and-bitfieldro)
+    - [Custom commands](#custom-commands)
   - [Telemetry](#telemetry)
 - [Encoding](#encoding)
 - [Retry mechanism](#retry-mechanism)
 - [Formatting returns](#formatting-returns)
 - [Contributing](#contributing)
   - [Preparing the environment](#preparing-the-environment)
   - [Config](#config)
@@ -102,14 +107,57 @@
         await redis.set("a", "b")
         print(await redis.get("a"))
 
 run(main())
 
 ```
 
+### Command groups
+Most of the command groups, such as `PUBSUB` and `SCRIPT`, are available as an instance attribute of the `Redis` class.
+
+```python
+await redis.pubsub.channels()
+
+await redis.script.flush(mode="ASYNC")
+```
+
+
+### BITFIELD and BITFIELD_RO
+One particular case is represented by these two chained commands, which are available as functions that return an instance of 
+the `BITFIELD` and, respectively, `BITFIELD_RO` classes. Use the `execute` function to run the commands.
+
+```python
+await (
+    redis.bitfield("test_key")
+    .incrby(encoding="i8", offset=100, increment=100)
+    .overflow("SAT")
+    .incrby(encoding="i8", offset=100, increment=100)
+    .execute()
+)
+
+await (
+    redis.bitfield_ro("test_key_2")
+    .get(encoding="u8", offset=0)
+    .get(encoding="u8", offset="#1")
+    .execute()
+)
+```
+
+
+### Custom commands
+If you want to run a command that hasn't been implemented, you can use the `run` function of your client instance
+and pass the command as `list`
+
+```python
+await redis.run(command=["XLEN", "test_stream"])
+```
+
+If you want to have more control over your session management or need to use multiple custom values, use
+the [execute](./upstash_redis/http/execute.py) function directly.
+
 
 # Telemetry
 The SDK can collect the following anonymous telemetry:
   - the runtime (ex: `python@v.3.10.0`)
   - the SDK or SDKs you're using (ex: `upstash-redisy@development, upstash-ratelimit@v.0.1.0`)
   - the platform you're running on (ex: `AWS-lambda`)
```

