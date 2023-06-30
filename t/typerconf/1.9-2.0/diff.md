# Comparing `tmp/typerconf-1.9.tar.gz` & `tmp/typerconf-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-1.9.tar", max compression
+gzip compressed data, was "typerconf-2.0.tar", max compression
```

## Comparing `typerconf-1.9.tar` & `typerconf-2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.9/LICENSE
--rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.9/README.md
--rw-r--r--   0        0        0      934 2023-04-27 11:58:27.492674 typerconf-1.9/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.9/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.9/src/typerconf/Makefile
--rw-r--r--   0        0        0     8324 2023-04-27 12:06:24.076825 typerconf-1.9/src/typerconf/__init__.py
--rw-r--r--   0        0        0    22677 2023-04-27 12:05:46.191776 typerconf-1.9/src/typerconf/init.nw
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.0/LICENSE
+-rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-2.0/README.md
+-rw-r--r--   0        0        0      934 2023-06-30 11:40:51.751242 typerconf-2.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.0/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.0/src/typerconf/Makefile
+-rw-r--r--   0        0        0    10261 2023-06-30 11:40:04.195065 typerconf-2.0/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    29554 2023-06-30 11:39:40.246977 typerconf-2.0/src/typerconf/init.nw
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-2.0/PKG-INFO
```

### Comparing `typerconf-1.9/LICENSE` & `typerconf-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-1.9/README.md` & `typerconf-2.0/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-1.9/pyproject.toml` & `typerconf-2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "1.9"
+version = "2.0"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-1.9/src/typerconf/__init__.py` & `typerconf-2.0/src/typerconf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,40 @@
 normalized_path = os.path.normpath(sys.argv[0])
 basename = os.path.basename(normalized_path)
 dirs = appdirs.AppDirs(basename)
 
 class Config:
   """Navigates nested JSON structures by dot-separated addressing."""
 
-  def __init__(self, json_data={}):
+  def __init__(self, json_data={},
+                     conf_file=None):
     """
     Constructs a config object to navigate from JSON data `json_data`.
+
+    `conf_file` takes a path to a file which will be used as a config file. If this 
+    argument is supplied, the data will be read from the file.
+
+    Also, if `conf_file` is not None, we will enable automatic write back. So 
+    that any changes (invokations of the `.set` method) will be written to the 
+    config file immediately.
+
+    To not enable write back, load file contents with the `.read_config` method.
     """
     self.__data = json_data
+    if isinstance(conf_file, io.IOBase):
+      try:
+        self.__conf_file = conf_file.name
+      except AttributeError:
+        raise ValueError(f"can't enable writeback when `conf_file` is "
+                         f"a file-like object without a name: {conf_file}")
+    else:
+      self.__conf_file = conf_file
+
+    if self.__conf_file:
+      self.read_config(self.__conf_file)
 
   def get(self, path: str = "") -> typing.Any:
     """
     Returns object at `path`.
     Example:
     - `path = "courses.datintro22.url"` and
     - Config contains `{"courses": {"datintro22": {"url": "https://..."}}}` 
@@ -45,15 +66,14 @@
         pass
       try:
         structure = structure[part]
       except KeyError:
         raise KeyError(f"{part} along {path} doesn't exist")
 
     return structure
-
   def set(self, path: str, value: typing.Any):
     """
     Sets `value` at `path`. Any parts along the path that don't exist will be 
     created.
 
     Example:
     - `value = "https://..."`,
@@ -62,14 +82,17 @@
 
     Any part of the path that can be converted to an integer, will be converted 
     to an integer. This way we can access elements of lists too. However, we 
     cannot create index 3 in a list if it doesn't exist (we can't expand 
     lists).
 
     If `value` is `None`, the entry at `path` will be deleted, if it exists.
+
+    If write back is set (see `.__init__` and `.read_config`), a successful set 
+    will also update the original config file.
     """
     structure = self.__data
 
     parts = path.split(".")
 
     for part in parts[:-1]:
       try:
@@ -94,14 +117,16 @@
     if value is None:
       try:
         del structure[part]
       except KeyError:
         pass
     else:
       structure[part] = value
+    if self.__conf_file:
+      self.write_config(self.__conf_file)
   def paths(self, from_root=""):
     """
     Returns all existing paths.
 
     The optional argument `from_root` is a path and the method return all 
     subpaths rooted at that point.
     """
@@ -117,53 +142,71 @@
 
         paths.append(path)
         paths += self.paths(from_root=path)
     elif isinstance(root, list):
       paths += [f"{from_root}.{x}" for x in range(len(root))]
 
     return paths
-  def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
+  def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json",
+                        writeback=False):
     """
     Reads the config data structure (JSON) into the Config object.
