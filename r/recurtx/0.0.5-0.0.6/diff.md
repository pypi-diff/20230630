# Comparing `tmp/recurtx-0.0.5.tar.gz` & `tmp/recurtx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recurtx-0.0.5.tar", last modified: Thu Jun 29 07:48:32 2023, max compression
+gzip compressed data, was "recurtx-0.0.6.tar", last modified: Fri Jun 30 03:29:31 2023, max compression
```

## Comparing `recurtx-0.0.5.tar` & `recurtx-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:48:32.000000 recurtx-0.0.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-26 05:04:07.000000 recurtx-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-29 07:48:32.000000 recurtx-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5715 2023-06-26 05:04:07.000000 recurtx-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-26 05:04:07.000000 recurtx-0.0.5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:48:32.000000 recurtx-0.0.5/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 05:04:08.000000 recurtx-0.0.5/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-06-29 05:58:08.000000 recurtx-0.0.5/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4043 2023-06-29 07:43:05.000000 recurtx-0.0.5/recurtx/ll.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-06-27 14:45:56.000000 recurtx-0.0.5/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     4628 2023-06-27 14:46:00.000000 recurtx-0.0.5/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     3786 2023-06-29 02:59:29.000000 recurtx-0.0.5/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-26 05:04:08.000000 recurtx-0.0.5/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-06-28 13:50:26.000000 recurtx-0.0.5/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:48:32.000000 recurtx-0.0.5/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-29 07:48:32.000000 recurtx-0.0.5/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-29 07:48:31.000000 recurtx-0.0.5/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-29 07:48:32.000000 recurtx-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1596 2023-06-29 05:57:26.000000 recurtx-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:29:31.910000 recurtx-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-29 07:50:39.000000 recurtx-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-30 03:29:31.910000 recurtx-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-06-29 07:50:39.000000 recurtx-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-30 02:28:42.000000 recurtx-0.0.6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:29:31.900000 recurtx-0.0.6/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-29 07:50:40.000000 recurtx-0.0.6/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 15:19:50.000000 recurtx-0.0.6/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4043 2023-06-30 03:17:02.000000 recurtx-0.0.6/recurtx/ll.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-06-30 02:16:12.000000 recurtx-0.0.6/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     4643 2023-06-30 02:04:12.000000 recurtx-0.0.6/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     3868 2023-06-30 02:58:56.000000 recurtx-0.0.6/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2023-06-30 02:00:44.000000 recurtx-0.0.6/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-06-30 02:49:28.000000 recurtx-0.0.6/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:29:31.910000 recurtx-0.0.6/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-30 03:29:31.910000 recurtx-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1596 2023-06-29 07:50:41.000000 recurtx-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `recurtx-0.0.5/LICENSE` & `recurtx-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.5/PKG-INFO` & `recurtx-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.5/README.md` & `recurtx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.5/recurtx/__main__.py` & `recurtx-0.0.6/recurtx/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,18 +43,7 @@
 
 def xsearch():
     fire.Fire(search)
 
 
 def xll():
     fire.Fire(ll)
-
-
-if __name__ == "__main__":
-    main()
-    xpandas()
-    xpolars()
-    xbatch()
-    xunder()
-    xfind()
-    xsearch()
-    xstat()
```

### Comparing `recurtx-0.0.5/recurtx/ll.py` & `recurtx-0.0.6/recurtx/ll.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     number_limit: int = 100,
     sort_paths: str = "asc",
     info: bool = True,
     extension_most_common: int = 1,
 ):
     """Compute statistics for the directory recursively."""
 
-    paths = paths or ["."]
+    paths = paths or (".",)
 
     if depth:
         glob = "".join(["*/"] * (depth - 1)) + "*"
 
     stat_ls = []
 
     for path in paths:
-        path = Path(upath(path))
+        _path = Path(upath(path))
 
         if type:
-            dir_path_ls = [p for p in (path.glob(glob)) if getattr(p, "is_" + type)()]
+            dir_path_ls = [p for p in (_path.glob(glob)) if getattr(p, "is_" + type)()]
         else:
-            dir_path_ls = list(path.glob(glob))
+            dir_path_ls = list(_path.glob(glob))
 
         if sort_paths:
             assert isinstance(sort_paths, str), sort_paths
             dir_path_ls.sort(reverse=(sort_paths.lower().startswith("desc")))
 
         if info:
             for dir_path in dir_path_ls:
