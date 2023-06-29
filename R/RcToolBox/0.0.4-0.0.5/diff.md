# Comparing `tmp/RcToolBox-0.0.4.tar.gz` & `tmp/RcToolBox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RcToolBox-0.0.4.tar", last modified: Sat May 27 09:17:49 2023, max compression
+gzip compressed data, was "RcToolBox-0.0.5.tar", last modified: Thu Jun 29 23:23:51 2023, max compression
```

## Comparing `RcToolBox-0.0.4.tar` & `RcToolBox-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.552139 RcToolBox-0.0.4/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-05-27 09:17:49.550529 RcToolBox-0.0.4/PKG-INFO
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.507301 RcToolBox-0.0.4/RcToolBox/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-03-07 20:28:07.000000 RcToolBox-0.0.4/RcToolBox/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4075 2023-05-27 09:09:01.000000 RcToolBox-0.0.4/RcToolBox/basic_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     6635 2023-04-09 10:46:20.000000 RcToolBox-0.0.4/RcToolBox/dataset_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.534760 RcToolBox-0.0.4/RcToolBox/draw/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:14.000000 RcToolBox-0.0.4/RcToolBox/draw/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2614 2023-04-09 10:09:08.000000 RcToolBox-0.0.4/RcToolBox/draw/df_plot.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3737 2023-04-06 22:20:13.000000 RcToolBox-0.0.4/RcToolBox/nifti_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4412 2023-04-01 22:32:30.000000 RcToolBox-0.0.4/RcToolBox/pandas_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.546235 RcToolBox-0.0.4/RcToolBox/segmentation/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:02.000000 RcToolBox-0.0.4/RcToolBox/segmentation/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2802 2023-04-17 23:00:58.000000 RcToolBox-0.0.4/RcToolBox/segmentation/evaluation.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     1718 2023-05-26 19:08:31.000000 RcToolBox-0.0.4/RcToolBox/segmentation/metric.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      928 2023-04-09 10:06:45.000000 RcToolBox-0.0.4/RcToolBox/xeon_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-05-27 09:17:49.526865 RcToolBox-0.0.4/RcToolBox.egg-info/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/PKG-INFO
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      464 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/SOURCES.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        1 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/dependency_links.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       68 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/requires.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       10 2023-05-27 09:17:49.000000 RcToolBox-0.0.4/RcToolBox.egg-info/top_level.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       38 2023-05-27 09:17:49.553180 RcToolBox-0.0.4/setup.cfg
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      840 2023-05-27 09:11:03.000000 RcToolBox-0.0.4/setup.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-06-29 23:23:51.850986 RcToolBox-0.0.5/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-06-29 23:23:51.849364 RcToolBox-0.0.5/PKG-INFO
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-06-29 23:23:51.800970 RcToolBox-0.0.5/RcToolBox/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-03-07 20:28:07.000000 RcToolBox-0.0.5/RcToolBox/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3690 2023-06-15 12:52:10.000000 RcToolBox-0.0.5/RcToolBox/basic_op.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     6635 2023-04-09 10:46:20.000000 RcToolBox-0.0.5/RcToolBox/dataset_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-06-29 23:23:51.830811 RcToolBox-0.0.5/RcToolBox/draw/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:14.000000 RcToolBox-0.0.5/RcToolBox/draw/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2614 2023-04-09 10:09:08.000000 RcToolBox-0.0.5/RcToolBox/draw/df_plot.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3737 2023-04-06 22:20:13.000000 RcToolBox-0.0.5/RcToolBox/nifti_op.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4412 2023-04-01 22:32:30.000000 RcToolBox-0.0.5/RcToolBox/pandas_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-06-29 23:23:51.844372 RcToolBox-0.0.5/RcToolBox/segmentation/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:02.000000 RcToolBox-0.0.5/RcToolBox/segmentation/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2802 2023-04-17 23:00:58.000000 RcToolBox-0.0.5/RcToolBox/segmentation/evaluation.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     1718 2023-05-26 19:08:31.000000 RcToolBox-0.0.5/RcToolBox/segmentation/metric.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      928 2023-04-09 10:06:45.000000 RcToolBox-0.0.5/RcToolBox/xeon_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-06-29 23:23:51.822377 RcToolBox-0.0.5/RcToolBox.egg-info/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-06-29 23:23:51.000000 RcToolBox-0.0.5/RcToolBox.egg-info/PKG-INFO
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      464 2023-06-29 23:23:51.000000 RcToolBox-0.0.5/RcToolBox.egg-info/SOURCES.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        1 2023-06-29 23:23:51.000000 RcToolBox-0.0.5/RcToolBox.egg-info/dependency_links.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       68 2023-06-29 23:23:51.000000 RcToolBox-0.0.5/RcToolBox.egg-info/requires.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       10 2023-06-29 23:23:51.000000 RcToolBox-0.0.5/RcToolBox.egg-info/top_level.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       38 2023-06-29 23:23:51.852027 RcToolBox-0.0.5/setup.cfg
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      840 2023-06-29 23:19:25.000000 RcToolBox-0.0.5/setup.py
```

### Comparing `RcToolBox-0.0.4/RcToolBox/basic_op.py` & `RcToolBox-0.0.5/RcToolBox/basic_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,34 +5,14 @@
 import json
 import time
 import glob
 import shutil
 import sys
 """load and save file"""
 