+
     `conf_file` is an optional argument providing one of the following:
     - an already opened file object (anything derived from `io.IOBase`);
     - anything that `open` can handle, for instance:
       - a string, which is the path to the config file;
       - an integer, which is a file descriptor (see `os.open`).
 
+    If `writeback` is set to True, store the `conf_file` object and turn on 
+    automatic write back. This means that any changes using the `.set` method will 
+    cause the config being written back to the file.
+
+    Note that write back cannot be enabled with already opened files (as the mode 
+    is already fixed).
+
     Errors:
 
-    - The first is that the file doesn't exist ([[FileNotFoundError]]). We silently 
+    - The first is that the file doesn't exist (FileNotFoundError). We silently 
       fail this error. The reason is that the file doesn't exist, which means it's 
       an empty config. We fail silently as a later write would succeed.
-    - There is also a related one, [[NotADirectoryError]]. The problem of 
-      [[NotADirectoryError]] occurs when a file on the path is used as a directory 
-      --- but only for reading, when trying to create a directory hierarchy, it 
-      will yield [[FileExistsError]]. We can't recover from this error, as an 
-      attempt to write to the file will also fail. We will reraise the exception 
-      with a better error message.
-    - Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]). 
-      This is also a fatal error, we don't want a subsequent write to overwrite a 
-      corrupted config. We reraise the exception with a better error message.
+    - There is also a related one, NotADirectoryError. The problem of 
+      NotADirectoryError occurs when a file on the path is used as a directory --- 
+      but only for reading, when trying to create a directory hierarchy, it will 
+      yield FileExistsError. We can't recover from this error, as an attempt to 
+      write to the file will also fail. We will reraise the exception with a better 
+      error message.
+    - Finally, the file exists, but it's not proper JSON (JSONDecodeError). This is 
+      also a fatal error, we don't want a subsequent write to overwrite a corrupted 
+      config. We reraise the exception with a better error message.
     """
     if isinstance(conf_file, io.IOBase):
       self.__data = json.load(conf_file)
     else:
       try:
         with open(conf_file) as conf_file:
           self.__data = json.load(conf_file)
-          return
       except FileNotFoundError as err:
         pass
       except NotADirectoryError as err:
         raise NotADirectoryError(f"A part of the path is a file, "
                                  f"but used as directory: {err}")
       except json.decoder.JSONDecodeError as err:
         raise ValueError(f"Config file {conf_file} "
                          f"could not be decoded: {err}")
+
+    if writeback:
+      if isinstance(conf_file, io.IOBase):
+        try:
+          self.__conf_file = conf_file.name
+        except AttributeError:
+          raise ValueError(f"can't enable writeback when `conf_file` is "
+                           f"a file-like object without a name: {conf_file}")
+      else:
+        self.__conf_file = conf_file
   def write_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
     """
     Stores the config data (as JSON) in the config file.
     `conf_file` is an optional argument providing one of the following:
     - an already opened file object (anything derived from `io.IOBase`);
     - anything that `open` can handle, for instance:
       - a string, which is the path to the config file;
@@ -174,22 +217,34 @@
     else:
       conf_dir = os.path.dirname(conf_file)
       if not os.path.isdir(conf_dir):
         os.makedirs(conf_dir)
 
       with open(conf_file, "w") as conf_file:
         json.dump(self.__data, conf_file)
-def add_config_cmd(cli: typer.Typer):
+def add_config_cmd(cli: typer.Typer, conf_path: str = None):
   """
-  Add config command to Typer cli
+  Add config command to Typer instance `cli`.
+
+  If `conf_path` is not None, use that file instead of the default.
   """
