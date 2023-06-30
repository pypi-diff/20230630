# Comparing `tmp/rpi_reactive_gpio-0.1.5.tar.gz` & `tmp/rpi_reactive_gpio-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.5.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.6.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.5.tar` & `rpi_reactive_gpio-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-06-29 15:42:19.679609 rpi_reactive_gpio-0.1.5/LICENSE
--rw-r--r--   0        0        0       80 2023-06-29 15:42:19.679609 rpi_reactive_gpio-0.1.5/README.md
--rw-r--r--   0        0        0      766 2023-06-29 15:42:38.531732 rpi_reactive_gpio-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      207 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3504 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      478 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      850 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1263 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/README.md
+-rw-r--r--   0        0        0      766 2023-06-30 17:51:48.325478 rpi_reactive_gpio-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1607 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3508 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      482 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      850 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1263 2023-06-30 17:51:17.829130 rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.6/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.5/LICENSE` & `rpi_reactive_gpio-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.5/pyproject.toml` & `rpi_reactive_gpio-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.5"
+version = "0.1.6"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
 documentation = "https://github.com/MarkParker5/rpi-reactive-gpio/blob/main/README.md"
 keywords = ["raspberry-pi", "gpio", "reactive", "rxpy", "rx", "rpi", "rpi-gpio", "RPi.GPIO"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-"RPi.GPIO" = "^0.7.1"
+raspi-gpio = "^0.1.0"
 
 [tools.mypy]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/buttons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typing import Callable, Any, TypeVar
 import time
-import RPi.GPIO as GPIO
+from raspi_gpio import GPIO
 from .pin_manager import tickables
 
 
 ButtonCallback = TypeVar('ButtonCallback', bound = Callable[[int], None] | Callable[['ButtonClick', int], None])
     
 class ButtonClick:
```

### Comparing `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/leds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from enum import Enum
 from typing import Callable
-import RPi.GPIO as GPIO
+from raspi_gpio import GPIO
 from .pin_manager import tickables, managers
 
 
 class LedState(Enum):
     off = 0
     on = 1
     blink = 2
```

### Comparing `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/pin_manager.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.6/rpi_reactive_gpio/scene.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.5/PKG-INFO` & `rpi_reactive_gpio-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.5
+Version: 0.1.6
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: RPi.GPIO (>=0.7.1,<0.8.0)
+Requires-Dist: raspi-gpio (>=0.1.0,<0.2.0)
 Project-URL: Documentation, https://github.com/MarkParker5/rpi-reactive-gpio/blob/main/README.md
 Project-URL: Repository, https://github.com/MarkParker5/rpi-reactive-gpio
 Description-Content-Type: text/markdown
 
 # rpi-reactive-gpio
 
 Syntax sugar for controlling RPi.GPIO with reactive design.
```

