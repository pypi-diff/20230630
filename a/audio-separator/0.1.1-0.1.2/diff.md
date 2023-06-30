# Comparing `tmp/audio_separator-0.1.1.tar.gz` & `tmp/audio-separator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.1.1.tar", last modified: Fri Jun 30 06:40:12 2023, max compression
+gzip compressed data, was "audio-separator-0.1.2.tar", last modified: Fri Jun 30 06:44:08 2023, max compression
```

## Comparing `audio_separator-0.1.1.tar` & `audio-separator-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:40:12.272699 audio_separator-0.1.1/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio_separator-0.1.1/LICENSE
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2875 2023-06-30 06:40:12.272297 audio_separator-0.1.1/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2461 2023-06-30 06:38:55.000000 audio_separator-0.1.1/README.md
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:40:12.241615 audio_separator-0.1.1/audio_separator/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio_separator-0.1.1/audio_separator/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10089 2023-06-30 06:26:46.000000 audio_separator-0.1.1/audio_separator/audio_separator.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:40:12.271587 audio_separator-0.1.1/audio_separator/utils/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio_separator-0.1.1/audio_separator/utils/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio_separator-0.1.1/audio_separator/utils/pyrb.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24824 2023-06-30 05:58:37.000000 audio_separator-0.1.1/audio_separator/utils/spec_utils.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:40:12.258888 audio_separator-0.1.1/audio_separator.egg-info/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2875 2023-06-30 06:40:11.000000 audio_separator-0.1.1/audio_separator.egg-info/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      425 2023-06-30 06:40:12.000000 audio_separator-0.1.1/audio_separator.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 06:40:11.000000 audio_separator-0.1.1/audio_separator.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       57 2023-06-30 06:40:11.000000 audio_separator-0.1.1/audio_separator.egg-info/entry_points.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 06:40:11.000000 audio_separator-0.1.1/audio_separator.egg-info/requires.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 06:40:11.000000 audio_separator-0.1.1/audio_separator.egg-info/top_level.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 06:40:12.272779 audio_separator-0.1.1/setup.cfg
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      982 2023-06-30 06:39:45.000000 audio_separator-0.1.1/setup.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.747485 audio-separator-0.1.2/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio-separator-0.1.2/LICENSE
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:44:08.746280 audio-separator-0.1.2/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2507 2023-06-30 06:43:31.000000 audio-separator-0.1.2/README.md
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.727528 audio-separator-0.1.2/audio_separator/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio-separator-0.1.2/audio_separator/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10089 2023-06-30 06:26:46.000000 audio-separator-0.1.2/audio_separator/audio_separator.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.744830 audio-separator-0.1.2/audio_separator/utils/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio-separator-0.1.2/audio_separator/utils/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio-separator-0.1.2/audio_separator/utils/pyrb.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24824 2023-06-30 05:58:37.000000 audio-separator-0.1.2/audio_separator/utils/spec_utils.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.742067 audio-separator-0.1.2/audio_separator.egg-info/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      425 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       58 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/entry_points.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/requires.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/top_level.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 06:44:08.747637 audio-separator-0.1.2/setup.cfg
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      983 2023-06-30 06:43:36.000000 audio-separator-0.1.2/setup.py
```

### Comparing `audio_separator-0.1.1/LICENSE` & `audio-separator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.1.1/PKG-INFO` & `audio-separator-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: audio_separator
-Version: 0.1.1
+Name: audio-separator
+Version: 0.1.2
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -35,24 +35,27 @@
 ## Usage
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
-audio_separator [audio_file] --model_name [model_name]
-audio_file: The path to the WAV audio file to be separated.
-model_name: (Optional) The name of the model to use for separation.
+audio-separator [audio_file] --model_name [model_name]
+    
+    audio_file: The path to the WAV audio file to be separated.
+    model_name: (Optional) The name of the model to use for separation.
 ```
 
 Example:
 
-audio_separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
+```
+audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
+```
 
-This command will process the file and generate two new files, one for each stem.
+This command will process the file and generate two new files in the current directory, one for each stem.
 
 ### As a Dependency in a Python Project
 
 You can also use Audio Separator in your Python project. Here's how you can use it:
 
 ```
 from audio_separator import Separator
```

### Comparing `audio_separator-0.1.1/README.md` & `audio-separator-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 ## Usage
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
-audio_separator [audio_file] --model_name [model_name]
-audio_file: The path to the WAV audio file to be separated.
-model_name: (Optional) The name of the model to use for separation.
+audio-separator [audio_file] --model_name [model_name]
+    
+    audio_file: The path to the WAV audio file to be separated.
+    model_name: (Optional) The name of the model to use for separation.
 ```
 
 Example:
 
-audio_separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
+```
+audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
+```
 
-This command will process the file and generate two new files, one for each stem.
+This command will process the file and generate two new files in the current directory, one for each stem.
 
 ### As a Dependency in a Python Project
 
 You can also use Audio Separator in your Python project. Here's how you can use it:
 
 ```
 from audio_separator import Separator
```

### Comparing `audio_separator-0.1.1/audio_separator/audio_separator.py` & `audio-separator-0.1.2/audio_separator/audio_separator.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.1.1/audio_separator/utils/pyrb.py` & `audio-separator-0.1.2/audio_separator/utils/pyrb.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.1.1/audio_separator/utils/spec_utils.py` & `audio-separator-0.1.2/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.1.1/audio_separator.egg-info/PKG-INFO` & `audio-separator-0.1.2/audio_separator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -35,24 +35,27 @@
 ## Usage
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
 ```sh
-audio_separator [audio_file] --model_name [model_name]
-audio_file: The path to the WAV audio file to be separated.
-model_name: (Optional) The name of the model to use for separation.
+audio-separator [audio_file] --model_name [model_name]
+    
+    audio_file: The path to the WAV audio file to be separated.
+    model_name: (Optional) The name of the model to use for separation.
 ```
 
 Example:
 
-audio_separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
+```
+audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
+```
 
-This command will process the file and generate two new files, one for each stem.
+This command will process the file and generate two new files in the current directory, one for each stem.
 
 ### As a Dependency in a Python Project
 
 You can also use Audio Separator in your Python project. Here's how you can use it:
 
 ```
 from audio_separator import Separator
```

### Comparing `audio_separator-0.1.1/setup.py` & `audio-separator-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="audio_separator",
-    version="0.1.1",
+    name="audio-separator",
+    version="0.1.2",
     packages=find_packages(),
 
     # Metadata
     author="Andrew Beveridge",
     author_email="andrew@beveridge.uk",
     description="Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/karaokenerds/python-audio-separator",
     license='MIT',
 
     # Specify entry script
     entry_points={
         'console_scripts': [
-            'separate-audio=scripts.separate:main',
+            'audio-separator=scripts.separate:main',
         ],
     },
 
     # Specify python version and dependencies
     python_requires='>=3.9',
     install_requires=[
         'onnx',
```

