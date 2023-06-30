# Comparing `tmp/lasfile-0.1.8.tar.gz` & `tmp/lasfile-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasfile-0.1.8.tar", last modified: Thu Jun  1 20:26:59 2023, max compression
+gzip compressed data, was "lasfile-0.1.9.tar", last modified: Fri Jun  2 15:00:45 2023, max compression
```

## Comparing `lasfile-0.1.8.tar` & `lasfile-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:26:59.358343 lasfile-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 20:26:45.000000 lasfile-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 20:26:45.000000 lasfile-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-01 20:26:59.358343 lasfile-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 20:26:45.000000 lasfile-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 20:26:45.000000 lasfile-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:26:59.358343 lasfile-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:26:59.354343 lasfile-0.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:26:45.000000 lasfile-0.1.8/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:26:59.354343 lasfile-0.1.8/src/lasfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-01 20:26:59.000000 lasfile-0.1.8/src/lasfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 20:26:59.000000 lasfile-0.1.8/src/lasfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:26:59.000000 lasfile-0.1.8/src/lasfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 20:26:59.000000 lasfile-0.1.8/src/lasfile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 20:26:59.000000 lasfile-0.1.8/src/lasfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 20:26:59.000000 lasfile-0.1.8/src/lasfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    61680 2023-06-01 20:26:45.000000 lasfile-0.1.8/src/lasfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:26:59.354343 lasfile-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-01 20:26:45.000000 lasfile-0.1.8/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:00:45.408222 lasfile-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-02 15:00:35.000000 lasfile-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 15:00:35.000000 lasfile-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-02 15:00:45.408222 lasfile-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-02 15:00:35.000000 lasfile-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-02 15:00:35.000000 lasfile-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:00:45.408222 lasfile-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:00:45.404222 lasfile-0.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:00:35.000000 lasfile-0.1.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:00:45.408222 lasfile-0.1.9/src/lasfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-02 15:00:45.000000 lasfile-0.1.9/src/lasfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-02 15:00:45.000000 lasfile-0.1.9/src/lasfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:00:45.000000 lasfile-0.1.9/src/lasfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 15:00:45.000000 lasfile-0.1.9/src/lasfile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 15:00:45.000000 lasfile-0.1.9/src/lasfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 15:00:45.000000 lasfile-0.1.9/src/lasfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67203 2023-06-02 15:00:35.000000 lasfile-0.1.9/src/lasfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:00:45.408222 lasfile-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-02 15:00:35.000000 lasfile-0.1.9/tests/tests.py
```

### Comparing `lasfile-0.1.8/LICENSE` & `lasfile-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.8/PKG-INFO` & `lasfile-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lasfile
  Library for reading CWLS Log ASCII Standard v. 1.2, 2.0, and 3.0 .las files.
 
 ## Installation
```

### Comparing `lasfile-0.1.8/README.md` & `lasfile-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lasfile-0.1.8/src/lasfile.egg-info/PKG-INFO` & `lasfile-0.1.9/src/lasfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lasfile
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python library for reading LAS files.
 Project-URL: homepage, https://github.com/bzlmnop/lasfile
 Keywords: las,CWLS,las logs,petrophysical logs
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lasfile
  Library for reading CWLS Log ASCII Standard v. 1.2, 2.0, and 3.0 .las files.
 
 ## Installation
```

### Comparing `lasfile-0.1.8/src/lasfile.py` & `lasfile-0.1.9/src/lasfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,463 +1,563 @@
 # A python module for reading LAS files
 
 import re
 import traceback
 from io import StringIO
 from numpy import genfromtxt
 from pandas import DataFrame
-import json
-from os import path
-from pkgutil import get_data
-
+import warnings
 
 # Set known versions
-known_versions = ['1.2','2.0','3.0']
+known_versions = ['1.2', '2.0', '3.0']
 # Set known sections