-  path_arg = typer.Argument(...,
+  conf = Config()
+  try:
+    if conf_path:
+      conf.read_config(conf_path)
+    else:
+      conf.read_config()
+  except ValueError:
+    pass
+
+  path_arg = typer.Argument("",
                             help="Path in config, e.g. 'courses.datintro22'. "
-                                 "Empty string is root of config.",
-                            shell_complete=complete_path_callback)
+                                 "Empty string is root of config. Defaults to "
+                                 "the empty string.",
+                            autocompletion=complete_path_callback)
   value_arg = typer.Option([], "-s", "--set",
                            help="Values to store. "
                                 "More than one value makes a list. "
                                 "Values are treated as JSON if possible.")
 
   @cli.command(name="config")
   def config_cmd(path: str = path_arg,
@@ -198,17 +253,17 @@
     Reads values from or writes values to the config.
     """
     if values:
       if len(values) == 1:
         values = values[0]
       if values == "":
         values = None
-      set(path, values)
+      conf.set(path, values)
     else:
-      print_config(get(path), path)
+      print_config(conf.get(path), path)
 def get(path: str = "") -> typing.Any:
   """
   Returns the value stored at `path` in the config.
 
   By default, `path = ""`, which returns the entire configuration as a Config 
   object.
   """
@@ -234,17 +289,15 @@
   If `conf` is not None, use that instead of the actual config.
   """
   if not conf:
     conf = Config(get())
 
   return filter(lambda x: x.startswith(initial_path),
                 conf.paths())
-def complete_path_callback(ctx: typer.Context,
-                           args: typing.List[str],
-                           initial_path: str):
+def complete_path_callback(initial_path: str):
   return complete_path(initial_path)
 def print_config(conf, path=""):
   """
   Prints the config tree contained in `conf` to stdout.
   Optional `path` is prepended.
   """
   try:
```

### Comparing `typerconf-1.9/src/typerconf/init.nw` & `typerconf-2.0/src/typerconf/init.nw`

 * *Files 16% similar despite different names*

```diff
@@ -45,17 +45,19 @@
 \begin{minted}{python}
 import typerconf as config
 # ...
 config.add_config_cmd(cli)
 \end{minted}
 So we need to provide such a function.
 <<helper functions>>=
-def add_config_cmd(cli: typer.Typer):
+def add_config_cmd(cli: typer.Typer, conf_path: str = None):
   """
-  Add config command to Typer cli
+  Add config command to Typer instance `cli`.
+
+  If `conf_path` is not None, use that file instead of the default.
   """
   <<config subcommands>>
 @
 
 To make this module runnable on its own (using [[main]]), we will create a 
 [[cli]] object in the [[main]] function, then add the config command and 
 finally run it.
@@ -117,19 +119,23 @@
 This class has two methods that are central:
 The first gets a value out, the other sets a value in.
 Both work with these dot-separated addresses.
 <<classes>>=
 class Config:
   """Navigates nested JSON structures by dot-separated addressing."""
 
-  def __init__(self, json_data={}):
+  def __init__(self, json_data={},
+                     <<Config constructor args>>):
     """
     Constructs a config object to navigate from JSON data `json_data`.
+
+    <<Config constructor args doc>>
     """
     self.__data = json_data
+    <<Config attributes>>
 
   <<Config methods for get and set>>
   <<Config methods for available paths>>
   <<Config methods for reading from and writing to file>>
 @
 
 We will use the following test data for the test functions.
@@ -144,49 +150,39 @@
 }
 conf = Config(test_data)
 @
 
 \subsection{Getting and setting values}
 
 We want to be able to get and set values at different paths in the config.
+We'll provide methods [[.get]] and [[.set]] for this.
+
+\subsubsection{Getting values}
+
+The get method looks like this.
 <<Config methods for get and set>>=
 def get(self, path: str = "") -> typing.Any:
   """
   Returns object at `path`.
   Example:
   - `path = "courses.datintro22.url"` and
   - Config contains `{"courses": {"datintro22": {"url": "https://..."}}}` 
     will return "https://...".
 
   Any part of the path that can be converted to an integer, will be converted 
   to an integer. This way we can access elements of lists too.
   """
   <<get value at path>>
-
-def set(self, path: str, value: typing.Any):
-  """
-  Sets `value` at `path`. Any parts along the path that don't exist will be 
-  created.
-
-  Example:
-  - `value = "https://..."`,
-  - `path = "courses.datintro22.url"`
-  will create `{"courses": {"datintro22": {"url": "https://..."}}}`.
-
-  Any part of the path that can be converted to an integer, will be converted 
-  to an integer. This way we can access elements of lists too. However, we 
-  cannot create index 3 in a list if it doesn't exist (we can't expand 
-  lists).
-
-  If `value` is `None`, the entry at `path` will be deleted, if it exists.
-  """
-  <<set value at path>>
 @
 
