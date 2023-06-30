# Comparing `tmp/pipevcr-0.1.0.tar.gz` & `tmp/pipevcr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipevcr-0.1.0.tar", last modified: Tue Oct 11 17:51:43 2022, max compression
+gzip compressed data, was "pipevcr-0.1.1.tar", last modified: Fri Jun 30 21:10:05 2023, max compression
```

## Comparing `pipevcr-0.1.0.tar` & `pipevcr-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 spark      (501) staff       (20)        0 2022-10-11 17:51:43.107236 pipevcr-0.1.0/
--rw-------   0 spark      (501) staff       (20)     1083 2020-11-12 15:12:49.000000 pipevcr-0.1.0/LICENSE
--rw-r--r--   0 spark      (501) staff       (20)     1408 2022-10-11 17:51:43.107010 pipevcr-0.1.0/PKG-INFO
--rw-r--r--   0 spark      (501) staff       (20)     1158 2022-10-11 17:48:44.000000 pipevcr-0.1.0/README.md
--rwxr-xr-x   0 spark      (501) staff       (20)     2602 2022-10-11 17:46:17.000000 pipevcr-0.1.0/pipevcr
-drwxr-xr-x   0 spark      (501) staff       (20)        0 2022-10-11 17:51:43.106703 pipevcr-0.1.0/pipevcr.egg-info/
--rw-r--r--   0 spark      (501) staff       (20)     1408 2022-10-11 17:51:43.000000 pipevcr-0.1.0/pipevcr.egg-info/PKG-INFO
--rw-r--r--   0 spark      (501) staff       (20)      169 2022-10-11 17:51:43.000000 pipevcr-0.1.0/pipevcr.egg-info/SOURCES.txt
--rw-r--r--   0 spark      (501) staff       (20)        1 2022-10-11 17:51:43.000000 pipevcr-0.1.0/pipevcr.egg-info/dependency_links.txt
--rw-r--r--   0 spark      (501) staff       (20)        8 2022-10-11 17:51:43.000000 pipevcr-0.1.0/pipevcr.egg-info/top_level.txt
--rwxr-xr-x   0 spark      (501) staff       (20)     2602 2022-10-11 17:46:17.000000 pipevcr-0.1.0/pipevcr.py
--rw-r--r--   0 spark      (501) staff       (20)       38 2022-10-11 17:51:43.107313 pipevcr-0.1.0/setup.cfg
--rw-r--r--   0 spark      (501) staff       (20)      534 2022-10-11 17:46:46.000000 pipevcr-0.1.0/setup.py
+drwxr-xr-x   0 spark      (501) staff       (20)        0 2023-06-30 21:10:05.422208 pipevcr-0.1.1/
+-rw-------   0 spark      (501) staff       (20)     1083 2020-11-12 15:12:49.000000 pipevcr-0.1.1/LICENSE
+-rw-r--r--   0 spark      (501) staff       (20)     1408 2023-06-30 21:10:05.421946 pipevcr-0.1.1/PKG-INFO
+-rw-r--r--   0 spark      (501) staff       (20)     1158 2022-10-11 17:48:44.000000 pipevcr-0.1.1/README.md
+-rwxr-xr-x   0 spark      (501) staff       (20)     2705 2023-06-30 15:38:20.000000 pipevcr-0.1.1/pipevcr
+drwxr-xr-x   0 spark      (501) staff       (20)        0 2023-06-30 21:10:05.421619 pipevcr-0.1.1/pipevcr.egg-info/
+-rw-r--r--   0 spark      (501) staff       (20)     1408 2023-06-30 21:10:05.000000 pipevcr-0.1.1/pipevcr.egg-info/PKG-INFO
+-rw-r--r--   0 spark      (501) staff       (20)      169 2023-06-30 21:10:05.000000 pipevcr-0.1.1/pipevcr.egg-info/SOURCES.txt
+-rw-r--r--   0 spark      (501) staff       (20)        1 2023-06-30 21:10:05.000000 pipevcr-0.1.1/pipevcr.egg-info/dependency_links.txt
+-rw-r--r--   0 spark      (501) staff       (20)        8 2023-06-30 21:10:05.000000 pipevcr-0.1.1/pipevcr.egg-info/top_level.txt
+-rwxr-xr-x   0 spark      (501) staff       (20)     2705 2023-06-30 15:38:20.000000 pipevcr-0.1.1/pipevcr.py
+-rw-r--r--   0 spark      (501) staff       (20)       38 2023-06-30 21:10:05.422285 pipevcr-0.1.1/setup.cfg
+-rw-r--r--   0 spark      (501) staff       (20)      534 2023-06-30 15:40:10.000000 pipevcr-0.1.1/setup.py
```

### Comparing `pipevcr-0.1.0/LICENSE` & `pipevcr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipevcr-0.1.0/PKG-INFO` & `pipevcr-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipevcr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Record and play back pipes.
 Home-page: https://github.com/laktak/pipevcr
 Author: Christian Zangl
 Author-email: laktak@cdak.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pipevcr-0.1.0/README.md` & `pipevcr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pipevcr-0.1.0/pipevcr` & `pipevcr-0.1.1/pipevcr`

 * *Files 7% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             sys.stdout.fileno(), args.file, max_pause=args.max_pause, speed=args.speed
         )
 
     return 0
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(description=f"pipevcr - the linux pipe recorder")
 
     parser.add_argument("file", metavar="FILE", type=str, help="data file")
     parser.add_argument("-r", "--record", action="store_true", help="record pipe")
     parser.add_argument(
         "-s",
         "--speed",
@@ -88,8 +87,12 @@
         default=-1,
         help="max pause time between outputs in seconds",
     )
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
     else:
-        sys.exit(main(parser))
+        try:
+            sys.exit(main(parser))
+        except KeyboardInterrupt:
+            print("aborted")
+            sys.exit(1)
```

### Comparing `pipevcr-0.1.0/pipevcr.egg-info/PKG-INFO` & `pipevcr-0.1.1/pipevcr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipevcr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Record and play back pipes.
 Home-page: https://github.com/laktak/pipevcr
 Author: Christian Zangl
 Author-email: laktak@cdak.net
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pipevcr-0.1.0/pipevcr.py` & `pipevcr-0.1.1/pipevcr.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             sys.stdout.fileno(), args.file, max_pause=args.max_pause, speed=args.speed
         )
 
     return 0
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(description=f"pipevcr - the linux pipe recorder")
 
     parser.add_argument("file", metavar="FILE", type=str, help="data file")
     parser.add_argument("-r", "--record", action="store_true", help="record pipe")
     parser.add_argument(
         "-s",
         "--speed",
@@ -88,8 +87,12 @@
         default=-1,
         help="max pause time between outputs in seconds",
     )
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
     else:
-        sys.exit(main(parser))
+        try:
+            sys.exit(main(parser))
+        except KeyboardInterrupt:
+            print("aborted")
+            sys.exit(1)
```

### Comparing `pipevcr-0.1.0/setup.py` & `pipevcr-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="pipevcr",
-    version="0.1.0",
+    version="0.1.1",
     url="https://github.com/laktak/pipevcr",
     author="Christian Zangl",
     author_email="laktak@cdak.net",
     description="Record and play back pipes.",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=[],
```

