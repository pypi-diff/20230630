# Comparing `tmp/trazhash-0.1.2.tar.gz` & `tmp/trazhash-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trazhash-0.1.2.tar", last modified: Fri Jun 30 03:50:35 2023, max compression
+gzip compressed data, was "trazhash-0.1.3.tar", last modified: Fri Jun 30 03:53:51 2023, max compression
```

## Comparing `trazhash-0.1.2.tar` & `trazhash-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 03:50:35.207383 trazhash-0.1.2/
--rw-rw-rw-   0        0        0     3481 2023-06-30 03:50:35.206381 trazhash-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3046 2023-06-30 03:48:51.000000 trazhash-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 03:50:35.207383 trazhash-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-06-30 03:50:16.000000 trazhash-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:50:35.203810 trazhash-0.1.2/trazhash.egg-info/
--rw-rw-rw-   0        0        0     3481 2023-06-30 03:50:35.000000 trazhash-0.1.2/trazhash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-06-30 03:50:35.000000 trazhash-0.1.2/trazhash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 03:50:35.000000 trazhash-0.1.2/trazhash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 03:50:35.000000 trazhash-0.1.2/trazhash.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 03:53:51.377242 trazhash-0.1.3/
+-rw-rw-rw-   0        0        0     3481 2023-06-30 03:53:51.376243 trazhash-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3046 2023-06-30 03:48:51.000000 trazhash-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 03:53:51.377242 trazhash-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-06-30 03:53:43.000000 trazhash-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:53:51.374255 trazhash-0.1.3/trazhash.egg-info/
+-rw-rw-rw-   0        0        0     3481 2023-06-30 03:53:51.000000 trazhash-0.1.3/trazhash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-06-30 03:53:51.000000 trazhash-0.1.3/trazhash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:53:51.000000 trazhash-0.1.3/trazhash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:53:51.000000 trazhash-0.1.3/trazhash.egg-info/top_level.txt
```

### Comparing `trazhash-0.1.2/PKG-INFO` & `trazhash-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trazhash
-Version: 0.1.2
+Version: 0.1.3
 Summary: TrazHash is a Python library designed to hash data strings, called a System-Dependent Hash, or a SDHASH, or file contents using a combination of your system's specific values and cryptographic hash functions.
 Home-page: https://github.com/traztech/trazhash
 Author: TrazTech
 Author-email: contact@traztech.ca
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `trazhash-0.1.2/README.md` & `trazhash-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trazhash-0.1.2/setup.py` & `trazhash-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='trazhash',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         # List your library dependencies here
     ],
     author='TrazTech',
     author_email='contact@traztech.ca',
     description="TrazHash is a Python library designed to hash data strings, called a System-Dependent Hash, or a SDHASH, or file contents using a combination of your system's specific values and cryptographic hash functions.",
```

### Comparing `trazhash-0.1.2/trazhash.egg-info/PKG-INFO` & `trazhash-0.1.3/trazhash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trazhash
-Version: 0.1.2
+Version: 0.1.3
 Summary: TrazHash is a Python library designed to hash data strings, called a System-Dependent Hash, or a SDHASH, or file contents using a combination of your system's specific values and cryptographic hash functions.
 Home-page: https://github.com/traztech/trazhash
 Author: TrazTech
 Author-email: contact@traztech.ca
 License: MIT
 Description-Content-Type: text/markdown
```

