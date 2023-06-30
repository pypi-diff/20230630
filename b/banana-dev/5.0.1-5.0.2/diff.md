# Comparing `tmp/banana_dev-5.0.1.tar.gz` & `tmp/banana_dev-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banana_dev-5.0.1.tar", last modified: Sat Jun 24 00:17:32 2023, max compression
+gzip compressed data, was "banana_dev-5.0.2.tar", last modified: Fri Jun 30 13:41:21 2023, max compression
```

## Comparing `banana_dev-5.0.1.tar` & `banana_dev-5.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-24 00:17:32.754984 banana_dev-5.0.1/
--rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-24 00:17:32.755069 banana_dev-5.0.1/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-25 00:43:43.000000 banana_dev-5.0.1/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-24 00:17:32.754062 banana_dev-5.0.1/banana_dev/
--rw-r--r--   0 erik       (501) staff       (20)       26 2023-06-24 00:11:50.000000 banana_dev-5.0.1/banana_dev/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     4050 2023-06-24 00:14:10.000000 banana_dev-5.0.1/banana_dev/client.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-24 00:17:32.754878 banana_dev-5.0.1/banana_dev.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     1867 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      241 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       24 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       11 2023-06-24 00:17:32.000000 banana_dev-5.0.1/banana_dev.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       79 2023-06-24 00:17:32.755311 banana_dev-5.0.1/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1222 2023-06-24 00:15:02.000000 banana_dev-5.0.1/setup.py
+drwxr-xr-x   0 erikkaum   (501) staff       (20)        0 2023-06-30 13:41:21.562911 banana_dev-5.0.2/
+-rw-r--r--   0 erikkaum   (501) staff       (20)     1525 2023-06-30 13:41:21.562956 banana_dev-5.0.2/PKG-INFO
+-rw-r--r--   0 erikkaum   (501) staff       (20)      879 2023-06-30 13:38:55.000000 banana_dev-5.0.2/README.md
+drwxr-xr-x   0 erikkaum   (501) staff       (20)        0 2023-06-30 13:41:21.562331 banana_dev-5.0.2/banana_dev/
+-rw-r--r--   0 erikkaum   (501) staff       (20)       26 2023-06-30 07:35:05.000000 banana_dev-5.0.2/banana_dev/__init__.py
+-rw-r--r--   0 erikkaum   (501) staff       (20)     4312 2023-06-30 13:38:55.000000 banana_dev-5.0.2/banana_dev/client.py
+drwxr-xr-x   0 erikkaum   (501) staff       (20)        0 2023-06-30 13:41:21.562816 banana_dev-5.0.2/banana_dev.egg-info/
+-rw-r--r--   0 erikkaum   (501) staff       (20)     1525 2023-06-30 13:41:21.000000 banana_dev-5.0.2/banana_dev.egg-info/PKG-INFO
+-rw-r--r--   0 erikkaum   (501) staff       (20)      241 2023-06-30 13:41:21.000000 banana_dev-5.0.2/banana_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 erikkaum   (501) staff       (20)        1 2023-06-30 13:41:21.000000 banana_dev-5.0.2/banana_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 erikkaum   (501) staff       (20)       24 2023-06-30 13:41:21.000000 banana_dev-5.0.2/banana_dev.egg-info/requires.txt
+-rw-r--r--   0 erikkaum   (501) staff       (20)       11 2023-06-30 13:41:21.000000 banana_dev-5.0.2/banana_dev.egg-info/top_level.txt
+-rw-r--r--   0 erikkaum   (501) staff       (20)       79 2023-06-30 13:41:21.563104 banana_dev-5.0.2/setup.cfg
+-rw-r--r--   0 erikkaum   (501) staff       (20)     1222 2023-06-30 13:39:02.000000 banana_dev-5.0.2/setup.py
```

### Comparing `banana_dev-5.0.1/banana_dev/client.py` & `banana_dev-5.0.2/banana_dev/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,10 +96,16 @@
             
             # banana had a temporary error -> retry
             elif res.status_code == 503:
                 if not retry:
                     raise ClientException(res=res)
                 time.sleep(backoff_interval)
                 continue
+                
+            # gateway timeout
+            elif res.status_code == 504:
+                message="Reached timeout limit of 5min. To avoid this we recommend using a app.background() handler."
+                raise ClientException(message=message)
+
 
             else:
                 raise ClientException(message="unexpected http response code: " + str(res.status_code))
```

### Comparing `banana_dev-5.0.1/setup.py` & `banana_dev-5.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='banana_dev',
     packages=['banana_dev'],
-    version='5.0.1',
+    version='5.0.2',
     license='MIT',
     # Give a short description about your library
     description='The banana package is a python client to interact with your machine learning models hosted on Banana',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
```

