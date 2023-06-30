# Comparing `tmp/cetpy-0.0.1.tar.gz` & `tmp/cetpy-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cetpy-0.0.1.tar", last modified: Thu Jun 29 23:24:59 2023, max compression
+gzip compressed data, was "cetpy-0.0.1.post1.tar", last modified: Fri Jun 30 00:34:05 2023, max compression
```

## Comparing `cetpy-0.0.1.tar` & `cetpy-0.0.1.post1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-29 23:24:49.000000 cetpy-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 23:24:49.000000 cetpy-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-29 23:24:59.472666 cetpy-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-29 23:24:49.000000 cetpy-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.468666 cetpy-0.0.1/cetpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Configuration/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Configuration/_Session.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Configuration/default_config_parameters.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Modules/Fluid/
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Fluid/_FluidCoolProp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Fluid/_FluidSkeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Fluid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Modules/Material/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Material/_MaterialGiven.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Material/_MaterialSkeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Material/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Modules/Solver/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Solver/_Solver.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Solver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Modules/SysML/
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/SysML/_Block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/SysML/_PartProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/SysML/_ValueProperty.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/SysML/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy/Modules/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Utilities/Labelling.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/Modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 23:24:49.000000 cetpy-0.0.1/cetpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:24:59.472666 cetpy-0.0.1/cetpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-29 23:24:59.000000 cetpy-0.0.1/cetpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-29 23:24:59.000000 cetpy-0.0.1/cetpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:24:59.000000 cetpy-0.0.1/cetpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 23:24:59.000000 cetpy-0.0.1/cetpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 23:24:59.000000 cetpy-0.0.1/cetpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 23:24:49.000000 cetpy-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 23:24:59.472666 cetpy-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-29 23:24:49.000000 cetpy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.271528 cetpy-0.0.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-30 00:34:05.271528 cetpy-0.0.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Configuration/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Configuration/_Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Configuration/default_config_parameters.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/Modules/Fluid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Fluid/_FluidCoolProp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Fluid/_FluidSkeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Fluid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/Modules/Material/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Material/_MaterialGiven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Material/_MaterialSkeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Material/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/Modules/Solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Solver/_Solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Solver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy/Modules/SysML/
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/SysML/_Block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/SysML/_PartProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/SysML/_ValueProperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/SysML/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.271528 cetpy-0.0.1.post1/cetpy/Modules/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Utilities/Labelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/Modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/cetpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:34:05.267528 cetpy-0.0.1.post1/cetpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-30 00:34:05.000000 cetpy-0.0.1.post1/cetpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 00:34:05.000000 cetpy-0.0.1.post1/cetpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:34:05.000000 cetpy-0.0.1.post1/cetpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 00:34:05.000000 cetpy-0.0.1.post1/cetpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 00:34:05.000000 cetpy-0.0.1.post1/cetpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 00:34:05.271528 cetpy-0.0.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-30 00:33:55.000000 cetpy-0.0.1.post1/setup.py
```

### Comparing `cetpy-0.0.1/LICENSE.txt` & `cetpy-0.0.1.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/PKG-INFO` & `cetpy-0.0.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cetpy
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Congruent Engineering Toolbox
 Home-page: https://github.com/CongruentEngineeringToolbox/cetpy
 Author: CET developers
 Keywords: engineering,system engineering,congruent engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cetpy-0.0.1/cetpy/Configuration/_ConfigurationManager.py` & `cetpy-0.0.1.post1/cetpy/Configuration/_ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Configuration/_Session.py` & `cetpy-0.0.1.post1/cetpy/Configuration/_Session.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/Fluid/_FluidCoolProp.py` & `cetpy-0.0.1.post1/cetpy/Modules/Fluid/_FluidCoolProp.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/Fluid/_FluidSkeleton.py` & `cetpy-0.0.1.post1/cetpy/Modules/Fluid/_FluidSkeleton.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/Material/_MaterialGiven.py` & `cetpy-0.0.1.post1/cetpy/Modules/Material/_MaterialGiven.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/Material/_MaterialSkeleton.py` & `cetpy-0.0.1.post1/cetpy/Modules/Material/_MaterialSkeleton.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/Solver/_Solver.py` & `cetpy-0.0.1.post1/cetpy/Modules/Solver/_Solver.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/SysML/_Block.py` & `cetpy-0.0.1.post1/cetpy/Modules/SysML/_Block.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/SysML/_PartProperty.py` & `cetpy-0.0.1.post1/cetpy/Modules/SysML/_PartProperty.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/SysML/_ValueProperty.py` & `cetpy-0.0.1.post1/cetpy/Modules/SysML/_ValueProperty.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy/Modules/Utilities/Labelling.py` & `cetpy-0.0.1.post1/cetpy/Modules/Utilities/Labelling.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/cetpy.egg-info/PKG-INFO` & `cetpy-0.0.1.post1/cetpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cetpy
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Congruent Engineering Toolbox
 Home-page: https://github.com/CongruentEngineeringToolbox/cetpy
 Author: CET developers
 Keywords: engineering,system engineering,congruent engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cetpy-0.0.1/cetpy.egg-info/SOURCES.txt` & `cetpy-0.0.1.post1/cetpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cetpy-0.0.1/setup.py` & `cetpy-0.0.1.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='cetpy',
-    version='0.0.1',
+    version='0.0.1.post1',
     description='Congruent Engineering Toolbox',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CongruentEngineeringToolbox/cetpy",
     author='CET developers',
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

