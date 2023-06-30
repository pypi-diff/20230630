# Comparing `tmp/asplode-0.0.5.tar.gz` & `tmp/asplode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asplode-0.0.5.tar", last modified: Tue Aug  3 21:18:42 2021, max compression
+gzip compressed data, was "asplode-1.0.0.tar", last modified: Fri Jun 30 21:25:51 2023, max compression
```

## Comparing `asplode-0.0.5.tar` & `asplode-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brent      (502) staff       (20)        0 2021-08-03 21:18:42.251455 asplode-0.0.5/
--rw-r--r--   0 brent      (502) staff       (20)    11357 2021-07-09 18:47:25.000000 asplode-0.0.5/LICENSE
--rw-r--r--   0 brent      (502) staff       (20)      505 2021-08-03 21:18:42.251172 asplode-0.0.5/PKG-INFO
--rw-r--r--   0 brent      (502) staff       (20)       42 2021-08-03 21:17:53.000000 asplode-0.0.5/README.md
-drwxr-xr-x   0 brent      (502) staff       (20)        0 2021-08-03 21:18:42.250786 asplode-0.0.5/asplode.egg-info/
--rw-r--r--   0 brent      (502) staff       (20)      505 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/PKG-INFO
--rw-r--r--   0 brent      (502) staff       (20)      255 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (502) staff       (20)        1 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (502) staff       (20)       42 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/entry_points.txt
--rw-r--r--   0 brent      (502) staff       (20)        1 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/not-zip-safe
--rw-r--r--   0 brent      (502) staff       (20)        5 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/requires.txt
--rw-r--r--   0 brent      (502) staff       (20)        8 2021-08-03 21:18:42.000000 asplode-0.0.5/asplode.egg-info/top_level.txt
--rw-r--r--   0 brent      (502) staff       (20)     4030 2021-07-28 16:49:21.000000 asplode-0.0.5/asplode.py
--rw-r--r--   0 brent      (502) staff       (20)       38 2021-08-03 21:18:42.251537 asplode-0.0.5/setup.cfg
--rw-r--r--   0 brent      (502) staff       (20)      765 2021-08-03 21:18:34.000000 asplode-0.0.5/setup.py
+drwxr-xr-x   0 brent      (502) staff       (20)        0 2023-06-30 21:25:51.294404 asplode-1.0.0/
+-rw-r--r--   0 brent      (502) staff       (20)    11357 2021-07-09 18:47:25.000000 asplode-1.0.0/LICENSE
+-rw-r--r--   0 brent      (502) staff       (20)      510 2023-06-30 21:25:51.294134 asplode-1.0.0/PKG-INFO
+-rw-r--r--   0 brent      (502) staff       (20)      624 2023-06-30 20:55:30.000000 asplode-1.0.0/README.md
+drwxr-xr-x   0 brent      (502) staff       (20)        0 2023-06-30 21:25:51.293727 asplode-1.0.0/asplode.egg-info/
+-rw-r--r--   0 brent      (502) staff       (20)      510 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (502) staff       (20)      255 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (502) staff       (20)        1 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (502) staff       (20)       41 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/entry_points.txt
+-rw-r--r--   0 brent      (502) staff       (20)        1 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/not-zip-safe
+-rw-r--r--   0 brent      (502) staff       (20)        5 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/requires.txt
+-rw-r--r--   0 brent      (502) staff       (20)        8 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/top_level.txt
+-rw-r--r--   0 brent      (502) staff       (20)     4122 2023-06-30 20:50:08.000000 asplode-1.0.0/asplode.py
+-rw-r--r--   0 brent      (502) staff       (20)       38 2023-06-30 21:25:51.294493 asplode-1.0.0/setup.cfg
+-rw-r--r--   0 brent      (502) staff       (20)      778 2023-06-30 21:24:57.000000 asplode-1.0.0/setup.py
```

### Comparing `asplode-0.0.5/LICENSE` & `asplode-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asplode-0.0.5/asplode.py` & `asplode-1.0.0/asplode.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,121 +1,132 @@
 import os
 import gzip
 import tarfile
 import datetime
 import re
 import shutil
 from zipfile import ZipFile, BadZipfile
+from pathlib import Path
+
 
 import plac
 
 
 # plac annotation format
 # arg = (help, kind, abbrev, type, choices, metavar)
-@plac.annotations(name =    ("Path to the archive file",
-                             "positional", None, str, None, "ARCHIVE"))
-@plac.annotations(verbose = ("Enable verbose output",
-                             "flag", "v", None, None, None))
-@plac.annotations(cd =      ("Directory to change to before extraction, ala tar",
-                             "option", "C", None, str, "DIRECTORY"))
-def asplode(name, verbose=False, cd="."):
-    name = os.path.abspath(name)
-    start_dir = os.path.abspath(cd)
+@plac.flg("verbose", "Enable verbose output")
+@plac.pos("name", "Path to the archive file", type=Path, metavar="ARCHIVE")
+@plac.opt("cd", "Directory to change to before extraction, ala tar (default: .)", abbrev="C", metavar="DIR")
+@plac.opt("level", "Levels of recursion (default: 0, infinite)", type=int)
+def asplode(name, verbose=False, cd=Path("."), level=0):
+    end_recursion = False
+
+    if level > 0:
+        level -= 1
+        if level == 0:
+            end_recursion = True
+
+    raw_exts = r'zip|tar|tgz|tar\.gz|tar\.bz2|tar\.bz|gz'
+    archive_exts = set(raw_exts.replace("\\", "").split("|"))
 
