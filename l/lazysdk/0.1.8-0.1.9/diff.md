# Comparing `tmp/lazysdk-0.1.8.tar.gz` & `tmp/lazysdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.8.tar", last modified: Fri Jun  9 08:48:55 2023, max compression
+gzip compressed data, was "lazysdk-0.1.9.tar", last modified: Fri Jun  9 10:27:00 2023, max compression
```

## Comparing `lazysdk-0.1.8.tar` & `lazysdk-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 08:48:55.782142 lazysdk-0.1.8/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-09 08:48:55.781995 lazysdk-0.1.8/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.8/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 08:48:55.781134 lazysdk-0.1.8/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.8/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.8/lazysdk/lazyCrypto.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.8/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.8/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    31932 2023-06-09 08:48:32.000000 lazysdk-0.1.8/lazysdk/lazym3u8.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5159 2023-06-07 09:23:18.000000 lazysdk-0.1.8/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.8/lazysdk/lazywebhook.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 08:48:55.781822 lazysdk-0.1.8/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-09 08:48:55.000000 lazysdk-0.1.8/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-09 08:48:55.000000 lazysdk-0.1.8/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-09 08:48:55.000000 lazysdk-0.1.8/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-09 08:48:55.000000 lazysdk-0.1.8/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-09 08:48:55.000000 lazysdk-0.1.8/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-09 08:48:55.782197 lazysdk-0.1.8/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-09 08:48:32.000000 lazysdk-0.1.8/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 10:27:00.415120 lazysdk-0.1.9/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-09 10:27:00.415009 lazysdk-0.1.9/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.9/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 10:27:00.414218 lazysdk-0.1.9/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.9/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.9/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.9/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.9/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    31954 2023-06-09 10:26:14.000000 lazysdk-0.1.9/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5159 2023-06-07 09:23:18.000000 lazysdk-0.1.9/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazywebhook.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 10:27:00.414833 lazysdk-0.1.9/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-09 10:27:00.415159 lazysdk-0.1.9/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-09 10:26:14.000000 lazysdk-0.1.9/setup.py
```

### Comparing `lazysdk-0.1.8/PKG-INFO` & `lazysdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.8/README.md` & `lazysdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazybase64.py` & `lazysdk-0.1.9/lazysdk/lazybase64.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazydict.py` & `lazysdk-0.1.9/lazysdk/lazydict.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyenv.py` & `lazysdk-0.1.9/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyexcel.py` & `lazysdk-0.1.9/lazysdk/lazyexcel.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyfile.py` & `lazysdk-0.1.9/lazysdk/lazyfile.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyflask.py` & `lazysdk-0.1.9/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyid.py` & `lazysdk-0.1.9/lazysdk/lazyid.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazym3u8.py` & `lazysdk-0.1.9/lazysdk/lazym3u8.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,16 @@
         )
         fragment_file_name = '%s%s%s.%s' % (fragment_path, path_separator, url_index, fragment_suffix)  # 生成碎片文件名
         fragment_file_name_list.append(fragment_file_name)
 
     lazyprocess.run(
         task_list=task_list,
         task_function=download_fragment_single,
-        subprocess_limit=subprocess_limit
+        subprocess_limit=subprocess_limit,
+        silence=True
     )
 
     download_res = {
         'fragment_path': fragment_path,
         'fragment_suffix': fragment_suffix,
         'fragment_file_name_list': fragment_file_name_list
     }
```

### Comparing `lazysdk-0.1.8/lazysdk/lazymd5.py` & `lazysdk-0.1.9/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazypath.py` & `lazysdk-0.1.9/lazysdk/lazypath.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyprocess.py` & `lazysdk-0.1.9/lazysdk/lazyprocess.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyproxies.py` & `lazysdk-0.1.9/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyrandom.py` & `lazysdk-0.1.9/lazysdk/lazyrandom.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyredis.py` & `lazysdk-0.1.9/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyrequests.py` & `lazysdk-0.1.9/lazysdk/lazyrequests.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazytext.py` & `lazysdk-0.1.9/lazysdk/lazytext.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazytime.py` & `lazysdk-0.1.9/lazysdk/lazytime.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazyua.py` & `lazysdk-0.1.9/lazysdk/lazyua.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk/lazywebhook.py` & `lazysdk-0.1.9/lazysdk/lazywebhook.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/lazysdk.egg-info/PKG-INFO` & `lazysdk-0.1.9/lazysdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.8/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.9/lazysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.8/setup.py` & `lazysdk-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.8",
+    version="0.1.9",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
```

