# Comparing `tmp/oester-1.2.0.tar.gz` & `tmp/oester-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oester-1.2.0.tar", last modified: Fri Jun 30 09:29:11 2023, max compression
+gzip compressed data, was "oester-1.3.0.tar", last modified: Fri Jun 30 09:44:43 2023, max compression
```

## Comparing `oester-1.2.0.tar` & `oester-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:29:11.302648 oester-1.2.0/
--rw-rw-rw-   0        0        0      104 2023-06-30 09:29:11.295609 oester-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 09:29:11.288145 oester-1.2.0/oester.egg-info/
--rw-rw-rw-   0        0        0      104 2023-06-30 09:29:09.000000 oester-1.2.0/oester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-06-30 09:29:09.000000 oester-1.2.0/oester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:29:09.000000 oester-1.2.0/oester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 09:29:09.000000 oester-1.2.0/oester.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      407 2023-06-30 09:21:26.000000 oester-1.2.0/oester.py
--rw-rw-rw-   0        0        0       42 2023-06-30 09:29:11.302648 oester-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      185 2023-06-30 09:24:55.000000 oester-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:44:43.197536 oester-1.3.0/
+-rw-rw-rw-   0        0        0      104 2023-06-30 09:44:43.180241 oester-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 09:44:43.176621 oester-1.3.0/oester.egg-info/
+-rw-rw-rw-   0        0        0      104 2023-06-30 09:44:42.000000 oester-1.3.0/oester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-06-30 09:44:42.000000 oester-1.3.0/oester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:44:42.000000 oester-1.3.0/oester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 09:44:42.000000 oester-1.3.0/oester.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      502 2023-06-30 09:42:30.000000 oester-1.3.0/oester.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:44:43.197536 oester-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      185 2023-06-30 09:43:56.000000 oester-1.3.0/setup.py
```

