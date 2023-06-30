# Comparing `tmp/panelapp-0.7.3.tar.gz` & `tmp/panelapp-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/panelapp-0.7.3.tar", last modified: Fri Dec 18 14:45:40 2020, max compression
+gzip compressed data, was "panelapp-0.7.4.tar", last modified: Fri Jun 30 13:30:28 2023, max compression
```

## Comparing `panelapp-0.7.3.tar` & `panelapp-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2020-12-18 14:45:40.000000 panelapp-0.7.3/
-drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2020-12-18 14:45:40.000000 panelapp-0.7.3/panelapp.egg-info/
--rw-rw-r--   0 kimy      (1000) kimy      (1000)       18 2020-12-18 14:45:39.000000 panelapp-0.7.3/panelapp.egg-info/top_level.txt
--rw-rw-r--   0 kimy      (1000) kimy      (1000)      224 2020-12-18 14:45:39.000000 panelapp-0.7.3/panelapp.egg-info/SOURCES.txt
--rw-rw-r--   0 kimy      (1000) kimy      (1000)        1 2020-12-18 14:45:39.000000 panelapp-0.7.3/panelapp.egg-info/dependency_links.txt
--rw-rw-r--   0 kimy      (1000) kimy      (1000)     2882 2020-12-18 14:45:39.000000 panelapp-0.7.3/panelapp.egg-info/PKG-INFO
--rw-rw-r--   0 kimy      (1000) kimy      (1000)     2094 2020-12-15 14:40:25.000000 panelapp-0.7.3/README.md
--rw-rw-r--   0 kimy      (1000) kimy      (1000)       38 2020-12-18 14:45:40.000000 panelapp-0.7.3/setup.cfg
--rw-rw-r--   0 kimy      (1000) kimy      (1000)      670 2020-12-18 13:24:19.000000 panelapp-0.7.3/setup.py
-drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2020-12-18 14:45:40.000000 panelapp-0.7.3/panelapp/
--rw-rw-r--   0 kimy      (1000) kimy      (1000)     2478 2020-11-12 16:31:45.000000 panelapp-0.7.3/panelapp/api.py
--rw-rw-r--   0 kimy      (1000) kimy      (1000)        0 2020-10-21 16:06:54.000000 panelapp-0.7.3/panelapp/__init__.py
--rw-rw-r--   0 kimy      (1000) kimy      (1000)    15499 2020-12-18 13:24:05.000000 panelapp-0.7.3/panelapp/Panelapp.py
--rw-rw-r--   0 kimy      (1000) kimy      (1000)     2160 2020-12-15 14:40:25.000000 panelapp-0.7.3/panelapp/queries.py
--rw-rw-r--   0 kimy      (1000) kimy      (1000)     2882 2020-12-18 14:45:40.000000 panelapp-0.7.3/PKG-INFO
+drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2023-06-30 13:30:28.376475 panelapp-0.7.4/
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)     2949 2023-06-30 13:30:28.372475 panelapp-0.7.4/PKG-INFO
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)     2161 2023-06-30 13:25:26.000000 panelapp-0.7.4/README.md
+drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2023-06-30 13:30:28.372475 panelapp-0.7.4/panelapp/
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)    15499 2023-06-30 13:25:24.000000 panelapp-0.7.4/panelapp/Panelapp.py
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)        0 2022-03-23 10:02:01.000000 panelapp-0.7.4/panelapp/__init__.py
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)     2478 2022-03-23 10:02:01.000000 panelapp-0.7.4/panelapp/api.py
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)     2195 2023-06-30 13:25:26.000000 panelapp-0.7.4/panelapp/queries.py
+drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2023-06-30 13:30:28.372475 panelapp-0.7.4/panelapp.egg-info/
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)     2949 2023-06-30 13:30:28.000000 panelapp-0.7.4/panelapp.egg-info/PKG-INFO
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)      264 2023-06-30 13:30:28.000000 panelapp-0.7.4/panelapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)        1 2023-06-30 13:30:28.000000 panelapp-0.7.4/panelapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)       24 2023-06-30 13:30:28.000000 panelapp-0.7.4/panelapp.egg-info/top_level.txt
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)       38 2023-06-30 13:30:28.376475 panelapp-0.7.4/setup.cfg
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)      670 2023-06-30 13:26:13.000000 panelapp-0.7.4/setup.py
+drwxrwxr-x   0 kimy      (1000) kimy      (1000)        0 2023-06-30 13:30:28.372475 panelapp-0.7.4/tests/
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)        1 2023-06-30 13:25:26.000000 panelapp-0.7.4/tests/__init__.py
+-rw-rw-r--   0 kimy      (1000) kimy      (1000)     2556 2023-06-30 13:25:26.000000 panelapp-0.7.4/tests/test_queries.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `panelapp-0.7.3/panelapp.egg-info/PKG-INFO` & `panelapp-0.7.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panelapp
-Version: 0.7.3
+Version: 0.7.4
 Summary: General purpose Panelapp package
 Home-page: https://github.com/NHS-NGS/panelapp
 Author: Yujin Kim
 Author-email: yujin.kim@hotmail.fr
 License: UNKNOWN
 Description: # panelapp
         
@@ -40,15 +40,15 @@
         panel.is_signedoff()               # Return date of signedoff or False if not signedoff
         panel.get_data()                   # Return all the data the API sent, you can use that there's something that is lacking in my methods
         panel.write()                      # Write a file for the panel containing the most important data (according to me at least, you can customize this yourself using the .get_data() method)
         
         from panelapp import queries
         
         panels = queries.get_all_panels()                                         # Return dict {panel_id: Panelapp.Panel} of all panels in Panelapp
-        signedoff_panels = queries.get_all_signedoff_panels()                     # Return dict {panel_id: Panelapp.Panel} of signedoff panels
+        signedoff_panels = queries.get_all_signedoff_panels()                     # Return dict {panel_id: Panelapp.Panel} of signedoff panels. Note that this only returns the latest versions on public panels.
         matches, differences = queries.compare_versions(Panelapp.Panel, "2.7")    # Return tuple of match and differences between the given panel and another panel version
         panel = queries.get_signedoff_panel(269)                                  # Return panel object with latest signedoff version
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panelapp-0.7.3/README.md` & `panelapp-0.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,11 +32,11 @@
 panel.is_signedoff()               # Return date of signedoff or False if not signedoff
 panel.get_data()                   # Return all the data the API sent, you can use that there's something that is lacking in my methods
 panel.write()                      # Write a file for the panel containing the most important data (according to me at least, you can customize this yourself using the .get_data() method)
 
 from panelapp import queries
 
 panels = queries.get_all_panels()                                         # Return dict {panel_id: Panelapp.Panel} of all panels in Panelapp
-signedoff_panels = queries.get_all_signedoff_panels()                     # Return dict {panel_id: Panelapp.Panel} of signedoff panels
+signedoff_panels = queries.get_all_signedoff_panels()                     # Return dict {panel_id: Panelapp.Panel} of signedoff panels. Note that this only returns the latest versions on public panels.
 matches, differences = queries.compare_versions(Panelapp.Panel, "2.7")    # Return tuple of match and differences between the given panel and another panel version
 panel = queries.get_signedoff_panel(269)                                  # Return panel object with latest signedoff version
 ```
