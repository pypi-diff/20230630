# Comparing `tmp/recurtx-0.0.6.tar.gz` & `tmp/recurtx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurtx-0.0.6.tar", last modified: Fri Jun 30 03:29:31 2023, max compression
+gzip compressed data, was "recurtx-0.0.7.tar", last modified: Fri Jun 30 15:35:49 2023, max compression
```

## Comparing `recurtx-0.0.6.tar` & `recurtx-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:29:31.910000 recurtx-0.0.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-29 07:50:39.000000 recurtx-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-30 03:29:31.910000 recurtx-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5715 2023-06-29 07:50:39.000000 recurtx-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-30 02:28:42.000000 recurtx-0.0.6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:29:31.900000 recurtx-0.0.6/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-29 07:50:40.000000 recurtx-0.0.6/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-29 15:19:50.000000 recurtx-0.0.6/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4043 2023-06-30 03:17:02.000000 recurtx-0.0.6/recurtx/ll.py
--rw-r--r--   0 root         (0) root         (0)     6742 2023-06-30 02:16:12.000000 recurtx-0.0.6/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     4643 2023-06-30 02:04:12.000000 recurtx-0.0.6/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     3868 2023-06-30 02:58:56.000000 recurtx-0.0.6/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     3279 2023-06-30 02:00:44.000000 recurtx-0.0.6/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-30 02:49:28.000000 recurtx-0.0.6/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 03:29:31.910000 recurtx-0.0.6/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-30 03:29:31.000000 recurtx-0.0.6/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-30 03:29:31.910000 recurtx-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1596 2023-06-29 07:50:41.000000 recurtx-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:35:49.950000 recurtx-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-30 14:54:37.000000 recurtx-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-30 15:35:49.950000 recurtx-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-06-30 14:54:37.000000 recurtx-0.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-30 14:54:37.000000 recurtx-0.0.7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:35:49.940000 recurtx-0.0.7/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/ll.py
+-rw-r--r--   0 root         (0) root         (0)     7134 2023-06-30 15:06:35.000000 recurtx-0.0.7/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-06-30 14:54:37.000000 recurtx-0.0.7/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-06-30 14:54:38.000000 recurtx-0.0.7/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-06-30 14:54:38.000000 recurtx-0.0.7/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-06-30 14:54:38.000000 recurtx-0.0.7/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 15:35:49.950000 recurtx-0.0.7/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-30 15:35:49.000000 recurtx-0.0.7/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-30 15:35:49.950000 recurtx-0.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1547 2023-06-30 14:54:39.000000 recurtx-0.0.7/setup.py
```

### Comparing `recurtx-0.0.6/LICENSE` & `recurtx-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.6/PKG-INFO` & `recurtx-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.6
+Version: 0.0.7
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recurtx-0.0.6/README.md` & `recurtx-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # recurtx
 
