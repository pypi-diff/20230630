# Comparing `tmp/zope.site-4.6.1.tar.gz` & `tmp/zope.site-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.site-4.6.1.tar", last modified: Fri Sep  2 07:26:39 2022, max compression
+gzip compressed data, was "zope.site-5.0.tar", last modified: Fri Jun 30 06:54:49 2023, max compression
```

## Comparing `zope.site-4.6.1.tar` & `zope.site-5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.277779 zope.site-4.6.1/
--rw-r--r--   0 mac        (513) staff       (20)     6568 2022-09-02 07:26:37.000000 zope.site-4.6.1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-09-02 07:26:37.000000 zope.site-4.6.1/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-09-02 07:26:37.000000 zope.site-4.6.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-09-02 07:26:37.000000 zope.site-4.6.1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      400 2022-09-02 07:26:37.000000 zope.site-4.6.1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    19972 2022-09-02 07:26:39.277939 zope.site-4.6.1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1250 2022-09-02 07:26:37.000000 zope.site-4.6.1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      384 2022-09-02 07:26:37.000000 zope.site-4.6.1/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      295 2022-09-02 07:26:37.000000 zope.site-4.6.1/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.268997 zope.site-4.6.1/docs/
--rw-r--r--   0 mac        (513) staff       (20)     6770 2022-09-02 07:26:37.000000 zope.site-4.6.1/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      254 2022-09-02 07:26:37.000000 zope.site-4.6.1/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-09-02 07:26:37.000000 zope.site-4.6.1/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)     9933 2022-09-02 07:26:37.000000 zope.site-4.6.1/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      399 2022-09-02 07:26:37.000000 zope.site-4.6.1/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       39 2022-09-02 07:26:37.000000 zope.site-4.6.1/docs/site.rst
--rw-r--r--   0 mac        (513) staff       (20)      446 2022-09-02 07:26:39.278651 zope.site-4.6.1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3662 2022-09-02 07:26:37.000000 zope.site-4.6.1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.262296 zope.site-4.6.1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.269318 zope.site-4.6.1/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.274655 zope.site-4.6.1/src/zope/site/
--rw-r--r--   0 mac        (513) staff       (20)     1790 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2721 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     2744 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/folder.py
--rw-r--r--   0 mac        (513) staff       (20)      829 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/hooks.py
--rw-r--r--   0 mac        (513) staff       (20)     3285 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      105 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/next.py
--rw-r--r--   0 mac        (513) staff       (20)     9608 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/site.py
--rw-r--r--   0 mac        (513) staff       (20)    10709 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/site.rst
--rw-r--r--   0 mac        (513) staff       (20)     2455 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.277527 zope.site-4.6.1/src/zope/site/tests/
--rw-r--r--   0 mac        (513) staff       (20)       61 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1752 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/folder.txt
--rw-r--r--   0 mac        (513) staff       (20)     1195 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_bwc.py
--rw-r--r--   0 mac        (513) staff       (20)     1668 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_configure.py
--rw-r--r--   0 mac        (513) staff       (20)     1817 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_folder.py
--rw-r--r--   0 mac        (513) staff       (20)     1795 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_localsitemanager.py
--rw-r--r--   0 mac        (513) staff       (20)     3251 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_registration.py
--rw-r--r--   0 mac        (513) staff       (20)     5836 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_site.py
--rw-r--r--   0 mac        (513) staff       (20)     2396 2022-09-02 07:26:37.000000 zope.site-4.6.1/src/zope/site/tests/test_sitemanagercontainer.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-09-02 07:26:39.271768 zope.site-4.6.1/src/zope.site.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    19972 2022-09-02 07:26:38.000000 zope.site-4.6.1/src/zope.site.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1070 2022-09-02 07:26:39.000000 zope.site-4.6.1/src/zope.site.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-09-02 07:26:38.000000 zope.site-4.6.1/src/zope.site.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-09-02 07:26:38.000000 zope.site-4.6.1/src/zope.site.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-09-02 07:26:38.000000 zope.site-4.6.1/src/zope.site.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      324 2022-09-02 07:26:38.000000 zope.site-4.6.1/src/zope.site.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-09-02 07:26:39.000000 zope.site-4.6.1/src/zope.site.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1636 2022-09-02 07:26:37.000000 zope.site-4.6.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.212905 zope.site-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)     6678 2023-06-30 06:54:48.000000 zope.site-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-06-30 06:54:48.000000 zope.site-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-06-30 06:54:48.000000 zope.site-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-06-30 06:54:48.000000 zope.site-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      400 2023-06-30 06:54:48.000000 zope.site-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    19868 2023-06-30 06:54:49.213144 zope.site-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1250 2023-06-30 06:54:48.000000 zope.site-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      384 2023-06-30 06:54:48.000000 zope.site-5.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      295 2023-06-30 06:54:48.000000 zope.site-5.0/doc-requirements.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.203351 zope.site-5.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     6770 2023-06-30 06:54:48.000000 zope.site-5.0/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)      254 2023-06-30 06:54:48.000000 zope.site-5.0/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-06-30 06:54:48.000000 zope.site-5.0/docs/changelog.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9933 2023-06-30 06:54:48.000000 zope.site-5.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)      399 2023-06-30 06:54:48.000000 zope.site-5.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)       39 2023-06-30 06:54:48.000000 zope.site-5.0/docs/site.rst
+-rw-r--r--   0 mac        (513) staff       (20)      447 2023-06-30 06:54:49.213939 zope.site-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     3363 2023-06-30 06:54:48.000000 zope.site-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.197716 zope.site-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.203660 zope.site-5.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.209466 zope.site-5.0/src/zope/site/
+-rw-r--r--   0 mac        (513) staff       (20)     1790 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     2721 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     2736 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/folder.py
+-rw-r--r--   0 mac        (513) staff       (20)      829 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/hooks.py
+-rw-r--r--   0 mac        (513) staff       (20)     3277 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)      105 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/next.py
+-rw-r--r--   0 mac        (513) staff       (20)     9576 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/site.py
+-rw-r--r--   0 mac        (513) staff       (20)    10709 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/site.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2236 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/testing.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.212581 zope.site-5.0/src/zope/site/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       61 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1749 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/folder.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1195 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_bwc.py
+-rw-r--r--   0 mac        (513) staff       (20)     1668 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_configure.py
+-rw-r--r--   0 mac        (513) staff       (20)     1760 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_folder.py
+-rw-r--r--   0 mac        (513) staff       (20)     1825 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_localsitemanager.py
+-rw-r--r--   0 mac        (513) staff       (20)     3251 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_registration.py
+-rw-r--r--   0 mac        (513) staff       (20)     5806 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_site.py
+-rw-r--r--   0 mac        (513) staff       (20)     2388 2023-06-30 06:54:48.000000 zope.site-5.0/src/zope/site/tests/test_sitemanagercontainer.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-30 06:54:49.206263 zope.site-5.0/src/zope.site.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    19868 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1070 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      324 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-06-30 06:54:49.000000 zope.site-5.0/src/zope.site.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1612 2023-06-30 06:54:48.000000 zope.site-5.0/tox.ini
```

### Comparing `zope.site-4.6.1/CHANGES.rst` & `zope.site-5.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+5.0 (2023-06-30)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.6.1 (2022-09-02)
 ==================
 
 - Fix more deprecation warnings.
 
 
 4.6 (2022-08-23)
