# Comparing `tmp/teamanchorhello-0.0.4.tar.gz` & `tmp/teamanchorhello-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamanchorhello-0.0.4.tar", last modified: Thu Jun 29 18:44:26 2023, max compression
+gzip compressed data, was "teamanchorhello-0.0.5.tar", last modified: Thu Jun 29 18:53:35 2023, max compression
```

## Comparing `teamanchorhello-0.0.4.tar` & `teamanchorhello-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.4/LICENSE
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1857 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1161 2023-06-29 18:43:23.000000 teamanchorhello-0.0.4/README.md
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/setup.cfg
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-29 18:43:38.000000 teamanchorhello-0.0.4/setup.py
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/teamanchorhello/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/teamanchorhello/src/
-drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:44:26.882962 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1857 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-29 18:44:26.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
--rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-29 18:43:40.000000 teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:53:35.816958 teamanchorhello-0.0.5/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       11 2023-06-29 18:10:08.000000 teamanchorhello-0.0.5/LICENSE
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     2151 2023-06-29 18:53:35.816958 teamanchorhello-0.0.5/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     1407 2023-06-29 18:53:01.000000 teamanchorhello-0.0.5/README.md
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       38 2023-06-29 18:53:35.816958 teamanchorhello-0.0.5/setup.cfg
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      690 2023-06-29 18:53:05.000000 teamanchorhello-0.0.5/setup.py
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:53:35.816958 teamanchorhello-0.0.5/teamanchorhello/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:53:35.816958 teamanchorhello-0.0.5/teamanchorhello/src/
+drwxr-xr-x   0 aoshfan   (1000) aoshfan   (1000)        0 2023-06-29 18:53:35.816958 teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.egg-info/
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)     2151 2023-06-29 18:53:35.000000 teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)      301 2023-06-29 18:53:35.000000 teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.egg-info/SOURCES.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)        1 2023-06-29 18:53:35.000000 teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.egg-info/dependency_links.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       16 2023-06-29 18:53:35.000000 teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.egg-info/top_level.txt
+-rw-r--r--   0 aoshfan   (1000) aoshfan   (1000)       54 2023-06-29 18:52:55.000000 teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.py
```

### Comparing `teamanchorhello-0.0.4/PKG-INFO` & `teamanchorhello-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.4
+Version: 0.0.5
 Summary: teamanchor say hello using Pypi package.
 Home-page: UNKNOWN
 Author: fanis
 License: UNKNOWN
 Description: ## TEAMANCHORHELLO
         
         Team Anchor say hello using Pypi package.
         
-        
+        ## VENV
+        Active: source venv/bin/activate
+        Deactive: deactivate
         ## UPDATE PACKAGE
         1. $vim teamanchorhello\src\teamanchorhello.py
             * print('Team Anchor say hello <UPDATE>')
         2. $vim setup.py
             * version: <UPDATE>
         3. python3 setup.py sdist bdist_wheel
             * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
         4. pip3 install -e .
         5. pyhon3
             * import teamanchorhello
             * teamanchorhello.hello()
