# Comparing `tmp/string_treatment-0.0.3.tar.gz` & `tmp/string_treatment-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.0.3.tar", last modified: Fri Jun 30 14:13:51 2023, max compression
+gzip compressed data, was "string_treatment-0.0.4.tar", last modified: Fri Jun 30 14:24:21 2023, max compression
```

## Comparing `string_treatment-0.0.3.tar` & `string_treatment-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:13:51.212952 string_treatment-0.0.3/
--rw-rw-rw-   0        0        0      620 2023-06-30 14:13:51.208972 string_treatment-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-06-30 13:50:49.000000 string_treatment-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 14:13:51.212952 string_treatment-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-06-30 14:13:44.000000 string_treatment-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:13:51.204954 string_treatment-0.0.3/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      620 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4274 2023-06-29 13:01:26.000000 string_treatment-0.0.3/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:24:21.162272 string_treatment-0.0.4/
+-rw-rw-rw-   0        0        0      620 2023-06-30 14:24:21.160267 string_treatment-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-06-30 13:50:49.000000 string_treatment-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:24:21.163290 string_treatment-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-30 14:24:14.000000 string_treatment-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:24:21.153800 string_treatment-0.0.4/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-06-30 14:24:20.000000 string_treatment-0.0.4/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-30 14:24:21.000000 string_treatment-0.0.4/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:24:20.000000 string_treatment-0.0.4/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-30 14:24:20.000000 string_treatment-0.0.4/string_treatment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:24:20.000000 string_treatment-0.0.4/string_treatment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4280 2023-06-30 14:21:14.000000 string_treatment-0.0.4/string_treatment.py
```

### Comparing `string_treatment-0.0.3/PKG-INFO` & `string_treatment-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_treatment
-Version: 0.0.3
+Version: 0.0.4
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `string_treatment-0.0.3/README.md` & `string_treatment-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `string_treatment-0.0.3/setup.py` & `string_treatment-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'String treatment package'
 LONG_DESCRIPTION = '''
 Method to treat strings with inconsistencies in your data
 
 Github: https://github.com/guilhermehuther/string_treatment
 '''
```

### Comparing `string_treatment-0.0.3/string_treatment.egg-info/PKG-INFO` & `string_treatment-0.0.4/string_treatment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-treatment
-Version: 0.0.3
+Version: 0.0.4
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `string_treatment-0.0.3/string_treatment.py` & `string_treatment-0.0.4/string_treatment.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 metrics_dict = {
   'jaro_winkler_similarity': jaro_winkler_similarity, 
   'damerau_levenshtein_distance': damerau_levenshtein_distance, 
   'hamming_distance': hamming_distance
 }
 
-def string_treatment(strings_compared, reference = None, metrics = 'all', threshold = 0.9) -> list:
+def string_treatment(strings_compared: list, reference = None, metrics = 'all', threshold = 0.9) -> list:
 
     """
     Compare with a list of reference or creating the list within the strings 
     each other and returns the most similar string for each one.
     
     :param strings_compared: list of strings to be compared
     :param reference: list of reference strings or None if you want to build the list of reference within the 'strings_compared'
```

