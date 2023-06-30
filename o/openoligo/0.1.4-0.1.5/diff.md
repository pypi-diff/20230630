# Comparing `tmp/openoligo-0.1.4.tar.gz` & `tmp/openoligo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openoligo-0.1.4.tar", max compression
+gzip compressed data, was "openoligo-0.1.5.tar", max compression
```

## Comparing `openoligo-0.1.4.tar` & `openoligo-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-06-20 15:02:43.473844 openoligo-0.1.4/LICENSE
--rw-r--r--   0        0        0      790 2023-06-25 07:46:12.264702 openoligo-0.1.4/README.md
--rw-r--r--   0        0        0      446 2023-06-26 08:40:53.804108 openoligo-0.1.4/openoligo/__init__.py
--rw-r--r--   0        0        0      560 2023-06-29 09:09:57.109970 openoligo-0.1.4/openoligo/hal/__init__.py
--rw-r--r--   0        0        0     3971 2023-06-27 18:50:16.320135 openoligo-0.1.4/openoligo/hal/board.py
--rw-r--r--   0        0        0     3799 2023-06-29 09:09:57.132406 openoligo-0.1.4/openoligo/hal/devices.py
--rw-r--r--   0        0        0     3584 2023-06-29 08:40:46.802559 openoligo-0.1.4/openoligo/hal/gpio.py
--rw-r--r--   0        0        0     4365 2023-06-29 04:58:15.204050 openoligo-0.1.4/openoligo/hal/types.py
--rw-r--r--   0        0        0     4261 2023-06-29 09:09:57.133908 openoligo-0.1.4/openoligo/instrument.py
--rw-r--r--   0        0        0      912 2023-06-29 05:09:56.508723 openoligo-0.1.4/openoligo/log_config.py
--rw-r--r--   0        0        0       52 2023-06-24 07:46:31.998299 openoligo-0.1.4/openoligo/protocols/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-29 09:09:31.145859 openoligo-0.1.4/openoligo/protocols/dna_synthesis.py
--rw-r--r--   0        0        0      632 2023-06-29 09:10:53.278742 openoligo-0.1.4/openoligo/seq.py
--rw-r--r--   0        0        0      157 2023-06-25 07:46:47.338022 openoligo-0.1.4/openoligo/steps/__init__.py
--rw-r--r--   0        0        0     2341 2023-06-28 08:29:24.566340 openoligo-0.1.4/openoligo/steps/flow.py
--rw-r--r--   0        0        0     1292 2023-06-28 14:40:11.940888 openoligo-0.1.4/openoligo/steps/types.py
--rw-r--r--   0        0        0      261 2023-06-26 08:40:53.818037 openoligo-0.1.4/openoligo/utils/__init__.py
--rw-r--r--   0        0        0      628 2023-06-29 09:09:31.128856 openoligo-0.1.4/openoligo/utils/sim.py
--rw-r--r--   0        0        0      402 2023-06-27 11:25:14.508079 openoligo-0.1.4/openoligo/utils/singleton.py
--rw-r--r--   0        0        0     1320 2023-06-28 14:40:37.043551 openoligo-0.1.4/openoligo/utils/wait.py
--rw-r--r--   0        0        0     1263 2023-06-29 09:13:02.930980 openoligo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 openoligo-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 17:13:35.712827 openoligo-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1099 2023-06-30 17:13:35.712827 openoligo-0.1.5/README.md
+-rw-r--r--   0        0        0      433 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/__init__.py
+-rw-r--r--   0        0        0      587 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/__init__.py
+-rw-r--r--   0        0        0     3978 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/board.py
+-rw-r--r--   0        0        0     3564 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/devices.py
+-rw-r--r--   0        0        0     3414 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/gpio.py
+-rw-r--r--   0        0        0     2235 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/platform.py
+-rw-r--r--   0        0        0     3871 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/types.py
+-rw-r--r--   0        0        0     4196 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/instrument.py
+-rw-r--r--   0        0        0      912 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/log_config.py
+-rw-r--r--   0        0        0       52 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/protocols/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/protocols/dna_synthesis.py
+-rw-r--r--   0        0        0     1460 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/seq.py
+-rw-r--r--   0        0        0      157 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/steps/__init__.py
+-rw-r--r--   0        0        0     2341 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/steps/flow.py
+-rw-r--r--   0        0        0     1292 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/steps/types.py
+-rw-r--r--   0        0        0      237 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/utils/__init__.py
+-rw-r--r--   0        0        0      537 2023-06-30 17:13:35.720828 openoligo-0.1.5/openoligo/utils/sim.py
+-rw-r--r--   0        0        0      402 2023-06-30 17:13:35.720828 openoligo-0.1.5/openoligo/utils/singleton.py
+-rw-r--r--   0        0        0      839 2023-06-30 17:13:35.720828 openoligo-0.1.5/openoligo/utils/wait.py
+-rw-r--r--   0        0        0     1373 2023-06-30 17:13:35.720828 openoligo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 openoligo-0.1.5/PKG-INFO
```

### Comparing `openoligo-0.1.4/LICENSE` & `openoligo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.4/openoligo/hal/__init__.py` & `openoligo-0.1.5/openoligo/hal/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 Driver imports for convenience.
 """
 
 from openoligo.hal.board import Pinout
 from openoligo.hal.devices import Switch, Valve
-from openoligo.hal.gpio import is_rpi
+from openoligo.hal.gpio import Platform, __platform__
 from openoligo.hal.types import (
-    Board,
     GpioMode,
     InvalidManifoldSizeError,
     Switchable,
     SwitchingError,
     Valvable,
     ValveState,
     ValveType,
 )
 
 __all__ = [
-    "is_rpi",
+    "__platform__",
+    "Platform",
     "Valve",
     "Switch",
-    "Board",
+    "board",
     "GpioMode",
     "Pinout",
     "InvalidManifoldSizeError",
     "Switchable",
     "SwitchingError",
     "Valvable",
     "ValveState",
```

### Comparing `openoligo-0.1.4/openoligo/hal/board.py` & `openoligo-0.1.5/openoligo/hal/board.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Pins in the Raspberry Pi GPIO header.
 """
 from typing import Dict, TypedDict
 
 from openoligo.hal.devices import Switch, Valve
