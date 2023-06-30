# Comparing `tmp/audio_separator-0.2.0.tar.gz` & `tmp/audio_separator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.2.0.tar", max compression
+gzip compressed data, was "audio_separator-0.2.1.tar", max compression
```

## Comparing `audio_separator-0.2.0.tar` & `audio_separator-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.2.0/LICENSE
--rw-r--r--   0        0        0     5621 2023-06-30 18:35:00.806625 audio_separator-0.2.0/README.md
--rw-r--r--   0        0        0       39 2023-06-30 18:24:22.760767 audio_separator-0.2.0/audio_separator/__init__.py
--rw-r--r--   0        0        0    10882 2023-06-30 18:25:09.140022 audio_separator-0.2.0/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.2.0/audio_separator/utils/__init__.py
--rw-r--r--   0        0        0     2135 2023-06-30 05:58:37.421373 audio_separator-0.2.0/audio_separator/utils/pyrb.py
--rwxr-xr-x   0        0        0     1096 2023-06-30 18:25:49.961751 audio_separator-0.2.0/audio_separator/utils/separate.py
--rw-r--r--   0        0        0    24840 2023-06-30 06:51:10.010639 audio_separator-0.2.0/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      677 2023-06-30 18:30:32.298791 audio_separator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6442 1970-01-01 00:00:00.000000 audio_separator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6022 2023-06-30 18:37:13.543869 audio_separator-0.2.1/README.md
+-rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.2.1/audio_separator/__init__.py
+-rw-r--r--   0        0        0    10882 2023-06-30 18:25:09.140022 audio_separator-0.2.1/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.2.1/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     1096 2023-06-30 18:25:49.961751 audio_separator-0.2.1/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0     2135 2023-06-30 05:58:37.421373 audio_separator-0.2.1/audio_separator/utils/pyrb.py
+-rw-r--r--   0        0        0    24840 2023-06-30 06:51:10.010639 audio_separator-0.2.1/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      672 2023-06-30 18:39:39.309095 audio_separator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6843 1970-01-01 00:00:00.000000 audio_separator-0.2.1/PKG-INFO
```

### Comparing `audio_separator-0.2.0/LICENSE` & `audio_separator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.0/README.md` & `audio_separator-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -113,14 +113,32 @@
 
 You can run the CLI command directly within the virtual environment. For example:
 
 ```
 audio-separator path/to/your/audio-file.wav
 ```
 
+### Deactivate the Virtual Environment
+
+Once you are done with your development work, you can exit the virtual environment by simply typing:
+
+```
+exit
+```
+
+### Building the Package
+
+To build the package for distribution, use the following command:
+
+```
+poetry build
+```
+
+This will generate the distribution packages in the dist directory - but for now only @beveradb will be able to publish to PyPI.
+
 ## Contributing
 
 Contributions are very much welcome! Please fork the repository and submit a pull request with your changes, and I'll try to review, merge and publish promptly!
 
 - This project is 100% open-source and free for anyone to use and modify as they wish. 
 - If the maintenance workload for this repo somehow becomes too much for me I'll ask for volunteers to share maintainership of the repo, though I don't think that is very likely
 - Development and support for the MDX-Net separation models is part of the main [UVR project](https://github.com/Anjok07/ultimatevocalremovergui), this repo is just a CLI/Python package wrapper to simplify running those models programmatically. So, if you want to try and improve the actual models, please get involved in the UVR project and look for guidance there!
```

### Comparing `audio_separator-0.2.0/audio_separator/separator.py` & `audio_separator-0.2.1/audio_separator/separator.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.0/audio_separator/utils/pyrb.py` & `audio_separator-0.2.1/audio_separator/utils/pyrb.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.0/audio_separator/utils/separate.py` & `audio_separator-0.2.1/audio_separator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.0/audio_separator/utils/spec_utils.py` & `audio_separator-0.2.1/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.2.0/pyproject.toml` & `audio_separator-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.2.0"
+version = "0.2.1"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 
 [tool.poetry.dependencies]
@@ -15,12 +15,12 @@
 soundfile = "^0.11"
 librosa = "^0.9"
 torch = "^1.13"
 wget = "^3"
 six = "^1.16"
 
 [tool.poetry.scripts]
-audio-separator = 'audio_separator.utils.separate:main'
+audio-separator = 'audio_separator.utils.cli:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `audio_separator-0.2.0/PKG-INFO` & `audio_separator-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -135,14 +135,32 @@
 
 You can run the CLI command directly within the virtual environment. For example:
 
 ```
 audio-separator path/to/your/audio-file.wav
 ```
 
+### Deactivate the Virtual Environment
+
+Once you are done with your development work, you can exit the virtual environment by simply typing:
+
+```
+exit
+```
+
+### Building the Package
+
+To build the package for distribution, use the following command:
+
+```
+poetry build
+```
+
+This will generate the distribution packages in the dist directory - but for now only @beveradb will be able to publish to PyPI.
+
 ## Contributing
 
 Contributions are very much welcome! Please fork the repository and submit a pull request with your changes, and I'll try to review, merge and publish promptly!
 
 - This project is 100% open-source and free for anyone to use and modify as they wish. 
 - If the maintenance workload for this repo somehow becomes too much for me I'll ask for volunteers to share maintainership of the repo, though I don't think that is very likely
 - Development and support for the MDX-Net separation models is part of the main [UVR project](https://github.com/Anjok07/ultimatevocalremovergui), this repo is just a CLI/Python package wrapper to simplify running those models programmatically. So, if you want to try and improve the actual models, please get involved in the UVR project and look for guidance there!
```