-        6. Upload to testpypi:
+        6. Upload to testpypi (can't upload same file version else delete dist/*):
             * python3 -m twine upload --repository testpypi dist/*
                 * Enter user & password (register if you didn't have).
         7. Upload to pypi:
             * python3 -m twine upload dist/*
         
-        ## FASTEST WAY
+        ## UPDATE PACKAGE - FASTEST WAY
         1. $vim teamanchorhello\src\teamanchorhello.py
             * print('Team Anchor say hello <UPDATE>')
         2. $vim setup.py
             * version: <UPDATE>
-        3. Delete file in dist/*
-            * rm -rf dist/*
-        4. Upload to Pypi:
+        3. Upload to Pypi:
             * python3 -m twine upload dist/*
+        
+        ## HOW TO USE
+        1. $ pip3 install teamanchorhello
+        2. $ pyhon3
+        3. >> import teamanchorhello
+        4. >> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5
         ## PYPI
-        TESTPYPI: https://test.pypi.org/project/teamanchorhello/
+        TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
         PYPI: https://pypi.org/project/teamanchorhello/
         
         ## CERTIFICATE ISSUE
         * Can't use venv, exit venv & upload to Pypi.
         * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `teamanchorhello-0.0.4/README.md` & `teamanchorhello-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 ## TEAMANCHORHELLO
 
 Team Anchor say hello using Pypi package.
 
-
+## VENV
+Active: source venv/bin/activate
+Deactive: deactivate
 ## UPDATE PACKAGE
 1. $vim teamanchorhello\src\teamanchorhello.py
     * print('Team Anchor say hello <UPDATE>')
 2. $vim setup.py
     * version: <UPDATE>
 3. python3 setup.py sdist bdist_wheel
     * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
 4. pip3 install -e .
 5. pyhon3
     * import teamanchorhello
     * teamanchorhello.hello()
-6. Upload to testpypi:
+6. Upload to testpypi (can't upload same file version else delete dist/*):
     * python3 -m twine upload --repository testpypi dist/*
         * Enter user & password (register if you didn't have).
 7. Upload to pypi:
     * python3 -m twine upload dist/*
 
-## FASTEST WAY
+## UPDATE PACKAGE - FASTEST WAY
 1. $vim teamanchorhello\src\teamanchorhello.py
     * print('Team Anchor say hello <UPDATE>')
 2. $vim setup.py
     * version: <UPDATE>
-3. Delete file in dist/*
-    * rm -rf dist/*
-4. Upload to Pypi:
+3. Upload to Pypi:
     * python3 -m twine upload dist/*
+
+## HOW TO USE
+1. $ pip3 install teamanchorhello
+2. $ pyhon3
+3. >> import teamanchorhello
+4. >> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5
 ## PYPI
-TESTPYPI: https://test.pypi.org/project/teamanchorhello/
+TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
 PYPI: https://pypi.org/project/teamanchorhello/
 
 ## CERTIFICATE ISSUE
 * Can't use venv, exit venv & upload to Pypi.
 * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
```

### Comparing `teamanchorhello-0.0.4/setup.py` & `teamanchorhello-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="teamanchorhello",
-    version="0.0.4",
+    version="0.0.5",
     author="fanis",
     description="teamanchor say hello using Pypi package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `teamanchorhello-0.0.4/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO` & `teamanchorhello-0.0.5/teamanchorhello/src/teamanchorhello.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 Metadata-Version: 2.1
 Name: teamanchorhello
-Version: 0.0.4
+Version: 0.0.5
 Summary: teamanchor say hello using Pypi package.
 Home-page: UNKNOWN
 Author: fanis
 License: UNKNOWN
 Description: ## TEAMANCHORHELLO
         
         Team Anchor say hello using Pypi package.
         
-        
+        ## VENV
+        Active: source venv/bin/activate
+        Deactive: deactivate
         ## UPDATE PACKAGE
         1. $vim teamanchorhello\src\teamanchorhello.py
             * print('Team Anchor say hello <UPDATE>')
         2. $vim setup.py
             * version: <UPDATE>
         3. python3 setup.py sdist bdist_wheel
             * verify vesion update: $ cat teamanchorhello\src\teamanchorhello.egg-info\PKG-INFO
         4. pip3 install -e .
         5. pyhon3
             * import teamanchorhello
             * teamanchorhello.hello()
-        6. Upload to testpypi:
+        6. Upload to testpypi (can't upload same file version else delete dist/*):
             * python3 -m twine upload --repository testpypi dist/*
                 * Enter user & password (register if you didn't have).
         7. Upload to pypi:
             * python3 -m twine upload dist/*
         
-        ## FASTEST WAY
+        ## UPDATE PACKAGE - FASTEST WAY
         1. $vim teamanchorhello\src\teamanchorhello.py
             * print('Team Anchor say hello <UPDATE>')
         2. $vim setup.py
             * version: <UPDATE>
-        3. Delete file in dist/*
-            * rm -rf dist/*
-        4. Upload to Pypi:
+        3. Upload to Pypi:
             * python3 -m twine upload dist/*
+        
+        ## HOW TO USE
+        1. $ pip3 install teamanchorhello
+        2. $ pyhon3
+        3. >> import teamanchorhello
+        4. >> teamanchorhello.hello() // Output: Team Anchor say hello 0.0.5
         ## PYPI
-        TESTPYPI: https://test.pypi.org/project/teamanchorhello/
+        TESTPYPI: https://test.pypi.org/project/teamanchorhello/  
         PYPI: https://pypi.org/project/teamanchorhello/
         
         ## CERTIFICATE ISSUE
         * Can't use venv, exit venv & upload to Pypi.
         * If use Python >= 3.10, maybe can use https://pip.pypa.io/en/latest/topics/https-certificates/.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