-from openoligo.hal.types import Board, NoSuchPinInPinout, Switchable, ValveRole
+from openoligo.hal.types import Board, NoSuchPinInPinout, Switchable, ValveRole, board
 from openoligo.utils.singleton import Singleton
 
 
 # Initialize fixed pinout
 class FixedPinoutDict(TypedDict):
     """
     A dictionary of pinout that can not be configured by the library users.
@@ -22,33 +22,33 @@
     sol: Valve
     gas: Valve
     valve_pressure: Switch
     gas_pressure: Switch
 
 
 fixed_pinout: FixedPinoutDict = {
-    "waste": Valve(gpio_pin=Board.P7, role=ValveRole.OUTLET),
-    "waste_rxn": Valve(gpio_pin=Board.P5, role=ValveRole.OUTLET),
-    "prod": Valve(gpio_pin=Board.P8, role=ValveRole.OUTLET),
-    "branch": Valve(gpio_pin=Board.P12, role=ValveRole.BRANCH),
-    "rxn_out": Valve(gpio_pin=Board.P13, role=ValveRole.TRANSIT),
-    "sol": Valve(gpio_pin=Board.P3),
-    "gas": Valve(gpio_pin=Board.P10),
-    "valve_pressure": Switch(gpio_pin=Board.P11),
-    "gas_pressure": Switch(gpio_pin=Board.P29),
+    "waste": Valve(gpio_pin=board.P7, role=ValveRole.OUTLET),
+    "waste_rxn": Valve(gpio_pin=board.P5, role=ValveRole.OUTLET),
+    "prod": Valve(gpio_pin=board.P8, role=ValveRole.OUTLET),
+    "branch": Valve(gpio_pin=board.P12, role=ValveRole.BRANCH),
+    "rxn_out": Valve(gpio_pin=board.P13, role=ValveRole.TRANSIT),
+    "sol": Valve(gpio_pin=board.P3),
+    "gas": Valve(gpio_pin=board.P10),
+    "valve_pressure": Switch(gpio_pin=board.P11),
+    "gas_pressure": Switch(gpio_pin=board.P29),
 }
 
 
 def list_configurable_pins() -> dict[str, Board]:
     """
     Returns a list of all configurable pins.
     These ar all pins in the board that are not part of the fiixed pinout.
     """
     fixed_pins = [sw.gpio_pin for sw in fixed_pinout.values()]  # type: ignore
-    return [pin for pin in Board if pin not in fixed_pins]  # type: ignore
+    return [pin for pin in board if pin not in fixed_pins]  # type: ignore
 
 
 class Pinout(metaclass=Singleton):
     """
     Pinout for the instrument.
     """
```

### Comparing `openoligo-0.1.4/openoligo/hal/devices.py` & `openoligo-0.1.5/openoligo/hal/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Switches can be used to control devices that can be turned on and off.
 """
 import logging
 from dataclasses import dataclass, field
 
 from openoligo.hal.gpio import get_gpio
