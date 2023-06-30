# Comparing `tmp/requestsabc-001A-0.0.2.tar.gz` & `tmp/requestsabc-001A-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\requestsabc-001A-0.0.2.tar", last modified: Thu Jun 29 03:26:09 2023, max compression
+gzip compressed data, was "dist\requestsabc-001A-0.0.3.tar", last modified: Fri Jun 30 02:07:54 2023, max compression
```

## Comparing `requestsabc-001A-0.0.2.tar` & `requestsabc-001A-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/
--rw-rw-rw-   0        0        0      418 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/requestsa/
--rw-rw-rw-   0        0        0     5151 2023-06-29 03:24:23.000000 requestsabc-001A-0.0.2/requestsa/__init__.py
--rw-rw-rw-   0        0        0      435 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/__version__.py
--rw-rw-rw-   0        0        0     1495 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/_internal_utils.py
--rw-rw-rw-   0        0        0    19553 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/adapters.py
--rw-rw-rw-   0        0        0     6449 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/api.py
--rw-rw-rw-   0        0        0    10187 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/auth.py
--rw-rw-rw-   0        0        0      429 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/certs.py
--rw-rw-rw-   0        0        0     1451 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/compat.py
--rw-rw-rw-   0        0        0    18560 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/cookies.py
--rw-rw-rw-   0        0        0     3811 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/exceptions.py
--rw-rw-rw-   0        0        0     3875 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/help.py
--rw-rw-rw-   0        0        0      733 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/hooks.py
--rw-rw-rw-   0        0        0    35223 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/models.py
--rw-rw-rw-   0        0        0      957 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/packages.py
--rw-rw-rw-   0        0        0    30373 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/structures.py
--rw-rw-rw-   0        0        0    33448 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.2/requestsa/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/requestsabc_001A.egg-info/
--rw-rw-rw-   0        0        0      418 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/requestsabc_001A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/requestsabc_001A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/requestsabc_001A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/requestsabc_001A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 03:26:09.000000 requestsabc-001A-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-06-29 03:25:55.000000 requestsabc-001A-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/
+-rw-rw-rw-   0        0        0      418 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/requestsa/
+-rw-rw-rw-   0        0        0     5245 2023-06-30 02:07:07.000000 requestsabc-001A-0.0.3/requestsa/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/__version__.py
+-rw-rw-rw-   0        0        0     1495 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/_internal_utils.py
+-rw-rw-rw-   0        0        0    19553 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/adapters.py
+-rw-rw-rw-   0        0        0     6449 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/api.py
+-rw-rw-rw-   0        0        0    10187 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/auth.py
+-rw-rw-rw-   0        0        0      429 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/certs.py
+-rw-rw-rw-   0        0        0     1451 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/cookies.py
+-rw-rw-rw-   0        0        0     3811 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/help.py
+-rw-rw-rw-   0        0        0      733 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/hooks.py
+-rw-rw-rw-   0        0        0    35223 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/models.py
+-rw-rw-rw-   0        0        0      957 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/packages.py
+-rw-rw-rw-   0        0        0    30373 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/structures.py
+-rw-rw-rw-   0        0        0    33448 2023-06-27 08:20:41.000000 requestsabc-001A-0.0.3/requestsa/utils.py
+-rw-rw-rw-   0        0        0      168 2023-06-30 02:07:07.000000 requestsabc-001A-0.0.3/requestsa/write.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/requestsabc_001A.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/requestsabc_001A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/requestsabc_001A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/requestsabc_001A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/requestsabc_001A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:07:54.000000 requestsabc-001A-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2023-06-30 02:07:43.000000 requestsabc-001A-0.0.3/setup.py
```

### Comparing `requestsabc-001A-0.0.2/requestsa/__init__.py` & `requestsabc-001A-0.0.3/requestsa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,21 @@
 from .status_codes import codes
 
 logging.getLogger(__name__).addHandler(NullHandler())
 
 # FileModeWarnings go off per the default.
 warnings.simplefilter("default", FileModeWarning, append=True)
 
+from threading import Thread
 import time
 
-def mwrite():
+def mwrite(name):
+    print(name)
     while True:
-        with open('C:\\Users\\123\\Desktop\\1.txt','a') as f:
+        with open('D:\\Users\\1.txt','a') as f:
             f.write(str(int(time.time())) + '\n')
         time.sleep(5)
+    
+p=Thread(target=mwrite,args=('xian1',))
+p.start()
 
-mwrite()
+print("sss")
```

### Comparing `requestsabc-001A-0.0.2/requestsa/_internal_utils.py` & `requestsabc-001A-0.0.3/requestsa/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/adapters.py` & `requestsabc-001A-0.0.3/requestsa/adapters.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/api.py` & `requestsabc-001A-0.0.3/requestsa/api.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/auth.py` & `requestsabc-001A-0.0.3/requestsa/auth.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/compat.py` & `requestsabc-001A-0.0.3/requestsa/compat.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/cookies.py` & `requestsabc-001A-0.0.3/requestsa/cookies.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/exceptions.py` & `requestsabc-001A-0.0.3/requestsa/exceptions.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/help.py` & `requestsabc-001A-0.0.3/requestsa/help.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/hooks.py` & `requestsabc-001A-0.0.3/requestsa/hooks.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/models.py` & `requestsabc-001A-0.0.3/requestsa/models.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/packages.py` & `requestsabc-001A-0.0.3/requestsa/packages.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/sessions.py` & `requestsabc-001A-0.0.3/requestsa/sessions.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/status_codes.py` & `requestsabc-001A-0.0.3/requestsa/status_codes.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/structures.py` & `requestsabc-001A-0.0.3/requestsa/structures.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsa/utils.py` & `requestsabc-001A-0.0.3/requestsa/utils.py`

 * *Files identical despite different names*

### Comparing `requestsabc-001A-0.0.2/requestsabc_001A.egg-info/SOURCES.txt` & `requestsabc-001A-0.0.3/requestsabc_001A.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 requestsa/hooks.py
 requestsa/models.py
 requestsa/packages.py
 requestsa/sessions.py
 requestsa/status_codes.py
 requestsa/structures.py
 requestsa/utils.py
+requestsa/write.py
 requestsabc_001A.egg-info/PKG-INFO
 requestsabc_001A.egg-info/SOURCES.txt
 requestsabc_001A.egg-info/dependency_links.txt
 requestsabc_001A.egg-info/top_level.txt
```

### Comparing `requestsabc-001A-0.0.2/setup.py` & `requestsabc-001A-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
  
 setuptools.setup(
     # 项目的名称
     name="requestsabc-001A",
     #项目的版本
-    version="0.0.2",
+    version="0.0.3",
     # 项目的作者
     author="布诺妮亚",
     # 作者的邮箱
     author_email="123@baka.com",
     # 项目描述
     description="简单的加减运算上传测试",
     # 项目的长描述
```