```

### Comparing `zope.site-4.6.1/CONTRIBUTING.md` & `zope.site-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/LICENSE.txt` & `zope.site-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/PKG-INFO` & `zope.site-5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.site
-Version: 4.6.1
+Version: 5.0
 Summary: Local registries for zope component architecture
 Home-page: http://zopesite.readthedocs.io
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope component architecture local
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
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
 Classifier: Framework :: Zope :: 3
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ===============
  ``zope.site``
 ===============
@@ -432,14 +428,22 @@
   ()
 
 
 =========
  Changes
 =========
 
+5.0 (2023-06-30)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.6.1 (2022-09-02)
 ==================
 
 - Fix more deprecation warnings.
 
 
 4.6 (2022-08-23)
@@ -658,9 +662,7 @@
 - Use zope.container instead of zope.app.container.
 
 3.5.1 (2009-01-27)
 ==================
 
 - Extracted from zope.app.component (trunk, 3.5.1 under development)
   as part of an effort to clean up dependencies between Zope packages.
-
-
```

### Comparing `zope.site-4.6.1/README.rst` & `zope.site-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/docs/Makefile` & `zope.site-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/docs/conf.py` & `zope.site-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/setup.py` & `zope.site-5.0/setup.py`

 * *Files 18% similar despite different names*

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
 """Setup for zope.site package
 """
 import os
 
@@ -36,17 +36,17 @@
     'zope.security[zcml]',
     'zope.testing',
     'zope.testrunner',
 ]
 
 setup(
     name='zope.site',
-    version='4.6.1',
+    version='5.0',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     description='Local registries for zope component architecture',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('src', 'zope', 'site', 'site.rst')
         + '\n\n' +
         read('CHANGES.rst')
@@ -54,23 +54,20 @@
     keywords="zope component architecture local",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
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
         'Framework :: Zope :: 3',
     ],
@@ -95,19 +92,11 @@
         'zope.security',
         'zope.component >= 4.5.0',
         'zope.event',
         'zope.interface >= 4.5.0',
         'zope.lifecycleevent',
         'zope.location',
     ],
-    tests_require=TESTS_REQUIRE,
     include_package_data=True,
     zip_safe=False,
-    python_requires=', '.join([
-        '>=2.7',
-        '!=3.0.*',
-        '!=3.1.*',
-        '!=3.2.*',
-        '!=3.3.*',
-        '!=3.4.*',
-    ]),
+    python_requires='>=3.7',
 )
```

