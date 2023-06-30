# Comparing `tmp/InjecToast-1.1.4.tar.gz` & `tmp/InjecToast-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InjecToast-1.1.4.tar", last modified: Fri Jun 30 19:40:17 2023, max compression
+gzip compressed data, was "InjecToast-1.1.5.tar", last modified: Fri Jun 30 19:42:00 2023, max compression
```

## Comparing `InjecToast-1.1.4.tar` & `InjecToast-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:40:17.279841 InjecToast-1.1.4/
--rw-r--r--   0 edwardferrari   (501) staff       (20)     7909 2023-06-30 19:40:17.279687 InjecToast-1.1.4/PKG-INFO
--rw-r--r--   0 edwardferrari   (501) staff       (20)     7289 2023-06-30 19:38:18.000000 InjecToast-1.1.4/README.md
--rw-r--r--   0 edwardferrari   (501) staff       (20)      762 2023-06-30 19:39:12.000000 InjecToast-1.1.4/pyproject.toml
--rw-r--r--   0 edwardferrari   (501) staff       (20)       38 2023-06-30 19:40:17.279881 InjecToast-1.1.4/setup.cfg
-drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:40:17.269073 InjecToast-1.1.4/src/
-drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:40:17.272724 InjecToast-1.1.4/src/InjecToast/
--rw-r--r--   0 edwardferrari   (501) staff       (20)    12678 2023-06-30 19:36:44.000000 InjecToast-1.1.4/src/InjecToast/ToastInjector.py
--rw-r--r--   0 edwardferrari   (501) staff       (20)       73 2023-02-18 04:15:04.000000 InjecToast-1.1.4/src/InjecToast/__init__.py
--rw-r--r--   0 edwardferrari   (501) staff       (20)     2280 2023-03-18 19:18:19.000000 InjecToast-1.1.4/src/InjecToast/argparser.py
-drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:40:17.279476 InjecToast-1.1.4/src/InjecToast.egg-info/
--rw-r--r--   0 edwardferrari   (501) staff       (20)     7909 2023-06-30 19:40:17.000000 InjecToast-1.1.4/src/InjecToast.egg-info/PKG-INFO
--rw-r--r--   0 edwardferrari   (501) staff       (20)      304 2023-06-30 19:40:17.000000 InjecToast-1.1.4/src/InjecToast.egg-info/SOURCES.txt
--rw-r--r--   0 edwardferrari   (501) staff       (20)        1 2023-06-30 19:40:17.000000 InjecToast-1.1.4/src/InjecToast.egg-info/dependency_links.txt
--rw-r--r--   0 edwardferrari   (501) staff       (20)       47 2023-06-30 19:40:17.000000 InjecToast-1.1.4/src/InjecToast.egg-info/entry_points.txt
--rw-r--r--   0 edwardferrari   (501) staff       (20)       11 2023-06-30 19:40:17.000000 InjecToast-1.1.4/src/InjecToast.egg-info/top_level.txt
+drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:42:00.651846 InjecToast-1.1.5/
+-rw-r--r--   0 edwardferrari   (501) staff       (20)     7909 2023-06-30 19:42:00.651687 InjecToast-1.1.5/PKG-INFO
+-rw-r--r--   0 edwardferrari   (501) staff       (20)     7289 2023-06-30 19:41:12.000000 InjecToast-1.1.5/README.md
+-rw-r--r--   0 edwardferrari   (501) staff       (20)      762 2023-06-30 19:41:07.000000 InjecToast-1.1.5/pyproject.toml
+-rw-r--r--   0 edwardferrari   (501) staff       (20)       38 2023-06-30 19:42:00.651888 InjecToast-1.1.5/setup.cfg
+drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:42:00.638476 InjecToast-1.1.5/src/
+drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:42:00.642345 InjecToast-1.1.5/src/InjecToast/
+-rw-r--r--   0 edwardferrari   (501) staff       (20)    12678 2023-06-30 19:36:44.000000 InjecToast-1.1.5/src/InjecToast/ToastInjector.py
+-rw-r--r--   0 edwardferrari   (501) staff       (20)       73 2023-02-18 04:15:04.000000 InjecToast-1.1.5/src/InjecToast/__init__.py
+-rw-r--r--   0 edwardferrari   (501) staff       (20)     2280 2023-03-18 19:18:19.000000 InjecToast-1.1.5/src/InjecToast/argparser.py
+drwxr-xr-x   0 edwardferrari   (501) staff       (20)        0 2023-06-30 19:42:00.651494 InjecToast-1.1.5/src/InjecToast.egg-info/
+-rw-r--r--   0 edwardferrari   (501) staff       (20)     7909 2023-06-30 19:42:00.000000 InjecToast-1.1.5/src/InjecToast.egg-info/PKG-INFO
+-rw-r--r--   0 edwardferrari   (501) staff       (20)      304 2023-06-30 19:42:00.000000 InjecToast-1.1.5/src/InjecToast.egg-info/SOURCES.txt
+-rw-r--r--   0 edwardferrari   (501) staff       (20)        1 2023-06-30 19:42:00.000000 InjecToast-1.1.5/src/InjecToast.egg-info/dependency_links.txt
+-rw-r--r--   0 edwardferrari   (501) staff       (20)       47 2023-06-30 19:42:00.000000 InjecToast-1.1.5/src/InjecToast.egg-info/entry_points.txt
+-rw-r--r--   0 edwardferrari   (501) staff       (20)       11 2023-06-30 19:42:00.000000 InjecToast-1.1.5/src/InjecToast.egg-info/top_level.txt
```

### Comparing `InjecToast-1.1.4/PKG-INFO` & `InjecToast-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InjecToast
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tool to inject toasts in Android applications.
 Author-email: PatzEdi <edwardferrari717@gmail.com>
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/InjecToast
 Project-URL: Bug Tracker, https://github.com/PatzEdi/InjecToast/issues
 Keywords: android,androidtool,reverse-engineering,development
 Classifier: Programming Language :: Python :: 3
