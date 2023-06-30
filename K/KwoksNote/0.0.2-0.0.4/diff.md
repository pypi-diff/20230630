# Comparing `tmp/KwoksNote-0.0.2.tar.gz` & `tmp/KwoksNote-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksNote-0.0.2.tar", last modified: Sun Apr  9 00:52:23 2023, max compression
+gzip compressed data, was "KwoksNote-0.0.4.tar", last modified: Fri Jun 30 12:06:55 2023, max compression
```

## Comparing `KwoksNote-0.0.2.tar` & `KwoksNote-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/KwoksNote/
--rw-rw-rw-   0        0        0      191 2023-04-09 00:49:33.000000 KwoksNote-0.0.2/KwoksNote/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-09 00:51:36.000000 KwoksNote-0.0.2/KwoksNote/_version.py
--rw-rw-rw-   0        0        0       23 2023-04-09 00:29:09.000000 KwoksNote-0.0.2/KwoksNote/数据分析.py
-drwxrwxrwx   0        0        0        0 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/KwoksNote.egg-info/
--rw-rw-rw-   0        0        0       56 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-04-09 00:51:47.000000 KwoksNote-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-30 12:06:55.244738 KwoksNote-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:06:55.229117 KwoksNote-0.0.4/KwoksNote/
+-rw-rw-rw-   0        0        0      581 2023-06-30 11:53:26.000000 KwoksNote-0.0.4/KwoksNote/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-06-30 12:06:32.000000 KwoksNote-0.0.4/KwoksNote/_version.py
+-rw-rw-rw-   0        0        0    15838 2023-06-30 11:48:49.000000 KwoksNote-0.0.4/KwoksNote/function.py
+-rw-rw-rw-   0        0        0      122 2023-06-30 11:40:02.000000 KwoksNote-0.0.4/KwoksNote/info.py
+-rw-rw-rw-   0        0        0      122 2023-06-30 11:40:02.000000 KwoksNote-0.0.4/KwoksNote/model.py
+-rw-rw-rw-   0        0        0       13 2023-06-30 11:59:27.000000 KwoksNote-0.0.4/KwoksNote/spider.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:06:55.244738 KwoksNote-0.0.4/KwoksNote.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-30 12:06:55.000000 KwoksNote-0.0.4/KwoksNote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-30 12:06:55.000000 KwoksNote-0.0.4/KwoksNote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:06:55.000000 KwoksNote-0.0.4/KwoksNote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 12:06:55.000000 KwoksNote-0.0.4/KwoksNote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-06-30 12:06:55.244738 KwoksNote-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-06-30 12:06:27.000000 KwoksNote-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 12:06:55.244738 KwoksNote-0.0.4/setup.cfg
```

