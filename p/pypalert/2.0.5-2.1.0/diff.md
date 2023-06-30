# Comparing `tmp/pypalert-2.0.5.tar.gz` & `tmp/pypalert-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.0.5.tar", last modified: Mon Jun 26 08:47:34 2023, max compression
+gzip compressed data, was "pypalert-2.1.0.tar", last modified: Fri Jun 30 01:36:02 2023, max compression
```

## Comparing `pypalert-2.0.5.tar` & `pypalert-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.232540 pypalert-2.0.5/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.0.5/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-26 08:47:34.233542 pypalert-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-26 08:47:34.234543 pypalert-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-26 08:47:21.000000 pypalert-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.203253 pypalert-2.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.217696 pypalert-2.0.5/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.0.5/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    14310 2023-06-26 08:47:12.000000 pypalert-2.0.5/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.0.5/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:47:34.232540 pypalert-2.0.5/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 08:47:34.000000 pypalert-2.0.5/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 01:36:02.979678 pypalert-2.1.0/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.1.0/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-30 01:36:02.979678 pypalert-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-30 01:36:02.980695 pypalert-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-30 01:35:59.000000 pypalert-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:36:02.963678 pypalert-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 01:36:02.970686 pypalert-2.1.0/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.1.0/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    24257 2023-06-30 01:11:42.000000 pypalert-2.1.0/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11827 2023-06-26 02:21:04.000000 pypalert-2.1.0/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-30 01:36:02.978678 pypalert-2.1.0/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-30 01:36:02.000000 pypalert-2.1.0/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-30 01:36:02.000000 pypalert-2.1.0/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 01:36:02.000000 pypalert-2.1.0/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 01:36:02.000000 pypalert-2.1.0/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.0.5/src/pypalert/pypalert.py` & `pypalert-2.1.0/src/pypalert/pypalert.py`

 * *Files identical despite different names*

