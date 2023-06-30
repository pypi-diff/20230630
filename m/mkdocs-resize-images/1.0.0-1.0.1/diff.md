# Comparing `tmp/mkdocs-resize-images-1.0.0.tar.gz` & `tmp/mkdocs-resize-images-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-resize-images-1.0.0.tar", last modified: Fri Jun 30 15:29:07 2023, max compression
+gzip compressed data, was "mkdocs-resize-images-1.0.1.tar", last modified: Fri Jun 30 16:20:42 2023, max compression
```

## Comparing `mkdocs-resize-images-1.0.0.tar` & `mkdocs-resize-images-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 15:29:07.572859 mkdocs-resize-images-1.0.0/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-06-30 13:14:40.000000 mkdocs-resize-images-1.0.0/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     3826 2023-06-30 15:29:07.572696 mkdocs-resize-images-1.0.0/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     3029 2023-06-30 15:09:20.000000 mkdocs-resize-images-1.0.0/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 15:29:07.572046 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     3826 2023-06-30 15:29:07.000000 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      342 2023-06-30 15:29:07.000000 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2023-06-30 15:29:07.000000 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       73 2023-06-30 15:29:07.000000 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/entry_points.txt
--rw-r--r--   0 kuba       (501) staff       (20)      119 2023-06-30 15:29:07.000000 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)       14 2023-06-30 15:29:07.000000 mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/top_level.txt
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 15:29:07.572279 mkdocs-resize-images-1.0.0/resize_images/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-03-26 20:51:00.000000 mkdocs-resize-images-1.0.0/resize_images/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     2785 2023-06-30 15:11:24.000000 mkdocs-resize-images-1.0.0/resize_images/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-06-30 15:29:07.572898 mkdocs-resize-images-1.0.0/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1412 2023-06-30 15:28:58.000000 mkdocs-resize-images-1.0.0/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 16:20:42.709214 mkdocs-resize-images-1.0.1/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-06-30 13:14:40.000000 mkdocs-resize-images-1.0.1/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     3812 2023-06-30 16:20:42.709068 mkdocs-resize-images-1.0.1/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     3015 2023-06-30 16:09:17.000000 mkdocs-resize-images-1.0.1/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 16:20:42.708450 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     3812 2023-06-30 16:20:42.000000 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)      342 2023-06-30 16:20:42.000000 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2023-06-30 16:20:42.000000 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       73 2023-06-30 16:20:42.000000 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      135 2023-06-30 16:20:42.000000 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       14 2023-06-30 16:20:42.000000 mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/top_level.txt
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 16:20:42.708701 mkdocs-resize-images-1.0.1/resize_images/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-03-26 20:51:00.000000 mkdocs-resize-images-1.0.1/resize_images/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2710 2023-06-30 15:39:53.000000 mkdocs-resize-images-1.0.1/resize_images/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-06-30 16:20:42.709273 mkdocs-resize-images-1.0.1/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1458 2023-06-30 16:19:07.000000 mkdocs-resize-images-1.0.1/setup.py
```

### Comparing `mkdocs-resize-images-1.0.0/LICENSE` & `mkdocs-resize-images-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-resize-images-1.0.0/PKG-INFO` & `mkdocs-resize-images-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-resize-images
-Version: 1.0.0
+Version: 1.0.1
 Summary: MkDocs plugin to resize images according to the configuration.
 Home-page: https://github.com/JakubAndrysek/mkdocs-resize-images
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Keywords: mkdocs plugin,resize images,mkdocs,plugin,images,resize
 Classifier: License :: OSI Approved :: MIT License
@@ -20,23 +20,23 @@
 License-File: LICENSE
 
 # MkDocs Resize Images Plugin
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-resize-images&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <img src="https://img.shields.io/github/license/JakubAndrysek/mkdocs-resize-images?style=flat-square">
-<img src="https://img.shields.io/github/v/release/JakubAndrysek/mkdocs-resize-images?style=flat-square">
+<img alt="PyPI" src="https://img.shields.io/pypi/v/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/stars/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://static.pepy.tech/personalized-badge/mkdocs-resize-images?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads">
 </p>
 
 This MkDocs plugin finds all folders with a certain name, by default `assets-large`, resizes all images in those folders according to the plugin configuration.
