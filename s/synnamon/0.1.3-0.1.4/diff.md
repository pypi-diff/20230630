# Comparing `tmp/synnamon-0.1.3.tar.gz` & `tmp/synnamon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnamon-0.1.3.tar", last modified: Fri Jun 30 17:23:09 2023, max compression
+gzip compressed data, was "synnamon-0.1.4.tar", last modified: Fri Jun 30 17:55:03 2023, max compression
```

## Comparing `synnamon-0.1.3.tar` & `synnamon-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:23:09.142412 synnamon-0.1.3/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.3/LICENSE.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-06-30 17:23:09.142100 synnamon-0.1.3/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1386 2023-06-30 15:50:01.000000 synnamon-0.1.3/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 17:23:09.142493 synnamon-0.1.3/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)      777 2023-06-30 17:22:29.000000 synnamon-0.1.3/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:23:09.131488 synnamon-0.1.3/synnamon/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       61 2023-06-30 17:22:36.000000 synnamon-0.1.3/synnamon/__init__.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:23:09.141329 synnamon-0.1.3/synnamon/data/
--rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.3/synnamon/data/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1089 2023-06-30 17:21:14.000000 synnamon-0.1.3/synnamon/get_syns.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:23:09.140682 synnamon-0.1.3/synnamon.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-06-30 17:23:09.000000 synnamon-0.1.3/synnamon.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 17:23:09.000000 synnamon-0.1.3/synnamon.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 17:23:09.000000 synnamon-0.1.3/synnamon.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-06-30 17:23:09.000000 synnamon-0.1.3/synnamon.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 17:23:09.000000 synnamon-0.1.3/synnamon.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:23:09.141689 synnamon-0.1.3/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.3/tests/test_get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.885316 synnamon-0.1.4/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.4/LICENSE.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1875 2023-06-30 17:55:03.885045 synnamon-0.1.4/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1399 2023-06-30 17:52:01.000000 synnamon-0.1.4/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 17:55:03.885400 synnamon-0.1.4/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      791 2023-06-30 17:51:35.000000 synnamon-0.1.4/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.880234 synnamon-0.1.4/synnamon/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       61 2023-06-30 17:51:41.000000 synnamon-0.1.4/synnamon/__init__.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.884092 synnamon-0.1.4/synnamon/data/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.4/synnamon/data/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      945 2023-06-30 17:53:48.000000 synnamon-0.1.4/synnamon/get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.883778 synnamon-0.1.4/synnamon.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1875 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       18 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.884590 synnamon-0.1.4/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.4/tests/test_get_syns.py
```

### Comparing `synnamon-0.1.3/LICENSE.md` & `synnamon-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.3/PKG-INFO` & `synnamon-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 A simple Python package that looks up synonyms for words.
 
 ![Synnamon Logo](https://raw.githubusercontent.com/eddiethedean/synnamon/main/docs/synnamon.png)
 -----------------
@@ -33,14 +33,15 @@
 ```sh
 # PyPI
 pip install synnamon
 ```
 
 ## Dependencies
 - inflex: used to convert plural word lookups to singular and then convert singular synonym results to plural
+- sqlitedict
 
 
 ## Example
 ```sh
 >>> import synnamon
 
 >>> synnamon.get_syns('jump')
```

### Comparing `synnamon-0.1.3/README.md` & `synnamon-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ```sh
 # PyPI
 pip install synnamon
 ```
 
 ## Dependencies
 - inflex: used to convert plural word lookups to singular and then convert singular synonym results to plural
+- sqlitedict
 
 
 ## Example
 ```sh
 >>> import synnamon
 
 >>> synnamon.get_syns('jump')
```

### Comparing `synnamon-0.1.3/setup.py` & `synnamon-0.1.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="synnamon",
-    version="0.1.3",
+    version="0.1.4",
     description="Pure Python package for getting synonyms for words.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/eddiethedean/synnamon",
     author="Odos Matthews",
     author_email="odosmatthews@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
     ],
     packages=find_packages(),
     include_package_data=True,
-    python_requires='>=3.6',
-    install_requires=['inflex']
+    python_requires='>=3.7',
+    install_requires=['inflex', 'sqlitedict']
 )
```

### Comparing `synnamon-0.1.3/synnamon/get_syns.py` & `synnamon-0.1.4/synnamon/get_syns.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import shelve
 import os
 import pathlib
 
 from inflex import Noun
+from sqlitedict import SqliteDict
 
 path = pathlib.Path(__file__).parent.resolve()
 
 
 def get_record(word: str) -> dict:
-    with shelve.open(os.path.join(path, 'data/en_thesaurus0')) as thesaurus0:
-        if word in thesaurus0:
-            return thesaurus0[word]
-    with shelve.open(os.path.join(path, 'data/en_thesaurus1')) as thesaurus1:
-        if word in thesaurus1:
-            return thesaurus1[word]
+    with SqliteDict(os.path.join(path, 'data/en_thesaurus.sqlite')) as db:
+        if word in db:
+            return db[word]
     return {}
 
 
 def get_syns(word: str) -> dict:
     """Get synonyms for a word from the thesaurus."""
     word = word.lower()
     record = get_record(word)
```

### Comparing `synnamon-0.1.3/synnamon.egg-info/PKG-INFO` & `synnamon-0.1.4/synnamon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 A simple Python package that looks up synonyms for words.
 
 ![Synnamon Logo](https://raw.githubusercontent.com/eddiethedean/synnamon/main/docs/synnamon.png)
 -----------------
@@ -33,14 +33,15 @@
 ```sh
 # PyPI
 pip install synnamon
 ```
 
 ## Dependencies
 - inflex: used to convert plural word lookups to singular and then convert singular synonym results to plural
+- sqlitedict
 
 
 ## Example
 ```sh
 >>> import synnamon
 
 >>> synnamon.get_syns('jump')
```

### Comparing `synnamon-0.1.3/tests/test_get_syns.py` & `synnamon-0.1.4/tests/test_get_syns.py`

 * *Files identical despite different names*

