# Comparing `tmp/synnamon-0.1.4.tar.gz` & `tmp/synnamon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnamon-0.1.4.tar", last modified: Fri Jun 30 17:55:03 2023, max compression
+gzip compressed data, was "synnamon-0.1.5.tar", last modified: Fri Jun 30 18:19:03 2023, max compression
```

## Comparing `synnamon-0.1.4.tar` & `synnamon-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.885316 synnamon-0.1.4/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.4/LICENSE.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1875 2023-06-30 17:55:03.885045 synnamon-0.1.4/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1399 2023-06-30 17:52:01.000000 synnamon-0.1.4/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 17:55:03.885400 synnamon-0.1.4/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)      791 2023-06-30 17:51:35.000000 synnamon-0.1.4/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.880234 synnamon-0.1.4/synnamon/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       61 2023-06-30 17:51:41.000000 synnamon-0.1.4/synnamon/__init__.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.884092 synnamon-0.1.4/synnamon/data/
--rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.4/synnamon/data/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      945 2023-06-30 17:53:48.000000 synnamon-0.1.4/synnamon/get_syns.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.883778 synnamon-0.1.4/synnamon.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1875 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)       18 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 17:55:03.000000 synnamon-0.1.4/synnamon.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 17:55:03.884590 synnamon-0.1.4/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.4/tests/test_get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:19:03.053553 synnamon-0.1.5/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.5/LICENSE.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:19:03.053285 synnamon-0.1.5/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1384 2023-06-30 18:16:35.000000 synnamon-0.1.5/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 18:19:03.053633 synnamon-0.1.5/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      791 2023-06-30 18:16:13.000000 synnamon-0.1.5/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:19:03.048774 synnamon-0.1.5/synnamon/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      479 2023-06-30 18:16:03.000000 synnamon-0.1.5/synnamon/__init__.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:19:03.052351 synnamon-0.1.5/synnamon/data/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.5/synnamon/data/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      965 2023-06-30 18:15:36.000000 synnamon-0.1.5/synnamon/get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:19:03.051942 synnamon-0.1.5/synnamon.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:19:03.000000 synnamon-0.1.5/synnamon.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      279 2023-06-30 18:19:03.000000 synnamon-0.1.5/synnamon.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 18:19:03.000000 synnamon-0.1.5/synnamon.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       18 2023-06-30 18:19:03.000000 synnamon-0.1.5/synnamon.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 18:19:03.000000 synnamon-0.1.5/synnamon.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:19:03.052788 synnamon-0.1.5/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.5/tests/test_get_syns.py
```

### Comparing `synnamon-0.1.4/LICENSE.md` & `synnamon-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.4/PKG-INFO` & `synnamon-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,28 +20,27 @@
 
 # Synnamon: Easy to use function for word synonym lookups
 [![PyPI Latest Release](https://img.shields.io/pypi/v/synnamon.svg)](https://pypi.org/project/synnamon/)
 ![Tests](https://github.com/eddiethedean/synnamon/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus shelve file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
+**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus json file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/synnamon
 
 ```sh
 # PyPI
 pip install synnamon
 ```
 
 ## Dependencies
 - inflex: used to convert plural word lookups to singular and then convert singular synonym results to plural
-- sqlitedict
 
 
 ## Example
 ```sh
 >>> import synnamon
 
 >>> synnamon.get_syns('jump')
```

### Comparing `synnamon-0.1.4/README.md` & `synnamon-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 
 # Synnamon: Easy to use function for word synonym lookups
 [![PyPI Latest Release](https://img.shields.io/pypi/v/synnamon.svg)](https://pypi.org/project/synnamon/)
 ![Tests](https://github.com/eddiethedean/synnamon/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus shelve file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
+**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus json file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/synnamon
 
 ```sh
 # PyPI
 pip install synnamon
 ```
 
 ## Dependencies
 - inflex: used to convert plural word lookups to singular and then convert singular synonym results to plural
-- sqlitedict
 
 
 ## Example
 ```sh
 >>> import synnamon
 
 >>> synnamon.get_syns('jump')
```

### Comparing `synnamon-0.1.4/setup.py` & `synnamon-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="synnamon",
-    version="0.1.4",
+    version="0.1.5",
     description="Pure Python package for getting synonyms for words.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/eddiethedean/synnamon",
     author="Odos Matthews",
     author_email="odosmatthews@gmail.com",
     license="MIT",
```

### Comparing `synnamon-0.1.4/synnamon/get_syns.py` & `synnamon-0.1.5/synnamon/get_syns.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import pathlib
+import json
 
 from inflex import Noun
-from sqlitedict import SqliteDict
 
 path = pathlib.Path(__file__).parent.resolve()
 
+with open(os.path.join(path, 'data/en_thesaurus_dict.json')) as f:
+    thesaurus = json.load(f)
+
 
 def get_record(word: str) -> dict:
-    with SqliteDict(os.path.join(path, 'data/en_thesaurus.sqlite')) as db:
-        if word in db:
-            return db[word]
-    return {}
+    if word in thesaurus:
+        return thesaurus[word]
+    else:
+        return {}
 
 
 def get_syns(word: str) -> dict:
     """Get synonyms for a word from the thesaurus."""
     word = word.lower()
     record = get_record(word)
     if record == {}:
```

### Comparing `synnamon-0.1.4/synnamon.egg-info/PKG-INFO` & `synnamon-0.1.5/synnamon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,28 +20,27 @@
 
 # Synnamon: Easy to use function for word synonym lookups
 [![PyPI Latest Release](https://img.shields.io/pypi/v/synnamon.svg)](https://pypi.org/project/synnamon/)
 ![Tests](https://github.com/eddiethedean/synnamon/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus shelve file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
+**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus json file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/synnamon
 
 ```sh
 # PyPI
 pip install synnamon
 ```
 
 ## Dependencies
 - inflex: used to convert plural word lookups to singular and then convert singular synonym results to plural
-- sqlitedict
 
 
 ## Example
 ```sh
 >>> import synnamon
 
 >>> synnamon.get_syns('jump')
```

### Comparing `synnamon-0.1.4/tests/test_get_syns.py` & `synnamon-0.1.5/tests/test_get_syns.py`

 * *Files identical despite different names*