-\subsubsection{Getting values}
+We can test this as follows, using the config data defined above.
+<<test functions>>=
+def test_get_path():
+  assert conf.get("courses.datintro22.url") == "https://..."
+@
 
 To get the value, we simply walk along the path and returns what remains.
 <<get value at path>>=
 structure = self.__data
 
 if not path:
   return structure
@@ -197,20 +193,14 @@
     structure = structure[part]
   except KeyError:
     raise KeyError(f"{part} along {path} doesn't exist")
 
 return structure
 @
 
-We can test this as follows.
-<<test functions>>=
-def test_get_path():
-  assert conf.get("courses.datintro22.url") == "https://..."
-@
-
 To handle integers on the path, we do it in the pythonic way: we try to convert 
 it, if it fails, we just continue with the non-integer value.
 <<check if part is an integer, if so, convert it>>=
 try:
   part = int(part)
 except ValueError:
   pass
@@ -220,14 +210,40 @@
 <<test functions>>=
 def test_get_path_int():
   assert conf.get("courses.datintro22.TAs.0") == "Asse"
 @
 
 \subsubsection{Setting values}
 
+The set method is analogous to the get method, just it's inverse of sorts.
+However, it has a write back feature that we will discuss in \cref{writeback}.
+<<Config methods for get and set>>=
+def set(self, path: str, value: typing.Any):
+  """
+  Sets `value` at `path`. Any parts along the path that don't exist will be 
+  created.
+
+  Example:
+  - `value = "https://..."`,
+  - `path = "courses.datintro22.url"`
+  will create `{"courses": {"datintro22": {"url": "https://..."}}}`.
+
+  Any part of the path that can be converted to an integer, will be converted 
+  to an integer. This way we can access elements of lists too. However, we 
+  cannot create index 3 in a list if it doesn't exist (we can't expand 
+  lists).
+
+  If `value` is `None`, the entry at `path` will be deleted, if it exists.
+
+  <<set writeback doc>>
+  """
+  <<set value at path>>
+  <<set writeback code>>
+@
+
 To set a value is a bit more complex.
 We want to be able to specify a path and create all parents along the path if 
 they don't exist.
 However, if the value is [[None]], we don't want to create an entry that 
 doesn't exist, but we want to delete one if it already exists.
 <<set value at path>>=
 structure = self.__data
@@ -391,25 +407,31 @@
 
 \subsubsection{Reading the config}
 
 Let's start with reading.
 Anything that is derived from [[io.IOBase]] is already opened.
 Anything else, we pass to [[open]] to handle.
 <<Config methods for reading from and writing to file>>=
-def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
+def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json",
+                      <<additional [[read_config]] args>>):
   """
   Reads the config data structure (JSON) into the Config object.
+
   <<[[conf_file]] argument doc>>
 
+  <<additional [[read_config]] args doc>>
+
   <<documentation of config read error handling>>
   """
   if isinstance(conf_file, io.IOBase):
     <<read the data into [[self.__data]]>>
   else:
     <<open and read the config file>>
+
+  <<additional [[read_config]] args processing>>
 <<[[conf_file]] argument doc>>=
 `conf_file` is an optional argument providing one of the following:
 - an already opened file object (anything derived from `io.IOBase`);
 - anything that `open` can handle, for instance:
   - a string, which is the path to the config file;
   - an integer, which is a file descriptor (see `os.open`).
 @
@@ -424,15 +446,14 @@
 If we must open the file ourselves, we simply do that.
 But we do it in such a way that we can reuse
 [[<<read the data into [[self.__data]]>>]].
 <<open and read the config file>>=
 try:
   with open(conf_file) as conf_file:
     <<read the data into [[self.__data]]>>
-    return
 <<handle read config file errors>>
 @
 
 Let's test this functionality.
 <<test functions>>=
 def test_read_config():
   tmp = tempfile.mkdtemp()
@@ -457,26 +478,26 @@
 When reading the config file there are some errors that can occur.
 We catch them and rephrase the error messages.
 We turn the [[json.JSONDecodeError]] into a [[ValueError]] too.
 Let's summarize in the API documentation.
 <<documentation of config read error handling>>=
 Errors:
 
