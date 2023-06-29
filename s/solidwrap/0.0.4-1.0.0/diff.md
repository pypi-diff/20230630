# Comparing `tmp/solidwrap-0.0.4.tar.gz` & `tmp/solidwrap-1.0.0.tar.gz`

## Comparing `solidwrap-0.0.4.tar` & `solidwrap-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,10 @@
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 solidwrap-0.0.4/setup.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 solidwrap-0.0.4/info/API Reference.rst
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 solidwrap-0.0.4/info/LICENSE
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap/__init__.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap/solidwrap.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap/extensions/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap/extensions/extensions.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap.egg-info/PKG-INFO
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap.egg-info/requires.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 solidwrap-0.0.4/solidwrap.egg-info/top_level.txt
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 solidwrap-0.0.4/tests/test.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 solidwrap-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 solidwrap-0.0.4/../README.rst
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 solidwrap-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 solidwrap-1.0.0/info/API Reference.rst
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 solidwrap-1.0.0/info/LICENSE
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 solidwrap-1.0.0/solidwrap/__init__.py
+-rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 solidwrap-1.0.0/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 solidwrap-1.0.0/solidwrap/extensions/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 solidwrap-1.0.0/solidwrap/extensions/extensions.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.0/tests/test.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 solidwrap-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 solidwrap-1.0.0/../README.rst
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 solidwrap-1.0.0/PKG-INFO
```

### Comparing `solidwrap-0.0.4/info/API Reference.rst` & `solidwrap-1.0.0/info/API Reference.rst`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 The SolidWorks API ( `SW-API <https://help.solidworks.com/2019/English/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1>`_ ) and PDM API ( `PDM-API <https://help.solidworks.com/2019/English/api/epdmapi/Welcome-epdmapi.html?id=2a67aaceb6984695a5ce8a75121853f3#Pg0>`_ ) are built on the Component Object Model ( `COM <https://learn.microsoft.com/en-us/windows/win32/com/component-object-model--com--portal>`_ ) to provide an interface with SolidWorks applications. They do not, however, have direct support for Python. SolidWrap leverages its own implementation of the COM pipeline to provide a streamlined Pythonic interface with SW-API and PDM-API.
 
 The core of SolidWrap relies on two objects: ``solidworks`` and ``vault``. These are treated as singletons; they come pre-instanced by the module and should not be manually created by the user. Most interactions with SolidWrap should flow through these objects.
 
 See the Appendix for an overview of the helper classes ( ``Filepath`` & ``Model`` ) that are embedded in many of the SolidWrap class methods.
 
+*NOTE: Items with a 'WIP' label are in development and are not garaunteed to function appropriately.*
+
 ``solidworks`` ( object )
 -------------------------
 The core object of the API. It serves as a representation of SolidWorks, and is responsible for handling all SolidWorks commands.
 
 Attributes
 ``````````
 - client ( `ISldWorks <https://help.solidworks.com/2019/english/api/sldworksapi/solidworks.interop.sldworks~solidworks.interop.sldworks.isldworks.html?verRedirect=1>`_ ) - Top level interface for SW-API
@@ -135,36 +137,36 @@
   # Checks out model from PDM Vault.
   def checkout(filepath: Filepath):
     """
     Parameters:
       - filepath ( Filepath ) - Target file to check out.
     """
 
-  # Checks out multiple models from the PDM Vault.
+  # WIP - Checks out multiple models from the PDM Vault.
   def batch_checkout(files):
     """
     Parameters:
       - files ( Filepath ) - Target files to check out.
     """
 
   # Checks in model from PDM Vault.
   def checkin(filepath: Filepath):
     """
     Parameters:
       - filepath ( Filepath ) - Target file to check in.
     """
 
-  # Checks in multiple models from the PDM Vault.
+  # WIP - Checks in multiple models from the PDM Vault.
   def batch_checkin(files):
     """
     Parameters:
       - files ( Filepath ) - Target files to check in.
     """
 
-  # Changes model's PDM state to the prescribed value, if allowed.
+  # WIP - Changes model's PDM state to the prescribed value, if allowed.
   def change_state(filepath: Filepath, state: str = "WIP", message: str = "SolidWrap Automated State Change"):
     """
     Parameters:
       - filepath ( Filepath ) - Target file whos state should change.
       - state ( str ) - Literal name of the target state.
       - message ( str ) - Message to include in the file's PDM history.
     """
