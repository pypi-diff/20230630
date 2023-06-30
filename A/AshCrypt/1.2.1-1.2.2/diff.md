# Comparing `tmp/AshCrypt-1.2.1.tar.gz` & `tmp/AshCrypt-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.2.1.tar", last modified: Thu Jun 29 13:13:10 2023, max compression
+gzip compressed data, was "AshCrypt-1.2.2.tar", last modified: Fri Jun 30 14:23:14 2023, max compression
```

## Comparing `AshCrypt-1.2.1.tar` & `AshCrypt-1.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.691218 AshCrypt-1.2.1/
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.669014 AshCrypt-1.2.1/AshCrypt/
--rw-rw-rw-   0        0        0     5157 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    35745 2023-06-28 15:21:31.000000 AshCrypt-1.2.1/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     8855 2023-06-29 12:59:01.000000 AshCrypt-1.2.1/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     4128 2023-06-27 15:57:29.000000 AshCrypt-1.2.1/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2074 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     6660 2023-06-29 12:50:18.000000 AshCrypt-1.2.1/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    18472 2023-06-29 13:08:37.000000 AshCrypt-1.2.1/AshCrypt/README.md
--rw-rw-rw-   0        0        0       91 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-17 18:15:01.000000 AshCrypt-1.2.1/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.686390 AshCrypt-1.2.1/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-27 15:57:29.000000 AshCrypt-1.2.1/AshCrypt/unittests/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-06-27 15:57:29.000000 AshCrypt-1.2.1/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:13:10.681802 AshCrypt-1.2.1/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    19499 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 13:13:10.000000 AshCrypt-1.2.1/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    19499 2023-06-29 13:13:10.691218 AshCrypt-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    21651 2023-06-29 13:08:37.000000 AshCrypt-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 13:13:10.692231 AshCrypt-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1629 2023-06-29 13:08:37.000000 AshCrypt-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:23:14.964053 AshCrypt-1.2.2/
+drwxrwxrwx   0        0        0        0 2023-06-30 14:23:14.891928 AshCrypt-1.2.2/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    35745 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     8854 2023-06-30 14:21:04.000000 AshCrypt-1.2.2/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     4128 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2074 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     6660 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    18472 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       91 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:23:14.958855 AshCrypt-1.2.2/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:23:14.903975 AshCrypt-1.2.2/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    19499 2023-06-30 14:23:14.000000 AshCrypt-1.2.2/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-06-30 14:23:14.000000 AshCrypt-1.2.2/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:23:14.000000 AshCrypt-1.2.2/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-30 14:23:14.000000 AshCrypt-1.2.2/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 14:23:14.000000 AshCrypt-1.2.2/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0    19499 2023-06-30 14:23:14.962879 AshCrypt-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    21651 2023-06-30 14:17:27.000000 AshCrypt-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:23:14.964564 AshCrypt-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1629 2023-06-30 14:22:52.000000 AshCrypt-1.2.2/setup.py
```

### Comparing `AshCrypt-1.2.1/AshCrypt/Ash.py` & `AshCrypt-1.2.2/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.2.2/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/AshDatabase.py` & `AshCrypt-1.2.2/AshCrypt/AshDatabase.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,16 @@
             except sqlite3.Error as e:
                 return (0, e)
 
     def update(self, column_name: str, new_column_val: str, ID: int, optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
-                    self.c.execute((f'UPDATE {self.tablename} SET ? = ? WHERE ID = ? '),
-                                   (column_name, new_column_val, ID))
+                    self.c.execute((f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? '),
+                                   (new_column_val, ID))
                     return 11
 
             except sqlite3.Error as e:
                 return (0.0, e)
 
         else:
             try:
```

### Comparing `AshCrypt-1.2.1/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.2.2/AshCrypt/AshFileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.2.2/AshCrypt/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/CliCrypt.py` & `AshCrypt-1.2.2/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/README.md` & `AshCrypt-1.2.2/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/qr.py` & `AshCrypt-1.2.2/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-1.2.2/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.2.2/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.2.1/LICENSE` & `AshCrypt-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/PKG-INFO` & `AshCrypt-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.2.1
+Version: 1.2.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.2.1/README.md` & `AshCrypt-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.2.1/setup.py` & `AshCrypt-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.2.1',
+    version='1.2.2',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

