# Comparing `tmp/aiomodbus-0.5.2.tar.gz` & `tmp/aiomodbus-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiomodbus-0.5.2.tar", last modified: Fri Jun 17 07:44:05 2022, max compression
+gzip compressed data, was "aiomodbus-0.6.0.tar", last modified: Fri Jun 30 03:27:38 2023, max compression
```

## Comparing `aiomodbus-0.5.2.tar` & `aiomodbus-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/
-drwxrwxrwx   0        0        0        0 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/.github/
-drwxrwxrwx   0        0        0        0 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/.github/workflows/
--rw-rw-rw-   0        0        0     1591 2020-06-19 07:47:21.000000 aiomodbus-0.5.2/.github/workflows/python-app.yml
--rw-rw-rw-   0        0        0     1307 2019-11-29 07:50:54.000000 aiomodbus-0.5.2/.gitignore
--rw-rw-rw-   0        0        0     1094 2020-04-02 00:07:50.000000 aiomodbus-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      744 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      171 2020-06-19 07:47:21.000000 aiomodbus-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/aiomodbus/
--rw-rw-rw-   0        0        0       22 2022-06-17 07:43:17.000000 aiomodbus-0.5.2/aiomodbus/__init__.py
--rw-rw-rw-   0        0        0     4069 2020-10-02 06:45:25.000000 aiomodbus-0.5.2/aiomodbus/crc.py
--rw-rw-rw-   0        0        0     1200 2020-10-02 06:45:25.000000 aiomodbus-0.5.2/aiomodbus/decoders.py
--rw-rw-rw-   0        0        0     1125 2020-10-02 06:45:25.000000 aiomodbus-0.5.2/aiomodbus/encoders.py
--rw-rw-rw-   0        0        0      925 2021-07-12 02:43:39.000000 aiomodbus-0.5.2/aiomodbus/exceptions.py
--rw-rw-rw-   0        0        0     9300 2022-06-17 07:41:43.000000 aiomodbus-0.5.2/aiomodbus/serial.py
--rw-rw-rw-   0        0        0     8744 2022-06-17 07:41:43.000000 aiomodbus-0.5.2/aiomodbus/tcp.py
-drwxrwxrwx   0        0        0        0 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/aiomodbus.egg-info/
--rw-rw-rw-   0        0        0      744 2022-06-17 07:44:02.000000 aiomodbus-0.5.2/aiomodbus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2022-06-17 07:44:02.000000 aiomodbus-0.5.2/aiomodbus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-17 07:44:02.000000 aiomodbus-0.5.2/aiomodbus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-04-01 23:25:25.000000 aiomodbus-0.5.2/aiomodbus.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2022-06-17 07:44:02.000000 aiomodbus-0.5.2/aiomodbus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-06-17 07:44:02.000000 aiomodbus-0.5.2/aiomodbus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2020-10-02 06:45:25.000000 aiomodbus-0.5.2/requirements-test.txt
--rw-rw-rw-   0        0        0       21 2021-07-12 04:30:49.000000 aiomodbus-0.5.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     2007 2022-06-17 07:41:43.000000 aiomodbus-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-17 07:44:04.000000 aiomodbus-0.5.2/test/
--rw-rw-rw-   0        0        0        0 2020-06-19 07:47:21.000000 aiomodbus-0.5.2/test/__init__.py
--rw-rw-rw-   0        0        0      905 2020-10-02 06:45:25.000000 aiomodbus-0.5.2/test/test_crc.py
--rw-rw-rw-   0        0        0     7266 2021-07-12 02:43:39.000000 aiomodbus-0.5.2/test/test_rtu_protocol.py
--rw-rw-rw-   0        0        0     7434 2020-10-02 06:45:25.000000 aiomodbus-0.5.2/test/test_tcp_protocol.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:27:38.755524 aiomodbus-0.6.0/
+-rw-rw-rw-   0        0        0     1073 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      741 2023-06-30 03:27:38.755524 aiomodbus-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3301 2023-06-30 01:36:12.000000 aiomodbus-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 03:27:38.728400 aiomodbus-0.6.0/aiomodbus/
+-rw-rw-rw-   0        0        0       22 2023-06-30 01:36:12.000000 aiomodbus-0.6.0/aiomodbus/__init__.py
+-rw-rw-rw-   0        0        0     3785 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/aiomodbus/crc.py
+-rw-rw-rw-   0        0        0     1153 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/aiomodbus/decoders.py
+-rw-rw-rw-   0        0        0     1082 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/aiomodbus/encoders.py
+-rw-rw-rw-   0        0        0      868 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/aiomodbus/exceptions.py
+-rw-rw-rw-   0        0        0     9511 2023-06-30 01:35:44.000000 aiomodbus-0.6.0/aiomodbus/serial.py
+-rw-rw-rw-   0        0        0     8823 2023-06-30 01:34:23.000000 aiomodbus-0.6.0/aiomodbus/tcp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:27:38.733465 aiomodbus-0.6.0/aiomodbus.egg-info/
+-rw-rw-rw-   0        0        0      741 2023-06-30 03:27:38.000000 aiomodbus-0.6.0/aiomodbus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-06-30 03:27:38.000000 aiomodbus-0.6.0/aiomodbus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:27:38.000000 aiomodbus-0.6.0/aiomodbus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 00:27:07.000000 aiomodbus-0.6.0/aiomodbus.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2023-06-30 03:27:38.000000 aiomodbus-0.6.0/aiomodbus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 03:27:38.000000 aiomodbus-0.6.0/aiomodbus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 03:27:38.755524 aiomodbus-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1974 2023-06-30 01:36:12.000000 aiomodbus-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:27:38.754524 aiomodbus-0.6.0/test/
+-rw-rw-rw-   0        0        0      868 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/test/test_crc.py
+-rw-rw-rw-   0        0        0     7008 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/test/test_rtu_protocol.py
+-rw-rw-rw-   0        0        0     7166 2023-06-29 23:31:07.000000 aiomodbus-0.6.0/test/test_tcp_protocol.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiomodbus-0.5.2/LICENSE` & `aiomodbus-0.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Ryan Parry-Jones
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Ryan Parry-Jones
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `aiomodbus-0.5.2/aiomodbus/decoders.py` & `aiomodbus-0.6.0/aiomodbus/decoders.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import struct
-from aiomodbus.exceptions import modbus_exception_codes
-
-
-def _unpack_bits(data, bytesize=8):
-    (size,) = struct.unpack(">B", data[0:1])
-    values = struct.unpack(">" + "B" * size, data[1:])
-    vals = []
-    for val in values:
-        for ind in range(bytesize):
-            vals.append(bool((val >> ind) & 1))
-    return vals
-
-
-def _unpack_words(data):
-    (size,) = struct.unpack(">B", data[0:1])
-    return struct.unpack(">" + "H" * (size // 2), data[1:])
-
-
-def _unpack_single_register(data):
-    return struct.unpack(">H", data[2:4])[0]
-
-
-def _unpack_single_coil(data):
-    return bool(_unpack_single_register(data))
-
-
-function_codes = {
-    1: _unpack_bits,
-    2: _unpack_bits,
-    3: _unpack_words,
-    4: _unpack_words,
-    5: _unpack_single_coil,
-    6: _unpack_single_register,
-    15: _unpack_single_register,
-    16: _unpack_single_register,
-}
-
-
-def from_func_code(fut, func_code, data):
-    if func_code & 0x80:
-        fut.set_exception(modbus_exception_codes[data[0]])
-    else:
-        try:
-            fut.set_result(function_codes[func_code](data))
-        except BaseException as e:
-            fut.set_exception(e)
+import struct
+from aiomodbus.exceptions import modbus_exception_codes
+
+
+def _unpack_bits(data, bytesize=8):
+    (size,) = struct.unpack(">B", data[0:1])
+    values = struct.unpack(">" + "B" * size, data[1:])
+    vals = []
+    for val in values:
+        for ind in range(bytesize):
+            vals.append(bool((val >> ind) & 1))
+    return vals
+
+
+def _unpack_words(data):
+    (size,) = struct.unpack(">B", data[0:1])
+    return struct.unpack(">" + "H" * (size // 2), data[1:])
+
+
+def _unpack_single_register(data):
+    return struct.unpack(">H", data[2:4])[0]
+
+
+def _unpack_single_coil(data):
+    return bool(_unpack_single_register(data))
+
+
+function_codes = {
+    1: _unpack_bits,
+    2: _unpack_bits,
+    3: _unpack_words,
+    4: _unpack_words,
+    5: _unpack_single_coil,
+    6: _unpack_single_register,
+    15: _unpack_single_register,
+    16: _unpack_single_register,
+}
+
+
+def from_func_code(fut, func_code, data):
+    if func_code & 0x80:
+        fut.set_exception(modbus_exception_codes[data[0]])
+    else:
+        try:
+            fut.set_result(function_codes[func_code](data))
+        except BaseException as e:
+            fut.set_exception(e)
```

