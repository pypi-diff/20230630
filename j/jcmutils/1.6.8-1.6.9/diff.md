# Comparing `tmp/jcmutils-1.6.8.tar.gz` & `tmp/jcmutils-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.6.8.tar", last modified: Fri Jun 30 02:22:45 2023, max compression
+gzip compressed data, was "jcmutils-1.6.9.tar", last modified: Fri Jun 30 02:25:56 2023, max compression
```

## Comparing `jcmutils-1.6.8.tar` & `jcmutils-1.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 02:22:45.957251 jcmutils-1.6.8/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.8/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-30 02:22:45.957251 jcmutils-1.6.8/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.8/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 02:22:45.957251 jcmutils-1.6.8/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.8/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    17686 2023-06-30 02:22:21.000000 jcmutils-1.6.8/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.8/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.8/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.8/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 02:22:45.957251 jcmutils-1.6.8/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-30 02:22:45.000000 jcmutils-1.6.8/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-30 02:22:45.000000 jcmutils-1.6.8/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-30 02:22:45.000000 jcmutils-1.6.8/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-30 02:22:45.000000 jcmutils-1.6.8/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-30 02:22:45.000000 jcmutils-1.6.8/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-30 02:22:45.957251 jcmutils-1.6.8/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-30 02:22:29.000000 jcmutils-1.6.8/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 02:25:56.187342 jcmutils-1.6.9/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.9/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-30 02:25:56.187342 jcmutils-1.6.9/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.9/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 02:25:56.187342 jcmutils-1.6.9/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.9/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    17686 2023-06-30 02:25:33.000000 jcmutils-1.6.9/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.9/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.9/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.9/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-30 02:25:56.187342 jcmutils-1.6.9/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-30 02:25:56.000000 jcmutils-1.6.9/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-30 02:25:56.000000 jcmutils-1.6.9/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-30 02:25:56.000000 jcmutils-1.6.9/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-30 02:25:56.000000 jcmutils-1.6.9/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-30 02:25:56.000000 jcmutils-1.6.9/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-30 02:25:56.187342 jcmutils-1.6.9/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-30 02:25:40.000000 jcmutils-1.6.9/setup.py
```

### Comparing `jcmutils-1.6.8/LICENSE` & `jcmutils-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.8/README.md` & `jcmutils-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.8/jcmutils/dataset_utils.py` & `jcmutils-1.6.9/jcmutils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         # 合并最终结果
         vmaxa = np.max(total_results) if vmax is None else vmax
         afield = (total_results/ vmaxa)*235
         afield = np.rot90(afield)
 
         (output_image,(xpos,ypos,width,height)) = self.__process_image(afield,template_image,signal_level)
         
-        lower_border = 1.1*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
-        lower_warn = 1.5*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
+        lower_border = 0.6*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
+        lower_warn = 1.0*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
         upper_warn = 2.0*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
         upper_border = 2.4*max(periodic_x,periodic_y)/source_density/max(output_image.shape[0],output_image.shape[1])
         # 大致检测结果正确性
         if width <=lower_border or height <=lower_border :
             logger.error(f"false mixed image detected,key-{self.origin_key} was detected too small width or height. the width is {width},height is {height},which is smaller than ({lower_border},{lower_border}) , try a smaller signal_level")
             raise Exception("error detected , please read log")
         if width <= lower_warn or height <=lower_warn:
```

### Comparing `jcmutils-1.6.8/jcmutils/gen_sources.py` & `jcmutils-1.6.9/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.8/jcmutils/logger.py` & `jcmutils-1.6.9/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.8/jcmutils/solver.py` & `jcmutils-1.6.9/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.8/setup.py` & `jcmutils-1.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.6.8'
+VERSION = '1.6.9'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

