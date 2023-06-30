# Comparing `tmp/mathkit-0.1.0.tar.gz` & `tmp/mathkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-0.1.0.tar", last modified: Fri Jun 30 06:50:44 2023, max compression
+gzip compressed data, was "mathkit-0.1.1.tar", last modified: Fri Jun 30 06:54:31 2023, max compression
```

## Comparing `mathkit-0.1.0.tar` & `mathkit-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 06:50:44.104979 mathkit-0.1.0/
--rw-rw-rw-   0        0        0     2325 2023-06-30 06:50:44.098979 mathkit-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 06:50:44.069431 mathkit-0.1.0/mathkit/
--rw-rw-rw-   0        0        0      966 2023-06-30 06:18:35.000000 mathkit-0.1.0/mathkit/__init__.py
--rw-rw-rw-   0        0        0      160 2023-06-30 04:01:47.000000 mathkit-0.1.0/mathkit/addition.py
--rw-rw-rw-   0        0        0      117 2023-06-30 06:13:56.000000 mathkit-0.1.0/mathkit/cube.py
--rw-rw-rw-   0        0        0      128 2023-06-30 05:06:59.000000 mathkit-0.1.0/mathkit/cube_root.py
--rw-rw-rw-   0        0        0      153 2023-06-30 04:06:14.000000 mathkit-0.1.0/mathkit/division.py
--rw-rw-rw-   0        0        0      356 2023-06-30 06:12:35.000000 mathkit-0.1.0/mathkit/factorial.py
--rw-rw-rw-   0        0        0      388 2023-06-30 05:08:17.000000 mathkit-0.1.0/mathkit/hcf_custom.py
--rw-rw-rw-   0        0        0      526 2023-06-30 05:07:56.000000 mathkit-0.1.0/mathkit/lcm_custom.py
--rw-rw-rw-   0        0        0      574 2023-06-30 05:08:44.000000 mathkit-0.1.0/mathkit/log_custom.py
--rw-rw-rw-   0        0        0     1524 2023-06-30 06:13:55.000000 mathkit-0.1.0/mathkit/main.py
--rw-rw-rw-   0        0        0      158 2023-06-30 04:06:46.000000 mathkit-0.1.0/mathkit/modulas.py
--rw-rw-rw-   0        0        0      143 2023-06-30 04:04:06.000000 mathkit-0.1.0/mathkit/multiply.py
--rw-rw-rw-   0        0        0      940 2023-06-30 06:12:48.000000 mathkit-0.1.0/mathkit/percentage.py
--rw-rw-rw-   0        0        0      175 2023-06-30 06:18:16.000000 mathkit-0.1.0/mathkit/power.py
--rw-rw-rw-   0        0        0      226 2023-06-30 06:13:01.000000 mathkit-0.1.0/mathkit/remainder.py
--rw-rw-rw-   0        0        0      106 2023-06-30 04:09:37.000000 mathkit-0.1.0/mathkit/square.py
--rw-rw-rw-   0        0        0      105 2023-06-30 04:11:40.000000 mathkit-0.1.0/mathkit/square_root.py
--rw-rw-rw-   0        0        0      158 2023-06-30 04:01:39.000000 mathkit-0.1.0/mathkit/subtract.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:50:44.096003 mathkit-0.1.0/mathkit.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-06-30 06:50:43.000000 mathkit-0.1.0/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-06-30 06:50:43.000000 mathkit-0.1.0/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 06:50:43.000000 mathkit-0.1.0/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 06:50:43.000000 mathkit-0.1.0/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 06:50:44.107978 mathkit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2453 2023-06-30 06:47:36.000000 mathkit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:54:31.928839 mathkit-0.1.1/
+-rw-rw-rw-   0        0        0     2320 2023-06-30 06:54:31.927821 mathkit-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 06:54:31.908512 mathkit-0.1.1/mathkit/
+-rw-rw-rw-   0        0        0      966 2023-06-30 06:18:35.000000 mathkit-0.1.1/mathkit/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-06-30 04:01:47.000000 mathkit-0.1.1/mathkit/addition.py
+-rw-rw-rw-   0        0        0      117 2023-06-30 06:13:56.000000 mathkit-0.1.1/mathkit/cube.py
+-rw-rw-rw-   0        0        0      128 2023-06-30 05:06:59.000000 mathkit-0.1.1/mathkit/cube_root.py
+-rw-rw-rw-   0        0        0      153 2023-06-30 04:06:14.000000 mathkit-0.1.1/mathkit/division.py
+-rw-rw-rw-   0        0        0      356 2023-06-30 06:12:35.000000 mathkit-0.1.1/mathkit/factorial.py
+-rw-rw-rw-   0        0        0      388 2023-06-30 05:08:17.000000 mathkit-0.1.1/mathkit/hcf_custom.py
+-rw-rw-rw-   0        0        0      526 2023-06-30 05:07:56.000000 mathkit-0.1.1/mathkit/lcm_custom.py
+-rw-rw-rw-   0        0        0      574 2023-06-30 05:08:44.000000 mathkit-0.1.1/mathkit/log_custom.py
+-rw-rw-rw-   0        0        0     1524 2023-06-30 06:13:55.000000 mathkit-0.1.1/mathkit/main.py
+-rw-rw-rw-   0        0        0      158 2023-06-30 04:06:46.000000 mathkit-0.1.1/mathkit/modulas.py
+-rw-rw-rw-   0        0        0      143 2023-06-30 04:04:06.000000 mathkit-0.1.1/mathkit/multiply.py
+-rw-rw-rw-   0        0        0      940 2023-06-30 06:12:48.000000 mathkit-0.1.1/mathkit/percentage.py
+-rw-rw-rw-   0        0        0      175 2023-06-30 06:18:16.000000 mathkit-0.1.1/mathkit/power.py
+-rw-rw-rw-   0        0        0      226 2023-06-30 06:13:01.000000 mathkit-0.1.1/mathkit/remainder.py
+-rw-rw-rw-   0        0        0      106 2023-06-30 04:09:37.000000 mathkit-0.1.1/mathkit/square.py
+-rw-rw-rw-   0        0        0      105 2023-06-30 04:11:40.000000 mathkit-0.1.1/mathkit/square_root.py
+-rw-rw-rw-   0        0        0      158 2023-06-30 04:01:39.000000 mathkit-0.1.1/mathkit/subtract.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:54:31.926821 mathkit-0.1.1/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     2320 2023-06-30 06:54:31.000000 mathkit-0.1.1/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-06-30 06:54:31.000000 mathkit-0.1.1/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 06:54:31.000000 mathkit-0.1.1/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 06:54:31.000000 mathkit-0.1.1/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 06:54:31.928839 mathkit-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2448 2023-06-30 06:54:28.000000 mathkit-0.1.1/setup.py
```

### Comparing `mathkit-0.1.0/PKG-INFO` & `mathkit-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Math Simplifies - A Python library for mathematical calculations.
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhecker@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 
-Math Simplifies is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations. 
+Math Simplifies is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
 
 Example Usage:
 from addition import add
 from subtract import sub
 from multiply import mul
 from division import div
 from modulas import mod
