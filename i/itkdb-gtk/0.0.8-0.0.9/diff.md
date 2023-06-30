# Comparing `tmp/itkdb_gtk-0.0.8.tar.gz` & `tmp/itkdb_gtk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.8.tar", last modified: Fri May 26 18:34:37 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.0.9.tar", last modified: Tue May 30 07:07:48 2023, max compression
```

## Comparing `itkdb_gtk-0.0.8.tar` & `itkdb_gtk-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-26 18:34:37.830705 itkdb_gtk-0.0.8/
--rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-26 18:34:37.830267 itkdb_gtk-0.0.8/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     2187 2023-05-24 15:05:26.000000 itkdb_gtk-0.0.8/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-26 18:34:37.827098 itkdb_gtk-0.0.8/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.8/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDB.desktop
--rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDB.svg
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14824 2023-05-25 13:27:59.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4693 2023-05-24 15:19:53.000000 itkdb_gtk-0.0.8/itkdb_gtk/ShowAttachments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2989 2023-05-24 13:13:04.000000 itkdb_gtk-0.0.8/itkdb_gtk/ShowComments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3329 2023-05-24 13:24:38.000000 itkdb_gtk-0.0.8/itkdb_gtk/ShowDefects.py
--rw-r--r--   0 lacasta    (503) staff       (20)      691 2023-05-26 18:34:32.000000 itkdb_gtk-0.0.8/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3731 2023-05-24 13:12:38.000000 itkdb_gtk-0.0.8/itkdb_gtk/checkComponent.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.8/itkdb_gtk/checkJSon.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4412 2023-05-25 15:33:11.000000 itkdb_gtk-0.0.8/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20713 2023-05-24 14:24:41.000000 itkdb_gtk-0.0.8/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.8/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7142 2023-05-24 13:24:49.000000 itkdb_gtk-0.0.8/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.8/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.8/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.8/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    19648 2023-05-26 18:33:54.000000 itkdb_gtk-0.0.8/itkdb_gtk/uploadMultipleTests.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    22252 2023-05-24 13:37:58.000000 itkdb_gtk-0.0.8/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    12154 2023-05-24 16:04:02.000000 itkdb_gtk-0.0.8/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-26 18:34:37.829700 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      767 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      291 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)     1141 2023-05-26 18:31:37.000000 itkdb_gtk-0.0.8/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-26 18:34:37.830832 itkdb_gtk-0.0.8/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-30 07:07:48.484977 itkdb_gtk-0.0.9/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-30 07:07:48.484562 itkdb_gtk-0.0.9/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     2187 2023-05-24 15:05:26.000000 itkdb_gtk-0.0.9/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-30 07:07:48.480496 itkdb_gtk-0.0.9/itkdb_gtk/
+-rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.9/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-05-30 06:57:54.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14824 2023-05-25 13:27:59.000000 itkdb_gtk-0.0.9/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4693 2023-05-24 15:19:53.000000 itkdb_gtk-0.0.9/itkdb_gtk/ShowAttachments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2989 2023-05-24 13:13:04.000000 itkdb_gtk-0.0.9/itkdb_gtk/ShowComments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3329 2023-05-24 13:24:38.000000 itkdb_gtk-0.0.9/itkdb_gtk/ShowDefects.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      691 2023-05-30 07:07:43.000000 itkdb_gtk-0.0.9/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3731 2023-05-24 13:12:38.000000 itkdb_gtk-0.0.9/itkdb_gtk/checkComponent.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.9/itkdb_gtk/checkJSon.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4412 2023-05-25 15:33:11.000000 itkdb_gtk-0.0.9/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20713 2023-05-24 14:24:41.000000 itkdb_gtk-0.0.9/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.9/itkdb_gtk/getShipments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7142 2023-05-24 13:24:49.000000 itkdb_gtk-0.0.9/itkdb_gtk/groundingTest.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    19379 2023-05-30 07:01:45.000000 itkdb_gtk-0.0.9/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.9/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.9/itkdb_gtk/sendShipments.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    19648 2023-05-26 18:33:54.000000 itkdb_gtk-0.0.9/itkdb_gtk/uploadMultipleTests.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    22252 2023-05-24 13:37:58.000000 itkdb_gtk-0.0.9/itkdb_gtk/uploadPetalInformation.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    12154 2023-05-24 16:04:02.000000 itkdb_gtk-0.0.9/itkdb_gtk/uploadTest.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-30 07:07:48.484099 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      767 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      291 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       56 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-30 07:07:48.000000 itkdb_gtk-0.0.9/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)     1130 2023-05-30 07:06:48.000000 itkdb_gtk-0.0.9/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-30 07:07:48.485070 itkdb_gtk-0.0.9/setup.cfg
```

### Comparing `itkdb_gtk-0.0.8/PKG-INFO` & `itkdb_gtk-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.8/README.md` & `itkdb_gtk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.0.9/itkdb_gtk/GlueWeight.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/ITkDB.svg` & `itkdb_gtk-0.0.9/itkdb_gtk/ITkDB.svg`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.0.9/itkdb_gtk/ITkDBlogin.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         """Create the window."""
         # set border width
         self.set_border_width(10)
 
         #
         self.has_window = True
         self.add_buttons(
-            Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL, Gtk.STOCK_OK, Gtk.ResponseType.OK
+            Gtk.STOCK_OK, Gtk.ResponseType.OK, Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL
         )
         # self.set_position(Gtk.WindowPosition.CENTER_ALWAYS)
 
         self.set_title("Login to the ITk DB")
 
         mainBox = Gtk.Box(orientation=Gtk.Orientation.VERTICAL)
         self.get_content_area().add(mainBox)
```

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.0.9/itkdb_gtk/ITkDButils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/ShowAttachments.py` & `itkdb_gtk-0.0.9/itkdb_gtk/ShowAttachments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/ShowComments.py` & `itkdb_gtk-0.0.9/itkdb_gtk/ShowComments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/ShowDefects.py` & `itkdb_gtk-0.0.9/itkdb_gtk/ShowDefects.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/__init__.py` & `itkdb_gtk-0.0.9/itkdb_gtk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import dashBoard
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 def dash_board():
     """Launches the dash board."""
     dashBoard.main()