### Comparing `zope.site-4.6.1/src/zope/site/__init__.py` & `zope.site-5.0/src/zope/site/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/configure.zcml` & `zope.site-5.0/src/zope/site/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/folder.py` & `zope.site-5.0/src/zope/site/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def rootFolder():
     """Factory for a :class:`zope.site.interfaces.IRootFolder`"""
     f = Folder()
     directlyProvides(f, IRootFolder)
     return f
 
 
-class FolderSublocations(object):
+class FolderSublocations:
     """
     Adapter for an :class:`zope.site.interfaces.IFolder` to
     :class:`zope.location.interfaces.ISublocations`.
 
     The subobjects of a folder include it's contents and it's site
     manager if it is a site::
```

### Comparing `zope.site-4.6.1/src/zope/site/hooks.py` & `zope.site-5.0/src/zope/site/hooks.py`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/interfaces.py` & `zope.site-5.0/src/zope/site/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class INewLocalSite(zope.interface.Interface):
     """Event: a local site was created
     """
     manager = zope.interface.Attribute("The new site manager")
 
 
 @zope.interface.implementer(INewLocalSite)
-class NewLocalSite(object):
+class NewLocalSite:
     """Event: a local site was created
     """
     def __init__(self, manager):
         self.manager = manager
 
 
 class ILocalSiteManager(zope.interface.interfaces.IComponents):
```

### Comparing `zope.site-4.6.1/src/zope/site/site.py` & `zope.site-5.0/src/zope/site/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 @zope.interface.implementer(interfaces.ISiteManagementFolder)
 class SiteManagementFolder(BTreeContainer):
     """Implementation of a :class:`~.ISiteManagementFolder`"""
 
 
 @zope.interface.implementer(IDirectoryFactory)
-class SMFolderFactory(object):
+class SMFolderFactory:
     """
     Implementation of a :class:`~.IDirectoryFactory` that creates
     :class:`SiteManagementFolder`
     """
 
     def __init__(self, context):
         self.context = context
@@ -149,15 +149,15 @@
 
         for base in bases:
             if ((base not in self.__bases__)
                     # pylint:disable=no-value-for-parameter
                     and interfaces.ILocalSiteManager.providedBy(base)):
                 base.addSub(self)
 
-        super(LocalSiteManager, self)._setBases(bases)
+        super()._setBases(bases)
 
     def __init__(self, site, default_folder=True):
         BTreeContainer.__init__(self)
         PersistentComponents.__init__(self)
 
         # Locate the site manager
         self.__parent__ = site
@@ -175,16 +175,16 @@
             zope.event.notify(ObjectCreatedEvent(folder))
             self['default'] = folder
 
     def _init_registries(self):
         self.adapters = _LocalAdapterRegistry()
         self.utilities = _LocalAdapterRegistry()
         self.adapters.__parent__ = self.utilities.__parent__ = self
-        self.adapters.__name__ = u'adapters'
-        self.utilities.__name__ = u'utilities'
+        self.adapters.__name__ = 'adapters'
+        self.utilities.__name__ = 'utilities'
 
     def _p_repr(self):
         return PersistentComponents.__repr__(self)
 
     def addSub(self, sub):
         """See :meth:`zope.site.interfaces.ILocalSiteManager.addSub`"""
         self.subs += (sub, )
```

### Comparing `zope.site-4.6.1/src/zope/site/site.rst` & `zope.site-5.0/src/zope/site/site.rst`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/testing.py` & `zope.site-5.0/src/zope/site/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,40 +9,28 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Reusable functionality for testing site-related code
 """
