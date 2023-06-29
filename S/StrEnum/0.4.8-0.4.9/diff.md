# Comparing `tmp/StrEnum-0.4.8.tar.gz` & `tmp/StrEnum-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StrEnum-0.4.8.tar", last modified: Wed Jun 22 06:03:41 2022, max compression
+gzip compressed data, was "StrEnum-0.4.9.tar", last modified: Tue Dec  6 12:41:55 2022, max compression
```

## Comparing `StrEnum-0.4.8.tar` & `StrEnum-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jsinclair   (501) staff       (20)        0 2022-06-22 06:03:41.389621 StrEnum-0.4.8/
--rw-r--r--   0 jsinclair   (501) staff       (20)     1073 2019-03-01 02:33:11.000000 StrEnum-0.4.8/LICENSE
--rw-r--r--   0 jsinclair   (501) staff       (20)       50 2020-05-20 06:23:14.000000 StrEnum-0.4.8/MANIFEST.in
--rw-r--r--   0 jsinclair   (501) staff       (20)     4777 2022-06-22 06:03:41.389893 StrEnum-0.4.8/PKG-INFO
--rw-r--r--   0 jsinclair   (501) staff       (20)     4043 2021-10-13 23:49:23.000000 StrEnum-0.4.8/README.md
-drwxr-xr-x   0 jsinclair   (501) staff       (20)        0 2022-06-22 06:03:41.384506 StrEnum-0.4.8/StrEnum.egg-info/
--rw-r--r--   0 jsinclair   (501) staff       (20)     4777 2022-06-22 06:03:40.000000 StrEnum-0.4.8/StrEnum.egg-info/PKG-INFO
--rw-r--r--   0 jsinclair   (501) staff       (20)      299 2022-06-22 06:03:41.000000 StrEnum-0.4.8/StrEnum.egg-info/SOURCES.txt
--rw-r--r--   0 jsinclair   (501) staff       (20)        1 2022-06-22 06:03:40.000000 StrEnum-0.4.8/StrEnum.egg-info/dependency_links.txt
--rw-r--r--   0 jsinclair   (501) staff       (20)      130 2022-06-22 06:03:41.000000 StrEnum-0.4.8/StrEnum.egg-info/requires.txt
--rw-r--r--   0 jsinclair   (501) staff       (20)        8 2022-06-22 06:03:41.000000 StrEnum-0.4.8/StrEnum.egg-info/top_level.txt
--rw-r--r--   0 jsinclair   (501) staff       (20)      173 2022-06-22 06:03:41.391790 StrEnum-0.4.8/setup.cfg
--rw-r--r--   0 jsinclair   (501) staff       (20)     1370 2022-06-22 05:48:52.000000 StrEnum-0.4.8/setup.py
-drwxr-xr-x   0 jsinclair   (501) staff       (20)        0 2022-06-22 06:03:41.393956 StrEnum-0.4.8/strenum/
--rw-r--r--   0 jsinclair   (501) staff       (20)     8530 2021-10-14 03:36:59.000000 StrEnum-0.4.8/strenum/__init__.py
--rw-r--r--   0 jsinclair   (501) staff       (20)     3397 2021-10-14 03:24:23.000000 StrEnum-0.4.8/strenum/_name_mangler.py
--rw-r--r--   0 jsinclair   (501) staff       (20)      497 2022-06-22 06:03:41.394517 StrEnum-0.4.8/strenum/_version.py
--rw-r--r--   0 jsinclair   (501) staff       (20)     2042 2021-10-14 00:50:41.000000 StrEnum-0.4.8/strenum/mixins.py
--rw-r--r--   0 jsinclair   (501) staff       (20)    68611 2020-05-20 06:23:14.000000 StrEnum-0.4.8/versioneer.py
+drwxr-xr-x   0 jsinclair   (501) staff       (20)        0 2022-12-06 12:41:55.563984 StrEnum-0.4.9/
+-rw-r--r--   0 jsinclair   (501) staff       (20)     1073 2019-03-01 02:33:11.000000 StrEnum-0.4.9/LICENSE
+-rw-r--r--   0 jsinclair   (501) staff       (20)       50 2020-05-20 06:23:14.000000 StrEnum-0.4.9/MANIFEST.in
+-rw-r--r--   0 jsinclair   (501) staff       (20)     4880 2022-12-06 12:41:55.564371 StrEnum-0.4.9/PKG-INFO
+-rw-r--r--   0 jsinclair   (501) staff       (20)     4043 2022-12-06 12:20:48.000000 StrEnum-0.4.9/README.md
+drwxr-xr-x   0 jsinclair   (501) staff       (20)        0 2022-12-06 12:41:55.561670 StrEnum-0.4.9/StrEnum.egg-info/
+-rw-r--r--   0 jsinclair   (501) staff       (20)     4880 2022-12-06 12:41:54.000000 StrEnum-0.4.9/StrEnum.egg-info/PKG-INFO
+-rw-r--r--   0 jsinclair   (501) staff       (20)      299 2022-12-06 12:41:55.000000 StrEnum-0.4.9/StrEnum.egg-info/SOURCES.txt
+-rw-r--r--   0 jsinclair   (501) staff       (20)        1 2022-12-06 12:41:54.000000 StrEnum-0.4.9/StrEnum.egg-info/dependency_links.txt
+-rw-r--r--   0 jsinclair   (501) staff       (20)      130 2022-12-06 12:41:55.000000 StrEnum-0.4.9/StrEnum.egg-info/requires.txt
+-rw-r--r--   0 jsinclair   (501) staff       (20)        8 2022-12-06 12:41:55.000000 StrEnum-0.4.9/StrEnum.egg-info/top_level.txt
+-rw-r--r--   0 jsinclair   (501) staff       (20)      173 2022-12-06 12:41:55.565095 StrEnum-0.4.9/setup.cfg
+-rw-r--r--   0 jsinclair   (501) staff       (20)     1471 2022-12-06 12:20:48.000000 StrEnum-0.4.9/setup.py
+drwxr-xr-x   0 jsinclair   (501) staff       (20)        0 2022-12-06 12:41:55.565498 StrEnum-0.4.9/strenum/
+-rw-r--r--   0 jsinclair   (501) staff       (20)     8530 2021-10-14 03:36:59.000000 StrEnum-0.4.9/strenum/__init__.py
+-rw-r--r--   0 jsinclair   (501) staff       (20)     3397 2021-10-14 03:24:23.000000 StrEnum-0.4.9/strenum/_name_mangler.py
+-rw-r--r--   0 jsinclair   (501) staff       (20)      497 2022-12-06 12:41:55.565613 StrEnum-0.4.9/strenum/_version.py
+-rw-r--r--   0 jsinclair   (501) staff       (20)     2042 2021-10-14 00:50:41.000000 StrEnum-0.4.9/strenum/mixins.py
+-rw-r--r--   0 jsinclair   (501) staff       (20)    68611 2020-05-20 06:23:14.000000 StrEnum-0.4.9/versioneer.py
```

### Comparing `StrEnum-0.4.8/LICENSE` & `StrEnum-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `StrEnum-0.4.8/PKG-INFO` & `StrEnum-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: StrEnum
-Version: 0.4.8
+Version: 0.4.9
 Summary: An Enum that inherits from str.
 Home-page: https://github.com/irgeek/StrEnum
 Author: James Sinclair
 Author-email: james@nurfherder.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 # StrEnum
 
 [![Build Status](https://github.com/irgeek/StrEnum/workflows/Python%20package/badge.svg)](https://github.com/irgeek/StrEnum/actions)
 
 StrEnum is a Python `enum.Enum` that inherits from `str` to complement
-`enum.IntEnum` in the standard library. Supports python 3.6+.
+`enum.IntEnum` in the standard library. Supports python 3.7+.
 
 ## Installation
 
 You can use [pip](https://pip.pypa.io/en/stable/) to install.
 
 ```bash
 pip install StrEnum
