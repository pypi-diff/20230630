# Comparing `tmp/teamanchorhello-0.0.7.tar.gz` & `tmp/teamanchorhello-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamanchorhello-0.0.7.tar", last modified: Fri Jun 30 03:36:22 2023, max compression
+gzip compressed data, was "teamanchorhello-0.0.8.tar", last modified: Fri Jun 30 03:46:20 2023, max compression
```

## Comparing `teamanchorhello-0.0.7.tar` & `teamanchorhello-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.7/LICENSE
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1769 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1413 2023-06-29 18:56:03.000000 teamanchorhello-0.0.7/README.md
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/setup.cfg
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-30 03:35:58.000000 teamanchorhello-0.0.7/setup.py
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/teamanchorhello/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/teamanchorhello/src/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1769 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-30 03:36:02.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:46:20.676676 teamanchorhello-0.0.8/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.8/LICENSE
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1769 2023-06-30 03:46:20.676676 teamanchorhello-0.0.8/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1413 2023-06-29 18:56:03.000000 teamanchorhello-0.0.8/README.md
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-30 03:46:20.676676 teamanchorhello-0.0.8/setup.cfg
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-30 03:46:11.000000 teamanchorhello-0.0.8/setup.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:46:20.676676 teamanchorhello-0.0.8/teamanchorhello/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:46:20.676676 teamanchorhello-0.0.8/teamanchorhello/src/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:46:20.676676 teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.egg-info/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1769 2023-06-30 03:46:20.000000 teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-30 03:46:20.000000 teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-30 03:46:20.000000 teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-30 03:46:20.000000 teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-30 03:46:09.000000 teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.py
```

### Comparing `teamanchorhello-0.0.7/PKG-INFO` & `teamanchorhello-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.7
+Version: 0.0.8
 Summary: teamanchor say hello using Pypi package.
 Author: fanis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamanchorhello-0.0.7/README.md` & `teamanchorhello-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `teamanchorhello-0.0.7/setup.py` & `teamanchorhello-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="teamanchorhello",
-    version="0.0.7",
+    version="0.0.8",
     author="fanis",
     description="teamanchor say hello using Pypi package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO` & `teamanchorhello-0.0.8/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.7
+Version: 0.0.8
 Summary: teamanchor say hello using Pypi package.
 Author: fanis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

