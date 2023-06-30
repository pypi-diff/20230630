# Comparing `tmp/yaml2dataclass-0.3.1.tar.gz` & `tmp/yaml2dataclass-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yaml2dataclass-0.3.1.tar", last modified: Fri May 29 06:03:19 2020, max compression
+gzip compressed data, was "yaml2dataclass-0.3.3.tar", last modified: Fri Jun 30 16:02:56 2023, max compression
```

## Comparing `yaml2dataclass-0.3.1.tar` & `yaml2dataclass-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,14 @@
-drwxr-xr-x   0 gandalf   (1000) gandalf   (1000)        0 2020-05-29 06:03:19.601215 yaml2dataclass-0.3.1/
--rw-r--r--   0 gandalf   (1000) gandalf   (1000)      671 2020-05-29 06:03:19.601215 yaml2dataclass-0.3.1/PKG-INFO
--rw-r--r--   0 gandalf   (1000) gandalf   (1000)      935 2020-05-29 05:56:39.898693 yaml2dataclass-0.3.1/setup.py
-drwxr-xr-x   0 gandalf   (1000) gandalf   (1000)        0 2020-05-29 06:03:19.601215 yaml2dataclass-0.3.1/yaml2dataclass/
--rw-r--r--   0 gandalf   (1000) gandalf   (1000)     2888 2020-05-29 05:56:39.898693 yaml2dataclass-0.3.1/yaml2dataclass/__init__.py
--rw-r--r--   0 gandalf   (1000) gandalf   (1000)      111 2020-05-29 06:02:52.405702 yaml2dataclass-0.3.1/yaml2dataclass/version.py
+drwxrwxr-x   0 gandalf  (20000) gandalf  (20000)        0 2023-06-30 16:02:56.861825 yaml2dataclass-0.3.3/
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)    11357 2023-06-30 15:57:30.000000 yaml2dataclass-0.3.3/LICENSE
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)      663 2023-06-30 16:02:56.861825 yaml2dataclass-0.3.3/PKG-INFO
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)      101 2023-06-30 15:57:30.000000 yaml2dataclass-0.3.3/README.md
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)       38 2023-06-30 16:02:56.861825 yaml2dataclass-0.3.3/setup.cfg
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)     1004 2023-06-30 16:00:39.000000 yaml2dataclass-0.3.3/setup.py
+drwxrwxr-x   0 gandalf  (20000) gandalf  (20000)        0 2023-06-30 16:02:56.861825 yaml2dataclass-0.3.3/yaml2dataclass/
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)     2888 2023-06-30 15:57:30.000000 yaml2dataclass-0.3.3/yaml2dataclass/__init__.py
+drwxrwxr-x   0 gandalf  (20000) gandalf  (20000)        0 2023-06-30 16:02:56.861825 yaml2dataclass-0.3.3/yaml2dataclass.egg-info/
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)      663 2023-06-30 16:02:56.000000 yaml2dataclass-0.3.3/yaml2dataclass.egg-info/PKG-INFO
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)      242 2023-06-30 16:02:56.000000 yaml2dataclass-0.3.3/yaml2dataclass.egg-info/SOURCES.txt
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)        1 2023-06-30 16:02:56.000000 yaml2dataclass-0.3.3/yaml2dataclass.egg-info/dependency_links.txt
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)        7 2023-06-30 16:02:56.000000 yaml2dataclass-0.3.3/yaml2dataclass.egg-info/requires.txt
+-rw-rw-r--   0 gandalf  (20000) gandalf  (20000)       15 2023-06-30 16:02:56.000000 yaml2dataclass-0.3.3/yaml2dataclass.egg-info/top_level.txt
```

### Comparing `yaml2dataclass-0.3.1/PKG-INFO` & `yaml2dataclass-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: yaml2dataclass
-Version: 0.3.1
+Version: 0.3.3
 Summary: Load type annotated dataclasses from YAML files.
 Home-page: https://github.com/nagylzs/yaml2dataclass
 Author: László Zsolt Nagy
 Author-email: nagylzs@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
-Description: A little helper class that lets you load type annotated dataclasses from YAML files. Supports nested data structures.
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
+License-File: LICENSE
+
+A little helper class that lets you load type annotated dataclasses from YAML files. Supports nested data structures.
```

### Comparing `yaml2dataclass-0.3.1/setup.py` & `yaml2dataclass-0.3.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 #!/usr/bin/env python
 from distutils.core import setup
-from yaml2dataclass.version import release
+
+MAJOR = 0
+MINOR = 3
+BUILD = 3
+
+version = "%s.%s" % (MAJOR, MINOR)
+release = "%s.%s.%s" % (MAJOR, MINOR, BUILD)
 
 setup(name='yaml2dataclass',
       version=release,
       description='Load type annotated dataclasses from YAML files.',
       long_description="A little helper class that lets you load type annotated dataclasses from YAML files. "
                        "Supports nested data structures.",
       author='László Zsolt Nagy',
```

### Comparing `yaml2dataclass-0.3.1/yaml2dataclass/__init__.py` & `yaml2dataclass-0.3.3/yaml2dataclass/__init__.py`

 * *Files identical despite different names*