@@ -182,10 +184,10 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 **N.B. Starting with Python 3.11, `enum.StrEnum` is available in the standard
 library. This implementation is _not_ a drop-in replacement for the standard
-library implementation. Sepcifically, the Python devs have decided to case fold
+library implementation. Specifically, the Python devs have decided to case fold
 name to lowercase by default when `auto()` is used which I think violates the
 principle of least surprise.**
```

### Comparing `StrEnum-0.4.8/README.md` & `StrEnum-0.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # StrEnum
 
 [![Build Status](https://github.com/irgeek/StrEnum/workflows/Python%20package/badge.svg)](https://github.com/irgeek/StrEnum/actions)
 
 StrEnum is a Python `enum.Enum` that inherits from `str` to complement
-`enum.IntEnum` in the standard library. Supports python 3.6+.
+`enum.IntEnum` in the standard library. Supports python 3.7+.
 
 ## Installation
 
 You can use [pip](https://pip.pypa.io/en/stable/) to install.
 
 ```bash
 pip install StrEnum
@@ -161,10 +161,10 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 **N.B. Starting with Python 3.11, `enum.StrEnum` is available in the standard
 library. This implementation is _not_ a drop-in replacement for the standard
-library implementation. Sepcifically, the Python devs have decided to case fold
+library implementation. Specifically, the Python devs have decided to case fold
 name to lowercase by default when `auto()` is used which I think violates the
 principle of least surprise.**
```

### Comparing `StrEnum-0.4.8/StrEnum.egg-info/PKG-INFO` & `StrEnum-0.4.9/StrEnum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: StrEnum
-Version: 0.4.8
+Version: 0.4.9
 Summary: An Enum that inherits from str.
 Home-page: https://github.com/irgeek/StrEnum
 Author: James Sinclair
 Author-email: james@nurfherder.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 # StrEnum
 
 [![Build Status](https://github.com/irgeek/StrEnum/workflows/Python%20package/badge.svg)](https://github.com/irgeek/StrEnum/actions)
 
 StrEnum is a Python `enum.Enum` that inherits from `str` to complement
-`enum.IntEnum` in the standard library. Supports python 3.6+.
+`enum.IntEnum` in the standard library. Supports python 3.7+.
 
 ## Installation
 
 You can use [pip](https://pip.pypa.io/en/stable/) to install.
 
 ```bash
 pip install StrEnum
@@ -182,10 +184,10 @@
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 **N.B. Starting with Python 3.11, `enum.StrEnum` is available in the standard
 library. This implementation is _not_ a drop-in replacement for the standard
-library implementation. Sepcifically, the Python devs have decided to case fold
+library implementation. Specifically, the Python devs have decided to case fold
 name to lowercase by default when `auto()` is used which I think violates the
 principle of least surprise.**
```

### Comparing `StrEnum-0.4.8/setup.py` & `StrEnum-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         ],
         "release": ["twine"],
     },
     setup_requires=["pytest-runner"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `StrEnum-0.4.8/strenum/__init__.py` & `StrEnum-0.4.9/strenum/__init__.py`

 * *Files identical despite different names*

### Comparing `StrEnum-0.4.8/strenum/_name_mangler.py` & `StrEnum-0.4.9/strenum/_name_mangler.py`

 * *Files identical despite different names*

### Comparing `StrEnum-0.4.8/strenum/mixins.py` & `StrEnum-0.4.9/strenum/mixins.py`

 * *Files identical despite different names*

### Comparing `StrEnum-0.4.8/versioneer.py` & `StrEnum-0.4.9/versioneer.py`

 * *Files identical despite different names*

