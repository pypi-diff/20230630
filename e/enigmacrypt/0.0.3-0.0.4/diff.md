# Comparing `tmp/enigmacrypt-0.0.3.tar.gz` & `tmp/enigmacrypt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmacrypt-0.0.3.tar", last modified: Fri Jun 30 18:11:20 2023, max compression
+gzip compressed data, was "enigmacrypt-0.0.4.tar", last modified: Fri Jun 30 20:35:53 2023, max compression
```

## Comparing `enigmacrypt-0.0.3.tar` & `enigmacrypt-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.375152 enigmacrypt-0.0.3/
--rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:14.000000 enigmacrypt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2511 2023-06-30 18:11:20.374153 enigmacrypt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:14.000000 enigmacrypt-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.365385 enigmacrypt-0.0.3/app/
--rw-rw-rw-   0        0        0       23 2023-06-30 16:03:21.000000 enigmacrypt-0.0.3/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.366892 enigmacrypt-0.0.3/app/enigmacrypt/
--rw-rw-rw-   0        0        0      116 2023-06-30 17:17:09.000000 enigmacrypt-0.0.3/app/enigmacrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.373151 enigmacrypt-0.0.3/enigmacrypt.egg-info/
--rw-rw-rw-   0        0        0     2511 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 18:11:20.375152 enigmacrypt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-06-30 16:03:21.000000 enigmacrypt-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.879362 enigmacrypt-0.0.4/
+-rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:14.000000 enigmacrypt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2511 2023-06-30 20:35:53.879362 enigmacrypt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:14.000000 enigmacrypt-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.870651 enigmacrypt-0.0.4/app/
+-rw-rw-rw-   0        0        0       23 2023-06-30 20:35:52.000000 enigmacrypt-0.0.4/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.872157 enigmacrypt-0.0.4/app/enigmacrypt/
+-rw-rw-rw-   0        0        0      119 2023-06-30 18:25:58.000000 enigmacrypt-0.0.4/app/enigmacrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:35:53.878328 enigmacrypt-0.0.4/enigmacrypt.egg-info/
+-rw-rw-rw-   0        0        0     2511 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-30 20:35:53.000000 enigmacrypt-0.0.4/enigmacrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 20:35:53.879362 enigmacrypt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-06-30 20:35:52.000000 enigmacrypt-0.0.4/setup.py
```

### Comparing `enigmacrypt-0.0.3/LICENSE` & `enigmacrypt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.3/PKG-INFO` & `enigmacrypt-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `enigmacrypt-0.0.3/README.md` & `enigmacrypt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.3/enigmacrypt.egg-info/PKG-INFO` & `enigmacrypt-0.0.4/enigmacrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `enigmacrypt-0.0.3/setup.py` & `enigmacrypt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Encoding and decoding strings using keys'
 
 # Setting up
 setup(
     name="enigmacrypt",
     version=VERSION,
     author="WooksCode (Wojciech Karwowski)",
```