-known_sections = {
+known_secs = {
     "1.2":
     {
         "version":
         {
-            "type":"header",
-            "titles":["v","V"]
+            "type": "header",
+            "titles": ["v", "V"]
         },
         "well":
         {
-            "type":"header",
-            "titles":["w","W"]
+            "type": "header",
+            "titles": ["w", "W"]
         },
         "parameters":
         {
-            "type":"header",
-            "titles":["p","P"]
+            "type": "header",
+            "titles": ["p", "P"]
         },
         "curves":
         {
-            "type":"header",
-            "titles":["c","C"]
+            "type": "header",
+            "titles": ["c", "C"]
         },
         "data":
         {
-            "type":"data",
-            "titles":["a","A"]
+            "type": "data",
+            "titles": ["a", "A"]
         },
         "other":
         {
-            "type":"header",
-            "titles":["o","O"]
+            "type": "header",
+            "titles": ["o", "O"]
         }
     },
     "2.0":
     {
         "version":
         {
-            "type":"header",
-            "titles":["v","V"]
+            "type": "header",
+            "titles": ["v", "V"]
         },
         "well":
         {
-            "type":"header",
-            "titles":["w","W"]
+            "type": "header",
+            "titles": ["w", "W"]
         },
         "parameters":
         {
-            "type":"header",
-            "titles":["p","P"]
+            "type": "header",
+            "titles": ["p", "P"]
         },
         "curves":
         {
-            "type":"header",
-            "titles":["c","C"]
+            "type": "header",
+            "titles": ["c", "C"]
         },
         "data":
         {
-            "type":"data",
-            "titles":["a","A"]
+            "type": "data",
+            "titles": ["a", "A"]
         },
         "other":
         {
-            "type":"header",
-            "titles":["o","O"]
+            "type": "header",
+            "titles": ["o", "O"]
         }
     },
     "3.0":
     {
         "version":
         {
             "type": "header",
-            "titles":["version"]
+            "titles": ["version"]
         },
         "well":
         {
             "type": "header",
             "titles": ["well"]
         },
         "parameters":
         {
             "type": "header",
-            "titles":["parameter","log_parameter"]
+            "titles": ["parameter", "log_parameter"]
         },
         "curves":
         {
             "type": "header",
-            "titles":["curves","curve","curve_definition","log_definition"]
+            "titles": ["curves", "curve", "curve_definition", "log_definition"]
         },
         "data":
         {
             "type": "data",
-            "titles":["log_data","ascii","data"]
+            "titles": ["log_data", "ascii", "data"]
         },
         "core_parameters":
         {
             "type": "header",
-            "titles":["core_parameters"]
+            "titles": ["core_parameters"]
         },
         "core_definition":
         {
             "type": "header",
-            "titles":["core_definition"]
+            "titles": ["core_definition"]
         },
         "core_data":
         {
             "type": "data",
-            "titles":["core_data"]
+            "titles": ["core_data"]
         },
         "inclinometry_parameters":
         {
             "type": "header",
-            "titles":["inclinometry_parameters"]
+            "titles": ["inclinometry_parameters"]
         },
         "inclinometry_definition":
         {
             "type": "header",
-            "titles":["inclinometry_definition"]
+            "titles": ["inclinometry_definition"]
         },
         "inclinometry_data":
         {
             "type": "data",
-            "titles":["inclinometry_data"]
+            "titles": ["inclinometry_data"]
         },
         "drill_parameters":
         {
             "type": "header",
-            "titles":["drill_parameters"]
+            "titles": ["drill_parameters"]
         },
         "drill_definition":
         {
             "type": "header",
-            "titles":["drill_definition"]
+            "titles": ["drill_definition"]
         },
         "drill_data":
         {
             "type": "data",
-            "titles":["drill_data"]
+            "titles": ["drill_data"]
         },
         "tops_parameters":
         {
             "type": "header",
-            "titles":["tops_parameters"]
+            "titles": ["tops_parameters"]
         },
         "tops_definition":
         {
             "type": "header",
-            "titles":["tops_definition"]
+            "titles": ["tops_definition"]
         },
         "tops_data":
         {
             "type": "data",
-            "titles":["tops_data"]
+            "titles": ["tops_data"]
         },
         "test_parameters":
         {
             "type": "header",
-            "titles":["test_parameters"]
+            "titles": ["test_parameters"]
         },
         "test_definition":
         {
             "type": "header",
-            "titles":["test_definition"]
+            "titles": ["test_definition"]
         },
         "test_data":
         {
             "type": "data",
-            "titles":["test_data"]
+            "titles": ["test_data"]
         }
     }
 }
 
-def get_version_num(
-        data,
-        handle_common_errors=True,
-        accept_unknown_versions=False,
-        allow_non_numeric=False,
-        unknown_value=None
-    ):
+
+def get_version_num(data,
+                    handle_common_errors=True,
+                    accept_unknown_versions=False,
+                    allow_non_numeric=False,
+                    unknown_value=None):
     """
     Extracts and validates the version number from the given data.
 
-    This function accepts either a string containing a version section, 
-    or a DataFrame containing a mnemonic column with a "VERS" value. 
-    It then tries to extract the version number and validate it. 
-    It handles several common errors, such as non-numeric versions, and 
-    allows the acceptance of unknown versions. 
+    This function accepts either a string containing a version section,
+    or a DataFrame containing a mnemonic column with a "VERS" value.
+    It then tries to extract the version number and validate it.
+    It handles several common errors, such as non-numeric versions, and
+    allows the acceptance of unknown versions.
 
     Parameters:
     ----------
     data : str or pandas.DataFrame
-        The input data to extract the version number from. 
-        If a string, it should contain a version section marked with '~V'. 
-        If a DataFrame, it should contain a column named 'mnemonic' with a 
+        The input data to extract the version number from.
+        If a string, it should contain a version section marked with '~V'.
+        If a DataFrame, it should contain a column named 'mnemonic' with a
         "VERS" value.
 
     handle_common_errors : bool, optional
-        Whether to handle common errors, such as whole number versions. 
+        Whether to handle common errors, such as whole number versions.
         (default is True)
 
     accept_unknown_versions : bool, optional
         Whether to accept and return unknown versions. (default is False)
 
     allow_non_numeric : bool, optional
-        Whether to allow and return non-numeric versions. This only works 
+        Whether to allow and return non-numeric versions. This only works
         if `accept_unknown_versions` is also True. (default is False)
 
     Returns:
     -------
     version_num : str
         The extracted version number.
 
     Raises:
     ------
     ValueError:
         If the input data is neither a string nor a DataFrame.
 
     Exception:
-        If the version number could not be retrieved, or if it 
+        If the version number could not be retrieved, or if it
         was not recognized and `accept_unknown_versions` is False.
     """
-    if type(data) == str:
+    # Parse input data based on its type
+    if isinstance(data, str):
         section_regex = re.compile(r'(~[V].+?)(?=~[VW]|$)', re.DOTALL)
-        section_list = re.findall(section_regex, data)
-        #print(f"section_list: {section_list}")
-        version_section = section_list[0]
-        #print(f"version_section: {version_section}")
+        version_section = re.findall(section_regex, data)[0]
         df = parse_header_section(version_section)
-        #print(f"parsed_section: {results}")
-        try:
-            version_num = df.loc[df['mnemonic']=="VERS","value"].values[0]
-        except Exception as e:
-            raise Exception(f"couldnt get version: {str(e)}")
-    elif type(data) == DataFrame:
+    elif isinstance(data, DataFrame):
         df = data
-        try:
-            version_num = df.loc[df['mnemonic']=="VERS","value"].values[0]
-        except Exception as e:
-            raise Exception(f"Couldnt get version: {str(e)}")
     else:
         raise ValueError("Input must be str or DataFrame.")
+
+    # Try to extract version number
+    try:
+        version_num = df.loc[df['mnemonic'] == "VERS", "value"].values[0]
+    except Exception as e:
+        raise Exception(f"Could not get version: {str(e)}")
+
+    # Check if version number is known
     if version_num in known_versions:
         return version_num
-    else:
-        if handle_common_errors:
-            # Try to convert to float
-            try:
-                float_version_num = str(float(version_num))
-                # Handle whole number version values
-                if str(float_version_num) in known_versions:
-                    version_num = str(float(version_num))
-                    return version_num
-                # Handle float version values with trailing zeros
-                elif float_version_num in known_versions:
-                    version_num = float_version_num
-                    return version_num
-            except:
-                pass
-        elif accept_unknown_versions:
-            try:
-                # Verify it is an integer and return it
-                float_version_num = float(version_num)
+
+    # Handle common errors like conversion to float
+    if handle_common_errors:
+        try:
+            float_version_num = str(float(version_num))
+            if float_version_num in known_versions:
+                return float_version_num
+        except ValueError:
+            pass
+
+    # Accept unknown versions, verify if they are integers
+    if accept_unknown_versions:
+        try:
+            float(version_num)
+            return version_num
+        except ValueError:
+            if allow_non_numeric:
                 return version_num
-            except:
-                if allow_non_numeric:
-                    return version_num
-        else:
-            raise Exception(
-                f"Couldnt get version, version number not recognized."
-            )
 
-def get_version_section(
-        data,
-        handle_common_errors=True,
-        accept_unknown_versions=False,
-        allow_non_numeric=False,
-        unknown_value=None
-    ):
+    raise Exception("Could not get version, version number not recognized.")
+
+
+# def get_version_section(
+#         data,
+#         handle_common_errors=True,
+#         accept_unknown_versions=False,
+#         allow_non_numeric=False,
+#         unknown_value=None
+#     ):
+#     """
+#     Extracts the version section from the given raw data, parses it,
+#     validates it, and returns a loaded section object.
+
+#     This function performs several steps to process the version section
+#     from the raw data. It extracts the version section, parses it into
+#     a DataFrame, attempts to extract and validate a version number, and
+#     then tries to load this all into a LASSection object.
+
+#     Parameters:
+#     ----------
+#     data : str
+#         The raw data string to extract the version section from. The
+#         version section should be marked with '~V'.
+
+#     handle_common_errors : bool, optional
+#         Whether to handle common errors when extracting the
+#         version number. (default is True)
+
+#     accept_unknown_versions : bool, optional
+#         Whether to accept unknown versions when extracting the version
+#         number. (default is False)
+
+#     allow_non_numeric : bool, optional
+#         Whether to allow non-numeric versions when extracting the
+#         version number. (default is False)
+
+#     unknown_value : any, optional
+#         The value to use when an unknown version number is encountered.
+#         This only applies if `accept_unknown_versions`
+#         is also True. (default is None)
+
+#     Returns:
+#     -------
+#     loaded_section : LASSection
+#         The loaded version section.
+
+#     Raises:
+#     ------
+#     Exception:
+#         If parsing the version section fails, if extracting the
+#         version number fails, if validating the version section fails,
+#         or if loading the section into a LASSection object fails.
+#     """
+#     # Extract version section from raw data
+#     section_regex = re.compile(r'(~[V].+?)(?=~[VW]|$)', re.DOTALL)
+#     section_list = re.findall(section_regex, data)
+#     version_section = section_list[0]
+#     # Parse version section
+#     try:
+#         df = parse_header_section(version_section)
+#     except:
+#         raise Exception("Failed to parse version section.")
+#     # Attempt to extract a version number from the parsed section
+#     try:
+#         version_num = get_version_num(
+#             df,
+#             handle_common_errors=handle_common_errors,
+#             accept_unknown_versions=accept_unknown_versions,
+#             allow_non_numeric=allow_non_numeric,
+#             unknown_value=unknown_value
+#         )
+#     except Exception as e:
+#         raise e
+#     # Attempt to validate the section
+#     if validate_version(df,version_num=version_num):
+#         try:
+#             wrap_val = df.loc[df['mnemonic']=="WRAP","value"].values[0]
+#         except Exception as e:
+#             raise Exception(f"couldnt get wrap: {str(e)}")
+#         if version_num == "3.0":
+#             try:
+#                 dlm_val = df.loc[df['mnemonic']=="DLM","value"].values[0]
+#             except Exception as e:
+#                 raise Exception(f"couldnt get version: {str(e)}")
+#         else:
+#             dlm_val = None
+#         # Attempt to load the section into a section object
+#         try:
+#             loaded_section = LASSection(
+#                 'version',
+#                 version_section,
+#                 'header',
+#                 version_num,
+#                 delimiter=dlm_val,
+#                 parse_on_init=False,
+#                 validate_on_init=False
+#             )
+#             loaded_section.df = df
+#             loaded_section.validated = True
+#             loaded_section.version_num = version_num
+#             return loaded_section
+#         except:
+#             raise Exception("Couldn't load into section object.")
+#     else:
+#         raise Exception("Coulnt validate version section.")
+
+
+def get_version_section(data,
+                        handle_common_errors=True,
+                        accept_unknown_versions=False,
+                        allow_non_numeric=False,
+                        unknown_value=None):
     """
-    Extracts the version section from the given raw data, parses it, 
+    Extracts the version section from the given raw data, parses it,
     validates it, and returns a loaded section object.
 
-    This function performs several steps to process the version section 
-    from the raw data. It extracts the version section, parses it into 
-    a DataFrame, attempts to extract and validate a version number, and 
+    This function performs several steps to process the version section
+    from the raw data. It extracts the version section, parses it into
+    a DataFrame, attempts to extract and validate a version number, and
     then tries to load this all into a LASSection object.
 
     Parameters:
     ----------
     data : str
-        The raw data string to extract the version section from. The 
-        version section should be marked with '~V'. 
+        The raw data string to extract the version section from. The
+        version section should be marked with '~V'.
 
     handle_common_errors : bool, optional
-        Whether to handle common errors when extracting the 
+        Whether to handle common errors when extracting the
         version number. (default is True)
 
     accept_unknown_versions : bool, optional
-        Whether to accept unknown versions when extracting the version 
+        Whether to accept unknown versions when extracting the version
         number. (default is False)
 
     allow_non_numeric : bool, optional
-        Whether to allow non-numeric versions when extracting the 
+        Whether to allow non-numeric versions when extracting the
         version number. (default is False)
 
     unknown_value : any, optional
-        The value to use when an unknown version number is encountered. 
-        This only applies if `accept_unknown_versions` 
+        The value to use when an unknown version number is encountered.
+        This only applies if `accept_unknown_versions`
         is also True. (default is None)
 
     Returns:
     -------
     loaded_section : LASSection
         The loaded version section.
 
     Raises:
     ------
     Exception:
-        If parsing the version section fails, if extracting the 
-        version number fails, if validating the version section fails, 
+        If parsing the version section fails, if extracting the
+        version number fails, if validating the version section fails,
         or if loading the section into a LASSection object fails.
     """
     # Extract version section from raw data
     section_regex = re.compile(r'(~[V].+?)(?=~[VW]|$)', re.DOTALL)
     section_list = re.findall(section_regex, data)
     version_section = section_list[0]
+
     # Parse version section
     try:
         df = parse_header_section(version_section)
-    except:
+    except Exception:
         raise Exception("Failed to parse version section.")
+
     # Attempt to extract a version number from the parsed section
     try:
         version_num = get_version_num(
             df,
             handle_common_errors=handle_common_errors,
             accept_unknown_versions=accept_unknown_versions,
             allow_non_numeric=allow_non_numeric,
             unknown_value=unknown_value
         )
     except Exception as e:
         raise e
+
     # Attempt to validate the section
-    if validate_version(df,version_num=version_num):
+    if not validate_version(df, version_num=version_num):
+        raise Exception("Could not validate version section.")
+
+    try:
+        wrap_val = df.loc[df['mnemonic'] == "WRAP", "value"].values[0]
+        if wrap_val.upper() == 'YES':
+            wrap = True
+        elif wrap_val.upper() == 'NO':
+            wrap = False
+    except Exception as e:
+        raise Exception(f"could not get wrap: {str(e)}")
+
+    if version_num == "3.0":
         try:
-            wrap_val = df.loc[df['mnemonic']=="WRAP","value"].values[0]
+            dlm_val = df.loc[df['mnemonic'] == "DLM", "value"].values[0]
         except Exception as e:
-            raise Exception(f"couldnt get wrap: {str(e)}")
-        if version_num == "3.0":
-            try:
-                dlm_val = df.loc[df['mnemonic']=="DLM","value"].values[0]
-            except Exception as e:
-                raise Exception(f"couldnt get version: {str(e)}")
-        else:
-            dlm_val = None
-        # Attempt to load the section into a section object
-        try:
-            loaded_section = LASSection(
-                'version',
-                version_section,
-                'header',
-                version_num,
-                delimiter=dlm_val,
-                parse_on_init=False,
-                validate_on_init=False
-            )
-            loaded_section.df = df
-            loaded_section.validated = True
-            loaded_section.version_num = version_num
-            return loaded_section
-        except:
-            raise Exception("Couldn't load into section object.")
+            raise Exception(f"could not get version: {str(e)}")
     else:
-        raise Exception("Coulnt validate version section.")
+        dlm_val = None
 
-def parse_title_line(
-        title_line,
-        version_num,
-        all_lowercase=True,
-        associations=False
-    ):
+    # Attempt to load the section into a section object
+    try:
+        loaded_section = LASSection(
+            'version',
+            version_section,
+            'header',
+            version_num,
+            delimiter=dlm_val,
+            parse_on_init=False,
+            validate_on_init=False,
+            wrap=wrap
+        )
+        loaded_section.df = df
+        loaded_section.validated = True
+        loaded_section.version_num = version_num
+        return loaded_section
+    except Exception:
+        raise Exception("Couldn't load into section object.")
+
+
+def parse_title_line(title_line,
+                     version_num,
+                     all_lowercase=True,
+                     assocs=False):
     """
     Parses the title line based on the provided version number.
 
-    This function handles parsing of title lines differently based 
-    on the given version number. Specifically, it handles versions 
+    This function handles parsing of title lines differently based
+    on the given version number. Specifically, it handles versions
     1.2 and 2.0 differently from version 3.0.
 
     Parameters:
     ----------
     title_line : str
         The title line to be parsed.
 
     version_num : str
-        The version number, which determines how the title line is 
+        The version number, which determines how the title line is
         parsed. Can be "1.2", "2.0", or "3.0".
 
     all_lowercase : bool, optional
-        Whether to convert all characters in the title line to 
+        Whether to convert all characters in the title line to
         lowercase before parsing. (default is True)
 
-    associations : bool, optional
-        Whether to consider associations in the parsing process. 
+    assocs : bool, optional
+        Whether to consider associations in the parsing process.
         This is only relevant for version "3.0". (default is False)
 
     Returns:
     -------
     Parsed title line : varies
-        The result of the title line parsing, which depends on the 
+        The result of the title line parsing, which depends on the
         version number.
 
     Raises:
     ------
     Exception:
-        If the version number is not one of the expected values 
+        If the version number is not one of the expected values
         ("1.2", "2.0", "3.0").
     """
     if version_num == "1.2" or version_num == "2.0":
-        return parse_v2_title(title_line,all_lowercase=all_lowercase)
+        return parse_v2_title(title_line, all_lowercase=all_lowercase)
     elif version_num == "3.0":
         return parse_v3_title(
             title_line,
             all_lowercase=all_lowercase,
-            associations=associations
+            assocs=assocs
         )
 
-def parse_v2_title(title_line,all_lowercase=True):
+
+def parse_v2_title(title_line, all_lowercase=True):
     """
     Parses a version 2.0 title line.
 
-    This function specifically handles the parsing of title lines for 
-    version 2.0. It checks if the line begins with '~', extracts the 
+    This function specifically handles the parsing of title lines for
+    version 2.0. It checks if the line begins with '~', extracts the
     section title, and optionally converts it to lowercase.
 
     Parameters:
     ----------
     title_line : str
         The title line to be parsed. This should begin with '~'.
 
     all_lowercase : bool, optional
-        Whether to convert the section title to lowercase. 
+        Whether to convert the section title to lowercase.
         (default is True)
 
     Returns:
     -------
     section_title : str
         The parsed section title from the title line.
 
@@ -477,127 +577,129 @@
         return section_title
     else:
         raise Exception(
             "Cannot parse a line that does not begin with '~' as a "
             "title line."
         )
 
-def parse_v3_title(title_line,all_lowercase=True,associations=False):
+
+def parse_v3_title(title_line, all_lowercase=True, assocs=False):
     """
     Parses a version 3.0 title line.
 
-    This function specifically handles the parsing of title lines for 
-    version 3.0. It checks if the line begins with '~', extracts the 
-    section title and optionally an associated value, and converts them 
+    This function specifically handles the parsing of title lines for
+    version 3.0. It checks if the line begins with '~', extracts the
+    section title and optionally an associated value, and converts them
     to lowercase if requested.
 
     Parameters:
     ----------
     title_line : str
         The title line to be parsed. This should begin with '~'.
 
     all_lowercase : bool, optional
-        Whether to convert the section title and association to 
+        Whether to convert the section title and association to
         lowercase. (default is True)
 
-    associations : bool, optional
-        Whether to consider associations in the parsing process. 
+    assocs : bool, optional
+        Whether to consider associations in the parsing process.
         (default is False)
 
     Returns:
     -------
     section_title : str or tuple
-        The parsed section title from the title line. If 'associations' 
-        is True and an association is present, a tuple of 
+        The parsed section title from the title line. If 'associations'
+        is True and an association is present, a tuple of
         (section_title, association) is returned.
 
     Raises:
     ------
     Exception:
         If the title line does not begin with '~'.
     """
-    has_association = False
+    has_assoc = False
     # Strip leading and trailing whitespace
     title_line = title_line.strip()
     # Check if it actually is a title line
     if title_line.startswith('~'):
         # Strip leading '~'
         title_line = title_line.strip('~')
         # Check if there is an association
         if '|' in title_line:
             # If so, split the title line into the title and association
-            has_association = True
-            title_line,association = title_line.split('|')
-            # If the association is not empty, strip leading and 
+            has_assoc = True
+            title_line, assoc = title_line.split('|')
+            # If the association is not empty, strip leading and
             # trailing whitespace
-            if association.strip().split(' ')[0] != '':
-                association = association.strip().split(' ')[0]
+            if assoc.strip().split(' ')[0] != '':
+                assoc = assoc.strip().split(' ')[0]
             # Otherwise, set the association to None
             else:
-                association = None
+                assoc = None
         # Extract the section title
         if title_line.split(' ')[0] != '':
             section_title = title_line.split(' ')[0]
         else:
             section_title = None
         # Convert to lowercase if requested
         if all_lowercase:
             section_title = section_title.lower()
-            if associations and has_association:
-                association.lower()
+            if assocs and has_assoc:
+                assoc.lower()
         # Return the section title and association if requested
-        if associations and has_association:
-            return section_title,association
+        if assocs and has_assoc:
+            return section_title, assoc
         # Otherwise, just return the section title
         else:
             return section_title
     else:
         # If the line does not begin with '~', raise an exception
         raise Exception(
             "Cannot parse a line that does not begin with '~' as a "
             "title line."
         )
 
-def split_sections(data,version_num,known_sections=known_sections):
+
+def split_sections(data, version_num, known_secs=known_secs):
     """
-    Splits the input data into sections based on the 
+    Splits the input data into sections based on the
     provided version number.
 
-    This function handles the splitting of input data 
-    differently based on the given version number. It 
-    handles versions 1.2 and 2.0 differently from version 
-    3.0. For each version, it uses regular expressions to 
-    identify and extract the sections, and then stores these 
+    This function handles the splitting of input data
+    differently based on the given version number. It
+    handles versions 1.2 and 2.0 differently from version
+    3.0. For each version, it uses regular expressions to
+    identify and extract the sections, and then stores these
     sections in a dictionary using appropriate keys.
 
     Parameters:
     ----------
     data : str
         The input data to be split into sections.
 
     version_num : str
-        The version number, which determines how the 
+        The version number, which determines how the
         data is split. Can be "1.2", "2.0", or "3.0".
 
-    known_sections : dict, optional
-        A dictionary mapping known section names to 
-        their details for each version. 
-        (default is known_sections)
+    known_secs : dict, optional
+        A dictionary mapping known section names to
+        their details for each version.
+        (default is known_secs)
 
     Returns:
     -------
     section_dict : dict
-        A dictionary with the parsed sections. The keys 
-        depend on the version number and the content of 
+        A dictionary with the parsed sections. The keys
+        depend on the version number and the content of
         the sections.
 
     Raises:
     ------
     Exception:
-        If the version number is not one of the expected 
+        If the version number is not one of the expected
         values ("1.2", "2.0", "3.0").
     """
     # Split the data into sections based on the version number
     if version_num == '1.2' or version_num == '2.0':
         # Use a regular expression to split the data into sections
         section_regex = re.compile(r'(~[VWPCOA].+?)(?=~[VWPCOA]|$)', re.DOTALL)
         sections = re.findall(section_regex, data)
@@ -625,64 +727,69 @@
     elif version_num == '3.0':
         # Use a regular expression to split the data into sections
         section_regex = re.compile(r'(~[A-Za-z].+?)(?=~[A-Za-z]|$)', re.DOTALL)
         sections = re.findall(section_regex, data)
         # Store the sections in a dictionary
         section_dict = {}
         # Get the known sections for version 3.0
-        known_sections = known_sections["3.0"]
-        known_section_names = known_sections.keys()
+        known_secs = known_secs["3.0"]
+        known_sec_names = known_secs.keys()
         for section in sections:
             # Get the title line/header of the section
             section_found = False
             title_line_end = section.index('\n')
             title_line = section[:title_line_end].strip()
             # Parse the title line to get the section title
-            section_title = parse_title_line(title_line,"3.0",all_lowercase=True)
+            section_title = parse_title_line(
+                title_line,
+                "3.0",
+                all_lowercase=True
+            )
             # If the section title is a known section name, store it
             # using the known section name as the key
-            if section_title in known_section_names:
+            if section_title in known_sec_names:
                 section_dict[section_title] = section.strip()
                 section_found = True
             # If the section title is not a known section name, check
             # if it is an alias for a known section name then store it
             # using the known section name as the key
             else:
-                for known_section_name,known_section in known_sections.items():
-                    if section_title in known_section["titles"]:
-                        section_dict[known_section_name] = section.strip()
+                for known_sec_name, known_sec in known_secs.items():
+                    if section_title in known_sec["titles"]:
+                        section_dict[known_sec_name] = section.strip()
                         section_found = True
                 if not section_found:
                     section_dict[section_title] = section.strip()
         # Return the dictionary of sections
         return section_dict
     else:
-        # Raise an exception if the version number is not one of the 
+        # Raise an exception if the version number is not one of the
         # expected values
         raise Exception("Unknown version. Must be '1.2','2.0', or '3.0'")
 
+
 def parse_header_section(section_string, version_num='2.0', delimiter=None):
     """
     Parses the header section of a LAS file.
-    
+
     This function parses the header section of a LAS file and returns
     a dictionary with the parsed information. The version number is
     used to determine how the header section is parsed. The delimiter
     is used to split the header section into lines. If no delimiter is
     provided, the header section is split into lines using the newline
     character.
 
     Parameters:
     ----------
     section_string : str
         The header section of a LAS file.
-    
+
     version_num : str, optional
         The version number of the LAS file. (default is '2.0')
-    
+
     delimiter : str, optional
         The delimiter used to split the header section into lines.
         (default is None)
 
     Returns:
     -------
     header_dict : dict
@@ -690,23 +797,23 @@
     """
     results = []
     lines = section_string.strip().split("\n")
     if version_num == '2.0' or version_num == '1.2':
         # Skip comment, title, and empty lines
         for line in lines:
             if (
-                line.strip().startswith("#") or 
-                line.strip().startswith("~") or 
+                line.strip().startswith("#") or
+                line.strip().startswith("~") or
                 line.strip().strip("\n") == ""
             ):
                 continue
             # Remove whitespace from the line
             line = line.strip()
             # Get the mnemonic.
-            # The mnemonic is everything before the first period, 
+            # The mnemonic is everything before the first period,
             # stripped of whitespace.
             frst_prd = line.index('.')
             mnemonic = line[:frst_prd].strip()
             # Get the units.
             # The units are everything between the first period
             # and the first space after the first period, stripped
             # of whitespace.
@@ -715,224 +822,293 @@
             units = line_aft_frst_prd[:frst_spc_aft_frst_prd].strip()
             # Get the value.
             # The value is everything between the first space after
             # the first period and the last colon, stripped of whitespace.
             lst_col = line_aft_frst_prd.rindex(':')
             value = line_aft_frst_prd[frst_spc_aft_frst_prd:lst_col].strip()
             # Get the description.
-            # The description is everything after the last colon, 
+            # The description is everything after the last colon,
             # stripped of whitespace.
-            description = line_aft_frst_prd[lst_col+1:].strip()
+            descr = line_aft_frst_prd[lst_col+1:].strip()
             results.append(
                 {
                     "mnemonic": mnemonic,
                     "units": units if units != "" else None,
                     "value": value if value != "" else None,
-                    "description": description if description != "" else None
+                    "description": descr if descr != "" else None
                 }
             )
         return DataFrame(results)
     if version_num == '3.0':
         for line in lines:
             format = None
-            associations = None
+            assocs = None
             # Skip comment, title, and empty lines
             if (
-                line.strip().startswith("#") or 
-                line.strip().startswith("~") or 
+                line.strip().startswith("#") or
+                line.strip().startswith("~") or
                 line.strip().strip("\n") == ""
             ):
                 continue
             # Remove whitespace from the line
             line = line.strip()
-            # Get the mnemonic. 
-            # The mnemonic is everything before the 
+            # Get the mnemonic.
+            # The mnemonic is everything before the
             # first period, stripped of whitespace
             frst_prd = line.index('.')
             mnemonic = line[:frst_prd].strip()
-            # Get the units. 
-            # The units are everything between the first period and the 
+            # Get the units.
+            # The units are everything between the first period and the
             # first space after the first period, stripped of whitespace.
             line_aft_frst_prd = line[frst_prd+1:]
             frst_spc_aft_frst_prd = line_aft_frst_prd.index(' ')
             units = line_aft_frst_prd[:frst_spc_aft_frst_prd].strip()
             # Get the value.
             # The value is everything between the first space after the
             # first period and the last colon, stripped of whitespace.
             lst_col = line_aft_frst_prd.rindex(':')
             value = line_aft_frst_prd[frst_spc_aft_frst_prd:lst_col].strip()
             # Get the description, format, and associations.
-            # The description is everything after the last colon and 
-            # before the first brace or pipe, if no braces are present, 
+            # The description is everything after the last colon and
+            # before the first brace or pipe, if no braces are present,
             # stripped of whitespace.
             line_aft_lst_col = line_aft_frst_prd[lst_col+1:]
             if '{' in line_aft_lst_col and '}' in line_aft_lst_col:
                 frst_brc_aft_lst_col = line_aft_lst_col.index('{')
-                description = line_aft_lst_col[:frst_brc_aft_lst_col]
+                descr = line_aft_lst_col[:frst_brc_aft_lst_col]
                 line_aft_frst_brc = line_aft_lst_col[frst_brc_aft_lst_col+1:]
                 clsng_brc = line_aft_frst_brc.rindex('}')
                 format = line_aft_frst_brc[:clsng_brc].strip()
                 line_aft_clsng_brc = line_aft_frst_brc[clsng_brc+1:]
                 if '|' in line_aft_clsng_brc:
                     bar = line_aft_clsng_brc.index('|')
-                    associations = line_aft_clsng_brc[bar+1:].strip()
+                    assocs = line_aft_clsng_brc[bar+1:].strip()
             elif '|' in line_aft_lst_col:
                 bar = line_aft_lst_col.index('|')
-                associations = line_aft_lst_col[bar+1:].strip()
+                assocs = line_aft_lst_col[bar+1:].strip()
             else:
-                description = line_aft_frst_prd[lst_col+1:].strip()
+                descr = line_aft_frst_prd[lst_col+1:].strip()
             # Add the parsed values to the results list
             results.append(
                 {
                     "mnemonic": mnemonic,
                     "units": units if units != "" else None,
                     "value": value if value != "" else None,
-                    "description": description if description != "" else None,
+                    "description": descr if descr != "" else None,
                     "format": format if format != "" else None,
-                    "associations": associations if associations != "" else None
+                    "associations": assocs if assocs != "" else None
                 }
             )
         # Return the results as a DataFrame
         return DataFrame(results)
 
-def parse_data_section(raw_data,version_num,delimiter=None):
+
+def parse_data_section(raw_data, version_num, delimiter=None):
     """
-    Parses the data section of the input raw data based on the provided 
+    Parses the data section of the input raw data based on the provided
     version number.
 
-    This function handles the parsing of the data section from the 
-    input raw data. It removes lines beginning with '#' or '~', and 
+    This function handles the parsing of the data section from the
+    input raw data. It removes lines beginning with '#' or '~', and
     then loads the data into a LASData object.
 
     Parameters:
     ----------
     raw_data : str
         The raw data to be parsed.
 
     version_num : str
-        The version number, which is used when loading the data into a 
+        The version number, which is used when loading the data into a
         LASData object.
 
     delimiter : str, optional
-        The delimiter character used to separate values in the data. If 
-        not provided, the default delimiter for the LASData class is 
+        The delimiter character used to separate values in the data. If
+        not provided, the default delimiter for the LASData class is
         used.
 
     Returns:
     -------
     loaded_data : LASData
         The loaded data as a LASData object.
 
     """
     filtered_data = re.sub(r'^[#~].*\n', '', raw_data, flags=re.MULTILINE)
-    loaded_data = LASData(filtered_data,version_num,delimiter=delimiter)
+    loaded_data = LASData(filtered_data, version_num, delimiter=delimiter)
     return loaded_data
 
-def validate_version(df,version_num=None):
+
+# def validate_version(df, version_num=None):
+#     """
+#     Validates the version of a dataframe.
+
+#     This function checks if the dataframe contains all required
+#     mnemonics for the given version number and verifies the values of
+#     these mnemonics. The specific checks differ based on the version
+#     number.
+
+#     Parameters:
+#     ----------
+#     df : DataFrame
+#         The dataframe to be validated. This dataframe should contain a
+#         'mnemonic' column and a 'value' column.
+
+#     version_num : str, optional
+#         The version number of the dataframe. Must be either "1.2",
+#         "2.0", or "3.0". If not provided, the function will use the
+#         value in the dataframe.
+
+#     Returns:
+#     -------
+#     bool:
+#         Returns True if the dataframe is valid for the given version
+#         number.
+
+#     Raises:
+#     ------
+#     Exception:
+#         If any of the required mnemonics are missing or have invalid
+#         values, or if the version number is not one of the expected
+#         values ("1.2", "2.0", "3.0").
+#     """
+#     if version_num == "1.2" or version_num == "2.0":
+#         req_mnemonics = [
+#             "VERS",
+#             "WRAP"
+#         ]
+#     elif version_num == "3.0":
+#         req_mnemonics = [
+#             "VERS",
+#             "WRAP",
+#             "DLM"
+#         ]
+#     if all(mnemonic in df.mnemonic.values for mnemonic in req_mnemonics):
+#         if version_num == "1.2" or version_num == "2.0":
+#             try:
+#                 vers = df.loc[df['mnemonic'] == "VERS", "value"].values[0]
+#             except Exception as e:
+#                 raise Exception(f"Couldnt get VERS value: {str(e)}")
+#             try:
+#                 wrap = df.loc[df['mnemonic'] == "WRAP", "value"].values[0]
+#             except Exception as e:
+#                 raise Exception(f"Couldnt get WRAP value: {str(e)}")
+#             if wrap.upper() in ["YES", "NO"]:
+#                 return True
+#             else:
+#                 raise Exception("Wrap value must be 'YES' or 'NO'.")
+#         elif version_num == "3.0":
+#             try:
+#                 vers = df.loc[df['mnemonic'] == "VERS", "value"].values[0]
+#             except Exception as e:
+#                 raise Exception(f"Couldnt get VERS value: {str(e)}")
+#             try:
+#                 wrap = df.loc[df['mnemonic'] == "WRAP", "value"].values[0]
+#             except Exception as e:
+#                 raise Exception(f"Couldnt get WRAP value: {str(e)}")
+#             try:
+#                 dlm = df.loc[df['mnemonic'] == "DLM", "value"].values[0]
+#             except Exception as e:
+#                 raise Exception(f"Couldnt get DLM value: {str(e)}")
+#             if wrap.upper() in ["NO"]:
+#                 if dlm.upper() in ["SPACE", "COMMA", "TAB"]:
+#                     return True
+#                 elif dlm is None or dlm == '':
+#                     return True
+#                 else:
+#                     raise Exception("Unrecognized delimiter.")
+#             else:
+#                 raise Exception("Wrap value must be 'NO'.")
+#         else:
+#             raise Exception("Only accepts version 1.2, 2.0, and 3.0")
+#     else:
+#         raise Exception("Missing required version section mnemonic.")
+
+
+def validate_version(df, version_num=None):
     """
     Validates the version of a dataframe.
 
-    This function checks if the dataframe contains all required 
-    mnemonics for the given version number and verifies the values of 
-    these mnemonics. The specific checks differ based on the version 
+    This function checks if the dataframe contains all required
+    mnemonics for the given version number and verifies the values of
+    these mnemonics. The specific checks differ based on the version
     number.
 
     Parameters:
     ----------
     df : DataFrame
-        The dataframe to be validated. This dataframe should contain a 
+        The dataframe to be validated. This dataframe should contain a
         'mnemonic' column and a 'value' column.
 
     version_num : str, optional
-        The version number of the dataframe. Must be either "1.2", 
-        "2.0", or "3.0". If not provided, the function will use the 
+        The version number of the dataframe. Must be either "1.2",
+        "2.0", or "3.0". If not provided, the function will use the
         value in the dataframe.
 
     Returns:
     -------
     bool:
-        Returns True if the dataframe is valid for the given version 
+        Returns True if the dataframe is valid for the given version
         number.
 
     Raises:
     ------
     Exception:
-        If any of the required mnemonics are missing or have invalid 
-        values, or if the version number is not one of the expected 
+        If any of the required mnemonics are missing or have invalid
+        values, or if the version number is not one of the expected
         values ("1.2", "2.0", "3.0").
     """
-    if version_num == "1.2" or version_num == "2.0":
-        req_mnemonics = [
-            "VERS",
-            "WRAP"
-        ]
+    if version_num in ["1.2", "2.0"]:
+        req_mnemonics = ["VERS", "WRAP"]
     elif version_num == "3.0":
-        req_mnemonics = [
-            "VERS",
-            "WRAP",
-            "DLM"
-        ]
-    if all(mnemonic in df.mnemonic.values for mnemonic in req_mnemonics):
-        if version_num == "1.2" or version_num == "2.0":
-            try:
-                vers = df.loc[df['mnemonic'] == "VERS", "value"].values[0]
-            except Exception as e:
-                raise Exception(f"Couldnt get VERS value: {str(e)}")
-            try:
-                wrap = df.loc[df['mnemonic'] == "WRAP", "value"].values[0]
-            except Exception as e:
-                raise Exception(f"Couldnt get WRAP value: {str(e)}")
-            if wrap.upper() in ["YES","NO"]:
-                return True
-            else:
-                raise Exception("Wrap value must be 'YES' or 'NO'.")
-        elif version_num == "3.0":
-            try:
-                vers = df.loc[df['mnemonic'] == "VERS", "value"].values[0]
-            except Exception as e:
-                raise Exception(f"Couldnt get VERS value: {str(e)}")
-            try:
-                wrap = df.loc[df['mnemonic'] == "WRAP", "value"].values[0]
-            except Exception as e:
-                raise Exception(f"Couldnt get WRAP value: {str(e)}")
-            try:
-                dlm = df.loc[df['mnemonic'] == "DLM", "value"].values[0]
-            except Exception as e:
-                raise Exception(f"Couldnt get DLM value: {str(e)}")
-            if wrap.upper() in ["NO"]:
-                if dlm.upper() in ["SPACE","COMMA","TAB"]:
-                    return True
-                elif dlm == None or dlm == '':
-                    return True
-                else:
-                    raise Exception("Unrecognized delimiter.")
-            else:
-                raise Exception("Wrap value must be 'NO'.")
-        else:
-            raise Exception("Only accepts version 1.2, 2.0, and 3.0")
+        req_mnemonics = ["VERS", "WRAP", "DLM"]
     else:
+        raise Exception("Only accepts version 1.2, 2.0, and 3.0")
+
+    if not all(mnemonic in df.mnemonic.values for mnemonic in req_mnemonics):
         raise Exception("Missing required version section mnemonic.")
 
+    try:
+        wrap = df.loc[df['mnemonic'] == "WRAP", "value"].values[0]
+    except Exception as e:
+        raise Exception(f"Couldnt get WRAP value: {str(e)}")
+
+    if version_num == "3.0":
+        try:
+            dlm = df.loc[df['mnemonic'] == "DLM", "value"].values[0]
+        except Exception as e:
+            raise Exception(f"Couldnt get DLM value: {str(e)}")
+        if (
+            wrap.upper() not in ["NO"] or
+            dlm.upper() not in ["SPACE", "COMMA", "TAB", None, '']
+        ):
+            raise Exception("Invalid wrap or delimiter value for version 3.0")
+    elif wrap.upper() not in ["YES", "NO"]:
+        raise Exception(
+            "Wrap value for versions 1.2 and 2.0 must be 'YES' or 'NO'."
+        )
+
+    return True
+
+
 def validate_v2_well(df):
     """
     Validates the well section of a dataframe for version 2 LAS files.
 
-    This function checks if the dataframe contains all the required 
+    This function checks if the dataframe contains all the required
     mnemonics specific to the well section of a version 2 LAS file.
 
     Parameters:
     ----------
     df : DataFrame
-        The dataframe to be validated. This dataframe should contain a 
+        The dataframe to be validated. This dataframe should contain a
         'mnemonic' column.
 
     Returns:
     -------
     bool:
-        Returns True if the dataframe is valid for the well section of 
+        Returns True if the dataframe is valid for the well section of
         a version 2 LAS file.
 
     Raises:
     ------
     Exception:
         If any of the required mnemonics are missing.
     """
@@ -949,62 +1125,66 @@
         "SRVC",
         "DATE",
     ]
     if all(mnemonic in df.mnemonic.values for mnemonic in req_mnemonics):
         if (
             "PROV" in df.mnemonic.values or
             all(
-                mnemonic 
-                in df.mnemonic.values 
-                for mnemonic in ["CNTY","STAT","CTRY"]
+                mnemonic
+                in df.mnemonic.values
+                for mnemonic in ["CNTY", "STAT", "CTRY"]
             )
         ):