@@ -33,16 +33,16 @@
 This script uses android application decompilation tools and the FinderZ library in order to function properly.
 HUGE credits to the authors of the tools that are able to decompile android applications.
 
 **This tool is made for educational purposes only!**
 
 ## **A command line application that provides you with the ability to inject toasts in Android Applications, written in Python** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.1.4**
-- Release Version 1.1.3
+## **CHANGELOG: 1.1.5**
+- Release Version 1.1.5
 - Fixed comptaibility issue with FinderZ V2.
 
 ## **Tool Information (IMPORTANT)**
 - Before you proceed, make sure to install my FinderZ library at: [FinderZ](https://pypi.org/project/FinderZ/) This is used in order to manage files properly.
 - It is important to understand that a decompilation tool is required. You MUST decompile the .apk file before using the injector, you can not just give the injector the .apk file, you need to decompile it first.
 - Concerning which tools to use, HUGE credits to those who decompile android applications:
 - Apktool, and ApkToolM.
```

### Comparing `InjecToast-1.1.4/README.md` & `InjecToast-1.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 This script uses android application decompilation tools and the FinderZ library in order to function properly.
 HUGE credits to the authors of the tools that are able to decompile android applications.
 
 **This tool is made for educational purposes only!**
 
 ## **A command line application that provides you with the ability to inject toasts in Android Applications, written in Python** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.1.4**
-- Release Version 1.1.3
+## **CHANGELOG: 1.1.5**
+- Release Version 1.1.5
 - Fixed comptaibility issue with FinderZ V2.
 
 ## **Tool Information (IMPORTANT)**
 - Before you proceed, make sure to install my FinderZ library at: [FinderZ](https://pypi.org/project/FinderZ/) This is used in order to manage files properly.
 - It is important to understand that a decompilation tool is required. You MUST decompile the .apk file before using the injector, you can not just give the injector the .apk file, you need to decompile it first.
 - Concerning which tools to use, HUGE credits to those who decompile android applications:
 - Apktool, and ApkToolM.
```

### Comparing `InjecToast-1.1.4/pyproject.toml` & `InjecToast-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InjecToast"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
 	{ name="PatzEdi", email="edwardferrari717@gmail.com" },
 ]
 description = "A tool to inject toasts in Android applications."
 readme = "README.md"
 keywords = ["android", "androidtool", "reverse-engineering", "development"]
 requires-python = ">=3.9"
```

### Comparing `InjecToast-1.1.4/src/InjecToast/ToastInjector.py` & `InjecToast-1.1.5/src/InjecToast/ToastInjector.py`

 * *Files identical despite different names*

### Comparing `InjecToast-1.1.4/src/InjecToast/argparser.py` & `InjecToast-1.1.5/src/InjecToast/argparser.py`

 * *Files identical despite different names*

### Comparing `InjecToast-1.1.4/src/InjecToast.egg-info/PKG-INFO` & `InjecToast-1.1.5/src/InjecToast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InjecToast
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tool to inject toasts in Android applications.
 Author-email: PatzEdi <edwardferrari717@gmail.com>
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/InjecToast
 Project-URL: Bug Tracker, https://github.com/PatzEdi/InjecToast/issues
 Keywords: android,androidtool,reverse-engineering,development
 Classifier: Programming Language :: Python :: 3
@@ -33,16 +33,16 @@
 This script uses android application decompilation tools and the FinderZ library in order to function properly.
 HUGE credits to the authors of the tools that are able to decompile android applications.
 
 **This tool is made for educational purposes only!**
 
 ## **A command line application that provides you with the ability to inject toasts in Android Applications, written in Python** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.1.4**
-- Release Version 1.1.3
+## **CHANGELOG: 1.1.5**
+- Release Version 1.1.5
 - Fixed comptaibility issue with FinderZ V2.
 
 ## **Tool Information (IMPORTANT)**
 - Before you proceed, make sure to install my FinderZ library at: [FinderZ](https://pypi.org/project/FinderZ/) This is used in order to manage files properly.
 - It is important to understand that a decompilation tool is required. You MUST decompile the .apk file before using the injector, you can not just give the injector the .apk file, you need to decompile it first.
 - Concerning which tools to use, HUGE credits to those who decompile android applications:
 - Apktool, and ApkToolM.
```