```

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/checkComponent.py` & `itkdb_gtk-0.0.9/itkdb_gtk/checkComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/checkJSon.py` & `itkdb_gtk-0.0.9/itkdb_gtk/checkJSon.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.0.9/itkdb_gtk/dashBoard.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.0.9/itkdb_gtk/dbGtkUtils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.0.9/itkdb_gtk/getShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.0.9/itkdb_gtk/groundingTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.0.9/itkdb_gtk/readAVSdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 try:
     import ITkDBlogin
     import ITkDButils
 except ModuleNotFoundError:
     from itkdb_gtk import ITkDBlogin, ITkDButils
 
 import dateutil.parser
-import numpy as np
 import openpyxl as XL
 from openpyxl.cell.cell import MergedCell
 from openpyxl.utils.exceptions import InvalidFileException
 
 sk_defaults = {
     "institution": "AVS",
     "runNumber": "1",
@@ -504,15 +503,15 @@
     manufacturing["results"]["EPOXY_ADHESIVE"] = split_comp_list(sheet['c20'].value)
     manufacturing["results"]["EPOXY_PUTTY"] = split_comp_list(sheet['c21'].value)
     manufacturing["results"]["EPOXY_CONDUCTIVE"] = split_comp_list(sheet['c22'].value)
 
     # Weighing
     weighing = create_weight(session, SN, test_date, manager)
     comp_weight = [get_float(x[0]) for x in sheet['d12:d22']]
-    petal_weight = np.sum([float(x) for x in comp_weight])
+    petal_weight = sum([float(x) for x in comp_weight])
     weighing["results"]["WEIGHT_FACING_FRONT"] = comp_weight[0]
     weighing["results"]["WEIGHT_FACING_BACK"] = comp_weight[1]
     weighing["results"]["WEIGHT_LOCATOR_A"] = comp_weight[2]
     weighing["results"]["WEIGHT_LOCATOR_B"] = comp_weight[3]
     weighing["results"]["WEIGHT_LOCATOR_C"] = comp_weight[4]
     weighing["results"]["WEIGHT_COOLINGLOOPASSEMBLY"] = comp_weight[6]
     weighing["results"]["WEIGHT_HONEYCOMBSET"] = comp_weight[5]
```

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.0.9/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.0.9/itkdb_gtk/sendShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/uploadMultipleTests.py` & `itkdb_gtk-0.0.9/itkdb_gtk/uploadMultipleTests.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.0.9/itkdb_gtk/uploadPetalInformation.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.0.9/itkdb_gtk/uploadTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.0.9/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb-gtk
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.8/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.0.9/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.8/pyproject.toml` & `itkdb_gtk-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "itkdb>=0.4.0",
-  "numpy",
   "openpyxl",
   "pyserial",
   "python_dateutil",
   "requests"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

