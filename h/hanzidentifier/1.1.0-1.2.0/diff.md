# Comparing `tmp/hanzidentifier-1.1.0.tar.gz` & `tmp/hanzidentifier-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hanzidentifier-1.1.0.tar", last modified: Sun Oct 16 01:18:10 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hanzidentifier-1.1.0.tar` & `hanzidentifier-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 tsr       (1000) tsr       (1000)        0 2022-10-16 01:18:10.078727 hanzidentifier-1.1.0/
--rw-r--r--   0 tsr       (1000) tsr       (1000)     1056 2022-10-13 11:59:25.000000 hanzidentifier-1.1.0/LICENSE.txt
--rw-r--r--   0 tsr       (1000) tsr       (1000)       20 2022-10-13 11:59:25.000000 hanzidentifier-1.1.0/MANIFEST.in
--rw-r--r--   0 tsr       (1000) tsr       (1000)     4378 2022-10-16 01:18:10.078727 hanzidentifier-1.1.0/PKG-INFO
--rw-r--r--   0 tsr       (1000) tsr       (1000)     3641 2022-10-16 01:17:53.000000 hanzidentifier-1.1.0/README.rst
-drwxr-xr-x   0 tsr       (1000) tsr       (1000)        0 2022-10-16 01:18:10.078727 hanzidentifier-1.1.0/hanzidentifier.egg-info/
--rw-r--r--   0 tsr       (1000) tsr       (1000)     4378 2022-10-16 01:18:10.000000 hanzidentifier-1.1.0/hanzidentifier.egg-info/PKG-INFO
--rw-r--r--   0 tsr       (1000) tsr       (1000)      267 2022-10-16 01:18:10.000000 hanzidentifier-1.1.0/hanzidentifier.egg-info/SOURCES.txt
--rw-r--r--   0 tsr       (1000) tsr       (1000)        1 2022-10-16 01:18:10.000000 hanzidentifier-1.1.0/hanzidentifier.egg-info/dependency_links.txt
--rw-r--r--   0 tsr       (1000) tsr       (1000)       12 2022-10-16 01:18:10.000000 hanzidentifier-1.1.0/hanzidentifier.egg-info/requires.txt
--rw-r--r--   0 tsr       (1000) tsr       (1000)       15 2022-10-16 01:18:10.000000 hanzidentifier-1.1.0/hanzidentifier.egg-info/top_level.txt
--rw-r--r--   0 tsr       (1000) tsr       (1000)     3174 2022-10-16 01:15:43.000000 hanzidentifier-1.1.0/hanzidentifier.py
--rw-r--r--   0 tsr       (1000) tsr       (1000)       18 2022-10-16 00:57:27.000000 hanzidentifier-1.1.0/requirements.txt
--rw-r--r--   0 tsr       (1000) tsr       (1000)       38 2022-10-16 01:18:10.078727 hanzidentifier-1.1.0/setup.cfg
--rw-r--r--   0 tsr       (1000) tsr       (1000)     1095 2022-10-16 01:17:53.000000 hanzidentifier-1.1.0/setup.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/src/hanzidentifier/__init__.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/src/hanzidentifier/core.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/src/hanzidentifier/helpers.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/README.rst
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 hanzidentifier-1.2.0/PKG-INFO
```

### Comparing `hanzidentifier-1.1.0/LICENSE.txt` & `hanzidentifier-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hanzidentifier-1.1.0/PKG-INFO` & `hanzidentifier-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 Metadata-Version: 2.1
 Name: hanzidentifier
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python module that identifies Chinese text as Simplified or Traditional.
-Home-page: https://github.com/tsroten/hanzidentifier
-Author: Thomas Roten
-Author-email: thomas@roten.us
-Keywords: chinese,mandarin,hanzi,characters,simplified,traditional,identify,identification,cjk
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Changes, https://github.com/tsroten/hanzidentifier/blob/main/CHANGES.rst
+Project-URL: Issue Tracker, https://github.com/tsroten/hanzidentifier/issues
+Project-URL: Source Code, https://github.com/tsroten/hanzidentifier
+Author-email: Thomas Roten <thomas@roten.us>
+License-Expression: MIT
+License-File: LICENSE.txt
+Keywords: characters,chinese,cjk,hanzi,mandarin,simplified,traditional
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
-License-File: LICENSE.txt
+Requires-Python: >=3.7
+Requires-Dist: zhon~=2.0
+Description-Content-Type: text/x-rst
 
 ================
 Hanzi Identifier
 ================
 