-[![Python version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue.svg)](https://pypi.org/project/recurtx/)
+[![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)](https://pypi.org/project/recurtx/)
 [![PyPI version](https://badge.fury.io/py/recurtx.svg)](https://badge.fury.io/py/recurtx)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/Minyus/recurtx/blob/main/LICENSE)
 
 CLI to transform text files recursively
 
 ## Install
```

### Comparing `recurtx-0.0.6/recurtx/ll.py` & `recurtx-0.0.7/recurtx/ll.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 import sys
 from collections import Counter
 from pathlib import Path
+from typing import Any, Dict, List, Optional
 
 from .utils import upath
 
 
 def ll(
     *paths: str,
     depth: int = 1,
     glob: str = "**/*",
-    type: str = None,
+    type: Optional[str] = None,
     file_glob: str = "**/*",
     number_limit: int = 100,
     sort_paths: str = "asc",
     info: bool = True,
     extension_most_common: int = 1,
-):
+) -> None:
     """Compute statistics for the directory recursively."""
 
     paths = paths or (".",)
 
     if depth:
         glob = "".join(["*/"] * (depth - 1)) + "*"
 
@@ -53,97 +54,94 @@
             sys.stdout.write("\n".join([str(p) for p in dir_path_ls]) + "\n")
 
     if info:
         _output_stat(stat_ls)
 
 
 def _get_stat(
-    dir_path,
-    glob,
-    type,
-    number_limit,
-    extension_most_common,
-):
+    dir_path: Path,
+    glob: str,
+    type: Optional[str],
+    number_limit: int,
+    extension_most_common: int,
+) -> Optional[Dict]:
     if dir_path.is_dir():
         path_ls = [p for p in dir_path.glob(glob) if p.is_file()]
     else:
         path_ls = [dir_path]
 
     if not path_ls:
         return None
 
-    if True:
-        if True:
-            num_files = len(path_ls)
-
-            divisor = None
-            if num_files > number_limit:
-                divisor = num_files / number_limit
-
-            path_ls = path_ls[:number_limit]
-
-            size_ls = []
-            # mtime_ls = []
-            ext_ls = []
-            for p in path_ls:
-                st = os.stat(p)
-                size_ls.append(st.st_size)
-                # mtime_ls.append(st.st_mtime)
-
-                ext = p.suffix
-                ext_ls.append(ext)
-
-            total_size = sum(size_ls)
-            max_size = max(size_ls)
-            # latest_mtime = max(mtime_ls)
-            if extension_most_common:
-                common_ext_count_ls = Counter(ext_ls).most_common(extension_most_common)
-                common_ext_dict = {
-                    "ext_" + str(i + 1): common_ext_count_ls[i][0]
-                    for i in range(extension_most_common)
-                }
-
-            d = dict(path=str(dir_path) + (os.sep if dir_path.is_dir() else ""))
-
-            num_files = "{:,}".format(num_files)
-
-            if divisor:
-                total_size = round(total_size * divisor)
-                total_size = "~ {:,}".format(total_size)
-                max_size = ">= {:,}".format(max_size)
-            else:
-                total_size = "{:,}".format(total_size)
-                max_size = "{:,}".format(max_size)
-
-            if type == "file":
-                d.update(dict(size=total_size))
-            else:
-                d.update(
-                    dict(
-                        files=num_files,
-                        total_size=total_size,
-                        max_size=max_size,
-                        # latest_mtime=latest_mtime,
-                    )
-                )
-                d.update(common_ext_dict)
-
-            return d
-
+    num_files = len(path_ls)
 
-def _output_stat(stat_ls):
-    if True:
-        try:
-            import pandas as pd
-
-            colalign_ls = None
-            if stat_ls:
-                colalign_ls = ["right"] * len(stat_ls[0])
-                colalign_ls[0] = "left"
+    divisor = None
+    if num_files > number_limit:
+        divisor = num_files / number_limit
+
+    path_ls = path_ls[:number_limit]
+
+    size_ls = []
+    # mtime_ls = []
+    ext_ls = []
+    for p in path_ls:
+        st = p.stat()
+        size_ls.append(st.st_size)
+        # mtime_ls.append(st.st_mtime)
+
+        ext = p.suffix
+        ext_ls.append(ext)
+
+    total_size = sum(size_ls)
+    max_size = max(size_ls)
+    # latest_mtime = max(mtime_ls)
+    if extension_most_common:
+        common_ext_count_ls = Counter(ext_ls).most_common(extension_most_common)
+        common_ext_dict = {
+            "ext_" + str(i + 1): common_ext_count_ls[i][0]
+            for i in range(extension_most_common)
+        }
+
+    d = {"path": str(dir_path) + (os.sep if dir_path.is_dir() else "")}
+
+    _num_files = f"{num_files:,}"
+
+    if divisor:
+        total_size = round(total_size * divisor)
+        _total_size = f"~ {total_size:,}"
+        _max_size = f">= {max_size:,}"
+    else:
+        _total_size = f"{total_size:,}"
+        _max_size = f"{max_size:,}"
 
-            df = pd.DataFrame(stat_ls)
-            md = df.to_markdown(index=False, colalign=colalign_ls)
-            sys.stdout.write(str(md) + "\n")
-        except:
-            import json
+    if type == "file":
+        d.update({"size": _total_size})
+    else:
+        d.update(
+            {
+                "files": _num_files,
+                "total_size": _total_size,
+                "max_size": _max_size,
+                # "latest_mtime": latest_mtime,
+            },
+        )
+        d.update(common_ext_dict)
+
+    return d
+
+
+def _output_stat(stat_ls: List[Dict[str, Any]]) -> None:
+    try:
+        import pandas as pd
+
+        colalign_ls = None
+        if stat_ls:
+            colalign_ls = ["right"] * len(stat_ls[0])
+            colalign_ls[0] = "left"
+
+        df = pd.DataFrame(stat_ls)
+        md = df.to_markdown(index=False, colalign=colalign_ls)
+        sys.stdout.write(str(md) + "\n")
+    except Exception:
+        import json
 
-            sys.stdout.write(json.dumps(stat_ls, indent=2) + "\n")
+        sys.stdout.write(json.dumps(stat_ls, indent=2) + "\n")
```

### Comparing `recurtx-0.0.6/recurtx/pandas.py` & `recurtx-0.0.7/recurtx/pandas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
-from typing import List, Tuple
+from typing import Any, List, Optional, Tuple
 
-from .utils import infer_type, stdout_lines
+from .utils import infer_format, stdout_lines
 
 DATA_TYPES = {
     "pickle",
     "table",
     "csv",
     "fwf",
     "clipboard",
@@ -26,46 +26,45 @@
     "stata",
 }
 
 
 def pandas(
     *paths: str,
     package: str = "pandas",
-    read_type: str = None,
-    columns: List[str] = None,
-    excluding_columns: List[str] = None,
-    filepath_column: str = None,
-    join: str = None,
-    merge: str = None,
-    on: str = None,
-    left_on: str = None,
-    right_on: str = None,
+    input_format: Optional[str] = None,
+    columns: Optional[List[str]] = None,
+    excluding_columns: Optional[List[str]] = None,
+    filepath_column: Optional[str] = None,
+    join: Optional[str] = None,
+    merge: Optional[str] = None,
+    on: Optional[str] = None,
+    left_on: Optional[str] = None,
+    right_on: Optional[str] = None,
     left_index: bool = False,
     right_index: bool = False,
     sort: bool = False,
     suffixes: Tuple[str, str] = ("_x", "_y"),
     copy: bool = True,
     indicator: bool = False,
-    validate: str = None,
-    lsuffix: str = None,
-    rsuffix: str = None,
-    query: str = None,
-    head: int = None,
-    tail: int = None,
-    sample: int = None,
-    method: str = None,
-    write_type: str = None,
-    write_path: str = None,
-    **kwargs,
-):
+    validate: Optional[str] = None,
+    lsuffix: Optional[str] = None,
+    rsuffix: Optional[str] = None,
+    query: Optional[str] = None,
+    head: Optional[int] = None,
+    tail: Optional[int] = None,
+    sample: Optional[int] = None,
+    method: Optional[str] = None,
+    output_format: Optional[str] = None,
+    output_path: Optional[str] = None,
+    **kwargs: Any,
+) -> None:
     """Read and transform tabular files using pandas."""
-
     """Workaround for unexpected behavior of Fire"""
     kwargs.pop("package", None)
-    kwargs.pop("read_type", None)
+    kwargs.pop("input_format", None)
     kwargs.pop("columns", None)
     kwargs.pop("excluding_columns", None)
     kwargs.pop("filepath_column", None)
     kwargs.pop("join", None)
     kwargs.pop("merge", None)
     kwargs.pop("on", None)
     kwargs.pop("left_on", None)
@@ -80,44 +79,45 @@
     kwargs.pop("lsuffix", "")
     kwargs.pop("rsuffix", "")
     kwargs.pop("query", None)
     kwargs.pop("head", None)
     kwargs.pop("tail", None)
     kwargs.pop("sample", None)
     kwargs.pop("method", None)
-    kwargs.pop("write_type", None)
-    kwargs.pop("write_path", None)
+    kwargs.pop("output_format", None)
+    kwargs.pop("output_path", None)
 
-    _write_type = (
-        infer_type(write_type, write_path, DATA_TYPES.union({"markdown"})) or "csv"
+    _output_format = (
+        infer_format(output_format, output_path, DATA_TYPES.union({"markdown"}))
+        or "csv"
     )
 
     if package == "modin":
         import modin.pandas as pd
     elif package == "pandas":
         import pandas as pd
     else:
         raise NotImplementedError(
             "'" + package + "' not supported. Set one of ['pandas', 'modin']"
         )
-    import numpy as np
+    import numpy as np  # noqa: F401
 
     if columns and isinstance(columns, str):
         columns = [columns]
     if excluding_columns and isinstance(excluding_columns, str):
         excluding_columns = [excluding_columns]
 
     ls = []
     for path in paths:
-        _read_type = infer_type(read_type, path, DATA_TYPES)
-        if not _read_type:
+        _input_format = infer_format(input_format, path, DATA_TYPES)
+        if not _input_format:
             continue
-        read_func = getattr(pd, "read_" + _read_type)
+        read_func = getattr(pd, "read_" + _input_format)
         _kwargs = kwargs.copy()
-        if read_type == "csv":
+        if input_format == "csv":
             _kwargs.setdefault("dtype", str)
             _kwargs.setdefault("keep_default_na", False)
             if columns:
                 _kwargs.setdefault("usecols", columns)
         df = read_func(path, **_kwargs)
 
         if columns:
@@ -132,15 +132,15 @@
 
         if query:
             df = df.query(query)
         ls.append(df)
 
     if not ls:
         return
-    elif len(ls) == 1:
+    if len(ls) == 1:
         df = ls[0]
     elif merge is not None:
         df = ls[0]
         for right_df in ls[1:]:
             if merge == "anti":
                 cols = df.columns
                 df = (
@@ -207,37 +207,40 @@
     if sample is not None:
         df = df.sample(sample)
 
     if method is not None:
         df = eval("df." + method)
 
     if not isinstance(df, pd.DataFrame):
-        text = "{}".format(df)
-        if write_path:
-            Path(write_path).write_text(text)
+        text = f"{df}"
+        if output_path:
+            Path(output_path).write_text(text)
         else:
             stdout_lines(text)
         return
 
-    _write_func = getattr(df, "to_" + _write_type)
+    _write_func = getattr(df, "to_" + _output_format)
 
-    def write_func(write_path: str = None, index=False):
+    def write_func(
+        output_path: Optional[str] = None,
+        index: bool = False,
+    ) -> Optional[str]:
         nonlocal _write_func, df
         try:
-            if _write_type == "json":
+            if _output_format == "json":
                 import json
 
                 ls = df.to_dict(orient="records")
-                if write_path:
-                    with open(write_path, "w") as f:
+                if output_path:
+                    with open(output_path, "w") as f:
                         json.dump(ls, f)
                 else:
                     return json.dumps(ls)
-            return _write_func(write_path, index=index)
-        except:
-            return _write_func(write_path)
+            return _write_func(output_path, index=index)
+        except Exception:
+            return _write_func(output_path)
 
-    if write_path:
-        write_func(write_path, index=False)
+    if output_path:
+        write_func(output_path=output_path, index=False)
     else:
-        text = write_func(index=False)
-        stdout_lines(text)
+        out_text = write_func(output_path=None, index=False)
+        stdout_lines(out_text)
```

### Comparing `recurtx-0.0.6/recurtx/polars.py` & `recurtx-0.0.7/recurtx/polars.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from pathlib import Path
-from typing import List
+from typing import Any, List, Optional
 
-from .utils import infer_type, stdout_lines
+import polars as pl
+
+from .utils import infer_format, stdout_lines
 
 DATA_TYPES = {
     "csv",
     "ipc",
     "parquet",
     "database",
     "json",
@@ -15,52 +17,51 @@
     "delta",
 }
 
 TRUE_VALUES = {"", "True", "true", "T", "t", "1"}
 
 
 def activate(
-    df,
-    fetch: int = None,
-    streaming: bool = None,
-):
-    df = (
+    df: pl.LazyFrame,
+    fetch: Optional[int] = None,
+    streaming: bool = False,
+) -> pl.DataFrame:
+    return (
         df.fetch(n_rows=fetch, streaming=streaming)
         if fetch
         else df.collect(streaming=streaming)
     )
-    return df
 
 
 def polars(
     *paths: str,
-    read_type: str = None,
-    columns: List[str] = None,
-    excluding_columns: List[str] = None,
-    filepath_column: str = None,
-    streaming: str = None,  # actually bool
-    fetch: int = None,
-    join: str = None,
-    on: str = None,
-    left_on: str = None,
-    right_on: str = None,
+    input_format: Optional[str] = None,
+    columns: Optional[List[str]] = None,
+    excluding_columns: Optional[List[str]] = None,
+    filepath_column: Optional[str] = None,
+    streaming: Optional[str] = None,  # actually bool
+    fetch: Optional[int] = None,
+    join: Optional[str] = None,
+    on: Optional[str] = None,
+    left_on: Optional[str] = None,
+    right_on: Optional[str] = None,
     suffix: str = "_right",
     validate: str = "m:m",
-    head: int = None,
-    tail: int = None,
-    sample: int = None,
-    method: str = None,
-    write_type: str = None,
-    write_path: str = None,
-    **kwargs,
-):
+    head: Optional[int] = None,
+    tail: Optional[int] = None,
+    sample: Optional[int] = None,
+    method: Optional[str] = None,
+    output_format: Optional[str] = None,
+    output_path: Optional[str] = None,
+    **kwargs: Any,
+) -> None:
     """Read and transform tabular files using polars."""
 
     """Workaround for unexpected behavior of Fire"""
-    kwargs.pop("read_type", None)
+    kwargs.pop("input_format", None)
     kwargs.pop("columns", None)
     kwargs.pop("excluding_columns", None)
     kwargs.pop("filepath_column", None)
     kwargs.pop("streaming", None)
     kwargs.pop("fetch", None)
     kwargs.pop("join", None)
     kwargs.pop("on", None)
@@ -68,40 +69,40 @@
     kwargs.pop("right_on", None)
     kwargs.pop("suffix", "_right")
     kwargs.pop("validate", "m:m")
     kwargs.pop("head", None)
     kwargs.pop("tail", None)
     kwargs.pop("sample", None)
     kwargs.pop("method", None)
-    kwargs.pop("write_type", None)
-    kwargs.pop("write_path", None)
+    kwargs.pop("output_format", None)
+    kwargs.pop("output_path", None)
 
-    _write_type = (
-        infer_type(write_type, write_path, DATA_TYPES.union({"markdown"}), polars=True)
+    _output_format = (
+        infer_format(
+            output_format, output_path, DATA_TYPES.union({"markdown"}), polars=True
+        )
         or "csv"
     )
 
     streaming_flag = streaming in TRUE_VALUES
 
-    import polars as pl
-
     ls = []
     for path in paths:
-        _read_type = infer_type(read_type, path, DATA_TYPES, polars=True)
-        if not _read_type:
+        _input_format = infer_format(input_format, path, DATA_TYPES, polars=True)
+        if not _input_format:
             continue
 
         _kwargs = kwargs.copy()
-        if read_type == "csv":
+        if input_format == "csv":
             _kwargs.setdefault("missing_utf8_is_empty_string", True)
             _kwargs.setdefault("infer_schema_length", 0)
 
-        read_func = getattr(pl, "scan_" + _read_type, None)
+        read_func = getattr(pl, "scan_" + _input_format, None)
         if read_func is None:
-            read_func = getattr(pl, "read_" + _read_type)
+            read_func = getattr(pl, "read_" + _input_format)
             df = read_func(path, **_kwargs).lazy()
         else:
             df = read_func(path, **_kwargs)
 
         if columns:
             df = df.select(columns)
         if excluding_columns:
@@ -114,15 +115,15 @@
         if filepath_column:
             df = df.with_columns(pl.lit(path).alias(filepath_column))
 
         ls.append(df)
 
     if not ls:
         return
-    elif len(ls) == 1:
+    if len(ls) == 1:
         df = ls[0]
     elif join is not None:
         df = ls[0]
         for right_df in ls[1:]:
             df = df.join(
                 right_df,
                 on=on,
@@ -150,34 +151,34 @@
 
     if method is not None:
         df = eval("df." + method)
 
     df = activate(df, fetch, streaming_flag)
 
     if not isinstance(df, pl.DataFrame):
-        text = "{}".format(df)
-        if write_path:
-            Path(write_path).write_text(text)
+        text = f"{df}"
+        if output_path:
+            Path(output_path).write_text(text)
         else:
             stdout_lines(text)
         return
 
-    if _write_type == "markdown":
+    if _output_format == "markdown":
 
-        def write_func(write_path: str = None):
+        def write_func(output_path: Optional[str] = None) -> Optional[str]:
             from io import StringIO
 
             import pandas as pd
 
             nonlocal df
             csv_text = df.write_csv()
             df = pd.read_csv(StringIO(csv_text), dtype=str, keep_default_na=False)
-            return df.to_markdown(write_path, index=False)
+            return df.to_markdown(output_path, index=False)
 
     else:
-        write_func = getattr(df, "write_" + _write_type)
+        write_func = getattr(df, "write_" + _output_format)
 
-    if write_path:
-        write_func(write_path)
+    if output_path:
+        write_func(output_path)
     else:
-        text = write_func()
-        stdout_lines(text)
+        out_text = write_func()
+        stdout_lines(out_text)
```

### Comparing `recurtx-0.0.6/recurtx/recur.py` & `recurtx-0.0.7/recurtx/recur.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 import re
 import sys
 from pathlib import Path
+from typing import Any, List, Tuple
 
 from .utils import get_exception_msg, subprocess_run, upath
 
 
 def recur(
     path: str,
     *scripts: str,
-    **kwargs: str,
-):
+    **kwargs: Any,
+) -> Tuple[List[str], List[str], str, bool]:
     glob = kwargs.pop("glob", "**/*")
     regex = kwargs.pop(
         "regex",
         r"^(?!.*(\.git\/|__pycache__\/|\.ipynb_checkpoints\/|\.pytest_cache\/|\.vscode\/|\.idea\/|\.DS_Store)).*$",
     )
     type = kwargs.pop("type", "file")
     sort_paths = kwargs.pop("sort_paths", "asc")
     replace_str = kwargs.pop("replace_str", "@@")
     show_paths = kwargs.pop("show_paths", False)
     show_scripts = kwargs.pop("show_scripts", False)
 
-    if regex:
-        rx = re.compile(regex)
-    else:
-        rx = None
+    rx = re.compile(regex) if regex else None
 
     script_ls = list(scripts)
     if len(kwargs) and len(script_ls) == 1:
         script_ls = script_ls[0].split(" ")
     for k, v in kwargs.items():
-        if isinstance(v, bool) and v == False:
+        if isinstance(v, bool) and not v:
             continue
         if len(k) >= 2:
             script_ls.append("--" + k)
         elif len(k) == 1:
             script_ls.append("-" + k)
         else:
-            raise NotImplementedError()
+            raise NotImplementedError
         if isinstance(v, bool):
             continue
         script_ls.append(str(v))
 
     if not script_ls:
         script_ls = ["echo"]
 
-    if replace_str and all([replace_str not in script for script in script_ls]):
+    if replace_str and all(replace_str not in script for script in script_ls):
         if len(script_ls) >= 2:
             script_ls.append(replace_str)
         else:
             script_ls[0] += " " + replace_str
 
     _path = Path(upath(path))
     assert _path.exists(), str(_path.resolve()) + " does not exist."
@@ -71,15 +69,15 @@
     return path_ls, script_ls, replace_str, show_scripts
 
 
 def under(
     path: str,
     *scripts: str,
     **kwargs: str,
-):
+) -> None:
     """Run any scripts for each file under a directory recursively."""
 
     path_ls, script_ls, replace_str, show_scripts = recur(
         path,
         *scripts,
         **kwargs,
     )
@@ -90,47 +88,49 @@
             if replace_str:
                 running_script_ls = [
                     script.replace(replace_str, p)
                     if isinstance(script, str)
                     else script
                     for script in script_ls
                 ]
+
             if len(running_script_ls) == 1:
-                running_script_ls = running_script_ls[0]
-            subprocess_run(running_script_ls, show_scripts)
+                subprocess_run(running_script_ls[0], show_scripts)
+            else:
+                subprocess_run(running_script_ls, show_scripts)
         except Exception:
             msg = get_exception_msg()
             sys.stdout.write(msg)
             continue
 
 
 def batch(
     path: str,
     *scripts: str,
     **kwargs: str,
-):
+) -> None:
     """Run any scripts for a batch of files in a directory recursively."""
 
     path_ls, script_ls, replace_str, show_scripts = recur(
         path,
         *scripts,
         **kwargs,
     )
 
-    if len(script_ls) == 1:
-        running_script_ls = script_ls[0]
-        if replace_str:
-            running_script_ls = running_script_ls.replace(
-                replace_str, " ".join(path_ls)
-            )
-    else:
-        running_script_ls = []
-        for script in script_ls:
-            if replace_str and (script == replace_str):
-                running_script_ls.extend(path_ls)
-            else:
-                running_script_ls.append(script)
     try:
-        subprocess_run(running_script_ls, show_scripts)
+        if len(script_ls) == 1:
+            running_script = script_ls[0]
+            if replace_str:
+                running_script = running_script.replace(replace_str, " ".join(path_ls))
+            subprocess_run(running_script, show_scripts)
+        else:
+            running_script_ls = []
+            for script in script_ls:
+                if replace_str and (script == replace_str):
+                    running_script_ls.extend(path_ls)
+                else:
+                    running_script_ls.append(script)
+
+            subprocess_run(running_script_ls, show_scripts)
     except Exception:
         msg = get_exception_msg()
         sys.stdout.write(msg)
```

### Comparing `recurtx-0.0.6/recurtx/search.py` & `recurtx-0.0.7/recurtx/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 import sys
 from pathlib import Path
-from typing import List, Set, Tuple, Union
+from typing import List, Optional, Set, Tuple, Union
 
 
 def run_search(
     text: str,
     target: Union[str, List, Tuple, Set],
     path: Path,
-    sub: Union[str, List, Tuple, Set] = None,
+    sub: Optional[Union[str, List, Tuple, Set]] = None,
     wildcard: str = "*",
     separator: str = "/",
     verbose: int = 1,
-):
+) -> str:
     assert isinstance(separator, str), str(separator) + ": " + str(type(separator))
 
     if isinstance(target, (list, set, tuple)):
         targets = target
     else:
         assert isinstance(target, str), str(type(target))
