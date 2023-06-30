# Comparing `tmp/AFR-0.2.4.tar.gz` & `tmp/AFR-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AFR-0.2.4.tar", last modified: Thu Jun 29 20:20:13 2023, max compression
+gzip compressed data, was "dist/AFR-0.2.5.tar", last modified: Fri Jun 30 02:39:25 2023, max compression
```

## Comparing `AFR-0.2.4.tar` & `AFR-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-29 20:20:13.926652 AFR-0.2.4/
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-29 20:20:13.910106 AFR-0.2.4/AFR/
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-29 20:20:13.918425 AFR-0.2.4/AFR/AFR.egg-info/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-29 20:20:13.000000 AFR-0.2.4/AFR/AFR.egg-info/PKG-INFO
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      402 2023-06-29 20:20:13.000000 AFR-0.2.4/AFR/AFR.egg-info/SOURCES.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-29 20:20:13.000000 AFR-0.2.4/AFR/AFR.egg-info/dependency_links.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)       87 2023-06-29 20:20:13.000000 AFR-0.2.4/AFR/AFR.egg-info/requires.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-29 20:20:13.000000 AFR-0.2.4/AFR/AFR.egg-info/top_level.txt
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-29 20:20:13.925266 AFR-0.2.4/AFR/load/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    62311 2023-06-21 10:38:03.000000 AFR-0.2.4/AFR/load/finratKZ.csv
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    10137 2023-02-28 06:28:15.000000 AFR-0.2.4/AFR/load/finratKZ_dataset.html
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1843 2023-03-15 10:12:56.000000 AFR-0.2.4/AFR/load/finratKZ_dataset.rst
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    19643 2023-06-13 10:48:38.000000 AFR-0.2.4/AFR/load/macroKZ.csv
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13295 2023-03-28 09:46:08.000000 AFR-0.2.4/AFR/load/macroKZ_dataset.html
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     4178 2023-03-28 09:43:27.000000 AFR-0.2.4/AFR/load/macroKZ_dataset.rst
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14541 2023-06-19 13:01:26.000000 AFR-0.2.4/AFR manual.md
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1878 2023-03-25 06:06:59.000000 AFR-0.2.4/LICENSE.rtf
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      123 2023-06-29 20:01:11.000000 AFR-0.2.4/MANIFEST.in
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-29 20:20:13.926252 AFR-0.2.4/PKG-INFO
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)   105732 2023-03-25 08:12:22.000000 AFR-0.2.4/example_process.ipynb
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      159 2023-06-29 19:54:34.000000 AFR-0.2.4/requirements.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)       38 2023-06-29 20:20:13.926779 AFR-0.2.4/setup.cfg
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      959 2023-06-29 19:57:12.000000 AFR-0.2.4/setup.py
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 02:39:25.918680 AFR-0.2.5/
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 02:39:25.902495 AFR-0.2.5/AFR/
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 02:39:25.910665 AFR-0.2.5/AFR/AFR.egg-info/
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-30 02:39:25.000000 AFR-0.2.5/AFR/AFR.egg-info/PKG-INFO
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      402 2023-06-30 02:39:25.000000 AFR-0.2.5/AFR/AFR.egg-info/SOURCES.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-30 02:39:25.000000 AFR-0.2.5/AFR/AFR.egg-info/dependency_links.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)       87 2023-06-30 02:39:25.000000 AFR-0.2.5/AFR/AFR.egg-info/requires.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-30 02:39:25.000000 AFR-0.2.5/AFR/AFR.egg-info/top_level.txt
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 02:39:25.917126 AFR-0.2.5/AFR/load/
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    62311 2023-06-21 10:38:03.000000 AFR-0.2.5/AFR/load/finratKZ.csv
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    10137 2023-02-28 06:28:15.000000 AFR-0.2.5/AFR/load/finratKZ_dataset.html
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1843 2023-03-15 10:12:56.000000 AFR-0.2.5/AFR/load/finratKZ_dataset.rst
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    19643 2023-06-13 10:48:38.000000 AFR-0.2.5/AFR/load/macroKZ.csv
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13295 2023-03-28 09:46:08.000000 AFR-0.2.5/AFR/load/macroKZ_dataset.html
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     4178 2023-03-28 09:43:27.000000 AFR-0.2.5/AFR/load/macroKZ_dataset.rst
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14541 2023-06-19 13:01:26.000000 AFR-0.2.5/AFR manual.md
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1878 2023-03-25 06:06:59.000000 AFR-0.2.5/LICENSE.rtf
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      123 2023-06-29 20:01:11.000000 AFR-0.2.5/MANIFEST.in
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-30 02:39:25.918249 AFR-0.2.5/PKG-INFO
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)   105732 2023-03-25 08:12:22.000000 AFR-0.2.5/example_process.ipynb
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      159 2023-06-29 19:54:34.000000 AFR-0.2.5/requirements.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)       38 2023-06-30 02:39:25.918806 AFR-0.2.5/setup.cfg
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      959 2023-06-30 02:36:12.000000 AFR-0.2.5/setup.py
```

### Comparing `AFR-0.2.4/AFR/AFR.egg-info/PKG-INFO` & `AFR-0.2.5/AFR/AFR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AFR
-Version: 0.2.4
+Version: 0.2.5
 Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
 Home-page: https://github.com/AFRKZ/AFR
 Author: Timur Abilkassymov, Alua Makhmetova
 Author-email: alua.makhmetova@gmail.com
 License: 3-clause BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.rtf
```

### Comparing `AFR-0.2.4/AFR/load/finratKZ.csv` & `AFR-0.2.5/AFR/load/finratKZ.csv`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/AFR/load/finratKZ_dataset.html` & `AFR-0.2.5/AFR/load/finratKZ_dataset.html`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/AFR/load/finratKZ_dataset.rst` & `AFR-0.2.5/AFR/load/finratKZ_dataset.rst`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/AFR/load/macroKZ.csv` & `AFR-0.2.5/AFR/load/macroKZ.csv`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/AFR/load/macroKZ_dataset.html` & `AFR-0.2.5/AFR/load/macroKZ_dataset.html`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/AFR/load/macroKZ_dataset.rst` & `AFR-0.2.5/AFR/load/macroKZ_dataset.rst`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/AFR manual.md` & `AFR-0.2.5/AFR manual.md`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/LICENSE.rtf` & `AFR-0.2.5/LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/PKG-INFO` & `AFR-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AFR
-Version: 0.2.4
+Version: 0.2.5
 Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
 Home-page: https://github.com/AFRKZ/AFR
 Author: Timur Abilkassymov, Alua Makhmetova
 Author-email: alua.makhmetova@gmail.com
 License: 3-clause BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.rtf
```

### Comparing `AFR-0.2.4/example_process.ipynb` & `AFR-0.2.5/example_process.ipynb`

 * *Files identical despite different names*

### Comparing `AFR-0.2.4/setup.py` & `AFR-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AFR manual.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='AFR',
-    version='0.2.4',
+    version='0.2.5',
     description='Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data',
     author='Timur Abilkassymov, Alua Makhmetova',
     author_email='alua.makhmetova@gmail.com',
     url='https://github.com/AFRKZ/AFR',
     license="3-clause BSD",
     packages=find_packages(where="AFR"),
     install_requires=[
```

