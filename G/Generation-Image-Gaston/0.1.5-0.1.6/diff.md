# Comparing `tmp/Generation_Image_Gaston-0.1.5.tar.gz` & `tmp/Generation_Image_Gaston-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Generation_Image_Gaston-0.1.5.tar", last modified: Fri Jun 30 07:08:54 2023, max compression
+gzip compressed data, was "Generation_Image_Gaston-0.1.6.tar", last modified: Fri Jun 30 07:58:21 2023, max compression
```

## Comparing `Generation_Image_Gaston-0.1.5.tar` & `Generation_Image_Gaston-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:08:54.279374 Generation_Image_Gaston-0.1.5/
--rw-rw-rw-   0        0        0       82 2023-06-29 18:15:17.000000 Generation_Image_Gaston-0.1.5/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 07:08:54.257138 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston/
--rw-rw-rw-   0        0        0     2891 2023-06-30 06:57:40.000000 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:08:54.277321 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston.egg-info/
--rw-rw-rw-   0        0        0      466 2023-06-30 07:08:54.000000 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-30 07:08:54.000000 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:08:54.000000 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-30 07:08:54.000000 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-30 07:08:54.000000 Generation_Image_Gaston-0.1.5/Generation_Image_Gaston.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1064 2023-06-29 18:10:48.000000 Generation_Image_Gaston-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 18:14:08.000000 Generation_Image_Gaston-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      466 2023-06-30 07:08:54.278379 Generation_Image_Gaston-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-30 07:08:54.279374 Generation_Image_Gaston-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-06-30 07:08:15.000000 Generation_Image_Gaston-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:21.738791 Generation_Image_Gaston-0.1.6/
+-rw-rw-rw-   0        0        0       82 2023-06-29 18:15:17.000000 Generation_Image_Gaston-0.1.6/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:21.725866 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston/
+-rw-rw-rw-   0        0        0     2892 2023-06-30 07:37:34.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:58:21.736793 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/
+-rw-rw-rw-   0        0        0      466 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-30 07:58:21.000000 Generation_Image_Gaston-0.1.6/Generation_Image_Gaston.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1064 2023-06-29 18:10:48.000000 Generation_Image_Gaston-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:14:08.000000 Generation_Image_Gaston-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      466 2023-06-30 07:58:21.738791 Generation_Image_Gaston-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:58:21.739788 Generation_Image_Gaston-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-06-30 07:41:10.000000 Generation_Image_Gaston-0.1.6/setup.py
```

### Comparing `Generation_Image_Gaston-0.1.5/Generation_Image_Gaston/__init__.py` & `Generation_Image_Gaston-0.1.6/Generation_Image_Gaston/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,12 +51,12 @@
     image = drivers.find_element(By.XPATH, """//*[@id="app"]/div[2]/div/div[3]/div/div/div/div[1]/div[1]/img""")
     image.click()
     downloadButton = drivers.find_element(By.XPATH, """//*[@id="main"]/main/div/div/div[2]/div[2]/div/div[2]/div[1]/div/button[1]""")
     drivers.execute_script("arguments[0].scrollIntoView();", downloadButton)
     downloadButton.click()
     time.sleep(20)
     try:
-        drivers.quit()
+        drivers.close()
         print("Le téléchargement est finie")
     except:
         pass
```

### Comparing `Generation_Image_Gaston-0.1.5/LICENSE.txt` & `Generation_Image_Gaston-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Generation_Image_Gaston-0.1.5/setup.py` & `Generation_Image_Gaston-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Generation_Image_Gaston',
-    version='0.1.5',
+    version='0.1.6',
     packages=['Generation_Image_Gaston'],
     install_requires=[
         'selenium',
         'undetected_chromedriver'
     ],
     author='Gaston Robé',
     author_email='gaston01.robe@gmail.com',
```

