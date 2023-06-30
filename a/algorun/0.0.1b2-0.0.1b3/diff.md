# Comparing `tmp/algorun-0.0.1b2-py3-none-any.whl.zip` & `tmp/algorun-0.0.1b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 20672 bytes, number of entries: 25
+Zip file size: 20713 bytes, number of entries: 25
 -rw-r--r--  2.0 unx     1168 b- defN 80-Jan-01 00:00 algorun/__init__.py
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 algorun/__main__.py
 -rw-r--r--  2.0 unx     1008 b- defN 80-Jan-01 00:00 algorun/cli/__init__.py
 -rw-r--r--  2.0 unx      295 b- defN 80-Jan-01 00:00 algorun/cli/config.py
 -rw-r--r--  2.0 unx     2515 b- defN 80-Jan-01 00:00 algorun/cli/goal.py
 -rw-r--r--  2.0 unx      970 b- defN 80-Jan-01 00:00 algorun/cli/reset.py
 -rw-r--r--  2.0 unx     2622 b- defN 80-Jan-01 00:00 algorun/cli/start.py
@@ -15,13 +15,13 @@
 -rw-r--r--  2.0 unx     5128 b- defN 80-Jan-01 00:00 algorun/core/log_handlers.py
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 algorun/core/proc.py
 -rw-r--r--  2.0 unx     1970 b- defN 80-Jan-01 00:00 algorun/core/questionary_extensions.py
 -rw-r--r--  2.0 unx     4844 b- defN 80-Jan-01 00:00 algorun/core/sandbox.py
 -rw-r--r--  2.0 unx      508 b- defN 80-Jan-01 00:00 algorun/core/utils.py
 -rw-r--r--  2.0 unx     4170 b- defN 80-Jan-01 00:00 algorun/core/version_prompt.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algorun/py.typed
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3214 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algorun-0.0.1b2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1977 b- defN 16-Jan-01 00:00 algorun-0.0.1b2.dist-info/RECORD
-25 files, 44062 bytes uncompressed, 17506 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algorun-0.0.1b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3294 b- defN 80-Jan-01 00:00 algorun-0.0.1b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algorun-0.0.1b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algorun-0.0.1b3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1977 b- defN 16-Jan-01 00:00 algorun-0.0.1b3.dist-info/RECORD
+25 files, 44142 bytes uncompressed, 17547 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: algorun/core/version_prompt.py
 Comment: 
 
 Filename: algorun/py.typed
 Comment: 
 
-Filename: algorun-0.0.1b2.dist-info/LICENSE
+Filename: algorun-0.0.1b3.dist-info/LICENSE
 Comment: 
 
-Filename: algorun-0.0.1b2.dist-info/METADATA
+Filename: algorun-0.0.1b3.dist-info/METADATA
 Comment: 
 
-Filename: algorun-0.0.1b2.dist-info/WHEEL
+Filename: algorun-0.0.1b3.dist-info/WHEEL
 Comment: 
 
-Filename: algorun-0.0.1b2.dist-info/entry_points.txt
+Filename: algorun-0.0.1b3.dist-info/entry_points.txt
 Comment: 
 
-Filename: algorun-0.0.1b2.dist-info/RECORD
+Filename: algorun-0.0.1b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `algorun-0.0.1b2.dist-info/LICENSE` & `algorun-0.0.1b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algorun-0.0.1b2.dist-info/METADATA` & `algorun-0.0.1b3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorun
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Algorand development kit command-line interface
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,16 @@
 
 The key required dependency is Python 3.10+, but some of the installation options below will install that for you.
 
 Algorun also has some runtime dependencies that also need to be available for particular commands.
 
 - Docker - Docker Compose (and by association, Docker) is used to run the Algorand mainnet container, we require Docker Compose 2.5.0+
 
+- Pipx - a better package manager than pip that you'll use to install the cli
+
 ## Install Algorun with pipx on any Mac, Linux and Windows subsystem for Linux
 
 1. Ensure desired prerequisites are installed
 
    - [Python 3.10+](https://www.python.org/downloads/)
    - [pipx](https://pypa.github.io/pipx/installation/)
    - [Docker](https://docs.docker.com/get-docker/)
@@ -66,15 +68,15 @@
 ## Usage
 
 Create a directory where you're comfortable keeping the node config and files, we suggest naming it `algorand`, open that directory in a terminal
 
 - `algorun start` will start your node by creating `docker-compose.yml`, `config.json` files and a `data` directory where your node will persist.
 - `algorun stop` will shut down your node
 - `algorun goal` is a wrapper for the [Goal CLI](https://developer.algorand.org/docs/clis/goal/goal/)
-- typing `algorun goal node status` will return your nodes status typing `algorun goal node status -w 1000` instead will keep giving you node status updates every 1 second
+- typing `algorun goal node status` will return your nodes status, typing `algorun goal node status -w 1000` instead will keep giving you node status updates every 1 second
 
 > **Note**
 > If you get receive one of the following errors:
 >
 > - `command not found: algorun` (bash/zsh)
 > - `The term 'algorun' is not recognized as the name of a cmdlet, function, script file, or operable program.` (PowerShell)
 >
```

## Comparing `algorun-0.0.1b2.dist-info/RECORD` & `algorun-0.0.1b3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 algorun/core/log_handlers.py,sha256=IT9mo8NhiLl2rzH6t6F9kEflmmFbOfOhKaPzRp7CVTM,5128
 algorun/core/proc.py,sha256=UsMC8ysyjVZ2Ql8dzodK2qS_PaH_U9rUviZQw_vbE80,3520
 algorun/core/questionary_extensions.py,sha256=QvUGXL_GxcPvdGemy_5-Fza4d1PSJ2ml7aZAS3r4M20,1970
 algorun/core/sandbox.py,sha256=RnNVAslpgUI6xODkiBhBfKn-yW5kywCIYAZRBbNnQIQ,4844
 algorun/core/utils.py,sha256=hgemlB8znOsGCO090BQOydnbq4ZRAsD9CzMbApEMGY8,508
 algorun/core/version_prompt.py,sha256=Tixd0RZEcDTv1-sSopG8ngLvP4MZjRgKO8QQtiDnGEQ,4170
 algorun/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algorun-0.0.1b2.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
-algorun-0.0.1b2.dist-info/METADATA,sha256=HavFocgU5ty15osQKWwvKla_vrSjCQz-BM6EKX6qocQ,3214
-algorun-0.0.1b2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algorun-0.0.1b2.dist-info/entry_points.txt,sha256=fxs3JmtSLlx0RPAWt5Sj7MiHmnuQWxeNiZpL1xLX4-g,47
-algorun-0.0.1b2.dist-info/RECORD,,
+algorun-0.0.1b3.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
+algorun-0.0.1b3.dist-info/METADATA,sha256=w-gWXOomT-eaYbW9neodsNp0qVLWQY2QdJP37-W_nWk,3294
+algorun-0.0.1b3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algorun-0.0.1b3.dist-info/entry_points.txt,sha256=fxs3JmtSLlx0RPAWt5Sj7MiHmnuQWxeNiZpL1xLX4-g,47
+algorun-0.0.1b3.dist-info/RECORD,,
```