@@ -30,15 +30,14 @@
 from factorial import fact
 from percentage import percent
 from remainder import remain
 from lcm_custom import lcm
 from hcf_custom import hcf
 from log_custom import log
 
-
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
 print("3. Multiplication")
 print("4. Division")
 print("5. Modulas")
 print("6. Power")
@@ -50,15 +49,14 @@
 print("12. Percentage")
 print("13. Remainder")
 print("14. LCM")
 print("15. HCF")
 print("16. Logarithm")
 print("17. Exit")
 
-
 choice = int(input("Enter your choice: "))
 
 if choice == 1:
     add()
 elif choice == 2:
     sub()
 elif choice == 3:
```

### Comparing `mathkit-0.1.0/mathkit/__init__.py` & `mathkit-0.1.1/mathkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.1.0/mathkit/lcm_custom.py` & `mathkit-0.1.1/mathkit/lcm_custom.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.1.0/mathkit/log_custom.py` & `mathkit-0.1.1/mathkit/log_custom.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.1.0/mathkit/main.py` & `mathkit-0.1.1/mathkit/main.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.1.0/mathkit/percentage.py` & `mathkit-0.1.1/mathkit/percentage.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.1.0/mathkit.egg-info/PKG-INFO` & `mathkit-0.1.1/mathkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Math Simplifies - A Python library for mathematical calculations.
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhecker@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 
-Math Simplifies is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations. 
+Math Simplifies is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
 
 Example Usage:
 from addition import add
 from subtract import sub
 from multiply import mul
 from division import div
 from modulas import mod
@@ -30,15 +30,14 @@
 from factorial import fact
 from percentage import percent
 from remainder import remain
 from lcm_custom import lcm
 from hcf_custom import hcf
 from log_custom import log
 
-
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
 print("3. Multiplication")
 print("4. Division")
 print("5. Modulas")
 print("6. Power")
@@ -50,15 +49,14 @@
 print("12. Percentage")
 print("13. Remainder")
 print("14. LCM")
 print("15. HCF")
 print("16. Logarithm")
 print("17. Exit")
 
-
 choice = int(input("Enter your choice: "))
 
 if choice == 1:
     add()
 elif choice == 2:
     sub()
 elif choice == 3:
```

### Comparing `mathkit-0.1.0/setup.py` & `mathkit-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='mathkit',
-    version='0.1.0',
+    version='0.1.1',
     description='Math Simplifies - A Python library for mathematical calculations.',
-    long_description='''Math Simplifies is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations. 
+    long_description='''Math Simplifies is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
 
 Example Usage:
 from addition import add
 from subtract import sub
 from multiply import mul
 from division import div
 from modulas import mod
@@ -20,15 +20,14 @@
 from factorial import fact
 from percentage import percent
 from remainder import remain
 from lcm_custom import lcm
 from hcf_custom import hcf
 from log_custom import log
 
-
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
 print("3. Multiplication")
 print("4. Division")
 print("5. Modulas")
 print("6. Power")
@@ -40,15 +39,14 @@
 print("12. Percentage")
 print("13. Remainder")
 print("14. LCM")
 print("15. HCF")
 print("16. Logarithm")
 print("17. Exit")
 
-
 choice = int(input("Enter your choice: "))
 
 if choice == 1:
     add()
 elif choice == 2:
     sub()
 elif choice == 3:
```

