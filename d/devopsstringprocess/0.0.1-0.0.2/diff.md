# Comparing `tmp/devopsstringprocess-0.0.1.tar.gz` & `tmp/devopsstringprocess-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsstringprocess-0.0.1.tar", last modified: Fri Jun 30 01:23:17 2023, max compression
+gzip compressed data, was "devopsstringprocess-0.0.2.tar", last modified: Fri Jun 30 01:55:49 2023, max compression
```

## Comparing `devopsstringprocess-0.0.1.tar` & `devopsstringprocess-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:17.095584 devopsstringprocess-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-22 22:39:20.000000 devopsstringprocess-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      636 2023-06-30 01:23:17.092615 devopsstringprocess-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-06-22 22:39:20.000000 devopsstringprocess-0.0.1/README.md
--rw-rw-rw-   0        0        0      751 2023-06-30 01:22:32.000000 devopsstringprocess-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-30 01:16:34.000000 devopsstringprocess-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 01:23:17.097097 devopsstringprocess-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:17.023002 devopsstringprocess-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:17.080066 devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/
--rw-rw-rw-   0        0        0      636 2023-06-30 01:23:16.000000 devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-06-30 01:23:17.000000 devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:23:16.000000 devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-30 01:23:16.000000 devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-30 01:23:16.000000 devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:17.087575 devopsstringprocess-0.0.1/src/stringstandardization/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:13:38.000000 devopsstringprocess-0.0.1/src/stringstandardization/__init__.py
--rw-rw-rw-   0        0        0       89 2023-06-22 23:37:10.000000 devopsstringprocess-0.0.1/src/stringstandardization/stringstd.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:23:17.089584 devopsstringprocess-0.0.1/test/
--rw-rw-rw-   0        0        0      185 2023-06-22 23:37:22.000000 devopsstringprocess-0.0.1/test/test_stringstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:55:49.640611 devopsstringprocess-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-30 01:55:49.640611 devopsstringprocess-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 01:55:49.640611 devopsstringprocess-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:55:49.636611 devopsstringprocess-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:55:49.640611 devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-30 01:55:49.000000 devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-30 01:55:49.000000 devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:55:49.000000 devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-30 01:55:49.000000 devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 01:55:49.000000 devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:55:49.640611 devopsstringprocess-0.0.2/src/stringstandardization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/src/stringstandardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/src/stringstandardization/stringstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:55:49.640611 devopsstringprocess-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-30 01:55:39.000000 devopsstringprocess-0.0.2/test/test_stringstd.py
```

### Comparing `devopsstringprocess-0.0.1/LICENSE` & `devopsstringprocess-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ramon Durães
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ramon Durães
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `devopsstringprocess-0.0.1/PKG-INFO` & `devopsstringprocess-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: devopsstringprocess
-Version: 0.0.1
-Summary: String standardization package for devops course
-Author-email: Ramon Durães <ramongduraes@gmail.com>
-Project-URL: Homepage, https://github.com/ramongduraes/devops-string
-Project-URL: Bug Tracker, https://github.com/ramongduraes/devops-string/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# devops-string
-Simple project tutorial for standardizing strings
+Metadata-Version: 2.1
+Name: devopsstringprocess
+Version: 0.0.2
+Summary: String standardization package for devops course
+Author-email: Ramon Durães <ramongduraes@gmail.com>
+Project-URL: Homepage, https://github.com/ramongduraes/devops-string
+Project-URL: Bug Tracker, https://github.com/ramongduraes/devops-string/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# devops-string
+Simple project tutorial for standardizing strings
```

### Comparing `devopsstringprocess-0.0.1/src/devopsstringprocess.egg-info/PKG-INFO` & `devopsstringprocess-0.0.2/src/devopsstringprocess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: devopsstringprocess
-Version: 0.0.1
-Summary: String standardization package for devops course
-Author-email: Ramon Durães <ramongduraes@gmail.com>
-Project-URL: Homepage, https://github.com/ramongduraes/devops-string
-Project-URL: Bug Tracker, https://github.com/ramongduraes/devops-string/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# devops-string
-Simple project tutorial for standardizing strings
+Metadata-Version: 2.1
+Name: devopsstringprocess
+Version: 0.0.2
+Summary: String standardization package for devops course
+Author-email: Ramon Durães <ramongduraes@gmail.com>
+Project-URL: Homepage, https://github.com/ramongduraes/devops-string
+Project-URL: Bug Tracker, https://github.com/ramongduraes/devops-string/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# devops-string
+Simple project tutorial for standardizing strings
```