-            if "API" in df.mnemonic.values or\
-                "UWI" in df.mnemonic.values:
-                 return True
+            if (
+                "API" in df.mnemonic.values or
+                "UWI" in df.mnemonic.values
+            ):
+                return True
             else:
                 raise Exception(
                     "Couldnt validate section, 'UWI' and 'API' items missing."
                     )
         else:
             raise Exception(
                 "Couldnt validate section, missing 'PROV' or "
                 "('CNTY','STAT','CTRY') items."
             )
     else:
         raise Exception("Missing required mnemonics.")
 
+
 # Set of valid country codes for the CTRY mnemonic
-valid_country_codes = ["US","CA"]
+valid_country_codes = ["US", "CA"]
+
 
 def validate_v3_well(df):
     """
-    Validates the well section of a DataFrame for 
+    Validates the well section of a DataFrame for
     version 3 LAS files.
 
-    This function checks if the DataFrame contains all the required 
-    mnemonics specific to the well section of a version 3 LAS file. It 
+    This function checks if the DataFrame contains all the required
+    mnemonics specific to the well section of a version 3 LAS file. It
     also validates geographic coordinates and country code.
 
     Parameters:
     ----------
     df : DataFrame
-        The DataFrame to be validated. This DataFrame should contain a 
+        The DataFrame to be validated. This DataFrame should contain a
         'mnemonic' column.
 
     Returns:
     -------
     bool:
-        Returns True if the DataFrame is valid for the well section of 
+        Returns True if the DataFrame is valid for the well section of
         a version 3 LAS file.
 
     Raises:
     ------
     Exception:
-        If any of the required mnemonics are missing, or if geographic 
+        If any of the required mnemonics are missing, or if geographic
         coordinates or country code are not properly specified.
     """
     # Set of required mnemonics for version 3.0 well sections
     req_mnemonics = [
         "STRT",
         "STOP",
         "STEP",
@@ -1014,184 +1194,187 @@
         "FLD",
         "LOC",
         "SRVC",
         "CTRY",
         "DATE",
     ]
     if all(
-        mnemonic 
-        in df.mnemonic.values 
+        mnemonic
+        in df.mnemonic.values
         for mnemonic in req_mnemonics
     ):
         if (
             all(
-                mnemonic 
-                in df.mnemonic.values 
-                for mnemonic in ["LATI","LONG","GDAT"]
-            ) 
+                mnemonic
+                in df.mnemonic.values
+                for mnemonic in ["LATI", "LONG", "GDAT"]
+            )
             or
             all(
-                mnemonic 
-                in df.mnemonic.values 
-                for mnemonic in ["X","Y","GDAT","HZCS"]
+                mnemonic
+                in df.mnemonic.values
+                for mnemonic in ["X", "Y", "GDAT", "HZCS"]
             )
         ):
             country_code = df.loc[
                 df["mnemonic"] == "CTRY", 'value'
             ].values[0].upper()
             if country_code in valid_country_codes:
                 if country_code == "CA":
                     if all(
-                        mnemonic 
-                        in df.mnemonic.values 
-                        for mnemonic in ["PROV","UWI","LIC"]
+                        mnemonic
+                        in df.mnemonic.values
+                        for mnemonic in ["PROV", "UWI", "LIC"]
                     ):
                         return True
                 elif country_code == "US":
                     if all(
-                        mnemonic 
-                        in df.mnemonic.values 
-                        for mnemonic in ["PROV","UWI","LIC"]
+                        mnemonic
+                        in df.mnemonic.values
+                        for mnemonic in ["PROV", "UWI", "LIC"]
                     ):
                         return True