-    if not os.path.isfile(name):
+    start_dir = Path(".").absolute()
+    name = Path(name)
+
+    if not name.is_file():
         return 1
 
     # Match on the filename
     # [base].[ext]
     # where ext is one of zip, tar, gz, tgz, tar.gz, or tar.bz2
-    m = re.match(
-        r'^(?P<base>.*?)[.](?P<ext>zip|tar|tgz|tar\.gz|tar\.bz2|tar\.bz|gz)$', name)
+    m = re.match(r'^(?P<base>.*?)[.](?P<ext>' + raw_exts + r')$',
+                 str(name.absolute()))
+
     if not m:
         # Not a compressed file that we're going to try to extract
         return 1
 
     if verbose:
-        print(f' Extracting {name}')
+        print(f' Extracting {name.name}')
 
-    basepath, ext = m.groups()
-    basename = os.path.basename(basepath)
+    basepath = Path(m.groups()[0])
+    ext = m.groups()[1]
 
     try:
         if ext == 'zip':
             cfile = ZipFile(name)
         elif ext == 'gz':
             cfile = gzip.open(name, 'r')
         else:
             cfile = tarfile.open(name, 'r:*')
     except (IOError, tarfile.ReadError, BadZipfile):
         print(f' Error reading file for extraction {name}')
         return
 
     try:
         # extract to a dir of its own to start with.
-        extract_dir = datetime.datetime.now().isoformat()
+        extract_dir = Path(datetime.datetime.now().isoformat())
         if ext == 'gz':
-            os.makedirs(extract_dir)
-            f = open(os.path.join(extract_dir, basename), 'wb')
+            extract_dir.mkdir()
+            f = open(extract_dir / basepath.name, 'wb')
             chunk = 1024*8
             buff = cfile.read(chunk)
             while buff:
                 f.write(buff)
                 buff = cfile.read(chunk)
             f.close()
         else:
-            cfile.extractall(extract_dir)
+            cfile.extractall(extract_dir.name)
     except OSError:
         print(f' Error extracting {name}')
         return
     finally:
         cfile.close()
 
     # If there's no directory at all, then it was probably an empty archive
-    if not os.path.isdir(extract_dir):
+    if not extract_dir.is_dir():
         return
 
     try:
-        extract_files = os.listdir(extract_dir)
-        if len(extract_files) == 1 and extract_files[0] == basename:
-            # If there's only one file/dir in the dir, and that file/dir
-            # matches the base name of the archive, move the file/dir back one
-            # into the parent dir and remove the extract directory.
-            # The classic tar.gz -> dir and txt.gz -> file cases.
-            shutil.move(os.path.join(extract_dir, extract_files[0]), start_dir)
-            shutil.rmtree(extract_dir)
+        extract_files = [f for f in list(extract_dir.glob("*")) if f != extract_dir]
+        if len(extract_files) == 1:
+            # If there's only one file/dir in the dir, move the file/dir back
+            # one into the parent dir and remove the extract directory.  The
+            # classic tar.gz -> dir and txt.gz -> file cases.
+            shutil.move(extract_files[0], str(start_dir))
+            shutil.rmtree(extract_dir.name)
 
             # Set the name of the extracted dir for recursive decompression
-            extract_dir = extract_files[0]
+            extract_dir = start_dir / Path(extract_files[0].name)
         else:
-            # If there's more than one file in the dir, or if that file/dir
-            # doesn't match the base name of the archive rename the extract dir
-            # to the basename of the archive.
-            # The 'barfing files all over pwd' case, the 'archive contains
-            # var/log/blah/blah' case, and the 'archive contains a single,
-            # differently named file' case.
-            shutil.move(os.path.join(extract_dir), basename)
+            # If there's more than one file in the dir, rename the extract dir
+            # to the basename of the archive. The 'barfing files all over pwd'
+            # case, the 'archive contains usr/bin and var/log/blah/blah and
+            # etc' case.
+            shutil.move(extract_dir.name, basepath.name)
 
             # Set the name of the extracted dir for recursive decompression
             extract_dir = basepath
     except shutil.Error as e:
         print(' Error arranging directories:')
         print(' ' + e)
         return
 
     # See if there's anything left to do
-    if not os.path.isdir(extract_dir):
+    if end_recursion or not extract_dir.is_dir():
         return
 
-    # Get a list of files for recursive decompression
-    sub_files = os.listdir(extract_dir)
+    # Get a list of files for recursive decompression.
+    sub_files = []
+    for path in extract_dir.glob(r'*'):
+        if path.suffix[1:] in archive_exts:
+            sub_files.append(path)
 
     # Extract anything compressed that this archive had in it.
     os.chdir(extract_dir)
     for sub_file in sub_files:
-        asplode(sub_file)
-    os.chdir(start_dir)
+        asplode(sub_file, level=level)
+    os.chdir(str(start_dir))
 
 
 def main(argv=None):
     plac.call(asplode)
     return 0
```

### Comparing `asplode-0.0.5/setup.py` & `asplode-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name="asplode",
-    version="0.0.5",
+    version="1.0.0",
     description="Recursively decompress archives",
     long_description="Recursively decompress archives",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Utilities",
     ],
     keywords="decompression archives zip gzip tar",
     author="Brent Woodruff",
     author_email="brent@fprimex.com",
```

