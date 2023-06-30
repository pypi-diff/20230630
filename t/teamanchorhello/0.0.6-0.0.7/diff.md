# Comparing `tmp/teamanchorhello-0.0.6.tar.gz` & `tmp/teamanchorhello-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamanchorhello-0.0.6.tar", last modified: Fri Jun 30 02:50:30 2023, max compression
+gzip compressed data, was "teamanchorhello-0.0.7.tar", last modified: Fri Jun 30 03:36:22 2023, max compression
```

## Comparing `teamanchorhello-0.0.6.tar` & `teamanchorhello-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 02:50:30.026519 teamanchorhello-0.0.6/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.6/LICENSE
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     2157 2023-06-30 02:50:30.026519 teamanchorhello-0.0.6/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1413 2023-06-29 18:56:03.000000 teamanchorhello-0.0.6/README.md
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-30 02:50:30.026519 teamanchorhello-0.0.6/setup.cfg
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-30 02:49:46.000000 teamanchorhello-0.0.6/setup.py
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 02:50:30.026519 teamanchorhello-0.0.6/teamanchorhello/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 02:50:30.026519 teamanchorhello-0.0.6/teamanchorhello/src/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 02:50:30.026519 teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.egg-info/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     2157 2023-06-30 02:50:29.000000 teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-30 02:50:30.000000 teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-30 02:50:29.000000 teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-30 02:50:29.000000 teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-30 02:49:50.000000 teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.7/LICENSE
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1769 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1413 2023-06-29 18:56:03.000000 teamanchorhello-0.0.7/README.md
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/setup.cfg
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-30 03:35:58.000000 teamanchorhello-0.0.7/setup.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/teamanchorhello/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/teamanchorhello/src/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-30 03:36:22.206382 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1769 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-30 03:36:22.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-30 03:36:02.000000 teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.py
```

### Comparing `teamanchorhello-0.0.6/PKG-INFO` & `teamanchorhello-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.6
+Version: 0.0.7
 Summary: teamanchor say hello using Pypi package.
-Home-page: UNKNOWN
 Author: fanis