-            elif country_code == None or\
-                country_code == '':
+            elif (
+                    country_code is None or
+                    country_code == ''
+            ):
                 return True
             else:
                 raise Exception(f"Invalid country code {country_code}")
         else:
             raise Exception(
-                f"Couldnt validate section, missing ('LATI','LONG','GDAT') "
-                f"or ('X','Y','GDAT','HZCS') items."
+                "Couldnt validate section, missing ('LATI','LONG','GDAT') "
+                "or ('X','Y','GDAT','HZCS') items."
                 )
     else:
         raise Exception("Missing required mnemonics.")
 
-def validate_well(df,version_num):
+
+def validate_well(df, version_num):
     """
-    Validates the well section of a DataFrame for specified LAS file 
+    Validates the well section of a DataFrame for specified LAS file
     versions.
 
-    This function calls either validate_v2_well or validate_v3_well 
-    depending on the version number provided. It verifies the DataFrame 
+    This function calls either validate_v2_well or validate_v3_well
+    depending on the version number provided. It verifies the DataFrame
     for the required structure according to the LAS version.
 
     Parameters:
     ----------
     df : DataFrame
-        The DataFrame to be validated. This DataFrame should contain a 
+        The DataFrame to be validated. This DataFrame should contain a
         'mnemonic' column.
 
     version_num : str
-        A string representing the LAS version. Valid values are "1.2", 
+        A string representing the LAS version. Valid values are "1.2",
         "2.0", and "3.0".
 
     Returns:
     -------
     bool:
-        Returns True if the DataFrame is valid for the well section of 
+        Returns True if the DataFrame is valid for the well section of
         the given LAS version.
 
     Raises:
     ------
     Exception:
         If validation fails in the respective validate function.
     """