-from openoligo.hal.types import Board, Switchable, Valvable, ValveRole, ValveState, ValveType
+from openoligo.hal.types import Switchable, Valvable, ValveRole, ValveState, ValveType
 
 
 @dataclass
 class Switch(Switchable):
     """
     A switch that actually controls a GPIO pin on the Raspberry Pi.
 
     Attributes:
         name: Name of the switch.
         gpio_pin: GPIO pin number.
         board: Board object to access the GPIO pins.
     """
 
-    gpio_pin: Board
+    gpio_pin: str
     _state: bool = field(default=False, init=False)
     _switch_count: int = field(default=0, init=False, repr=False)
 
     def __post_init__(self):
         """Initialize the switch."""
         self.controller = get_gpio()
         self.controller.setup_pin(self.gpio_pin)
@@ -45,19 +45,14 @@
             "Switch (%s) set from %s to [bold]%s[/]",
             self.gpio_pin,
             __old_state,
             __new_state,
             extra={"markup": True},
         )
 
-    @property
-    def gpio(self) -> Board:
-        """Get the GPIO pin number."""
-        return self.gpio_pin
-
     def toggle(self):
         """Toggle the state of the switch."""
         self.set(not self._state)
 
     @property
     def value(self) -> bool:
         """
@@ -68,15 +63,15 @@
 
 @dataclass
 class Valve(Valvable):
     """
     A valve that actually controls a GPIO pin on the Raspberry Pi.
     """
 
-    gpio_pin: Board
+    gpio_pin: str
     role: ValveRole = field(default=ValveRole.INLET)
     valve_type: ValveType = field(default=ValveType.NORMALLY_OPEN)
     _switch_count: int = field(init=False, default=0)
     _state: ValveState = field(init=False)
 
     def __post_init__(self):
         """Initialize the valve."""
@@ -116,19 +111,14 @@
             self.gpio_pin,
             __old_state,
             self._state,
             extra={"markup": True},
         )
 
     @property
-    def gpio(self) -> Board:
-        """Get the GPIO pin number."""
-        return self.gpio_pin
-
-    @property
     def value(self) -> bool:
         """Get the current value of the valve."""
         return self._state == ValveState.OPEN_FLOW
 
     @property
     def get_type(self) -> ValveType:
         """Get the type of the valve."""
```

### Comparing `openoligo-0.1.4/openoligo/hal/gpio.py` & `openoligo-0.1.5/openoligo/hal/gpio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 """
 GPIO access abstraction: RPi.GPIO on Raspberry Pi, MockGPIO otherwise.
 """
 import importlib
 import logging
 from abc import ABC, abstractmethod
 
-from openoligo.hal.types import Board, GpioMode, is_rpi
+from openoligo.hal.platform import Platform, __platform__
+from openoligo.hal.types import GpioMode, board
 
 
 def get_gpio():
     """Get the GPIO module."""
-    try:
-        with open("/proc/cpuinfo", "r", encoding="utf-8") as file:
-            if "Raspberry" in file.read():
-                gpio = importlib.import_module("RPi.GPIO")
-                return RPiGPIO(gpio)
-            return MockGPIO()
-    except (FileNotFoundError, ModuleNotFoundError):
+    if __platform__ == Platform.BB:
         return MockGPIO()
+    if __platform__ == Platform.RPI:
+        gpio = importlib.import_module("RPi.GPIO")
+        return RPiGPIO(gpio)
+    return MockGPIO()
 
 
 class GPIOInterface(ABC):
     """GPIO interface."""
 
     @abstractmethod
-    def setup(self) -> None:
-        """Setup GPIO."""
-
-    @abstractmethod
-    def setup_pin(self, pin: Board, mode: GpioMode) -> None:
+    def setup_pin(self, pin: str, mode: GpioMode) -> None:
         """Set up a GPIO pin."""
 
     @abstractmethod
-    def set(self, pin: Board, value: bool) -> None:
+    def set(self, pin: str, value: bool) -> None:
         """Set the output value of a GPIO pin."""
         logging.debug("Setting pin %s to %s", pin, value)
 
     @abstractmethod
-    def value(self, pin: Board) -> bool:
+    def value(self, pin: str) -> bool:
         """Get the value of a GPIO pin."""
 
     @abstractmethod
     def cleanup(self) -> None:
         """Clean up GPIO."""
 
     @abstractmethod
@@ -49,76 +44,74 @@
         """Return a string representation of the GPIO module."""
 
 
 class RPiGPIO(GPIOInterface):
     """GPIO access on Raspberry Pi."""
 
     def __init__(self, gpio):
-        """Import Board.GPIO"""
+        """Import RPi.GPIO"""
         self.gpio = gpio
-        self.gpio.setmode(self.gpio.BOARD)
+        self.gpio.setmode(self.gpio.BCM)
         self.gpio.setwarnings(False)
 
-    def setup(self):
-        """Set up all pins."""
-        for pin in Board:
-            self.setup_pin(pin)
-
-    def setup_pin(self, pin: Board, mode: GpioMode = GpioMode.OUT) -> None:
+    def setup_pin(self, pin: str, mode: GpioMode = GpioMode.OUT) -> None:
         """Set up a GPIO pin."""
-        self.gpio.setup(pin.value, self.gpio.OUT if mode == GpioMode.OUT else self.gpio.IN)
+        self.gpio.setup(pin, self.gpio.OUT if mode == GpioMode.OUT else self.gpio.IN)
 
-    def set(self, pin: Board, value: bool) -> None:
+    def set(self, pin: str, value: bool) -> None:
         """Set the output value of a GPIO pin."""
         super().set(pin, value)
-        self.gpio.output(pin.value, self.gpio.HIGH if value else self.gpio.LOW)
+        self.gpio.output(int(pin), self.gpio.HIGH if value else self.gpio.LOW)
 
-    def value(self, pin: Board) -> bool:
-        return self.gpio.input(pin.value)
+    def value(self, pin: str) -> bool:
+        return self.gpio.input(pin)
 
     def cleanup(self):
         """Clean up GPIO."""
         self.gpio.cleanup()
 
     def __repr__(self) -> str:
         """Return a string representation of the GPIO module."""
-        return ", ".join(f"({pin.value}, {1 if self.value(pin) else 0})" for pin in Board)
+        return ", ".join(f"({pin}, {1 if self.value(pin) else 0})" for pin, _ in board)
 
 
 class MockGPIO(GPIOInterface):
     """Mock GPIO access."""
 
     def __init__(self):
         """
         Initialize the state. Its keys are the pin numbers,
         and the values are their mock states
         """
-        self.state: dict[int, bool] = {}
-
-    def setup(self) -> None:
-        """Setup all pins."""
-        for pin in Board:
-            self.setup_pin(pin)
+        self.state: dict[str, bool] = {}
+        for pin, _ in board:
+            self.state[pin] = False
 
     def setup_pin(
-        self, pin: Board, mode: GpioMode = GpioMode.OUT
+        self, pin: str, _: GpioMode = GpioMode.OUT
     ) -> None:  # pylint: disable=unused-argument
         """Set up a GPIO pin."""
-        self.state[pin.value] = False
+        self.state[pin] = False
 
-    def set(self, pin: Board, value: bool):
+    def set(self, pin: str, value: bool) -> None:
         """Set the output value of a GPIO pin."""
-        super().set(pin, value)
-        self.state[pin.value] = value
+        # super().set(pin, value)
+        if pin.startswith("P"):
+            self.state[pin] = value
+        else:
+            self.state[f"P{pin}"] = value
 
-    def value(self, pin: Board) -> bool:
+    def value(self, pin: str) -> bool:
         """Get the value of a GPIO pin."""
-        return self.state[pin.value]
+        if pin.startswith("P"):
+            return self.state[pin]
+        return self.state[f"P{pin}"]
 
     def cleanup(self):
         """Clean up GPIO."""
-        for pin in Board:
+        for pin, _ in board:
             self.set(pin, False)
 
     def __repr__(self) -> str:
         """Return a string representation of the GPIO module."""
-        return ", ".join(f"({pin.value}, {1 if self.value(pin) else 0})" for pin in Board)
+        # return ", ".join(f"({pin}, {self.value(pin)})" for pin, _ in board)
+        return self.state.__repr__()
```

### Comparing `openoligo-0.1.4/openoligo/hal/types.py` & `openoligo-0.1.5/openoligo/hal/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,56 @@
 """
 This module contains definitions of protocols and exceptions related to switchable devices.
 """
 from enum import Enum
-from typing import Protocol
+from typing import Iterator, Protocol
 
+from openoligo.hal.platform import (
+    PLATFORM_TO_BOARD,
+    MinimumCommonPinout,
+    Platform,
+    __platform__,
+    rpi_board_pins,
+)
 
-def is_rpi() -> bool:
-    """Returns True if running on a Raspberry Pi, False otherwise."""
-    try:
-        with open("/proc/cpuinfo", "r", encoding="utf-8") as file:
-            return "Raspberry" in file.read()
-    except FileNotFoundError:
-        return False
 
+class Board:
+    """
+    Represents a board with a minimum common pinout.
+    """
 
-def is_bb() -> bool:
-    """Returns True if running on a Raspberry Pi, False otherwise."""
-    try:
-        with open("/proc/cpuinfo", "r", encoding="utf-8") as file:
-            return "AM33XX" in file.read()
-    except FileNotFoundError:
-        return False
-
-
-class Platform(Enum):
-    """Platform type."""
-
-    RPI = "RPI"
-    BB = "BB"
-    SIM = "SIM"
-
+    board_dict: MinimumCommonPinout
 
-def get_platform() -> Platform:
-    """Get the platform type."""
-    if is_rpi():
-        return Platform.RPI
-    if is_bb():
-        return Platform.BB
-    return Platform.SIM
+    def __init__(self, platform: Platform) -> None:
+        """Creates a board given a particular platform."""
+        self.board_dict = PLATFORM_TO_BOARD.get(platform, rpi_board_pins)
 
+    def __getattr__(self, name: str) -> str:
+        """Return the pin number (as a string) for a given pin name."""
+        if name.startswith("P"):
+            try:
+                return self.board_dict[name]
+            except KeyError as exc:
+                raise AttributeError(f"{self.__class__.__name__} has no pin {name}") from exc
+        raise AttributeError(f"{self.__class__.__name__} has no attribute {name}")
 
-class RPiBoard(Enum):
-    """
-    Enumerates the GPIO pins on the Raspberry Pi 3 Model B.
-    """
+    def __len__(self) -> int:
+        """Return the number of pins on the board."""
+        return len(self.board_dict)
 
-    P3 = 3
-    P5 = 5
-    P7 = 7
-    P8 = 8
-    P10 = 10
-    P11 = 11
-    P12 = 12
-    P13 = 13
-    P15 = 15
-    P16 = 16
-    P18 = 18
-    P19 = 19
-    P21 = 21
-    P22 = 22
-    P23 = 23
-    P24 = 24
-    P26 = 26
-    P27 = 27
-    P28 = 28
-    P29 = 29
-    P31 = 31
-    P32 = 32
-    P33 = 33
-    P35 = 35
-    P36 = 36
-    P37 = 37
-    P38 = 38
-    P40 = 40
+    def __repr__(self) -> str:
+        """Return a string representation of the board."""
+        return f"{self.__class__.__name__}({self.board_dict})"
 
+    def __iter__(self) -> Iterator[tuple[str, str]]:
+        """Return an iterator over the pin names."""
+        return iter(self.board_dict.items())
 
-class BbBoard(Enum):
-    """
-    Enumerates the GPIO pins on the Beaglebone Black.
-    """
 
-    P3 = 3
-    P5 = 5
-    P7 = 7
-    P8 = 8
-    P10 = 10
-    P11 = 11
-    P12 = 12
-    P13 = 13
-    P15 = 15
-    P16 = 16
-    P18 = 18
-    P19 = 19
-    P21 = 21
-    P22 = 22
-    P23 = 23
-    P24 = 24
-    P26 = 26
-    P27 = 27
-    P28 = 28
-    P29 = 29
-    P31 = 31
-    P32 = 32
-    P33 = 33
-    P35 = 35
-    P36 = 36
-    P37 = 37
-    P38 = 38
-    P40 = 40
-
-
-__platform__ = get_platform()
-
-
-if __platform__ == Platform.BB:
-    Board = BbBoard
-else:
-    Board = RPiBoard  # Also acts as a mock board
+board = Board(__platform__)
 
 
 class GpioMode(Enum):
     """GPIO mode."""
 
     IN = 0
     OUT = 1
@@ -159,18 +89,18 @@
         """Initialize the switchable device."""
         raise NotImplementedError
 
     def set(self, state: bool):
         """Set the state of the switch."""
         raise NotImplementedError
 
-    @property
-    def gpio(self) -> Board:
-        """Get the GPIO pin number."""
-        raise NotImplementedError
+    #    @property
+    #    def gpio(self) -> Board:
+    #        """Get the GPIO pin number."""
+    #        raise NotImplementedError
 
     @property
     def value(self) -> bool:
         """Get the current value of the switch."""
         raise NotImplementedError
```

### Comparing `openoligo-0.1.4/openoligo/instrument.py` & `openoligo-0.1.5/openoligo/instrument.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,56 +2,47 @@
 Unified access to configuring and using the instrument.
 """
 import logging
 
 from openoligo.hal.board import Pinout
 from openoligo.hal.devices import Valve
 from openoligo.hal.gpio import get_gpio
