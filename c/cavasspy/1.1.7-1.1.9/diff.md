# Comparing `tmp/cavasspy-1.1.7.tar.gz` & `tmp/cavasspy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cavasspy-1.1.7.tar", last modified: Thu Apr 20 08:22:50 2023, max compression
+gzip compressed data, was "cavasspy-1.1.9.tar", last modified: Fri Jun 30 12:37:29 2023, max compression
```

## Comparing `cavasspy-1.1.7.tar` & `cavasspy-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:22:50.214810 cavasspy-1.1.7/
--rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 cavasspy-1.1.7/LICENSE
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 08:22:50.214538 cavasspy-1.1.7/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)      438 2022-08-03 14:11:17.000000 cavasspy-1.1.7/README.md
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:22:50.211305 cavasspy-1.1.7/cavasspy/
--rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-03 11:45:14.000000 cavasspy-1.1.7/cavasspy/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     1045 2023-04-20 08:22:18.000000 cavasspy-1.1.7/cavasspy/converter.py
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 01:40:19.000000 cavasspy-1.1.7/cavasspy/match.py
--rw-r--r--   0 daijian    (501) staff       (20)     5346 2023-04-20 08:22:05.000000 cavasspy-1.1.7/cavasspy/op.py
--rw-r--r--   0 daijian    (501) staff       (20)      552 2022-09-01 11:35:28.000000 cavasspy-1.1.7/cavasspy/window_transform.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-04-20 08:22:50.213938 cavasspy-1.1.7/cavasspy.egg-info/
--rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 08:22:49.000000 cavasspy-1.1.7/cavasspy.egg-info/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)      290 2023-04-20 08:22:50.000000 cavasspy-1.1.7/cavasspy.egg-info/SOURCES.txt
--rw-r--r--   0 daijian    (501) staff       (20)        1 2023-04-20 08:22:49.000000 cavasspy-1.1.7/cavasspy.egg-info/dependency_links.txt
--rw-r--r--   0 daijian    (501) staff       (20)       16 2023-04-20 08:22:49.000000 cavasspy-1.1.7/cavasspy.egg-info/requires.txt
--rw-r--r--   0 daijian    (501) staff       (20)        9 2023-04-20 08:22:49.000000 cavasspy-1.1.7/cavasspy.egg-info/top_level.txt
--rw-r--r--   0 daijian    (501) staff       (20)       38 2023-04-20 08:22:50.214895 cavasspy-1.1.7/setup.cfg
--rw-r--r--   0 daijian    (501) staff       (20)      672 2023-04-20 08:22:46.000000 cavasspy-1.1.7/setup.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-06-30 12:37:29.076416 cavasspy-1.1.9/
+-rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 cavasspy-1.1.9/LICENSE
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-06-30 12:37:29.076014 cavasspy-1.1.9/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)      438 2022-08-03 14:11:17.000000 cavasspy-1.1.9/README.md
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-06-30 12:37:29.072479 cavasspy-1.1.9/cavasspy/
+-rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-03 11:45:14.000000 cavasspy-1.1.9/cavasspy/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1029 2023-06-30 12:37:11.000000 cavasspy-1.1.9/cavasspy/converter.py
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-04-20 01:40:19.000000 cavasspy-1.1.9/cavasspy/match.py
+-rw-r--r--   0 daijian    (501) staff       (20)     5355 2023-04-20 08:27:06.000000 cavasspy-1.1.9/cavasspy/op.py
+-rw-r--r--   0 daijian    (501) staff       (20)      861 2023-04-20 08:22:05.000000 cavasspy-1.1.9/cavasspy/sys_helper.py
+-rw-r--r--   0 daijian    (501) staff       (20)      552 2022-09-01 11:35:28.000000 cavasspy-1.1.9/cavasspy/window_transform.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2023-06-30 12:37:29.075355 cavasspy-1.1.9/cavasspy.egg-info/
+-rw-r--r--   0 daijian    (501) staff       (20)      837 2023-06-30 12:37:27.000000 cavasspy-1.1.9/cavasspy.egg-info/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)      313 2023-06-30 12:37:28.000000 cavasspy-1.1.9/cavasspy.egg-info/SOURCES.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        1 2023-06-30 12:37:28.000000 cavasspy-1.1.9/cavasspy.egg-info/dependency_links.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       16 2023-06-30 12:37:28.000000 cavasspy-1.1.9/cavasspy.egg-info/requires.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        9 2023-06-30 12:37:28.000000 cavasspy-1.1.9/cavasspy.egg-info/top_level.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       38 2023-06-30 12:37:29.076571 cavasspy-1.1.9/setup.cfg
+-rw-r--r--   0 daijian    (501) staff       (20)      672 2023-04-26 13:31:11.000000 cavasspy-1.1.9/setup.py
```

### Comparing `cavasspy-1.1.7/LICENSE` & `cavasspy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.7/PKG-INFO` & `cavasspy-1.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavasspy
-Version: 1.1.7
+Version: 1.1.9
 Summary: CAVASS python APIs.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