-    if version_num == "1.2" or version_num =="2.0":
+    if version_num == "1.2" or version_num == "2.0":
         try:
             validate_v2_well(df)
             return True
         except Exception as e:
             raise e
     if version_num == "3.0":
         try:
             validate_v3_well(df)
             return True
         except Exception as e:
             raise e
 
-def validate_parsed_section(name,type,parsed_section,version_num):
+
+def validate_parsed_section(name, type, parsed_section, version_num):
     """
-    Validates parsed sections from a LAS file depending on the section 
+    Validates parsed sections from a LAS file depending on the section
     name, type and the file's version.
 
-    This function checks the validity of parsed sections from a LAS 
-    file based on their name and type. It calls specific validation 
-    functions (validate_version, validate_well) for version and well 
+    This function checks the validity of parsed sections from a LAS
+    file based on their name and type. It calls specific validation
+    functions (validate_version, validate_well) for version and well
     headers and checks for read_errors attribute in data section.
 
     Parameters:
     ----------
     name : str
-        Name of the section to be validated. For example 'version', 
+        Name of the section to be validated. For example 'version',
         'well', 'data'.
 
     type : str
         Type of the section. For example 'header', 'data'.
 
     parsed_section : object
-        The parsed section which is to be validated. This could be a 
+        The parsed section which is to be validated. This could be a
         DataFrame or a LASData object.
 
     version_num : str
         The version of the LAS file. For example '1.2', '2.0', '3.0'.
 
     Returns:
     -------
     bool:
-        Returns True if the parsed section is valid according to the 
-        section's name, type, and LAS file's version. Returns False 
+        Returns True if the parsed section is valid according to the
+        section's name, type, and LAS file's version. Returns False
         otherwise.
     """
     if name == 'version' and type == 'header':