-License: UNKNOWN
-Description: ## TEAMANCHORHELLO
-        
-        Team Anchor say hello using Pypi package.
-        
-        ## VENV
-        Active: source venv/bin/activate  
-        Deactive: deactivate
-        ## UPDATE PACKAGE
-        1. $vim teamanchorhello\src\teamanchorhello.py
-            * print('Team Anchor say hello <UPDATE>')
-        2. $vim setup.py
-            * version: <UPDATE>
-        3. python3 setup.py sdist bdist_wheel
-            * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
-        4. pip3 install -e .
-        5. pyhon3
-            * import teamanchorhello
-            * teamanchorhello.hello()
-        6. Upload to testpypi (can't upload same file version else delete dist/*):
-            * python3 -m twine upload --repository testpypi dist/*
-                * Enter user & password (register if you didn't have).
-        7. Upload to pypi:
-            * python3 -m twine upload dist/*
-        
-        ## UPDATE PACKAGE - FASTEST WAY
-        1. $vim teamanchorhello\src\teamanchorhello.py
-            * print('Team Anchor say hello <UPDATE>')
-        2. $vim setup.py
-            * version: <UPDATE>
-        3. Upload to Pypi:
-            * python3 -m twine upload dist/*
-        
-        ## HOW TO USE
-        1. $ pip3 install teamanchorhello
-        2. $ pyhon3
-        3. `>> import teamanchorhello`
-        4. `>> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5`
-        ## PYPI
-        TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
-        PYPI: https://pypi.org/project/teamanchorhello/
-        
-        ## CERTIFICATE ISSUE
-        * Can't use venv, exit venv & upload to Pypi.
-        * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## TEAMANCHORHELLO
+
+Team Anchor say hello using Pypi package.
+
+## VENV
+Active: source venv/bin/activate  
+Deactive: deactivate
+## UPDATE PACKAGE
+1. $vim teamanchorhello\src\teamanchorhello.py
+    * print('Team Anchor say hello <UPDATE>')
+2. $vim setup.py
+    * version: <UPDATE>
+3. python3 setup.py sdist bdist_wheel
+    * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
+4. pip3 install -e .
+5. pyhon3
+    * import teamanchorhello
+    * teamanchorhello.hello()
+6. Upload to testpypi (can't upload same file version else delete dist/*):
+    * python3 -m twine upload --repository testpypi dist/*
+        * Enter user & password (register if you didn't have).
+7. Upload to pypi:
+    * python3 -m twine upload dist/*
+
+## UPDATE PACKAGE - FASTEST WAY
+1. $vim teamanchorhello\src\teamanchorhello.py
+    * print('Team Anchor say hello <UPDATE>')
+2. $vim setup.py
+    * version: <UPDATE>
+3. Upload to Pypi:
+    * python3 -m twine upload dist/*
+
+## HOW TO USE
+1. $ pip3 install teamanchorhello
+2. $ pyhon3
+3. `>> import teamanchorhello`
+4. `>> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5`
+## PYPI
+TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
+PYPI: https://pypi.org/project/teamanchorhello/
+
+## CERTIFICATE ISSUE
+* Can't use venv, exit venv & upload to Pypi.
+* If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
```

### Comparing `teamanchorhello-0.0.6/README.md` & `teamanchorhello-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `teamanchorhello-0.0.6/setup.py` & `teamanchorhello-0.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="teamanchorhello",
-    version="0.0.6",
+    version="0.0.7",
     author="fanis",
     description="teamanchor say hello using Pypi package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `teamanchorhello-0.0.6/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO` & `teamanchorhello-0.0.7/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.6
+Version: 0.0.7
 Summary: teamanchor say hello using Pypi package.
-Home-page: UNKNOWN
 Author: fanis
-License: UNKNOWN
-Description: ## TEAMANCHORHELLO
-        
-        Team Anchor say hello using Pypi package.
-        
-        ## VENV
-        Active: source venv/bin/activate  
-        Deactive: deactivate
-        ## UPDATE PACKAGE
-        1. $vim teamanchorhello\src\teamanchorhello.py
-            * print('Team Anchor say hello <UPDATE>')
-        2. $vim setup.py
-            * version: <UPDATE>
-        3. python3 setup.py sdist bdist_wheel
-            * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
-        4. pip3 install -e .
-        5. pyhon3
-            * import teamanchorhello
-            * teamanchorhello.hello()
-        6. Upload to testpypi (can't upload same file version else delete dist/*):
-            * python3 -m twine upload --repository testpypi dist/*
-                * Enter user & password (register if you didn't have).
-        7. Upload to pypi:
-            * python3 -m twine upload dist/*
-        
-        ## UPDATE PACKAGE - FASTEST WAY
-        1. $vim teamanchorhello\src\teamanchorhello.py
-            * print('Team Anchor say hello <UPDATE>')
-        2. $vim setup.py
-            * version: <UPDATE>
-        3. Upload to Pypi:
-            * python3 -m twine upload dist/*
-        
-        ## HOW TO USE
-        1. $ pip3 install teamanchorhello
-        2. $ pyhon3
-        3. `>> import teamanchorhello`
-        4. `>> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5`
-        ## PYPI
-        TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
-        PYPI: https://pypi.org/project/teamanchorhello/
-        
-        ## CERTIFICATE ISSUE
-        * Can't use venv, exit venv & upload to Pypi.
-        * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## TEAMANCHORHELLO
+
+Team Anchor say hello using Pypi package.
+
+## VENV
+Active: source venv/bin/activate  
+Deactive: deactivate
+## UPDATE PACKAGE
+1. $vim teamanchorhello\src\teamanchorhello.py
+    * print('Team Anchor say hello <UPDATE>')
+2. $vim setup.py
+    * version: <UPDATE>
+3. python3 setup.py sdist bdist_wheel
+    * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
+4. pip3 install -e .
+5. pyhon3
+    * import teamanchorhello
+    * teamanchorhello.hello()
+6. Upload to testpypi (can't upload same file version else delete dist/*):
+    * python3 -m twine upload --repository testpypi dist/*
+        * Enter user & password (register if you didn't have).
+7. Upload to pypi:
+    * python3 -m twine upload dist/*
+
+## UPDATE PACKAGE - FASTEST WAY
+1. $vim teamanchorhello\src\teamanchorhello.py
+    * print('Team Anchor say hello <UPDATE>')
+2. $vim setup.py
+    * version: <UPDATE>
+3. Upload to Pypi:
+    * python3 -m twine upload dist/*
+
+## HOW TO USE
+1. $ pip3 install teamanchorhello
+2. $ pyhon3
+3. `>> import teamanchorhello`
+4. `>> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5`
+## PYPI
+TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
+PYPI: https://pypi.org/project/teamanchorhello/
+
+## CERTIFICATE ISSUE
+* Can't use venv, exit venv & upload to Pypi.
+* If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
```

