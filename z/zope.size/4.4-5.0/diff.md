# Comparing `tmp/zope.size-4.4.tar.gz` & `tmp/zope.size-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.size-4.4.tar", last modified: Tue Aug 30 06:27:44 2022, max compression
+gzip compressed data, was "zope.size-5.0.tar", last modified: Fri Jun 30 06:23:56 2023, max compression
```

## Comparing `zope.size-4.4.tar` & `zope.size-5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-30 06:27:44.265017 zope.size-4.4/
--rw-r--r--   0 mac        (513) staff       (20)     1345 2022-08-30 06:27:42.000000 zope.size-4.4/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-08-30 06:27:42.000000 zope.size-4.4/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-08-30 06:27:42.000000 zope.size-4.4/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-08-30 06:27:42.000000 zope.size-4.4/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      344 2022-08-30 06:27:42.000000 zope.size-4.4/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4105 2022-08-30 06:27:44.265146 zope.size-4.4/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1386 2022-08-30 06:27:42.000000 zope.size-4.4/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       97 2022-08-30 06:27:42.000000 zope.size-4.4/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)       87 2022-08-30 06:27:42.000000 zope.size-4.4/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-30 06:27:44.260417 zope.size-4.4/docs/
--rw-r--r--   0 mac        (513) staff       (20)     6770 2022-08-30 06:27:42.000000 zope.size-4.4/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      189 2022-08-30 06:27:42.000000 zope.size-4.4/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-08-30 06:27:42.000000 zope.size-4.4/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)     9154 2022-08-30 06:27:42.000000 zope.size-4.4/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      182 2022-08-30 06:27:42.000000 zope.size-4.4/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      446 2022-08-30 06:27:44.265808 zope.size-4.4/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3190 2022-08-30 06:27:42.000000 zope.size-4.4/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-30 06:27:44.253499 zope.size-4.4/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-30 06:27:44.260782 zope.size-4.4/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-08-30 06:27:42.000000 zope.size-4.4/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-30 06:27:44.264753 zope.size-4.4/src/zope/size/
--rw-r--r--   0 mac        (513) staff       (20)     2039 2022-08-30 06:27:42.000000 zope.size-4.4/src/zope/size/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      388 2022-08-30 06:27:42.000000 zope.size-4.4/src/zope/size/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     1460 2022-08-30 06:27:42.000000 zope.size-4.4/src/zope/size/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     4346 2022-08-30 06:27:42.000000 zope.size-4.4/src/zope/size/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-30 06:27:44.263427 zope.size-4.4/src/zope.size.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4105 2022-08-30 06:27:43.000000 zope.size-4.4/src/zope.size.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      616 2022-08-30 06:27:44.000000 zope.size-4.4/src/zope.size.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-30 06:27:43.000000 zope.size-4.4/src/zope.size.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-30 06:27:43.000000 zope.size-4.4/src/zope.size.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-30 06:27:43.000000 zope.size-4.4/src/zope.size.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      224 2022-08-30 06:27:43.000000 zope.size-4.4/src/zope.size.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-30 06:27:44.000000 zope.size-4.4/src/zope.size.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1635 2022-08-30 06:27:42.000000 zope.size-4.4/tox.ini
--rw-r--r--   0 mac        (513) staff       (20)        4 2022-08-30 06:27:42.000000 zope.size-4.4/version.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:23:56.451599 zope.size-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)     1455 2023-06-30 06:23:55.000000 zope.size-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-06-30 06:23:55.000000 zope.size-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-06-30 06:23:55.000000 zope.size-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-06-30 06:23:55.000000 zope.size-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      344 2023-06-30 06:23:55.000000 zope.size-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     4071 2023-06-30 06:23:56.451742 zope.size-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1386 2023-06-30 06:23:55.000000 zope.size-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       97 2023-06-30 06:23:55.000000 zope.size-5.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)       87 2023-06-30 06:23:55.000000 zope.size-5.0/doc-requirements.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:23:56.447520 zope.size-5.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     6770 2023-06-30 06:23:55.000000 zope.size-5.0/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)      189 2023-06-30 06:23:55.000000 zope.size-5.0/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-06-30 06:23:55.000000 zope.size-5.0/docs/changelog.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9154 2023-06-30 06:23:55.000000 zope.size-5.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)      182 2023-06-30 06:23:55.000000 zope.size-5.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)      447 2023-06-30 06:23:56.452420 zope.size-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     3078 2023-06-30 06:23:55.000000 zope.size-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:23:56.441850 zope.size-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:23:56.447858 zope.size-5.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-06-30 06:23:55.000000 zope.size-5.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:23:56.451327 zope.size-5.0/src/zope/size/
+-rw-r--r--   0 mac        (513) staff       (20)     2031 2023-06-30 06:23:55.000000 zope.size-5.0/src/zope/size/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      388 2023-06-30 06:23:55.000000 zope.size-5.0/src/zope/size/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     1460 2023-06-30 06:23:55.000000 zope.size-5.0/src/zope/size/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     4298 2023-06-30 06:23:55.000000 zope.size-5.0/src/zope/size/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:23:56.450070 zope.size-5.0/src/zope.size.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     4071 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      616 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      224 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-06-30 06:23:56.000000 zope.size-5.0/src/zope.size.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1611 2023-06-30 06:23:55.000000 zope.size-5.0/tox.ini
+-rw-r--r--   0 mac        (513) staff       (20)        4 2023-06-30 06:23:55.000000 zope.size-5.0/version.txt
```

### Comparing `zope.size-4.4/CHANGES.rst` & `zope.size-5.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changes
 =======
 
