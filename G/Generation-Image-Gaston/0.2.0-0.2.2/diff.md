# Comparing `tmp/Generation_Image_Gaston-0.2.0.tar.gz` & `tmp/Generation_Image_Gaston-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Generation_Image_Gaston-0.2.0.tar", last modified: Fri Jun 30 09:36:40 2023, max compression
+gzip compressed data, was "Generation_Image_Gaston-0.2.2.tar", last modified: Fri Jun 30 09:43:42 2023, max compression
```

## Comparing `Generation_Image_Gaston-0.2.0.tar` & `Generation_Image_Gaston-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:36:40.011979 Generation_Image_Gaston-0.2.0/
--rw-rw-rw-   0        0        0       82 2023-06-29 18:15:17.000000 Generation_Image_Gaston-0.2.0/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 09:36:39.986192 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston/
--rw-rw-rw-   0        0        0     2892 2023-06-30 07:37:34.000000 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:36:40.008475 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/
--rw-rw-rw-   0        0        0     1905 2023-06-30 09:36:39.000000 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-30 09:36:39.000000 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:36:39.000000 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-30 09:36:39.000000 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-30 09:36:39.000000 Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1064 2023-06-29 18:10:48.000000 Generation_Image_Gaston-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 18:14:08.000000 Generation_Image_Gaston-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1905 2023-06-30 09:36:40.008475 Generation_Image_Gaston-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2023-06-30 09:35:01.000000 Generation_Image_Gaston-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 09:36:40.011979 Generation_Image_Gaston-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-06-30 09:36:34.000000 Generation_Image_Gaston-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:43:42.417832 Generation_Image_Gaston-0.2.2/
+-rw-rw-rw-   0        0        0       82 2023-06-29 18:15:17.000000 Generation_Image_Gaston-0.2.2/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 09:43:42.397763 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston/
+-rw-rw-rw-   0        0        0     2892 2023-06-30 07:37:34.000000 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:43:42.415838 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/
+-rw-rw-rw-   0        0        0     1889 2023-06-30 09:43:42.000000 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-30 09:43:42.000000 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:43:42.000000 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-30 09:43:42.000000 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-30 09:43:42.000000 Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1064 2023-06-29 18:10:48.000000 Generation_Image_Gaston-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:14:08.000000 Generation_Image_Gaston-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1889 2023-06-30 09:43:42.416834 Generation_Image_Gaston-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1320 2023-06-30 09:39:03.000000 Generation_Image_Gaston-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:43:42.417832 Generation_Image_Gaston-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-06-30 09:43:39.000000 Generation_Image_Gaston-0.2.2/setup.py
```

### Comparing `Generation_Image_Gaston-0.2.0/Generation_Image_Gaston/__init__.py` & `Generation_Image_Gaston-0.2.2/Generation_Image_Gaston/__init__.py`

 * *Files identical despite different names*

### Comparing `Generation_Image_Gaston-0.2.0/Generation_Image_Gaston.egg-info/PKG-INFO` & `Generation_Image_Gaston-0.2.2/Generation_Image_Gaston.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: Generation-Image-Gaston
-Version: 0.2.0
+Version: 0.2.2
 Author: Gaston Robé
 Author-email: gaston01.robe@gmail.com
 License: MIT
-Keywords: Gaston Robe 13 ans
+Keywords: Capitain America Avengers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
-# Generation-image_Gaston
-## Description
-GÃ©nÃ©ration-image_Gaston is a Python package that allows you to generate images from a given prompt using the craiyon.com site. This package uses Selenium to automate the image build and upload process.
+Generation-image_Gaston
+Description
+Generation-image_Gaston is a Python package that allows you to generate images from a given prompt using the craiyon.com site. This package uses Selenium to automate the image build and upload process.
 
-## Facility
-You can install the GÃ©nÃ©ration-image_Gaston package using pip:
+Facility
+You can install the Generation-image_Gaston package using pip:
 
 pip install Generation-image_Gaston
 Make sure you have the following dependencies installed:
 
 undetected_chromedriver
 selenium
 It settles down on its own normally.
-## Use
+Use
 Here is an example of using the package:
 
 
 from Generation_Image_Gaston import SelectStyle
 
 SelectStyle("Three Crying Cat...", "PHOTO")
 The SelectStyle function takes two parameters:
```

### Comparing `Generation_Image_Gaston-0.2.0/LICENSE.txt` & `Generation_Image_Gaston-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Generation_Image_Gaston-0.2.0/PKG-INFO` & `Generation_Image_Gaston-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: Generation_Image_Gaston
-Version: 0.2.0
+Version: 0.2.2
 Author: Gaston Robé
 Author-email: gaston01.robe@gmail.com
 License: MIT
-Keywords: Gaston Robe 13 ans
+Keywords: Capitain America Avengers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
-# Generation-image_Gaston
-## Description
-GÃ©nÃ©ration-image_Gaston is a Python package that allows you to generate images from a given prompt using the craiyon.com site. This package uses Selenium to automate the image build and upload process.
+Generation-image_Gaston
+Description
+Generation-image_Gaston is a Python package that allows you to generate images from a given prompt using the craiyon.com site. This package uses Selenium to automate the image build and upload process.
 
-## Facility
-You can install the GÃ©nÃ©ration-image_Gaston package using pip:
+Facility
+You can install the Generation-image_Gaston package using pip:
 
 pip install Generation-image_Gaston
 Make sure you have the following dependencies installed:
 
 undetected_chromedriver
 selenium
 It settles down on its own normally.
-## Use
+Use
 Here is an example of using the package:
 
 
 from Generation_Image_Gaston import SelectStyle
 
 SelectStyle("Three Crying Cat...", "PHOTO")
 The SelectStyle function takes two parameters:
```

### Comparing `Generation_Image_Gaston-0.2.0/README.md` & `Generation_Image_Gaston-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generation-image_Gaston
-## Description
-Génération-image_Gaston is a Python package that allows you to generate images from a given prompt using the craiyon.com site. This package uses Selenium to automate the image build and upload process.
+Generation-image_Gaston
+Description
+Generation-image_Gaston is a Python package that allows you to generate images from a given prompt using the craiyon.com site. This package uses Selenium to automate the image build and upload process.
 
-## Facility
-You can install the Génération-image_Gaston package using pip:
+Facility
+You can install the Generation-image_Gaston package using pip:
 
 pip install Generation-image_Gaston
 Make sure you have the following dependencies installed:
 
 undetected_chromedriver
 selenium
 It settles down on its own normally.
-## Use
+Use
 Here is an example of using the package:
 
 
 from Generation_Image_Gaston import SelectStyle
 
 SelectStyle("Three Crying Cat...", "PHOTO")
 The SelectStyle function takes two parameters:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Generation_Image_Gaston-0.2.0/setup.py` & `Generation_Image_Gaston-0.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,20 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Generation_Image_Gaston',
-    version='0.2.0',
+    version='0.2.2',
     packages=['Generation_Image_Gaston'],
     install_requires=[
         'selenium',
         'undetected_chromedriver'
     ],
     author='Gaston Robé',
     author_email='gaston01.robe@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords='Gaston Robe 13 ans',
+    keywords='Capitain America Avengers',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
 )
```

