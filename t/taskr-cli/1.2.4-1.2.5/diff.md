# Comparing `tmp/taskr_cli-1.2.4-py3-none-any.whl.zip` & `tmp/taskr_cli-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14838 bytes, number of entries: 13
+Zip file size: 14972 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       61 b- defN 23-Jan-18 04:37 taskr/__init__.py
 -rw-r--r--  2.0 unx       78 b- defN 23-Jan-18 04:37 taskr/__version__.py
 -rw-r--r--  2.0 unx     1995 b- defN 23-Mar-05 18:49 taskr/cli.py
 -rw-r--r--  2.0 unx     2709 b- defN 23-Jan-18 04:37 taskr/runners.py
 -rw-r--r--  2.0 unx     8853 b- defN 23-Mar-05 18:49 taskr/taskr.py
 -rw-r--r--  2.0 unx     1950 b- defN 23-Jan-18 04:37 taskr/template.py
--rw-r--r--  2.0 unx     5454 b- defN 23-Jun-20 04:11 taskr/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     9159 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      997 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/RECORD
-13 files, 32464 bytes uncompressed, 13186 bytes compressed:  59.4%
+-rw-r--r--  2.0 unx     5762 b- defN 23-Jun-30 03:17 taskr/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-30 03:17 taskr_cli-1.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9220 b- defN 23-Jun-30 03:17 taskr_cli-1.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 03:17 taskr_cli-1.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-30 03:17 taskr_cli-1.2.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-30 03:17 taskr_cli-1.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      997 b- defN 23-Jun-30 03:17 taskr_cli-1.2.5.dist-info/RECORD
+13 files, 32833 bytes uncompressed, 13320 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: taskr/template.py
 Comment: 
 
 Filename: taskr/utils.py
 Comment: 
 
-Filename: taskr_cli-1.2.4.dist-info/LICENSE
+Filename: taskr_cli-1.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: taskr_cli-1.2.4.dist-info/METADATA
+Filename: taskr_cli-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: taskr_cli-1.2.4.dist-info/WHEEL
+Filename: taskr_cli-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: taskr_cli-1.2.4.dist-info/entry_points.txt
+Filename: taskr_cli-1.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: taskr_cli-1.2.4.dist-info/top_level.txt
+Filename: taskr_cli-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: taskr_cli-1.2.4.dist-info/RECORD
+Filename: taskr_cli-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taskr/utils.py

```diff
@@ -58,14 +58,29 @@
 def inVenv() -> bool:
     """
     Let's you know if you're in a virtual environment or not.
     """
     return sys.prefix != sys.base_prefix or os.environ.get("VIRTUAL_ENV") is not None
 
 
+def inContainer() -> bool:
+    """
+    Are we running in docker or not
+    """
+
+    path = '/proc/self/cgroup'
+
+    return (
+        os.path.exists("/run/.containerenv")
+        or os.path.exists('/.dockerenv')
+        or os.path.isfile(path)
+        and any('docker' in line for line in open(path))
+    )
+
+
 def readEnvFile(filename: str) -> Dict[str, str]:
     """
     Reads in a file of ENV settings and returns a Dict
     Ana alternative way of running 'source vars.env' before a command
     """
     if not os.path.exists(filename):
         print(f"Environment File {filename} not found")
```

## Comparing `taskr_cli-1.2.4.dist-info/LICENSE` & `taskr_cli-1.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `taskr_cli-1.2.4.dist-info/METADATA` & `taskr_cli-1.2.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskr-cli
-Version: 1.2.4
+Version: 1.2.5
 Summary: A language agnostic make-like tool meant for python projects
 Author-email: Kyle Peasley <Kyle.Peasley@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kyle Peasley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -202,15 +202,15 @@
 
 ```python
 from taskr import runners
 
 # Get the number of env variables
 def get_count():
     ret = runners.run_output("env | wc -l")
-    print(ret.status) # True 
+    print(ret.status) # True
     print(ret.stdout) # "90"
     print(ret.sterr)  # ""
 ```
 
 You can an environment dict to this function.
 
 ## Passing arguments to functions
@@ -269,14 +269,17 @@
 
 # Remove compiled files and folders (.pyc, __pycache__)
 utils.cleanCompiles()
 
 # In a venv or not
 utils.inVenv()
 
+# In a container (docker, podman) or not
+utils.inContainer()
+
 # Transforms an ENV file into a dict
 utils.readEnvFile(filename = None)
 
 # Bumps setup.py's version number by 0.0.1, or replaces it with argument
 utils.bumpVersion(version = None, variable = "version", filename = "setup.py"):
 
 # Adds `export TASKR_DIR=CWD' to your VENV activation, so
```

## Comparing `taskr_cli-1.2.4.dist-info/RECORD` & `taskr_cli-1.2.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 taskr/__init__.py,sha256=HYyXgZ4SQ_RWUTv3TM7IBKVz0_daPGS1MdmjNkBVHRs,61
 taskr/__version__.py,sha256=UpLk4osKJTqB53nr1gFoPa9lNzecaM2WpL_-opMzswY,78
 taskr/cli.py,sha256=OXD0e-vNJ_5HGyN8blfP5iKLY6dc8kxmgrKr-G57JwM,1995
 taskr/runners.py,sha256=dQxljblRsvDWtE7s_9nzeNAMTj_xNEk3cR7pP9SVCMI,2709
 taskr/taskr.py,sha256=Y1uUr6JN-auSfB6X2l8m2sRnn17mgmF5mKinYVr95VU,8853
 taskr/template.py,sha256=uzT2HlbPJcL-OlYaxrpm5mmIbS2RnaypxV55_p3u3io,1950
-taskr/utils.py,sha256=RQOP159B14eL0wCWNrzVpA0MvXUtwro7Ccox-dtbC2Q,5454
-taskr_cli-1.2.4.dist-info/LICENSE,sha256=r-dZ3nX2dvIGBQgIGllf9ITlGguIqi8OqBm-x6oWS7U,1069
-taskr_cli-1.2.4.dist-info/METADATA,sha256=SzwZNbmUU4YcMB8ypdUNP0YsGDCKPNeU9gqwSXpR2zA,9159
-taskr_cli-1.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-taskr_cli-1.2.4.dist-info/entry_points.txt,sha256=Mc2MUGWo4v25gpWXBZVzox8NklMvXZQt352WLhs9oiA,41
-taskr_cli-1.2.4.dist-info/top_level.txt,sha256=nUs61tNfbfharkZ-iKd9ugpnblA61ctB_cj3yljwmPs,6
-taskr_cli-1.2.4.dist-info/RECORD,,
+taskr/utils.py,sha256=SFoy8hzuW1XHXRBKfYr4WdoI2snIWCyD56jSG4RZAz4,5762
+taskr_cli-1.2.5.dist-info/LICENSE,sha256=r-dZ3nX2dvIGBQgIGllf9ITlGguIqi8OqBm-x6oWS7U,1069
+taskr_cli-1.2.5.dist-info/METADATA,sha256=ElWiMRKWw1HRbuM8auaQq04gifiA7Ge9g4tvI591jC4,9220
+taskr_cli-1.2.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+taskr_cli-1.2.5.dist-info/entry_points.txt,sha256=Mc2MUGWo4v25gpWXBZVzox8NklMvXZQt352WLhs9oiA,41
+taskr_cli-1.2.5.dist-info/top_level.txt,sha256=nUs61tNfbfharkZ-iKd9ugpnblA61ctB_cj3yljwmPs,6
+taskr_cli-1.2.5.dist-info/RECORD,,
```

