# Comparing `tmp/synnamon-0.1.1.tar.gz` & `tmp/synnamon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnamon-0.1.1.tar", last modified: Fri Jun 30 15:52:18 2023, max compression
+gzip compressed data, was "synnamon-0.1.2.tar", last modified: Fri Jun 30 16:10:45 2023, max compression
```

## Comparing `synnamon-0.1.1.tar` & `synnamon-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 15:52:18.668299 synnamon-0.1.1/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.1/LICENSE.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-06-30 15:52:18.668037 synnamon-0.1.1/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1386 2023-06-30 15:50:01.000000 synnamon-0.1.1/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 15:52:18.668387 synnamon-0.1.1/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)      777 2023-06-30 15:50:42.000000 synnamon-0.1.1/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 15:52:18.654022 synnamon-0.1.1/synnamon/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       61 2023-06-30 15:50:34.000000 synnamon-0.1.1/synnamon/__init__.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 15:52:18.667024 synnamon-0.1.1/synnamon/data/
--rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.1/synnamon/data/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      893 2023-06-30 15:51:40.000000 synnamon-0.1.1/synnamon/get_syns.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 15:52:18.666586 synnamon-0.1.1/synnamon.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-06-30 15:52:18.000000 synnamon-0.1.1/synnamon.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 15:52:18.000000 synnamon-0.1.1/synnamon.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 15:52:18.000000 synnamon-0.1.1/synnamon.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-06-30 15:52:18.000000 synnamon-0.1.1/synnamon.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 15:52:18.000000 synnamon-0.1.1/synnamon.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 15:52:18.667436 synnamon-0.1.1/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.1/tests/test_get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 16:10:45.740779 synnamon-0.1.2/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.2/LICENSE.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-06-30 16:10:45.740474 synnamon-0.1.2/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1386 2023-06-30 15:50:01.000000 synnamon-0.1.2/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 16:10:45.740870 synnamon-0.1.2/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      777 2023-06-30 16:10:20.000000 synnamon-0.1.2/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 16:10:45.734571 synnamon-0.1.2/synnamon/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       61 2023-06-30 16:10:29.000000 synnamon-0.1.2/synnamon/__init__.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 16:10:45.739564 synnamon-0.1.2/synnamon/data/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.2/synnamon/data/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      893 2023-06-30 15:51:40.000000 synnamon-0.1.2/synnamon/get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 16:10:45.739170 synnamon-0.1.2/synnamon.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-06-30 16:10:45.000000 synnamon-0.1.2/synnamon.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 16:10:45.000000 synnamon-0.1.2/synnamon.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 16:10:45.000000 synnamon-0.1.2/synnamon.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-06-30 16:10:45.000000 synnamon-0.1.2/synnamon.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 16:10:45.000000 synnamon-0.1.2/synnamon.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 16:10:45.739915 synnamon-0.1.2/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.2/tests/test_get_syns.py
```

### Comparing `synnamon-0.1.1/LICENSE.md` & `synnamon-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.1/PKG-INFO` & `synnamon-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synnamon-0.1.1/README.md` & `synnamon-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.1/setup.py` & `synnamon-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="synnamon",
-    version="0.1.1",
+    version="0.1.2",
     description="Pure Python package for getting synonyms for words.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/eddiethedean/synnamon",
     author="Odos Matthews",
     author_email="odosmatthews@gmail.com",
     license="MIT",
```

### Comparing `synnamon-0.1.1/synnamon/get_syns.py` & `synnamon-0.1.2/synnamon/get_syns.py`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.1/synnamon.egg-info/PKG-INFO` & `synnamon-0.1.2/synnamon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synnamon-0.1.1/tests/test_get_syns.py` & `synnamon-0.1.2/tests/test_get_syns.py`

 * *Files identical despite different names*

