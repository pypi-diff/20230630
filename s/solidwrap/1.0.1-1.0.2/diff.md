# Comparing `tmp/solidwrap-1.0.1.tar.gz` & `tmp/solidwrap-1.0.2.tar.gz`

## Comparing `solidwrap-1.0.1.tar` & `solidwrap-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 solidwrap-1.0.1/info/API Reference.rst
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 solidwrap-1.0.1/info/LICENSE
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 solidwrap-1.0.1/solidwrap/__init__.py
--rw-r--r--   0        0        0    13536 2020-02-02 00:00:00.000000 solidwrap-1.0.1/solidwrap/solidwrap.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 solidwrap-1.0.1/solidwrap/extensions/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 solidwrap-1.0.1/solidwrap/extensions/extensions.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.1/tests/test.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 solidwrap-1.0.1/../README.rst
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 solidwrap-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 solidwrap-1.0.2/info/API Reference.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/__init__.py
+-rw-r--r--   0        0        0    13857 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/extensions/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/extensions/extensions.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 solidwrap-1.0.2/solidwrap/profiling/profiling.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.2/tests/test.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 solidwrap-1.0.2/../README.rst
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 solidwrap-1.0.2/PKG-INFO
```

### Comparing `solidwrap-1.0.1/info/API Reference.rst` & `solidwrap-1.0.2/info/API Reference.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.1/solidwrap/solidwrap.py` & `solidwrap-1.0.2/solidwrap/solidwrap.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,28 @@
 
 # Standard imports
 import os                                   # manipulate folders
 import win32com.client  as win              # COM object handling
 import pythoncom        as pycom            # used in conjunction with win32com.client
 import subprocess       as subproc          # quick process disconnect
 
+# Project imports
+from .profiling        import profile       # function execution timing
+
 
 # ---------------------
 # II. Import Definition
 # ---------------------
 
 __all__ = [
     "solidworks",
     "vault",
     "Model",
-    "Filepath"
+    "Filepath",
+    "profile"
 ]
 
 
 # ------------
 # III. Classes
 # ------------
 
@@ -55,36 +59,39 @@
     # Attributes
     # ----------
     client  = None
     version = None
 
     # Pubic Methods
     # -------------
+    @profile
     def connect(self, version: int=2021, visible: bool=False):
         """
         Creates a connection to the SolidWorks process.
         """
         print(f"Connecting to SolidWorks client...")
 
         # Instantiate SolidWorks application via win32com dispatch (w/o concrete CLSID)
         self.version = version
         if not self.client:                                                                     # if a client is not defined...
             self.client = win.Dispatch("SldWorks.Application.%d" % (int(self.version)-1992))    # connect to new client  
             self.client.Visible = visible                                                       # make application visible
         else:                                                                                   # ...else terminal warning
             print(f"SolidWorks client connection is already established!")
 
+    @profile
     def disconnect(self):
         """
         Terminates connection to the SolidWorks process.
         """
         print(f"Terminating SolidWorks process...")
         subproc.call(f"Taskkill /IM SLDWORKS.exe /F")
         # No follow-up terminal message necessary; subproc.call() auto-responds
 
+    @profile
     def open(self, filepath: Filepath) -> Model:
         """
         Opens a model using the specified complete path.
         """
         print(f"Opening: {filepath.name}")
 
         # Define COM VARIANT arguments
@@ -101,69 +108,74 @@
         # Execute SW-API method - activate document
         # arg1 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 0)
         # self.client.ActivateDoc3(filepath.complete, False, 2, arg1)
 
         # Return Model
         return Model(raw_model)
     
+    @profile
     def safeclose(self, model: Model):
         """
         Closes the target model ( WITH rebuild and save methods ).
         """
         self.rebuild(model)
         self.save(model)
 
         print(f"Closing: {model.filepath.name}")
 
         # Execute SW-API method
         self.client.CloseDoc(model.filepath.complete)
 
+    @profile
     def close(self, model: Model):
         """
         Closes the target model ( WITHOUT rebuild and save methods ).
         """
         print(f"Closing: {model.filepath.name}")
 
         # Execute SW-API method
         self.client.CloseDoc(model.filepath.complete)
 
+    @profile
     def save(self, model: Model):
         """
         Saves the target model.
         """
         print(f"Saving: {model.filepath.name}")
 
         # Define COM VARIANT arguments
         options     = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 1)
         errors      = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 1)
         warnings    = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 1)
 
         # Execute SW-API method
         model.swobj.Save3(options, errors, warnings)
 
+    @profile
     def rebuild(self, model: Model):
         """
         Rebuilds the target model.
         """
         print(f"Rebuilding: {model.filepath.name}")
         
         # Define COM VARIANT arguments
         arg1 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, False)
 
         # Execute SW-API method
         model.swobj.ForceRebuild3(arg1)
 
+    @profile
     def export(self, model: Model, as_type: str="PNG"):
         """
         Exports the target model as the prescribed file type.
         """
         # Format components
         extension   = str("." + as_type)
         desktop     = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
-        destination = str(desktop + fr"\Exports")
+        destination = str(desktop + fr"\SolidWrap Exports")
         file        = Filepath(f"{destination}\{model.filepath.root}{extension}")
 
         # Make export directory
         if not os.path.exists(destination):
             os.makedirs(destination)
 
         print(f"Exporting: {file.name}")
@@ -175,14 +187,15 @@
         arg2 = win.VARIANT(pycom.VT_BOOL, 0) 
         arg3 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 0)
         arg4 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 0)
 
         # Execute SW-API method
         model.swobj.Extension.SaveAs2(file.complete, 0, 1, arg1, "", arg2, arg3, arg4)
 
