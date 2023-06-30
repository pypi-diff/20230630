# Comparing `tmp/ssh_remote_control-0.2.0.tar.gz` & `tmp/ssh_remote_control-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.2.0.tar", last modified: Wed Jun 28 10:41:41 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.2.1.tar", last modified: Fri Jun 30 11:25:51 2023, max compression
```

## Comparing `ssh_remote_control-0.2.0.tar` & `ssh_remote_control-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 10:41:41.282119 ssh_remote_control-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1569 2023-06-28 10:41:41.279117 ssh_remote_control-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.2.0/README.md
--rw-rw-rw-   0        0        0      846 2023-06-28 10:40:43.000000 ssh_remote_control-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 10:41:41.283116 ssh_remote_control-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 10:41:41.169983 ssh_remote_control-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 10:41:41.212988 ssh_remote_control-0.2.0/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10443 2023-06-28 10:38:00.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-06-28 10:38:00.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/collection.py
--rw-rw-rw-   0        0        0     5370 2023-06-28 10:38:00.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/command.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:41:41.277116 ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/
--rw-rw-rw-   0        0        0      161 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/const.py
--rw-rw-rw-   0        0        0     3825 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/linux.py
--rw-rw-rw-   0        0        0     3720 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/windows_cmd.py
--rw-rw-rw-   0        0        0     3961 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/windows_ps.py
--rw-rw-rw-   0        0        0      637 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/errors.py
--rw-rw-rw-   0        0        0      645 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      222 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1346 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     4526 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     8447 2023-06-28 10:38:01.000000 ssh_remote_control-0.2.0/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:41:41.261276 ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1569 2023-06-28 10:41:41.000000 ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      840 2023-06-28 10:41:41.000000 ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 10:41:41.000000 ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-28 10:41:41.000000 ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-28 10:41:41.000000 ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 11:25:51.584272 ssh_remote_control-0.2.1/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-30 11:25:51.582271 ssh_remote_control-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.2.1/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-30 11:22:05.000000 ssh_remote_control-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:25:51.584272 ssh_remote_control-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 11:25:51.480646 ssh_remote_control-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 11:25:51.530584 ssh_remote_control-0.2.1/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10582 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/collection.py
+-rw-rw-rw-   0        0        0     5199 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/command.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:25:51.580270 ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/
+-rw-rw-rw-   0        0        0      161 2023-06-30 11:20:02.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-30 11:20:02.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/const.py
+-rw-rw-rw-   0        0        0     3825 2023-06-30 11:20:02.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/linux.py
+-rw-rw-rw-   0        0        0     3720 2023-06-30 11:20:02.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/windows_cmd.py
+-rw-rw-rw-   0        0        0     3961 2023-06-30 11:20:02.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/windows_ps.py
+-rw-rw-rw-   0        0        0      468 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/errors.py
+-rw-rw-rw-   0        0        0      645 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      222 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1346 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     4133 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     8606 2023-06-30 11:20:00.000000 ssh_remote_control-0.2.1/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:25:51.569275 ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-30 11:25:51.000000 ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2023-06-30 11:25:51.000000 ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:25:51.000000 ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-30 11:25:51.000000 ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-30 11:25:51.000000 ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.2.0/LICENSE` & `ssh_remote_control-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/PKG-INFO` & `ssh_remote_control-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_remote_control
-Version: 0.2.0
+Version: 0.2.1
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.2.0/README.md` & `ssh_remote_control-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/pyproject.toml` & `ssh_remote_control-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 import paramiko
 import wakeonlan
 
 from .collection import Collection
 from .command import ActionCommand, Command, SensorCommand
 from .default_collections import ActionKey, SensorKey
 from .errors import (
-    CommandExecuteError,
-    CommandFormatError,
-    MACAdressUnavailableError,
+    CommandError,
     OfflineError,
+    RemoteError,
     SSHAuthError,
     SSHConnectError,
     SSHHostKeyUnknownError,
 )
 from .event import Event
-from .helpers import name_to_key
 from .manager import DEFAULT_COMMAND_TIMEOUT, CommandOutput, Manager
 from .sensor import BinarySensor, NumberSensor, Sensor, TextSensor
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("")
 
 DEFAULT_SSH_PORT = 22
@@ -61,15 +59,15 @@
 
     def update(self, name, value) -> None:
         """Update."""
         if getattr(self, name) == value:
             return
 
         setattr(self, name, value)
