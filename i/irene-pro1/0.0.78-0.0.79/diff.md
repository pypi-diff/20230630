# Comparing `tmp/irene_pro1-0.0.78.tar.gz` & `tmp/irene_pro1-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro1-0.0.78.tar", last modified: Fri Jun 30 07:38:08 2023, max compression
+gzip compressed data, was "irene_pro1-0.0.79.tar", last modified: Fri Jun 30 08:36:12 2023, max compression
```

## Comparing `irene_pro1-0.0.78.tar` & `irene_pro1-0.0.79.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:38:08.811100 irene_pro1-0.0.78/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro1-0.0.78/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro1-0.0.78/MANIFEST.in
--rw-rw-rw-   0        0        0     1281 2023-06-30 07:38:08.809116 irene_pro1-0.0.78/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro1-0.0.78/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 07:38:08.761231 irene_pro1-0.0.78/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro1-0.0.78/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     5918 2023-06-30 07:20:45.000000 irene_pro1-0.0.78/irene_pro/logics.py
--rw-rw-rw-   0        0        0    36957 2023-06-30 07:18:16.000000 irene_pro1-0.0.78/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:38:08.805116 irene_pro1-0.0.78/irene_pro1.egg-info/
--rw-rw-rw-   0        0        0     1281 2023-06-30 07:38:08.000000 irene_pro1-0.0.78/irene_pro1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-30 07:38:08.000000 irene_pro1-0.0.78/irene_pro1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:38:08.000000 irene_pro1-0.0.78/irene_pro1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-30 07:38:08.000000 irene_pro1-0.0.78/irene_pro1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-30 07:38:08.000000 irene_pro1-0.0.78/irene_pro1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:38:08.812111 irene_pro1-0.0.78/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-06-30 07:35:51.000000 irene_pro1-0.0.78/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:36:12.186113 irene_pro1-0.0.79/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro1-0.0.79/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro1-0.0.79/MANIFEST.in
+-rw-rw-rw-   0        0        0     1281 2023-06-30 08:36:12.183086 irene_pro1-0.0.79/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro1-0.0.79/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 08:36:12.148178 irene_pro1-0.0.79/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro1-0.0.79/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     5918 2023-06-30 07:20:45.000000 irene_pro1-0.0.79/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    36831 2023-06-30 08:35:02.000000 irene_pro1-0.0.79/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:36:12.177224 irene_pro1-0.0.79/irene_pro1.egg-info/
+-rw-rw-rw-   0        0        0     1281 2023-06-30 08:36:12.000000 irene_pro1-0.0.79/irene_pro1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-30 08:36:12.000000 irene_pro1-0.0.79/irene_pro1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 08:36:12.000000 irene_pro1-0.0.79/irene_pro1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-30 08:36:12.000000 irene_pro1-0.0.79/irene_pro1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 08:36:12.000000 irene_pro1-0.0.79/irene_pro1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 08:36:12.187075 irene_pro1-0.0.79/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-06-30 08:35:15.000000 irene_pro1-0.0.79/setup.py
```

### Comparing `irene_pro1-0.0.78/PKG-INFO` & `irene_pro1-0.0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro1
-Version: 0.0.78
+Version: 0.0.79
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro1-0.0.78/README.md` & `irene_pro1-0.0.79/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro1-0.0.78/irene_pro/logics.py` & `irene_pro1-0.0.79/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro1-0.0.78/irene_pro/widgets.py` & `irene_pro1-0.0.79/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,19 +47,18 @@
     
 class Validate:
     def __init__(self) -> None:
         pass
 
     def validate_email(self, email):
         email = email.strip()
-        if "@gmail.com" in email and not email[0] not in punctuations and " " not in email:
+        if "@" in email and '.com' in email and email[0] not in punctuations and " " not in email:
             return True
-        elif "@" in email and '.com' in email and "gmail" not in email and email[0] not in punctuations and " " not in email:
-            return True
-        return False
+        else:
+            return False
     
     def all_are_numbers(self, value):
         nums = [str(i) for i in range(10)]
         decision = True
         for i in str(value):
             if i not in nums:
                 decision = False
```

### Comparing `irene_pro1-0.0.78/irene_pro1.egg-info/PKG-INFO` & `irene_pro1-0.0.79/irene_pro1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro1
-Version: 0.0.78
+Version: 0.0.79
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro1-0.0.78/setup.py` & `irene_pro1-0.0.79/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3738 270d 0a44 4553 4352   '0.0.78'..DESCR
+00000100: 2027 302e 302e 3739 270d 0a44 4553 4352   '0.0.79'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

