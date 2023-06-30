# Comparing `tmp/ffmpeg_python_utils-0.0.3.tar.gz` & `tmp/ffmpeg_python_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_python_utils-0.0.3.tar", last modified: Thu Jun 29 13:29:24 2023, max compression
+gzip compressed data, was "ffmpeg_python_utils-0.0.4.tar", last modified: Thu Jun 29 15:26:00 2023, max compression
```

## Comparing `ffmpeg_python_utils-0.0.3.tar` & `ffmpeg_python_utils-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:29:24.005845 ffmpeg_python_utils-0.0.3/
--rw-rw-rw-   0        0        0     1097 2023-06-28 17:21:41.000000 ffmpeg_python_utils-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      808 2023-06-29 13:29:24.005845 ffmpeg_python_utils-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1634 2023-06-28 22:10:37.000000 ffmpeg_python_utils-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 13:29:23.997845 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/
--rw-rw-rw-   0        0        0     1043 2023-06-28 19:38:55.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-06-29 13:01:42.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/config.py
--rw-rw-rw-   0        0        0     4983 2023-06-29 09:14:35.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/inc.py
--rw-rw-rw-   0        0        0    37683 2023-06-29 12:27:38.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/main.py
--rw-rw-rw-   0        0        0     8059 2023-06-28 21:33:03.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/other.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:29:24.004843 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/
--rw-rw-rw-   0        0        0      808 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-29 13:29:23.000000 ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:29:24.006846 ffmpeg_python_utils-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-29 13:28:36.000000 ffmpeg_python_utils-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:26:00.829249 ffmpeg_python_utils-0.0.4/
+-rw-rw-rw-   0        0        0     1097 2023-06-28 17:21:41.000000 ffmpeg_python_utils-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      808 2023-06-29 15:26:00.829249 ffmpeg_python_utils-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2023-06-28 22:10:37.000000 ffmpeg_python_utils-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:26:00.794249 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/
+-rw-rw-rw-   0        0        0     1043 2023-06-28 19:38:55.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/__init__.py
+-rw-rw-rw-   0        0        0     1304 2023-06-29 14:20:15.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/config.py
+-rw-rw-rw-   0        0        0     4983 2023-06-29 09:14:35.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/inc.py
+-rw-rw-rw-   0        0        0    37683 2023-06-29 12:27:38.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/main.py
+-rw-rw-rw-   0        0        0     8131 2023-06-29 14:20:15.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/other.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:26:00.827250 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-06-29 15:26:00.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-29 15:26:00.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:26:00.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-29 15:26:00.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-29 15:26:00.000000 ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 15:26:00.831249 ffmpeg_python_utils-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-29 15:25:49.000000 ffmpeg_python_utils-0.0.4/setup.py
```

### Comparing `ffmpeg_python_utils-0.0.3/LICENSE` & `ffmpeg_python_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.3/PKG-INFO` & `ffmpeg_python_utils-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ffmpeg_python_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python scripts constructing ffmpeg commands and running them by subprocess.
 Home-page: https://github.com/LionelCrowl/ffmpeg-python-utils
-Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.3.zip
+Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.4.zip
 Author: LionelCrowl
 Author-email: mr.lihenko@yandex.ru
 License: MIT License, see LICENSE file
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ffmpeg_python_utils-0.0.3/README.md` & `ffmpeg_python_utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/__init__.py` & `ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/config.py` & `ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 C_CODEC_SETTINGS = {
     'nvidia': '-c:v h264_nvenc -profile:v high -tune hq -rc-lookahead 8 -bf 2 -rc vbr -cq 10 -b:v 0 -maxrate 120M -bufsize 240M',
     'amd': '-c:v h264_amf',
     'cpu': '-c:v libx264 -crf 15',
 }
 """
 Specific settings for the codec. Nvidia is described here: 
-"https://video.stackexchange.com/questions/29659/is-there-a-way-to-improve-h264-nvenc-output-quality"
-"https://superuser.com/questions/1236275/how-can-i-use-crf-encoding-with-nvenc-in-ffmpeg"
+
+"https://video.stackexchange.com/questions/29659/is-there-a-way-to-improve-h264-nvenc-output-quality",
+"https://superuser.com/questions/1236275/how-can-i-use-crf-encoding-with-nvenc-in-ffmpeg".
+
 The default crf for cpu is 23. The higher the crf or cq, the worse the quality, but the smaller the file size.
 """
 
 C_TO_PRINT_PACKAGE_INFO = True
 """Whether to show package info."""
 C_TO_PRINT_EXECUTION_TIME = True
 """Whether to show each function's execution time."""
