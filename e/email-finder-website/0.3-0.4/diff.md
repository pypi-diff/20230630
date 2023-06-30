# Comparing `tmp/email-finder-website-0.3.tar.gz` & `tmp/email-finder-website-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-finder-website-0.3.tar", last modified: Fri Jun 30 13:13:39 2023, max compression
+gzip compressed data, was "email-finder-website-0.4.tar", last modified: Fri Jun 30 13:18:14 2023, max compression
```

## Comparing `email-finder-website-0.3.tar` & `email-finder-website-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:13:39.360126 email-finder-website-0.3/
--rw-r--r--   0 savascal   (501) staff       (20)      489 2023-06-30 13:13:39.359576 email-finder-website-0.3/PKG-INFO
--rw-r--r--   0 savascal   (501) staff       (20)      978 2023-06-30 13:05:03.000000 email-finder-website-0.3/README.md
-drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:13:39.356473 email-finder-website-0.3/email_crawler/
--rw-r--r--   0 savascal   (501) staff       (20)       33 2023-06-28 17:47:26.000000 email-finder-website-0.3/email_crawler/__init__.py
--rw-r--r--   0 savascal   (501) staff       (20)     4743 2023-06-28 18:23:25.000000 email-finder-website-0.3/email_crawler/crawler.py
-drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:13:39.359032 email-finder-website-0.3/email_finder_website.egg-info/
--rw-r--r--   0 savascal   (501) staff       (20)      489 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/PKG-INFO
--rw-r--r--   0 savascal   (501) staff       (20)      335 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/SOURCES.txt
--rw-r--r--   0 savascal   (501) staff       (20)        1 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/dependency_links.txt
--rw-r--r--   0 savascal   (501) staff       (20)       59 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/entry_points.txt
--rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/requires.txt
--rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-30 13:13:39.000000 email-finder-website-0.3/email_finder_website.egg-info/top_level.txt
--rw-r--r--   0 savascal   (501) staff       (20)       38 2023-06-30 13:13:39.360305 email-finder-website-0.3/setup.cfg
--rw-r--r--   0 savascal   (501) staff       (20)      796 2023-06-30 13:13:14.000000 email-finder-website-0.3/setup.py
+drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:18:14.484393 email-finder-website-0.4/
+-rw-r--r--   0 savascal   (501) staff       (20)     1509 2023-06-30 13:18:14.483877 email-finder-website-0.4/PKG-INFO
+-rw-r--r--   0 savascal   (501) staff       (20)      978 2023-06-30 13:05:03.000000 email-finder-website-0.4/README.md
+drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:18:14.480639 email-finder-website-0.4/email_crawler/
+-rw-r--r--   0 savascal   (501) staff       (20)       33 2023-06-28 17:47:26.000000 email-finder-website-0.4/email_crawler/__init__.py
+-rw-r--r--   0 savascal   (501) staff       (20)     4743 2023-06-28 18:23:25.000000 email-finder-website-0.4/email_crawler/crawler.py
+drwxr-xr-x   0 savascal   (501) staff       (20)        0 2023-06-30 13:18:14.483326 email-finder-website-0.4/email_finder_website.egg-info/
+-rw-r--r--   0 savascal   (501) staff       (20)     1509 2023-06-30 13:18:14.000000 email-finder-website-0.4/email_finder_website.egg-info/PKG-INFO
+-rw-r--r--   0 savascal   (501) staff       (20)      335 2023-06-30 13:18:14.000000 email-finder-website-0.4/email_finder_website.egg-info/SOURCES.txt
+-rw-r--r--   0 savascal   (501) staff       (20)        1 2023-06-30 13:18:14.000000 email-finder-website-0.4/email_finder_website.egg-info/dependency_links.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       59 2023-06-30 13:18:14.000000 email-finder-website-0.4/email_finder_website.egg-info/entry_points.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-30 13:18:14.000000 email-finder-website-0.4/email_finder_website.egg-info/requires.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       14 2023-06-30 13:18:14.000000 email-finder-website-0.4/email_finder_website.egg-info/top_level.txt
+-rw-r--r--   0 savascal   (501) staff       (20)       38 2023-06-30 13:18:14.484517 email-finder-website-0.4/setup.cfg
+-rw-r--r--   0 savascal   (501) staff       (20)     1107 2023-06-30 13:17:23.000000 email-finder-website-0.4/setup.py
```

### Comparing `email-finder-website-0.3/README.md` & `email-finder-website-0.4/README.md`

 * *Files identical despite different names*

### Comparing `email-finder-website-0.3/email_crawler/crawler.py` & `email-finder-website-0.4/email_crawler/crawler.py`

 * *Files identical despite different names*

