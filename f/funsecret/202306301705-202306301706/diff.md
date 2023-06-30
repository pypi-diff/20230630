# Comparing `tmp/funsecret-202306301705.tar.gz` & `tmp/funsecret-202306301706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funsecret-202306301705.tar", last modified: Fri Jun 30 09:05:30 2023, max compression
+gzip compressed data, was "funsecret-202306301706.tar", last modified: Fri Jun 30 09:06:45 2023, max compression
```

## Comparing `funsecret-202306301705.tar` & `funsecret-202306301706.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:05:30.982128 funsecret-202306301705/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      168 2023-06-30 09:05:30.982128 funsecret-202306301705/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      313 2023-06-30 09:05:04.000000 funsecret-202306301705/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:05:30.982128 funsecret-202306301705/funsecret/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      181 2023-06-30 09:04:45.000000 funsecret-202306301705/funsecret/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2301 2023-06-30 09:04:45.000000 funsecret-202306301705/funsecret/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1123 2023-06-30 09:04:45.000000 funsecret-202306301705/funsecret/fernet.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7597 2023-06-30 09:05:04.000000 funsecret-202306301705/funsecret/secret.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:05:30.982128 funsecret-202306301705/funsecret.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      168 2023-06-30 09:05:30.000000 funsecret-202306301705/funsecret.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 09:05:30.000000 funsecret-202306301705/funsecret.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 09:05:30.000000 funsecret-202306301705/funsecret.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       21 2023-06-30 09:05:30.000000 funsecret-202306301705/funsecret.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       10 2023-06-30 09:05:30.000000 funsecret-202306301705/funsecret.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 09:05:30.982128 funsecret-202306301705/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      460 2023-06-30 09:05:20.000000 funsecret-202306301705/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:06:45.232309 funsecret-202306301706/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      168 2023-06-30 09:06:45.232309 funsecret-202306301706/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      313 2023-06-30 09:05:04.000000 funsecret-202306301706/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:06:45.228309 funsecret-202306301706/funsecret/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      181 2023-06-30 09:04:45.000000 funsecret-202306301706/funsecret/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2301 2023-06-30 09:04:45.000000 funsecret-202306301706/funsecret/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1123 2023-06-30 09:04:45.000000 funsecret-202306301706/funsecret/fernet.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7597 2023-06-30 09:05:04.000000 funsecret-202306301706/funsecret/secret.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 09:06:45.232309 funsecret-202306301706/funsecret.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      168 2023-06-30 09:06:45.000000 funsecret-202306301706/funsecret.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 09:06:45.000000 funsecret-202306301706/funsecret.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-06-30 09:06:45.000000 funsecret-202306301706/funsecret.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       21 2023-06-30 09:06:45.000000 funsecret-202306301706/funsecret.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       10 2023-06-30 09:06:45.000000 funsecret-202306301706/funsecret.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-06-30 09:06:45.232309 funsecret-202306301706/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      460 2023-06-30 09:05:20.000000 funsecret-202306301706/setup.py
```

### Comparing `funsecret-202306301705/funsecret/base.py` & `funsecret-202306301706/funsecret/base.py`

 * *Files identical despite different names*

### Comparing `funsecret-202306301705/funsecret/fernet.py` & `funsecret-202306301706/funsecret/fernet.py`

 * *Files identical despite different names*

### Comparing `funsecret-202306301705/funsecret/secret.py` & `funsecret-202306301706/funsecret/secret.py`

 * *Files identical despite different names*