-
-def add_parent_path(level=2):
-
-    if level == 2:
-        sys.path.append(
-            os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-    elif level == 3:
-        sys.path.append(
-            os.path.dirname(
-                os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
-
-    elif level == 4:
-        sys.path.append(
-            os.path.dirname(
-                os.path.dirname(
-                    os.path.dirname(os.path.dirname(
-                        os.path.abspath(__file__))))))
-
-
 def load_yaml(file):
     """
 
     :param file: yaml
     :return:
     """
     return yaml.load(open(file), Loader=yaml.FullLoader)
@@ -70,21 +50,25 @@
             filestream.append(line)
     return filestream
 
 
 """print with highlight"""
 
 
-def sprint(content, placeholder=40):
+def hprint(content, placeholder=40):
     if isinstance(content, str):
-        placeholder -= len(content)
-        left_placeholder = int(placeholder / 2)
-        right_placeholder = int(placeholder - left_placeholder)
-        print('\n' + '-' * left_placeholder + content +
-              '-' * right_placeholder)
+        
+        if len(content) > placeholder:
+            print(content)
+        else:
+            placeholder -= len(content)
+            left_placeholder = int(placeholder / 2)
+            right_placeholder = int(placeholder - left_placeholder)
+            print('\n' + '-' * left_placeholder + content +
+                '-' * right_placeholder)
     else:
         print('content should be str')
 
 
 """Timer"""
 
 
@@ -103,15 +87,17 @@
                                                    time_slot % 60))
     elif time_slot > 60:
         print('{} cost: {} min {} s'.format(program_name, int(time_slot // 60),
                                             int(time_slot % 60)))
     else:
         print('{} cost: {:.1f} s'.format(program_name, time_slot))
 
-
+    return time_slot
+    
+    
 """Date"""
 
 
 def get_date(detail=False):
     if detail:
         return time.strftime('%Y-%m-%d %H-%M-%S', time.localtime(time.time()))
     else:
@@ -130,15 +116,15 @@
         result_folder = join(os.environ["Server_Result"], project_name)
 
         os.makedirs(result_folder, exist_ok=False)
 
         if add_date:
             result_folder = join(result_folder, get_date())
 
-        sprint('Create Project Result folder')
+        hprint('Create Project Result folder')
         print('\n' + result_folder + '\n')
         
         if overwrite:
             print("be careful! we will delete {0}".format(result_folder))
             shutil.rmtree(result_folder, ignore_errors=True)
         
         os.makedirs(result_folder, exist_ok=False)
```

### Comparing `RcToolBox-0.0.4/RcToolBox/dataset_op.py` & `RcToolBox-0.0.5/RcToolBox/dataset_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/RcToolBox/draw/df_plot.py` & `RcToolBox-0.0.5/RcToolBox/draw/df_plot.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/RcToolBox/nifti_op.py` & `RcToolBox-0.0.5/RcToolBox/nifti_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/RcToolBox/pandas_op.py` & `RcToolBox-0.0.5/RcToolBox/pandas_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/RcToolBox/segmentation/evaluation.py` & `RcToolBox-0.0.5/RcToolBox/segmentation/evaluation.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/RcToolBox/segmentation/metric.py` & `RcToolBox-0.0.5/RcToolBox/segmentation/metric.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/RcToolBox/xeon_op.py` & `RcToolBox-0.0.5/RcToolBox/xeon_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.4/setup.py` & `RcToolBox-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages            
 
 setup(
     name = "RcToolBox",      # 这里是pip项目发布的名称
-    version = "0.0.4",  # 版本号，数值大的会优先被pip
+    version = "0.0.5",  # 版本号，数值大的会优先被pip
     keywords = ["pip", "RcToolBox"],			# 关键字
     description = "RC personal ToolBox",	# 描述
     long_description = "RC personal ToolBox",
     license = "MIT Licence",		# 许可证
 
     url = "",     #项目相关文件地址，一般是github项目地址即可
     author = "RC",			# 作者
```

