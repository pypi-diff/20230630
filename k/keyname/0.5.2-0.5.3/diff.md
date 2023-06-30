# Comparing `tmp/keyname-0.5.2.tar.gz` & `tmp/keyname-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyname-0.5.2.tar", last modified: Sun Feb  5 20:27:54 2023, max compression
+gzip compressed data, was "keyname-0.5.3.tar", last modified: Fri Jun 30 00:10:44 2023, max compression
```

## Comparing `keyname-0.5.2.tar` & `keyname-0.5.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-05 20:27:54.770833 keyname-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-02-05 20:27:51.000000 keyname-0.5.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-02-05 20:27:51.000000 keyname-0.5.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-02-05 20:27:51.000000 keyname-0.5.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-02-05 20:27:51.000000 keyname-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-02-05 20:27:51.000000 keyname-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10130 2023-02-05 20:27:54.770833 keyname-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9200 2023-02-05 20:27:51.000000 keyname-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-05 20:27:54.766833 keyname-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)     4836 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-02-05 20:27:51.000000 keyname-0.5.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-05 20:27:54.766833 keyname-0.5.2/keyname/
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-02-05 20:27:51.000000 keyname-0.5.2/keyname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-02-05 20:27:51.000000 keyname-0.5.2/keyname/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-02-05 20:27:51.000000 keyname-0.5.2/keyname/keyname.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-02-05 20:27:51.000000 keyname-0.5.2/keyname/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-05 20:27:54.770833 keyname-0.5.2/keyname.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10130 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-05 20:27:54.000000 keyname-0.5.2/keyname.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-02-05 20:27:54.770833 keyname-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-02-05 20:27:51.000000 keyname-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-05 20:27:54.770833 keyname-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-02-05 20:27:51.000000 keyname-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8003 2023-02-05 20:27:51.000000 keyname-0.5.2/tests/test_keyname.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 00:10:44.559964 keyname-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-06-30 00:10:40.000000 keyname-0.5.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-30 00:10:40.000000 keyname-0.5.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-30 00:10:40.000000 keyname-0.5.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-30 00:10:40.000000 keyname-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-30 00:10:40.000000 keyname-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10198 2023-06-30 00:10:44.559964 keyname-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9268 2023-06-30 00:10:40.000000 keyname-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 00:10:44.555964 keyname-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4836 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-06-30 00:10:40.000000 keyname-0.5.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 00:10:44.555964 keyname-0.5.3/keyname/
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-06-30 00:10:40.000000 keyname-0.5.3/keyname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-06-30 00:10:40.000000 keyname-0.5.3/keyname/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-06-30 00:10:40.000000 keyname-0.5.3/keyname/keyname.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-06-30 00:10:40.000000 keyname-0.5.3/keyname/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 00:10:44.559964 keyname-0.5.3/keyname.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10198 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-30 00:10:44.000000 keyname-0.5.3/keyname.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-30 00:10:44.559964 keyname-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1618 2023-06-30 00:10:40.000000 keyname-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 00:10:44.559964 keyname-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-30 00:10:40.000000 keyname-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8003 2023-06-30 00:10:40.000000 keyname-0.5.3/tests/test_keyname.py
```

### Comparing `keyname-0.5.2/CONTRIBUTING.rst` & `keyname-0.5.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/LICENSE` & `keyname-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/PKG-INFO` & `keyname-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyname
-Version: 0.5.2
+Version: 0.5.3
 Summary: Easily pack and unpack metadata in a filename.
 Home-page: https://github.com/mmore500/keyname
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Keywords: keyname
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -83,14 +83,15 @@
 
 Most operating systems only allow filename lengths of up to 255 characters.
 (And in Docker containers, the limit is sometimes 224 characters.)
 Trying to use longer filenames will fail.
 
 Keyname provides tools to work around this restriction by chunking overlength filenames into nested directories and a file.
 (Basically, using the path to store the filename.)
+Path segments with continuations are denoted with the suffix "...".
 
 .. code-block:: python3
 
   from pathlib import Path
 
   from keyname import keyname as kn
```

### Comparing `keyname-0.5.2/README.rst` & `keyname-0.5.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 Most operating systems only allow filename lengths of up to 255 characters.
 (And in Docker containers, the limit is sometimes 224 characters.)
 Trying to use longer filenames will fail.
 
 Keyname provides tools to work around this restriction by chunking overlength filenames into nested directories and a file.
 (Basically, using the path to store the filename.)
+Path segments with continuations are denoted with the suffix "...".
 
 .. code-block:: python3
 
   from pathlib import Path
 
   from keyname import keyname as kn
```

### Comparing `keyname-0.5.2/docs/Makefile` & `keyname-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/docs/conf.py` & `keyname-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/docs/installation.rst` & `keyname-0.5.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/docs/make.bat` & `keyname-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/docs/usage.rst` & `keyname-0.5.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/keyname/cli.py` & `keyname-0.5.3/keyname/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,8 +132,8 @@
     subprocess.run(" ".join([
         "echo", stash,
         ">", dest + ".meta"
     ]), shell=True, stdout=subprocess.DEVNULL)
     click.echo("created metadata file " + dest + ".meta")
 
 if __name__ == "__main__":
-    sys.exit(cli())  # pragma: no cover
+    sys.exit(main())  # pragma: no cover
```

### Comparing `keyname-0.5.2/keyname/keyname.py` & `keyname-0.5.3/keyname/keyname.py`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/keyname.egg-info/PKG-INFO` & `keyname-0.5.3/keyname.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyname
-Version: 0.5.2
+Version: 0.5.3
 Summary: Easily pack and unpack metadata in a filename.
 Home-page: https://github.com/mmore500/keyname
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Keywords: keyname
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -83,14 +83,15 @@
 
 Most operating systems only allow filename lengths of up to 255 characters.
 (And in Docker containers, the limit is sometimes 224 characters.)
 Trying to use longer filenames will fail.
 
 Keyname provides tools to work around this restriction by chunking overlength filenames into nested directories and a file.
 (Basically, using the path to store the filename.)
+Path segments with continuations are denoted with the suffix "...".
 
 .. code-block:: python3
 
   from pathlib import Path
 
   from keyname import keyname as kn
```

### Comparing `keyname-0.5.2/keyname.egg-info/SOURCES.txt` & `keyname-0.5.3/keyname.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyname-0.5.2/setup.py` & `keyname-0.5.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords='keyname',
     name='keyname',
     packages=find_packages(include=['keyname']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mmore500/keyname',
-    version='0.5.2',
+    version='0.5.3',
     zip_safe=False,
 )
```

### Comparing `keyname-0.5.2/tests/test_keyname.py` & `keyname-0.5.3/tests/test_keyname.py`

 * *Files identical despite different names*

