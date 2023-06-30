# Comparing `tmp/pynaroma-0.4.0.tar.gz` & `tmp/pynaroma-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynaroma-0.4.0.tar", last modified: Mon Jul  4 17:37:18 2022, max compression
+gzip compressed data, was "pynaroma-0.4.1.tar", last modified: Fri Jun 30 13:10:33 2023, max compression
```

## Comparing `pynaroma-0.4.0.tar` & `pynaroma-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 shred     (1000) shred     (1000)        0 2022-07-04 17:37:18.277304 pynaroma-0.4.0/
--rw-rw-r--   0 shred     (1000) shred     (1000)    35147 2021-07-15 12:08:07.000000 pynaroma-0.4.0/LICENSE.txt
--rw-rw-r--   0 shred     (1000) shred     (1000)     8379 2022-07-04 17:37:18.277304 pynaroma-0.4.0/PKG-INFO
--rw-rw-r--   0 shred     (1000) shred     (1000)     7281 2022-07-04 06:41:34.000000 pynaroma-0.4.0/README.md
-drwxrwxr-x   0 shred     (1000) shred     (1000)        0 2022-07-04 17:37:18.276304 pynaroma-0.4.0/pynaroma/
--rw-rw-r--   0 shred     (1000) shred     (1000)       18 2021-07-28 20:49:28.000000 pynaroma-0.4.0/pynaroma/__init__.py
--rwxrwxr-x   0 shred     (1000) shred     (1000)     7899 2022-07-04 06:26:31.000000 pynaroma-0.4.0/pynaroma/bin2rom.py
--rw-r--r--   0 shred     (1000) shred     (1000)     3020 2022-06-26 08:57:21.000000 pynaroma-0.4.0/pynaroma/bin2split.py
--rwxrwxr-x   0 shred     (1000) shred     (1000)     5872 2022-07-04 06:28:34.000000 pynaroma-0.4.0/pynaroma/rom2bin.py
-drwxrwxr-x   0 shred     (1000) shred     (1000)        0 2022-07-04 17:37:18.277304 pynaroma-0.4.0/pynaroma.egg-info/
--rw-rw-r--   0 shred     (1000) shred     (1000)     8379 2022-07-04 17:37:18.000000 pynaroma-0.4.0/pynaroma.egg-info/PKG-INFO
--rw-rw-r--   0 shred     (1000) shred     (1000)      276 2022-07-04 17:37:18.000000 pynaroma-0.4.0/pynaroma.egg-info/SOURCES.txt
--rw-rw-r--   0 shred     (1000) shred     (1000)        1 2022-07-04 17:37:18.000000 pynaroma-0.4.0/pynaroma.egg-info/dependency_links.txt
--rw-rw-r--   0 shred     (1000) shred     (1000)      119 2022-07-04 17:37:18.000000 pynaroma-0.4.0/pynaroma.egg-info/entry_points.txt
--rw-rw-r--   0 shred     (1000) shred     (1000)        9 2022-07-04 17:37:18.000000 pynaroma-0.4.0/pynaroma.egg-info/top_level.txt
--rw-rw-r--   0 shred     (1000) shred     (1000)       38 2022-07-04 17:37:18.277304 pynaroma-0.4.0/setup.cfg
--rw-rw-r--   0 shred     (1000) shred     (1000)     2293 2022-07-04 06:41:46.000000 pynaroma-0.4.0/setup.py
+drwxr-xr-x   0 shred     (1000) shred     (1000)        0 2023-06-30 13:10:33.292092 pynaroma-0.4.1/
+-rw-rw-r--   0 shred     (1000) shred     (1000)    35147 2021-07-15 12:08:07.000000 pynaroma-0.4.1/LICENSE.txt
+-rw-r--r--   0 shred     (1000) shred     (1000)     8354 2023-06-30 13:10:33.292092 pynaroma-0.4.1/PKG-INFO
+-rw-rw-r--   0 shred     (1000) shred     (1000)     7276 2023-06-30 13:06:41.000000 pynaroma-0.4.1/README.md
+drwxr-xr-x   0 shred     (1000) shred     (1000)        0 2023-06-30 13:10:33.291092 pynaroma-0.4.1/pynaroma/
+-rw-rw-r--   0 shred     (1000) shred     (1000)       18 2021-07-28 20:49:28.000000 pynaroma-0.4.1/pynaroma/__init__.py
+-rwxrwxr-x   0 shred     (1000) shred     (1000)     7899 2022-07-04 06:26:31.000000 pynaroma-0.4.1/pynaroma/bin2rom.py
+-rw-r--r--   0 shred     (1000) shred     (1000)     3020 2022-06-26 08:57:21.000000 pynaroma-0.4.1/pynaroma/bin2split.py
+-rwxrwxr-x   0 shred     (1000) shred     (1000)     5872 2022-07-04 06:28:34.000000 pynaroma-0.4.1/pynaroma/rom2bin.py
+drwxr-xr-x   0 shred     (1000) shred     (1000)        0 2023-06-30 13:10:33.292092 pynaroma-0.4.1/pynaroma.egg-info/
+-rw-rw-r--   0 shred     (1000) shred     (1000)     8354 2023-06-30 13:10:33.000000 pynaroma-0.4.1/pynaroma.egg-info/PKG-INFO
+-rw-rw-r--   0 shred     (1000) shred     (1000)      276 2023-06-30 13:10:33.000000 pynaroma-0.4.1/pynaroma.egg-info/SOURCES.txt
+-rw-rw-r--   0 shred     (1000) shred     (1000)        1 2023-06-30 13:10:33.000000 pynaroma-0.4.1/pynaroma.egg-info/dependency_links.txt
+-rw-rw-r--   0 shred     (1000) shred     (1000)      118 2023-06-30 13:10:33.000000 pynaroma-0.4.1/pynaroma.egg-info/entry_points.txt
+-rw-rw-r--   0 shred     (1000) shred     (1000)        9 2023-06-30 13:10:33.000000 pynaroma-0.4.1/pynaroma.egg-info/top_level.txt
+-rw-r--r--   0 shred     (1000) shred     (1000)       38 2023-06-30 13:10:33.292092 pynaroma-0.4.1/setup.cfg
+-rw-rw-r--   0 shred     (1000) shred     (1000)     2316 2023-06-30 13:09:41.000000 pynaroma-0.4.1/setup.py
```

### Comparing `pynaroma-0.4.0/LICENSE.txt` & `pynaroma-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynaroma-0.4.0/PKG-INFO` & `pynaroma-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pynaroma
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for converting Amiga ROM images
 Home-page: https://github.com/shred/pynaroma
 Author: Richard Körber
 Author-email: dev@shredzone.de
 License: GPLv3+
 Project-URL: Source, https://github.com/shred/pynaroma
 Project-URL: Tracker, https://github.com/shred/pynaroma/issues
 Keywords: Amiga ROM
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -161,15 +160,15 @@
 
 ## 8-bit Mode
 
 Usually 16-bit ROMs are used in Amiga hardware. Some extensions (like Action Replay) use two 8-bit ROMs though. One ROM is for the lower, and the other one for the upper part of the 16-bit data bus. Also the Atari ST line uses 8-bit ROMs.
 
 With the `--8bit` option, _pynaroma_ converts a ROM dump into two ROM images for 8-bit EPROMs, and vice versa. When the 8-bit mode is enabled, the upper part of the word (bit 8-15) is in the `--low` file, while the lower part of the word (bit 0-7) is in the `--high` file. This is because _pynaroma_ works in big-endian mode by default.
 