-Then saves the resized images in a different folder, by default `assets`. 
+Then saves the resized images in a different folder, by default `assets`.
 The plugin also supports caching: if a file has not changed since the last time the plugin ran, it won't be processed again.
 
 ## Installation
 
 Install the plugin using pip from [PyPI](https://pypi.org/project/mkdocs-resize-images/):
 
 ```bash
```

#### html2text {}

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1 Name: mkdocs-resize-images Version: 1.0.0 Summary: MkDocs
+Metadata-Version: 2.1 Name: mkdocs-resize-images Version: 1.0.1 Summary: MkDocs
 plugin to resize images according to the configuration. Home-page: https://
 github.com/JakubAndrysek/mkdocs-resize-images Author: Jakub AndrÃ½sek Author-
 email: email@kubaandrysek.cz License: MIT Keywords: mkdocs plugin,resize
 images,mkdocs,plugin,images,resize Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE # MkDocs Resize Images Plugin
                  [https://hits.seeyoufarm.com/api/count/incr/
     badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-resize-
 images&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
       [https://img.shields.io/github/license/JakubAndrysek/mkdocs-resize-
-      images?style=flat-square] [https://img.shields.io/github/v/release/
+    images?style=flat-square] [PyPI] [https://img.shields.io/github/stars/
 JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://img.shields.io/
- github/stars/JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://
-  img.shields.io/github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-
-  square] [https://img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-
-images?style=flat-square] [https://static.pepy.tech/personalized-badge/mkdocs-
-                                    resize-
+ github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://
+  img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-images?style=flat-
+      square] [https://static.pepy.tech/personalized-badge/mkdocs-resize-
 images?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads]
 This MkDocs plugin finds all folders with a certain name, by default `assets-
 large`, resizes all images in those folders according to the plugin
 configuration. Then saves the resized images in a different folder, by default
 `assets`. The plugin also supports caching: if a file has not changed since the
 last time the plugin ran, it won't be processed again. ## Installation Install
 the plugin using pip from [PyPI](https://pypi.org/project/mkdocs-resize-images/
```

### Comparing `mkdocs-resize-images-1.0.0/README.md` & `mkdocs-resize-images-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # MkDocs Resize Images Plugin
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-resize-images&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <img src="https://img.shields.io/github/license/JakubAndrysek/mkdocs-resize-images?style=flat-square">
-<img src="https://img.shields.io/github/v/release/JakubAndrysek/mkdocs-resize-images?style=flat-square">
+<img alt="PyPI" src="https://img.shields.io/pypi/v/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/stars/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://static.pepy.tech/personalized-badge/mkdocs-resize-images?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads">
 </p>
 
 This MkDocs plugin finds all folders with a certain name, by default `assets-large`, resizes all images in those folders according to the plugin configuration.
-Then saves the resized images in a different folder, by default `assets`. 
+Then saves the resized images in a different folder, by default `assets`.
 The plugin also supports caching: if a file has not changed since the last time the plugin ran, it won't be processed again.
 
 ## Installation
 
 Install the plugin using pip from [PyPI](https://pypi.org/project/mkdocs-resize-images/):
 
 ```bash
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
 # MkDocs Resize Images Plugin
                  [https://hits.seeyoufarm.com/api/count/incr/
     badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-resize-
 images&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
       [https://img.shields.io/github/license/JakubAndrysek/mkdocs-resize-
-      images?style=flat-square] [https://img.shields.io/github/v/release/
+    images?style=flat-square] [PyPI] [https://img.shields.io/github/stars/
 JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://img.shields.io/
- github/stars/JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://
-  img.shields.io/github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-
-  square] [https://img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-
-images?style=flat-square] [https://static.pepy.tech/personalized-badge/mkdocs-
-                                    resize-
+ github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://
+  img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-images?style=flat-
+      square] [https://static.pepy.tech/personalized-badge/mkdocs-resize-
 images?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads]
 This MkDocs plugin finds all folders with a certain name, by default `assets-
 large`, resizes all images in those folders according to the plugin
 configuration. Then saves the resized images in a different folder, by default
 `assets`. The plugin also supports caching: if a file has not changed since the
 last time the plugin ran, it won't be processed again. ## Installation Install
 the plugin using pip from [PyPI](https://pypi.org/project/mkdocs-resize-images/
```

### Comparing `mkdocs-resize-images-1.0.0/mkdocs_resize_images.egg-info/PKG-INFO` & `mkdocs-resize-images-1.0.1/mkdocs_resize_images.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-resize-images
-Version: 1.0.0
+Version: 1.0.1
 Summary: MkDocs plugin to resize images according to the configuration.
 Home-page: https://github.com/JakubAndrysek/mkdocs-resize-images
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Keywords: mkdocs plugin,resize images,mkdocs,plugin,images,resize
 Classifier: License :: OSI Approved :: MIT License
@@ -20,23 +20,23 @@
 License-File: LICENSE
 
 # MkDocs Resize Images Plugin
 
 <p align="center">
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-resize-images&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 <img src="https://img.shields.io/github/license/JakubAndrysek/mkdocs-resize-images?style=flat-square">
-<img src="https://img.shields.io/github/v/release/JakubAndrysek/mkdocs-resize-images?style=flat-square">
+<img alt="PyPI" src="https://img.shields.io/pypi/v/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/stars/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-images?style=flat-square">
 <img src="https://static.pepy.tech/personalized-badge/mkdocs-resize-images?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads">
 </p>
 
 This MkDocs plugin finds all folders with a certain name, by default `assets-large`, resizes all images in those folders according to the plugin configuration.
-Then saves the resized images in a different folder, by default `assets`. 
+Then saves the resized images in a different folder, by default `assets`.
 The plugin also supports caching: if a file has not changed since the last time the plugin ran, it won't be processed again.
 
 ## Installation
 
 Install the plugin using pip from [PyPI](https://pypi.org/project/mkdocs-resize-images/):
 
 ```bash
```

#### html2text {}

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1 Name: mkdocs-resize-images Version: 1.0.0 Summary: MkDocs
+Metadata-Version: 2.1 Name: mkdocs-resize-images Version: 1.0.1 Summary: MkDocs
 plugin to resize images according to the configuration. Home-page: https://
 github.com/JakubAndrysek/mkdocs-resize-images Author: Jakub AndrÃ½sek Author-
 email: email@kubaandrysek.cz License: MIT Keywords: mkdocs plugin,resize
 images,mkdocs,plugin,images,resize Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE # MkDocs Resize Images Plugin
                  [https://hits.seeyoufarm.com/api/count/incr/
     badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2Fmkdocs-resize-
 images&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
       [https://img.shields.io/github/license/JakubAndrysek/mkdocs-resize-
-      images?style=flat-square] [https://img.shields.io/github/v/release/
+    images?style=flat-square] [PyPI] [https://img.shields.io/github/stars/
 JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://img.shields.io/
- github/stars/JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://
-  img.shields.io/github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-
-  square] [https://img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-
-images?style=flat-square] [https://static.pepy.tech/personalized-badge/mkdocs-
-                                    resize-
+ github/forks/JakubAndrysek/mkdocs-resize-images?style=flat-square] [https://
+  img.shields.io/github/issues/JakubAndrysek/mkdocs-resize-images?style=flat-
+      square] [https://static.pepy.tech/personalized-badge/mkdocs-resize-
 images?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads]
 This MkDocs plugin finds all folders with a certain name, by default `assets-
 large`, resizes all images in those folders according to the plugin
 configuration. Then saves the resized images in a different folder, by default
 `assets`. The plugin also supports caching: if a file has not changed since the
 last time the plugin ran, it won't be processed again. ## Installation Install
 the plugin using pip from [PyPI](https://pypi.org/project/mkdocs-resize-images/
```

### Comparing `mkdocs-resize-images-1.0.0/resize_images/plugin.py` & `mkdocs-resize-images-1.0.1/resize_images/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Author: Jakub Andrýsek
 # Email: email@kubaandrysek.cz
 # Website: https://kubaandrysek.cz
 # License: MIT
 # GitHub: https://github.com/JakubAndrysek/mkdocs-resize-images
-# PyPI: https://pypi.org/project/mkdocs-open-in-new-tab/
-# Inspired by: https://github.com/timvink/mkdocs-charts-plugin/tree/main
+# PyPI: https://pypi.org/project/mkdocs-resize-images/
 
 from pathlib import Path
 from itertools import chain
 from PIL import Image
 import hashlib
 import logging
```

### Comparing `mkdocs-resize-images-1.0.0/setup.py` & `mkdocs-resize-images-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,33 @@
     with open('README.md') as f:
         return f.read()
 
 
 # https://pypi.org/project/mkdocs-resize-images/
 setup(
     name='mkdocs-resize-images',
-    version='1.0.0',
+    version='1.0.1',
     description='MkDocs plugin to resize images according to the configuration.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdocs plugin, resize images, mkdocs, plugin, images, resize',
     url='https://github.com/JakubAndrysek/mkdocs-resize-images',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
     license='MIT',
     python_requires='>=3.7',
-    install_requires=['mkdocs', 'Pillow'],
+    install_requires=['mkdocs', 'pillow'],
 	extras_require={
 		'dev': [
 			'mkdocs-material',
 			'mkdocs-open-in-new-tab',
 			'mkdocs-glightbox',
 			'mkdocs-git-revision-date-localized-plugin',
+            'cairosvg',
+            'pillow',
 		]
 	},
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

