# Comparing `tmp/email-finder-website-0.1.tar.gz` & `tmp/email-finder-website-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-finder-website-0.1.tar", last modified: Wed Jun 28 19:21:54 2023, max compression
+gzip compressed data, was "email-finder-website-0.3.tar", last modified: Fri Jun 30 13:13:39 2023, max compression
```

## Comparing `email-finder-website-0.1.tar` & `email-finder-website-0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-28 19:21:54.303837 email-finder-website-0.1/
--rw-r--r--   0 savascal   (501) staff       (20)      536 2023-06-28 19:21:54.303518 email-finder-website-0.1/PKG-INFO
-drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-28 19:21:54.300607 email-finder-website-0.1/email_crawler/
--rw-r--r--   0 savascal   (501) staff       (20)       33 2023-06-28 17:47:26.000000 email-finder-website-0.1/email_crawler/__init__.py
--rw-r--r--   0 savascal   (501) staff       (20)     4743 2023-06-28 18:23:25.000000 email-finder-website-0.1/email_crawler/crawler.py
-drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-28 19:21:54.303003 email-finder-website-0.1/email_finder_website.egg-info/
--rw-r--r--   0 savascal   (501) staff       (20)      536 2023-06-28 19:21:54.000000 email-finder-website-0.1/email_finder_website.egg-info/PKG-INFO
--rw-r--r--   0 savascal   (501) staff       (20)      325 2023-06-28 19:21:54.000000 email-finder-website-0.1/email_finder_website.egg-info/SOURCES.txt
--rw-r--r--   0 savascal   (501) staff       (20)        1 2023-06-28 19:21:54.000000 email-finder-website-0.1/email_finder_website.egg-info/dependency_links.txt
--rw-r--r--   0 savascal   (501) staff       (20)       59 2023-06-28 19:21:54.000000 email-finder-website-0.1/email_finder_website.egg-info/entry_points.txt
--rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-28 19:21:54.000000 email-finder-website-0.1/email_finder_website.egg-info/requires.txt
--rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-28 19:21:54.000000 email-finder-website-0.1/email_finder_website.egg-info/top_level.txt
--rw-r--r--   0 savascal   (501) staff       (20)       38 2023-06-28 19:21:54.303958 email-finder-website-0.1/setup.cfg
--rw-r--r--   0 savascal   (501) staff       (20)      842 2023-06-28 19:21:13.000000 email-finder-website-0.1/setup.py
+drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:13:39.360126 email-finder-website-0.3/
+-rw-r--r--   0 savascal   (501) staff       (20)      489 2023-06-30 13:13:39.359576 email-finder-website-0.3/PKG-INFO
+-rw-r--r--   0 savascal   (501) staff       (20)      978 2023-06-30 13:05:03.000000 email-finder-website-0.3/README.md
+drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:13:39.356473 email-finder-website-0.3/email_crawler/
+-rw-r--r--   0 savascal   (501) staff       (20)       33 2023-06-28 17:47:26.000000 email-finder-website-0.3/email_crawler/__init__.py
+-rw-r--r--   0 savascal   (501) staff       (20)     4743 2023-06-28 18:23:25.000000 email-finder-website-0.3/email_crawler/crawler.py
+drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:13:39.359032 email-finder-website-0.3/email_finder_website.egg-info/
+-rw-r--r--   0 savascal   (501) staff       (20)      489 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/PKG-INFO
+-rw-r--r--   0 savascal   (501) staff       (20)      335 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/SOURCES.txt
+-rw-r--r--   0 savascal   (501) staff       (20)        1 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/dependency_links.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       59 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/entry_points.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/requires.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/top_level.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       38 2023-06-30 13:13:39.360305 email-finder-website-0.3/setup.cfg
+-rw-r--r--   0 savascal   (501) staff       (20)      796 2023-06-30 13:13:14.000000 email-finder-website-0.3/setup.py
```

### Comparing `email-finder-website-0.1/email_crawler/crawler.py` & `email-finder-website-0.3/email_crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `email-finder-website-0.1/setup.py` & `email-finder-website-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="email-finder-website",
-    version="0.1",
+    version="0.3",
     description="A Python library to crawl websites and collect emails",
     author="Sav Cal",
     author_email="savadamcal@gmail.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "lxml",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
             'emailfinder=email_crawler.crawler:main',
         ],
     },
```

