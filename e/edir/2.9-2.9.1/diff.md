# Comparing `tmp/edir-2.9.tar.gz` & `tmp/edir-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edir-2.9.tar", last modified: Wed Dec 15 23:40:39 2021, max compression
+gzip compressed data, was "edir-2.9.1.tar", last modified: Wed Dec 15 23:59:28 2021, max compression
```

## Comparing `edir-2.9.tar` & `edir-2.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-12-15 23:40:39.584135 edir-2.9/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2020-06-17 09:41:57.000000 edir-2.9/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-04-04 23:25:32.000000 edir-2.9/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)     1195 2021-01-27 05:34:22.000000 edir-2.9/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    15328 2021-12-15 23:40:39.584135 edir-2.9/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    14930 2021-10-29 03:33:42.000000 edir-2.9/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-12-15 23:40:39.584135 edir-2.9/edir.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    15328 2021-12-15 23:40:39.000000 edir-2.9/edir.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      224 2021-12-15 23:40:39.000000 edir-2.9/edir.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-12-15 23:40:39.000000 edir-2.9/edir.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       36 2021-12-15 23:40:39.000000 edir-2.9/edir.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        5 2021-12-15 23:40:39.000000 edir-2.9/edir.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        5 2021-12-15 23:40:39.000000 edir-2.9/edir.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)    15844 2021-12-15 23:39:39.000000 edir-2.9/edir.py
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2021-12-15 23:40:39.584135 edir-2.9/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)      973 2021-12-15 23:40:01.000000 edir-2.9/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-12-15 23:59:28.136649 edir-2.9.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2020-06-17 09:41:57.000000 edir-2.9.1/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-04-04 23:25:32.000000 edir-2.9.1/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)     1195 2021-01-27 05:34:22.000000 edir-2.9.1/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    15523 2021-12-15 23:59:28.136649 edir-2.9.1/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    15123 2021-12-15 23:57:31.000000 edir-2.9.1/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2021-12-15 23:59:28.133315 edir-2.9.1/edir.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    15523 2021-12-15 23:59:28.000000 edir-2.9.1/edir.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      224 2021-12-15 23:59:28.000000 edir-2.9.1/edir.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2021-12-15 23:59:28.000000 edir-2.9.1/edir.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       36 2021-12-15 23:59:28.000000 edir-2.9.1/edir.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        5 2021-12-15 23:59:28.000000 edir-2.9.1/edir.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        5 2021-12-15 23:59:28.000000 edir-2.9.1/edir.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)    15844 2021-12-15 23:39:39.000000 edir-2.9.1/edir.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2021-12-15 23:59:28.136649 edir-2.9.1/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)      975 2021-12-15 23:58:25.000000 edir-2.9.1/setup.py
```

### Comparing `edir-2.9/Makefile` & `edir-2.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `edir-2.9/PKG-INFO` & `edir-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edir
-Version: 2.9
+Version: 2.9.1
 Summary: Utility to rename, remove, and copy files/dirs using your editor
 Home-page: https://github.com/bulletmark/edir
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: vidir
 Platform: UNKNOWN
@@ -125,45 +125,49 @@
 14. `edir` adds a [`-t/--trash` option](#using-trash) to delete to your
     [Trash](https://specifications.freedesktop.org/trash-spec/trashspec-1.0.html).
     This option invokes
     [`trash-put`](https://www.mankier.com/1/trash-put) from the
     [trash-cli](https://github.com/andreafrancia/trash-cli) package to do
     deletions.
 
-15. `edir` shows a message "No files or directories" if there is nothing
+15. `edir` adds `-N/--sort-name, -I/--sort-time, -S/--sort-size` options
+    to sort the paths when listed in your editor. There is also a
+    `-E/--sort-reverse` option to reverse the order.
+
+16. `edir` shows a message "No files or directories" if there is nothing
     to edit, rather than opening an empty file to edit.
 
-16. `edir` filters out any duplicate paths you may inadvertently specify
+17. `edir` filters out any duplicate paths you may inadvertently specify
     on it's command line.
 
-17. `edir` always invokes a consistent duplicate renaming scheme. E.g. if
+18. `edir` always invokes a consistent duplicate renaming scheme. E.g. if
     you rename `b`, `c`, `d` all to the same pre-existing name `a` then
     `edir` will rename `b` to `a~`, `c` to `a~1`, `d` to `a~2`.
     Depending on order of operations, `vidir` is not always consistent
     about this, E.g. sometimes it creates a `a~1` with no `a~` (this may
     be a bug in `vidir` that nobody has ever bothered to
     report/address?).
 
-18. `edir` creates the temporary editing file with a `.sh` suffix so
+19. `edir` creates the temporary editing file with a `.sh` suffix so
     your EDITOR may syntax highlight the entries. Optionally, you can
     change this default suffix.
 
-19. `edir` provides an optional environment value to add custom options
+20. `edir` provides an optional environment value to add custom options
     to the invocation of your editor. See [section
     below](#edir_editor-environment-variable).
 
-20. `edir` provides an optional configuration file to set default `edir`
+21. `edir` provides an optional configuration file to set default `edir`
     command line arguments. See [section
     below](#edir-command-default-arguments).
 
-21. Contrary to what it's name implies, `vidir` actually respects your
+22. Contrary to what it's name implies, `vidir` actually respects your
     `$EDITOR` variable and runs your preferred editor like `edir` does
     but `edir` has been given a generic name to make this more apparent.
 
-22. `edir` is very strict about the format of the lines you edit and
+23. `edir` is very strict about the format of the lines you edit and
     immediately exits with an error message (before changing anything)
     if you format one of the lines incorrectly. All lines in the edited
     list:
 
     1. Must start with a number and that number must be in range.
     2. Must have at least one white space/tab after the number,
     3. Must have a remaining valid path name.
@@ -171,15 +175,15 @@
        same as deleted.
 
     Note the final edited order of lines does not matter, only the first
     number value is used to match the newly edited line to the original
     line so an easy way to swap two file names is just to swap their
     numbers.
 
-23. `edir` always actions files consistently. The sequence of
+24. `edir` always actions files consistently. The sequence of
      operations applied is:
 
     1. Deleted files are removed and all renamed files and directories
        are renamed to temporaries. The temporaries are made on the same
        file-system as the target.
  
     2. Empty deleted directories are removed.
```

