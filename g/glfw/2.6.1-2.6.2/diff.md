# Comparing `tmp/glfw-2.6.1.tar.gz` & `tmp/glfw-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glfw-2.6.1.tar", last modified: Mon Jun 26 18:43:34 2023, max compression
+gzip compressed data, was "glfw-2.6.2.tar", last modified: Fri Jun 30 18:32:45 2023, max compression
```

## Comparing `glfw-2.6.1.tar` & `glfw-2.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:43:34.533474 glfw-2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     3494 2023-06-26 18:43:21.000000 glfw-2.6.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-26 18:43:21.000000 glfw-2.6.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-26 18:43:21.000000 glfw-2.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5312 2023-06-26 18:43:34.533474 glfw-2.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4596 2023-06-26 18:43:21.000000 glfw-2.6.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:43:34.532474 glfw-2.6.1/glfw/
--rw-rw-rw-   0 root         (0) root         (0)    19575 2023-06-26 18:43:21.000000 glfw-2.6.1/glfw/GLFW.py
--rw-rw-rw-   0 root         (0) root         (0)   115553 2023-06-26 18:43:21.000000 glfw-2.6.1/glfw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7054 2023-06-26 18:43:21.000000 glfw-2.6.1/glfw/library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 18:43:34.533474 glfw-2.6.1/glfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5312 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 18:43:34.000000 glfw-2.6.1/glfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 18:43:34.534474 glfw-2.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-06-26 18:43:21.000000 glfw-2.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 18:32:45.110782 glfw-2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3591 2023-06-30 18:32:33.000000 glfw-2.6.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-30 18:32:33.000000 glfw-2.6.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-30 18:32:33.000000 glfw-2.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5343 2023-06-30 18:32:45.110782 glfw-2.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4627 2023-06-30 18:32:33.000000 glfw-2.6.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 18:32:45.108782 glfw-2.6.2/glfw/
+-rw-rw-rw-   0 root         (0) root         (0)    19575 2023-06-30 18:32:33.000000 glfw-2.6.2/glfw/GLFW.py
+-rw-rw-rw-   0 root         (0) root         (0)   115553 2023-06-30 18:32:33.000000 glfw-2.6.2/glfw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8956 2023-06-30 18:32:33.000000 glfw-2.6.2/glfw/library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 18:32:45.109783 glfw-2.6.2/glfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5343 2023-06-30 18:32:45.000000 glfw-2.6.2/glfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-30 18:32:45.000000 glfw-2.6.2/glfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 18:32:45.000000 glfw-2.6.2/glfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-30 18:32:45.000000 glfw-2.6.2/glfw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-30 18:32:45.000000 glfw-2.6.2/glfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 18:32:45.110782 glfw-2.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-06-30 18:32:33.000000 glfw-2.6.2/setup.py
```

### Comparing `glfw-2.6.1/CHANGELOG.md` & `glfw-2.6.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 For information on changes in GLFW itself, see the [GLFW version history](https://www.glfw.org/changelog.html).
 
+## [2.6.2] - 2023-06-30
+- Implemented search for GLFW library specific to frozen executables
+
 ## [2.6.1] - 2023-06-23
 - Revert changes made in 2.6.0
-- Do not search for GLFW library when running in a frozen library
+- Do not search for GLFW library when running in a frozen executable
 
 ## [2.6.0] - 2023-06-23
 - Use multiprocessing for library version detection on non-Windows systems
 
 ## [2.5.9] - 2023-04-01
 - Fixed package version in CHANGELOG.md and glfw/__init__.py
```

### Comparing `glfw-2.6.1/LICENSE.txt` & `glfw-2.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glfw-2.6.1/PKG-INFO` & `glfw-2.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glfw
-Version: 2.6.1
+Version: 2.6.2
 Summary: A ctypes-based wrapper for GLFW3.
 Home-page: https://github.com/FlorianRhiem/pyGLFW
 Author: Florian Rhiem
 Author-email: florian.rhiem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,17 +93,18 @@
 pyGLFW will search for the library in a list of search paths (including those
 in ``LD_LIBRARY_PATH``). If you want to use a specific library, you can set
 the ``PYGLFW_LIBRARY`` environment variable to its path.
 
 cx_Freeze / PyInstaller
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-pyGLFW is unable to dynamically search for the GLFW library on non-Windows platforms if
-running in an executable frozen with cx_Freeze or PyInstaller, so a path to the library
-must be provided using the ``PYGLFW_LIBRARY`` environment variable.
+pyGLFW will search for the GLFW library in the current working directory, the directory
+of the executable and in the package on non-Windows platforms if running in an
+executable frozen with cx_Freeze or PyInstaller, unless the ``PYGLFW_LIBRARY``
+environment variable is set.
 
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 If you are using the development version of GLFW and would like to use wrappers
 for currently unreleased macros and functions, you can instead install:
```

### Comparing `glfw-2.6.1/README.rst` & `glfw-2.6.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,18 @@
 pyGLFW will search for the library in a list of search paths (including those
 in ``LD_LIBRARY_PATH``). If you want to use a specific library, you can set
 the ``PYGLFW_LIBRARY`` environment variable to its path.
 
 cx_Freeze / PyInstaller
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-pyGLFW is unable to dynamically search for the GLFW library on non-Windows platforms if
-running in an executable frozen with cx_Freeze or PyInstaller, so a path to the library
-must be provided using the ``PYGLFW_LIBRARY`` environment variable.
+pyGLFW will search for the GLFW library in the current working directory, the directory
+of the executable and in the package on non-Windows platforms if running in an
+executable frozen with cx_Freeze or PyInstaller, unless the ``PYGLFW_LIBRARY``
+environment variable is set.
 
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 If you are using the development version of GLFW and would like to use wrappers
 for currently unreleased macros and functions, you can instead install:
```

### Comparing `glfw-2.6.1/glfw/GLFW.py` & `glfw-2.6.2/glfw/GLFW.py`

 * *Files identical despite different names*

### Comparing `glfw-2.6.1/glfw/__init__.py` & `glfw-2.6.2/glfw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import print_function
 from __future__ import division
 from __future__ import unicode_literals
 
 __author__ = 'Florian Rhiem (florian.rhiem@gmail.com)'
 __copyright__ = 'Copyright (c) 2013-2023 Florian Rhiem'
 __license__ = 'MIT'
-__version__ = '2.6.1'
+__version__ = '2.6.2'
 
 # By default, GLFW errors will be handled by a pre-defined error callback.
 # Depending on the value of ERROR_REPORTING, this callback will:
 # - Raise a GLFWError exception, if ERROR_REPORTING is 'raise', 'exception'
 #   or True.
 # - Issue a GLFWError warning, if ERROR_REPORTING is 'warn' or 'warning'.
 # - Log on debug level using the 'glfw' logger, if ERROR_REPORTING is 'log'.
```

### Comparing `glfw-2.6.1/glfw/library.py` & `glfw-2.6.2/glfw/library.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,60 +16,95 @@
 
 def _find_library_candidates(library_names,
                              library_file_extensions,
                              library_search_paths):
     """
     Finds and returns filenames which might be the library you are looking for.
     """
-    candidates = set()
-    for library_name in library_names:
-        for search_path in library_search_paths:
-            glob_query = os.path.join(search_path, '*'+library_name+'*')
+    candidates = []
+    for search_path in library_search_paths:
+        if not search_path:
+            continue
+        for library_name in library_names:
+            glob_query = os.path.join(search_path, '*'+library_name+'.*')
             for filename in glob.iglob(glob_query):
                 filename = os.path.realpath(filename)
                 if filename in candidates:
                     continue
                 basename = os.path.basename(filename)
                 if basename.startswith('lib'+library_name):
                     basename_end = basename[len('lib'+library_name):]
                 elif basename.startswith(library_name):
                     basename_end = basename[len(library_name):]
                 else:
                     continue
                 for file_extension in library_file_extensions:
                     if basename_end.startswith(file_extension):
                         if basename_end[len(file_extension):][:1] in ('', '.'):
-                            candidates.add(filename)
-                    if basename_end.endswith(file_extension):
+                            candidates.append(filename)
+                    elif basename_end.endswith(file_extension):
                         basename_middle = basename_end[:-len(file_extension)]
                         if all(c in '0123456789.' for c in basename_middle):
-                            candidates.add(filename)
+                            candidates.append(filename)
     return candidates
 
 
 def _load_library(library_names, library_file_extensions,
                   library_search_paths, version_check_callback):
     """
     Finds, loads and returns the most recent version of the library.
     """
     candidates = _find_library_candidates(library_names,
                                           library_file_extensions,
                                           library_search_paths)
     library_versions = []
-    for filename in candidates:
+    for filename in set(candidates):
         version = version_check_callback(filename)
         if version is not None and version >= (3, 0, 0):
             library_versions.append((version, filename))
 
     if not library_versions:
         return None
     library_versions.sort()
     return ctypes.CDLL(library_versions[-1][1])
 
 
+def _load_first_library(library_names, library_file_extensions,
+                        library_search_paths):
+    """
+    Finds, loads and returns the first found version of the library.
+    """
+    candidates = _find_library_candidates(
+        library_names,
+        library_file_extensions,
+        library_search_paths
+    )
+    library = None
+    for filename in candidates:
+        if os.path.isfile(filename):
+            try:
+                library = ctypes.CDLL(filename)
+                break
+            except OSError:
+                pass
+    if library is not None:
+        major_value = ctypes.c_int(0)
+        major = ctypes.pointer(major_value)
+        minor_value = ctypes.c_int(0)
+        minor = ctypes.pointer(minor_value)
+        rev_value = ctypes.c_int(0)
+        rev = ctypes.pointer(rev_value)
+        if hasattr(library, 'glfwGetVersion'):
+            library.glfwGetVersion(major, minor, rev)
+            version = (major_value.value, minor_value.value, rev_value.value)
+            if version >= (3, 0, 0):
+                return library
+    return None
+
+
 def _glfw_get_version(filename):
     """
     Queries and returns the library version tuple or None by using a
     subprocess.
     """
     version_checker_source = '''
         import sys
@@ -136,33 +171,56 @@
         '/opt/homebrew/lib',
         '/run/current-system/sw/lib',
         '/usr/lib/x86_64-linux-gnu/',
         '/usr/lib/aarch64-linux-gnu/',
         '/usr/lib/arm-linux-gnueabihf',
     ]
 
-    if sys.platform != 'darwin':
-        # manylinux2014 wheels contain libraries built for X11 and Wayland
-        if os.environ.get('PYGLFW_LIBRARY_VARIANT', '').lower() in ['wayland', 'x11']:
-            search_paths.insert(1, os.path.join(package_path, os.environ['PYGLFW_LIBRARY_VARIANT'].lower()))
-        elif os.environ.get('XDG_SESSION_TYPE') == 'wayland':
-            search_paths.insert(1, os.path.join(package_path, 'wayland'))
-        else:
-            # X11 is the default, even if XDG_SESSION_TYPE is not set
-            search_paths.insert(1, os.path.join(package_path, 'x11'))
+    package_path_variant = _get_package_path_variant(package_path)
+    if package_path_variant:
+        search_paths.insert(1, package_path_variant)
 
     if sys.platform == 'darwin':
         path_environment_variable = 'DYLD_LIBRARY_PATH'
     else:
         path_environment_variable = 'LD_LIBRARY_PATH'
     if path_environment_variable in os.environ:
         search_paths.extend(os.environ[path_environment_variable].split(':'))
     return search_paths
 
 
+def _get_frozen_library_search_paths():
+    """
+    Returns a list of library search paths for frozen executables.
+    """
+    current_path = os.path.abspath(os.getcwd())
+    executable_path = os.path.abspath(os.path.dirname(sys.executable))
+    package_path = os.path.abspath(os.path.dirname(__file__))
+    package_path_variant = _get_package_path_variant(package_path)
+    return [
+        executable_path,
+        package_path_variant,
+        package_path,
+        current_path
+    ]
+
+
+def _get_package_path_variant(package_path):
+    if sys.platform in ('darwin', 'win32'):
+        return None
+    # manylinux2014 wheels contain libraries built for X11 and Wayland
+    if os.environ.get('PYGLFW_LIBRARY_VARIANT', '').lower() in ['wayland', 'x11']:
+        return os.path.join(package_path, os.environ['PYGLFW_LIBRARY_VARIANT'].lower())
+    elif os.environ.get('XDG_SESSION_TYPE') == 'wayland':
+        return os.path.join(package_path, 'wayland')
+    else:
+        # X11 is the default, even if XDG_SESSION_TYPE is not set
+        return os.path.join(package_path, 'x11')
+
+
 if os.environ.get('PYGLFW_LIBRARY', ''):
     try:
         glfw = ctypes.CDLL(os.environ['PYGLFW_LIBRARY'])
     except OSError:
         glfw = None
 elif sys.platform == 'win32':
     glfw = None  # Will become `not None` on success.
@@ -192,8 +250,10 @@
             glfw = ctypes.CDLL(os.path.join(sys.prefix, 'Library', 'bin', 'glfw3.dll'))
         except OSError:
             pass
 elif not getattr(sys, "frozen", False):
     glfw = _load_library(['glfw', 'glfw3'], ['.so', '.dylib'],
                           _get_library_search_paths(), _glfw_get_version)
 else:
-    glfw = None
+
+    glfw = _load_first_library(['glfw', 'glfw3'], ['.so', '.dylib'],
+                               _get_frozen_library_search_paths())
```

### Comparing `glfw-2.6.1/glfw.egg-info/PKG-INFO` & `glfw-2.6.2/glfw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glfw
-Version: 2.6.1
+Version: 2.6.2
 Summary: A ctypes-based wrapper for GLFW3.
 Home-page: https://github.com/FlorianRhiem/pyGLFW
 Author: Florian Rhiem
 Author-email: florian.rhiem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,17 +93,18 @@
 pyGLFW will search for the library in a list of search paths (including those
 in ``LD_LIBRARY_PATH``). If you want to use a specific library, you can set
 the ``PYGLFW_LIBRARY`` environment variable to its path.
 
 cx_Freeze / PyInstaller
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-pyGLFW is unable to dynamically search for the GLFW library on non-Windows platforms if
-running in an executable frozen with cx_Freeze or PyInstaller, so a path to the library
-must be provided using the ``PYGLFW_LIBRARY`` environment variable.
+pyGLFW will search for the GLFW library in the current working directory, the directory
+of the executable and in the package on non-Windows platforms if running in an
+executable frozen with cx_Freeze or PyInstaller, unless the ``PYGLFW_LIBRARY``
+environment variable is set.
 
 Development Version
 ~~~~~~~~~~~~~~~~~~~
 
 If you are using the development version of GLFW and would like to use wrappers
 for currently unreleased macros and functions, you can instead install:
```

### Comparing `glfw-2.6.1/setup.py` & `glfw-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(setup_directory, 'README.rst')) as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='glfw',
-    version='2.6.1',
+    version='2.6.2',
     description='A ctypes-based wrapper for GLFW3.',
     long_description=long_description,
     url='https://github.com/FlorianRhiem/pyGLFW',
     author='Florian Rhiem',
     author_email='florian.rhiem@gmail.com',
     license='MIT',
     classifiers=[
```

