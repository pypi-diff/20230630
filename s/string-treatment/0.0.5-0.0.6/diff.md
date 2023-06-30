# Comparing `tmp/string_treatment-0.0.5.tar.gz` & `tmp/string_treatment-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_treatment-0.0.5.tar", last modified: Fri Jun 30 15:16:56 2023, max compression
+gzip compressed data, was "string_treatment-0.0.6.tar", last modified: Fri Jun 30 15:26:52 2023, max compression
```

## Comparing `string_treatment-0.0.5.tar` & `string_treatment-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:16:56.885928 string_treatment-0.0.5/
--rw-rw-rw-   0        0        0      620 2023-06-30 15:16:56.883928 string_treatment-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-06-30 15:14:17.000000 string_treatment-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 15:16:56.885928 string_treatment-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-06-30 15:16:47.000000 string_treatment-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:16:56.879791 string_treatment-0.0.5/string_treatment.egg-info/
--rw-rw-rw-   0        0        0      620 2023-06-30 15:16:56.000000 string_treatment-0.0.5/string_treatment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-30 15:16:56.000000 string_treatment-0.0.5/string_treatment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:16:56.000000 string_treatment-0.0.5/string_treatment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-30 15:16:56.000000 string_treatment-0.0.5/string_treatment.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:16:56.000000 string_treatment-0.0.5/string_treatment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4317 2023-06-30 15:13:11.000000 string_treatment-0.0.5/string_treatment.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:26:52.184462 string_treatment-0.0.6/
+-rw-rw-rw-   0        0        0      620 2023-06-30 15:26:52.176884 string_treatment-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-06-30 15:26:14.000000 string_treatment-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 15:26:52.184462 string_treatment-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-30 15:26:28.000000 string_treatment-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:26:52.173442 string_treatment-0.0.6/string_treatment.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:26:51.000000 string_treatment-0.0.6/string_treatment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4317 2023-06-30 15:13:11.000000 string_treatment-0.0.6/string_treatment.py
```

### Comparing `string_treatment-0.0.5/PKG-INFO` & `string_treatment-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_treatment
-Version: 0.0.5
+Version: 0.0.6
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `string_treatment-0.0.5/README.md` & `string_treatment-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 ```shell
 pip install string-treatment
 ```
 
 # Quick start
 #### With reference list
 ``` python
->>> from string_treatment import treat_referenced
+>>> import string_treatment as st
 >>> list_of_reference = ['João Pessoa/PB']
 >>> data_with_inconsistency = ['João Pessoa PB', 'Joao pessoa--PB', 'joa pssoa(pb)']
->>> treat_referenced(data_with_inconsistency, list_of_reference)
+>>> st.treat_referenced(data_with_inconsistency, list_of_reference)
 ['João Pessoa PB', 'João Pessoa PB', 'João Pessoa PB']
 ```
 
 #### Without reference list
 ``` python
->>> from string_treatment import treat_unreferenced
+>>> import string_treatment as st
 >>> data_with_inconsistency = ['João Pessoa PB', 'Joao pessoa--PB', 'joa pssoa(pb)']
->>> treat_unreferenced(data_with_inconsistency)
+>>> st.treat_unreferenced(data_with_inconsistency)
 ['João Pessoa PB', 'João Pessoa PB', 'João Pessoa PB']
 ```
 
 # Usage
 To learn about how to use this library and examples,
-[visit the User Guide, which is a Jupyter notebook](https://github.com/guilhermehuther/string_treatment/blob/main/example.ipynb).
+[visit the User Guide, which is a Jupyter notebook](https://github.com/guilhermehuther/string_treatment/blob/main/guide.ipynb).
```

### Comparing `string_treatment-0.0.5/setup.py` & `string_treatment-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'String treatment package'
 LONG_DESCRIPTION = '''
 Method to treat strings with inconsistencies in your data
 
 Github: https://github.com/guilhermehuther/string_treatment
 '''
```

### Comparing `string_treatment-0.0.5/string_treatment.egg-info/PKG-INFO` & `string_treatment-0.0.6/string_treatment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-treatment
-Version: 0.0.5
+Version: 0.0.6
 Summary: String treatment package
 Author: Guilherme Huther Baldo
 Author-email: guilhermehuther@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `string_treatment-0.0.5/string_treatment.py` & `string_treatment-0.0.6/string_treatment.py`

 * *Files identical despite different names*

