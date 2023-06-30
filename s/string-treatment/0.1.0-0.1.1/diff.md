# Comparing `tmp/string_treatment-0.1.0.tar.gz` & `tmp/string_treatment-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.1.0.tar", last modified: Fri Jun 30 15:39:56 2023, max compression
+gzip compressed data, was "string_treatment-0.1.1.tar", last modified: Fri Jun 30 15:52:01 2023, max compression
```

## Comparing `string_treatment-0.1.0.tar` & `string_treatment-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:56.046358 string_treatment-0.1.0/
--rw-rw-rw-   0        0        0      620 2023-06-30 15:39:56.044366 string_treatment-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-06-30 15:26:14.000000 string_treatment-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 15:39:56.046358 string_treatment-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-06-30 15:39:44.000000 string_treatment-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:39:56.039822 string_treatment-0.1.0/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      620 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:39:55.000000 string_treatment-0.1.0/string_treatment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4111 2023-06-30 15:37:14.000000 string_treatment-0.1.0/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:52:01.778163 string_treatment-0.1.1/
+-rw-rw-rw-   0        0        0      478 2023-06-30 15:52:01.774645 string_treatment-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-06-30 15:26:14.000000 string_treatment-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 15:52:01.778678 string_treatment-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-06-30 15:51:50.000000 string_treatment-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:52:01.768055 string_treatment-0.1.1/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:52:01.000000 string_treatment-0.1.1/string_treatment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4111 2023-06-30 15:37:14.000000 string_treatment-0.1.1/string_treatment.py
```

### Comparing `string_treatment-0.1.0/README.md` & `string_treatment-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `string_treatment-0.1.0/setup.py` & `string_treatment-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'String treatment package'
 LONG_DESCRIPTION = '''
 Method to treat strings with inconsistencies in your data
 
 Github: https://github.com/guilhermehuther/string_treatment
 '''
 
@@ -16,15 +16,12 @@
         author_email="guilhermehuther@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=['jellyfish', 'numpy', 'pandas'],
         keywords=['python', 'first package'],
         classifiers= [
-            "Development Status :: 3 - Alpha",
-            "Intended Audience :: Education",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
-            "Operating System :: MacOS :: MacOS X",
-            "Operating System :: Microsoft :: Windows",
+            "License :: OSI Approved :: MIT License", 
+            "Operating System :: OS Independent",
         ]
 )
```

### Comparing `string_treatment-0.1.0/string_treatment.py` & `string_treatment-0.1.1/string_treatment.py`

 * *Files identical despite different names*

