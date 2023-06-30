# Comparing `tmp/enigmacrypt-0.0.2.tar.gz` & `tmp/enigmacrypt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enigmacrypt-0.0.2.tar", last modified: Thu Jun 29 20:42:26 2023, max compression
+gzip compressed data, was "enigmacrypt-0.0.3.tar", last modified: Fri Jun 30 18:11:20 2023, max compression
```

## Comparing `enigmacrypt-0.0.2.tar` & `enigmacrypt-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.867506 enigmacrypt-0.0.2/
--rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:14.000000 enigmacrypt-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2510 2023-06-29 20:42:26.865508 enigmacrypt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:14.000000 enigmacrypt-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.851163 enigmacrypt-0.0.2/app/
--rw-rw-rw-   0        0        0        0 2023-06-29 19:51:33.000000 enigmacrypt-0.0.2/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.852164 enigmacrypt-0.0.2/app/enigmacrypt/
--rw-rw-rw-   0        0        0       82 2023-06-29 20:06:55.000000 enigmacrypt-0.0.2/app/enigmacrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:42:26.860445 enigmacrypt-0.0.2/enigmacrypt.egg-info/
--rw-rw-rw-   0        0        0     2510 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 20:42:26.000000 enigmacrypt-0.0.2/enigmacrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 20:42:26.868503 enigmacrypt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-06-29 20:42:01.000000 enigmacrypt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.375152 enigmacrypt-0.0.3/
+-rw-rw-rw-   0        0        0     1096 2023-06-29 20:42:14.000000 enigmacrypt-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2511 2023-06-30 18:11:20.374153 enigmacrypt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-06-29 20:42:14.000000 enigmacrypt-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.365385 enigmacrypt-0.0.3/app/
+-rw-rw-rw-   0        0        0       23 2023-06-30 16:03:21.000000 enigmacrypt-0.0.3/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.366892 enigmacrypt-0.0.3/app/enigmacrypt/
+-rw-rw-rw-   0        0        0      116 2023-06-30 17:17:09.000000 enigmacrypt-0.0.3/app/enigmacrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:11:20.373151 enigmacrypt-0.0.3/enigmacrypt.egg-info/
+-rw-rw-rw-   0        0        0     2511 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-30 18:11:20.000000 enigmacrypt-0.0.3/enigmacrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 18:11:20.375152 enigmacrypt-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-06-30 16:03:21.000000 enigmacrypt-0.0.3/setup.py
```

### Comparing `enigmacrypt-0.0.2/LICENSE` & `enigmacrypt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.2/PKG-INFO` & `enigmacrypt-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.07
 Description-Content-Type: text/markdown
```

### Comparing `enigmacrypt-0.0.2/README.md` & `enigmacrypt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `enigmacrypt-0.0.2/enigmacrypt.egg-info/PKG-INFO` & `enigmacrypt-0.0.3/enigmacrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: enigmacrypt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Encoding and decoding strings using keys
 Home-page: https://github.com/Wooks08/EnigmaCrypt
 Author: WooksCode (Wojciech Karwowski)
 Author-email: <wookscode.kontakt@gmail.com>
 License: MIT
 Keywords: python,encode,decode,decoder,encoder,string encryption,string decryption
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.07
 Description-Content-Type: text/markdown
```

### Comparing `enigmacrypt-0.0.2/setup.py` & `enigmacrypt-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     LONG_DESCRIPTION = f.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Encoding and decoding strings using keys'
 
 # Setting up
 setup(
     name="enigmacrypt",
     version=VERSION,
     author="WooksCode (Wojciech Karwowski)",
@@ -21,15 +21,15 @@
     python_requires=">=3.07",
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"]
     },
     keywords=['python', 'encode', 'decode', 'decoder',
               'encoder', 'string encryption', 'string decryption'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