-        if separator:
-            targets = target.split(separator)
-        else:
-            targets = [target]
+        targets = target.split(separator) if separator else [target]
 
     if isinstance(sub, (list, tuple, set)):
         subs = sub
     elif sub is None:
         subs = [None] * len(targets)
     else:
         assert isinstance(sub, str), str(type(sub))
-        if separator:
-            subs = sub.split(separator)
-        else:
-            subs = [sub]
+        subs = sub.split(separator) if separator else [sub]
 
     assert len(targets) == len(subs), str(len(targets)) + " != " + str(len(subs))
 
     for _target, _sub in zip(targets, subs):
         target_ls = eval("'''" + _target + "'''").split(wildcard)
 
         replacing_ls = []
@@ -56,34 +50,33 @@
             if start_index and (index >= 0):
                 end_index = index
                 if _sub is not None:
                     replacing = text[start_index:end_index]
                     replacing_ls.append(replacing)
                 if verbose >= 1:
                     sys.stdout.write(
-                        f"{path} [{start_index}:{end_index}]\n{text[start_index:end_index]}\n"
+                        f"{path} [{start_index}:{end_index}]\n{text[start_index:end_index]}\n",
                     )
             else:
                 break
         for replacing in list(set(replacing_ls)):
             text = text.replace(replacing, _sub)
 
     return text
 
 
 def search(
     target: str,
     path: str,
-    sub: str = None,
+    sub: Optional[str] = None,
     wildcard: str = "*",
     separator: str = "/",
     verbose: int = 1,
-):
+) -> None:
     """Search a keyword, which may include wildcards, in the text file content, and optionally substitute (replace)."""
