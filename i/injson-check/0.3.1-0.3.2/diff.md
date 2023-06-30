# Comparing `tmp/injson_check-0.3.1.tar.gz` & `tmp/injson_check-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\injson_check-0.3.1.tar", last modified: Wed May 24 05:54:41 2023, max compression
+gzip compressed data, was "dist\injson_check-0.3.2.tar", last modified: Fri Jun 30 11:56:47 2023, max compression
```

## Comparing `injson_check-0.3.1.tar` & `injson_check-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 05:54:41.000000 injson_check-0.3.1/
--rw-rw-rw-   0        0        0       48 2023-05-24 05:54:30.000000 injson_check-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      333 2023-05-24 05:54:41.000000 injson_check-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check/
--rw-rw-rw-   0        0        0     1160 2023-05-24 05:50:35.000000 injson_check-0.3.1/injson_check/__init__.py
--rw-rw-rw-   0        0        0    20628 2023-05-24 05:50:40.000000 injson_check-0.3.1/injson_check/injson_check.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-05-19 12:18:31.000000 injson_check-0.3.1/injson_check/pytransform/__init__.py
--rw-rw-rw-   0        0        0  1373198 2023-05-24 05:48:57.000000 injson_check-0.3.1/injson_check/pytransform/_pytransform.dll
-drwxrwxrwx   0        0        0        0 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check.egg-info/
--rw-rw-rw-   0        0        0      333 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-24 05:54:41.000000 injson_check-0.3.1/injson_check.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 05:54:41.000000 injson_check-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1183 2023-05-24 05:51:37.000000 injson_check-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:56:47.000000 injson_check-0.3.2/
+-rw-rw-rw-   0        0        0       48 2023-05-24 05:54:30.000000 injson_check-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      333 2023-06-30 11:56:47.000000 injson_check-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check/
+-rw-rw-rw-   0        0        0     1160 2023-05-24 05:50:35.000000 injson_check-0.3.2/injson_check/__init__.py
+-rw-rw-rw-   0        0        0   111127 2023-06-30 11:56:05.000000 injson_check-0.3.2/injson_check/abs.py
+-rw-rw-rw-   0        0        0    20628 2023-05-24 05:50:40.000000 injson_check-0.3.2/injson_check/injson_check.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-05-19 12:18:31.000000 injson_check-0.3.2/injson_check/pytransform/__init__.py
+-rw-rw-rw-   0        0        0  1373198 2023-05-24 05:48:57.000000 injson_check-0.3.2/injson_check/pytransform/_pytransform.dll
+drwxrwxrwx   0        0        0        0 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check.egg-info/
+-rw-rw-rw-   0        0        0      333 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-30 11:56:47.000000 injson_check-0.3.2/injson_check.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 11:56:47.000000 injson_check-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1183 2023-06-30 11:50:57.000000 injson_check-0.3.2/setup.py
```

### Comparing `injson_check-0.3.1/injson_check/__init__.py` & `injson_check-0.3.2/injson_check/__init__.py`

 * *Files identical despite different names*

### Comparing `injson_check-0.3.1/injson_check/injson_check.py` & `injson_check-0.3.2/injson_check/injson_check.py`

 * *Files identical despite different names*

### Comparing `injson_check-0.3.1/injson_check/pytransform/__init__.py` & `injson_check-0.3.2/injson_check/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `injson_check-0.3.1/injson_check/pytransform/_pytransform.dll` & `injson_check-0.3.2/injson_check/pytransform/_pytransform.dll`

 * *Files identical despite different names*

### Comparing `injson_check-0.3.1/setup.py` & `injson_check-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @Auther:sahala
 
 import os
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 setup(
     name="injson_check",  # 这里是pip项目发布的名称
-    version="0.3.1",  # 版本号，数值大的会优先被pip
+    version="0.3.2",  # 版本号，数值大的会优先被pip
     keywords=["pip", "injson_check", "featureextraction"],
     description="数据校验器：injson同版本替代 可正常使用",
     long_description="数据校验器：injson同版本替代",
     license="MIT Licence",
 
     url="https://github.com/",  # 项目相关文件地址，一般是github
     author="liyubin",
```