```

### Comparing `panelapp-0.7.3/setup.py` & `panelapp-0.7.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="panelapp",
-    version="0.7.3",
+    version="0.7.4",
     author="Yujin Kim",
     author_email="yujin.kim@hotmail.fr",
     description="General purpose Panelapp package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NHS-NGS/panelapp",
     packages=setuptools.find_packages(),
```

### Comparing `panelapp-0.7.3/panelapp/api.py` & `panelapp-0.7.4/panelapp/api.py`

 * *Files identical despite different names*

### Comparing `panelapp-0.7.3/panelapp/Panelapp.py` & `panelapp-0.7.4/panelapp/Panelapp.py`

 * *Files identical despite different names*

### Comparing `panelapp-0.7.3/panelapp/queries.py` & `panelapp-0.7.4/panelapp/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,25 +50,25 @@
     matches = set(original_genes).intersection(set(compare_genes))
     difference = set(original_genes).symmetric_difference(set(compare_genes))
 
     return (matches, difference)
 
 
 def get_signedoff_panel(panel_id: str):
-    """ Return data of signedoff panel
+    """ Return data for the latest version of a signedoff panel
 
     Args:
         panel_id (str): Panel id
 
     Returns:
         dict: Data of the panel
     """
 
     signedoff_panel = get_panelapp_response(
-        ext_url="panels/signedoff/{}".format(panel_id)
+        ext_url="panels/signedoff/?panel_id={}".format(panel_id)
     )
     return signedoff_panel
 
 
 def get_all_panels():
     """ Returns all panels
```

### Comparing `panelapp-0.7.3/PKG-INFO` & `panelapp-0.7.4/panelapp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panelapp
-Version: 0.7.3
+Version: 0.7.4
 Summary: General purpose Panelapp package
 Home-page: https://github.com/NHS-NGS/panelapp
 Author: Yujin Kim
 Author-email: yujin.kim@hotmail.fr
 License: UNKNOWN
 Description: # panelapp
         
@@ -40,15 +40,15 @@
         panel.is_signedoff()               # Return date of signedoff or False if not signedoff
         panel.get_data()                   # Return all the data the API sent, you can use that there's something that is lacking in my methods
         panel.write()                      # Write a file for the panel containing the most important data (according to me at least, you can customize this yourself using the .get_data() method)
         
         from panelapp import queries
         
         panels = queries.get_all_panels()                                         # Return dict {panel_id: Panelapp.Panel} of all panels in Panelapp
-        signedoff_panels = queries.get_all_signedoff_panels()                     # Return dict {panel_id: Panelapp.Panel} of signedoff panels
+        signedoff_panels = queries.get_all_signedoff_panels()                     # Return dict {panel_id: Panelapp.Panel} of signedoff panels. Note that this only returns the latest versions on public panels.
         matches, differences = queries.compare_versions(Panelapp.Panel, "2.7")    # Return tuple of match and differences between the given panel and another panel version
         panel = queries.get_signedoff_panel(269)                                  # Return panel object with latest signedoff version
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

