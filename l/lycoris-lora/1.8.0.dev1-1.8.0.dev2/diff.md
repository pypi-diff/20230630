# Comparing `tmp/lycoris_lora-1.8.0.dev1.tar.gz` & `tmp/lycoris_lora-1.8.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.0.dev1.tar", last modified: Wed Jun 28 16:02:07 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.0.dev2.tar", last modified: Fri Jun 30 13:57:22 2023, max compression
```

## Comparing `lycoris_lora-1.8.0.dev1.tar` & `lycoris_lora-1.8.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 16:02:07.801101 lycoris_lora-1.8.0.dev1/
--rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev1/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-28 16:02:07.801101 lycoris_lora-1.8.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 16:02:07.785065 lycoris_lora-1.8.0.dev1/lycoris/
--rw-rw-rw-   0        0        0       62 2023-06-28 13:25:50.000000 lycoris_lora-1.8.0.dev1/lycoris/__init__.py
--rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev1/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 16:02:07.800101 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-28 16:02:07.000000 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-28 16:02:07.000000 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 16:02:07.000000 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-28 16:02:07.000000 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-28 16:02:07.000000 lycoris_lora-1.8.0.dev1/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 16:02:07.802101 lycoris_lora-1.8.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-28 13:21:49.000000 lycoris_lora-1.8.0.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:57:22.102915 lycoris_lora-1.8.0.dev2/
+-rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev2/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-30 13:57:22.101891 lycoris_lora-1.8.0.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     7677 2023-06-28 12:51:02.000000 lycoris_lora-1.8.0.dev2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 13:57:22.096132 lycoris_lora-1.8.0.dev2/lycoris/
+-rw-rw-rw-   0        0        0       62 2023-06-29 04:44:57.000000 lycoris_lora-1.8.0.dev2/lycoris/__init__.py
+-rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-1.8.0.dev2/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:57:22.101891 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-30 13:57:21.000000 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-30 13:57:22.000000 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 13:57:21.000000 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-30 13:57:21.000000 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 13:57:21.000000 lycoris_lora-1.8.0.dev2/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 13:57:22.102915 lycoris_lora-1.8.0.dev2/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-30 12:31:27.000000 lycoris_lora-1.8.0.dev2/setup.py
```

### Comparing `lycoris_lora-1.8.0.dev1/LICENSE.md` & `lycoris_lora-1.8.0.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev1/README.md` & `lycoris_lora-1.8.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev1/lycoris/utils.py` & `lycoris_lora-1.8.0.dev2/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev1/setup.py` & `lycoris_lora-1.8.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='1.8.0.dev1',
+    version='1.8.0.dev2',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

