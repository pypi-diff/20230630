# Comparing `tmp/sinol-make-1.1.0.tar.gz` & `tmp/sinol-make-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.1.0.tar", last modified: Sat Jun 17 09:55:45 2023, max compression
+gzip compressed data, was "sinol-make-1.1.1.tar", last modified: Fri Jun 30 18:25:36 2023, max compression
```

## Comparing `sinol-make-1.1.0.tar` & `sinol-make-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-17 09:55:35.000000 sinol-make-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 09:55:45.885949 sinol-make-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-17 09:55:35.000000 sinol-make-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-17 09:55:35.000000 sinol-make-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 09:55:45.885949 sinol-make-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.881949 sinol-make-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.881949 sinol-make-1.1.0/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.881949 sinol-make-1.1.0/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    29611 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/helpers/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-17 09:55:35.000000 sinol-make-1.1.0/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 09:55:45.000000 sinol-make-1.1.0/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:55:45.885949 sinol-make-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-17 09:55:35.000000 sinol-make-1.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-30 18:25:23.000000 sinol-make-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 18:25:36.438901 sinol-make-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-30 18:25:23.000000 sinol-make-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 18:25:23.000000 sinol-make-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 18:25:36.438901 sinol-make-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.430900 sinol-make-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    36055 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/helpers/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-30 18:25:23.000000 sinol-make-1.1.1/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.434900 sinol-make-1.1.1/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 18:25:36.000000 sinol-make-1.1.1/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:25:36.438901 sinol-make-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-30 18:25:23.000000 sinol-make-1.1.1/tests/test_util.py
```

### Comparing `sinol-make-1.1.0/LICENSE` & `sinol-make-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.0/PKG-INFO` & `sinol-make-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # <img src="https://avatars.githubusercontent.com/u/2264918?s=200&v=4" height=60em> sinol-make
 
 `sinol-make` is a CLI tool for creating and verifying problem packages
```

### Comparing `sinol-make-1.1.0/README.md` & `sinol-make-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.0/pyproject.toml` & `sinol-make-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   { name="Mateusz Masiarz", email="m.masiarz@fri.edu.pl" }
 ]
 maintainers = [
   { name="Tomasz Nowak", email="tomasz.nowak@tonowak.com" }
 ]
 description = "CLI tool for creating sio2 task packages"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
 	"argparse",
```

### Comparing `sinol-make-1.1.0/src/sinol_make/__init__.py` & `sinol-make-1.1.1/src/sinol_make/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 def configure_parsers():
-	parser = argparse.ArgumentParser(
-		prog='sinol-make',
-		description='Tool for creating and testing sio2 tasks',
-	)
-	parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
-	subparsers = parser.add_subparsers(
-		title='commands',
-		description='sinol-make commands',
-		dest='command',
-	)
-	subparsers.required = False
-
-	commands = util.get_commands()
-
-	for command in commands:
-		command.configure_subparser(subparsers)
-	return parser
+    parser = argparse.ArgumentParser(
+        prog='sinol-make',
+        description='Tool for creating and testing sio2 tasks',
+    )
+    parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
+    subparsers = parser.add_subparsers(
+        title='commands',
+        description='sinol-make commands',
+        dest='command',
+    )
+    subparsers.required = False
+
+    commands = util.get_commands()
+
+    for command in commands:
+        command.configure_subparser(subparsers)
+    return parser
 
 
 def main():
