# Comparing `tmp/audio-separator-0.1.2.tar.gz` & `tmp/audio-separator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio-separator-0.1.2.tar", last modified: Fri Jun 30 06:44:08 2023, max compression
+gzip compressed data, was "audio-separator-0.1.3.tar", last modified: Fri Jun 30 06:57:11 2023, max compression
```

## Comparing `audio-separator-0.1.2.tar` & `audio-separator-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.747485 audio-separator-0.1.2/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio-separator-0.1.2/LICENSE
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:44:08.746280 audio-separator-0.1.2/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2507 2023-06-30 06:43:31.000000 audio-separator-0.1.2/README.md
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.727528 audio-separator-0.1.2/audio_separator/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio-separator-0.1.2/audio_separator/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10089 2023-06-30 06:26:46.000000 audio-separator-0.1.2/audio_separator/audio_separator.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.744830 audio-separator-0.1.2/audio_separator/utils/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio-separator-0.1.2/audio_separator/utils/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio-separator-0.1.2/audio_separator/utils/pyrb.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24824 2023-06-30 05:58:37.000000 audio-separator-0.1.2/audio_separator/utils/spec_utils.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:44:08.742067 audio-separator-0.1.2/audio_separator.egg-info/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      425 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       58 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/entry_points.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/requires.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 06:44:08.000000 audio-separator-0.1.2/audio_separator.egg-info/top_level.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 06:44:08.747637 audio-separator-0.1.2/setup.cfg
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      983 2023-06-30 06:43:36.000000 audio-separator-0.1.2/setup.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.062073 audio-separator-0.1.3/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-06-30 05:57:58.000000 audio-separator-0.1.3/LICENSE
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:57:11.061755 audio-separator-0.1.3/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2507 2023-06-30 06:43:31.000000 audio-separator-0.1.3/README.md
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.050662 audio-separator-0.1.3/audio_separator/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:26:40.000000 audio-separator-0.1.3/audio_separator/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)    10105 2023-06-30 06:50:36.000000 audio-separator-0.1.3/audio_separator/audio_separator.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.060975 audio-separator-0.1.3/audio_separator/utils/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 05:58:37.000000 audio-separator-0.1.3/audio_separator/utils/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2135 2023-06-30 05:58:37.000000 audio-separator-0.1.3/audio_separator/utils/pyrb.py
+-rwxr-xr-x   0 andrew.beveridge   (503) staff       (20)      952 2023-06-30 06:55:53.000000 audio-separator-0.1.3/audio_separator/utils/separate.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)    24840 2023-06-30 06:51:10.000000 audio-separator-0.1.3/audio_separator/utils/spec_utils.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-30 06:57:11.056094 audio-separator-0.1.3/audio_separator.egg-info/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     2921 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      459 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       72 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/entry_points.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      100 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/requires.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       16 2023-06-30 06:57:10.000000 audio-separator-0.1.3/audio_separator.egg-info/top_level.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-30 06:57:11.062134 audio-separator-0.1.3/setup.cfg
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      997 2023-06-30 06:52:06.000000 audio-separator-0.1.3/setup.py
```

### Comparing `audio-separator-0.1.2/LICENSE` & `audio-separator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.2/PKG-INFO` & `audio-separator-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `audio-separator-0.1.2/README.md` & `audio-separator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.2/audio_separator/audio_separator.py` & `audio-separator-0.1.3/audio_separator/audio_separator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import warnings
 import wget
 import torch
 import librosa
 import numpy as np
 import onnxruntime as ort
 import soundfile as sf
-from utils import spec_utils
+from audio_separator.utils import spec_utils
 
 def print_with_timestamp(message):
     timestamp = datetime.datetime.now().isoformat()
     print(f"{timestamp} - {message}")
 
 class Separator:
     def __init__(self, audio_file, model_name='UVR_MDXNET_KARA_2', output_dir=None):
```

### Comparing `audio-separator-0.1.2/audio_separator/utils/pyrb.py` & `audio-separator-0.1.3/audio_separator/utils/pyrb.py`

 * *Files identical despite different names*

### Comparing `audio-separator-0.1.2/audio_separator/utils/spec_utils.py` & `audio-separator-0.1.3/audio_separator/utils/spec_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 SYSTEM_ARCH = platform.platform()
 SYSTEM_PROC = platform.processor()
 ARM = 'arm'
 
 if OPERATING_SYSTEM == 'Windows':
     from pyrubberband import pyrb
 else:
-    from utils import pyrb
+    from audio_separator.utils import pyrb
 
 if OPERATING_SYSTEM == 'Darwin':
     wav_resolution = "polyphase" if SYSTEM_PROC == ARM or ARM in SYSTEM_ARCH else "sinc_fastest" 
 else:
     wav_resolution = "sinc_fastest"
 
 MAX_SPEC = 'Max Spec'
```

### Comparing `audio-separator-0.1.2/audio_separator.egg-info/PKG-INFO` & `audio-separator-0.1.3/audio_separator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `audio-separator-0.1.2/setup.py` & `audio-separator-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="audio-separator",
-    version="0.1.2",
+    version="0.1.3",
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
-            'audio-separator=scripts.separate:main',
+            'audio-separator=audio_separator.utils.separate:main',
         ],
     },
 
     # Specify python version and dependencies
     python_requires='>=3.9',
     install_requires=[
         'onnx',
```

