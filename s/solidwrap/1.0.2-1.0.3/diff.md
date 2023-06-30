# Comparing `tmp/solidwrap-1.0.2.tar.gz` & `tmp/solidwrap-1.0.3.tar.gz`

## Comparing `solidwrap-1.0.2.tar` & `solidwrap-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 solidwrap-1.0.2/info/API Reference.rst
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/__init__.py
--rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/solidwrap.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/extensions/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/extensions/extensions.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/profiling/__init__.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/profiling/profiling.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.2/tests/test.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 solidwrap-1.0.2/../README.rst
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 solidwrap-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 solidwrap-1.0.3/info/API Reference.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/__init__.py
+-rw-r--r--   0        0        0    13939 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/extensions/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/extensions/extensions.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/utilities/__init__.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/utilities/utilities.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.3/tests/test.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.3/../README.rst
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.3/PKG-INFO
```

### Comparing `solidwrap-1.0.2/info/API Reference.rst` & `solidwrap-1.0.3/info/API Reference.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.2/solidwrap/solidwrap.py` & `solidwrap-1.0.3/solidwrap/solidwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # Standard imports
 import os                                   # manipulate folders
 import win32com.client  as win              # COM object handling
 import pythoncom        as pycom            # used in conjunction with win32com.client
 import subprocess       as subproc          # quick process disconnect
 
 # Project imports
-from .profiling        import profile       # function execution timing
+from .utilities        import singleton     # singleton enforcement
+from .utilities        import profile       # process timing
 
 
 # ---------------------
 # II. Import Definition
 # ---------------------
 
 __all__ = [
@@ -46,14 +47,15 @@
     # Special Methods
     # ---------------
     def __init__(self, model):
         self.filepath = Filepath(model.GetPathName) # Filepath
         self.swobj = model                          # IModelDoc2
 
 # Core class
+@singleton
 class SolidWorks:
     """
     SolidWorks
     ---------
     Wrapper for SolidWorks API. Represents the top-level application.
     """
     # Attributes
@@ -240,14 +242,15 @@
         # Execute SW-API Method: ViewZoomtofit2 - center model in viewport
         model.swobj.ViewZoomtofit2()
 
         # Execute SW-API Method: InsertScene - force background to plain white
         model.swobj.Extension.InsertScene(fr"\scenes\01 basic scenes\11 white kitchen.p2s")
 
 # Core class
+@singleton
 class Vault:
     """
     Vault
     ---------
     Wrapper for SolidWorks PDM API. Represents PDM Vault.
     """
     # Attributes
```

### Comparing `solidwrap-1.0.2/tests/test.py` & `solidwrap-1.0.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.2/pyproject.toml` & `solidwrap-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Sean Yeatts" },
 ]
 license = {text = "MIT License"}
 description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "../README.rst"
 requires-python = ">=3.7"
```

### Comparing `solidwrap-1.0.2/../README.rst` & `solidwrap-1.0.3/../README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 This module wraps the SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 
 Key Features
 ------------
 - Intuitive Pythonic syntax for interacting with SolidWorks models & PDM states.
-- Logging and report generation for profiling automation performance. <-- ( under development )
+- Process profiling for insights into automated task performance.
 - Full API documentation detailing module components.
 
 Navigate to the `API Reference <https://github.com/SeanYeatts/SolidWrap/blob/main/solidwrap/info/API%20Reference.rst>`_ for a complete walkthrough of the module.
 
 Quickstart
 ----------
 
@@ -72,11 +72,11 @@
 
 **For a local installation**
 
 Extract the contents of this module to a safe location. Open a new terminal and navigate to the top level directory of your project. Run the following command:
 
 .. code:: sh
 
-  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-0.0.1.tar.gz"
+  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-1.0.0.tar.gz"
 
 - ``DIRECTORY_HERE`` should be replaced with the complete filepath to the folder where you saved the SolidWrap module contents.
-- Depending on the version of SolidWrap you've chosen, you may have to change ``0.0.1`` to reflect your specific version.
+- Depending on the version of SolidWrap you've chosen, you may have to change ``1.0.0`` to reflect your specific version.
```

### Comparing `solidwrap-1.0.2/PKG-INFO` & `solidwrap-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidwrap
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/users/SeanYeatts/projects/6/views/1
 Author: Sean Yeatts
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,15 +18,15 @@
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 This module wraps the SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 
 Key Features
 ------------
 - Intuitive Pythonic syntax for interacting with SolidWorks models & PDM states.
-- Logging and report generation for profiling automation performance. <-- ( under development )
+- Process profiling for insights into automated task performance.
 - Full API documentation detailing module components.
 
 Navigate to the `API Reference <https://github.com/SeanYeatts/SolidWrap/blob/main/solidwrap/info/API%20Reference.rst>`_ for a complete walkthrough of the module.
 
 Quickstart
 ----------
 
@@ -86,11 +86,11 @@
 
 **For a local installation**
 
 Extract the contents of this module to a safe location. Open a new terminal and navigate to the top level directory of your project. Run the following command:
 
 .. code:: sh
 
-  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-0.0.1.tar.gz"
+  py -m pip install "DIRECTORY_HERE\solidwrap\dist\solidwrap-1.0.0.tar.gz"
 
 - ``DIRECTORY_HERE`` should be replaced with the complete filepath to the folder where you saved the SolidWrap module contents.
-- Depending on the version of SolidWrap you've chosen, you may have to change ``0.0.1`` to reflect your specific version.
+- Depending on the version of SolidWrap you've chosen, you may have to change ``1.0.0`` to reflect your specific version.
```