-	parser = configure_parsers()
-	commands = util.get_commands()
-	args = parser.parse_args()
-
-	for command in commands:
-		if command.get_name() == args.command:
-			if sys.platform == 'linux' and not util.check_oiejq():
-				print(util.warning('`oiejq` in `~/.local/bin/` not detected, installing now...'))
-
-				try:
-					if util.install_oiejq():
-						print(util.info('`oiejq` was successfully installed.'))
-					else:
-						util.exit_with_error('`oiejq` could not be installed.\n'
-											 'You can download it from https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz'
-											 ', unpack it to `~/.local/bin/` and rename oiejq.sh to oiejq.\n'
-											 'You can also use --oiejq_path to specify path to your oiejq.')
-				except Exception as err:
-					util.exit_with_error('`oiejq` could not be installed.\n' + err)
+    parser = configure_parsers()
+    commands = util.get_commands()
+    args = parser.parse_args()
+
+    for command in commands:
+        if command.get_name() == args.command:
+            if sys.platform == 'linux' and not util.check_oiejq():
+                print(util.warning('`oiejq` in `~/.local/bin/` not detected, installing now...'))
+
+                try:
+                    if util.install_oiejq():
+                        print(util.info('`oiejq` was successfully installed.'))
+                    else:
+                        util.exit_with_error('`oiejq` could not be installed.\n'
+                                             'You can download it from https://oij.edu.pl/zawodnik/srodowisko/oiejq.tar.gz'
+                                             ', unpack it to `~/.local/bin/` and rename oiejq.sh to oiejq.\n'
+                                             'You can also use --oiejq_path to specify path to your oiejq.')
+                except Exception as err:
+                    util.exit_with_error('`oiejq` could not be installed.\n' + err)
 
-			command.run(args)
-			exit(0)
+            command.run(args)
+            exit(0)
 
-	parser.print_help()
+    parser.print_help()
```

### Comparing `sinol-make-1.1.0/src/sinol_make/commands/run/structs.py` & `sinol-make-1.1.1/src/sinol_make/commands/run/structs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from typing import List
 from dataclasses import dataclass
 
 @dataclass
 class ResultChange:
-	solution: str
-	group: int
-	old_result: str
-	result: str
+    solution: str
+    group: int
+    old_result: str
+    result: str
 
 @dataclass
 class ValidationResult:
-	added_solutions: set
-	removed_solutions: set
-	added_groups: set
-	removed_groups: set
-	changes: List[ResultChange]
-	expected_scores: dict
-	new_expected_scores: dict
+    added_solutions: set
+    removed_solutions: set
+    added_groups: set
+    removed_groups: set
+    changes: List[ResultChange]
+    expected_scores: dict
+    new_expected_scores: dict
 
 @dataclass
 class ExecutionResult:
-	# Result status of execution. Can be one of:
-	# "OK", "WA", "TL", "ML", "RE", "CE"
-	Status: str
-	# Time in milliseconds
-	Time: float
-	# Memory in KB
-	Memory: int
+    # Result status of execution. Can be one of:
+    # "OK", "WA", "TL", "ML", "RE", "CE"
+    Status: str
+    # Time in milliseconds
+    Time: float
+    # Memory in KB
+    Memory: int
 
 @dataclass
 class ExecutionData:
-	"""
-	Represents data for execution of a solution on a specified test.
-	"""
-	# Name of the solution
-	name: str
-	# Filename of the executable
-	executable: str
-	# Filename of the test
-	test: str
-	# Time limit for this test in milliseconds
-	time_limit: int
-	# Memory limit in KB
-	memory_limit: int
-	# Path to the timetool executable
-	timetool_path: str
+    """
+    Represents data for execution of a solution on a specified test.
+    """
+    # Name of the solution
+    name: str
+    # Filename of the executable
+    executable: str
+    # Filename of the test
+    test: str
+    # Time limit for this test in milliseconds
+    time_limit: int
+    # Memory limit in KB
+    memory_limit: int
+    # Path to the timetool executable
+    timetool_path: str
```

### Comparing `sinol-make-1.1.0/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.1.1/src/sinol_make.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # <img src="https://avatars.githubusercontent.com/u/2264918?s=200&v=4" height=60em> sinol-make
 
 `sinol-make` is a CLI tool for creating and verifying problem packages
```

### Comparing `sinol-make-1.1.0/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.1.1/src/sinol_make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

