# Comparing `tmp/pwasopt-0.0.1.tar.gz` & `tmp/pwasopt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.1.tar", last modified: Fri Jun 30 11:58:11 2023, max compression
+gzip compressed data, was "pwasopt-0.0.2.tar", last modified: Fri Jun 30 12:38:01 2023, max compression
```

## Comparing `pwasopt-0.0.1.tar` & `pwasopt-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:58:11.597468 pwasopt-0.0.1/
--rw-rw-rw-   0        0        0    11524 2023-02-06 14:50:31.000000 pwasopt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2669 2023-06-30 11:58:11.597468 pwasopt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-02-11 20:07:08.000000 pwasopt-0.0.1/README.md
--rw-rw-rw-   0        0        0      923 2023-06-30 11:56:38.000000 pwasopt-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 11:58:11.597468 pwasopt-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 11:58:11.550588 pwasopt-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 11:58:11.581824 pwasopt-0.0.1/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.1/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.1/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.1/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.1/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.1/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21944 2023-06-30 11:56:38.000000 pwasopt-0.0.1/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22256 2023-06-30 11:56:38.000000 pwasopt-0.0.1/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0    44725 2022-05-24 21:25:29.000000 pwasopt-0.0.1/src/pwasopt/parc.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.1/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.1/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12425 2023-06-30 11:57:28.000000 pwasopt-0.0.1/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30956 2023-06-30 11:57:36.000000 pwasopt-0.0.1/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:58:11.581824 pwasopt-0.0.1/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0     2669 2023-06-30 11:58:11.000000 pwasopt-0.0.1/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-06-30 11:58:11.000000 pwasopt-0.0.1/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:58:11.000000 pwasopt-0.0.1/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-30 11:58:11.000000 pwasopt-0.0.1/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 11:58:11.000000 pwasopt-0.0.1/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.575028 pwasopt-0.0.2/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2669 2023-06-30 12:38:01.575028 pwasopt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-02-11 20:07:08.000000 pwasopt-0.0.2/README.md
+-rw-rw-rw-   0        0        0      923 2023-06-30 12:36:56.000000 pwasopt-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 12:38:01.575028 pwasopt-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.521623 pwasopt-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.559400 pwasopt-0.0.2/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.2/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.2/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.2/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14260 2023-02-08 22:16:44.000000 pwasopt-0.0.2/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.2/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21920 2023-06-30 12:35:26.000000 pwasopt-0.0.2/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22232 2023-06-30 12:35:53.000000 pwasopt-0.0.2/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0    44725 2022-05-24 21:25:29.000000 pwasopt-0.0.2/src/pwasopt/parc.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.2/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.2/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.2/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.2/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:38:01.559400 pwasopt-0.0.2/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0     2669 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 12:38:01.000000 pwasopt-0.0.2/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.1/LICENSE` & `pwasopt-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,20 +182,20 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Mengjia Zhu, Alberto Bemporad
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pwasopt-0.0.1/PKG-INFO` & `pwasopt-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.1
+Version: 0.0.2
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pwasopt-0.0.1/README.md` & `pwasopt-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/pyproject.toml` & `pwasopt-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pwasopt-0.0.1/src/pwasopt/acquisition.py` & `pwasopt-0.0.2/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.2/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.2/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.2/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/main_pwas.py` & `pwasopt-0.0.2/src/pwasopt/main_pwas.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 reference code:
                 - parc.py by A. Bemporad, 2021, http://cse.lab.imtlucca.it/~bemporad/parc/
                 - GLIS package by A.Bemporad & M. Zhu, 2023, https://github.com/bemporad/GLIS
 
 (C) 2021-2023 Mengjia Zhu, Alberto Bemporad
 """
 
-from src.pwasopt.parc import PARC
-from src.pwasopt.prob_setup import *
-from src.pwasopt.sample import *
-from src.pwasopt.acquisition import *
-from src.pwasopt.categorical_encoder import *
-from src.pwasopt.integ_encoder import *
+from pwasopt.parc import PARC
+from pwasopt.prob_setup import *
+from pwasopt.sample import *
+from pwasopt.acquisition import *
+from pwasopt.categorical_encoder import *
+from pwasopt.integ_encoder import *
 
 import time
 
 
 class PWAS:
     """
     Main class for PWAS
```

### Comparing `pwasopt-0.0.1/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.2/src/pwasopt/main_pwasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 reference code:
                 - parc.py by A. Bemporad, 2021, http://cse.lab.imtlucca.it/~bemporad/parc/
                 - GLIS package by A.Bemporad & M. Zhu, 2023, https://github.com/bemporad/GLIS
 
 (C) 2021-2023 Mengjia Zhu, Alberto Bemporad
 """
 
-from src.pwasopt.prob_setup import *
-from src.pwasopt.sample import *
-from src.pwasopt.acquisition import *
-from src.pwasopt.categorical_encoder import *
-from src.pwasopt.integ_encoder import *
-from src.pwasopt.fit_surrogate_pwasp import *
+from pwasopt.prob_setup import *
+from pwasopt.sample import *
+from pwasopt.acquisition import *
+from pwasopt.categorical_encoder import *
+from pwasopt.integ_encoder import *
+from pwasopt.fit_surrogate_pwasp import *
 
 import time
 
 class PWASp:
     """
     Main class for PWASp
     Note:
```

### Comparing `pwasopt-0.0.1/src/pwasopt/parc.py` & `pwasopt-0.0.2/src/pwasopt/parc.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/pref_fun.py` & `pwasopt-0.0.2/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.2/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.1/src/pwasopt/prob_setup.py` & `pwasopt-0.0.2/src/pwasopt/prob_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 (C) 2021-2023 Mengjia Zhu, Alberto Bemporad
 """
 
 import numpy as np
 from scipy.optimize import linprog as linprog
 import sys
 
-from src.pwasopt.pref_fun1 import PWASp_fun1
-from src.pwasopt.pref_fun import PWASp_fun
+from pwasopt.pref_fun1 import PWASp_fun1
+from pwasopt.pref_fun import PWASp_fun
 
 
 class problem_defn:
     """
     Initial set up of the problem (problem description/definition)
 
     """
```

### Comparing `pwasopt-0.0.1/src/pwasopt/sample.py` & `pwasopt-0.0.2/src/pwasopt/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 import math as mt
 from pyDOE import lhs #https://pythonhosted.org/pyDOE/
 import pulp as plp
 import cdd  #https://pypi.org/project/pycddlib/
 import random
 
-from src.pwasopt.categorical_encoder import *
-from src.pwasopt.integ_encoder import *
+from pwasopt.categorical_encoder import *
+from pwasopt.integ_encoder import *
 
 class init_sampl:
 
     def __init__(self, prob):
         """
         Obtain and constructs all necessary attributes for self
         """
```

### Comparing `pwasopt-0.0.1/src/pwasopt.egg-info/PKG-INFO` & `pwasopt-0.0.2/src/pwasopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.1
+Version: 0.0.2
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pwasopt-0.0.1/src/pwasopt.egg-info/SOURCES.txt` & `pwasopt-0.0.2/src/pwasopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

