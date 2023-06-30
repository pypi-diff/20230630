# Comparing `tmp/typerconf-1.8.tar.gz` & `tmp/typerconf-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-1.8.tar", max compression
+gzip compressed data, was "typerconf-1.9.tar", max compression
```

## Comparing `typerconf-1.8.tar` & `typerconf-1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.8/LICENSE
--rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.8/README.md
--rw-r--r--   0        0        0      934 2023-04-26 12:29:14.870139 typerconf-1.8/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.8/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.8/src/typerconf/Makefile
--rw-r--r--   0        0        0     8204 2023-04-26 12:32:10.814792 typerconf-1.8/src/typerconf/__init__.py
--rw-r--r--   0        0        0    22337 2023-04-26 12:28:13.873901 typerconf-1.8/src/typerconf/init.nw
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.9/LICENSE
+-rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.9/README.md
+-rw-r--r--   0        0        0      934 2023-04-27 11:58:27.492674 typerconf-1.9/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.9/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.9/src/typerconf/Makefile
+-rw-r--r--   0        0        0     8324 2023-04-27 12:06:24.076825 typerconf-1.9/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    22677 2023-04-27 12:05:46.191776 typerconf-1.9/src/typerconf/init.nw
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.9/PKG-INFO
```

### Comparing `typerconf-1.8/LICENSE` & `typerconf-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-1.8/README.md` & `typerconf-1.9/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-1.8/pyproject.toml` & `typerconf-1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "1.8"
+version = "1.9"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-1.8/src/typerconf/__init__.py` & `typerconf-1.9/src/typerconf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,14 +196,16 @@
                  values: typing.List[str] = value_arg):
     """
     Reads values from or writes values to the config.
     """
     if values:
       if len(values) == 1:
         values = values[0]
+      if values == "":
+        values = None
       set(path, values)
     else:
       print_config(get(path), path)
 def get(path: str = "") -> typing.Any:
   """
   Returns the value stored at `path` in the config.
 
@@ -230,17 +232,19 @@
   """
   Returns all valid paths in the config starting with `initial_path`.
   If `conf` is not None, use that instead of the actual config.
   """
   if not conf:
     conf = Config(get())
 
-  return list(filter(lambda x: x.startswith(initial_path),
-                     conf.paths()))
-def complete_path_callback(ctx, param, initial_path: str):
+  return filter(lambda x: x.startswith(initial_path),
+                conf.paths())
+def complete_path_callback(ctx: typer.Context,
+                           args: typing.List[str],
+                           initial_path: str):
   return complete_path(initial_path)
 def print_config(conf, path=""):
   """
   Prints the config tree contained in `conf` to stdout.
   Optional `path` is prepended.
   """
   try:
```

### Comparing `typerconf-1.8/src/typerconf/init.nw` & `typerconf-1.9/src/typerconf/init.nw`

 * *Files 1% similar despite different names*

```diff
@@ -635,27 +635,35 @@
 def config_cmd(path: str = path_arg,
                values: typing.List[str] = value_arg):
   """
   Reads values from or writes values to the config.
   """
   if values:
     <<change [[values]] to non-list if one-element list>>
+    <<if [[values]] is empty string, replace it with [[None]]>>
     set(path, values)
   else:
     print_config(get(path), path)
 @
 
 If the user supplies only one argument on the command line, we don't want it to 
 be interpreted as a one-element list, but rather as a value that is not a list.
 Hence, we check and convert if necessary.
 <<change [[values]] to non-list if one-element list>>=
 if len(values) == 1:
   values = values[0]
 @
 
+Additionally, if that one element is an empty string, we replace it with 
+[[None]] to trigger a delete.
+<<if [[values]] is empty string, replace it with [[None]]>>=
+if values == "":
+  values = None
+@
+
 Let's test this command.
 <<test functions>>=
 runner = CliRunner()
 
 def test_cli():
   # set example data
   result = runner.invoke(cli,
@@ -692,16 +700,16 @@
   """
   Returns all valid paths in the config starting with `initial_path`.
   If `conf` is not None, use that instead of the actual config.
   """
   if not conf:
     conf = Config(get())
 
-  return list(filter(lambda x: x.startswith(initial_path),
-                     conf.paths()))
+  return filter(lambda x: x.startswith(initial_path),
+                conf.paths())
 @
 
 We test this function as follows.
 <<test functions>>=
 def test_complete_path():
   conf = Config({
     "courses": {
@@ -717,15 +725,17 @@
   assert "courses.datintro22.url" not in complete_path(incomplete, conf)
   assert len(complete_path(incomplete, conf)) >= 0
 @
 
 Now, the callback must not have any additional arguments, like we want that 
 [[conf]] argument for testing.
 <<helper functions>>=
-def complete_path_callback(ctx, param, initial_path: str):
+def complete_path_callback(ctx: typer.Context,
+                           args: typing.List[str],
+                           initial_path: str):
   return complete_path(initial_path)
 @
 
 
 \subsection{Printing the config}
 
 That [[print_config]] function should print the remaining levels of the config
```

### Comparing `typerconf-1.8/PKG-INFO` & `typerconf-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 1.8
+Version: 1.9
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
```

