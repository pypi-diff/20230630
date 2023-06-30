# Comparing `tmp/Generation_Image_Gaston-0.1.6.tar.gz` & `tmp/Generation_Image_Gaston-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Generation_Image_Gaston-0.1.6.tar", last modified: Fri Jun 30 07:58:21 2023, max compression
+gzip compressed data, was "Generation_Image_Gaston-0.1.8.tar", last modified: Fri Jun 30 09:27:50 2023, max compression
```

## Comparing `Generation_Image_Gaston-0.1.6.tar` & `Generation_Image_Gaston-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:21.738791 Generation_Image_Gaston-0.1.6/
--rw-rw-rw-   0        0        0       82 2023-06-29 18:15:17.000000 Generation_Image_Gaston-0.1.6/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:21.725866 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston/
--rw-rw-rw-   0        0        0     2892 2023-06-30 07:37:34.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:58:21.736793 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/
--rw-rw-rw-   0        0        0      466 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1064 2023-06-29 18:10:48.000000 Generation_Image_Gaston-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 18:14:08.000000 Generation_Image_Gaston-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      466 2023-06-30 07:58:21.738791 Generation_Image_Gaston-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 07:58:21.739788 Generation_Image_Gaston-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-06-30 07:41:10.000000 Generation_Image_Gaston-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:27:50.208461 Generation_Image_Gaston-0.1.8/
+-rw-rw-rw-   0        0        0       82 2023-06-29 18:15:17.000000 Generation_Image_Gaston-0.1.8/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 09:27:50.182053 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston/
+-rw-rw-rw-   0        0        0     2892 2023-06-30 07:37:34.000000 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:27:50.206461 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston.egg-info/
+-rw-rw-rw-   0        0        0     2160 2023-06-30 09:27:50.000000 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-30 09:27:50.000000 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:27:50.000000 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-30 09:27:50.000000 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-30 09:27:50.000000 Generation_Image_Gaston-0.1.8/Generation_Image_Gaston.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1064 2023-06-29 18:10:48.000000 Generation_Image_Gaston-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:14:08.000000 Generation_Image_Gaston-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2160 2023-06-30 09:27:50.207466 Generation_Image_Gaston-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1497 2023-06-30 09:21:00.000000 Generation_Image_Gaston-0.1.8/README.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:27:50.208461 Generation_Image_Gaston-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-06-30 09:27:37.000000 Generation_Image_Gaston-0.1.8/setup.py
```

### Comparing `Generation_Image_Gaston-0.1.6/Generation_Image_Gaston/__init__.py` & `Generation_Image_Gaston-0.1.8/Generation_Image_Gaston/__init__.py`

 * *Files identical despite different names*

### Comparing `Generation_Image_Gaston-0.1.6/LICENSE.txt` & `Generation_Image_Gaston-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Generation_Image_Gaston-0.1.6/setup.py` & `Generation_Image_Gaston-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,20 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Generation_Image_Gaston',
-    version='0.1.6',
+    version='0.1.8',
     packages=['Generation_Image_Gaston'],
     install_requires=[
         'selenium',
         'undetected_chromedriver'
     ],
     author='Gaston Robé',
     author_email='gaston01.robe@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords='Gaston Image',
+    keywords='GASTON PROCESSING COMPUTER VISION',
+    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 )
```

