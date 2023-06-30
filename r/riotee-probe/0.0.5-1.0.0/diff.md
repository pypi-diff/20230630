# Comparing `tmp/riotee_probe-0.0.5.tar.gz` & `tmp/riotee_probe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_probe-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_probe-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_probe-0.0.5.tar` & `riotee_probe-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1116 2023-06-30 15:57:05.203880 riotee_probe-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      515 2023-06-30 15:57:09.757214 riotee_probe-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      325 2023-06-28 21:07:34.953887 riotee_probe-0.0.5/riotee_probe/__init__.py
--rw-r--r--   0        0        0     2980 2023-06-29 20:41:32.997112 riotee_probe-0.0.5/riotee_probe/cli.py
--rw-r--r--   0        0        0     1668 2023-06-28 14:45:07.836937 riotee_probe-0.0.5/riotee_probe/intelhex.py
--rw-r--r--   0        0        0     2591 2023-06-29 20:36:50.317094 riotee_probe-0.0.5/riotee_probe/probe.py
--rw-r--r--   0        0        0      893 2023-06-28 19:28:15.886844 riotee_probe-0.0.5/riotee_probe/protocol.py
--rw-r--r--   0        0        0      965 2023-06-29 20:35:25.067089 riotee_probe-0.0.5/riotee_probe/session.py
--rw-r--r--   0        0        0     4223 2023-06-29 20:08:11.163652 riotee_probe-0.0.5/riotee_probe/target.py
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 riotee_probe-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      515 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/cli.py
+-rw-r--r--   0        0        0     1668 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/intelhex.py
+-rw-r--r--   0        0        0     2591 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/probe.py
+-rw-r--r--   0        0        0      893 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/protocol.py
+-rw-r--r--   0        0        0      965 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/session.py
+-rw-r--r--   0        0        0     4223 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/target.py
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 riotee_probe-1.0.0/PKG-INFO
```

### Comparing `riotee_probe-0.0.5/LICENSE.txt` & `riotee_probe-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/pyproject.toml` & `riotee_probe-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/riotee_probe/cli.py` & `riotee_probe-1.0.0/riotee_probe/cli.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/riotee_probe/intelhex.py` & `riotee_probe-1.0.0/riotee_probe/intelhex.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/riotee_probe/probe.py` & `riotee_probe-1.0.0/riotee_probe/probe.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/riotee_probe/protocol.py` & `riotee_probe-1.0.0/riotee_probe/protocol.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/riotee_probe/session.py` & `riotee_probe-1.0.0/riotee_probe/session.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-0.0.5/riotee_probe/target.py` & `riotee_probe-1.0.0/riotee_probe/target.py`

 * *Files identical despite different names*