-from openoligo.hal.types import Board, OneDestinationException, OneSourceException, ValveRole
+from openoligo.hal.types import OneDestinationException, OneSourceException, ValveRole, board
 from openoligo.utils.singleton import Singleton
 
 default_pinout = Pinout(
     phosphoramidites={
-        "A": Valve(gpio_pin=Board.P26),
-        "C": Valve(gpio_pin=Board.P28),
-        "G": Valve(gpio_pin=Board.P15),
-        "T": Valve(gpio_pin=Board.P16),
+        "A": Valve(gpio_pin=board.P26),
+        "C": Valve(gpio_pin=board.P28),
+        "G": Valve(gpio_pin=board.P15),
+        "T": Valve(gpio_pin=board.P16),
     },
     reactants={
-        "ACT": Valve(gpio_pin=Board.P18),
-        "OXI": Valve(gpio_pin=Board.P19),
-        "CAP1": Valve(gpio_pin=Board.P21),
-        "CAP2": Valve(gpio_pin=Board.P22),
-        "DEB": Valve(gpio_pin=Board.P23),
-        "CLDE": Valve(gpio_pin=Board.P24),
+        "ACT": Valve(gpio_pin=board.P18),
+        "OXI": Valve(gpio_pin=board.P19),
+        "CAP1": Valve(gpio_pin=board.P21),
+        "CAP2": Valve(gpio_pin=board.P22),
+        "DEB": Valve(gpio_pin=board.P23),
+        "CLDE": Valve(gpio_pin=board.P24),
     },
 )
 
 
 class Instrument(metaclass=Singleton):
     """
     Unified access to the instrument. Hide the details of the hardware.
     """
 
     def __init__(self, pinout: Pinout = default_pinout) -> None:
         """
         Initialize the instrument.
         """
         self.pinout = pinout
