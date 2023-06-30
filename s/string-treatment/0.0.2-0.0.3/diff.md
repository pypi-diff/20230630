# Comparing `tmp/string_treatment-0.0.2.tar.gz` & `tmp/string_treatment-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.0.2.tar", last modified: Fri Jun 30 14:00:13 2023, max compression
+gzip compressed data, was "string_treatment-0.0.3.tar", last modified: Fri Jun 30 14:13:51 2023, max compression
```

## Comparing `string_treatment-0.0.2.tar` & `string_treatment-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 14:00:13.387403 string_treatment-0.0.2/
--rw-rw-rw-   0        0        0      555 2023-06-30 14:00:13.385407 string_treatment-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-06-30 13:50:49.000000 string_treatment-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 14:00:13.387403 string_treatment-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-06-30 13:56:20.000000 string_treatment-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 14:00:13.379412 string_treatment-0.0.2/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      555 2023-06-30 14:00:13.000000 string_treatment-0.0.2/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-30 14:00:13.000000 string_treatment-0.0.2/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:00:13.000000 string_treatment-0.0.2/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-30 14:00:13.000000 string_treatment-0.0.2/string_treatment.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 14:00:13.000000 string_treatment-0.0.2/string_treatment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4274 2023-06-29 13:01:26.000000 string_treatment-0.0.2/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:13:51.212952 string_treatment-0.0.3/
+-rw-rw-rw-   0        0        0      620 2023-06-30 14:13:51.208972 string_treatment-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-06-30 13:50:49.000000 string_treatment-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:13:51.212952 string_treatment-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-30 14:13:44.000000 string_treatment-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:13:51.204954 string_treatment-0.0.3/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:13:51.000000 string_treatment-0.0.3/string_treatment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4274 2023-06-29 13:01:26.000000 string_treatment-0.0.3/string_treatment.py
```

### Comparing `string_treatment-0.0.2/PKG-INFO` & `string_treatment-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: string_treatment
-Version: 0.0.2
+Version: 0.0.3
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
+
 Method to treat strings with inconsistencies in your data
+
+Github: https://github.com/guilhermehuther/string_treatment
```

### Comparing `string_treatment-0.0.2/README.md` & `string_treatment-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `string_treatment-0.0.2/setup.py` & `string_treatment-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'String treatment package'
-LONG_DESCRIPTION = 'Method to treat strings with inconsistencies in your data'
+LONG_DESCRIPTION = '''
+Method to treat strings with inconsistencies in your data
+
+Github: https://github.com/guilhermehuther/string_treatment
+'''
 
 setup(
         scripts=['string_treatment.py'],
         name="string_treatment", 
         version=VERSION,
         author="Guilherme Huther Baldo",
         author_email="guilhermehuther@gmail.com",
```

### Comparing `string_treatment-0.0.2/string_treatment.egg-info/PKG-INFO` & `string_treatment-0.0.3/string_treatment.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: string-treatment
-Version: 0.0.2
+Version: 0.0.3
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
+
 Method to treat strings with inconsistencies in your data
+
+Github: https://github.com/guilhermehuther/string_treatment
```

### Comparing `string_treatment-0.0.2/string_treatment.py` & `string_treatment-0.0.3/string_treatment.py`

 * *Files identical despite different names*