-        return validate_version(parsed_section,version_num)
+        return validate_version(parsed_section, version_num)
     elif name == 'well' and type == 'header':
-        return validate_well(parsed_section,version_num)
+        return validate_well(parsed_section, version_num)
     elif name == 'data' and type == 'data':
-        if hasattr(parsed_section,'read_errors'):
+        if hasattr(parsed_section, 'read_errors'):
             return False
         else:
             return True
     else:
         return False
 
-import warnings
 
 class LASData():
     """
-    Class for storing and handling Log ASCII 
+    Class for storing and handling Log ASCII
     Standard (LAS) data.
 
-    The class provides an interface to load, handle and validate LAS 
-    data. The LAS format is used to store well log data in the oil and 
+    The class provides an interface to load, handle and validate LAS
+    data. The LAS format is used to store well log data in the oil and
     gas industry.
 
     Attributes:
     ----------
     raw_data : str
         The raw LAS data as a string.
 
     version_num : str
         The version of the LAS file.
 
     delimiter : str, optional
-        The delimiter used in the LAS data, such as SPACE, COMMA, or 
+        The delimiter used in the LAS data, such as SPACE, COMMA, or
         TAB. Defaults to None, indicating a space delimiter.
 
     invalid_raise : bool, optional
         Whether to raise an exception when invalid data is encountered.
         Defaults to False.
 
     unrecognized_delimiters : bool, optional
-        If True, any unrecognized delimiters are replaced with the 
+        If True, any unrecognized delimiters are replaced with the
         default delimiter.
         Defaults to True.
 
     default_delimiter : str, optional
-        The default delimiter to use if an unrecognized delimiter is 
+        The default delimiter to use if an unrecognized delimiter is
         found. Defaults to a space.
 
     delimiter_error : str, optional
         Stores an error message if an unrecognized delimiter is found.
 
     data : numpy.ndarray
         The parsed LAS data, stored as a numpy array.
@@ -1200,178 +1383,183 @@
         The parsed LAS data, stored as a pandas DataFrame.
 
     read_errors : list, optional
         Stores any read errors encountered when loading the data.
 
     Methods:
     -------
-    __init__(self, raw_data, version_num, delimiter=None, 
-    invalid_raise=False, unrecognized_delimiters=True, 
+    __init__(self, raw_data, version_num, delimiter=None,
+    invalid_raise=False, unrecognized_delimiters=True,
     default_delimiter=' ')
-        Initializes the LASData object by parsing the provided 
+        Initializes the LASData object by parsing the provided
         raw LAS data.
     """
     def __init__(
-        self, 
-        raw_data, 
-        version_num, 
-        delimiter=None, 
-        invalid_raise=False, 
-        unrecognized_delimiters=True, 
+        self,
+        raw_data,
+        version_num,
+        delimiter=None,
+        invalid_raise=False,
+        unrecognized_delimiters=True,
         default_delimiter=' '
     ):
         self.raw_data = raw_data
         self.delimiter = delimiter
         delim_dict = {
-            'SPACE':' ',
-            'COMMA':',',
-            'TAB':'\t'
+            'SPACE': ' ',
+            'COMMA': ',',
+            'TAB': '\t'
         }
         if self.delimiter in delim_dict.keys():
             delim = delim_dict[self.delimiter]
