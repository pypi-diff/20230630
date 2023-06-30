# Comparing `tmp/ezregex-1.2.1.tar.gz` & `tmp/ezregex-1.3.0.tar.gz`

## Comparing `ezregex-1.2.1.tar` & `ezregex-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.2.1/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.2.1/MANIFEST.in
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 ezregex-1.2.1/README.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ezregex-1.2.1/requirements.txt
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ezregex-1.2.1/setup.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ezregex-1.2.1/todo.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.2.1/tox.ini
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 ezregex-1.2.1/ezregex/EZRegexMember.py
--rw-r--r--   0        0        0    14264 2020-02-02 00:00:00.000000 ezregex-1.2.1/ezregex/__init__.py
--rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 ezregex-1.2.1/ezregex/invert.py
--rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 ezregex-1.2.1/tests/tests.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ezregex-1.2.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.2.1/LICENSE
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ezregex-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ezregex-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.3.0/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.3.0/MANIFEST.in
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 ezregex-1.3.0/README.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ezregex-1.3.0/requirements.txt
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ezregex-1.3.0/setup.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ezregex-1.3.0/todo.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.3.0/tox.ini
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 ezregex-1.3.0/ezregex/EZRegexMember.py
+-rw-r--r--   0        0        0    14264 2020-02-02 00:00:00.000000 ezregex-1.3.0/ezregex/__init__.py
+-rw-r--r--   0        0        0    10022 2020-02-02 00:00:00.000000 ezregex-1.3.0/ezregex/invert.py
+-rw-r--r--   0        0        0    16308 2020-02-02 00:00:00.000000 ezregex-1.3.0/tests/tests.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ezregex-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.3.0/LICENSE
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ezregex-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ezregex-1.3.0/PKG-INFO
```

### Comparing `ezregex-1.2.1/README.md` & `ezregex-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ezregex-1.2.1/setup.py` & `ezregex-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.2.1/ezregex/EZRegexMember.py` & `ezregex-1.3.0/ezregex/EZRegexMember.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.2.1/ezregex/__init__.py` & `ezregex-1.3.0/ezregex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 from .EZRegexMember import EZRegexMember
 from sys import version_info
 from .invert import invertRegex as invert
 from re import RegexFlag, escape
 
 # Positional
 # wordStartsWith = EZRegexMember(lambda cur, input: input + r'\<' + cur)
```

### Comparing `ezregex-1.2.1/ezregex/invert.py` & `ezregex-1.3.0/ezregex/invert.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.2.1/tests/tests.py` & `ezregex-1.3.0/tests/tests.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.2.1/LICENSE` & `ezregex-1.3.0/LICENSE`

 * *Files identical despite different names*