-The `--8bit` mode requires the `--low` and `--high` options to be set. This is not a limitation, because an 8-bit ROM dump and an 8-bit ROM image is essentially the same file. 😉
+The `--8bit` mode requires the `--low` and `--high` options to be set. This is not a limitation, because an 8-bit ROM dump and an 8-bit ROM image is essentially the same file.
 
 ## Endianness
 
 _pynaroma_ was made for Amiga and Atari enthusiasts. Since these machines base on the Motorola 68000 architecture, the default mode is big-endian, and byte swapping takes place when reading or writing ROM images (see [Endianness](https://en.wikipedia.org/wiki/Endianness)).
 
 If your target system has a little-endian architecture, you can set the `--little` option at `rom2bin` and `bin2rom`. If this option is set, no byte swapping is done.
 
@@ -179,9 +178,7 @@
 
 * Fork the [Source code at GitHub](https://github.com/shred/pynaroma). Feel free to send pull requests.
 * Found a bug? [File a bug report!](https://github.com/shred/pynaroma/issues)
 
 ## License
 
 _pynaroma_ is open source software. The source code is distributed under the terms of [GNU General Public License (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html#content).
-
-
```

### Comparing `pynaroma-0.4.0/README.md` & `pynaroma-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 ## 8-bit Mode
 
 Usually 16-bit ROMs are used in Amiga hardware. Some extensions (like Action Replay) use two 8-bit ROMs though. One ROM is for the lower, and the other one for the upper part of the 16-bit data bus. Also the Atari ST line uses 8-bit ROMs.
 
 With the `--8bit` option, _pynaroma_ converts a ROM dump into two ROM images for 8-bit EPROMs, and vice versa. When the 8-bit mode is enabled, the upper part of the word (bit 8-15) is in the `--low` file, while the lower part of the word (bit 0-7) is in the `--high` file. This is because _pynaroma_ works in big-endian mode by default.
 
-The `--8bit` mode requires the `--low` and `--high` options to be set. This is not a limitation, because an 8-bit ROM dump and an 8-bit ROM image is essentially the same file. 😉
+The `--8bit` mode requires the `--low` and `--high` options to be set. This is not a limitation, because an 8-bit ROM dump and an 8-bit ROM image is essentially the same file.
 
 ## Endianness
 
 _pynaroma_ was made for Amiga and Atari enthusiasts. Since these machines base on the Motorola 68000 architecture, the default mode is big-endian, and byte swapping takes place when reading or writing ROM images (see [Endianness](https://en.wikipedia.org/wiki/Endianness)).
 
 If your target system has a little-endian architecture, you can set the `--little` option at `rom2bin` and `bin2rom`. If this option is set, no byte swapping is done.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pynaroma-0.4.0/pynaroma/bin2rom.py` & `pynaroma-0.4.1/pynaroma/bin2rom.py`

 * *Files identical despite different names*

### Comparing `pynaroma-0.4.0/pynaroma/bin2split.py` & `pynaroma-0.4.1/pynaroma/bin2split.py`

 * *Files identical despite different names*

### Comparing `pynaroma-0.4.0/pynaroma/rom2bin.py` & `pynaroma-0.4.1/pynaroma/rom2bin.py`

 * *Files identical despite different names*

### Comparing `pynaroma-0.4.0/pynaroma.egg-info/PKG-INFO` & `pynaroma-0.4.1/pynaroma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pynaroma
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for converting Amiga ROM images
 Home-page: https://github.com/shred/pynaroma
 Author: Richard Körber
 Author-email: dev@shredzone.de
 License: GPLv3+
 Project-URL: Source, https://github.com/shred/pynaroma
 Project-URL: Tracker, https://github.com/shred/pynaroma/issues
 Keywords: Amiga ROM
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -161,15 +160,15 @@
 
 ## 8-bit Mode
 
 Usually 16-bit ROMs are used in Amiga hardware. Some extensions (like Action Replay) use two 8-bit ROMs though. One ROM is for the lower, and the other one for the upper part of the 16-bit data bus. Also the Atari ST line uses 8-bit ROMs.
 
 With the `--8bit` option, _pynaroma_ converts a ROM dump into two ROM images for 8-bit EPROMs, and vice versa. When the 8-bit mode is enabled, the upper part of the word (bit 8-15) is in the `--low` file, while the lower part of the word (bit 0-7) is in the `--high` file. This is because _pynaroma_ works in big-endian mode by default.
 
-The `--8bit` mode requires the `--low` and `--high` options to be set. This is not a limitation, because an 8-bit ROM dump and an 8-bit ROM image is essentially the same file. 😉
+The `--8bit` mode requires the `--low` and `--high` options to be set. This is not a limitation, because an 8-bit ROM dump and an 8-bit ROM image is essentially the same file.
 
 ## Endianness
 
 _pynaroma_ was made for Amiga and Atari enthusiasts. Since these machines base on the Motorola 68000 architecture, the default mode is big-endian, and byte swapping takes place when reading or writing ROM images (see [Endianness](https://en.wikipedia.org/wiki/Endianness)).
 
 If your target system has a little-endian architecture, you can set the `--little` option at `rom2bin` and `bin2rom`. If this option is set, no byte swapping is done.
 
@@ -179,9 +178,7 @@
 
 * Fork the [Source code at GitHub](https://github.com/shred/pynaroma). Feel free to send pull requests.
 * Found a bug? [File a bug report!](https://github.com/shred/pynaroma/issues)
 
 ## License
 
 _pynaroma_ is open source software. The source code is distributed under the terms of [GNU General Public License (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html#content).
-
-
```

### Comparing `pynaroma-0.4.0/setup.py` & `pynaroma-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 from setuptools import setup
 
 def readme():
-    with open('README.md') as f:
+    with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 setup(
     name='pynaroma',
-    version='0.4.0',
+    version='0.4.1',
     description='Tools for converting Amiga ROM images',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/shred/pynaroma',
     keywords='Amiga ROM',
     license='GPLv3+',
```

