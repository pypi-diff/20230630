# Comparing `tmp/waivek-0.1.8.tar.gz` & `tmp/waivek-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waivek-0.1.8.tar", last modified: Thu Jun 29 05:35:10 2023, max compression
+gzip compressed data, was "waivek-0.1.9.tar", last modified: Thu Jun 29 11:29:46 2023, max compression
```

## Comparing `waivek-0.1.8.tar` & `waivek-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 05:35:10.207301 waivek-0.1.8/
--rw-rw-rw-   0        0        0     1470 2023-06-29 05:35:10.207301 waivek-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1295 2023-06-27 07:27:31.000000 waivek-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 05:35:10.207301 waivek-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1575 2023-06-28 09:47:28.000000 waivek-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 05:35:10.191273 waivek-0.1.8/waivek/
--rw-rw-rw-   0        0        0      377 2023-06-28 14:52:26.000000 waivek-0.1.8/waivek/__init__.py
--rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.8/waivek/color.py
--rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.8/waivek/common.py
--rw-rw-rw-   0        0        0    18824 2023-06-28 14:43:11.000000 waivek-0.1.8/waivek/db.py
--rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.8/waivek/error.py
--rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.8/waivek/frame.py
--rw-rw-rw-   0        0        0     9044 2023-06-28 14:50:21.000000 waivek-0.1.8/waivek/get.py
--rw-rw-rw-   0        0        0    28068 2023-06-27 06:18:33.000000 waivek-0.1.8/waivek/ic.py
--rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.8/waivek/print_utils.py
--rw-rw-rw-   0        0        0     3326 2023-06-28 14:51:23.000000 waivek-0.1.8/waivek/reltools.py
--rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.8/waivek/reqs.py
--rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.8/waivek/tdd.py
--rw-rw-rw-   0        0        0      324 2023-06-28 10:02:01.000000 waivek-0.1.8/waivek/template.py
--rw-rw-rw-   0        0        0    23039 2023-06-27 07:29:46.000000 waivek-0.1.8/waivek/test.py
--rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.8/waivek/timer.py
--rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.8/waivek/trace.py
-drwxrwxrwx   0        0        0        0 2023-06-29 05:35:10.207301 waivek-0.1.8/waivek.egg-info/
--rw-rw-rw-   0        0        0     1470 2023-06-29 05:35:09.000000 waivek-0.1.8/waivek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-06-29 05:35:09.000000 waivek-0.1.8/waivek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 05:35:09.000000 waivek-0.1.8/waivek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-29 05:35:09.000000 waivek-0.1.8/waivek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 05:35:09.000000 waivek-0.1.8/waivek.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 11:29:46.325274 waivek-0.1.9/
+-rw-rw-rw-   0        0        0     1470 2023-06-29 11:29:46.324279 waivek-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1295 2023-06-27 07:27:31.000000 waivek-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 11:29:46.326275 waivek-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1575 2023-06-28 09:47:28.000000 waivek-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:29:46.275941 waivek-0.1.9/waivek/
+-rw-rw-rw-   0        0        0      377 2023-06-28 14:52:26.000000 waivek-0.1.9/waivek/__init__.py
+-rw-rw-rw-   0        0        0     5601 2023-06-26 13:00:33.000000 waivek-0.1.9/waivek/color.py
+-rw-rw-rw-   0        0        0    17147 2023-06-26 13:00:47.000000 waivek-0.1.9/waivek/common.py
+-rw-rw-rw-   0        0        0    18824 2023-06-28 14:43:11.000000 waivek-0.1.9/waivek/db.py
+-rw-rw-rw-   0        0        0    25668 2023-06-26 13:01:04.000000 waivek-0.1.9/waivek/error.py
+-rw-rw-rw-   0        0        0     4725 2023-06-26 13:01:06.000000 waivek-0.1.9/waivek/frame.py
+-rw-rw-rw-   0        0        0     9044 2023-06-28 14:50:21.000000 waivek-0.1.9/waivek/get.py
+-rw-rw-rw-   0        0        0    28068 2023-06-27 06:18:33.000000 waivek-0.1.9/waivek/ic.py
+-rw-rw-rw-   0        0        0     6272 2023-06-26 13:01:23.000000 waivek-0.1.9/waivek/print_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-06-29 11:28:56.000000 waivek-0.1.9/waivek/reltools.py
+-rw-rw-rw-   0        0        0     4431 2023-06-26 16:58:35.000000 waivek-0.1.9/waivek/reqs.py
+-rw-rw-rw-   0        0        0     1191 2023-06-26 13:01:34.000000 waivek-0.1.9/waivek/tdd.py
+-rw-rw-rw-   0        0        0      324 2023-06-28 10:02:01.000000 waivek-0.1.9/waivek/template.py
+-rw-rw-rw-   0        0        0    23039 2023-06-27 07:29:46.000000 waivek-0.1.9/waivek/test.py
+-rw-rw-rw-   0        0        0     3668 2023-06-25 06:42:04.000000 waivek-0.1.9/waivek/timer.py
+-rw-rw-rw-   0        0        0     5908 2023-06-26 13:02:00.000000 waivek-0.1.9/waivek/trace.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:29:46.321325 waivek-0.1.9/waivek.egg-info/
+-rw-rw-rw-   0        0        0     1470 2023-06-29 11:29:45.000000 waivek-0.1.9/waivek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-06-29 11:29:45.000000 waivek-0.1.9/waivek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:29:45.000000 waivek-0.1.9/waivek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-29 11:29:45.000000 waivek-0.1.9/waivek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 11:29:45.000000 waivek-0.1.9/waivek.egg-info/top_level.txt
```

### Comparing `waivek-0.1.8/PKG-INFO` & `waivek-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waivek
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Code - Print colored text
```

### Comparing `waivek-0.1.8/README.md` & `waivek-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/setup.py` & `waivek-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/color.py` & `waivek-0.1.9/waivek/color.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/common.py` & `waivek-0.1.9/waivek/common.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/db.py` & `waivek-0.1.9/waivek/db.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/error.py` & `waivek-0.1.9/waivek/error.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/frame.py` & `waivek-0.1.9/waivek/frame.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/get.py` & `waivek-0.1.9/waivek/get.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/ic.py` & `waivek-0.1.9/waivek/ic.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/print_utils.py` & `waivek-0.1.9/waivek/print_utils.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/reltools.py` & `waivek-0.1.9/waivek/reltools.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,42 @@
 #
 #     reltools:write
 #     reltools:read
 #     db:db_init`
 
 import os
 import sys
