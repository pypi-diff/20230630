# Comparing `tmp/pybind11-stubgen-0.9.tar.gz` & `tmp/pybind11-stubgen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybind11-stubgen-0.9.tar", last modified: Sat Dec  4 11:05:03 2021, max compression
+gzip compressed data, was "dist/pybind11-stubgen-0.9.1.tar", last modified: Tue Dec  7 04:43:51 2021, max compression
```

## Comparing `pybind11-stubgen-0.9.tar` & `pybind11-stubgen-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2021-12-04 11:04:17.000000 pybind11-stubgen-0.9/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      491 2021-12-04 11:04:17.000000 pybind11-stubgen-0.9/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2200 2021-12-04 11:04:17.000000 pybind11-stubgen-0.9/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      288 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/pybind11_stubgen/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2021-12-04 11:04:17.000000 pybind11-stubgen-0.9/pybind11_stubgen/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37746 2021-12-04 11:04:17.000000 pybind11-stubgen-0.9/pybind11_stubgen/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2021-12-04 11:05:03.000000 pybind11-stubgen-0.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2021-12-07 04:43:07.000000 pybind11-stubgen-0.9.1/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      493 2021-12-07 04:43:07.000000 pybind11-stubgen-0.9.1/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2200 2021-12-07 04:43:07.000000 pybind11-stubgen-0.9.1/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       17 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1817 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      288 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/pybind11_stubgen/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2021-12-07 04:43:07.000000 pybind11-stubgen-0.9.1/pybind11_stubgen/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37210 2021-12-07 04:43:07.000000 pybind11-stubgen-0.9.1/pybind11_stubgen/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1817 2021-12-07 04:43:51.000000 pybind11-stubgen-0.9.1/PKG-INFO
```

### Comparing `pybind11-stubgen-0.9/README.rst` & `pybind11-stubgen-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pybind11-stubgen-0.9/LICENSE` & `pybind11-stubgen-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybind11-stubgen-0.9/pybind11_stubgen.egg-info/PKG-INFO` & `pybind11-stubgen-0.9.1/pybind11_stubgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybind11-stubgen
-Version: 0.9
+Version: 0.9.1
 Summary: PEP 561 type stubs generator for pybind11 modules
 Home-page: https://github.com/sizmailov/pybind11-stubgen
 Maintainer: Sergei Izmailov
 Maintainer-email: sergei.a.izmailov@gmail.com
 License: BSD
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `pybind11-stubgen-0.9/pybind11_stubgen/__init__.py` & `pybind11-stubgen-0.9.1/pybind11_stubgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional, Callable, Iterator, Iterable, List, Set, Mapping, Tuple, Any, Dict
-from functools import cmp_to_key
 import ast
 import warnings
 import importlib
 import itertools
 import inspect
 import logging
 import sys
@@ -50,28 +49,27 @@
             stack.pop()
         i += 1
 
     return len(stack) == 0
 
 
 class DirectoryWalkerGuard(object):
-
     def __init__(self, dirname):
         self.dirname = dirname
+        self.origin = os.getcwd()
 
     def __enter__(self):
         if not os.path.exists(self.dirname):
-            os.mkdir(self.dirname)
+            os.makedirs(self.dirname)
 
         assert os.path.isdir(self.dirname)
-
         os.chdir(self.dirname)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        os.chdir(os.path.pardir)
+        os.chdir(self.origin)
 
 
 _default_pybind11_repr_re = re.compile(r'(<(?P<class>\w+(\.\w+)*) object at 0x[0-9a-fA-F]+>)|'
                                        r'(<(?P<enum>\w+(.\w+)*): \d+>)')
 
 
 def replace_default_pybind11_repr(line):
@@ -226,15 +224,15 @@
 class StubsGenerator(object):
     INDENT = " " * 4
 
     GLOBAL_CLASSNAME_REPLACEMENTS = {
         re.compile(
             r"numpy.ndarray\[(?P<type>[^\[\]]+)(\[(?P<shape>[^\[\]]+)\])?(?P<extra>[^][]*)\]"): replace_numpy_array,
         re.compile(
-            r"(?<!\w)(?P<type>Callable|Dict|[Ii]terator|[Ii]terable|List|Optional|Set|Tuple|Union')(?!\w)"): replace_typing_types
+            r"(?<!\w)(?P<type>Callable|Dict|[Ii]terator|[Ii]terable|List|Optional|Set|Tuple|Union)(?!\w)"): replace_typing_types
     }
 
     def parse(self):
         raise NotImplementedError
 
     def to_lines(self):  # type: () -> List[str]
         raise NotImplementedError
@@ -841,18 +839,14 @@
         return result
 
     @property
     def short_name(self):
         return self.module.__name__.split(".")[-1]
 
     def write(self):
-        if not os.path.exists(self.short_name + self.stub_suffix):
-            logger.debug("mkdir `%s`" % (self.short_name + self.stub_suffix))
-            os.mkdir(self.short_name + self.stub_suffix)
-
         with DirectoryWalkerGuard(self.short_name + self.stub_suffix):
             with open("__init__.pyi", "w") as init_pyi:
                 init_pyi.write("\n".join(self.to_lines()))
             for m in self.submodules:
                 m.write()
 
             if self.write_setup_py:
@@ -879,24 +873,14 @@
     packages=['{package_name}-stubs'],
     # PEP 561 requires these
     install_requires=['{package_name}'],
     package_data=find_stubs('{package_name}-stubs'),
 )""".format(package_name=self.short_name))
 
 
-def recursive_mkdir_walker(subdirs, callback):  # type: (List[str], Callable) -> None
-    if len(subdirs) == 0:
-        callback()
-    else:
-        if not os.path.exists(subdirs[0]):
-            os.mkdir(subdirs[0])
-        with DirectoryWalkerGuard(subdirs[0]):
-            recursive_mkdir_walker(subdirs[1:], callback)
-
-
 def main(args=None):
     parser = ArgumentParser(prog='pybind11-stubgen', description="Generates stubs for specified modules")
     parser.add_argument("-o", "--output-dir", help="the root directory for output stubs", default="./stubs")
     parser.add_argument("--root-module-suffix", type=str, default="-stubs", dest='root_module_suffix',
                         help="optional suffix to disambiguate from the original package")
     parser.add_argument("--root_module_suffix", type=str, default=None, dest='root_module_suffix_deprecated',
                         help="Deprecated.  Use `--root-module-suffix`")
@@ -942,27 +926,25 @@
 
     logging.basicConfig(
         level=logging.getLevelName(sys_args.log_level),
         format='[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s',
         handlers=handlers
     )
 
-    output_path = sys_args.output_dir
-
-    if not os.path.exists(output_path):
-        os.mkdir(output_path)
-
-    with DirectoryWalkerGuard(output_path):
+    with DirectoryWalkerGuard(sys_args.output_dir):
         for _module_name in sys_args.module_names:
             _module = ModuleStubsGenerator(_module_name)
             _module.parse()
             if FunctionSignature.n_fatal_errors() == 0:
                 _module.stub_suffix = sys_args.root_module_suffix
                 _module.write_setup_py = not sys_args.no_setup_py
-                recursive_mkdir_walker(_module_name.split(".")[:-1], lambda: _module.write())
+                _dir = _module_name.split(".")[:-1] or ["."]
+                _dir = os.path.join(*_dir)
+                with DirectoryWalkerGuard(_dir):
+                    _module.write()
 
         if FunctionSignature.n_invalid_signatures > 0:
             logger.info("Useful link: Avoiding C++ types in docstrings:")
             logger.info("      https://pybind11.readthedocs.io/en/latest/advanced/misc.html"
                         "#avoiding-cpp-types-in-docstrings")
 
         if FunctionSignature.n_invalid_default_values > 0:
```

### Comparing `pybind11-stubgen-0.9/PKG-INFO` & `pybind11-stubgen-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybind11-stubgen
-Version: 0.9
+Version: 0.9.1
 Summary: PEP 561 type stubs generator for pybind11 modules
 Home-page: https://github.com/sizmailov/pybind11-stubgen
 Maintainer: Sergei Izmailov
 Maintainer-email: sergei.a.izmailov@gmail.com
 License: BSD
 Platform: UNKNOWN
 License-File: LICENSE
```