@@ -26,9 +28,7 @@
 """Whether to print only ffmpeg errors. C_TO_PRINT_ONLY_FFMPEG_ERRORS > C_TO_PRINT_FFMPEG_DEBUG. The code first 
 checks if to print only errors."""
 C_TO_PRINT_FFMPEG_DEBUG = False
 """Whether to show detailed information from ffmpeg."""
 
 C_TO_RENAME_FILES = False
 """Whether to rename files. It should work with False."""
-C_TO_PRINT_PLOTS = True
-"""Whether to show plots during finding offsets before proceeding."""
```

### Comparing `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/inc.py` & `ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/inc.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/main.py` & `ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/main.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils/other.py` & `ffmpeg_python_utils-0.0.4/ffmpeg_python_utils/other.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import pickle
 from pydub import AudioSegment
 import hashlib
 from functools import wraps
 import inspect
 from .inc import print_info
-from .config import C_TO_PRINT_PACKAGE_INFO, C_TO_PRINT_PLOTS
+from .config import C_TO_PRINT_PACKAGE_INFO
 
 
 def cache_results(function_to_modify):
     # Caches results from find_offsets just in case. Takes in account hash + kwargs.
     # Saves cache to "cached_offset_searches.pickle" file.
 
     @wraps(function_to_modify)
@@ -120,25 +120,26 @@
         if input_list[i] - output_list[-1] >= 1.0:
             output_list.append(input_list[i])
     return output_list
 
 
 @cache_results
 def find_offsets(within_file: str, find_file: str, multiplier: float, window: int = 2, number: int = None,
-                 max_tries_number: int = 400) -> list:
+                 max_tries_number: int = 400, to_print_plots=False) -> list:
     """
     Finds time codes of appearance audio of find_file in within_file using scipy.
 
     Args:
         within_file (str): path to the audio file to search within
         find_file (str): path to the audio file to search for
         multiplier (float): a multiplier used to calculate the prominence of peaks in the correlation signal. The bigger you set it, the less time codes function returns.
         window (int): the length of find_file audio to use for the correlation (in seconds)
         number (int): the goal number of offsets to return
         max_tries_number (int): maximum number of tries to find the number
+        to_print_plots (bool): whether to print plot before proceeding
 
     Returns:
         list: list of time codes
     """
 
     y_within, sr_within = librosa.load(within_file, sr=None)
     y_find, _ = librosa.load(find_file, sr=sr_within)
@@ -146,27 +147,27 @@
     if number is not None and number < 1:
         print_info(f'Number of peaks you are looking for is {number}. Returning empty list.', 'red',
                    C_TO_PRINT_PACKAGE_INFO)
         return []
 
     elif number == 1:
         c = np.argmax(c)
-        if C_TO_PRINT_PLOTS:
+        if to_print_plots:
             plot_offsets(c, find_file)
         peak = round(c / sr_within, 2)
         return [peak]
     else:
         prominence = int(c[np.argmax(c)] * multiplier)
         counter = 0
         while True:
             try:
                 peaks, _ = signal.find_peaks(c, prominence=prominence)
                 points_of_time = [round(peak / sr_within, 2) for peak in peaks]
                 points_of_time = delete_neighbors(points_of_time)
-                if C_TO_PRINT_PLOTS:
+                if to_print_plots:
                     plot_offsets(c, find_file)
                 if counter < max_tries_number:
                     if C_TO_PRINT_PACKAGE_INFO: print(
                         f'Max try number reached. Returning the last time codes. {points_of_time}')
                     return points_of_time
                 if number and number != len(points_of_time):
                     print(
```

### Comparing `ffmpeg_python_utils-0.0.3/ffmpeg_python_utils.egg-info/PKG-INFO` & `ffmpeg_python_utils-0.0.4/ffmpeg_python_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ffmpeg-python-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python scripts constructing ffmpeg commands and running them by subprocess.
 Home-page: https://github.com/LionelCrowl/ffmpeg-python-utils
-Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.3.zip
+Download-URL: https://github.com/LionelCrowl/ffmpeg-python-utils/archive/v0.0.4.zip
 Author: LionelCrowl
 Author-email: mr.lihenko@yandex.ru
 License: MIT License, see LICENSE file
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ffmpeg_python_utils-0.0.3/setup.py` & `ffmpeg_python_utils-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '0.0.3'
+version = '0.0.4'
 
 description = 'Python scripts constructing ffmpeg commands and running them by subprocess.'
 
 long_description = ''' Python scripts constructing ffmpeg commands and running them by subprocess.
                     Check documentation: https://lionelcrowl.github.io/ffmpeg-python-utils/
                     '''
```