@@ -115,15 +115,15 @@
                 max_size = "{:,}".format(max_size)
 
             if type == "file":
                 d.update(dict(size=total_size))
             else:
                 d.update(
                     dict(
-                        num_files=num_files,
+                        files=num_files,
                         total_size=total_size,
                         max_size=max_size,
                         # latest_mtime=latest_mtime,
                     )
                 )
                 d.update(common_ext_dict)
```

### Comparing `recurtx-0.0.5/recurtx/pandas.py` & `recurtx-0.0.6/recurtx/pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List
+from typing import List, Tuple
 
 from .utils import infer_type, stdout_lines
 
 DATA_TYPES = {
     "pickle",
     "table",
     "csv",
@@ -38,15 +38,15 @@
     merge: str = None,
     on: str = None,
     left_on: str = None,
     right_on: str = None,
     left_index: bool = False,
     right_index: bool = False,
     sort: bool = False,
-    suffixes: str = ("_x", "_y"),
+    suffixes: Tuple[str, str] = ("_x", "_y"),
     copy: bool = True,
     indicator: bool = False,
     validate: str = None,
     lsuffix: str = None,
     rsuffix: str = None,
     query: str = None,
     head: int = None,
@@ -224,15 +224,16 @@
         nonlocal _write_func, df
         try:
             if _write_type == "json":
                 import json
 
                 ls = df.to_dict(orient="records")
                 if write_path:
-                    json.dump(ls, write_path)
+                    with open(write_path, "w") as f:
+                        json.dump(ls, f)
                 else:
                     return json.dumps(ls)
             return _write_func(write_path, index=index)
         except:
             return _write_func(write_path)
 
     if write_path:
```

### Comparing `recurtx-0.0.5/recurtx/polars.py` & `recurtx-0.0.6/recurtx/polars.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     kwargs.pop("write_path", None)
 
     _write_type = (
         infer_type(write_type, write_path, DATA_TYPES.union({"markdown"}), polars=True)
         or "csv"
     )
 
-    streaming = streaming in TRUE_VALUES
+    streaming_flag = streaming in TRUE_VALUES
 
     import polars as pl
 
     ls = []
     for path in paths:
         _read_type = infer_type(read_type, path, DATA_TYPES, polars=True)
         if not _read_type:
@@ -140,22 +140,22 @@
         subset_ls.append(df.head(head))
     if tail is not None:
         subset_ls.append(df.tail(tail))
     if subset_ls:
         df = pl.concat(subset_ls)
 
     if sample is not None:
-        df = activate(df, fetch, streaming)
+        df = activate(df, fetch, streaming_flag)
         df = df.sample(sample)
         df = df.lazy()
 
     if method is not None:
         df = eval("df." + method)
 
-    df = activate(df, fetch, streaming)
+    df = activate(df, fetch, streaming_flag)
 
     if not isinstance(df, pl.DataFrame):
         text = "{}".format(df)
         if write_path:
             Path(write_path).write_text(text)
         else:
             stdout_lines(text)
```

### Comparing `recurtx-0.0.5/recurtx/recur.py` & `recurtx-0.0.6/recurtx/recur.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,114 +22,115 @@
     show_scripts = kwargs.pop("show_scripts", False)
 
     if regex:
         rx = re.compile(regex)
     else:
         rx = None
 
-    scripts = list(scripts)
-    if len(kwargs) and len(scripts) == 1:
-        scripts = scripts[0].split(" ")
+    script_ls = list(scripts)
+    if len(kwargs) and len(script_ls) == 1:
+        script_ls = script_ls[0].split(" ")
     for k, v in kwargs.items():
         if isinstance(v, bool) and v == False:
             continue
         if len(k) >= 2:
-            scripts.append("--" + k)
+            script_ls.append("--" + k)
         elif len(k) == 1:
-            scripts.append("-" + k)
+            script_ls.append("-" + k)
         else:
             raise NotImplementedError()
         if isinstance(v, bool):
             continue
-        scripts.append(str(v))
+        script_ls.append(str(v))
 
-    if not scripts:
-        scripts = ["echo"]
+    if not script_ls:
+        script_ls = ["echo"]
 
-    if replace_str and all([replace_str not in script for script in scripts]):
-        if len(scripts) >= 2:
-            scripts.append(replace_str)
+    if replace_str and all([replace_str not in script for script in script_ls]):
+        if len(script_ls) >= 2:
+            script_ls.append(replace_str)
         else:
-            scripts[0] += " " + replace_str
+            script_ls[0] += " " + replace_str
 
-    path = Path(upath(path))
-    assert path.exists(), str(path.resolve()) + " does not exist."
+    _path = Path(upath(path))
+    assert _path.exists(), str(_path.resolve()) + " does not exist."
 
-    if path.is_file():
-        path_ls = [str(path)]
+    if _path.is_file():
+        path_ls = [str(_path)]
     else:
-        path_ls = [str(p) for p in path.glob(glob) if getattr(p, "is_" + type)()]
+        path_ls = [str(p) for p in _path.glob(glob) if getattr(p, "is_" + type)()]
         if rx:
             path_ls = [p for p in path_ls if rx.match(p)]
         if sort_paths:
             assert isinstance(sort_paths, str), sort_paths
             path_ls.sort(reverse=(sort_paths.lower().startswith("desc")))
 
     if show_paths:
         sys.stdout.write(
             "[Searching files]\n" + str("\n".join(["    " + p for p in path_ls]) + "\n")
         )
-    return path_ls, scripts, replace_str, show_scripts
+    return path_ls, script_ls, replace_str, show_scripts
 
 
 def under(
     path: str,
     *scripts: str,
     **kwargs: str,
 ):
     """Run any scripts for each file under a directory recursively."""
 
-    path_ls, scripts, replace_str, show_scripts = recur(
+    path_ls, script_ls, replace_str, show_scripts = recur(
         path,
         *scripts,
         **kwargs,
     )
 
-    running_scripts = scripts
     for p in path_ls:
         try:
+            running_script_ls = script_ls
             if replace_str:
-                running_scripts = [
+                running_script_ls = [
                     script.replace(replace_str, p)
                     if isinstance(script, str)
                     else script
-                    for script in scripts
+                    for script in script_ls
                 ]
-            if len(running_scripts) == 1:
-                running_scripts = running_scripts[0]
-            subprocess_run(running_scripts, show_scripts)
+            if len(running_script_ls) == 1:
+                running_script_ls = running_script_ls[0]
+            subprocess_run(running_script_ls, show_scripts)
         except Exception:
             msg = get_exception_msg()
             sys.stdout.write(msg)
             continue
 
 
 def batch(
     path: str,
     *scripts: str,
     **kwargs: str,
 ):
     """Run any scripts for a batch of files in a directory recursively."""
 
-    path_ls, scripts, replace_str, show_scripts = recur(
+    path_ls, script_ls, replace_str, show_scripts = recur(
         path,
         *scripts,
         **kwargs,
     )
 
-    running_scripts = scripts
-    if len(scripts) == 1:
-        running_scripts = scripts[0]
+    if len(script_ls) == 1:
+        running_script_ls = script_ls[0]
         if replace_str:
-            running_scripts = running_scripts.replace(replace_str, " ".join(path_ls))
+            running_script_ls = running_script_ls.replace(
+                replace_str, " ".join(path_ls)
+            )
     else:
-        running_scripts = []
-        for script in scripts:
+        running_script_ls = []
+        for script in script_ls:
             if replace_str and (script == replace_str):
-                running_scripts.extend(path_ls)
+                running_script_ls.extend(path_ls)
             else:
-                running_scripts.append(script)
+                running_script_ls.append(script)
     try:
-        subprocess_run(running_scripts, show_scripts)
+        subprocess_run(running_script_ls, show_scripts)
     except Exception:
         msg = get_exception_msg()
         sys.stdout.write(msg)
```

### Comparing `recurtx-0.0.5/recurtx/search.py` & `recurtx-0.0.6/recurtx/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import sys
 from pathlib import Path
+from typing import List, Set, Tuple, Union
 
 
 def run_search(
     text: str,
-    target: str,
+    target: Union[str, List, Tuple, Set],
     path: Path,
-    sub: str = None,
+    sub: Union[str, List, Tuple, Set] = None,
     wildcard: str = "*",
     separator: str = "/",
     verbose: int = 1,
 ):
     assert isinstance(separator, str), str(separator) + ": " + str(type(separator))
 
-    if isinstance(target, (list, tuple, set, dict)):
+    if isinstance(target, (list, set, tuple)):
         targets = target
     else:
         assert isinstance(target, str), str(type(target))
         if separator:
             targets = target.split(separator)
         else:
             targets = [target]
 
-    if isinstance(sub, (list, tuple, set, dict)):
+    if isinstance(sub, (list, tuple, set)):
         subs = sub
     elif sub is None:
         subs = [None] * len(targets)
     else:
         assert isinstance(sub, str), str(type(sub))
         if separator:
             subs = sub.split(separator)
         else:
             subs = [sub]
 
     assert len(targets) == len(subs), str(len(targets)) + " != " + str(len(subs))
 
-    for target, sub in zip(targets, subs):
-        target_ls = eval("'''" + target + "'''").split(wildcard)
+    for _target, _sub in zip(targets, subs):
+        target_ls = eval("'''" + _target + "'''").split(wildcard)
 
         replacing_ls = []
         end_index = 0
 
         while True:
             index = end_index
             start_index = None
@@ -50,79 +51,79 @@
                 if index >= 0:
                     start_index = start_index or index
                     index = index + len(target_ss)
                 else:
                     break
             if start_index and (index >= 0):
                 end_index = index
-                if sub is not None:
+                if _sub is not None:
                     replacing = text[start_index:end_index]
                     replacing_ls.append(replacing)
                 if verbose >= 1:
                     sys.stdout.write(
                         f"{path} [{start_index}:{end_index}]\n{text[start_index:end_index]}\n"
                     )
             else:
                 break
         for replacing in list(set(replacing_ls)):
-            text = text.replace(replacing, sub)
+            text = text.replace(replacing, _sub)
 
     return text
 
 
 def search(
     target: str,
     path: str,
     sub: str = None,
     wildcard: str = "*",
     separator: str = "/",
     verbose: int = 1,
 ):
     """Search a keyword, which may include wildcards, in the text file content, and optionally substitute (replace)."""
 
-    path = Path(path)
+    _path = Path(path)
     try:
-        text = path.read_text()
+        text = _path.read_text()
     except Exception:
         if verbose >= 3:
             raise
         return
 
     text = run_search(
         text=text,
         target=target,
-        path=path,
+        path=_path,
         sub=sub,
         wildcard=wildcard,
         separator=separator,
         verbose=verbose,
     )
 
     if sub is not None:
-        path.write_text(text)
+        _path.write_text(text)
 
 
 def find(
     target: str,
     path: str,
     sub: str = None,
     wildcard: str = "*",
     separator: str = "/",
     verbose: int = 1,
 ):
     """Find a keyword, which may include wildcards, in the file path, and optionally substitute (replace)."""
 
     text = path
-    path = Path(path)
+    _path = Path(path)
 
     text = run_search(
         text=text,
         target=target,
-        path=path,
+        path=_path,
         sub=sub,
         wildcard=wildcard,
         separator=separator,
         verbose=verbose,
     )
 
     if sub is not None:
-        path.rename(text)
+        _path.rename(text)
```

### Comparing `recurtx-0.0.5/recurtx/utils.py` & `recurtx-0.0.6/recurtx/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
+import subprocess
 import sys
 import traceback
 from pathlib import Path
-from typing import List, Set, Union
+from time import sleep
+from typing import List, Optional, Set, Union
 
 
-def get_exception_msg():
+def get_exception_msg() -> str:
     return "".join(traceback.format_exception(*sys.exc_info()))
 
 
 def upath(
     path: str,
-):
+) -> str:
     if isinstance(path, str) and path.startswith("~"):
         path = str(Path.home()) + path[1:]
     if isinstance(path, str) and path.startswith("."):
         path = str(Path.cwd()) + path[1:]
     return path
 
 
 def subprocess_run(
     script: Union[str, List[str]],
     verbose: bool = True,
-):
+) -> subprocess.CompletedProcess:
     if verbose:
         sys.stdout.write(r">>> " + str(script) + "\n")
 
-        from time import sleep
-
         sleep(0.2)
 
-    import subprocess
-
+    assert script, script
     shell = isinstance(script, str)
     return subprocess.run(script, shell=shell)
 
 
-def stdout_lines(text: str):
+def stdout_lines(text: str) -> None:
     if not text.endswith("\n"):
         text += "\n"
     sys.stdout.write(text)
+    return None
 
 
 def infer_type(
-    type: str,
-    path: str,
+    type: Optional[str],
+    path: Optional[str],
     supported_types: Set[str],
     polars: bool = False,
-):
+) -> Union[str, None]:
     if isinstance(type, str) and type:
         _type = type
         _type = _type.replace("md", "markdown")
         if polars:
             _type = _type.replace("jsonl", "ndjson")
         assert _type in supported_types, (
             _type + " not in supported set: " + str(supported_types)
```

### Comparing `recurtx-0.0.5/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.6/recurtx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.5/setup.py` & `recurtx-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": console_scripts},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

