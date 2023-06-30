# Comparing `tmp/testless_textanalyzer-0.1.0.tar.gz` & `tmp/testless_textanalyzer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_textanalyzer-0.1.0.tar", last modified: Fri Jun 30 13:06:02 2023, max compression
+gzip compressed data, was "testless_textanalyzer-0.1.1.tar", last modified: Fri Jun 30 14:28:35 2023, max compression
```

## Comparing `testless_textanalyzer-0.1.0.tar` & `testless_textanalyzer-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 13:06:02.704274 testless_textanalyzer-0.1.0/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      356 2023-06-30 13:06:02.704274 testless_textanalyzer-0.1.0/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-06-30 13:06:02.704274 testless_textanalyzer-0.1.0/setup.cfg
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      742 2023-06-30 12:57:51.000000 testless_textanalyzer-0.1.0/setup.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 13:06:02.700274 testless_textanalyzer-0.1.0/testless_textanalyzer.egg-info/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      356 2023-06-30 13:06:02.000000 testless_textanalyzer-0.1.0/testless_textanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      406 2023-06-30 13:06:02.000000 testless_textanalyzer-0.1.0/testless_textanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-06-30 13:06:02.000000 testless_textanalyzer-0.1.0/testless_textanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       62 2023-06-30 13:06:02.000000 testless_textanalyzer-0.1.0/testless_textanalyzer.egg-info/requires.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-06-30 13:06:02.000000 testless_textanalyzer-0.1.0/testless_textanalyzer.egg-info/top_level.txt
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 13:06:02.700274 testless_textanalyzer-0.1.0/textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.0/textanalyzer/__init__.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 13:06:02.704274 testless_textanalyzer-0.1.0/textanalyzer/testless_textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.0/textanalyzer/testless_textanalyzer/__init__.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.0/textanalyzer/testless_textanalyzer/feature_set.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     3818 2023-06-30 12:42:38.000000 testless_textanalyzer-0.1.0/textanalyzer/testless_textanalyzer/text_analyzer.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 14:28:35.811167 testless_textanalyzer-0.1.1/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-06-30 14:28:35.811167 testless_textanalyzer-0.1.1/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-06-30 14:28:35.811167 testless_textanalyzer-0.1.1/setup.cfg
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-06-30 14:28:01.000000 testless_textanalyzer-0.1.1/setup.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 14:28:35.811167 testless_textanalyzer-0.1.1/testless_textanalyzer.egg-info/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-06-30 14:28:35.000000 testless_textanalyzer-0.1.1/testless_textanalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      406 2023-06-30 14:28:35.000000 testless_textanalyzer-0.1.1/testless_textanalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-06-30 14:28:35.000000 testless_textanalyzer-0.1.1/testless_textanalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       62 2023-06-30 14:28:35.000000 testless_textanalyzer-0.1.1/testless_textanalyzer.egg-info/requires.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-06-30 14:28:35.000000 testless_textanalyzer-0.1.1/testless_textanalyzer.egg-info/top_level.txt
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 14:28:35.811167 testless_textanalyzer-0.1.1/textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.1/textanalyzer/__init__.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 14:28:35.811167 testless_textanalyzer-0.1.1/textanalyzer/testless_textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.1/textanalyzer/testless_textanalyzer/__init__.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.1/textanalyzer/testless_textanalyzer/feature_set.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     3818 2023-06-30 12:42:38.000000 testless_textanalyzer-0.1.1/textanalyzer/testless_textanalyzer/text_analyzer.py
```

### Comparing `testless_textanalyzer-0.1.0/setup.py` & `testless_textanalyzer-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
-with open("/home/yousif/Downloads/GP/testless/Text_Analyzer/README.md", "r") as f:
-    long_description = f.read()
+
 
 setup(
   name = 'testless_textanalyzer' ,
-  version='0.1.0',
+  version='0.1.1',
   description='A text analyzer for test step sentences',
   packages=find_packages(),
   author='Youssef Ahmed',
   include_package_data=True,
   license='MIT',
-  long_description=long_description,
+  long_description="Text analyzer for test step sentences",
   long_description_content_type="text/markdown",
   classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
   ],
   install_requires=["nltk>=3.8" , "numpy>=1.21.5" , "pandas>=1.5.3" , "sklearn_crfsuite>=0.3.6"],
```

### Comparing `testless_textanalyzer-0.1.0/textanalyzer/testless_textanalyzer/feature_set.py` & `testless_textanalyzer-0.1.1/textanalyzer/testless_textanalyzer/feature_set.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.0/textanalyzer/testless_textanalyzer/text_analyzer.py` & `testless_textanalyzer-0.1.1/textanalyzer/testless_textanalyzer/text_analyzer.py`

 * *Files identical despite different names*