-
         logging.info("Initializing instrument with pinout: %s", self.pinout)
-
-        self.__setup()
-
-    def __setup(self):
-        """
-        Setup the instrument.
-        """
         self.controller = get_gpio()
-        self.controller.setup()
 
     def __get_valve(self, name: str) -> Valve:
         """
         Get a valve by name.
         """
         valve = self.pinout.get(name)
         if not isinstance(valve, Valve):
@@ -95,15 +86,17 @@
         if len(valve_types[ValveRole.INLET]) != 1:
             raise OneSourceException("There must be exactly one source valve")
 
         if len(valve_types[ValveRole.OUTLET]) != 1:
             raise OneDestinationException("There must be exactly one destination valve")
 
         if len(valve_types[ValveRole.TRANSIT]) > 0:
-            logging.debug("Make sure that the transit valve(s) are in the route you expect")
+            logging.debug(
+                "Make sure that the transit valve(s) are in the route you expect"
+            )  # pragma: no cover
 
     def all_except(self, name: list[str]) -> None:
         """
         Set the state of a pin on the instrument.
 
         Args:
             name: A list of valve names
@@ -125,8 +118,8 @@
             "Set %s to [bold]open[/] and all others to close.", name, extra={"markup": True}
         )
 
     def __repr__(self):
         """
         Return a string representation of the instrument.
         """
-        return f"Instrument({self.pinout})"
+        return f"Instrument({self.pinout})"  # pragma: no cover
```

### Comparing `openoligo-0.1.4/openoligo/log_config.py` & `openoligo-0.1.5/openoligo/log_config.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.4/openoligo/protocols/dna_synthesis.py` & `openoligo-0.1.5/openoligo/protocols/dna_synthesis.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.4/openoligo/steps/flow.py` & `openoligo-0.1.5/openoligo/steps/flow.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.4/openoligo/steps/types.py` & `openoligo-0.1.5/openoligo/steps/types.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.4/openoligo/utils/sim.py` & `openoligo-0.1.5/openoligo/utils/sim.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import logging
 import os
 
 from openoligo.hal.types import Platform, __platform__
 
 # Simulation parameters
 # Can be set using env variable OO_SIM_SPEED=1000
-# SIMULATION_SPEEDUP_FACTOR = 1 if is_rpi() else int(os.environ.get("OO_SIM_SPEED", 1000))
 if os.environ.get("OO_SIM_SPEED") or __platform__ == Platform.SIM:
     SIMULATION_SPEEDUP_FACTOR = int(os.environ.get("OO_SIM_SPEED", 1000))
 else:
     SIMULATION_SPEEDUP_FACTOR = 1
 
 logging.info(
     "Using simulation speedup factor of %d (60min to %.2fs)",
```

### Comparing `openoligo-0.1.4/openoligo/utils/wait.py` & `openoligo-0.1.5/openoligo/utils/wait.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 """
 Utilities for waiting.
 """
 import asyncio
 import logging
 import time
-from typing import Callable
 
 from openoligo.utils.sim import SIMULATION_SPEEDUP_FACTOR
 
 
 async def wait_async(seconds: float) -> None:
     """Wait for a given number of seconds."""
-    logging.debug("Start waiting for %.2f seconds", seconds)
+    logging.debug("Start waiting for %.2f seconds", seconds)  # pragma: no cover
     await asyncio.sleep(seconds / SIMULATION_SPEEDUP_FACTOR)
-    logging.debug("Done waiting for %.2f seconds", seconds)
+    logging.debug("Done waiting for %.2f seconds", seconds)  # pragma: no cover
 
 
 def wait(seconds: float) -> None:
     """Wait for a given number of seconds."""
     logging.debug("Start waiting for %.2f seconds", seconds)
     time.sleep(seconds / SIMULATION_SPEEDUP_FACTOR)
     logging.debug("Done waiting for %.2f seconds", seconds)
 
 
-async def with_wait_async(func: Callable, seconds: float, *args, **kwargs) -> None:
-    """Call a function, then wait for a given number of seconds."""
-    func(*args, **kwargs)
-    await wait_async(seconds / SIMULATION_SPEEDUP_FACTOR)
-
-
-def with_wait(
-    func: Callable, seconds: float, *args, **kwargs
-) -> None:  # pylint: disable=unused-argument
-    """Call a function, then wait for a given number of seconds."""
-    func(*args, **kwargs)
-    wait(seconds / SIMULATION_SPEEDUP_FACTOR)
-
-
 def ms(seconds: float) -> float:  # pylint: disable=invalid-name
     """Convert seconds to milliseconds."""
     return seconds / 1000
```

### Comparing `openoligo-0.1.4/pyproject.toml` & `openoligo-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenOligo"
-version = "0.1.4"
+version = "0.1.5"
 description = "An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes."
 license = "Apache-2.0"
 authors = ["Satyam Tiwary <satyam@technoculture.io>"]
 readme = "README.md"
 keywords = ["DNA", "synthesis", "genetics", "open-source"]
 
 [tool.poetry.scripts]
@@ -14,14 +14,16 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.4.2"
 python-dotenv = "^1.0.0"
 tqdm = "^4.65.0"
 fastapi = "^0.98.0"
 pdocs = "^1.2.0"
+"RPi.GPIO" = { version = "^0.7.1", optional = true }
+Adafruit_BBIO = { version = "^1.2.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 flake8 = "^3.9.2"
 black = "^23.3.0"
 pylint = "^2.17.4"
@@ -43,12 +45,12 @@
 line-length = 100
 
 [tool.pytest.ini_options]
 addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=90"
 
 [tool.coverage.run]
 source = ["openoligo"]
-omit = ["**/types.py"]
+#omit = ["**/types.py"]
 
 [tool.poetry.extras]
 rpi = ["RPi.GPIO"]
 bb = ["Adafruit_BBIO"]
```

### Comparing `openoligo-0.1.4/PKG-INFO` & `openoligo-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: openoligo
-Version: 0.1.4
+Version: 0.1.5
 Summary: An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes.
 License: Apache-2.0
 Keywords: DNA,synthesis,genetics,open-source
 Author: Satyam Tiwary
 Author-email: satyam@technoculture.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: bb
 Provides-Extra: rpi
+Requires-Dist: Adafruit_BBIO (>=1.2.0,<2.0.0) ; extra == "bb"
+Requires-Dist: RPi.GPIO (>=0.7.1,<0.8.0) ; extra == "rpi"
 Requires-Dist: fastapi (>=0.98.0,<0.99.0)
 Requires-Dist: pdocs (>=1.2.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
@@ -34,9 +36,22 @@
 ```sh
 pip install openoligo
 ```
 
 ### A simple Example
 
 ```py
+import asyncio
+
+from openoligo.instrument import Instrument
+from openoligo.protocols.dna_synthesis import synthesize
+from openoligo.seq import Seq
+
+
+inst = Instrument()
+
+try:
+    asyncio.run(synthesize(inst, Seq("ATCGAAATTTTT")))
+except KeyboardInterrupt:
+    print("Keyboard interrupt received, exiting...")
 ```
```