+    @profile
     def freeze(self, model: Model):
         """
         Freezes the target model's feature tree.
         """
         print(f"Freezing: {model.filepath.name}")
 
         # Define COM VARIANT arguments
@@ -196,26 +209,28 @@
 
         # Define COM VARIANT arguments
         position = win.VARIANT(pycom.VT_I4, 3)
 
         # Execute SW-API method - move freeze bar to end of feature tree
         model.swobj.FeatureManager.EditFreeze(position, feature.Name, True)
 
+    @profile
     def declutter(self, model: Model, declutter: bool=True):
         """
         Hides/Shows all of the target model's sketches, reference geometry, etc.
         """
         print(f"Decluttering: {model.filepath.name}")
 
         # Define COM VARIANT arguments
         setting = win.VARIANT(pycom.VT_I4, 198) # swUserPreferenceToggle_e.swViewDisplayHideAllTypes
         
         # Execute SW-API Method: SetUserPreferenceToggle - hide all types (planes, sketches, etc.)
         model.swobj.Extension.SetUserPreferenceToggle(setting, 0, declutter)
         
+    @profile
     def stage(self, model: Model):
         """
         Decultters viewport and orients an isometric model view.
         """
         print(f"Staging: {model.filepath.name}")
         self.declutter(model=model)
 
@@ -239,39 +254,42 @@
     # ----------
     client      = None  # win32com application
     name        = None  # PDM Vault name (ex. "Goddard_Vault")
     auth_state  = False # login credential authorization flag
 
     # Public Methods
     # --------------
+    @profile
     def connect(self, name: str="Goddard_Vault"):
         """
         Creates a connection to the PDM Vault.
         """
         print(f"Connecting to PDM...")
 
         # Instantiate PDM Vault via win32com dispatch (w/o concrete CLSID)
         self.name = name
         if not self.client:                                     # if a client is not defined...
             self.client = win.Dispatch("ConisioLib.EdmVault")   # connect to client
         else:                                                   # ...else terminal warning
             print(f"PDM connection is already established!")
         self.authenticate()
 
+    @profile
     def authenticate(self):
         """
         Authenticates login credentials for PDM Vault.
         """
         print(f"Authentiating PDM credentials...")
 
         # Attempt login & flag authentication state
         if not self.client.IsLoggedIn:
             self.client.LoginAuto(self.name, 0)
             self.auth_state = True
 
+    @profile
     def checkout(self, filepath: Filepath):
         """
         Checks out model from PDM Vault.
         """
         print(f"Check Out: {filepath.name}")
 
         # Get PDM-API objects
@@ -281,14 +299,15 @@
         # Execute PDM-API method
         if not file.IsLocked:                       # if file is not checked out...
             file.LockFile(directory.ID, 0)          # check out file
         else:
             print(f"File is already checked out!")  # ...else terminal warning
     
     # WIP
+    @profile
     def batch_checkout(self, files):
         """
         Checks out a collection of models from PDM Vault.
         """
         for file in files:
             self.checkout(filepath=file)
         
@@ -308,14 +327,15 @@
         #     # utility.AddFile(file_id, folder_id)
         #     utility.AddSelectionEx(vault.client, file_id, folder_id, item.CurrentVersion)
         
         # utility.CreateTree(0, 2)    # @param2 (2) Egcf_Lock
         # # utility.GetFiles()
         # print(f"{utility.FileCount}")
 
+    @profile
     def checkin(self, filepath: Filepath, message: str="SolidWrap Automated Check In"):
         """
         Checks in model to PDM Vault.
         """
         print(f"Check In: {filepath.name}")
 
         # Get PDM-API objects
@@ -325,22 +345,24 @@
         # Execute PDM-API method
         if file.IsLocked:                           # if file is not checked in...
             file.UnlockFile(0, message)             # check in file
         else:
             print(f"File is already checked in!")   # ...else terminal warning
 
     # WIP
+    @profile
     def batch_checkin(self, files, message: str="SolidWrap Automated Check In"):
         """
         Checks in a collection of models to PDM Vault.
         """
         for file in files:
             self.checkin(filepath=file)
 
     # WIP
+    @profile
     def change_state(self, filepath: Filepath, state: str="WIP", message: str="SolidWrap Automated State Change"):
         """
         Changes model's PDM state to prescribed value, if allowed.
         """
         # print(f"Change State: {filepath.name}")
 
         # directory   = self.client.GetFolderFromPath(filepath.directory) # IEdmFolder5
@@ -373,9 +395,8 @@
     tree = manager.GetFeatureTreeRootItem2(0)
 
     # Iterate through tree to get last item (yes, it has to be done this way)
     feature = tree.GetFirstChild
     for item in range(count):           # for each feature...
         if feature.GetNext:             # if valid item...
             feature = feature.GetNext   # ...then get item
-    print(f"Last Feature: {feature.Object.Name}")
     return feature.Object               # return the feature
```

### Comparing `solidwrap-1.0.1/tests/test.py` & `solidwrap-1.0.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.1/pyproject.toml` & `solidwrap-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Sean Yeatts" },
 ]
 license = {text = "MIT License"}
 description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "../README.rst"
 requires-python = ">=3.7"
```

### Comparing `solidwrap-1.0.1/../README.rst` & `solidwrap-1.0.2/../README.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.1/PKG-INFO` & `solidwrap-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidwrap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/users/SeanYeatts/projects/6/views/1
 Author: Sean Yeatts
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