### Comparing `edir-2.9/README.md` & `edir-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,45 +111,49 @@
 14. `edir` adds a [`-t/--trash` option](#using-trash) to delete to your
     [Trash](https://specifications.freedesktop.org/trash-spec/trashspec-1.0.html).
     This option invokes
     [`trash-put`](https://www.mankier.com/1/trash-put) from the
     [trash-cli](https://github.com/andreafrancia/trash-cli) package to do
     deletions.
 
-15. `edir` shows a message "No files or directories" if there is nothing
+15. `edir` adds `-N/--sort-name, -I/--sort-time, -S/--sort-size` options
+    to sort the paths when listed in your editor. There is also a
+    `-E/--sort-reverse` option to reverse the order.
+
+16. `edir` shows a message "No files or directories" if there is nothing
     to edit, rather than opening an empty file to edit.
 
-16. `edir` filters out any duplicate paths you may inadvertently specify
+17. `edir` filters out any duplicate paths you may inadvertently specify
     on it's command line.
 
-17. `edir` always invokes a consistent duplicate renaming scheme. E.g. if
+18. `edir` always invokes a consistent duplicate renaming scheme. E.g. if
     you rename `b`, `c`, `d` all to the same pre-existing name `a` then
     `edir` will rename `b` to `a~`, `c` to `a~1`, `d` to `a~2`.
     Depending on order of operations, `vidir` is not always consistent
     about this, E.g. sometimes it creates a `a~1` with no `a~` (this may
     be a bug in `vidir` that nobody has ever bothered to
     report/address?).
 
-18. `edir` creates the temporary editing file with a `.sh` suffix so
+19. `edir` creates the temporary editing file with a `.sh` suffix so
     your EDITOR may syntax highlight the entries. Optionally, you can
     change this default suffix.
 
-19. `edir` provides an optional environment value to add custom options
+20. `edir` provides an optional environment value to add custom options
     to the invocation of your editor. See [section
     below](#edir_editor-environment-variable).
 
-20. `edir` provides an optional configuration file to set default `edir`
+21. `edir` provides an optional configuration file to set default `edir`
     command line arguments. See [section
     below](#edir-command-default-arguments).
 
-21. Contrary to what it's name implies, `vidir` actually respects your
+22. Contrary to what it's name implies, `vidir` actually respects your
     `$EDITOR` variable and runs your preferred editor like `edir` does
     but `edir` has been given a generic name to make this more apparent.
 
-22. `edir` is very strict about the format of the lines you edit and
+23. `edir` is very strict about the format of the lines you edit and
     immediately exits with an error message (before changing anything)
     if you format one of the lines incorrectly. All lines in the edited
     list:
 
     1. Must start with a number and that number must be in range.
     2. Must have at least one white space/tab after the number,
     3. Must have a remaining valid path name.
@@ -157,15 +161,15 @@
        same as deleted.
 
     Note the final edited order of lines does not matter, only the first
     number value is used to match the newly edited line to the original
     line so an easy way to swap two file names is just to swap their
     numbers.
 
-23. `edir` always actions files consistently. The sequence of
+24. `edir` always actions files consistently. The sequence of
      operations applied is:
 
     1. Deleted files are removed and all renamed files and directories
        are renamed to temporaries. The temporaries are made on the same
        file-system as the target.
  
     2. Empty deleted directories are removed.
```

### Comparing `edir-2.9/edir.egg-info/PKG-INFO` & `edir-2.9.1/edir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edir
-Version: 2.9
+Version: 2.9.1
 Summary: Utility to rename, remove, and copy files/dirs using your editor
 Home-page: https://github.com/bulletmark/edir
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: vidir
 Platform: UNKNOWN
@@ -125,45 +125,49 @@
 14. `edir` adds a [`-t/--trash` option](#using-trash) to delete to your
     [Trash](https://specifications.freedesktop.org/trash-spec/trashspec-1.0.html).
     This option invokes
     [`trash-put`](https://www.mankier.com/1/trash-put) from the
     [trash-cli](https://github.com/andreafrancia/trash-cli) package to do
     deletions.
 
-15. `edir` shows a message "No files or directories" if there is nothing
+15. `edir` adds `-N/--sort-name, -I/--sort-time, -S/--sort-size` options
+    to sort the paths when listed in your editor. There is also a
+    `-E/--sort-reverse` option to reverse the order.
+
+16. `edir` shows a message "No files or directories" if there is nothing
     to edit, rather than opening an empty file to edit.
 
-16. `edir` filters out any duplicate paths you may inadvertently specify
+17. `edir` filters out any duplicate paths you may inadvertently specify
     on it's command line.
 
-17. `edir` always invokes a consistent duplicate renaming scheme. E.g. if
+18. `edir` always invokes a consistent duplicate renaming scheme. E.g. if
     you rename `b`, `c`, `d` all to the same pre-existing name `a` then
     `edir` will rename `b` to `a~`, `c` to `a~1`, `d` to `a~2`.
     Depending on order of operations, `vidir` is not always consistent
     about this, E.g. sometimes it creates a `a~1` with no `a~` (this may
     be a bug in `vidir` that nobody has ever bothered to
     report/address?).
 
-18. `edir` creates the temporary editing file with a `.sh` suffix so
+19. `edir` creates the temporary editing file with a `.sh` suffix so
     your EDITOR may syntax highlight the entries. Optionally, you can
     change this default suffix.
 
-19. `edir` provides an optional environment value to add custom options
+20. `edir` provides an optional environment value to add custom options
     to the invocation of your editor. See [section
     below](#edir_editor-environment-variable).
 
-20. `edir` provides an optional configuration file to set default `edir`
+21. `edir` provides an optional configuration file to set default `edir`
     command line arguments. See [section
     below](#edir-command-default-arguments).
 
-21. Contrary to what it's name implies, `vidir` actually respects your
+22. Contrary to what it's name implies, `vidir` actually respects your
     `$EDITOR` variable and runs your preferred editor like `edir` does
     but `edir` has been given a generic name to make this more apparent.
 
-22. `edir` is very strict about the format of the lines you edit and
+23. `edir` is very strict about the format of the lines you edit and
     immediately exits with an error message (before changing anything)
     if you format one of the lines incorrectly. All lines in the edited
     list:
 
     1. Must start with a number and that number must be in range.
     2. Must have at least one white space/tab after the number,
     3. Must have a remaining valid path name.
@@ -171,15 +175,15 @@
        same as deleted.
 
     Note the final edited order of lines does not matter, only the first
     number value is used to match the newly edited line to the original
     line so an easy way to swap two file names is just to swap their
     numbers.
 
-23. `edir` always actions files consistently. The sequence of
+24. `edir` always actions files consistently. The sequence of
      operations applied is:
 
     1. Deleted files are removed and all renamed files and directories
        are renamed to temporaries. The temporaries are made on the same
        file-system as the target.
  
     2. Empty deleted directories are removed.
```

### Comparing `edir-2.9/edir.py` & `edir-2.9.1/edir.py`

 * *Files identical despite different names*

### Comparing `edir-2.9/setup.py` & `edir-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 name = 'edir'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='2.9',
+    version='2.9.1',
     description='Utility to rename, remove, and copy files/dirs using '
     'your editor',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/bulletmark/{}'.format(name),
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
```

