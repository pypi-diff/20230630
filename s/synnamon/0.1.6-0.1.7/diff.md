# Comparing `tmp/synnamon-0.1.6.tar.gz` & `tmp/synnamon-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnamon-0.1.6.tar", last modified: Fri Jun 30 18:26:43 2023, max compression
+gzip compressed data, was "synnamon-0.1.7.tar", last modified: Fri Jun 30 18:57:14 2023, max compression
```

## Comparing `synnamon-0.1.6.tar` & `synnamon-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:26:43.975772 synnamon-0.1.6/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.6/LICENSE.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:26:43.975480 synnamon-0.1.6/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1384 2023-06-30 18:16:35.000000 synnamon-0.1.6/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 18:26:43.975854 synnamon-0.1.6/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)      777 2023-06-30 18:25:35.000000 synnamon-0.1.6/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:26:43.969646 synnamon-0.1.6/synnamon/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       62 2023-06-30 18:25:27.000000 synnamon-0.1.6/synnamon/__init__.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:26:43.974650 synnamon-0.1.6/synnamon/data/
--rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.6/synnamon/data/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      965 2023-06-30 18:25:45.000000 synnamon-0.1.6/synnamon/get_syns.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:26:43.974305 synnamon-0.1.6/synnamon.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:26:43.000000 synnamon-0.1.6/synnamon.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 18:26:43.000000 synnamon-0.1.6/synnamon.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 18:26:43.000000 synnamon-0.1.6/synnamon.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-06-30 18:26:43.000000 synnamon-0.1.6/synnamon.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 18:26:43.000000 synnamon-0.1.6/synnamon.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:26:43.975002 synnamon-0.1.6/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.6/tests/test_get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.697414 synnamon-0.1.7/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.7/LICENSE.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:57:14.697090 synnamon-0.1.7/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1384 2023-06-30 18:16:35.000000 synnamon-0.1.7/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 18:57:14.697490 synnamon-0.1.7/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      777 2023-06-30 18:56:00.000000 synnamon-0.1.7/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.681112 synnamon-0.1.7/synnamon/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       62 2023-06-30 18:56:15.000000 synnamon-0.1.7/synnamon/__init__.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.686629 synnamon-0.1.7/synnamon/data/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.7/synnamon/data/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)  9230899 2023-06-30 18:53:58.000000 synnamon-0.1.7/synnamon/data/thesaurus.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      821 2023-06-30 18:55:31.000000 synnamon-0.1.7/synnamon/get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.685879 synnamon-0.1.7/synnamon.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      306 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.695784 synnamon-0.1.7/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.7/tests/test_get_syns.py
```

### Comparing `synnamon-0.1.6/LICENSE.md` & `synnamon-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.6/PKG-INFO` & `synnamon-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synnamon-0.1.6/README.md` & `synnamon-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.6/setup.py` & `synnamon-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="synnamon",
-    version="0.1.6",
+    version="0.1.7",
     description="Pure Python package for getting synonyms for words.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/eddiethedean/synnamon",
     author="Odos Matthews",
     author_email="odosmatthews@gmail.com",
     license="MIT",
```

### Comparing `synnamon-0.1.6/synnamon.egg-info/PKG-INFO` & `synnamon-0.1.7/synnamon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synnamon-0.1.6/tests/test_get_syns.py` & `synnamon-0.1.7/tests/test_get_syns.py`

 * *Files identical despite different names*

