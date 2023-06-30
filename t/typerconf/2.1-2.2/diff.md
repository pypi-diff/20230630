# Comparing `tmp/typerconf-2.1.tar.gz` & `tmp/typerconf-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-2.1.tar", max compression
+gzip compressed data, was "typerconf-2.2.tar", max compression
```

## Comparing `typerconf-2.1.tar` & `typerconf-2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.1/LICENSE
--rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-2.1/README.md
--rw-r--r--   0        0        0      934 2023-06-30 11:46:50.552583 typerconf-2.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.1/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.1/src/typerconf/Makefile
--rw-r--r--   0        0        0    11041 2023-06-30 11:46:09.116428 typerconf-2.1/src/typerconf/__init__.py
--rw-r--r--   0        0        0    31977 2023-06-30 11:44:31.096060 typerconf-2.1/src/typerconf/init.nw
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.2/LICENSE
+-rw-r--r--   0        0        0     2907 2023-06-30 12:44:28.813745 typerconf-2.2/README.md
+-rw-r--r--   0        0        0      934 2023-06-30 12:46:55.754292 typerconf-2.2/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.2/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.2/src/typerconf/Makefile
+-rw-r--r--   0        0        0    11041 2023-06-30 11:46:09.116428 typerconf-2.2/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    31977 2023-06-30 11:44:31.096060 typerconf-2.2/src/typerconf/init.nw
+-rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 typerconf-2.2/PKG-INFO
```

### Comparing `typerconf-2.1/LICENSE` & `typerconf-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-2.1/pyproject.toml` & `typerconf-2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "2.1"
+version = "2.2"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-2.1/src/typerconf/__init__.py` & `typerconf-2.2/src/typerconf/__init__.py`

 * *Files identical despite different names*

### Comparing `typerconf-2.1/src/typerconf/init.nw` & `typerconf-2.2/src/typerconf/init.nw`

 * *Files identical despite different names*

