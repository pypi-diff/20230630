# Comparing `tmp/tidypath-1.1.4.tar.gz` & `tmp/tidypath-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.1.4.tar", last modified: Tue Apr 25 10:39:25 2023, max compression
+gzip compressed data, was "tidypath-1.1.5.tar", last modified: Fri Jun 30 17:42:16 2023, max compression
```

## Comparing `tidypath-1.1.4.tar` & `tidypath-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 10:39:25.789180 tidypath-1.1.4/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-07 11:08:19.000000 tidypath-1.1.4/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2023-04-25 10:39:25.789180 tidypath-1.1.4/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2804 2022-11-25 17:30:15.000000 tidypath-1.1.4/README.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-25 10:39:25.793180 tidypath-1.1.4/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1161 2023-04-25 10:39:19.000000 tidypath-1.1.4/setup.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 10:39:25.765179 tidypath-1.1.4/tidypath/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2022-11-07 12:11:16.000000 tidypath-1.1.4/tidypath/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1629 2022-11-07 17:52:31.000000 tidypath-1.1.4/tidypath/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5054 2022-11-07 17:57:44.000000 tidypath-1.1.4/tidypath/config.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    11570 2023-04-25 10:36:09.000000 tidypath-1.1.4/tidypath/decorators.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     6075 2023-04-25 10:34:17.000000 tidypath-1.1.4/tidypath/fmt.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5197 2022-11-07 17:56:37.000000 tidypath-1.1.4/tidypath/inspection.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    13081 2023-04-25 10:34:17.000000 tidypath-1.1.4/tidypath/paths.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9844 2022-11-08 08:59:29.000000 tidypath-1.1.4/tidypath/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 10:39:25.785180 tidypath-1.1.4/tidypath.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-06-30 17:42:16.603755 tidypath-1.1.5/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.1.5/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-06-30 17:42:16.603755 tidypath-1.1.5/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.1.5/README.md
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2023-06-30 17:42:16.603755 tidypath-1.1.5/setup.cfg
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2023-06-30 17:41:03.000000 tidypath-1.1.5/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-06-30 17:42:16.600421 tidypath-1.1.5/tidypath/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/__init__.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/_helper.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5054 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/config.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    11943 2023-06-30 17:38:34.000000 tidypath-1.1.5/tidypath/decorators.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     6130 2023-06-30 17:36:32.000000 tidypath-1.1.5/tidypath/fmt.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/inspection.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    13171 2023-06-30 17:40:49.000000 tidypath-1.1.5/tidypath/paths.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.1.5/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-06-30 17:42:16.603755 tidypath-1.1.5/tidypath.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2023-06-30 17:42:16.000000 tidypath-1.1.5/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.1.4/LICENSE.md` & `tidypath-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.4/PKG-INFO` & `tidypath-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.4
+Version: 1.1.5
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.1.4/README.md` & `tidypath-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.4/setup.py` & `tidypath-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.1.4',
+    version='1.1.5',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.1.4/tidypath/_helper.py` & `tidypath-1.1.5/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.4/tidypath/config.py` & `tidypath-1.1.5/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.4/tidypath/decorators.py` & `tidypath-1.1.5/tidypath/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ._helper import merge_nested_dict
 
 
 def savedata(keys_or_function=None, include_classes="file",
              ext=config.EXT_DEFAULT_DATA, keys=config.KEYS_DEFAULT_DATA, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_DATA,
              overwrite=False, save=True, load_opts_default_save=True,  #defaults for extra arguments
              max_str_length=255,
+             iterable_maxsize=3,
              load_opts={}, **save_opts):
     """
     Decorator for automatically saving output and then loading cached data.
     Default behavior:
         1st function call:   stores the data with extension 'ext'.
         rest:                loads stored data if the key args passed to the function coincide.
 
@@ -62,14 +63,15 @@
         - ext:                     storing extension. Selects 'storage' functions save_ext, load_ext.
                                    Supported: 'lzma' (default), 'bz2', 'json', 'csv', 'npz'.
         - include_classes:         include class tree in saving_path.
         - load_opts:               kws for storage.load_ext. default kws are those of 'saving_options', those specified update saving_options dict.
         - save_opts:               kws for storage.save_ext
         - load_opts_default_save:  use save_opts as default for load_opts.
         - max_str_length:          max length of filename. If exceeded, filename is shortened by hashing it.
+        - iterable_maxsize:        max size of iterable keys. If exceeded, keys are shortened by counting val numbers.
         - rest:                    default behavior for decorated funcs extra arguments (above).
 
     Returns: Function decorator
     """
     if isinstance(keys_or_function, Iterable):
         keys = keys_or_function
         func = None
@@ -82,15 +84,15 @@
         load_opts = {**save_opts, **load_opts}
 
     def _savedata(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, funcname_in_filename=funcname_in_filename, **kwargs):
             key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
             save_keys = merge_nested_dict(key_opts, keys, key_default="all")
-            saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
+            saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
 
             filename_too_long = len(saving_path) > max_str_length
             if filename_too_long:
                 saving_path = hash_path(saving_path)
 
             if Path(saving_path).exists() and not overwrite:
                 try:
@@ -115,14 +117,15 @@
     else:
         return _savedata(func)
 
 
 def savefig(keys_or_function=None, include_classes="file",
             ext=config.EXT_DEFAULT_FIG, keys=config.KEYS_DEFAULT_FIG, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_FIG, return_fig=config.RETURN_FIG_DEFAULT,
             max_str_length=255,
+            iterable_maxsize=3,
             overwrite=True, save=True,  #defaults for extra arguments
             **save_opts):
     """
     Generates figsaver decorator.
     Figure returned by function is automatically saved. Compatible with matplotlib and plotly.
     If None or NaN is returned, avoid figure saving.
 
@@ -149,14 +152,15 @@
     Attrs:
         - function:                function to which the decorator is applied
         - ext:                     storing extension. 'eps' recommended for articles.
                                    Supported: any extension supported by matplotlib/plotly. Example: 'png', 'eps', 'html' (plotly), etc.
         - include_classes:         include class tree in saving_path.
         - save_opts:               kws for saving function.
         - max_str_length:          max length of filename. If exceeded, filename is shortened by hashing it.
+        - iterable_maxsize:        max size of iterable keys. If exceeded, keys are shortened by counting val numbers.
         - rest:                    default behavior for decorated funcs extra arguments (above).
 
     Returns: Function decorator
     """
     if isinstance(keys_or_function, Iterable):
         keys = keys_or_function
         func = None
@@ -170,15 +174,15 @@
     def _savefig(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, return_fig=return_fig, funcname_in_filename=funcname_in_filename, **kwargs):
             fig = func(*args, **kwargs)
             if isinstance(fig, (mpl_figure, plotly_figure)):
                 key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
                 save_keys = merge_nested_dict(key_opts, keys, key_default="all")
-                saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
+                saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
 
                 if len(saving_path) > max_str_length:
                     saving_path = hash_path(saving_path)
                     warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
 
                 if not Path(saving_path).exists() or overwrite:
                     if isinstance(fig, mpl_figure):
```

### Comparing `tidypath-1.1.4/tidypath/fmt.py` & `tidypath-1.1.5/tidypath/fmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,19 +60,19 @@
         except:
             return x
 
 def getopt_printer(opts):
     """Prints getopt input in a readable way."""
     print('\n'.join(f'{opt} => {arg}' for opt, arg in (("Args", "Values"), *opts)))
 
-def dict_to_id(*args, ndigits=2, join_char="_", **kwargs):
+def dict_to_id(*args, ndigits=2, join_char="_", iterable_maxsize=3, **kwargs):
     """Generate ID of the form k1-v1_k2-v2... for k_i, v_i keys and values of the dictionary d or the kwargs."""
     key_formatter = lambda k: k.replace("_", "-")
     d = args[0] if len(args) > 0 else kwargs
-    return join_char.join([f"{key_formatter(k)}-{encoder(d[k], ndigits=ndigits)}" for k in sorted(d.keys())])
+    return join_char.join([f"{key_formatter(k)}-{encoder(d[k], ndigits=ndigits, iterable_maxsize=iterable_maxsize)}" for k in sorted(d.keys())])
 
 def id_to_dict(identifier):
     """Inverse of dict_to_id."""
     s = identifier.split("/")[-1] # retain filename only
     s = os.path.splitext(s)[0] # remove extension
     d = {}
     for split in s.split("_"):
```

### Comparing `tidypath-1.1.4/tidypath/inspection.py` & `tidypath-1.1.5/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.4/tidypath/paths.py` & `tidypath-1.1.5/tidypath/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,25 @@
         else:
             class_tree = ""
     else:
         class_tree = ""
     path = os.path.join(*module.split(".")[1:], class_tree, func_name)
     return path
 
-def saving_path(Dir, ext, keys={}, subfolder="", return_dir=False, funcname_in_filename=False, **kwargs):
+def saving_path(Dir, ext, keys={}, subfolder="", return_dir=False, funcname_in_filename=False, iterable_maxsize=3, **kwargs):
     """Tree path: subfolder -> module -> (classes) -> func_name."""
     parentDir = os.path.join(Dir, subfolder, module_path(**kwargs))
     Path(parentDir).mkdir(exist_ok=True, parents=True)
     if return_dir:
         return parentDir
     else:
         if funcname_in_filename:
-            filename = parentDir.split("/")[-1] + f"_{dict_to_id(keys)}_.{ext}"
+            filename = parentDir.split("/")[-1] + f"_{dict_to_id(keys, iterable_maxsize=iterable_maxsize)}_.{ext}"
         else:
-            filename = f"{dict_to_id(keys)}_.{ext}"
+            filename = f"{dict_to_id(keys, iterable_maxsize=iterable_maxsize)}_.{ext}"
         return os.path.join(parentDir, filename)
 
 def figpath(ext="png", **kwargs):
     return saving_path(figDir, ext, **kwargs)
 
 def datapath(ext="lzma", **kwargs):
     return saving_path(dataDir, ext, **kwargs)
```

### Comparing `tidypath-1.1.4/tidypath/storage.py` & `tidypath-1.1.5/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.4/tidypath.egg-info/PKG-INFO` & `tidypath-1.1.5/tidypath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.4
+Version: 1.1.5
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