-import re
-
 import zope.component
 import zope.component.hooks
 import zope.component.interfaces
 import zope.container.interfaces
 import zope.container.testing
 from zope.interface import Interface
 from zope.interface.interfaces import IComponentLookup
-from zope.testing import renormalizing
 
 import zope.site.site
 from zope.site import LocalSiteManager
 from zope.site import SiteManagerAdapter
 from zope.site.folder import rootFolder
 
 
-checker = renormalizing.RENormalizing([
-    # Python 3 unicode removed the "u".
-    (re.compile("u('.*?')"),
-     r"\1"),
-    (re.compile('u(".*?")'),
-     r"\1"),
-])
-
-
 def createSiteManager(folder, setsite=False):
     if not zope.component.interfaces.ISite.providedBy(folder):
         folder.setSiteManager(LocalSiteManager(folder))
     if setsite:  # pragma: no cover
         zope.component.hooks.setSite(folder)
     return folder.getSiteManager()
```

### Comparing `zope.site-4.6.1/src/zope/site/tests/folder.txt` & `zope.site-5.0/src/zope/site/tests/folder.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 
   >>> from zope.site.folder import Folder
   >>> folder['test'] = Folder()
 
 The site folder now contains the new folder:
 
   >>> list(fs_folder.keys())
-  [u'test', '++etc++site']
+  ['test', '++etc++site']
   >>> fs_folder.get('test')
   <...Folder object at 0x...>
   >>> fs_folder['test']
   <...Folder object at 0x...>
   >>> list(fs_folder.__iter__())
-  [u'test', '++etc++site']
+  ['test', '++etc++site']
   >>> list(fs_folder.values())
   [...Folder object at 0x...>, <LocalSiteManager ++etc++site>]
   >>> len(fs_folder)
   2
   >>> list(fs_folder.items())
-  [(u'test', ...Folder object at 0x...>),
+  [('test', ...Folder object at 0x...>),
    ('++etc++site', <LocalSiteManager ++etc++site>)]
   >>> 'test' in fs_folder
   True
```

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_bwc.py` & `zope.site-5.0/src/zope/site/tests/test_bwc.py`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_configure.py` & `zope.site-5.0/src/zope/site/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_folder.py` & `zope.site-5.0/src/zope/site/tests/test_folder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-
-
 import doctest
 import unittest
 
 from zope.site.folder import Folder
-from zope.site.testing import checker
 from zope.site.testing import siteSetUp
 from zope.site.testing import siteTearDown
 from zope.site.tests.test_site import TestSiteManagerContainer
 
 
 def setUp(test=None):
     siteSetUp()
@@ -59,9 +56,9 @@
     flags = doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
     return unittest.TestSuite((
         unittest.defaultTestLoader.loadTestsFromName(__name__),
         doctest.DocTestSuite('zope.site.folder',
                              setUp=setUp, tearDown=tearDown),
         doctest.DocFileSuite("folder.txt",
                              setUp=setUp, tearDown=tearDown,
-                             checker=checker, optionflags=flags),
+                             optionflags=flags),
     ))