-- The first is that the file doesn't exist ([[FileNotFoundError]]). We silently 
+- The first is that the file doesn't exist (FileNotFoundError). We silently 
   fail this error. The reason is that the file doesn't exist, which means it's 
   an empty config. We fail silently as a later write would succeed.
-- There is also a related one, [[NotADirectoryError]]. The problem of 
-  [[NotADirectoryError]] occurs when a file on the path is used as a directory 
-  --- but only for reading, when trying to create a directory hierarchy, it 
-  will yield [[FileExistsError]]. We can't recover from this error, as an 
-  attempt to write to the file will also fail. We will reraise the exception 
-  with a better error message.
-- Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]). 
-  This is also a fatal error, we don't want a subsequent write to overwrite a 
-  corrupted config. We reraise the exception with a better error message.
+- There is also a related one, NotADirectoryError. The problem of 
+  NotADirectoryError occurs when a file on the path is used as a directory --- 
+  but only for reading, when trying to create a directory hierarchy, it will 
+  yield FileExistsError. We can't recover from this error, as an attempt to 
+  write to the file will also fail. We will reraise the exception with a better 
+  error message.
+- Finally, the file exists, but it's not proper JSON (JSONDecodeError). This is 
+  also a fatal error, we don't want a subsequent write to overwrite a corrupted 
+  config. We reraise the exception with a better error message.
 <<handle read config file errors>>=
 except FileNotFoundError as err:
   pass
 except NotADirectoryError as err:
   raise NotADirectoryError(f"A part of the path is a file, "
                            f"but used as directory: {err}")
 except json.decoder.JSONDecodeError as err:
@@ -580,14 +601,146 @@
     assert False
   """Should succeed"""
   path = tempfile.mkdtemp()
   conf.write_config(f"{path}/this/is/a/new/path/config.json")
 @
 
 
