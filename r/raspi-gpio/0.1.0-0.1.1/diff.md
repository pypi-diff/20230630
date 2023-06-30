# Comparing `tmp/raspi_gpio-0.1.0.tar.gz` & `tmp/raspi_gpio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspi_gpio-0.1.0.tar", max compression
+gzip compressed data, was "raspi_gpio-0.1.1.tar", max compression
```

## Comparing `raspi_gpio-0.1.0.tar` & `raspi_gpio-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-06-30 17:09:43.722802 raspi_gpio-0.1.0/LICENSE
--rw-r--r--   0        0        0       74 2023-06-30 17:09:43.722802 raspi_gpio-0.1.0/README.md
--rw-r--r--   0        0        0      693 2023-06-30 17:09:43.722802 raspi_gpio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1110 2023-06-30 17:09:43.722802 raspi_gpio-0.1.0/raspi_gpio/GPIO.py
--rw-r--r--   0        0        0      113 2023-06-30 17:09:43.722802 raspi_gpio-0.1.0/raspi_gpio/__init__.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 raspi_gpio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/LICENSE
+-rw-r--r--   0        0        0       85 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/README.md
+-rw-r--r--   0        0        0      741 2023-06-30 18:14:37.606896 raspi_gpio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1110 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/raspi_gpio/GPIO.py
+-rw-r--r--   0        0        0      233 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/raspi_gpio/__init__.py
+-rw-r--r--   0        0        0      703 2023-06-30 18:14:16.775162 raspi_gpio-0.1.1/raspi_gpio/spidev.py
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 raspi_gpio-0.1.1/PKG-INFO
```

### Comparing `raspi_gpio-0.1.0/LICENSE` & `raspi_gpio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raspi_gpio-0.1.0/pyproject.toml` & `raspi_gpio-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "raspi-gpio"
-version = "0.1.0"
+version = "0.1.1"
 description = "RPi.GPIO wrapper with mocks for developmennt on any platform"
 authors = ["Mark Parker <mark@parker-programs.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "raspi_gpio"}]
 homepage = "https://pypi.org/project/raspi-gpio/"
 repository = "https://github.com/MarkParker5/raspi-gpio"
 documentation = "https://github.com/MarkParker5/raspi-gpio/blob/main/README.md"
 keywords = ["raspberry-pi", "gpio", "rpi", "rpi-gpio", "RPi.GPIO"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rpi-gpio = {version = "^0.7.1", platform = "linux"}
+spidev = {version = "^3.6", platform = "linux"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `raspi_gpio-0.1.0/raspi_gpio/GPIO.py` & `raspi_gpio-0.1.1/raspi_gpio/GPIO.py`

 * *Files identical despite different names*