-        elif self.delimiter in delim_dict.values() or self.delimiter == None:
+        elif self.delimiter in delim_dict.values() or self.delimiter is None:
             delim = self.delimiter
         elif unrecognized_delimiters:
             if default_delimiter in delim_dict.values():
                 delim = default_delimiter
             else:
                 self.delimiter_error = (
                     f"Unrecognized delimiter: '{self.delimiter}', and default "
                     f"delimiter '{default_delimiter} unable to load!"
                 )
         else:
-            self.delimiter_error = f"Unrecognized delimiter: '{self.delimiter}', unable to load!"
+            self.delimiter_error = (
+                f"Unrecognized delimiter: '{self.delimiter}', unable to load!"
+            )
             return
         with StringIO(self.raw_data) as f:
             with warnings.catch_warnings(record=True) as w:
                 warnings.simplefilter("always")
                 self.data = genfromtxt(
-                    f, 
-                    delimiter=delim, 
+                    f,
+                    delimiter=delim,
                     invalid_raise=invalid_raise
                 )
                 self.df = DataFrame(self.data)
                 for warn in w:
                     if issubclass(warn.category, UserWarning):
                         self.read_errors = [
-                            err 
-                            for err 
+                            err
+                            for err
                             in str(warn.message).split("\n")
                         ]
                         return
 
+
 class LASSection():
     """
-    Class representing a section of Log ASCII 
+    Class representing a section of Log ASCII
     Standard (LAS) data.
 
-    This class provides methods and properties 
-    for parsing, validating and handling a LAS section. 
+    This class provides methods and properties
+    for parsing, validating and handling a LAS section.
 
     Attributes:
     ----------
     name : str
         The name of the section.
-    
+
     raw_data : str
         The raw data of the section as a string.
 
     type : str
         The type of the section, either 'header', 'data', or 'other'.
-    
+
     version_num : str
         The version number of the LAS file the section belongs to.
 
-    association : str, optional
-        The association of the section. 
+    assoc : str, optional
+        The association of the section.
         Defaults to None.
 
     delimiter : str, optional
-        The delimiter used in the section. 
+        The delimiter used in the section.
         Defaults to None.
 
     parsed_section : obj, optional
-        The parsed section. This is populated when the section is 
-        parsed. 
+        The parsed section. This is populated when the section is
+        parsed.
 
     parsed : bool, optional
-        Indicates whether the section has been parsed. 
+        Indicates whether the section has been parsed.
         Defaults to False.
-    
+
     validated : bool, optional
-        Indicates whether the section has been validated. 
+        Indicates whether the section has been validated.
         Defaults to False.
 
     df : pandas.DataFrame
         The DataFrame representing the parsed data of the section.
 
     Methods:
     -------
-    __init__(self, name, raw_data, section_type, version_num, 
-    association=None, delimiter=None, parse_on_init=True, 
+    __init__(self, name, raw_data, section_type, version_num,
+    assoc=None, delimiter=None, parse_on_init=True,
     validate_on_init=True)
-        Initializes the LASSection object, parses the raw data, 
-        validates the parsed section if parse_on_init and 
+        Initializes the LASSection object, parses the raw data,
+        validates the parsed section if parse_on_init and
         validate_on_init are set to True.
 
     __repr__(self)
-        Returns a string that represents the LASSection object in a way 
+        Returns a string that represents the LASSection object in a way
         that can be used to recreate the object.
 
     __str__(self)
-        Returns a user-friendly string representation of the LASSection 
-        object. 
+        Returns a user-friendly string representation of the LASSection
+        object.
 
     parse(self)
-        Parses the raw data into a usable format (not implemented in 
+        Parses the raw data into a usable format (not implemented in
         this code snippet).
 
     validate(self)
-        Validates the parsed section (not implemented in this code 
+        Validates the parsed section (not implemented in this code
         snippet).
 
     """
     def __init__(
         self,
         name,
         raw_data,
         section_type,
         version_num,
-        association=None,
+        assoc=None,
         delimiter=None,
         parse_on_init=True,
-        validate_on_init=True
+        validate_on_init=True,
+        wrap=False
     ):
         # initialize attributes
         self.name = name
         self.raw_data = raw_data
         self.type = section_type
         self.version_num = version_num
-        self.assocation = association
+        self.assocation = assoc
         self.delimiter = delimiter
         self.validated = False
+        self.wrap = wrap
         # parse section
         if '\n' in self.raw_data:
             # parse title line
             title_line_end = self.raw_data.index('\n')
             title_line = self.raw_data[:title_line_end].strip()
             if '|' in title_line:
                 result = parse_title_line(
                     title_line,
                     version_num=self.version_num,
                     all_lowercase=True,
-                    associations=True
+                    assocs=True
                 )
                 if type(result) != str:
                     self.association = result[1]
                 else:
                     self.association = None
             else:
                 self.association = None
-            
+
             # parse header section
             if self.type.lower() == 'header':
                 if parse_on_init:
                     try:
                         self.parsed_section = parse_header_section(
                             self.raw_data,
                             version_num=version_num
@@ -1383,15 +1571,15 @@
                         )
                         self.parse_tb = traceback.format_exc()
                         return
             # parse data section
             elif self.type.lower() == 'data':
                 if parse_on_init:
                     try:
-                        #print(f"section name: {name}")
+                        # print(f"section name: {name}")
                         self.parsed_section = parse_data_section(
                             self.raw_data,
                             version_num=version_num,
                             delimiter=self.delimiter
                         )
                         self.df = self.parsed_section.df
                     except Exception as e:
@@ -1405,15 +1593,15 @@
                 try:
                     self.parsed_section = parse_header_section(
                         self.raw_data,
                         version_num=version_num
                         )
                     self.df = self.parsed_section
                     self.type = 'header'
-                except:
+                except Exception:
                     try:
                         self.parsed_section = parse_data_section(
                             self.raw_data,
                             version_num=version_num,
                             delimiter=self.delimiter
                         )
                         self.df = self.parsed_section.df
@@ -1422,16 +1610,16 @@
                         self.parse_error = (
                             f"Couldn't parse '{self.name}' data: {str(e)}"
                         )
                         self.parse_tb = traceback.format_exc()
                         return
             # validate section
             if (
-                parse_on_init and validate_on_init and 
-                not hasattr(self,'parse_error')
+                parse_on_init and validate_on_init and
+                not hasattr(self, 'parse_error')
             ):
                 try:
                     validation = validate_parsed_section(
                         self.name,
                         self.type,
                         self.parsed_section,
                         self.version_num
@@ -1454,64 +1642,64 @@
     def __repr__(self):
         return (
             f"LASSection(name={self.name!r}, type={self.type!r}, "
             f"version_num={self.version_num!r})"
         )
 
     def __str__(self):
-        s = f"LASSection\n"
+        s = "LASSection\n"
         s += f"    Name: {self.name}\n"
         s += f"    Type: {self.type}\n"
         s += f"    Version: {self.version_num}\n"
         s += f"    Delimiter: {self.delimiter}\n"
         if not hasattr(self, 'parse_error'):
-            s += f"    Parsed: True\n" 
+            s += "    Parsed: True\n"
         else:
-            s += f"    Parsed: False\n"
-            s += f"    Errors:\n"
+            s += "    Parsed: False\n"
+            s += "    Errors:\n"
             s += f"        Parsing Error: {self.parse_error}\n"
             s += f"        Traceback:\n{self.parse_tb}\n"
         if not hasattr(self, 'validate_error'):
             s += f"    Validated: {self.validated}\n"
         else:
             s += f"    Validated: {self.validated}\n"
-            s += f"    Errors:\n"
+            s += "    Errors:\n"
             s += f"        Validation Error: {self.validate_error}\n"
             s += f"        Traceback:\n{self.validate_tb}\n"
         if hasattr(self, 'df'):
             s += f"    Rows: {len(self.df)}\n"
 
-        
         return s
 
+
 # Check for definition/curve and data column congruency
-def check_definitions_and_format_data(def_section,data_section):
+def check_definitions_and_format_data(def_section, data_section):
     """
-    Checks the congruency between the definitions (header) and data 
+    Checks the congruency between the definitions (header) and data
     sections of a LAS file and formats the data section accordingly.
-    
+
     Parameters:
     -----------
     def_section : LASSection
-        An instance of LASSection representing the definition section 
+        An instance of LASSection representing the definition section
         (usually the header) of a LAS file.
 
     data_section : LASSection
-        An instance of LASSection representing the data section of a 
+        An instance of LASSection representing the data section of a
         LAS file.
-        
+
     Returns:
     --------
     None
-    
+
     Note:
     ----
-    If the number of rows in the definition section matches the number 
-    of columns in the data section, it renames the columns of the data 
-    section with the column names of the definition section. This 
+    If the number of rows in the definition section matches the number
+    of columns in the data section, it renames the columns of the data
+    section with the column names of the definition section. This
     operation modifies the data_section in-place.
     """
     def_rows = def_section.df.shape[0]
     print(def_rows)
     data_cols = data_section.df.shape[1]
     print(data_cols)
     if hasattr(def_section, 'df') and hasattr(data_section, 'df'):
@@ -1524,153 +1712,157 @@
                 columns=dict(zip(
                         data_section.df.columns,
                         def_section.df.columns
                 )),
                 inplace=True
             )
 