-
     _path = Path(path)
     try:
         text = _path.read_text()
     except Exception:
         if verbose >= 3:
             raise
         return
@@ -101,19 +94,19 @@
     if sub is not None:
         _path.write_text(text)
 
 
 def find(
     target: str,
     path: str,
-    sub: str = None,
+    sub: Optional[str] = None,
     wildcard: str = "*",
     separator: str = "/",
     verbose: int = 1,
-):
+) -> None:
     """Find a keyword, which may include wildcards, in the file path, and optionally substitute (replace)."""
 
     text = path
     _path = Path(path)
 
     text = run_search(
         text=text,
```

### Comparing `recurtx-0.0.6/recurtx/utils.py` & `recurtx-0.0.7/recurtx/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,37 +30,39 @@
         sleep(0.2)
 
     assert script, script
     shell = isinstance(script, str)
     return subprocess.run(script, shell=shell)
 
 
-def stdout_lines(text: str) -> None:
+def stdout_lines(text: Optional[str]) -> None:
+    if not text:
+        return None
     if not text.endswith("\n"):
         text += "\n"
     sys.stdout.write(text)
     return None
 
 
-def infer_type(
-    type: Optional[str],
+def infer_format(
+    format: Optional[str],
     path: Optional[str],
     supported_types: Set[str],
     polars: bool = False,
 ) -> Union[str, None]:
-    if isinstance(type, str) and type:
-        _type = type
-        _type = _type.replace("md", "markdown")
+    if isinstance(format, str) and format:
+        _format = format
+        _format = _format.replace("md", "markdown")
         if polars:
-            _type = _type.replace("jsonl", "ndjson")
-        assert _type in supported_types, (
-            _type + " not in supported set: " + str(supported_types)
+            _format = _format.replace("jsonl", "ndjson")
+        assert _format in supported_types, (
+            _format + " not in supported set: " + str(supported_types)
         )
-        return _type
-    elif isinstance(path, str) and path:
-        _type = path.split(".")[-1]
-        _type = _type.replace("md", "markdown")
+        return _format
+    if isinstance(path, str) and path:
+        _format = path.split(".")[-1]
+        _format = _format.replace("md", "markdown")
         if polars:
-            _type = _type.replace("jsonl", "ndjson")
-        if _type in supported_types:
-            return _type
+            _format = _format.replace("jsonl", "ndjson")
+        if _format in supported_types:
+            return _format
     return None
```

### Comparing `recurtx-0.0.6/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.7/recurtx.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.6
+Version: 0.0.7
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `recurtx-0.0.6/setup.py` & `recurtx-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": console_scripts},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -38,14 +38,13 @@
     author="Yusuke Minami",
     author_email="me@minyus.github.com",
     zip_safe=False,
     keywords="CLI, recursive, text, find, xargs, sed",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
 )
```