-        self._remote.logger.info("%s: %s changed to %s", self._remote.name, name, value)
+        self._remote.logger.debug("%s: %s is %s", self._remote.name, name, value)
         self.on_change.notify(self)
 
 
 class Remote(Manager):
     """The Remote class."""
 
     def __init__(
@@ -104,15 +102,14 @@
         self.ssh_password = ssh_password
         self.ssh_key_file = ssh_key_file
         self.ssh_timeout = ssh_timeout
         self.ping_timeout = ping_timeout
         self.allow_turn_off = allow_turn_off
         self.state = State(self)
         self._ssh_client = paramiko.SSHClient()
-        self._ssh_client.set_log_channel(self.logger.name)
         self._ssh_client.load_system_host_keys()
         self._ssh_client.set_missing_host_key_policy(
             paramiko.AutoAddPolicy if add_host_keys else CustomRejectPolicy
         )
 
         if ssh_host_keys_file:
             with open(ssh_host_keys_file, "a", encoding="utf-8"):
@@ -153,49 +150,63 @@
 
     @property
     def machine_type(self) -> str | None:
         """Machine type."""
         if sensor := self.sensors_by_key.get(SensorKey.MACHINE_TYPE):
             return sensor.last_known_value
 
-    def _execute_command_string(self, string: str) -> CommandOutput:
+    def _execute_command_string(self, string: str, timeout: int) -> CommandOutput:
         if not self.state.is_connected:
-            raise CommandExecuteError("Not connected")
+            raise CommandError("Not connected")
 
         try:
-            _, stdout_file, stderr_file = self._ssh_client.exec_command(
-                string, timeout=float(self.ssh_timeout)
+            stdin, stdout, stderr = self._ssh_client.exec_command(
+                string,
+                get_pty=True,  # required to be able to interrupt the command
+                timeout=float(timeout),  # channel timeout, used to be self.ssh_timeout
             )
         except Exception as exc:
             self._disconnect()
-            raise CommandExecuteError("Disconnected during execution") from exc
+            raise CommandError("Disconnected before execution") from exc
 
         try:
             return CommandOutput(
                 time(),
-                [line.strip() for line in stdout_file.readlines()],
-                [line.strip() for line in stderr_file.readlines()],
-                stdout_file.channel.recv_exit_status(),
+                [line.strip() for line in stdout.readlines()],
+                [line.strip() for line in stderr.readlines()],
+                stdout.channel.recv_exit_status(),
             )
+        except TimeoutError:
+            pass
         except Exception as exc:
             self._disconnect()
-            raise CommandExecuteError("Disconnected after execution") from exc
+            raise CommandError("Disconnected during execution") from exc
+
+        try:
+            # Interrupt the command if it takes longer then timeout
+            # https://github.com/fabric/fabric/blob/2.0/fabric/runners.py#L47-L59
+            stdin.channel.send("\x03")
+        except Exception as exc:
+            self._disconnect()
+            raise CommandError(f"Disconnected after timeout ({exc})") from exc
+
+        raise CommandError("Command interrupted after timeout")
 
     def _connect(self) -> None:
         if self.state.is_connected:
             return
 
         try:
             self._ssh_client.connect(
                 self.host,
                 self.ssh_port,
                 self.ssh_user,
                 self.ssh_password,
                 key_filename=self.ssh_key_file,
-                timeout=self.ssh_timeout,
+                timeout=self.ssh_timeout,  # timeout for the TCP connect
                 allow_agent=False,
             )
         except SSHHostKeyUnknownError:
             self._disconnect()
             raise
         except paramiko.AuthenticationException as exc:
             self._disconnect()
@@ -210,29 +221,24 @@
         if not self.state.is_connected:
             return
 
         self._ssh_client.close()
         self.state.update(IS_CONNECTED, False)
 
         for command in self.sensor_commands:
-            command.update_sensors(None)
+            command.update_sensors(self, None)
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         loop = asyncio.get_running_loop()
         timeout = command_timeout or self.command_timeout
-
-        try:
-            async with async_timeout.timeout(timeout):
-                return await loop.run_in_executor(
-                    None, self._execute_command_string, string
-                )
-        except asyncio.TimeoutError as exc:
-            raise CommandExecuteError(f"Timeout reached ({timeout} sec)") from exc
+        return await loop.run_in_executor(
+            None, self._execute_command_string, string, timeout
+        )
 
     async def async_connect(self) -> None:
         """Connect the SSH client.
 
         Set `state.is_connected` to `True` and update all
         sensor commands if successful, otherwise disconnect
         and raise an error.
@@ -244,22 +250,22 @@
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._connect)
 
         for command in self.sensor_commands:
             try:
                 await self.async_execute_command(command)
-            except (CommandFormatError, CommandExecuteError):
+            except CommandError:
                 pass
 
     async def async_disconnect(self) -> None:
         """Disconnect the SSH client.
 
-        Set `state.is_connected` to `False` and the
-        sensor values of all sensor commands to `None`.
+        Set `state.is_connected` to `False` and
+        update all sensor commands with `None`.
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._disconnect)
 
     async def async_update_state(self, *, raise_errors: bool = False) -> None:
         """Update state.
 
@@ -269,26 +275,26 @@
             SSHAuthError
             SSHConnectError (`raise_errors`)
         """
         if self.state.is_connected:
             try:
                 await self.async_execute_command(_TEST_COMMAND)
                 return
-            except CommandExecuteError:
+            except CommandError:
                 pass
 
         try:
             host = await icmplib.async_ping(
                 self.host,
                 count=1,
                 timeout=self.ping_timeout,
                 privileged=False,
             )
         except Exception as exc:  # pylint: disable=broad-except
-            self.logger.info("%s: Ping request failed: %s", self.name, exc)
+            self.logger.debug("%s: Ping request failed (%s)", self.name, exc)
             self.state.update(IS_ONLINE, False)
         else:
             self.state.update(IS_ONLINE, host.is_alive)
 
         if not self.state.is_online:
             if raise_errors:
                 raise OfflineError("Host is offline")
@@ -300,28 +306,27 @@
             if raise_errors:
                 raise
 
     async def async_turn_on(self) -> None:
         """Turn the host on.
 
         Raises:
-            MACAddressUnavailableError
+            RemoteError
         """
         if self.state.is_online:
             return
 
         if self.mac_address is None:
-            raise MACAdressUnavailableError("MAC address is unavailable")
+            raise RemoteError("MAC address is unavailable")
 
         wakeonlan.send_magic_packet(self.mac_address)
 
     async def async_turn_off(self) -> None:
-        """Turn the host on.
+        """Turn the host off.
 
         Raises:
-            CommandFormatError
-            CommandExecuteError
+            CommandError
         """
         if self.allow_turn_off is False:
             return
 
         await self.async_run_action(ActionKey.TURN_OFF)
```

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/collection.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/collection.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/command.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from dataclasses import KW_ONLY, dataclass, field
 from string import Formatter
 from typing import TYPE_CHECKING
 
-from .errors import CommandExecuteError, CommandFormatError
+from .errors import CommandError
 from .helpers import name_to_key
 from .sensor import Sensor
 
 if TYPE_CHECKING:
     from .manager import CommandOutput, Manager
 
 SENSOR_PLACEHOLDER_KEY = "_"
@@ -25,81 +25,82 @@
     renderer: Callable[[str], str] | None = None
 
     @property
     def field_keys(self) -> list[str]:
         """Field keys."""
         return {key for _, key, _, _ in Formatter().parse(self.string) if key}
 
+    def _render(self, string: str) -> str:
+        if self.renderer:
+            return self.renderer(string)
+
+        return string
+
     def get_context_keys(self, manager: Manager) -> set[str]:
         """Get context keys."""
         return {key for key in self.field_keys if key not in manager.sensors_by_key}
 
     def get_sensor_keys(self, manager: Manager) -> set[str]:
         """Get sensor keys."""
         return {key for key in self.field_keys if key in manager.sensors_by_key}
 
     async def async_format(self, manager: Manager, context: dict | None = None) -> str:
         """Format the string.
 
         Raises:
-            CommandFormatError
+            CommandError
         """
-        context = context or {}
-        sensor_keys = set()
+        context = {**context} if context else {}
+        missing_sensor_keys = set()
 
         for key in self.get_context_keys(manager):
             if key not in context:
-                raise CommandFormatError(f"Context key {key} is missing")
+                raise CommandError(f"Context key {key} is missing")
 
         for key in self.get_sensor_keys(manager):
             if key not in context:
                 sensor = manager.get_sensor(key)
-                if sensor.value is None:
-                    sensor_keys.add(key)
+                if sensor.value is not None:
+                    context[sensor.key] = sensor.value
                 else:
-                    context[key] = sensor.value
+                    missing_sensor_keys.add(sensor.key)
 
-        for sensor in await manager.async_poll_sensors(sensor_keys):
-            if sensor.value is None:
-                raise CommandFormatError(f"Value of sensor {sensor.key} is None")
-            context[sensor.key] = sensor.value
-
-        string = self.string.format(**context)
-
-        if self.renderer:
-            try:
-                string = self.renderer(string)
-            except Exception as exc:
-                raise CommandFormatError("Can't render command") from exc
+        for sensor in await manager.async_poll_sensors(missing_sensor_keys):
+            if sensor.value is not None:
+                context[sensor.key] = sensor.value
+            else:
+                raise CommandError(f"Value of sensor {sensor.key} is None")
 
-        return string
+        try:
+            return self._render(self.string.format(**context))
+        except Exception as exc:
+            raise CommandError("Failed to generate string ({exc})") from exc
 
     async def async_execute(
         self, manager: Manager, context: dict | None = None
     ) -> CommandOutput:
         """Execute.
 
         Raises:
-            CommandFormatError
-            CommandExecuteError
+            CommandError
         """
         try:
             string = await self.async_format(manager, context)
-        except CommandFormatError as exc:
-            manager.logger.info("%s: %s -> %s", manager.name, self.string, exc)
+        except CommandError as exc:
+            manager.logger.debug("%s: %s => %s", manager.name, self.string, exc)
             raise
 
         try:
             output = await manager.async_execute_command_string(string, self.timeout)
-        except CommandExecuteError as exc:
-            manager.logger.info("%s: %s -> %s", manager.name, string, exc)
+        except CommandError as exc:
+            manager.logger.debug("%s: %s => %s", manager.name, string, exc)
             raise
 
-        manager.logger.info(
-            "%s: %s -> %s, %s, %s",
+        manager.logger.debug(
+            "%s: %s => %s, %s, %s",
             manager.name,
             string,
             output.stdout,
             output.stderr,
             output.code,
         )
 
@@ -109,15 +110,15 @@
 @dataclass
 class ActionCommand(Command):
     """The ActionCommand class."""
 
     name: str | None = None
     key: str | None = None
     _: KW_ONLY
-    options: dict = field(default_factory=dict)
+    attributes: dict = field(default_factory=dict)
 
     def __post_init__(self):
         self.key = self.key or name_to_key(self.name)
 
 
 @dataclass
 class SensorCommand(Command):
@@ -136,51 +137,40 @@
         return {
             sensor.key: sensor
             for command_sensor in self.sensors
             for sensor in (command_sensor, *command_sensor.child_sensors)
             if command_sensor.key != SENSOR_PLACEHOLDER_KEY
         }
 
-    @property
-    def dynamic_sensor(self) -> Sensor | None:
-        return next(
-            (sensor for sensor in self.sensors if sensor.is_dynamic),
-            None,
-        )
-
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor."""
         self.sensors = [
             Sensor(key=SENSOR_PLACEHOLDER_KEY) if sensor.key == key else sensor
             for sensor in self.sensors
         ]
 
-    def update_sensors(self, output: CommandOutput | None) -> None:
+    def update_sensors(self, manager: Manager, output: CommandOutput | None) -> None:
         """Update sensors."""
         if output and output.code == 0:
             self.last_update = output.timestamp
             data = output.stdout
         else:
-            data = None
-
-        if dynamic_sensor := self.dynamic_sensor:
-            dynamic_sensor.update(data)
-            return
-
-        if data is None:
             data = []
 
         for i, sensor in enumerate(self.sensors):
-            sensor.update(data[i] if len(data) > i else None)
+            if sensor.dynamic:
+                sensor.update(manager, data[i:] or None)
+                return
+            sensor.update(manager, data[i] if len(data) > i else None)
 
     async def async_execute(
         self, manager: Manager, context: dict | None = None
     ) -> CommandOutput:
         try:
             output = await super().async_execute(manager, context)
-        except (CommandFormatError, CommandExecuteError):
-            self.update_sensors(None)
+        except CommandError:
+            self.update_sensors(manager, None)
             raise
 
-        self.update_sensors(output)
+        self.update_sensors(manager, output)
 
         return output
```

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/const.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/linux.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/windows_cmd.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/default_collections/windows_ps.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/event.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/manager.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Sequence
 from dataclasses import dataclass
 import logging
 from typing import Any
 
 from .collection import Collection
 from .command import Command
-from .errors import CommandExecuteError, CommandFormatError
+from .errors import CommandError
 from .locker import Locker
 from .sensor import Sensor
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_NAME = "Manager"
 DEFAULT_COMMAND_TIMEOUT = 15
@@ -49,106 +49,100 @@
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         """Execute a command string.
 
         Raises:
-            CommandExecuteError
+            CommandError
         """
-        raise CommandExecuteError("Not implemented")
+        raise CommandError("Not implemented")
 
     async def async_execute_command(
         self, command: Command, context: dict | None = None
     ) -> CommandOutput:
         """Execute a command.
 
         Raises:
-            CommandFormatError
-            CommandExecuteError
+            CommandError
         """
         await command.async_execute(self, context)
 
     async def async_run_action(
         self, key: str, context: dict | None = None
     ) -> CommandOutput:
         """Run an action.
 
         Raises:
-            CommandFormatError
-            CommandExecuteError
+            CommandError
         """
         command = self.get_action_command(key)
         return await self.async_execute_command(command, context)
 
     async def async_poll_sensor(
         self, key: str, *, raise_errors: bool = False
     ) -> Sensor:
         """Poll a sensor.
 
         Raises:
-            CommandFormatError (`raise_errors`)
-            CommandExecuteError (`raise_errors`)
+            CommandError (`raise_errors`)
         """
         sensors = await self.async_poll_sensors([key], raise_errors=raise_errors)
         return sensors[0]
 
     async def async_poll_sensors(
         self, keys: Sequence[str], *, raise_errors: bool = False
     ) -> list[Sensor]:
         """Poll multiple sensors.
 
         Raises:
-            CommandFormatError (`raise_errors`)
-            CommandExecuteError (`raise_errors`)
+            CommandError (`raise_errors`)
         """
         sensors = [self.get_sensor(key) for key in keys]
         commands = [self.get_sensor_command(key) for key in set(keys)]
 
         for command in commands:
             try:
                 await self.async_execute_command(command)
-            except (CommandFormatError, CommandExecuteError):
+            except CommandError:
                 if raise_errors:
                     raise
 
         return sensors
 
     async def async_set_sensor_value(
         self, key: str, value: Any, *, raise_errors: bool = False
     ) -> Sensor:
         """Set the value of a sensor.
 
         Raises:
             TypeError (`raise_errors`)
             ValueError (`raise_errors`)
-            CommandFormatError (`raise_errors`)
-            CommandExecuteError (`raise_errors`)
+            CommandError (`raise_errors`)
         """
         sensors = await self.async_set_sensor_values(
             [key], [value], raise_errors=raise_errors
         )
         return sensors[0]
 
     async def async_set_sensor_values(
         self, keys: Sequence[str], values: Sequence[Any], *, raise_errors: bool = False
     ) -> list[Sensor]:
         """Set the value of multiple sensors.
 
         Raises:
             TypeError (`raise_errors`)
             ValueError (`raise_errors`)
-            CommandFormatError (`raise_errors`)
-            CommandExecuteError (`raise_errors`)
+            CommandError (`raise_errors`)
         """
         sensors = await self.async_poll_sensors(keys, raise_errors=raise_errors)
 
         for i, sensor in enumerate(sensors):
             if sensor.value is None:
                 continue
             try:
                 await sensor.async_set(self, values[i])
-            except (TypeError, ValueError, CommandFormatError, CommandExecuteError):
+            except (TypeError, ValueError, CommandError):
                 if raise_errors:
                     raise
 
         return await self.async_poll_sensors(keys, raise_errors=raise_errors)
```

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.2.1/src/ssh_remote_control/sensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from copy import deepcopy
 from dataclasses import KW_ONLY, dataclass, field
-import logging
 import re
 from typing import TYPE_CHECKING, Any
 
 from .event import Event
 from .helpers import name_to_key
 
 if TYPE_CHECKING:
     from .command import Command
     from .manager import Manager
 
-_LOGGER = logging.getLogger(__name__)
-
 TRUE_STRINGS = ["true", "enabled", "on", "active", "1"]
 FALSE_STRINGS = ["false", "disabled", "off", "inactive", "0"]
 
 
 @dataclass
 class Sensor:
     """The Sensor class."""
 
     name: str | None = None
     key: str | None = None
     _: KW_ONLY
-    dynamic: bool | None = None
+    dynamic: bool = False
     separator: str | None = None
     unit: str | None = None
     renderer: Callable[[str], str] | None = None
     command_set: Command | None = None
-    options: dict = field(default_factory=dict)
+    attributes: dict = field(default_factory=dict)
 
     def __post_init__(self):
         self.id = None
         self.key = self.key or name_to_key(self.name)
         self.value: Any | None = None
         self.last_known_value: Any | None = None
         self.child_sensors: list[Sensor] = []
         self.on_update = Event()
         self.on_child_added = Event()
         self.on_child_removed = Event()
 
     @property
-    def is_dynamic(self) -> bool:
-        """Is dynamic."""
-        return self.dynamic is True
-
-    @property
-    def is_controllable(self) -> bool:
-        """Is controllable."""
+    def controllable(self) -> bool:
+        """Controllable."""
         return self.command_set is not None
 
     @property
     def child_sensors_by_key(self) -> dict[str, Sensor]:
         """Child sensors by key."""
         return {child.key: child for child in self.child_sensors}
 
@@ -72,43 +64,42 @@
 
     def _render(self, value_string: str) -> str:
         if self.renderer:
             return self.renderer(value_string)
 
         return value_string
 
+    def _convert(self, value_string: str) -> Any:
+        return value_string
+
     def _validate(self, value: Any) -> None:
-        if value is None:
-            raise ValueError("Value is None")
+        ...
 
-    def _update_value(self, data: str | None) -> None:
+    def _update_value(self, manager: Manager, data: str | None) -> None:
         if data is None:
+            manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
             self.value = None
             return
 
         try:
-            value = self._render(data)
-        except Exception as exc:  # pylint: disable=broad-except
-            _LOGGER.warning("%s: Render error: %s (%s)", self.key, exc, data)
-            self.value = None
-            return
-
-        try:
+            value_string = self._render(data)
+            value = self._convert(value_string)
             self._validate(value)
-        except (TypeError, ValueError) as exc:
-            _LOGGER.warning("%s: Validate error: %s (%s)", self.key, exc, value)
+        except Exception as exc:  # pylint: disable=broad-except
+            manager.logger.warning("%s: %s => %s", manager.name, self.key, exc)
             self.value = None
             return
 
         self.value = self.last_known_value = value
+        manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
 
-    def _update_child_sensors(self, data: list[str] | None) -> None:
+    def _update_child_sensors(self, manager: Manager, data: list[str] | None) -> None:
         if data is None:
             for child in self.child_sensors:
-                child.update(None)
+                child.update(manager, None)
             return
 
         dynamic_data_list = [
             DynamicData(self.name, self.key, *(field.strip() for field in row))
             for row in (line.split(self.separator, 2) for line in data)
             if len(row) >= 2
         ]
@@ -125,37 +116,36 @@
                 child.name = dynamic_data.name
                 child.dynamic = False
                 self._add_child(child)
 
         for child in self.child_sensors:
             if child.key in dynamic_data_by_key:
                 dynamic_data = dynamic_data_by_key[child.key]
-                child.update(dynamic_data.value_string)
+                child.update(manager, dynamic_data.value_string)
             else:
                 self._remove_child(child)
 
-    def update(self, data: Any) -> None:
+    def update(self, manager: Manager, data: Any) -> None:
         """Update and notify `on_update` subscribers."""
-        if self.is_dynamic:
+        if self.dynamic:
             self.value = self.last_known_value = None
-            self._update_child_sensors(data)
+            self._update_child_sensors(manager, data)
         else:
             self.child_sensors = []
-            self._update_value(data)
+            self._update_value(manager, data)
 
         self.on_update.notify(self)
 
     async def async_set(self, manager: Manager, value: Any) -> None:
         """Set.
 
         Raises:
             TypeError
             ValueError
-            CommandFormatError
-            CommandExecuteError
+            CommandError
         """
         self._validate(value)
         command = self._get_control_command(value)
 
         if command is None or value == self.value:
             return
 
@@ -168,85 +158,89 @@
 class TextSensor(Sensor):
     """The TextSensor class."""
 
     _: KW_ONLY
     minimum: int | None = None
     maximum: int | None = None
     pattern: str | None = None
+    options: list[Any] | None = None
 
     def _validate(self, value: Any) -> None:
-        super()._validate(value)
-
         if not isinstance(value, str):
-            raise TypeError(f"Value is {type(value)} and not {str}")
+            raise TypeError(f"{value} is {type(value)} and not {str}")
 
         if self.minimum and len(value) < self.minimum:
-            raise ValueError(f"Value is shorter then {self.minimum}")
+            raise ValueError(f"{value} is shorter then {self.minimum}")
 
         if self.maximum and len(value) > self.maximum:
-            raise ValueError(f"Value is longer then {self.maximum}")
+            raise ValueError(f"{value} is longer then {self.maximum}")
 
         if self.pattern and not re.fullmatch(self.pattern, value):
-            raise ValueError(f"Value doesn't match {self.pattern}")
+            raise ValueError(f"{value} doesn't match {self.pattern}")
+
+        if self.options and value not in self.options:
+            raise ValueError(f"{value} is not in {self.options}")
 
 
 @dataclass
 class NumberSensor(Sensor):
     """The NumberSensor class."""
 
     _: KW_ONLY
-    minimum: float | None = None
-    maximum: float | None = None
+    integer: bool = False
+    minimum: int | float | None = None
+    maximum: int | float | None = None
+
+    def _convert(self, value_string: str) -> int | float:
+        if self.integer:
+            return int(float(value_string))
 
-    def _render(self, value_string: str) -> float:
-        value_string = super()._render(value_string)
         return float(value_string)
 
     def _validate(self, value: Any) -> None:
-        super()._validate(value)
+        if self.integer and not isinstance(value, int):
+            raise TypeError(f"{value} is {type(value)} and not {int}")
 
-        if not isinstance(value, float):
-            raise TypeError(f"Value is {type(value)} and not {float}")
+        if not self.integer and not isinstance(value, float):
+            raise TypeError(f"{value} is {type(value)} and not {float}")
 
         if self.minimum and value < self.minimum:
-            raise ValueError(f"Value is smaller then {self.minimum}")
+            raise ValueError(f"{value} is smaller then {self.minimum}")
 
         if self.maximum and value > self.maximum:
-            raise ValueError(f"Value is bigger then {self.maximum}")
+            raise ValueError(f"{value} is bigger then {self.maximum}")
 
 
 @dataclass
 class BinarySensor(Sensor):
     """The BinarySensor class."""
 
     _: KW_ONLY
     command_on: Command | None = None
     command_off: Command | None = None
     payload_on: str | None = None
     payload_off: str | None = None
 
     @property
-    def is_controllable(self) -> bool:
+    def controllable(self) -> bool:
         if self.command_on and self.command_off:
             return True
 
         return self.command_set is not None
 
     def _get_control_command(self, value: Any) -> Command | None:
         if self.command_on and value is True:
             return self.command_on
 
         if self.command_off and value is False:
             return self.command_off
 
         return self.command_set
 
-    def _render(self, value_string: str) -> bool:
-        value_string = super()._render(value_string)
-
+    def _convert(self, value_string: str) -> bool:
         if self.payload_on:
             if value_string == self.payload_on:
                 return True
             if not self.payload_off:
                 return False
 
         if self.payload_off:
@@ -257,21 +251,19 @@
 
         if value_string.lower() in TRUE_STRINGS:
             return True
 
         if value_string.lower() in FALSE_STRINGS:
             return False
 
-        raise ValueError("Can't generate boolean from string")
+        raise ValueError("Can't generate bool from {value_string}")
 
     def _validate(self, value: Any) -> None:
-        super()._validate(value)
-
         if not isinstance(value, bool):
-            raise TypeError(f"Value is {type(value)} and not {bool}")
+            raise TypeError(f"{value} is {type(value)} and not {bool}")
 
 
 class DynamicData:
     """The DynamicData class."""
 
     def __init__(
         self,
```

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-remote-control
-Version: 0.2.0
+Version: 0.2.1
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.2.0/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.2.1/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

