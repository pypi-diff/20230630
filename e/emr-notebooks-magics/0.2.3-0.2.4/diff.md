# Comparing `tmp/emr-notebooks-magics-0.2.3.tar.gz` & `tmp/emr-notebooks-magics-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emr-notebooks-magics-0.2.3.tar", last modified: Tue Jan 31 17:21:57 2023, max compression
+gzip compressed data, was "emr-notebooks-magics-0.2.4.tar", last modified: Fri Jun 30 19:20:25 2023, max compression
```

## Comparing `emr-notebooks-magics-0.2.3.tar` & `emr-notebooks-magics-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-01-31 17:21:57.448271 emr-notebooks-magics-0.2.3/
--rw-r--r--   0 npalania   (504) staff       (20)    10142 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.3/LICENSE
--rw-r--r--   0 npalania   (504) staff       (20)       67 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.3/NOTICE
--rw-r--r--   0 npalania   (504) staff       (20)     4816 2023-01-31 17:21:57.448339 emr-notebooks-magics-0.2.3/PKG-INFO
--rw-r--r--   0 npalania   (504) staff       (20)     4360 2023-01-31 17:16:02.000000 emr-notebooks-magics-0.2.3/README.md
-drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-01-31 17:21:57.446322 emr-notebooks-magics-0.2.3/emr_notebooks_magics/
--rw-r--r--   0 npalania   (504) staff       (20)      780 2023-01-26 23:33:00.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/__init__.py
--rw-r--r--   0 npalania   (504) staff       (20)     5665 2023-01-31 17:03:33.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/execute_emr_notebook.py
--rw-r--r--   0 npalania   (504) staff       (20)     4185 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/generate_s3_presigned_url.py
--rw-r--r--   0 npalania   (504) staff       (20)     8642 2022-12-06 16:41:11.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/mount_workspace_dir.py
-drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-01-31 17:21:57.447825 emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/
--rw-r--r--   0 npalania   (504) staff       (20)        0 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/__init__.py
--rw-r--r--   0 npalania   (504) staff       (20)      703 2023-01-31 17:03:33.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/display_utils.py
--rw-r--r--   0 npalania   (504) staff       (20)     1421 2023-01-26 23:32:27.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/instance_metadata_service_utils.py
--rw-r--r--   0 npalania   (504) staff       (20)      699 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/str_utils.py
-drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-01-31 17:21:57.447100 emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/
--rw-r--r--   0 npalania   (504) staff       (20)     4816 2023-01-31 17:21:57.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/PKG-INFO
--rw-r--r--   0 npalania   (504) staff       (20)      667 2023-01-31 17:21:57.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/SOURCES.txt
--rw-r--r--   0 npalania   (504) staff       (20)        1 2023-01-31 17:21:57.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/dependency_links.txt
--rw-r--r--   0 npalania   (504) staff       (20)        6 2023-01-31 17:21:57.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/requires.txt
--rw-r--r--   0 npalania   (504) staff       (20)       21 2023-01-31 17:21:57.000000 emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/top_level.txt
--rw-r--r--   0 npalania   (504) staff       (20)       79 2023-01-31 17:21:57.448566 emr-notebooks-magics-0.2.3/setup.cfg
--rw-r--r--   0 npalania   (504) staff       (20)      930 2023-01-31 17:21:50.000000 emr-notebooks-magics-0.2.3/setup.py
-drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-01-31 17:21:57.448018 emr-notebooks-magics-0.2.3/startup_script/
--rw-r--r--   0 npalania   (504) staff       (20)     1184 2023-01-26 23:34:08.000000 emr-notebooks-magics-0.2.3/startup_script/001-setup-emr-notebook-magics.py
+drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-06-30 19:20:25.380069 emr-notebooks-magics-0.2.4/
+-rw-r--r--   0 npalania   (504) staff       (20)    10142 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.4/LICENSE
+-rw-r--r--   0 npalania   (504) staff       (20)       67 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.4/NOTICE
+-rw-r--r--   0 npalania   (504) staff       (20)     4816 2023-06-30 19:20:25.380137 emr-notebooks-magics-0.2.4/PKG-INFO
+-rw-r--r--   0 npalania   (504) staff       (20)     4360 2023-01-31 17:16:02.000000 emr-notebooks-magics-0.2.4/README.md
+drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-06-30 19:20:25.377935 emr-notebooks-magics-0.2.4/emr_notebooks_magics/
+-rw-r--r--   0 npalania   (504) staff       (20)      780 2023-01-26 23:33:00.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/__init__.py
+-rw-r--r--   0 npalania   (504) staff       (20)     5665 2023-01-31 17:03:33.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/execute_emr_notebook.py
+-rw-r--r--   0 npalania   (504) staff       (20)     4185 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/generate_s3_presigned_url.py
+-rw-r--r--   0 npalania   (504) staff       (20)     8753 2023-06-30 19:19:29.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/mount_workspace_dir.py
+drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-06-30 19:20:25.379636 emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/
+-rw-r--r--   0 npalania   (504) staff       (20)        0 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/__init__.py
+-rw-r--r--   0 npalania   (504) staff       (20)      703 2023-01-31 17:03:33.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/display_utils.py
+-rw-r--r--   0 npalania   (504) staff       (20)     1421 2023-01-26 23:32:27.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/instance_metadata_service_utils.py
+-rw-r--r--   0 npalania   (504) staff       (20)      699 2022-12-06 16:40:00.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/str_utils.py
+drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-06-30 19:20:25.378833 emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/
+-rw-r--r--   0 npalania   (504) staff       (20)     4816 2023-06-30 19:20:25.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/PKG-INFO
+-rw-r--r--   0 npalania   (504) staff       (20)      667 2023-06-30 19:20:25.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/SOURCES.txt
+-rw-r--r--   0 npalania   (504) staff       (20)        1 2023-06-30 19:20:25.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/dependency_links.txt
+-rw-r--r--   0 npalania   (504) staff       (20)        6 2023-06-30 19:20:25.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/requires.txt
+-rw-r--r--   0 npalania   (504) staff       (20)       21 2023-06-30 19:20:25.000000 emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/top_level.txt
+-rw-r--r--   0 npalania   (504) staff       (20)       79 2023-06-30 19:20:25.380387 emr-notebooks-magics-0.2.4/setup.cfg
+-rw-r--r--   0 npalania   (504) staff       (20)      930 2023-06-30 19:20:03.000000 emr-notebooks-magics-0.2.4/setup.py
+drwxr-xr-x   0 npalania   (504) staff       (20)        0 2023-06-30 19:20:25.379816 emr-notebooks-magics-0.2.4/startup_script/
+-rw-r--r--   0 npalania   (504) staff       (20)     1184 2023-01-26 23:34:08.000000 emr-notebooks-magics-0.2.4/startup_script/001-setup-emr-notebook-magics.py
```

### Comparing `emr-notebooks-magics-0.2.3/LICENSE` & `emr-notebooks-magics-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/PKG-INFO` & `emr-notebooks-magics-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-notebooks-magics
-Version: 0.2.3
+Version: 0.2.4
 Summary: Jupyter Magics for EMR Notebooks.
 Author-email: emrnotebooks@amazon.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `emr-notebooks-magics-0.2.3/README.md` & `emr-notebooks-magics-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/__init__.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/execute_emr_notebook.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/execute_emr_notebook.py`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/generate_s3_presigned_url.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/generate_s3_presigned_url.py`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/mount_workspace_dir.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/mount_workspace_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,16 @@
         # use default iam role
         if "iam_role" not in mount_params:
             mount_params = "-o iam_role=auto " + mount_params
      
         # readonly mount by default
         if read_only and "umask" not in mount_params:
             mount_params = "-o umask=277 " + mount_params
+        if "notsup_compat_dir" not in mount_params:
+            mount_params = "-o compat_dir " + mount_params
 
         # mount the directory as the current user
         if "uid" not in mount_params:
             mount_params = "-o uid={} ".format(os.getuid()) + mount_params
 
         if "gid" not in mount_params:
             mount_params = "-o gid={} ".format(os.getgid()) + mount_params
```

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/display_utils.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/display_utils.py`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/instance_metadata_service_utils.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/instance_metadata_service_utils.py`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics/utils/str_utils.py` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/PKG-INFO` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-notebooks-magics
-Version: 0.2.3
+Version: 0.2.4
 Summary: Jupyter Magics for EMR Notebooks.
 Author-email: emrnotebooks@amazon.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `emr-notebooks-magics-0.2.3/emr_notebooks_magics.egg-info/SOURCES.txt` & `emr-notebooks-magics-0.2.4/emr_notebooks_magics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emr-notebooks-magics-0.2.3/setup.py` & `emr-notebooks-magics-0.2.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages
 from shutil import copy
 from pathlib import Path
 
 setup(
     name="emr-notebooks-magics",
-    version="0.2.3",
+    version="0.2.4",
     description="Jupyter Magics for EMR Notebooks.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=["emr_notebooks_magics", "emr_notebooks_magics.utils"],
     install_requires=[
           'boto3',
     ],
```

### Comparing `emr-notebooks-magics-0.2.3/startup_script/001-setup-emr-notebook-magics.py` & `emr-notebooks-magics-0.2.4/startup_script/001-setup-emr-notebook-magics.py`

 * *Files identical despite different names*