```

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_localsitemanager.py` & `zope.site-5.0/src/zope/site/tests/test_localsitemanager.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,9 +52,9 @@
         self.assertIsNot(
             self.root['copied_site'].getSiteManager().getUtility(I1),
             self.util)
 
 
 def test_suite():
     return unittest.TestSuite((
-        unittest.makeSuite(TestLocalSiteManager),
+        unittest.defaultTestLoader.loadTestsFromTestCase(TestLocalSiteManager),
     ))
```

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_registration.py` & `zope.site-5.0/src/zope/site/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_site.py` & `zope.site-5.0/src/zope/site/tests/test_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 from zope import site
 from zope.site import folder
 from zope.site import interfaces
 from zope.site import testing
 
 
 @zope.interface.implementer(interfaces.ILocalSiteManager)
-class SiteManagerStub(object):
+class SiteManagerStub:
     pass
 
 
 class CustomFolder(folder.Folder):
 
     def __init__(self, name):
         self.__name__ = name
-        super(CustomFolder, self).__init__()
+        super().__init__()
 
     def __repr__(self):  # pragma: no cover
-        return '<%s %s>' % (self.__class__.__name__, self.__name__)
+        return '<{} {}>'.format(self.__class__.__name__, self.__name__)
 
 
 def test_SiteManagerAdapter():
     """
     The site manager adapter is used to find the nearest site for any given
     location. If the provided context is a site,
 
@@ -177,15 +177,15 @@
     testing.siteSetUp()
 
 
 def tearDown(test):
     testing.siteTearDown()
 
 
-class Layer(object):
+class Layer:
 
     @staticmethod
     def setUp():
         pass
 
 
 def test_suite():
```

### Comparing `zope.site-4.6.1/src/zope/site/tests/test_sitemanagercontainer.py` & `zope.site-5.0/src/zope/site/tests/test_sitemanagercontainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from zope.lifecycleevent.interfaces import IObjectRemovedEvent
 
 import zope.site.testing
 from zope.site.folder import rootFolder
 from zope.site.site import SiteManagerContainer
 
 
-class Dummy(object):
+class Dummy:
     pass
 
 
 removed_called = False
 
 
 def removed_event(obj, event):
```

### Comparing `zope.site-4.6.1/src/zope.site.egg-info/PKG-INFO` & `zope.site-5.0/src/zope.site.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: zope.site
-Version: 4.6.1
+Version: 5.0
 Summary: Local registries for zope component architecture
 Home-page: http://zopesite.readthedocs.io
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope component architecture local
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
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
 Classifier: Framework :: Zope :: 3
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ===============
  ``zope.site``
 ===============
@@ -432,14 +428,22 @@
   ()
 
 
 =========
  Changes
 =========
 
+5.0 (2023-06-30)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 4.6.1 (2022-09-02)
 ==================
 
 - Fix more deprecation warnings.
 
 
 4.6 (2022-08-23)
@@ -658,9 +662,7 @@
 - Use zope.container instead of zope.app.container.
 
 3.5.1 (2009-01-27)
 ==================
 
 - Extracted from zope.app.component (trunk, 3.5.1 under development)
   as part of an effort to clean up dependencies between Zope packages.
-
-
```

### Comparing `zope.site-4.6.1/src/zope.site.egg-info/SOURCES.txt` & `zope.site-5.0/src/zope.site.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.site-4.6.1/tox.ini` & `zope.site-5.0/tox.ini`

 * *Files 8% similar despite different names*

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
@@ -39,14 +36,15 @@
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
@@ -60,24 +58,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
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
 source = zope.site
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

