# Comparing `tmp/btimer-1.0.6.tar.gz` & `tmp/btimer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btimer-1.0.6.tar", last modified: Sun Jun 25 13:39:37 2023, max compression
+gzip compressed data, was "btimer-1.0.7.tar", last modified: Fri Jun 30 03:33:40 2023, max compression
```

## Comparing `btimer-1.0.6.tar` & `btimer-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 13:39:37.856128 btimer-1.0.6/
--rw-r--r--   0 dylan      (501) staff       (20)     1075 2023-06-25 03:17:01.000000 btimer-1.0.6/LICENSE.txt
--rw-r--r--   0 dylan      (501) staff       (20)     1240 2023-06-25 13:39:37.856013 btimer-1.0.6/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      730 2023-06-25 13:37:38.000000 btimer-1.0.6/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-06-25 13:39:37.855874 btimer-1.0.6/btimer.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1240 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      227 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/entry_points.txt
--rw-r--r--   0 dylan      (501) staff       (20)       13 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)        6 2023-06-25 13:39:37.000000 btimer-1.0.6/btimer.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)      641 2023-06-25 13:38:33.000000 btimer-1.0.6/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-06-25 13:39:37.856164 btimer-1.0.6/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1508 2023-06-25 11:53:46.000000 btimer-1.0.6/timer.py
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 03:33:40.904377 btimer-1.0.7/
+-rw-r--r--   0 dylan      (502) staff       (20)     1075 2023-06-30 02:58:44.000000 btimer-1.0.7/LICENSE.txt
+-rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 03:33:40.904242 btimer-1.0.7/PKG-INFO
+-rw-r--r--   0 dylan      (502) staff       (20)      730 2023-06-30 02:58:44.000000 btimer-1.0.7/README.md
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 03:33:40.904062 btimer-1.0.7/btimer.egg-info/
+-rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (502) staff       (20)      227 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (502) staff       (20)        1 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/entry_points.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       13 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/requires.txt
+-rw-r--r--   0 dylan      (502) staff       (20)        6 2023-06-30 03:33:40.000000 btimer-1.0.7/btimer.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (502) staff       (20)      641 2023-06-30 03:31:11.000000 btimer-1.0.7/pyproject.toml
+-rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 03:33:40.904417 btimer-1.0.7/setup.cfg
+-rw-r--r--   0 dylan      (502) staff       (20)     1274 2023-06-30 03:25:13.000000 btimer-1.0.7/timer.py
```

### Comparing `btimer-1.0.6/LICENSE.txt` & `btimer-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btimer-1.0.6/PKG-INFO` & `btimer-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.6
+Version: 1.0.7
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.6/README.md` & `btimer-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `btimer-1.0.6/btimer.egg-info/PKG-INFO` & `btimer-1.0.7/btimer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.6
+Version: 1.0.7
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.6/pyproject.toml` & `btimer-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btimer"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Dylan Ngo", email="it.tinhngo@gmail.com" },
 ]
 description = "Help people get away from the computer"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `btimer-1.0.6/timer.py` & `btimer-1.0.7/timer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 #!/usr/bin/env python
 
 import subprocess
 import sys
 import random
 import time
+import json
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.progress import Progress
 
-verses = {
-    0: {
-        'quote': 'Self love brings happiness.',
-        'author': 'Thich Nhat Hanh'
-    },
-    1: {
-        'quote': 'There is no way to happiness, happiness is the way.',
-        'author': 'Thich Nhat Hanh'
-    },
-    2: {
-        'quote': 'Happiness is in the here and now.',
-        'author': 'Thich Nhat Hanh'
-    }
-}
 
 def count_down(t: any) -> None:
     console = Console()
     with Progress() as progress:
         task1 = progress.add_task("", total=t, transient=True)
 
         while not progress.finished:
             progress.update(task1, advance=1)
             time.sleep(1)
 
     console.print("\n")
 
 
+def read_json():
+    f = open('verses.json')
+    return json.load(f)
+
+
 def print_quotes() -> None:
     console = Console()
 
     randint = random.randint(0, 2)
+    verses = read_json()
     quote = verses[randint]
     console.print(Panel(""" "{}" - {} """.format(quote['quote'], quote['author']), title="Verses"))
 
 
 def active_window() -> None:
     applescript = """
     tell application "Terminal"
```