+\subsection{Writing back the changed config to file}\label{writeback}
+
+In some cases, when we read a config file and change it, we want to write the 
+changed back to the file we originally read.
+We will achieve that by letting the [[Config]] class remember the file the 
+config was read from.
+However, since we don't always want this, we will make it optional.
+
+We will start with the constructor of the [[Config]] class.
+<<Config constructor args doc>>=
+`conf_file` takes a path to a file which will be used as a config file. If this 
+argument is supplied, the data will be read from the file.
+
+Also, if `conf_file` is not None, we will enable automatic write back. So 
+that any changes (invokations of the `.set` method) will be written to the 
+config file immediately.
+
+To not enable write back, load file contents with the `.read_config` method.
+<<Config constructor args>>=
+conf_file=None
+@
+
+If we get a file, we simply call the [[.read_config]] method to load the data 
+into [[self.__data]].
+<<Config attributes>>=
+<<set [[self.__conf_file]] based on [[conf_file]]>>
+
+if self.__conf_file:
+  self.read_config(self.__conf_file)
+@
+
+If [[conf_file]] is a file-like object, we must extract the name of the file.
+This is so that we can reopen it in write mode when we want to do the write 
+back.
+If it doesn't have a name (attribute), then we raise an exception.
+If not a file-like object, we assume it's a path that can be passed directly to 
+[[open]].
+<<set [[self.__conf_file]] based on [[conf_file]]>>=
+if isinstance(conf_file, io.IOBase):
+  try:
+    self.__conf_file = conf_file.name
+  except AttributeError:
+    raise ValueError(f"can't enable writeback when `conf_file` is "
+                     f"a file-like object without a name: {conf_file}")
+else:
+  self.__conf_file = conf_file
+@
+
+We also want the corresponding write call in the [[.set]] method to actually 
+write back the config to file when it has successfully updated the config.
+<<set writeback doc>>=
+If write back is set (see `.__init__` and `.read_config`), a successful set 
+will also update the original config file.
+<<set writeback code>>=
+if self.__conf_file:
+  self.write_config(self.__conf_file)
+@
+
+Let's test this.
+We create a named temporary file.
+Then we write to it once, to have an initial config file.
+(Otherwise, JSON can't decode an empty file.)
+Then we try to get the original value and then change it.
+Finally, we try to read the config to see if the changed value was actually 
+written to the file.
+<<test functions>>=
+def test_writeback_constructor():
+  with tempfile.NamedTemporaryFile("w") as tmp_conf_file:
+    tmp_conf_file_name = "/tmp/writeback" #tmp_conf_file.name
+    path = "the.path"
+    first_value = "1st"
+    second_value = "2nd"
+
+    initial_conf = Config()
+    initial_conf.set(path, first_value)
+    initial_conf.write_config(tmp_conf_file_name)
+
+    conf = Config(conf_file=tmp_conf_file_name)
+    assert conf.get(path) == first_value
+    conf.set(path, second_value)
+
+    last_conf = Config()
+    last_conf.read_config(tmp_conf_file_name)
+    assert last_conf.get(path) == second_value
+<<test imports>>=
+import tempfile
+@
+
+We would like to be able to enable write back when we call [[.read_config]] 
+too.
+We want this in case we have an already created [[Config]] object, but want the 
+automatic write back.
+So we add an argument for that, but it defaults to not enabling it.
+<<additional [[read_config]] args>>=
+writeback=False
+<<additional [[read_config]] args doc>>=
+If `writeback` is set to True, store the `conf_file` object and turn on 
+automatic write back. This means that any changes using the `.set` method will 
+cause the config being written back to the file.
+
+Note that write back cannot be enabled with already opened files (as the mode 
+is already fixed).
+<<additional [[read_config]] args processing>>=
+if writeback:
+  <<set [[self.__conf_file]] based on [[conf_file]]>>
+@
+
+We test this in a similar fashion as before.
+However, now we will use the [[.read_config]] method to set the write back.
+<<test functions>>=
+def test_writeback_read_config():
+  with tempfile.NamedTemporaryFile("w") as tmp_conf_file:
+    tmp_conf_file_name = "/tmp/writeback" #tmp_conf_file.name
+    path = "the.path"
+    first_value = "1st"
+    second_value = "2nd"
+
+    initial_conf = Config()
+    initial_conf.set(path, first_value)
+    initial_conf.write_config(tmp_conf_file_name)
+
+    conf = Config()
+    conf.read_config(tmp_conf_file_name, writeback=True)
+    assert conf.get(path) == first_value
+    conf.set(path, second_value)
+
+    last_conf = Config()
+    last_conf.read_config(tmp_conf_file_name)
+    assert last_conf.get(path) == second_value
+@
+
+
 \section{Accessing the default configuration:
   the [[get]] and [[set]] functions}
 
 We will provide two module-level functions, [[get]] and [[set]], that allows 
 access to the default config, immediately syncing to the file system.
 <<helper functions>>=
 def get(path: str = "") -> typing.Any:
@@ -615,38 +768,65 @@
   conf.write_config()
 @
 
 
 \section{The [[config]] command}
 
 We will provide the [[config]] command as outlined above.
-If it gets a value, it will set it as the value at path.
-Otherwise, it will print the current value at path.
+If we get a path, but the user didn't use [[--set]] and provide a value, we 
+simply print the value at the end of the path.
+If we get a value through [[--set]], we'll update the value at the end of the 
+path (or create it if it doesn't exist).
+This corresponds to how the [[.set]] method of [[Config]] works.
+
+We have access to two variables: [[cli]], the Typer instance to which we want 
+to add the command; and [[conf_path]], which is the path to the config file.
+If [[conf_path]] is [[None]], we should use the default config file (as 
+determined by the [[.read_config]] method of [[Config]]).
+Otherwise, we supply [[.read_config]] with the [[conf_path]] value.
 <<config subcommands>>=
-path_arg = typer.Argument(...,
-                          help="Path in config, e.g. 'courses.datintro22'. "
-                               "Empty string is root of config.",
-                          shell_complete=complete_path_callback)
-value_arg = typer.Option([], "-s", "--set",
-                         help="Values to store. "
-                              "More than one value makes a list. "
-                              "Values are treated as JSON if possible.")
+conf = Config()
+try:
+  if conf_path:
+    conf.read_config(conf_path)
+  else:
+    conf.read_config()
+except ValueError:
+  pass
+
+<<default values for [[config_cmd]]>>
 
 @cli.command(name="config")
 def config_cmd(path: str = path_arg,
                values: typing.List[str] = value_arg):
   """
   Reads values from or writes values to the config.
   """
   if values:
     <<change [[values]] to non-list if one-element list>>
     <<if [[values]] is empty string, replace it with [[None]]>>
-    set(path, values)
+    conf.set(path, values)
   else:
-    print_config(get(path), path)
+    print_config(conf.get(path), path)
+@
+
+The default values are the special Typer objects that specify how the command 
+arguments and options should behave.
+We can autocomplete the path since we can predict the possible values.
+The same cannot be said of the value to store, that can be arbitrary.
+<<default values for [[config_cmd]]>>=
+path_arg = typer.Argument("",
+                          help="Path in config, e.g. 'courses.datintro22'. "
+                               "Empty string is root of config. Defaults to "
+                               "the empty string.",
+                          autocompletion=complete_path_callback)
+value_arg = typer.Option([], "-s", "--set",
+                         help="Values to store. "
+                              "More than one value makes a list. "
+                              "Values are treated as JSON if possible.")
 @
 
 If the user supplies only one argument on the command line, we don't want it to 
 be interpreted as a one-element list, but rather as a value that is not a list.
 Hence, we check and convert if necessary.
 <<change [[values]] to non-list if one-element list>>=
 if len(values) == 1:
@@ -657,43 +837,64 @@
 [[None]] to trigger a delete.
 <<if [[values]] is empty string, replace it with [[None]]>>=
 if values == "":
   values = None
 @
 
 Let's test this command.
+We'll set up the testing.
 <<test functions>>=
 runner = CliRunner()
 
 def test_cli():
-  # set example data
-  result = runner.invoke(cli,
-                         ["courses.datintro22.url", "--set", "https://..."])
-  assert result.exit_code == 0
-
-  # try access nonexisting
-  result = runner.invoke(cli, ["courses.datintro.url"])
-  assert result.exit_code == 1
-
-  # access existing
-  result = runner.invoke(cli, ["courses.datintro22.url"])
-  assert "courses.datintro22.url = https://..." in result.stdout
-
-  # clear config
-  result = runner.invoke(cli,
-                         ["courses", "--set", None])
-  assert result.exit_code == 0
-
-  # check that it's cleared
-  result = runner.invoke(cli, ["courses"])
-  assert "courses" not in result.stdout
+  <<run tests on [[cli]]>>
 <<test imports>>=
 from typer.testing import CliRunner
 @
 
+Let's look at the actual tests.
+<<run tests on [[cli]]>>=
+# set example data
+result = runner.invoke(cli,
+                        ["courses.datintro22.url", "--set", "https://..."])
+assert result.exit_code == 0
+
+# try access nonexisting
+result = runner.invoke(cli, ["courses.datintro.url"])
+assert result.exit_code == 1
+
+# access existing
+result = runner.invoke(cli, ["courses.datintro22.url"])
+assert "courses.datintro22.url = https://..." in result.stdout
+
+# clear config
+result = runner.invoke(cli,
+                        ["courses", "--set", None])
+assert result.exit_code == 0
+
+# check that it's cleared
+result = runner.invoke(cli, ["courses"])
+assert "courses" not in result.stdout
+@
+
+Let's also test it with the non-default config.
+Note that we want the temporary file to open it ourselves, hence we close it 
+immediately (through an empty [[with]] statement) and ensure it's not deleted 
+on closing.
+<<test functions>>=
+def test_cli_not_default_conf():
+  with tempfile.NamedTemporaryFile(delete=False) as tmp_conf:
+    pass
+
+  cli = typer.Typer()
+  add_config_cmd(cli, tmp_conf.name)
+
+  <<run tests on [[cli]]>>
+@
+
 
 \subsection{Autocompleting the path}
 
 The [[complete_path]] function returns the possible completions for an 
 incomplete path from the command line.
 <<helper functions>>=
 def complete_path(initial_path: str, conf: Config = None):
@@ -719,23 +920,21 @@
       }
     }
   })
 
   incomplete = "courses.datintro22.T"
   assert "courses.datintro22.TAs" in complete_path(incomplete, conf)
   assert "courses.datintro22.url" not in complete_path(incomplete, conf)
-  assert len(complete_path(incomplete, conf)) >= 0
+  assert len(list(complete_path(incomplete, conf))) >= 0
 @
 
 Now, the callback must not have any additional arguments, like we want that 
 [[conf]] argument for testing.
 <<helper functions>>=
-def complete_path_callback(ctx: typer.Context,
-                           args: typing.List[str],
-                           initial_path: str):
+def complete_path_callback(initial_path: str):
   return complete_path(initial_path)
 @
 
 
 \subsection{Printing the config}
 
 That [[print_config]] function should print the remaining levels of the config
```

### Comparing `typerconf-1.9/PKG-INFO` & `typerconf-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 1.9
+Version: 2.0
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
```