### Comparing `aiomodbus-0.5.2/aiomodbus/serial.py` & `aiomodbus-0.6.0/aiomodbus/serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         self.transport = None
         self.client = client
         self.current_request = None
         self.recv_callback = None
         self.q = asyncio.Queue()
         self.buffer = bytearray()
         self.loop = asyncio.get_event_loop()
+        self.byte_time = 0
 
     def connection_made(self, transport: serial_asyncio.SerialTransport):
         self.transport = transport
         self.byte_time = 1 / (
             transport.serial.baudrate
             / (transport.serial.bytesize + transport.serial.stopbits + 1)
             / 1.5
@@ -142,15 +143,15 @@
         self,
         unit: int,
         function_code: int,
         address: int,
         *values: int,
         decode_packing: str,
         packet_length: int,
-        timeout: float = 0.1,
+        turn_around_delay_timeout: float = 0.4,
     ):
         if unit is None:
             unit = self.default_unit_id
         async with self.transaction:
             try:
                 await asyncio.wait_for(self.connected.wait(), 2)
             except asyncio.TimeoutError as e:
@@ -160,15 +161,15 @@
             packet = self._encode_packet(unit, function_code, address, *values)
             self.protocol.buffer.clear()
             self.transport.write(packet)
             write_time = self.protocol.byte_time * len(packet)
             unit_id, func_code, *values, crc = await self.protocol.decode(
                 packet_length,
                 decode_packing,
-                turn_around_delay_timeout=0.4 + write_time,
+                turn_around_delay_timeout=turn_around_delay_timeout + write_time,
             )
             assert unit_id == unit
             assert function_code == func_code
             return values
 
     async def read_coils(
         self, address: int, count: int, *, unit=None, timeout: float = 0.1
@@ -176,57 +177,57 @@
         resp = await self._request(
             unit,
             0x01,
             address,
             count,
             decode_packing=">BBB" + "B" * ((count - 1) // 8 + 1) + "H",
             packet_length=5 + 1 * ((count - 1) // 8 + 1),
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
         return self._upack_bits(*resp[1:])[:count]
 
     async def read_discrete_inputs(
         self, address: int, count: int, *, unit=None, timeout: float = 0.1
     ):
         resp = await self._request(
             unit,
             0x02,
             address,
             count,
             decode_packing=">BBB" + "B" * ((count - 1) // 8 + 1) + "H",
             packet_length=5 + 1 * ((count - 1) // 8 + 1),
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
         return self._upack_bits(*resp[1:])[:count]
 
     async def read_holding_registers(
         self, address: int, count: int, *, unit=None, timeout: float = 0.1
     ):
         resp = await self._request(
             unit,
             0x03,
             address,
             count,
             decode_packing=">BBBH" + "H" * count,
             packet_length=5 + 2 * count,
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
         return resp[1:]
 
     async def read_input_registers(
         self, address: int, count: int, *, unit=None, timeout: float = 0.1
     ):
         resp = await self._request(
             unit,
             0x04,
             address,
             count,
             decode_packing=">BBBH" + "H" * count,
             packet_length=5 + 2 * count,
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
         return resp[1:]
 
     async def write_single_coil(
         self, address: int, value: bool, *, unit=None, timeout: float = 0.1
     ):
         if value:
@@ -234,54 +235,54 @@
         await self._request(
             unit,
             0x05,
             address,
             value,
             decode_packing=">BBHHH",
             packet_length=8,
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
 
     async def write_single_register(
         self, address: int, value: int, *, unit=None, timeout: float = 0.1
     ):
         return await self._request(
             unit,
             0x06,
             address,
             value,
             decode_packing=">BBHHH",
             packet_length=8,
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
 
     async def write_multiple_coils(
         self, address: int, *values: bool, unit=None, timeout: float = 0.1
     ):
         await self._request(
             unit,
             0x0F,
             address,
             *values,
             decode_packing=">BBHHH",
             packet_length=8,
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
 
     async def write_multiple_registers(
         self, address: int, *values: int, unit=None, timeout: float = 0.1
     ):
         await self._request(
             unit,
             0x10,
             address,
             *values,
             decode_packing=">BBHHH",
             packet_length=8,
-            timeout=timeout,
+            turn_around_delay_timeout=timeout,
         )
 
     async def read_exception_status(self, unit=None, timeout=None):
         function_code = 0x07
         raise NotImplementedError
 
     async def diagnostics(self, sub_function, *data, unit=None, timeout=None):
```

### Comparing `aiomodbus-0.5.2/aiomodbus/tcp.py` & `aiomodbus-0.6.0/aiomodbus/tcp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,244 +1,251 @@
-import asyncio
-import threading
-import logging
-import socket
-from typing import Optional, Tuple, Union, Dict
-import struct
-from dataclasses import dataclass
-from asyncio import transports
-from aiomodbus import decoders, encoders
-
-Number = Union[int, float]
-
-log = logging.getLogger(__file__)
-
-
-@dataclass
-class TransactionLimit:
-    limit: Optional[int] = None
-    evt_connected: Optional[asyncio.Event] = None
-    evt_connected_timeout: float = 2
-
-    def __post_init__(self):
-        self.semaphore = None
-        if self.limit:
-            self.semaphore = asyncio.Semaphore(self.limit)
-
-    async def __aenter__(self):
-        if self.evt_connected:
-            try:
-                await asyncio.wait_for(
-                    self.evt_connected.wait(), self.evt_connected_timeout
-                )
-            except asyncio.TimeoutError:
-                raise ConnectionError("Client isn't connected")
-        if self.semaphore:
-            await self.semaphore.__aenter__()
-
-    def __await__(self):
-        if self.semaphore:
-            return self.semaphore.__await__()
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        if self.semaphore:
-            await self.semaphore.__aexit__(exc_type, exc_val, exc_tb)
-
-
-class ModbusTcpProtocol(asyncio.Protocol):
-    def __init__(self, client):
-        self.client = client
-        self.transactions: Dict[str, asyncio.Future] = {}
-        self._cnt_lock = threading.Lock()
-        self.transaction_cnt = 0
-
-    def next_transaction(self):
-        with self._cnt_lock:
-            self.transaction_cnt = (self.transaction_cnt % 0xFFFE) + 1
-            return self.transaction_cnt
-
-    def connection_made(self, transport: transports.BaseTransport) -> None:
-        log.info(f"Modbus Client connected at {self.client.host}")
-
-    def data_received(self, data: bytes) -> None:
-        header, payload = data[:8], data[8:]
-        trans_id, protocol_id, length, unit_id, func_code = struct.unpack(
-            ">HHHBB", header
-        )
-        log.debug("Decode: " + " ".join(f"{byt:02X}" for byt in data))
-        fut = self.transactions.get(trans_id)
-        if fut:
-            decoders.from_func_code(fut, func_code, payload)
-
-    def connection_lost(self, exc: Optional[Exception]) -> None:
-        self.client.connected.clear()
-        log.info(f"Modbus Client disconnected from {self.client.host}")
-        if self.client.running:
-            for fut in self.transactions.values():
-                if not fut.done():
-                    fut.cancel()
-            asyncio.create_task(self.client.connect())
-
-    def new_transaction(self) -> Tuple[int, asyncio.Future]:
-        trans_id = self.next_transaction()
-        fut = asyncio.Future()
-        self.transactions[trans_id] = fut
-        return trans_id, fut
-
-
-@dataclass
-class ModbusTCPClient:
-    host: str
-    port: int = 502
-    client_port: int = 0
-    max_active_requests: Optional[int] = None
-    default_unit_id: int = 0
-    default_timeout: Optional[Number] = 0.2
-    auto_reconnect_after: Optional[Number] = None
-    transport: asyncio.Transport = None
-    protocol: ModbusTcpProtocol = None
-    running: bool = True
-
-    def __post_init__(self):
-        self.connected = asyncio.Event()
-        self.transaction_limit = TransactionLimit(
-            self.max_active_requests, self.connected
-        )
-
-    async def connect(self):
-        try:
-            if self.connected.is_set():
-                return
-        except AttributeError:
-            pass
-        loop = asyncio._get_running_loop()
-        while self.running:
-            try:
-                if self.client_port:
-                    sock = await self.build_reuse_socket()
-                    self.transport, self.protocol = await asyncio.wait_for(
-                        loop.create_connection(
-                            lambda: ModbusTcpProtocol(self),
-                            sock=sock,
-                        ),
-                        2,
-                    )
-                else:
-                    self.transport, self.protocol = await asyncio.wait_for(
-                        loop.create_connection(
-                            lambda: ModbusTcpProtocol(self), self.host, self.port
-                        ),
-                        2,
-                    )
-                self.connected.set()
-                return
-            except (OSError, asyncio.TimeoutError) as e:
-                if self.auto_reconnect_after:
-                    log.warning(e)
-                    log.info("Reconnecting to ModbusTCP")
-                    await asyncio.sleep(self.auto_reconnect_after)
-                else:
-                    log.exception(e)
-                    raise
-            except BaseException as e:
-                log.exception(e)
-                raise
-
-    async def build_reuse_socket(self):
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, struct.pack("ii", 1, 0))
-        sock.settimeout(10)
-        sock.bind(("", self.client_port))
-        sock.setblocking(False)
-        await asyncio.wait_for(
-            asyncio.get_event_loop().sock_connect(sock, (self.host, self.port)),
-            timeout=1,
-        )
-        return sock
-
-    def _encode_packet(
-        self, unit, function_code, address, trans_id, *values
-    ) -> bytearray:
-        packet = bytearray()
-        data = encoders.from_func_code(function_code, address, *values)
-        packet.extend(
-            struct.pack(">HHHBB", trans_id, 0x0000, len(data) + 2, unit, function_code)
-        )
-        packet.extend(data)
-        log.debug(("Encode: " + " ".join(f"{byt:02X}" for byt in packet)))
-        return packet
-
-    async def _request(
-        self, unit: int, function_code: int, address: int, *values: int, timeout
-    ):
-        if unit is None:
-            unit = self.default_unit_id
-        if not self.running:
-            raise RuntimeError("Client is stopped")
-        async with self.transaction_limit:
-            trans_id, fut = self.protocol.new_transaction()
-            packet = self._encode_packet(
-                unit, function_code, address, trans_id, *values
-            )
-            self.transport.write(packet)
-            timeout = timeout or self.default_timeout
-            try:
-                await asyncio.wait_for(fut, timeout)
-            finally:
-                self.protocol.transactions.pop(trans_id, None)
-            return fut.result()
-
-    async def read_coils(self, address: int, count: int, *, unit=None, timeout=None):
-        req = await self._request(unit, 0x01, address, count, timeout=timeout)
-        return req[:count]
-
-    async def read_discrete_inputs(
-        self, address: int, count: int, *, unit=None, timeout=None
-    ):
-        req = await self._request(unit, 0x02, address, count, timeout=timeout)
-        return req[:count]
-
-    async def read_holding_registers(
-        self, address: int, count: int, *, unit=None, timeout=None
-    ):
-        return await self._request(unit, 0x03, address, count, timeout=timeout)
-
-    async def read_input_registers(
-        self, address: int, count: int, *, unit=None, timeout=None
-    ):
-        return await self._request(unit, 0x04, address, count, timeout=timeout)
-
-    async def write_single_coil(
-        self, address: int, value: bool, *, unit=None, timeout=None
-    ):
-        return await self._request(unit, 0x05, address, value, timeout=timeout)
-
-    async def write_single_register(
-        self, address: int, value: int, *, unit=None, timeout=None
-    ):
-        return await self._request(unit, 0x06, address, value, timeout=timeout)
-
-    async def write_multiple_coils(
-        self, address: int, *values: bool, unit=None, timeout=None
-    ):
-        return await self._request(unit, 0x0F, address, *values, timeout=timeout)
-
-    async def write_multiple_registers(
-        self, address: int, *values: int, unit=None, timeout=None
-    ):
-        return await self._request(unit, 0x10, address, *values, timeout=timeout)
-
-    async def read_exception_status(self, unit=None, timeout=None):
-        function_code = 0x07
-        raise NotImplementedError
-
-    async def diagnostics(self, sub_function, *data, unit=None, timeout=None):
-        function_code = 0x08
-        raise NotImplementedError
-
-    def stop(self):
-        self.running = False
-        if self.transport:
-            self.transport.close()
-
-    disconnect = stop
+import asyncio
+import logging
+import socket
+from typing import Optional, Tuple, Union, Dict
+import struct
+from dataclasses import dataclass
+from asyncio import transports, Lock
+from aiomodbus import decoders, encoders
+
+Number = Union[int, float]
+
+log = logging.getLogger(__file__)
+
+
+@dataclass
+class TransactionLimit:
+    limit: Optional[int] = None
+    evt_connected: Optional[asyncio.Event] = None
+    evt_connected_timeout: float = 2
+
+    def __post_init__(self):
+        self.semaphore = None
+        if self.limit:
+            self.semaphore = asyncio.Semaphore(self.limit)
+
+    async def __aenter__(self):
+        if self.evt_connected:
+            try:
+                await asyncio.wait_for(
+                    self.evt_connected.wait(), self.evt_connected_timeout
+                )
+            except asyncio.TimeoutError:
+                raise ConnectionError("Client isn't connected")
+        if self.semaphore:
+            await self.semaphore.__aenter__()
+
+    def __await__(self):
+        if self.semaphore:
+            return self.semaphore.__await__()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        if self.semaphore:
+            await self.semaphore.__aexit__(exc_type, exc_val, exc_tb)
+
+
+class ModbusTcpProtocol(asyncio.Protocol):
+    def __init__(self, client):
+        self.client = client
+        self.transactions: Dict[int, asyncio.Future] = {}
+        self._cnt_lock = Lock()
+        self.transaction_cnt = 0
+
+    async def next_transaction(self):
+        async with self._cnt_lock:
+            self.transaction_cnt = (self.transaction_cnt % 0xFFFE) + 1
+            return self.transaction_cnt
+
+    def connection_made(self, transport: transports.BaseTransport) -> None:
+        log.info(f"Modbus Client connected at {self.client.host}")
+
+    def data_received(self, data: bytes) -> None:
+        while True:
+            header, payload = data[:8], data[8:]
+            trans_id, protocol_id, length, unit_id, func_code = struct.unpack(
+                ">HHHBB", header
+            )
+            log.debug("Decode: " + " ".join(f"{byt:02X}" for byt in data))
+            fut = self.transactions.get(trans_id)
+            if fut:
+                try:
+                    decoders.from_func_code(fut, func_code, payload[: length - 2])
+                    if len(payload) <= length - 2:
+                        break
+                except Exception as e:
+                    log.exception(e)
+                    break
+            data = payload[length - 2 :]
+
+    def connection_lost(self, exc: Optional[Exception]) -> None:
+        self.client.connected.clear()
+        log.info(f"Modbus Client disconnected from {self.client.host}")
+        if self.client.running:
+            for fut in self.transactions.values():
+                if not fut.done():
+                    fut.cancel()
+            asyncio.create_task(self.client.connect())
+
+    async def new_transaction(self) -> Tuple[int, asyncio.Future]:
+        trans_id = await self.next_transaction()
+        fut = asyncio.Future()
+        self.transactions[trans_id] = fut
+        return trans_id, fut
+
+
+@dataclass
+class ModbusTCPClient:
+    host: str
+    port: int = 502
+    client_port: int = 0
+    max_active_requests: Optional[int] = None
+    default_unit_id: int = 0
+    default_timeout: Optional[Number] = 0.2
+    auto_reconnect_after: Optional[Number] = None
+    transport: asyncio.Transport = None
+    protocol: ModbusTcpProtocol = None
+    running: bool = True
+
+    def __post_init__(self):
+        self.connected = asyncio.Event()
+        self.transaction_limit = TransactionLimit(
+            self.max_active_requests, self.connected
+        )
+
+    async def connect(self):
+        try:
+            if self.connected.is_set():
+                return
+        except AttributeError:
+            pass
+        loop = asyncio.get_running_loop()
+        while self.running:
+            try:
+                if self.client_port:
+                    sock = await self.build_reuse_socket()
+                    self.transport, self.protocol = await asyncio.wait_for(
+                        loop.create_connection(
+                            lambda: ModbusTcpProtocol(self),
+                            sock=sock,
+                        ),
+                        2,
+                    )
+                else:
+                    self.transport, self.protocol = await asyncio.wait_for(
+                        loop.create_connection(
+                            lambda: ModbusTcpProtocol(self), self.host, self.port
+                        ),
+                        2,
+                    )
+                self.connected.set()
+                return
+            except (OSError, asyncio.TimeoutError) as e:
+                if self.auto_reconnect_after:
+                    log.warning(e)
+                    log.info("Reconnecting to ModbusTCP")
+                    await asyncio.sleep(self.auto_reconnect_after)
+                else:
+                    log.exception(e)
+                    raise
+            except BaseException as e:
+                log.exception(e)
+                raise
+
+    async def build_reuse_socket(self):
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_LINGER, struct.pack("ii", 1, 0))
+        sock.settimeout(10)
+        sock.bind(("", self.client_port))
+        sock.setblocking(False)
+        await asyncio.wait_for(
+            asyncio.get_event_loop().sock_connect(sock, (self.host, self.port)),
+            timeout=1,
+        )
+        return sock
+
+    def _encode_packet(
+        self, unit, function_code, address, trans_id, *values
+    ) -> bytearray:
+        packet = bytearray()
+        data = encoders.from_func_code(function_code, address, *values)
+        packet.extend(
+            struct.pack(">HHHBB", trans_id, 0x0000, len(data) + 2, unit, function_code)
+        )
+        packet.extend(data)
+        log.debug(("Encode: " + " ".join(f"{byt:02X}" for byt in packet)))
+        return packet
+
+    async def _request(
+        self, unit: int, function_code: int, address: int, *values: int, timeout
+    ):
+        if unit is None:
+            unit = self.default_unit_id
+        if not self.running:
+            raise RuntimeError("Client is stopped")
+        async with self.transaction_limit:
+            trans_id, fut = await self.protocol.new_transaction()
+            packet = self._encode_packet(
+                unit, function_code, address, trans_id, *values
+            )
+            self.transport.write(packet)
+            timeout = timeout or self.default_timeout
+            try:
+                await asyncio.wait_for(fut, timeout)
+            finally:
+                self.protocol.transactions.pop(trans_id, None)
+            return fut.result()
+
+    async def read_coils(self, address: int, count: int, *, unit=None, timeout=None):
+        req = await self._request(unit, 0x01, address, count, timeout=timeout)
+        return req[:count]
+
+    async def read_discrete_inputs(
+        self, address: int, count: int, *, unit=None, timeout=None
+    ):
+        req = await self._request(unit, 0x02, address, count, timeout=timeout)
+        return req[:count]
+
+    async def read_holding_registers(
+        self, address: int, count: int, *, unit=None, timeout=None
+    ):
+        return await self._request(unit, 0x03, address, count, timeout=timeout)
+
+    async def read_input_registers(
+        self, address: int, count: int, *, unit=None, timeout=None
+    ):
+        return await self._request(unit, 0x04, address, count, timeout=timeout)
+
+    async def write_single_coil(
+        self, address: int, value: bool, *, unit=None, timeout=None
+    ):
+        return await self._request(unit, 0x05, address, value, timeout=timeout)
+
+    async def write_single_register(
+        self, address: int, value: int, *, unit=None, timeout=None
+    ):
+        return await self._request(unit, 0x06, address, value, timeout=timeout)
+
+    async def write_multiple_coils(
+        self, address: int, *values: bool, unit=None, timeout=None
+    ):
+        return await self._request(unit, 0x0F, address, *values, timeout=timeout)
+
+    async def write_multiple_registers(
+        self, address: int, *values: int, unit=None, timeout=None
+    ):
+        return await self._request(unit, 0x10, address, *values, timeout=timeout)
+
+    async def read_exception_status(self, unit=None, timeout=None):
+        function_code = 0x07
+        raise NotImplementedError
+
+    async def diagnostics(self, sub_function, *data, unit=None, timeout=None):
+        function_code = 0x08
+        raise NotImplementedError
+
+    def stop(self):
+        self.running = False
+        if self.transport:
+            self.transport.close()
+
+    disconnect = stop
```

### Comparing `aiomodbus-0.5.2/test/test_crc.py` & `aiomodbus-0.6.0/test/test_crc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import pytest
-import aiomodbus.crc
-
-
-@pytest.mark.parametrize(
-    "arr,result",
-    [
-        (bytearray(b"\x01\x03\x14" + b"\x00" * 20), 0xA367),
-        (bytearray(b"\x01\x03\x00\x01\x00\x0A"), 0x940D),
-    ],
-)
-def test_calc_crc(arr, result):
-    assert aiomodbus.crc.calc_crc(arr) == result
-
-
-@pytest.mark.parametrize(
-    "arr",
-    [
-        bytearray(b"\x01\x03\x14" + b"\x00" * 20 + b"\xA3\x67"),
-        bytearray(b"\x01\x03\x00\x01\x00\x0A\x94\x0D"),
-    ],
-)
-def test_check_crc_pass(arr):
-    aiomodbus.crc.check_crc(arr)
-
-
-@pytest.mark.parametrize(
-    "arr",
-    [
-        bytearray(b"\x01\x03\x14" + b"\x00" * 20 + b"\xA3\x67"),
-        bytearray(b"\x01\x03\x00\x01\x00\x0A\x94\x0D"),
-    ],
-)
-def test_check_crc_fail(arr):
-    arr[-1] = (arr[-1] + 1) % 255
-    with pytest.raises(aiomodbus.crc.CrcValidationError):
-        aiomodbus.crc.check_crc(arr)
+import pytest
+import aiomodbus.crc
+
+
+@pytest.mark.parametrize(
+    "arr,result",
+    [
+        (bytearray(b"\x01\x03\x14" + b"\x00" * 20), 0xA367),
+        (bytearray(b"\x01\x03\x00\x01\x00\x0A"), 0x940D),
+    ],
+)
+def test_calc_crc(arr, result):
+    assert aiomodbus.crc.calc_crc(arr) == result
+
+
+@pytest.mark.parametrize(
+    "arr",
+    [
+        bytearray(b"\x01\x03\x14" + b"\x00" * 20 + b"\xA3\x67"),
+        bytearray(b"\x01\x03\x00\x01\x00\x0A\x94\x0D"),
+    ],
+)
+def test_check_crc_pass(arr):
+    aiomodbus.crc.check_crc(arr)
+
+
+@pytest.mark.parametrize(
+    "arr",
+    [
+        bytearray(b"\x01\x03\x14" + b"\x00" * 20 + b"\xA3\x67"),
+        bytearray(b"\x01\x03\x00\x01\x00\x0A\x94\x0D"),
+    ],
+)
+def test_check_crc_fail(arr):
+    arr[-1] = (arr[-1] + 1) % 255
+    with pytest.raises(aiomodbus.crc.CrcValidationError):
+        aiomodbus.crc.check_crc(arr)
```

### Comparing `aiomodbus-0.5.2/test/test_rtu_protocol.py` & `aiomodbus-0.6.0/test/test_rtu_protocol.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-import pytest
-import struct
-from unittest.mock import MagicMock
-import aiomodbus
-import asyncio
-
-import aiomodbus.exceptions
-import aiomodbus.serial
-import aiomodbus.tcp
-
-
-def async_return(result):
-    f = asyncio.Future()
-    f.set_result(result)
-    return f
-
-
-def respond(protocol, arr):
-    def _tmp(data):
-        protocol.data_received(arr)
-
-    return _tmp
-
-
-@pytest.fixture
-def create_mock_coro(mocker, monkeypatch):
-    def _create_mock_patch_coro(to_patch=None):
-        mock = mocker.Mock()
-
-        async def _coro(*args, **kwargs):
-            return mock(*args, **kwargs)
-
-        if to_patch:  # <-- may not need/want to patch anything
-            monkeypatch.setattr(to_patch, _coro)
-        return mock, _coro
-
-    return _create_mock_patch_coro
-
-
-@pytest.fixture
-def mock_sleep(create_mock_coro):
-    # won't need the returned coroutine here
-    mock, _ = create_mock_coro(to_patch="asyncio.sleep")
-    return mock
-
-
-@pytest.fixture
-def client():
-    client = aiomodbus.serial.ModbusSerialClient("COM3", 9600, "N", 1)
-    client.transport = MagicMock()
-    client.protocol = aiomodbus.serial.ModbusSerialProtocol(client)
-    client.protocol.byte_time = 0.1
-    client.connected.set()
-    return client
-
-
-@pytest.mark.asyncio
-async def test_read_coils(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x01\x05\xCD\x6B\xB2\x0E\x1B\x45\xE6"
-    )
-    fut = asyncio.create_task(client.read_coils(0x13, 0x25, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(b"\x11\x01\x00\x13\x00\x25\x0E\x84")
-    assert fut.result() == [
-        True,
-        False,
-        True,
-        True,
-        False,
-        False,
-        True,
-        True,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-        False,
-        False,
-        True,
-        False,
-        False,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-        True,
-        False,
-        False,
-        False,
-        False,
-        True,
-        True,
-        False,
-        True,
-        True,
-    ]
-
-
-@pytest.mark.asyncio
-async def test_read_discrete_inputs(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x02\x03\xAC\xDB\x35\x20\x18"
-    )
-    fut = asyncio.create_task(client.read_discrete_inputs(0xC4, 0x16, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(b"\x11\x02\x00\xC4\x00\x16\xBA\xA9")
-    assert fut.result() == [
-        False,
-        False,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-        True,
-        False,
-        True,
-        True,
-        False,
-        True,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-    ]
-
-
-@pytest.mark.asyncio
-async def test_read_holding_registers(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD"
-    )
-    fut = asyncio.create_task(client.read_holding_registers(0x6B, 0x3, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(b"\x11\x03\x00\x6b\x00\x03\x76\x87")
-    assert fut.result() == [0xAE41, 0x5652, 0x4340]
-
-
-@pytest.mark.asyncio
-async def test_read_input_registers(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x04\x02\x00\x0A\xF8\xF4"
-    )
-    fut = asyncio.create_task(client.read_input_registers(0x08, 0x1, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(b"\x11\x04\x00\x08\x00\x01\xB2\x98")
-    assert fut.result() == [0xA]
-
-
-@pytest.mark.asyncio
-async def test_write_coil(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x05\x00\xAC\xFF\x00\x4E\x8B"
-    )
-    fut = asyncio.create_task(client.write_single_coil(0xAC, True, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(b"\x11\x05\x00\xAC\xFF\x00\x4E\x8B")
-
-
-@pytest.mark.asyncio
-async def test_write_register(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x06\x00\x01\x00\x03\x9A\x9B"
-    )
-    fut = asyncio.create_task(client.write_single_register(0x01, 0x3, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(b"\x11\x06\x00\x01\x00\x03\x9A\x9B")
-
-
-@pytest.mark.asyncio
-async def test_write_coils(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x0F\x00\x13\x00\x0A\x26\x99"
-    )
-    fut = asyncio.create_task(
-        client.write_multiple_coils(
-            0x13,
-            True,
-            False,
-            True,
-            True,
-            False,
-            False,
-            True,
-            True,
-            True,
-            False,
-            unit=0x11,
-        )
-    )
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x11\x0F\x00\x13\x00\x0A\x02\xCD\x01\xBF\x0B"
-    )
-
-
-@pytest.mark.asyncio
-async def test_write_registers(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x11\x10\x00\x01\x00\x02\x12\x98"
-    )
-    fut = asyncio.create_task(
-        client.write_multiple_registers(0x01, 0xA, 0x102, unit=0x11)
-    )
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x11\x10\x00\x01\x00\x02\x04\x00\x0A\x01\x02\xC6\xF0"
-    )
-
-
-@pytest.mark.parametrize(
-    "exceptioncls,exception_code",
-    [
-        (aiomodbus.exceptions.IllegalFunction, 1),
-        (aiomodbus.exceptions.IllegalDataAddress, 2),
-        (aiomodbus.exceptions.IllegalDataValue, 3),
-        (aiomodbus.exceptions.SlaveDeviceFailure, 4),
-        (aiomodbus.exceptions.AcknowledgeError, 5),
-        (aiomodbus.exceptions.DeviceBusy, 6),
-        (aiomodbus.exceptions.NegativeAcknowledgeError, 7),
-        (aiomodbus.exceptions.MemoryParityError, 8),
-        (aiomodbus.exceptions.GatewayPathUnavailable, 10),
-        (aiomodbus.exceptions.GatewayDeviceFailedToRespond, 11),
-        (ConnectionError, 12),
-    ],
-)
-@pytest.mark.asyncio
-async def test_exceptions(exceptioncls, exception_code, mock_sleep, client):
-    exc_packet = bytearray([0x11, 0x83, exception_code])
-    exc_packet.extend(struct.pack(">H", aiomodbus.crc.calc_crc(exc_packet)))
-    client.transport.write.side_effect = respond(client.protocol, exc_packet)
-    with pytest.raises(exceptioncls):
-        await client.read_holding_registers(0x6B, 0x3, unit=0x11)
-    client.transport.write.assert_called_once_with(b"\x11\x03\x00\x6b\x00\x03\x76\x87")
-
-
-@pytest.mark.asyncio
-async def test_read_exception_status(client):
-    with pytest.raises(NotImplementedError):
-        await client.read_exception_status()
-
-
-@pytest.mark.asyncio
-async def test_diagnostics(client):
-    with pytest.raises(NotImplementedError):
-        await client.diagnostics(None)
+import pytest
+import struct
+from unittest.mock import MagicMock
+import aiomodbus
+import asyncio
+
+import aiomodbus.exceptions
+import aiomodbus.serial
+import aiomodbus.tcp
+
+
+def async_return(result):
+    f = asyncio.Future()
+    f.set_result(result)
+    return f
+
+
+def respond(protocol, arr):
+    def _tmp(data):
+        protocol.data_received(arr)
+
+    return _tmp
+
+
+@pytest.fixture
+def create_mock_coro(mocker, monkeypatch):
+    def _create_mock_patch_coro(to_patch=None):
+        mock = mocker.Mock()
+
+        async def _coro(*args, **kwargs):
+            return mock(*args, **kwargs)
+
+        if to_patch:  # <-- may not need/want to patch anything
+            monkeypatch.setattr(to_patch, _coro)
+        return mock, _coro
+
+    return _create_mock_patch_coro
+
+
+@pytest.fixture
+def mock_sleep(create_mock_coro):
+    # won't need the returned coroutine here
+    mock, _ = create_mock_coro(to_patch="asyncio.sleep")
+    return mock
+
+
+@pytest.fixture
+def client():
+    client = aiomodbus.serial.ModbusSerialClient("COM3", 9600, "N", 1)
+    client.transport = MagicMock()
+    client.protocol = aiomodbus.serial.ModbusSerialProtocol(client)
+    client.protocol.byte_time = 0.1
+    client.connected.set()
+    return client
+
+
+@pytest.mark.asyncio
+async def test_read_coils(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x01\x05\xCD\x6B\xB2\x0E\x1B\x45\xE6"
+    )
+    fut = asyncio.create_task(client.read_coils(0x13, 0x25, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(b"\x11\x01\x00\x13\x00\x25\x0E\x84")
+    assert fut.result() == [
+        True,
+        False,
+        True,
+        True,
+        False,
+        False,
+        True,
+        True,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+        False,
+        False,
+        True,
+        False,
+        False,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+        True,
+        False,
+        False,
+        False,
+        False,
+        True,
+        True,
+        False,
+        True,
+        True,
+    ]
+
+
+@pytest.mark.asyncio
+async def test_read_discrete_inputs(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x02\x03\xAC\xDB\x35\x20\x18"
+    )
+    fut = asyncio.create_task(client.read_discrete_inputs(0xC4, 0x16, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(b"\x11\x02\x00\xC4\x00\x16\xBA\xA9")
+    assert fut.result() == [
+        False,
+        False,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+        True,
+        False,
+        True,
+        True,
+        False,
+        True,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+    ]
+
+
+@pytest.mark.asyncio
+async def test_read_holding_registers(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD"
+    )
+    fut = asyncio.create_task(client.read_holding_registers(0x6B, 0x3, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(b"\x11\x03\x00\x6b\x00\x03\x76\x87")
+    assert fut.result() == [0xAE41, 0x5652, 0x4340]
+
+
+@pytest.mark.asyncio
+async def test_read_input_registers(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x04\x02\x00\x0A\xF8\xF4"
+    )
+    fut = asyncio.create_task(client.read_input_registers(0x08, 0x1, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(b"\x11\x04\x00\x08\x00\x01\xB2\x98")
+    assert fut.result() == [0xA]
+
+
+@pytest.mark.asyncio
+async def test_write_coil(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x05\x00\xAC\xFF\x00\x4E\x8B"
+    )
+    fut = asyncio.create_task(client.write_single_coil(0xAC, True, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(b"\x11\x05\x00\xAC\xFF\x00\x4E\x8B")
+
+
+@pytest.mark.asyncio
+async def test_write_register(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x06\x00\x01\x00\x03\x9A\x9B"
+    )
+    fut = asyncio.create_task(client.write_single_register(0x01, 0x3, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(b"\x11\x06\x00\x01\x00\x03\x9A\x9B")
+
+
+@pytest.mark.asyncio
+async def test_write_coils(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x0F\x00\x13\x00\x0A\x26\x99"
+    )
+    fut = asyncio.create_task(
+        client.write_multiple_coils(
+            0x13,
+            True,
+            False,
+            True,
+            True,
+            False,
+            False,
+            True,
+            True,
+            True,
+            False,
+            unit=0x11,
+        )
+    )
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x11\x0F\x00\x13\x00\x0A\x02\xCD\x01\xBF\x0B"
+    )
+
+
+@pytest.mark.asyncio
+async def test_write_registers(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x11\x10\x00\x01\x00\x02\x12\x98"
+    )
+    fut = asyncio.create_task(
+        client.write_multiple_registers(0x01, 0xA, 0x102, unit=0x11)
+    )
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x11\x10\x00\x01\x00\x02\x04\x00\x0A\x01\x02\xC6\xF0"
+    )
+
+
+@pytest.mark.parametrize(
+    "exceptioncls,exception_code",
+    [
+        (aiomodbus.exceptions.IllegalFunction, 1),
+        (aiomodbus.exceptions.IllegalDataAddress, 2),
+        (aiomodbus.exceptions.IllegalDataValue, 3),
+        (aiomodbus.exceptions.SlaveDeviceFailure, 4),
+        (aiomodbus.exceptions.AcknowledgeError, 5),
+        (aiomodbus.exceptions.DeviceBusy, 6),
+        (aiomodbus.exceptions.NegativeAcknowledgeError, 7),
+        (aiomodbus.exceptions.MemoryParityError, 8),
+        (aiomodbus.exceptions.GatewayPathUnavailable, 10),
+        (aiomodbus.exceptions.GatewayDeviceFailedToRespond, 11),
+        (ConnectionError, 12),
+    ],
+)
+@pytest.mark.asyncio
+async def test_exceptions(exceptioncls, exception_code, mock_sleep, client):
+    exc_packet = bytearray([0x11, 0x83, exception_code])
+    exc_packet.extend(struct.pack(">H", aiomodbus.crc.calc_crc(exc_packet)))
+    client.transport.write.side_effect = respond(client.protocol, exc_packet)
+    with pytest.raises(exceptioncls):
+        await client.read_holding_registers(0x6B, 0x3, unit=0x11)
+    client.transport.write.assert_called_once_with(b"\x11\x03\x00\x6b\x00\x03\x76\x87")
+
+
+@pytest.mark.asyncio
+async def test_read_exception_status(client):
+    with pytest.raises(NotImplementedError):
+        await client.read_exception_status()
+
+
+@pytest.mark.asyncio
+async def test_diagnostics(client):
+    with pytest.raises(NotImplementedError):
+        await client.diagnostics(None)
```

### Comparing `aiomodbus-0.5.2/test/test_tcp_protocol.py` & `aiomodbus-0.6.0/test/test_tcp_protocol.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-import pytest
-import struct
-from unittest.mock import MagicMock
-import aiomodbus
-import asyncio
-
-import aiomodbus.exceptions
-import aiomodbus.serial
-import aiomodbus.tcp
-
-
-def async_return(result):
-    f = asyncio.Future()
-    f.set_result(result)
-    return f
-
-
-def respond(protocol, arr):
-    def _tmp(data):
-        protocol.data_received(arr)
-
-    return _tmp
-
-
-@pytest.fixture
-def create_mock_coro(mocker, monkeypatch):
-    def _create_mock_patch_coro(to_patch=None):
-        mock = mocker.Mock()
-
-        async def _coro(*args, **kwargs):
-            return mock(*args, **kwargs)
-
-        if to_patch:  # <-- may not need/want to patch anything
-            monkeypatch.setattr(to_patch, _coro)
-        return mock, _coro
-
-    return _create_mock_patch_coro
-
-
-@pytest.fixture
-def mock_sleep(create_mock_coro):
-    # won't need the returned coroutine here
-    mock, _ = create_mock_coro(to_patch="asyncio.sleep")
-    return mock
-
-
-@pytest.fixture
-def client():
-    client = aiomodbus.tcp.ModbusTCPClient("127.0.0.1", 502)
-    client.transport = MagicMock()
-    client.protocol = aiomodbus.tcp.ModbusTcpProtocol(client)
-    client.connected.set()
-    return client
-
-
-@pytest.mark.asyncio
-async def test_read_coils(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x08\x11\x01\x05\xCD\x6B\xB2\x0E\x1B"
-    )
-    fut = asyncio.create_task(client.read_coils(0x13, 0x25, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x06\x11\x01\x00\x13\x00\x25"
-    )
-    assert fut.result() == [
-        True,
-        False,
-        True,
-        True,
-        False,
-        False,
-        True,
-        True,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-        False,
-        False,
-        True,
-        False,
-        False,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-        True,
-        False,
-        False,
-        False,
-        False,
-        True,
-        True,
-        False,
-        True,
-        True,
-    ]
-
-
-@pytest.mark.asyncio
-async def test_read_discrete_inputs(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x02\x03\xAC\xDB\x35"
-    )
-    fut = asyncio.create_task(client.read_discrete_inputs(0xC4, 0x16, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x06\x11\x02\x00\xC4\x00\x16"
-    )
-    assert fut.result() == [
-        False,
-        False,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-        True,
-        False,
-        True,
-        True,
-        False,
-        True,
-        True,
-        True,
-        False,
-        True,
-        False,
-        True,
-        True,
-    ]
-
-
-@pytest.mark.asyncio
-async def test_read_holding_registers(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x09\x11\x03\x06\xAE\x41\x56\x52\x43\x40"
-    )
-    fut = asyncio.create_task(client.read_holding_registers(0x6B, 0x3, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x06\x11\x03\x00\x6b\x00\x03"
-    )
-    assert fut.result() == (0xAE41, 0x5652, 0x4340)
-
-
-@pytest.mark.asyncio
-async def test_read_input_registers(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x05\x11\x04\x02\x00\x0A"
-    )
-    fut = asyncio.create_task(client.read_input_registers(0x08, 0x1, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x06\x11\x04\x00\x08\x00\x01"
-    )
-    assert fut.result() == (0xA,)
-
-
-@pytest.mark.asyncio
-async def test_write_coil(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x05\x00\xAC\xFF\x00"
-    )
-    fut = asyncio.create_task(client.write_single_coil(0xAC, True, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x06\x11\x05\x00\xAC\xFF\x00"
-    )
-
-
-@pytest.mark.asyncio
-async def test_write_register(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x06\x00\x01\x00\x03"
-    )
-    fut = asyncio.create_task(client.write_single_register(0x01, 0x3, unit=0x11))
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x06\x11\x06\x00\x01\x00\x03"
-    )
-
-
-@pytest.mark.asyncio
-async def test_write_coils(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x0F\x00\x13\x00\x0A"
-    )
-    fut = asyncio.create_task(
-        client.write_multiple_coils(
-            0x13,
-            True,
-            False,
-            True,
-            True,
-            False,
-            False,
-            True,
-            True,
-            True,
-            False,
-            unit=0x11,
-        )
-    )
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x09\x11\x0F\x00\x13\x00\x0A\x02\xCD\x01"
-    )
-
-
-@pytest.mark.asyncio
-async def test_write_registers(mock_sleep, client):
-    client.transport.write.side_effect = respond(
-        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x10\x00\x01\x00\x02"
-    )
-    fut = asyncio.create_task(
-        client.write_multiple_registers(0x01, 0xA, 0x102, unit=0x11)
-    )
-    await fut
-    client.transport.write.assert_called_once_with(
-        b"\x00\x01\x00\x00\x00\x0b\x11\x10\x00\x01\x00\x02\x04\x00\x0A\x01\x02"
-    )
-
-
-@pytest.mark.parametrize(
-    "exceptioncls,exception_code",
-    [
-        (aiomodbus.exceptions.IllegalFunction, 1),
-        (aiomodbus.exceptions.IllegalDataAddress, 2),
-        (aiomodbus.exceptions.IllegalDataValue, 3),
-        (aiomodbus.exceptions.SlaveDeviceFailure, 4),
-        (aiomodbus.exceptions.AcknowledgeError, 5),
-        (aiomodbus.exceptions.DeviceBusy, 6),
-        (aiomodbus.exceptions.NegativeAcknowledgeError, 7),
-        (aiomodbus.exceptions.MemoryParityError, 8),
-        (aiomodbus.exceptions.GatewayPathUnavailable, 10),
-        (aiomodbus.exceptions.GatewayDeviceFailedToRespond, 11),
-        (ConnectionError, 12),
-    ],
-)
-@pytest.mark.asyncio
-async def test_exceptions(exceptioncls, exception_code, mock_sleep, client):
-    resp = bytearray(b"\x00\x01\x00\x00\x00\x03\x11\x83")
-    resp.append(exception_code)
-    client.transport.write.side_effect = respond(client.protocol, bytes(resp))
-    with pytest.raises(exceptioncls):
-        await client.read_holding_registers(0x6B, 0x3, unit=0x11)
-
-
-@pytest.mark.asyncio
-async def test_read_exception_status(client):
-    with pytest.raises(NotImplementedError):
-        await client.read_exception_status()
-
-
-@pytest.mark.asyncio
-async def test_diagnostics(client):
-    with pytest.raises(NotImplementedError):
-        await client.diagnostics(None)
+import pytest
+import struct
+from unittest.mock import MagicMock
+import aiomodbus
+import asyncio
+
+import aiomodbus.exceptions
+import aiomodbus.serial
+import aiomodbus.tcp
+
+
+def async_return(result):
+    f = asyncio.Future()
+    f.set_result(result)
+    return f
+
+
+def respond(protocol, arr):
+    def _tmp(data):
+        protocol.data_received(arr)
+
+    return _tmp
+
+
+@pytest.fixture
+def create_mock_coro(mocker, monkeypatch):
+    def _create_mock_patch_coro(to_patch=None):
+        mock = mocker.Mock()
+
+        async def _coro(*args, **kwargs):
+            return mock(*args, **kwargs)
+
+        if to_patch:  # <-- may not need/want to patch anything
+            monkeypatch.setattr(to_patch, _coro)
+        return mock, _coro
+
+    return _create_mock_patch_coro
+
+
+@pytest.fixture
+def mock_sleep(create_mock_coro):
+    # won't need the returned coroutine here
+    mock, _ = create_mock_coro(to_patch="asyncio.sleep")
+    return mock
+
+
+@pytest.fixture
+def client():
+    client = aiomodbus.tcp.ModbusTCPClient("127.0.0.1", 502)
+    client.transport = MagicMock()
+    client.protocol = aiomodbus.tcp.ModbusTcpProtocol(client)
+    client.connected.set()
+    return client
+
+
+@pytest.mark.asyncio
+async def test_read_coils(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x08\x11\x01\x05\xCD\x6B\xB2\x0E\x1B"
+    )
+    fut = asyncio.create_task(client.read_coils(0x13, 0x25, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x06\x11\x01\x00\x13\x00\x25"
+    )
+    assert fut.result() == [
+        True,
+        False,
+        True,
+        True,
+        False,
+        False,
+        True,
+        True,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+        False,
+        False,
+        True,
+        False,
+        False,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+        True,
+        False,
+        False,
+        False,
+        False,
+        True,
+        True,
+        False,
+        True,
+        True,
+    ]
+
+
+@pytest.mark.asyncio
+async def test_read_discrete_inputs(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x02\x03\xAC\xDB\x35"
+    )
+    fut = asyncio.create_task(client.read_discrete_inputs(0xC4, 0x16, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x06\x11\x02\x00\xC4\x00\x16"
+    )
+    assert fut.result() == [
+        False,
+        False,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+        True,
+        False,
+        True,
+        True,
+        False,
+        True,
+        True,
+        True,
+        False,
+        True,
+        False,
+        True,
+        True,
+    ]
+
+
+@pytest.mark.asyncio
+async def test_read_holding_registers(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x09\x11\x03\x06\xAE\x41\x56\x52\x43\x40"
+    )
+    fut = asyncio.create_task(client.read_holding_registers(0x6B, 0x3, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x06\x11\x03\x00\x6b\x00\x03"
+    )
+    assert fut.result() == (0xAE41, 0x5652, 0x4340)
+
+
+@pytest.mark.asyncio
+async def test_read_input_registers(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x05\x11\x04\x02\x00\x0A"
+    )
+    fut = asyncio.create_task(client.read_input_registers(0x08, 0x1, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x06\x11\x04\x00\x08\x00\x01"
+    )
+    assert fut.result() == (0xA,)
+
+
+@pytest.mark.asyncio
+async def test_write_coil(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x05\x00\xAC\xFF\x00"
+    )
+    fut = asyncio.create_task(client.write_single_coil(0xAC, True, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x06\x11\x05\x00\xAC\xFF\x00"
+    )
+
+
+@pytest.mark.asyncio
+async def test_write_register(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x06\x00\x01\x00\x03"
+    )
+    fut = asyncio.create_task(client.write_single_register(0x01, 0x3, unit=0x11))
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x06\x11\x06\x00\x01\x00\x03"
+    )
+
+
+@pytest.mark.asyncio
+async def test_write_coils(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x0F\x00\x13\x00\x0A"
+    )
+    fut = asyncio.create_task(
+        client.write_multiple_coils(
+            0x13,
+            True,
+            False,
+            True,
+            True,
+            False,
+            False,
+            True,
+            True,
+            True,
+            False,
+            unit=0x11,
+        )
+    )
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x09\x11\x0F\x00\x13\x00\x0A\x02\xCD\x01"
+    )
+
+
+@pytest.mark.asyncio
+async def test_write_registers(mock_sleep, client):
+    client.transport.write.side_effect = respond(
+        client.protocol, b"\x00\x01\x00\x00\x00\x06\x11\x10\x00\x01\x00\x02"
+    )
+    fut = asyncio.create_task(
+        client.write_multiple_registers(0x01, 0xA, 0x102, unit=0x11)
+    )
+    await fut
+    client.transport.write.assert_called_once_with(
+        b"\x00\x01\x00\x00\x00\x0b\x11\x10\x00\x01\x00\x02\x04\x00\x0A\x01\x02"
+    )
+
+
+@pytest.mark.parametrize(
+    "exceptioncls,exception_code",
+    [
+        (aiomodbus.exceptions.IllegalFunction, 1),
+        (aiomodbus.exceptions.IllegalDataAddress, 2),
+        (aiomodbus.exceptions.IllegalDataValue, 3),
+        (aiomodbus.exceptions.SlaveDeviceFailure, 4),
+        (aiomodbus.exceptions.AcknowledgeError, 5),
+        (aiomodbus.exceptions.DeviceBusy, 6),
+        (aiomodbus.exceptions.NegativeAcknowledgeError, 7),
+        (aiomodbus.exceptions.MemoryParityError, 8),
+        (aiomodbus.exceptions.GatewayPathUnavailable, 10),
+        (aiomodbus.exceptions.GatewayDeviceFailedToRespond, 11),
+        (ConnectionError, 12),
+    ],
+)
+@pytest.mark.asyncio
+async def test_exceptions(exceptioncls, exception_code, mock_sleep, client):
+    resp = bytearray(b"\x00\x01\x00\x00\x00\x03\x11\x83")
+    resp.append(exception_code)
+    client.transport.write.side_effect = respond(client.protocol, bytes(resp))
+    with pytest.raises(exceptioncls):
+        await client.read_holding_registers(0x6B, 0x3, unit=0x11)
+
+
+@pytest.mark.asyncio
+async def test_read_exception_status(client):
+    with pytest.raises(NotImplementedError):
+        await client.read_exception_status()
+
+
+@pytest.mark.asyncio
+async def test_diagnostics(client):
+    with pytest.raises(NotImplementedError):
+        await client.diagnostics(None)
```

