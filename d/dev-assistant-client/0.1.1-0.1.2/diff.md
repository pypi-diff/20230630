# Comparing `tmp/dev-assistant-client-0.1.1.tar.gz` & `tmp/dev-assistant-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.1.tar", last modified: Tue Jun 27 03:27:17 2023, max compression
+gzip compressed data, was "dev-assistant-client-0.1.2.tar", last modified: Fri Jun 30 21:51:02 2023, max compression
```

## Comparing `dev-assistant-client-0.1.1.tar` & `dev-assistant-client-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 03:27:17.884971 dev-assistant-client-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-27 03:10:31.000000 dev-assistant-client-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      343 2023-06-27 03:27:17.882970 dev-assistant-client-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1559 2023-06-27 03:12:02.000000 dev-assistant-client-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 03:27:17.872971 dev-assistant-client-0.1.1/dev_assistant_client/
--rw-rw-rw-   0        0        0        0 2023-06-26 03:07:42.000000 dev-assistant-client-0.1.1/dev_assistant_client/__init__.py
--rw-rw-rw-   0        0        0     3039 2023-06-27 03:19:57.000000 dev-assistant-client-0.1.1/dev_assistant_client/main.py
-drwxrwxrwx   0        0        0        0 2023-06-27 03:27:17.880972 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 03:27:17.000000 dev-assistant-client-0.1.1/dev_assistant_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 03:27:17.885968 dev-assistant-client-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      577 2023-06-27 03:22:34.000000 dev-assistant-client-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 21:51:02.567079 dev-assistant-client-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 03:10:31.000000 dev-assistant-client-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      343 2023-06-30 21:51:02.567079 dev-assistant-client-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2661 2023-06-29 23:12:03.000000 dev-assistant-client-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 21:51:02.535914 dev-assistant-client-0.1.2/dev_assistant_client/
+-rw-rw-rw-   0        0        0        0 2023-06-26 03:07:42.000000 dev-assistant-client-0.1.2/dev_assistant_client/__init__.py
+-rw-rw-rw-   0        0        0     2336 2023-06-29 21:09:54.000000 dev-assistant-client-0.1.2/dev_assistant_client/auth.py
+-rw-rw-rw-   0        0        0     2357 2023-06-29 21:49:15.000000 dev-assistant-client-0.1.2/dev_assistant_client/device.py
+-rw-rw-rw-   0        0        0     1358 2023-06-29 21:49:32.000000 dev-assistant-client-0.1.2/dev_assistant_client/main.py
+-rw-rw-rw-   0        0        0      613 2023-06-29 21:52:13.000000 dev-assistant-client-0.1.2/dev_assistant_client/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 21:51:02.551430 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-30 21:51:02.000000 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-30 21:51:02.000000 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 21:51:02.000000 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-30 21:51:02.000000 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 21:51:02.000000 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-30 21:51:02.000000 dev-assistant-client-0.1.2/dev_assistant_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 21:51:02.567079 dev-assistant-client-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      660 2023-06-30 21:50:54.000000 dev-assistant-client-0.1.2/setup.py
```

### Comparing `dev-assistant-client-0.1.1/LICENSE` & `dev-assistant-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-assistant-client-0.1.1/setup.py` & `dev-assistant-client-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
+
 setup(
     name='dev-assistant-client',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/lucianotonet/dev-assistant-client',
     author='Luciano Tonet',
     author_email='tonetlds@gmail.com',
     description='A local extension for ChatGPT plugin DevAssistant, which helps you with your development tasks straight in your machine.',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=required,
     entry_points={
         'console_scripts': [
             'dev-assistant=dev_assistant_client.main:main',
         ],
     },
 )
```