+
 class LASFile():
     """
     Class representing a Log ASCII Standard (LAS) file.
 
-    This class provides methods and attributes for 
+    This class provides methods and attributes for
     reading, parsing,
     validating, and handling a LAS file.
 
     Attributes
     ----------
     file_path : str
         Path to the LAS file.
 
     sections : list[LASSection]
-        List of LASSection objects, each representing a different 
+        List of LASSection objects, each representing a different
         section of the LAS file.
 
     version : LASSection
         Section of the LAS file containing version information.
 
     version_num : str
         Version number of the LAS file.
 
     delimiter : str
         Delimiter used in the LAS file.
 
     read_error : str
-        Error message generated if an error occurs while reading the 
+        Error message generated if an error occurs while reading the
         file.
 
     parse_error : str
-        Error message generated if an error occurs while parsing the 
+        Error message generated if an error occurs while parsing the
         file.
 
     parse_tb : str
         Traceback information if an error occurs while parsing the file.
 
     validate_error : str
-        Error message generated if an error occurs while validating the 
+        Error message generated if an error occurs while validating the
         file.
 
     validate_tb : str
-        Traceback information if an error occurs while validating the 
+        Traceback information if an error occurs while validating the
         file.
 
     Methods
     -------
     __init__(file_path: Optional[str]=None, always_try_split: bool=False)
-        Initializes a LASFile instance. If a file path is 
+        Initializes a LASFile instance. If a file path is
         provided, tries to read and split the LAS file into sections.
 
     validate_defs_and_data()
-        Ensures the congruency between the definition and 
+        Ensures the congruency between the definition and
         data sections in the LAS file.
 
     __str__()
-        Returns a human-readable string representation of 
-        the LASFile instance, including error messages if 
+        Returns a human-readable string representation of
+        the LASFile instance, including error messages if
         any errors occurred during initialization.
     """
     def __init__(self, file_path=None, always_try_split=False):
-        if file_path != None:
+        if file_path is not None:
             self.file_path = file_path
             # Try to open the file
             try:
                 with open(self.file_path, 'r') as f:
                     self.sections = []
                     # Try to read the file
                     try:
                         data = f.read()
                     except Exception as e:
                         self.read_error = f"Couldn't read file: {str(e)}"
                         return
-                    
+
                     # If it read correctly try to extract the version
                     try:
                         self.version = get_version_section(data)
                         self.version_num = self.version.version_num
                         self.delimiter = self.version.delimiter
                         self.sections.append(self.version)
-                    # If a version couldn't be extracted, and the user 
-                    # has decided to always try to split the sections 
-                    # anyway set the version to None otherwise return 
+                    # If a version couldn't be extracted, and the user
+                    # has decided to always try to split the sections
+                    # anyway set the version to None otherwise return
                     # the LASFile object
                     except Exception as e:
                         self.version_error = f"Couldn't get version: {str(e)}"
                         tb = traceback.format_exc()
                         self.version_tb = f"Couldn't get version: {tb}"
                         if always_try_split:
                             self.version_num = None
                         else:
                             return
-                    
+
                     # Try to split the file into sections
-                    if self.version_num != None and self.version_num != '':
-                        s = split_sections(data,self.version_num)
+                    if self.version_num is not None and self.version_num != '':
+                        s = split_sections(data, self.version_num)
                         if (
-                            s['version'] != '' and s['version'] != None and 
-                            s['well'] != '' and s['well'] != None
+                            s['version'] != '' and s['version'] is not None and
+                            s['well'] != '' and s['well'] is not None
                         ):
-                                sections_dict = s
+                            sections_dict = s
                         else:
                             self.split_error = (
                                 "Couldn't split into minimum required "
-                                "sections: Version and well sections are empty."
+                                "sections: Version and well sections "
+                                "are empty."
                             )
                             if not always_try_split:
                                 return
                     elif always_try_split:
                         try:
-                            s = split_sections(data,'2.0')
+                            s = split_sections(data, '2.0')
                             if (
-                                s['version'] != '' and s['version'] != None and 
-                                s['well'] != '' and s['well'] != None
+                                s['version'] != '' and s['version'] is not None
+                                and
+                                s['well'] != '' and s['well'] is not None
                             ):
                                 sections_dict = s
                             else:
                                 raise Exception(
                                     "Tried version 2.0 split, but version and "
                                     "well sections are still empty"
                                     )
                         except Exception as e:
-                            s = split_sections(data,'3.0')
+                            s = split_sections(data, '3.0')
                             if (
-                                s['version'] != '' and s['version'] != None and 
-                                s['well'] != '' and s['well'] != None
+                                s['version'] != '' and s['version'] is not None
+                                and
+                                s['well'] != '' and s['well'] is not None
                             ):
                                 sections_dict = s
                             else:
                                 self.split_error = (
                                     f"Couldn't split into minimum required "
                                     f"sections: {str(e)}"
                                 )
                                 return
-                    
-                    # If it split correctly generate las section items 
+
+                    # If it split correctly generate las section items
                     # from the strings
                     try:
-                        for name,raw_data in sections_dict.items():
+                        for name, raw_data in sections_dict.items():
                             header_section_names = [
                                 'version',
                                 'well',
                                 'parameters',
                                 'curves',
                                 'core_parameters',
                                 'core_definition',
@@ -1683,16 +1875,16 @@
                                 'test_parameters',
                                 'test_definition'
                             ]
                             data_section_names = ['data']
                             if name == 'version':
                                 continue
                             if (
-                                name in header_section_names or 
-                                '_parameters' in name or 
+                                name in header_section_names or
+                                '_parameters' in name or
                                 '_definition' in name
                             ):
                                 section_type = 'header'
                             elif name in data_section_names or '_data' in name:
                                 section_type = 'data'
                             else:
                                 section_type = ''
@@ -1700,25 +1892,25 @@
                                 name,
                                 raw_data,
                                 section_type,
                                 self.version_num,
                                 )
                             self.sections.append(section)
                         for section in self.sections:
-                            setattr(self,section.name,section)
+                            setattr(self, section.name, section)
                     except Exception as e:
                         self.section_load_error = (
                             f"Sections failed to load: {str(e)}"
                         )
                         self.sections_dict = sections_dict
                         tb = traceback.format_exc()
                         self.section_load_tb = f"Sections failed to load: {tb}"
                         return
-                    
-                    # If sections were built correctly, insure 
+
+                    # If sections were built correctly, insure
                     # congruency between definition and data sections
                     self.validate_defs_and_data()
             except FileNotFoundError:
                 self.open_error = f"File not found: {self.file_path}"
                 tb = traceback.format_exc()
                 self.open_tb = f"File not found: {tb}"
                 return
```

### Comparing `lasfile-0.1.8/tests/tests.py` & `lasfile-0.1.9/tests/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 import os
 import glob
 from src.lasfile import LASFile
 
+
 def get_test_las_paths():
     """Gets a list of las files in the test folder"""
-    return glob.glob(os.path.join(os.path.dirname(__file__),'*.las'))
+    return glob.glob(os.path.join(os.path.dirname(__file__), '*.las'))
+
 
 # Dictionary of file name tags to version numbers
 version_dict = {
     '1_2': '1.2',
     '2_0': '2.0',
     '3_0': '3.0'
 }
 
+
 def test_read_las():
     """Tests that las files can be read"""
     for las_path in get_test_las_paths():
         # Get the version number from the file name
         for tag, ver in version_dict.items():
             if tag in las_path:
                 version = ver
         # Test that the file can be read
         las = LASFile(file_path=las_path)
         assert las is not None
-        # Test that the version section is present, the version 
-        # number is correct, and that there are no errors in 
+        # Test that the version section is present, the version
+        # number is correct, and that there are no errors in
         # parsing or validating the version section
         assert 'version_error' not in vars(las).keys()
         assert 'version_tb' not in vars(las).keys()
         assert las.version is not None
         assert las.version_num == version
+        assert las.version.validated
         # Test that the well section is present, and that there are
         # no errors in parsing or validating the well section
         assert las.well is not None
         assert 'parse_error' not in vars(las.well).keys()
         assert 'validate_error' not in vars(las.well).keys()
         if version == '1.2' or version == '2.0':
-            # Test that the curves section is present, and that 
-            # there are no errors in parsing or validating the 
+            # Test that the curves section is present, and that
+            # there are no errors in parsing or validating the
             # curves section
             assert las.curves is not None
             assert 'parse_error' not in vars(las.curves).keys()
             assert 'validate_error' not in vars(las.curves).keys()
-            # Test that the data section is present, and that there 
-            # are no errors in parsing or validating the data 
+            # Test that the data section is present, and that there
+            # are no errors in parsing or validating the data
             # section
             assert las.data is not None
             assert 'parse_error' not in vars(las.data).keys()
             assert 'validate_error' not in vars(las.data).keys()
         elif version == '3.0':
             # Test that all sections present have no errors in
             # parsing or validating
             for section in las.sections:
                 assert 'parse_error' not in vars(section).keys()
                 assert 'validate_error' not in vars(section).keys()
 
+
 test_read_las()
```