-.. image:: https://badge.fury.io/py/hanzidentifier.png
-    :target: http://badge.fury.io/py/hanzidentifier
-    
-.. image:: https://travis-ci.org/tsroten/hanzidentifier.png?branch=develop
-        :target: https://travis-ci.org/tsroten/hanzidentifier
+.. image:: https://badge.fury.io/py/hanzidentifier.svg
+    :target: https://pypi.org/project/hanzidentifier
+
+.. image:: https://github.com/tsroten/hanzidentifier/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/tsroten/hanzidentifier/actions/workflows/ci.yml
 
 Hanzi Identifier is a simple Python module that identifies a string of text as 
 having Simplified or Traditional characters.
 
 * GitHub: https://github.com/tsroten/hanzidentifier
 * Free software: MIT license
 
@@ -73,54 +83,16 @@
 * ``hanzidentifier.MIXED``: the string consists of characters recognized solely as Traditional characters and also consists of characters recognized solely as Simplified characters.
 
 Characters that aren't found in CC-CEDICT are ignored when determining a string's identity.
 Hanzi Identifier uses the CC-CEDICT data provided by `Zhon <https://github.com/tsroten/zhon>`_ to identify Chinese characters.
 
 Because the Traditional and Simplified Chinese character systems overlap, a
 string containing Simplified characters could identify as
-``hanzidentifer.SIMPLIFIED`` or ``hanzidentifier.BOTH`` depending on if the
+``hanzidentifier.SIMPLIFIED`` or ``hanzidentifier.BOTH`` depending on if the
 characters are also Traditional characters.
 
-Hanzi Identifier's functions accept and return unicode.
-
 Getting Started
 ---------------
 
 * Install Hanzi Identifier: ``$ pip install hanzidentifier``
 * Report bugs and ask questions via `GitHub Issues <https://github.com/tsroten/hanzidentifier/issues>`_
-* `Contribute features or bug fixes <https://github.com/tsroten/hanzidentifier/pulls>`_
-
-
-Change Log
-----------
-
-v1.1.0 (2020-10-15)
-~~~~~~~~~~~~~~~~~~~
-
-* New function: ``count_chinese()``. Thanks to ramwin.
-* Drop Python 2.
-
-v1.0.2 (2015-08-06)
-~~~~~~~~~~~~~~~~~~~
-
-* New README format
-* Adds Travis CI support
-* Uses ``io.open()`` in ``setup.py``. Fixes #1.
-
-v1.0.1 (2014-04-14)
-~~~~~~~~~~~~~~~~~~~
-
-* Fixes URL typo.
-
-v1.0 (2014-04-12)
-~~~~~~~~~~~~~~~~~
-
-Version 1.0 merges some changes from Dragon Mapper. It is not backwards compatible with
-the previous versions of Hanzi Identifier (e.g. some of the constants are named differently).
-
-* Merges code from `Dragon Mapper <http://github.com/tsroten/dragonmapper>`_ project.
-* Adds tox support.
-
-v0.1 (2013-04-24)
-~~~~~~~~~~~~~~~~~
-
-* Initial release.
+* `Contribute features or bug fixes <https://github.com/tsroten/hanzidentifier/pulls>`_
```

### Comparing `hanzidentifier-1.1.0/hanzidentifier.py` & `hanzidentifier-1.2.0/src/hanzidentifier/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 # -*- coding: utf-8 -*-
-"""Python module that identifies Chinese text as Simplified or Traditional."""
-
-from __future__ import unicode_literals
-import re
-
-from zhon import cedict
+from hanzidentifier import helpers
 
 UNKNOWN = 0
 TRAD = TRADITIONAL = 1
 SIMP = SIMPLIFIED = 2
 BOTH = 3
 MIXED = 4
 
