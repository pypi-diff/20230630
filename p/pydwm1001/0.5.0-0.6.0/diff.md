# Comparing `tmp/pydwm1001-0.5.0.tar.gz` & `tmp/pydwm1001-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwm1001-0.5.0.tar", last modified: Thu Jun 29 23:57:22 2023, max compression
+gzip compressed data, was "pydwm1001-0.6.0.tar", last modified: Fri Jun 30 00:07:25 2023, max compression
```

## Comparing `pydwm1001-0.5.0.tar` & `pydwm1001-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-29 23:57:22.425969 pydwm1001-0.5.0/
--rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.5.0/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-29 23:57:22.425827 pydwm1001-0.5.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.5.0/README.md
--rw-r--r--   0 adam       (501) staff       (20)     4869 2023-06-29 23:55:35.000000 pydwm1001-0.5.0/dwm1001.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-29 23:57:22.425286 pydwm1001-0.5.0/pydwm1001.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-29 23:57:22.000000 pydwm1001-0.5.0/pydwm1001.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      229 2023-06-29 23:57:22.000000 pydwm1001-0.5.0/pydwm1001.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-29 23:57:22.000000 pydwm1001-0.5.0/pydwm1001.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2023-06-29 23:57:22.000000 pydwm1001-0.5.0/pydwm1001.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        8 2023-06-29 23:57:22.000000 pydwm1001-0.5.0/pydwm1001.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      640 2023-06-29 23:55:35.000000 pydwm1001-0.5.0/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-29 23:57:22.426009 pydwm1001-0.5.0/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-29 23:57:22.425462 pydwm1001-0.5.0/tests/
--rw-r--r--   0 adam       (501) staff       (20)     2782 2023-06-29 00:33:31.000000 pydwm1001-0.5.0/tests/test_dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:07:25.637481 pydwm1001-0.6.0/
+-rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.6.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:07:25.637357 pydwm1001-0.6.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.6.0/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     4485 2023-06-30 00:05:33.000000 pydwm1001-0.6.0/dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:07:25.636868 pydwm1001-0.6.0/pydwm1001.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      229 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      640 2023-06-30 00:05:33.000000 pydwm1001-0.6.0/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-30 00:07:25.637524 pydwm1001-0.6.0/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:07:25.637021 pydwm1001-0.6.0/tests/
+-rw-r--r--   0 adam       (501) staff       (20)     2782 2023-06-29 00:33:31.000000 pydwm1001-0.6.0/tests/test_dwm1001.py
```

### Comparing `pydwm1001-0.5.0/LICENSE` & `pydwm1001-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwm1001-0.5.0/PKG-INFO` & `pydwm1001-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.5.0/dwm1001.py` & `pydwm1001-0.6.0/dwm1001.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,33 +94,33 @@
         # If you quit shell mode (with `quit` command) without stopping
         # a running command, the command will automatically continue
         # when re-entering shell mode. This can be confusing, so we
         # reset the device instead to ensure previously-running commands
         # terminate.
         self.reset()
 
-
-class PassiveTag(UartDwm1001):
-    def __init__(self, serial_handle: Serial) -> None:
-        super().__init__(serial_handle)
-
-        # Device may not have shutdown properly previously
-        self.reset()
-        self.enter_shell_mode()
-
     def start_position_reporting(self) -> None:
         self.send_shell_command(ShellCommand.LEP)
 
         # The first line after invoking the command will have part of
         # the shell prompt mixed in, which would mess up parsing.
         self.serial_handle.reset_input_buffer()
 
     def stop_position_reporting(self) -> None:
         self.send_shell_command(ShellCommand.ENTER)
 
+
+class PassiveTag(UartDwm1001):
+    def __init__(self, serial_handle: Serial) -> None:
+        super().__init__(serial_handle)
+
+        # Device may not have shutdown properly previously
+        self.reset()
+        self.enter_shell_mode()
+
     def wait_for_position_report(self) -> Tuple[TagId, TagPosition]:
         report = self.serial_handle.readline().decode().split(",")
 
         if len(report) != 8:
             raise ParsingError("Position report has unexpected length.")
 
         if report[0] != "POS":
@@ -136,24 +136,14 @@
     def __init__(self, serial_handle) -> None:
         self.serial_handle = serial_handle
 
         # Device may not have shutdown properly previously
         self.reset()
         self.enter_shell_mode()
 
-    def start_position_reporting(self) -> None:
-        self.send_shell_command(ShellCommand.LEP)
-
-        # The first line after invoking the command will have part of
-        # the shell prompt mixed in, which would mess up parsing.
-        self.serial_handle.reset_input_buffer()
-
-    def stop_position_reporting(self) -> None:
-        self.send_shell_command(ShellCommand.ENTER)
-
     @property
     def position(self) -> TagPosition:
         report = self.serial_handle.readline().decode().split(",")
 
         if len(report) != 5:
             raise ParsingError("Position report has unexpected length.")
```

### Comparing `pydwm1001-0.5.0/pydwm1001.egg-info/PKG-INFO` & `pydwm1001-0.6.0/pydwm1001.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.5.0/pyproject.toml` & `pydwm1001-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydwm1001"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Adam Morrissett", email="morrissettal2@vcu.edu" },
 ]
 description = "A Python library for interfacing with DWM1001"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pydwm1001-0.5.0/tests/test_dwm1001.py` & `pydwm1001-0.6.0/tests/test_dwm1001.py`

 * *Files identical despite different names*