```

### Comparing `cavasspy-1.1.7/cavasspy/converter.py` & `cavasspy-1.1.9/cavasspy/converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import os
 import shutil
 from uuid import uuid4
 
-from sys_helper import execute_cmd
+from cavasspy.sys_helper import execute_cmd
 
 
 def nifti2dicom(input_file, output_dir, accession_number=1):
     """
     Require nifti2dicom.
     sudo apt install nifti2dicom
     https://github.com/biolab-unige/nifti2dicom
     """
     cmd = f'nifti2dicom -i {input_file} -o {output_dir} -a {accession_number}'
     result = os.popen(cmd)
     return result.readlines()
 
 
-def dicom2cavass(input_dir, output_file):
-    execute_cmd(f'from_dicom {input_dir}/* {output_file}')
+def dicom2cavass(input_dir, output_file, add_value=0):
+    """
+    Note that if the output file path is too long, this command may be failed.
+    """
+    r = execute_cmd(f'from_dicom {input_dir}/* {output_file} +{add_value}')
+    return r
 
 
-def nifti2cavass(input_file, output_file, dicom_accession_number=1):
+def nifti2cavass(input_file, output_file, add_value=1024, dicom_accession_number=1):
     save_path = os.path.split(output_file)[0]
     tmp_dicom_dir = os.path.join(save_path, f'{uuid4()}')
-    result = nifti2dicom(input_file, tmp_dicom_dir, dicom_accession_number)
-    dicom2cavass(tmp_dicom_dir, output_file)
+    r1 = nifti2dicom(input_file, tmp_dicom_dir, dicom_accession_number)
+    r2 = dicom2cavass(tmp_dicom_dir, output_file, add_value)
     shutil.rmtree(tmp_dicom_dir)
-    return result
-
-
-if __name__ == '__main__':
-    r = nifti2cavass('/home/ubuntu/sda1.8T/Dataset/AMOS/AMOS22/imagesTr/amos_0086.nii.gz',
-                 '/home/ubuntu/sdb1.8T/dj/amos_0086.IM0')
-    print(r)
+    return r1, r2
```

### Comparing `cavasspy-1.1.7/cavasspy/match.py` & `cavasspy-1.1.9/cavasspy/match.py`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.7/cavasspy/op.py` & `cavasspy-1.1.9/cavasspy/op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import uuid
 from typing import Optional, Iterable
 
 from hammer.io import read_mat, save_mat
 
-from sys_helper import execute_cmd
+from cavasspy.sys_helper import execute_cmd
 
 
 class CAVASSPyError(Exception):
     ...
 
 
 def get_ct_resolution(input_file):
```

### Comparing `cavasspy-1.1.7/cavasspy/window_transform.py` & `cavasspy-1.1.9/cavasspy/window_transform.py`

 * *Files identical despite different names*

### Comparing `cavasspy-1.1.7/cavasspy.egg-info/PKG-INFO` & `cavasspy-1.1.9/cavasspy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cavasspy
-Version: 1.1.7
+Version: 1.1.9
 Summary: CAVASS python APIs.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
```

### Comparing `cavasspy-1.1.7/setup.py` & `cavasspy-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cavasspy',
-    version='1.1.7',
+    version='1.1.9',
     author='Dai Jian',
     author_email='daijian@stumail.ysu.edu.cn',
     description='CAVASS python APIs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
```