-_TRADITIONAL_CHARACTERS = set(list(cedict.traditional))
-_SIMPLIFIED_CHARACTERS = set(list(cedict.simplified))
-_SHARED_CHARACTERS = _TRADITIONAL_CHARACTERS & _SIMPLIFIED_CHARACTERS
-_ALL_CHARACTERS = cedict.all
-HANZI_MATCH = re.compile(f"[^{_ALL_CHARACTERS}]")
-
-
-def _get_hanzi(s):
-    """Extract a string's Chinese characters."""
-    return set(HANZI_MATCH.sub("", s))
-
 
 def identify(s):
     """Identify what kind of Chinese characters a string contains.
 
     *s* is a string to examine. The string's Chinese characters are tested to
     see if they are compatible with the Traditional or Simplified characters
     systems, compatible with both, or contain a mixture of Traditional and
@@ -42,66 +26,66 @@
     string containing Simplified characters could identify as
     :data:`SIMPLIFIED` or :data:`BOTH` depending on if the characters are also
     Traditional characters. To make testing the identity of a string easier,
     the functions :func:`is_traditional`, :func:`is_simplified`, and
     :func:`has_chinese` are provided.
 
     """
-    chinese = _get_hanzi(s)
+    chinese = helpers.get_hanzi(s)
     if not chinese:
         return UNKNOWN
-    if chinese.issubset(_SHARED_CHARACTERS):
+    if chinese.issubset(helpers.SHARED_CHARACTERS):
         return BOTH
-    if chinese.issubset(_TRADITIONAL_CHARACTERS):
+    if chinese.issubset(helpers.TRADITIONAL_CHARACTERS):
         return TRADITIONAL
-    if chinese.issubset(_SIMPLIFIED_CHARACTERS):
+    if chinese.issubset(helpers.SIMPLIFIED_CHARACTERS):
         return SIMPLIFIED
     return MIXED
 
 
 def has_chinese(s):
     """Check if a string has Chinese characters in it.
 
     This is a faster version of:
         >>> identify('foo') is not UNKNOWN
 
     """
-    return bool(_get_hanzi(s))
+    return bool(helpers.get_hanzi(s))
 
 
 def is_traditional(s):
     """Check if a string's Chinese characters are Traditional.
 
     This is equivalent to:
         >>> identify('foo') in (TRADITIONAL, BOTH)
 
     """
-    chinese = _get_hanzi(s)
+    chinese = helpers.get_hanzi(s)
     if not chinese:
         return False
-    if chinese.issubset(_SHARED_CHARACTERS):
+    if chinese.issubset(helpers.SHARED_CHARACTERS):
         return True
-    if chinese.issubset(_TRADITIONAL_CHARACTERS):
+    if chinese.issubset(helpers.TRADITIONAL_CHARACTERS):
         return True
     return False
 
 
 def is_simplified(s):
     """Check if a string's Chinese characters are Simplified.
 
     This is equivalent to:
         >>> identify('foo') in (SIMPLIFIED, BOTH)
 
     """
-    chinese = _get_hanzi(s)
+    chinese = helpers.get_hanzi(s)
     if not chinese:
         return False
-    if chinese.issubset(_SHARED_CHARACTERS):
+    if chinese.issubset(helpers.SHARED_CHARACTERS):
         return True
-    if chinese.issubset(_SIMPLIFIED_CHARACTERS):
+    if chinese.issubset(helpers.SIMPLIFIED_CHARACTERS):
         return True
     return False
 
 
 def count_chinese(s: str) -> int:
     """count how many chinese exist in a string"""
     result = 0
```

