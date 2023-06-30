# Comparing `tmp/tybase-0.1.6.tar.gz` & `tmp/tybase-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.1.6.tar", last modified: Sun Jun 18 14:22:13 2023, max compression
+gzip compressed data, was "tybase-0.1.7.tar", last modified: Fri Jun 30 10:18:11 2023, max compression
```

## Comparing `tybase-0.1.6.tar` & `tybase-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.569557 tybase-0.1.6/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.1.6/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      581 2023-06-18 14:22:13.569296 tybase-0.1.6/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      156 2023-05-08 08:46:36.000000 tybase-0.1.6/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-06-18 14:22:13.569717 tybase-0.1.6/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1018 2023-06-18 14:20:26.000000 tybase-0.1.6/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.559253 tybase-0.1.6/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.1.6/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.563283 tybase-0.1.6/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.1.6/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.1.6/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.1.6/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.565690 tybase-0.1.6/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.1.6/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.1.6/tybase/dbtool/data_import.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2206 2023-05-13 03:56:34.000000 tybase-0.1.6/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.566981 tybase-0.1.6/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.1.6/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.1.6/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.568613 tybase-0.1.6/tybase/tools/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.1.6/tybase/tools/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.1.6/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2052 2023-06-15 09:08:20.000000 tybase-0.1.6/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.1.6/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-18 14:22:13.562386 tybase-0.1.6/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      581 2023-06-18 14:22:13.000000 tybase-0.1.6/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      482 2023-06-18 14:22:13.000000 tybase-0.1.6/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-06-18 14:22:13.000000 tybase-0.1.6/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      130 2023-06-18 14:22:13.000000 tybase-0.1.6/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-06-18 14:22:13.000000 tybase-0.1.6/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.180682 tybase-0.1.7/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.1.7/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      785 2023-06-30 10:18:11.180529 tybase-0.1.7/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.1.7/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-06-30 10:18:11.180719 tybase-0.1.7/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1014 2023-06-30 10:17:15.000000 tybase-0.1.7/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.177293 tybase-0.1.7/tybase/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.1.7/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.178393 tybase-0.1.7/tybase/baidu/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.1.7/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.1.7/tybase/baidu/kw_tool.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.1.7/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.179077 tybase-0.1.7/tybase/dbtool/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.1.7/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.1.7/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.1.7/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.179416 tybase-0.1.7/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.1.7/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.1.7/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.180196 tybase-0.1.7/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.1.7/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.1.7/tybase/tools/qiniu_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2052 2023-06-15 09:08:20.000000 tybase-0.1.7/tybase/tools/riqit_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.1.7/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-06-30 10:18:11.178175 tybase-0.1.7/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      785 2023-06-30 10:18:11.000000 tybase-0.1.7/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      482 2023-06-30 10:18:11.000000 tybase-0.1.7/tybase.egg-info/SOURCES.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-06-30 10:18:11.000000 tybase-0.1.7/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      130 2023-06-30 10:18:11.000000 tybase-0.1.7/tybase.egg-info/requires.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-06-30 10:18:11.000000 tybase-0.1.7/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.1.6/setup.py` & `tybase-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.1.6',
+    version='0.1.7',
     include_package_data=True,
-    description='配置了一个七牛云的方法',
+    description='新增了mysql的更新方法',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.1.6/tybase/baidu/kw_tool.py` & `tybase-0.1.7/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.6/tybase/dbtool/data_import.py` & `tybase-0.1.7/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.6/tybase/lc/eg1.py` & `tybase-0.1.7/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.6/tybase/tools/qiniu_tools.py` & `tybase-0.1.7/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.1.6/tybase/tools/riqit_tools.py` & `tybase-0.1.7/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