+from .color import Code
 
 def pathjoin(frame, relpath):
     frame_directory = os.path.dirname(frame.f_code.co_filename)
     return os.path.realpath(os.path.join(frame_directory, relpath))
 
+def readlines(relpath):
+    """
+    Read lines from a file.
+    relpath can be relative or absolute. Resolved via rel2abs methodology.
+    Leading and trailing whitespace is stripped.
+    """
+    path = relpath if os.path.isabs(relpath) else pathjoin(sys._getframe(1), relpath)
+    if os.path.exists(path) is False:
+        print(f"File not found: {Code.RED + path}")
+    with open(path, "rb") as f:
+        lines = f.read().decode("utf-8").strip().splitlines()
+    return lines
+    
+def writelines(relpath, lines):
+    """
+    Write lines to a file.
+    relpath can be relative or absolute. Resolved via rel2abs methodology.
+    """
+    path = relpath if os.path.isabs(relpath) else pathjoin(sys._getframe(1), relpath)
+    with open(path, "wb") as f:
+        f.write("\n".join(lines).encode("utf-8"))
+
 def read(relpath):
     import json
     from .color import Code
     filepath = relpath if os.path.isabs(relpath) else pathjoin(sys._getframe(1), relpath)
     filepath = os.path.normpath(filepath)
     if os.path.exists(filepath) is False:
         message = "[reltools.py:read()] " + (Code.YELLOW + "File does not exist: ") + (Code.RED + filepath)
```

### Comparing `waivek-0.1.8/waivek/reqs.py` & `waivek-0.1.9/waivek/reqs.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/tdd.py` & `waivek-0.1.9/waivek/tdd.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/test.py` & `waivek-0.1.9/waivek/test.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/timer.py` & `waivek-0.1.9/waivek/timer.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek/trace.py` & `waivek-0.1.9/waivek/trace.py`

 * *Files identical despite different names*

### Comparing `waivek-0.1.8/waivek.egg-info/PKG-INFO` & `waivek-0.1.9/waivek.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waivek
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Code - Print colored text
```