+5.0 (2023-06-30)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-08-30)
 ----------------
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.8, 3.9, 3.10.
```

### Comparing `zope.size-4.4/CONTRIBUTING.md` & `zope.size-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/LICENSE.txt` & `zope.size-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/PKG-INFO` & `zope.size-5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: zope.size
-Version: 4.4
+Version: 5.0
 Summary: Interfaces and simple adapter that give the size of an object
 Home-page: http://github.com/zopefoundation/zope.size
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: size display human bytes
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: zcml
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ===============
  ``zope.size``
@@ -65,14 +62,22 @@
 
 Documentation is hosted at https://zopesize.readthedocs.io
 
 
 Changes
 =======
 
+5.0 (2023-06-30)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-08-30)
 ----------------
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.8, 3.9, 3.10.
 
@@ -138,9 +143,7 @@
 
 - Change package's url to PyPI instead of Subversion.
 
 3.4.0 (2006-09-29)
 ------------------
 
 - First release as a separate egg
-
-
```

### Comparing `zope.size-4.4/README.rst` & `zope.size-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/docs/Makefile` & `zope.size-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/docs/conf.py` & `zope.size-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/setup.py` & `zope.size-5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.size package
 """
 import os
 
@@ -42,41 +42,39 @@
     version=read('version.txt').strip(),
     url='http://github.com/zopefoundation/zope.size',
     license='ZPL 2.1',
     description='Interfaces and simple adapter that give the size of an'
                 ' object',
     keywords="size display human bytes",
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     long_description=read('README.rst') + '\n\n' + read('CHANGES.rst'),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development',
     ],
     packages=find_packages('src'),
     package_dir={
         '': 'src'},
     namespace_packages=['zope'],
+    python_requires='>=3.7',
     extras_require={
         'zcml': ZCML_REQUIRES,
         'test': TESTS_REQUIRE,
         'docs': [
             'Sphinx',
             'repoze.sphinx.autointerface',
         ],
```

### Comparing `zope.size-4.4/src/zope/size/__init__.py` & `zope.size-5.0/src/zope/size/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from zope.size.interfaces import ISized
 
 
 _ = MessageFactory('zope')
 
 
 @implementer(ISized)
-class DefaultSized(object):
+class DefaultSized:
     """
     A default :class:`zope.size.interfaces.ISized` adapter
     producing bytes for any object that has a ``getSize`` method and
     (None, None) for all other objects.
     """
 
     def __init__(self, obj):
```

### Comparing `zope.size-4.4/src/zope/size/interfaces.py` & `zope.size-5.0/src/zope/size/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/src/zope/size/tests.py` & `zope.size-5.0/src/zope/size/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test ISized Adapter
 """
-from __future__ import unicode_literals
 
 import unittest
 
 import zope.component
 import zope.configuration.xmlconfig
 
 import zope.size
@@ -44,15 +43,15 @@
         self.assertEqual(u_count + 8, len(list(gsm.registeredUtilities())))
         self.assertEqual(a_count + 1, len(list(gsm.registeredAdapters())))
         self.assertEqual(
             s_count, len(list(gsm.registeredSubscriptionAdapters())))
         self.assertEqual(h_count, len(list(gsm.registeredHandlers())))
 
 
-class DummyObject(object):
+class DummyObject:
 
     def __init__(self, size):
         self._size = size
 
     def getSize(self):
         return self._size
```

### Comparing `zope.size-4.4/src/zope.size.egg-info/PKG-INFO` & `zope.size-5.0/src/zope.size.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: zope.size
-Version: 4.4
+Version: 5.0
 Summary: Interfaces and simple adapter that give the size of an object
 Home-page: http://github.com/zopefoundation/zope.size
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: size display human bytes
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
+Requires-Python: >=3.7
 Provides-Extra: zcml
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ===============
  ``zope.size``
@@ -65,14 +62,22 @@
 
 Documentation is hosted at https://zopesize.readthedocs.io
 
 
 Changes
 =======
 
+5.0 (2023-06-30)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.4 (2022-08-30)
 ----------------
 
 - Drop support for Python 3.4.
 
 - Add support for Python 3.8, 3.9, 3.10.
 
@@ -138,9 +143,7 @@
 
 - Change package's url to PyPI instead of Subversion.
 
 3.4.0 (2006-09-29)
 ------------------
 
 - First release as a separate egg
-
-
```

### Comparing `zope.size-4.4/src/zope.size.egg-info/SOURCES.txt` & `zope.size-5.0/src/zope.size.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.size-4.4/tox.ini` & `zope.size-5.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
@@ -38,14 +35,15 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
@@ -59,25 +57,23 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
     zope.testrunner
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=100
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.size
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