```

### Comparing `solidwrap-0.0.4/info/LICENSE` & `solidwrap-1.0.0/info/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 Sean Yeatts
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `solidwrap-0.0.4/solidwrap/solidwrap.py` & `solidwrap-1.0.0/solidwrap/solidwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 """
 Copyright (c) 2023 Sean Yeatts. All rights reserved.
 """
+
 # ----------------------
 # I. Module Dependencies
 # ----------------------
-import os                                   # manipulate windows folders
+
+# 3rd Party Imports
+from quickpathstr       import Filepath     # syntax standardization helper
+
+# Standard Imports
+import os                                   # manipulate folders
 import win32com.client  as win              # COM object handling
 import pythoncom        as pycom            # used in conjunction with win32com.client
 import subprocess       as subproc          # quick process disconnect
-from quickpathstr       import Filepath     # file syntax standardization
-
-
-# ------------------------
-# II. Forward Declarations
-# ------------------------
-class SolidWorks:   pass
-class Vault:        pass
-class Model:        pass
 
 
 # ------------
-# III. Classes
+# II. Classes
 # ------------
+
+# Helper class
+class Model:
+    """
+    Model
+    -----
+    Convenience wrapper for SolidWorks IModelDoc2 objects.
+    """
+    # Special Methods
+    # ---------------
+    def __init__(self, model):
+        self.filepath = Filepath(model.GetPathName) # Filepath
+        self.swobj = model                          # IModelDoc2
+
+# Core class
 class SolidWorks:
     """
     SolidWorks
     ---------
     Wrapper for SolidWorks API. Represents the top-level application.
     """
     # Attributes
@@ -200,14 +212,15 @@
 
         # Execute SW-API Method: ViewZoomtofit2 - center model in viewport
         model.swobj.ViewZoomtofit2()
 
         # Execute SW-API Method: InsertScene - force background to plain white
         model.swobj.Extension.InsertScene(fr"\scenes\01 basic scenes\11 white kitchen.p2s")
 
+# Core class
 class Vault:
     """
     Vault
     ---------
     Wrapper for SolidWorks PDM API. Represents PDM Vault.
     """
     # Attributes
@@ -255,14 +268,15 @@
 
         # Execute PDM-API method
         if not file.IsLocked:                       # if file is not checked out...
             file.LockFile(directory.ID, 0)          # check out file
         else:
             print(f"File is already checked out!")  # ...else terminal warning
     
+    # WIP
     def batch_checkout(self, files):
         """
         Checks out a collection of models from PDM Vault.
         """
         for file in files:
             self.checkout(filepath=file)
         
@@ -298,43 +312,33 @@
 
         # Execute PDM-API method
         if file.IsLocked:                           # if file is not checked in...
             file.UnlockFile(0, message)             # check in file
         else:
             print(f"File is already checked in!")   # ...else terminal warning
 
+    # WIP
     def batch_checkin(self, files, message: str="SolidWrap Automated Check In"):
         """
         Checks in a collection of models to PDM Vault.
         """
         for file in files:
             self.checkin(filepath=file)
 
+    # WIP
     def change_state(self, filepath: Filepath, state: str="WIP", message: str="SolidWrap Automated State Change"):
         """
         Changes model's PDM state to prescribed value, if allowed.
         """
         # print(f"Change State: {filepath.name}")
 
         # directory   = self.client.GetFolderFromPath(filepath.directory) # IEdmFolder5
         # folder_id   = directory.ID                                      # IEdmFolder5.ID (int?)
         # file        = directory.GetFile(filepath.name)                  # IEdmFile
         # file.ChangeState(state, folder_id, message, 0, 0)
 
-class Model:
-    """
-    Model
-    -----
-    Convenience wrapper for SolidWorks IModelDoc2 objects.
-    """
-    # Special Methods
-    # ---------------
-    def __init__(self, model):
-        self.filepath = Filepath(model.GetPathName) # Filepath
-        self.swobj = model                          # IModelDoc2
-
 
-# ---------------------
-# IV. Global Singletons
-# ---------------------
+# ---------------
+# III. Singletons
+# ---------------
 vault = Vault()
 solidworks = SolidWorks()
```

### Comparing `solidwrap-0.0.4/tests/test.py` & `solidwrap-1.0.0/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     # Export files
     for file in files:
         if model := solidworks.open(filepath=file):
             solidworks.export(model=model, as_type="png")
             solidworks.export(model=model, as_type="x_t")
             solidworks.close(model=model)
 
-# MAIN ENTRYPOINT
+# MAIN DEFINITION
 def main():
     if not solidworks.connect(version=2021):
         vault.connect('My_Vault')
         execute()
     input("\nPress any key to continue...")
     solidworks.disconnect()
 
-# TOP LEVEL SCRIPT ENTRYPOINT
+# TOP LEVEL ENTRYPOINT
 if __name__ == '__main__':
     main()
```

### Comparing `solidwrap-0.0.4/pyproject.toml` & `solidwrap-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "0.0.4"
+version = "1.0.0"
 authors = [
   { name="Sean Yeatts" },
 ]
-description = "This module wraps the SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
+license = {text = "MIT License"}
+description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "../README.rst"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
 ]
```

### Comparing `solidwrap-0.0.4/../README.rst` & `solidwrap-1.0.0/../README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 This module wraps the SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 
 Key Features
 ------------
 - Intuitive Pythonic syntax for interacting with SolidWorks models & PDM states.
-- Logging and report generation for profiling automation performance.
+- Logging and report generation for profiling automation performance. <-- ( under development )
 - Full API documentation detailing module components.
 
 Navigate to the `API Reference <https://github.com/SeanYeatts/SolidWrap/blob/main/solidwrap/info/API%20Reference.rst>`_ for a complete walkthrough of the module.
 
 Quickstart
 ----------
```

### Comparing `solidwrap-0.0.4/PKG-INFO` & `solidwrap-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: solidwrap
-Version: 0.0.4
-Summary: This module wraps the SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
+Version: 1.0.0
+Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/SeanYeatts/SolidWrap/tree/main
 Author: Sean Yeatts
+License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 
 SolidWrap
@@ -17,15 +18,15 @@
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 This module wraps the SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 
 Key Features
 ------------
 - Intuitive Pythonic syntax for interacting with SolidWorks models & PDM states.
-- Logging and report generation for profiling automation performance.
+- Logging and report generation for profiling automation performance. <-- ( under development )
 - Full API documentation detailing module components.
 
 Navigate to the `API Reference <https://github.com/SeanYeatts/SolidWrap/blob/main/solidwrap/info/API%20Reference.rst>`_ for a complete walkthrough of the module.
 
 Quickstart
 ----------
```

