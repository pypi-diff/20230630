# Comparing `tmp/siddhesh-0.1.6.tar.gz` & `tmp/siddhesh-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siddhesh-0.1.6.tar", last modified: Thu Jun  1 16:05:47 2023, max compression
+gzip compressed data, was "siddhesh-0.1.9.tar", last modified: Fri Jun 30 09:29:55 2023, max compression
```

## Comparing `siddhesh-0.1.6.tar` & `siddhesh-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 16:05:47.812002 siddhesh-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      767 2023-06-01 16:05:47.805482 siddhesh-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 16:05:47.812002 siddhesh-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-01 16:04:52.000000 siddhesh-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:05:47.787490 siddhesh-0.1.6/siddhesh/
--rw-rw-rw-   0        0        0     1359 2023-06-01 16:03:23.000000 siddhesh-0.1.6/siddhesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:05:47.805482 siddhesh-0.1.6/siddhesh.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 16:05:47.000000 siddhesh-0.1.6/siddhesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 09:29:55.528981 siddhesh-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      767 2023-06-30 09:29:55.525946 siddhesh-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:29:55.529946 siddhesh-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-30 09:29:42.000000 siddhesh-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:29:55.508267 siddhesh-0.1.9/siddhesh/
+-rw-rw-rw-   0        0        0     1359 2023-06-30 09:22:08.000000 siddhesh-0.1.9/siddhesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:29:55.523795 siddhesh-0.1.9/siddhesh.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/top_level.txt
```

### Comparing `siddhesh-0.1.6/LICENSE` & `siddhesh-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.6/PKG-INFO` & `siddhesh-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.6
+Version: 0.1.9
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `siddhesh-0.1.6/README.md` & `siddhesh-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.6/setup.py` & `siddhesh-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.6"
+VERSION = "0.1.9"
 DESCRIPTION = "Check out Siddhesh Kulthe's profile, or send him a direct message!"
 LONG_DESCRIPTION = "A package that downloads Siddhesh Kulthe's Resume on your computer. All you need to do is to import siddhesh and use .Start() method to start the app!"
 
 # Setting up
 setup(
     name="siddhesh",
     version=VERSION,
```

### Comparing `siddhesh-0.1.6/siddhesh/__init__.py` & `siddhesh-0.1.9/siddhesh/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def send_message():
     message = str(input("Enter your message: "))
     time.sleep(1)
     print("Just so that Siddhesh can get back to you,")
     time.sleep(1)
     email = str(input("Please enter your email:"))
-    vercel_url = "http://34.204.127.0:5000"
+    vercel_url = "http://34.204.127.0:5001"
     data = {"message": message, "email": email}
 
     # Make the HTTP POST request to your Vercel app's endpoint
     response = requests.post(vercel_url, json=data)
 
     if response.status_code == 200:
         print("Message sent successfully!")
```

### Comparing `siddhesh-0.1.6/siddhesh.egg-info/PKG-INFO` & `siddhesh-0.1.9/siddhesh.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.6
+Version: 0.1.9
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

