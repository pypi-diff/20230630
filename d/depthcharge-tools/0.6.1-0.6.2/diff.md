# Comparing `tmp/depthcharge-tools-0.6.1.tar.gz` & `tmp/depthcharge-tools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge-tools-0.6.1.tar", last modified: Thu Nov 24 21:36:52 2022, max compression
+gzip compressed data, was "depthcharge-tools-0.6.2.tar", last modified: Fri Jun 30 15:24:40 2023, max compression
```

## Comparing `depthcharge-tools-0.6.1.tar` & `depthcharge-tools-0.6.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.309654 depthcharge-tools-0.6.1/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    18092 2020-01-10 17:02:53.000000 depthcharge-tools-0.6.1/LICENSE
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      109 2021-04-28 11:45:38.000000 depthcharge-tools-0.6.1/MANIFEST.in
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8994 2022-11-24 21:36:52.309654 depthcharge-tools-0.6.1/PKG-INFO
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8282 2022-10-19 11:33:45.000000 depthcharge-tools-0.6.1/README.rst
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.293652 depthcharge-tools-0.6.1/completions/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     7943 2022-10-19 11:33:45.000000 depthcharge-tools-0.6.1/completions/_depthchargectl.bash
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     6301 2022-10-19 11:33:45.000000 depthcharge-tools-0.6.1/completions/_depthchargectl.zsh
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2418 2022-10-19 11:33:45.000000 depthcharge-tools-0.6.1/completions/_mkdepthcharge.bash
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2438 2022-10-19 11:33:45.000000 depthcharge-tools-0.6.1/completions/_mkdepthcharge.zsh
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.297652 depthcharge-tools-0.6.1/depthcharge_tools/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1597 2022-11-04 18:06:11.000000 depthcharge-tools-0.6.1/depthcharge_tools/__init__.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    67991 2022-11-22 17:51:59.000000 depthcharge-tools-0.6.1/depthcharge_tools/boards.ini
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      379 2022-11-08 08:39:59.000000 depthcharge-tools-0.6.1/depthcharge_tools/config.ini
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.305653 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    24019 2022-10-16 13:13:02.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/__init__.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      139 2021-04-28 11:45:38.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/__main__.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     7542 2022-11-24 10:37:39.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_bless.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    17910 2022-11-22 17:51:59.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_build.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     5984 2022-09-30 19:33:34.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_check.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2227 2022-09-30 19:33:34.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_config.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     7798 2022-09-30 19:33:34.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_list.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8030 2022-11-22 17:51:59.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_remove.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     7980 2022-10-01 18:14:20.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_target.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     9730 2022-11-04 17:56:37.000000 depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_write.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    33180 2022-10-18 22:41:43.000000 depthcharge-tools-0.6.1/depthcharge_tools/mkdepthcharge.py
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.305653 depthcharge-tools-0.6.1/depthcharge_tools/utils/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)        0 2021-04-27 18:18:49.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/__init__.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    32503 2022-10-13 12:56:18.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/argparse.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     6050 2022-09-07 13:59:17.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/collections.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    18602 2022-09-30 19:33:34.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/os.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1211 2022-10-19 11:33:45.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/pathlib.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    13524 2022-11-22 17:51:59.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/platform.py
--rwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)     1904 2022-09-26 10:51:23.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/string.py
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    13145 2022-10-16 13:13:02.000000 depthcharge-tools-0.6.1/depthcharge_tools/utils/subprocess.py
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.301653 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8994 2022-11-24 21:36:51.000000 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/PKG-INFO
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1397 2022-11-24 21:36:51.000000 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/SOURCES.txt
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)        1 2022-11-24 21:36:51.000000 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/dependency_links.txt
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      155 2022-11-24 21:36:51.000000 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/entry_points.txt
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)       11 2022-11-24 21:36:51.000000 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/requires.txt
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)       18 2022-11-24 21:36:51.000000 depthcharge-tools-0.6.1/depthcharge_tools.egg-info/top_level.txt
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    17312 2022-11-24 15:45:28.000000 depthcharge-tools-0.6.1/depthchargectl.rst
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.305653 depthcharge-tools-0.6.1/init.d/
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      673 2021-04-26 12:45:01.000000 depthcharge-tools-0.6.1/init.d/depthchargectl-bless
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    10048 2022-11-24 15:45:43.000000 depthcharge-tools-0.6.1/mkdepthcharge.rst
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)       38 2022-11-24 21:36:52.309654 depthcharge-tools-0.6.1/setup.cfg
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1348 2022-11-24 15:47:32.000000 depthcharge-tools-0.6.1/setup.py
-drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2022-11-24 21:36:52.309654 depthcharge-tools-0.6.1/systemd/
--rwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)     8255 2022-11-22 20:24:08.000000 depthcharge-tools-0.6.1/systemd/90-depthcharge-tools.install
--rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      842 2021-04-26 12:33:23.000000 depthcharge-tools-0.6.1/systemd/depthchargectl-bless.service
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     3706 2023-06-30 04:29:26.000000 depthcharge-tools-0.6.2/COPYRIGHT
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    18092 2023-06-26 15:55:34.000000 depthcharge-tools-0.6.2/LICENSE
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      340 2023-06-30 03:57:19.000000 depthcharge-tools-0.6.2/MANIFEST.in
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    10391 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/PKG-INFO
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     9655 2023-06-30 09:19:43.000000 depthcharge-tools-0.6.2/README.rst
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/completions/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8550 2023-06-30 09:47:04.000000 depthcharge-tools-0.6.2/completions/_depthchargectl.bash
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     6996 2023-06-30 09:38:20.000000 depthcharge-tools-0.6.2/completions/_depthchargectl.zsh
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2694 2023-06-30 09:31:28.000000 depthcharge-tools-0.6.2/completions/_mkdepthcharge.bash
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2836 2023-06-30 09:31:04.000000 depthcharge-tools-0.6.2/completions/_mkdepthcharge.zsh
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/depthcharge_tools/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1810 2023-06-30 07:52:01.000000 depthcharge-tools-0.6.2/depthcharge_tools/__init__.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    75117 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/boards.ini
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      628 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/config.ini
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    27038 2023-06-30 13:14:00.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/__init__.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      358 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/__main__.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     7775 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_bless.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    19824 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_build.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     6582 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_check.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2461 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_config.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8205 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_list.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8534 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_remove.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     8322 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_target.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    10303 2023-06-30 07:51:22.000000 depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_write.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    38583 2023-06-30 09:19:43.000000 depthcharge-tools-0.6.2/depthcharge_tools/mkdepthcharge.py
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/depthcharge_tools/utils/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-26 16:07:33.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/__init__.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    33256 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/argparse.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     6273 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/collections.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    18812 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/os.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1430 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/pathlib.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    14811 2023-06-30 07:51:47.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/platform.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     2117 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/string.py
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    14180 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/depthcharge_tools/utils/subprocess.py
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    10391 2023-06-30 15:24:40.000000 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/PKG-INFO
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1407 2023-06-30 15:24:40.000000 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)        1 2023-06-30 15:24:40.000000 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      155 2023-06-30 15:24:40.000000 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/entry_points.txt
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)       11 2023-06-30 15:24:40.000000 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/requires.txt
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)       18 2023-06-30 15:24:40.000000 depthcharge-tools-0.6.2/depthcharge_tools.egg-info/top_level.txt
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    19455 2023-06-30 09:22:06.000000 depthcharge-tools-0.6.2/depthchargectl.rst
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/init.d/
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)      912 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/init.d/depthchargectl-bless
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)    13469 2023-06-30 09:20:47.000000 depthcharge-tools-0.6.2/mkdepthcharge.rst
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)       38 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/setup.cfg
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1622 2023-06-30 15:16:51.000000 depthcharge-tools-0.6.2/setup.py
+drwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)        0 2023-06-30 15:24:40.638498 depthcharge-tools-0.6.2/systemd/
+-rwxr-xr-x   0 alpernebbi  (1000) alpernebbi  (1000)     8428 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/systemd/90-depthcharge-tools.install
+-rw-r--r--   0 alpernebbi  (1000) alpernebbi  (1000)     1029 2023-06-30 03:24:50.000000 depthcharge-tools-0.6.2/systemd/depthchargectl-bless.service
```

### Comparing `depthcharge-tools-0.6.1/LICENSE` & `depthcharge-tools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge-tools-0.6.1/PKG-INFO` & `depthcharge-tools-0.6.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-Metadata-Version: 2.1
-Name: depthcharge-tools
-Version: 0.6.1
-Summary: Tools to manage the Chrome OS bootloader
-Home-page: https://github.com/alpernebbi/depthcharge-tools
-Author: Alper Nebi Yasak
-Author-email: alpernebiyasak@gmail.com
-License: GPL2+
-Keywords: ChromeOS ChromiumOS depthcharge vboot vbutil_kernel
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Boot
-Description-Content-Type: text/x-rst
-License-File: LICENSE
+.. SPDX-License-Identifier: GPL-2.0-or-later
+
+.. depthcharge-tools README file
+.. Copyright (C) 2019-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+.. See COPYRIGHT and LICENSE files for full copyright information.
 
 =================
 Depthcharge-Tools
 =================
 This project is a collection of tools that ease and automate interacting
 with depthcharge_, the Chrome OS bootloader.
 
@@ -30,28 +17,28 @@
 `the format depthcharge expects`_. These tools are about the latter.
 
 Right now these are developed on and tested with only a few boards,
 but everything will attempt to work on other boards based on my best
 guesses.
 
 .. _depthcharge: https://chromium.googlesource.com/chromiumos/platform/depthcharge
-.. _the format depthcharge expects: https://www.chromium.org/chromium-os/chromiumos-design-docs/disk-format#TOC-Google-Chrome-OS-devices
+.. _the format depthcharge expects: https://chromium.googlesource.com/chromiumos/docs/+/HEAD/disk_format.md#Google-ChromeOS-devices
 .. _Debian: https://www.debian.org/
 
 
 mkdepthcharge
 =============
 The mkdepthcharge_ tool is intended to wrap mkimage_ and vbutil_kernel_
 to provide reasonable defaults to them, hide their idiosyncrasies and
 automate creating a depthcharge-bootable partition image appropriate for
 the running architecture. An example invocation on a Samsung Chromebook
 Plus (v1, arm64) could be::
 
     $ mkdepthcharge -o depthcharge.img --compress lzma \
-        --cmdline "console=tty1 root=/dev/mmcblk0p2 rootwait" \
+        --cmdline "console=tty1 root=/dev/mmcblk0p2 rootwait" -- \
         /boot/vmlinuz.gz /boot/initrd.img rk3399-gru-kevin.dtb
 
 Here, mkdepthcharge would automatically extract and recompress the
 kernel, create a FIT image, put command line parameters into a file,
 create an empty bootloader, and provide defaults for vboot keys and
 other arguments while building the partition image.
 
@@ -100,24 +87,46 @@
 the ``mkdepthcharge.rst`` and ``depthchargectl.rst`` files to manual
 pages. However, this is not automated here and has to be done manually.
 
 This project (or at least ``depthchargectl``) is meant to be integrated
 into your operating system by its maintainers, and the best way to
 install it is through your OS' package manager whenever possible.
 
+
 Debian
 ------
-An unofficial Debian package is available in the releases_ page, with
-it's packaging source tracked in salsa_. After downloading, you can
-install with::
+An official `depthcharge-tools Debian package`_ is available upstream,
+since Debian 12 (bookworm). You can install it like any other package::
+
+    $ sudo apt install depthcharge-tools
+
+It includes the necessary system hooks and services to make and keep
+your Chromebook bootable, enabled by default. These however do not
+trigger on the depthcharge-tools installation, but on kernel and
+initramfs changes. To trigger these hooks manually, run::
+
+    $ sudo update-initramfs -u
+
+.. _depthcharge-tools Debian package: https://packages.debian.org/sid/depthcharge-tools
+
 
-    $ sudo apt install ./depthcharge-tools_*.deb
+Alpine Linux
+------------
+Thanks to the efforts in supporting `postmarketOS on ChromeOS Devices`_,
+there is an official `depthcharge-tools package for Alpine Linux`_. You
+should be able to install it as::
+
+    $ sudo apk add depthcharge-tools
+
+However, this doesn't include any system hooks or services to keep your
+Chromebook bootable.
+
+.. _postmarketOS on ChromeOS Devices: https://wiki.postmarketos.org/wiki/Chrome_OS_devices
+.. _depthcharge-tools package for Alpine Linux: https://pkgs.alpinelinux.org/package/edge/testing/x86/depthcharge-tools
 
-.. _releases: https://github.com/alpernebbi/depthcharge-tools/releases
-.. _salsa: https://salsa.debian.org/alpernebbi/depthcharge-tools
 
 Pip
 ---
 Python binary wheels are uploaded to PyPI_, and it should be possible to
 install the python package using `pip`. However, this does not install
 the manual pages, bash/zsh completions, systemd/init.d service files,
 and OS-specific kernel/initramfs hooks.
@@ -155,14 +164,15 @@
     vboot-public-key: The public key for (.vbpubk) verifying images
 
     [depthchargectl]
     board: Codename of a board to build and check images for
     ignore-initramfs: Do not include an initramfs in the image
     images-dir: Directory to store built images
     kernel-cmdline: Kernel commandline parameters to use
+    zimage-initramfs-hack = How to support initramfs on x86 boards
 
 For longer explanations check the manual pages of each command for
 options named the same as these.
 
 .. |CONFIG_FILE| replace:: ``/etc/depthcharge-tools/config``
 .. |CONFIGD_DIR| replace:: ``/etc/depthcharge-tools/config.d``
 .. _config.ini: https://github.com/alpernebbi/depthcharge-tools/blob/master/depthcharge_tools/config.ini
@@ -192,29 +202,38 @@
 
     $ depthchargectl list /dev/mmcblk0
     S  P  T  PATH
     1  2  0  /dev/mmcblk0p2
     1  1  0  /dev/mmcblk0p4
     0  0  15 /dev/mmcblk0p6
 
+Or you can add a similar invocation to the /usr/local/bin files, so that
+it's available to both normal users and root::
 
-Contributing
-============
-I only own two chromebooks, so I need your help to make it work with all
-others. Pull requests, bug reports, or even pointers in the right
-direction for existing issues are all welcome.
+    $ sudo tee /usr/local/bin/depthchargectl <<EOF
+    #!/bin/sh
+    export PYTHONDONTWRITEBYTECODE=1
+    export PYTHONPATH=/path/to/depthcharge-tools
+    exec python3 -m depthcharge_tools.depthchargectl "\$@"
+    EOF
+
+    $ sudo chmod +x /usr/local/bin/depthchargectl
 
 
 License
 =======
+Copyright (C) 2019-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+
 This program is free software; you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation; either version 2 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <https://www.gnu.org/licenses/>
+
+See COPYRIGHT and LICENSE files for full copyright information.
```

### Comparing `depthcharge-tools-0.6.1/README.rst` & `depthcharge-tools-0.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: depthcharge-tools
+Version: 0.6.2
+Summary: Tools to manage the Chrome OS bootloader
+Home-page: https://github.com/alpernebbi/depthcharge-tools
+Author: Alper Nebi Yasak
+Author-email: alpernebiyasak@gmail.com
+License: GPL2+
+Keywords: ChromeOS ChromiumOS depthcharge vboot vbutil_kernel
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Boot
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: COPYRIGHT
+
+.. SPDX-License-Identifier: GPL-2.0-or-later
+
+.. depthcharge-tools README file
+.. Copyright (C) 2019-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+.. See COPYRIGHT and LICENSE files for full copyright information.
+
 =================
 Depthcharge-Tools
 =================
 This project is a collection of tools that ease and automate interacting
 with depthcharge_, the Chrome OS bootloader.
 
 Depthcharge is built into the firmware of Chrome OS boards, uses a
@@ -11,28 +37,28 @@
 `the format depthcharge expects`_. These tools are about the latter.
 
 Right now these are developed on and tested with only a few boards,
 but everything will attempt to work on other boards based on my best
 guesses.
 
 .. _depthcharge: https://chromium.googlesource.com/chromiumos/platform/depthcharge
-.. _the format depthcharge expects: https://www.chromium.org/chromium-os/chromiumos-design-docs/disk-format#TOC-Google-Chrome-OS-devices
+.. _the format depthcharge expects: https://chromium.googlesource.com/chromiumos/docs/+/HEAD/disk_format.md#Google-ChromeOS-devices
 .. _Debian: https://www.debian.org/
 
 
 mkdepthcharge
 =============
 The mkdepthcharge_ tool is intended to wrap mkimage_ and vbutil_kernel_
 to provide reasonable defaults to them, hide their idiosyncrasies and
 automate creating a depthcharge-bootable partition image appropriate for
 the running architecture. An example invocation on a Samsung Chromebook
 Plus (v1, arm64) could be::
 
     $ mkdepthcharge -o depthcharge.img --compress lzma \
-        --cmdline "console=tty1 root=/dev/mmcblk0p2 rootwait" \
+        --cmdline "console=tty1 root=/dev/mmcblk0p2 rootwait" -- \
         /boot/vmlinuz.gz /boot/initrd.img rk3399-gru-kevin.dtb
 
 Here, mkdepthcharge would automatically extract and recompress the
 kernel, create a FIT image, put command line parameters into a file,
 create an empty bootloader, and provide defaults for vboot keys and
 other arguments while building the partition image.
 
@@ -81,24 +107,46 @@
 the ``mkdepthcharge.rst`` and ``depthchargectl.rst`` files to manual
 pages. However, this is not automated here and has to be done manually.
 
 This project (or at least ``depthchargectl``) is meant to be integrated
 into your operating system by its maintainers, and the best way to
 install it is through your OS' package manager whenever possible.
 
+
 Debian
 ------
-An unofficial Debian package is available in the releases_ page, with
-it's packaging source tracked in salsa_. After downloading, you can
-install with::
+An official `depthcharge-tools Debian package`_ is available upstream,
+since Debian 12 (bookworm). You can install it like any other package::
+
+    $ sudo apt install depthcharge-tools
+
+It includes the necessary system hooks and services to make and keep
+your Chromebook bootable, enabled by default. These however do not
+trigger on the depthcharge-tools installation, but on kernel and
+initramfs changes. To trigger these hooks manually, run::
+
+    $ sudo update-initramfs -u
+
+.. _depthcharge-tools Debian package: https://packages.debian.org/sid/depthcharge-tools
+
 
-    $ sudo apt install ./depthcharge-tools_*.deb
+Alpine Linux
+------------
+Thanks to the efforts in supporting `postmarketOS on ChromeOS Devices`_,
+there is an official `depthcharge-tools package for Alpine Linux`_. You
+should be able to install it as::
+
+    $ sudo apk add depthcharge-tools
+
+However, this doesn't include any system hooks or services to keep your
+Chromebook bootable.
+
+.. _postmarketOS on ChromeOS Devices: https://wiki.postmarketos.org/wiki/Chrome_OS_devices
+.. _depthcharge-tools package for Alpine Linux: https://pkgs.alpinelinux.org/package/edge/testing/x86/depthcharge-tools
 
-.. _releases: https://github.com/alpernebbi/depthcharge-tools/releases
-.. _salsa: https://salsa.debian.org/alpernebbi/depthcharge-tools
 
 Pip
 ---
 Python binary wheels are uploaded to PyPI_, and it should be possible to
 install the python package using `pip`. However, this does not install
 the manual pages, bash/zsh completions, systemd/init.d service files,
 and OS-specific kernel/initramfs hooks.
@@ -136,14 +184,15 @@
     vboot-public-key: The public key for (.vbpubk) verifying images
 
     [depthchargectl]
     board: Codename of a board to build and check images for
     ignore-initramfs: Do not include an initramfs in the image
     images-dir: Directory to store built images
     kernel-cmdline: Kernel commandline parameters to use
+    zimage-initramfs-hack = How to support initramfs on x86 boards
 
 For longer explanations check the manual pages of each command for
 options named the same as these.
 
 .. |CONFIG_FILE| replace:: ``/etc/depthcharge-tools/config``
 .. |CONFIGD_DIR| replace:: ``/etc/depthcharge-tools/config.d``
 .. _config.ini: https://github.com/alpernebbi/depthcharge-tools/blob/master/depthcharge_tools/config.ini
@@ -173,29 +222,38 @@
 
     $ depthchargectl list /dev/mmcblk0
     S  P  T  PATH
     1  2  0  /dev/mmcblk0p2
     1  1  0  /dev/mmcblk0p4
     0  0  15 /dev/mmcblk0p6
 
+Or you can add a similar invocation to the /usr/local/bin files, so that
+it's available to both normal users and root::
 
-Contributing
-============
-I only own two chromebooks, so I need your help to make it work with all
-others. Pull requests, bug reports, or even pointers in the right
-direction for existing issues are all welcome.
+    $ sudo tee /usr/local/bin/depthchargectl <<EOF
+    #!/bin/sh
+    export PYTHONDONTWRITEBYTECODE=1
+    export PYTHONPATH=/path/to/depthcharge-tools
+    exec python3 -m depthcharge_tools.depthchargectl "\$@"
+    EOF
+
+    $ sudo chmod +x /usr/local/bin/depthchargectl
 
 
 License
 =======
+Copyright (C) 2019-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+
 This program is free software; you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation; either version 2 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <https://www.gnu.org/licenses/>
+
+See COPYRIGHT and LICENSE files for full copyright information.
```

### Comparing `depthcharge-tools-0.6.1/completions/_depthchargectl.bash` & `depthcharge-tools-0.6.2/completions/_depthchargectl.bash`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# vim: filetype=sh
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl bash completions
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 _depthchargectl__file() {
     COMPREPLY+=($(compgen -f -- "$cur"))
     compopt -o filenames
     if [ "${#COMPREPLY[@]}" -eq 1 ]; then
         if [ -d "${COMPREPLY[0]}" ]; then
             compopt -o nospace
@@ -24,14 +28,19 @@
 } 2>/dev/null
 
 _depthchargectl__root() {
     local root="$(findmnt --fstab -n -o SOURCE "/")"
     COMPREPLY+=($(compgen -W "$root" -- "$cur"))
 } 2>/dev/null
 
+_depthchargectl__boot() {
+    local boot="$(findmnt --fstab -n -o SOURCE "/boot")"
+    COMPREPLY+=($(compgen -W "$boot" -- "$cur"))
+} 2>/dev/null
+
 _depthchargectl__cmdline() {
     local cmdline="$(cat /proc/cmdline | sed -e 's/\(cros_secure\|kern_guid\)[^ ]* //g')"
     COMPREPLY+=($(compgen -W "$cmdline" -- "$cur"))
 } 2>/dev/null
 
 _depthchargectl__kernel() {
     if command -v _kernel_versions >/dev/null 2>/dev/null; then
@@ -63,23 +72,26 @@
         --vboot-keyblock --vboot-public-key --vboot-private-key
         --kernel-cmdline --ignore-initramfs
     )
     local cmds=(bless build config check list remove target write)
 
     case "$prev" in
         --root) _depthchargectl__root; _depthchargectl__disk; return ;;
+        --root-mountpoint) _depthchargectl__file; return ;;
+        --boot-mountpoint) _depthchargectl__file; return ;;
         --tmpdir) _depthchargectl__file; return ;;
         --config) _depthchargectl__file; return ;;
         --board) _depthchargectl__boards; return ;;
         --images-dir) _depthchargectl__file; return ;;
         --vboot-keyblock) _depthchargectl__file; return ;;
         --vboot-public-key) _depthchargectl__file; return ;;
         --vboot-private-key) _depthchargectl__file; return ;;
         --kernel-cmdline) _depthchargectl__cmdline; return ;;
         --ignore-initramfs) : ;;
+        --zimage-initramfs-hack) COMPREPLY+=($(compgen -W "set-init-size pad-vmlinuz none" -- "$cur")) ;;
         --) ;;
         *) ;;
     esac
 
     local cmd
     for cmd in "${COMP_WORDS[@]}"; do
         case "$cmd" in
@@ -223,7 +235,9 @@
             COMPREPLY+=($(compgen -W "${global_opts[*]}" -- "$cur"))
             COMPREPLY+=($(compgen -W "${config_opts[*]}" -- "$cur"))
             ;;
     esac
 }
 
 complete -F _depthchargectl depthchargectl
+
+# vim: filetype=sh
```

### Comparing `depthcharge-tools-0.6.1/completions/_depthchargectl.zsh` & `depthcharge-tools-0.6.2/completions/_depthchargectl.zsh`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 #compdef depthchargectl
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl zsh completions
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 function _depthchargectl {
     _arguments -C \
         {-h,--help}'[Show a help message.]' \
         {-v,--verbose}'[Print more detailed output.]' \
         {-V,--version}'[Print program version.]' \
         --tmpdir'[Directory to keep temporary files.]:temp dir:_directories' \
         --root'[Root device or mountpoint of the system to work on]:root device:{_depthchargectl__root; _depthchargectl__disk}' \
+        --root-mountpoint'[Root mountpoint of the system to work on]:root mountpoint:_directories' \
+        --boot-mountpoint'[Boot mountpoint of the system to work on]:boot mountpoint:_directories' \
         --config'[Additional configuration file to read]:config file:_files' \
         --board'[Assume running on the specified board]:board codenames:{_depthchargectl__board;}' \
         --images-dir'[Directory to store built images]:images dir:_directories' \
         --vboot-keyblock'[Keyblock file to include in images]:keyblock file:_files' \
         --vboot-public-key'[Public key file to verify images]:vbpubk file:_files' \
         --vboot-private-key'[Private key file to include in images]:vbprivk file:_files' \
         --kernel-cmdline'[Command line options for the kernel]:kernel cmdline:{_depthchargectl__cmdline;}' \
         --ignore-initramfs'[Do not include initramfs in images]' \
+        --zimage-initramfs-hack'[Initramfs support hack choice for zimage format]:zimage hack:(set-init-size pad-vmlinuz none)' \
         '1:command:(bless build config check list remove target write)' \
         '*::arg:->args' \
         ;
 
     case "$state:$line[1]" in
         args:bless)
             _arguments -S \
@@ -33,15 +41,15 @@
                 --description'[Human-readable description for the image]:image description:($(source /etc/os-release; echo "$NAME"))' \
                 --root'[Root device to add to kernel cmdline]:root device:{_depthchargectl__root; _depthchargectl__disk}' \
                 --compress'[Compression types to attempt]:compress:(none lz4 lzma)' \
                 --timestamp'[Build timestamp for the image]:timestamp:($(date "+%s"))' \
                 {-o,--output}'[Output image to path instead of storing in images-dir]:output path:_files' \
                 --kernel-release'[Release name for the kernel used in image name]:kernel release:{_depthchargectl__kernel;}' \
                 --kernel'[Kernel executable]:kernel:_files' \
-                --initramfs'[Ramdisk image]:initramfs:_files' \
+                --initramfs'[Ramdisk image]:*:initramfs:_files' \
                 --fdtdir'[Directory to search device-tree binaries for the board]:fdtdir:_directories' \
                 --dtbs'[Device-tree binary files to use instead of searching fdtdir]:*:dtb files:_files' \
                 ':kernel version:{_depthchargectl__kernel}' \
                 ;
             ;;
         args:config)
             _arguments -S \
@@ -130,8 +138,13 @@
 } 2>/dev/null
 
 function _depthchargectl__root {
     local root=($(findmnt --fstab -n -o SOURCE "/"))
     _describe root root
 } 2>/dev/null
 
+function _depthchargectl__boot {
+    local boot=($(findmnt --fstab -n -o SOURCE "/boot"))
+    _describe boot boot
+} 2>/dev/null
+
 _depthchargectl "$@"
```

### Comparing `depthcharge-tools-0.6.1/completions/_mkdepthcharge.bash` & `depthcharge-tools-0.6.2/completions/_mkdepthcharge.bash`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-# vim: filetype=sh
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools mkdepthcharge bash completions
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 _mkdepthcharge__file() {
     COMPREPLY+=($(compgen -f -- "$cur"))
     compopt -o filenames
     if [ "${#COMPREPLY[@]}" -eq 1 ]; then
         if [ -d "${COMPREPLY[0]}" ]; then
             compopt -o nospace
@@ -25,14 +29,15 @@
     local opts=(
         -h --help -V --version -v --verbose
         -d --vmlinuz -i --initramfs -b --dtbs
         -o --output --tmpdir -A --arch --format
         -C --compress -n --name --kernel-start
         --ramdisk-load-address --patch-dtbs --no-patch-dtbs
         --pad-vmlinuz --no-pad-vmlinuz
+        --set-init-size --no-set-init-size
         -c --cmdline --kern-guid --no-kern-guid --bootloader
         --keydir --keyblock --signprivate --signpubkey
     )
 
     case "$prev" in
         -d|--vmlinuz)   _mkdepthcharge__file ;;
         -i|--initramfs) _mkdepthcharge__file ;;
@@ -61,7 +66,9 @@
             COMPREPLY+=($(compgen -W "${opts[*]}" -- "$cur"))
             _mkdepthcharge__file
             ;;
     esac
 }
 
 complete -F _mkdepthcharge mkdepthcharge
+
+# vim: filetype=sh
```

### Comparing `depthcharge-tools-0.6.1/completions/_mkdepthcharge.zsh` & `depthcharge-tools-0.6.2/completions/_mkdepthcharge.zsh`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #compdef mkdepthcharge
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools mkdepthcharge zsh completions
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 function _mkdepthcharge {
     _arguments -S \
         {-d,--vmlinuz}'[Kernel executable]:vmlinuz file:_files' \
-        {-i,--initramfs}'[Ramdisk image]:initrd file:_files' \
+        {-i,--initramfs}'[Ramdisk image]:*:initrd files:_files' \
         {-b,--dtbs}'[Device-tree binary files]:*:dtbs files:_files' \
         {-h,--help}'[Show a help message.]' \
         {-v,--verbose}'[Print more detailed output.]' \
         {-V,--version}'[Print program version.]' \
         --tmpdir'[Directory to keep temporary files.]:temp dir:_directories' \
         --kernel-start'[Start of depthcharge kernel buffer in memory.]:kernel start:_numbers' \
         {-o,--output}'[Write resulting image to FILE.]:output:_files' \
@@ -16,14 +21,16 @@
         {-C,--compress}'[Compress vmlinuz with lz4 or lzma.]:compression:(none lz4 lzma)' \
         {-n,--name}'[Description of vmlinuz to put in the FIT.]:description:($(source /etc/os-release; echo "$NAME"))' \
         --ramdisk-load-address'[Add load address to FIT ramdisk image section.]:ramdisk load address:_numbers' \
         --patch-dtbs'[Add linux,initrd properties to device-tree binary files.]' \
         --no-patch-dtbs'[Do not add linux,initrd properties to device-tree binary files.]' \
         --pad-vmlinuz'[Pad the vmlinuz file for safe decompression]' \
         --no-pad-vmlinuz'[Do not pad the vmlinuz file for safe decompression]' \
+        --set-init-size'[Set init-size boot param for safe decompression]' \
+        --no-set-init-size'[Do not set init-size boot param for safe decompression]' \
         '*'{-c,--cmdline}'[Command-line parameters for the kernel.]:*:kernel cmdline:{_mkdepthcharge__cmdline}' \
         --kern-guid'[Prepend kern_guid=%U to the cmdline.]' \
         --no-kern-guid'[Do not prepend kern_guid=%U to the cmdline.]' \
         --bootloader'[Bootloader stub binary to use.]:bootloader file:_files' \
         --keydir'[Directory containing vboot keys to use.]:keys dir:_directories' \
         --keyblock'[The key block file (.keyblock).]:keyblock file:_files' \
         --signprivate'[Private key (.vbprivk) to sign the image.]:vbprivk file:_files' \
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/__init__.py` & `depthcharge-tools-0.6.2/depthcharge_tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools __init__.py
+# Copyright (C) 2020-2021 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import glob
 import logging
 import pathlib
 import pkg_resources
 import re
 import subprocess
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/boards.ini` & `depthcharge-tools-0.6.2/depthcharge_tools/boards.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-#
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools boards database
+# Copyright (C) 2021-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
+
 # The format of this boards.ini file is not stable. Instead of relying
 # on the section names and hierarchy here, you should add your own fully
 # specified sections with a unique codename, then set that codename as
 # your board, both in /etc/depthcharge-tools/config.d/*. For example:
 #
 #   [depthchargectl]
 #   board = custom-kevin
@@ -37,30 +42,80 @@
 [boards/amd64/alderlake/brya]
 codename = brya
 image-max-size = 512 MiB
 
 [boards/amd64/alderlake/brya/anahera]
 codename = anahera
 hwid-match = ^ANAHERA-TYOO.*
-name = HP Elite c640 14" G3 Chromebook / HP Elite c640 14" G3 Chromebook Enterprise
+name = HP Elite c640 14" G3 Chromebook (Enterprise)
 
 [boards/amd64/alderlake/brya/banshee]
 codename = banshee
 hwid-match = ^BANSHEE-UZTQ.*
 name = Framework Laptop Chromebook Edition
 
+[boards/amd64/alderlake/brya/brask]
+codename = brask
+
+[boards/amd64/alderlake/brya/brask/kinox]
+codename = kinox
+hwid-match = ^KINOX-WGMJ.*
+name = Lenovo ThinkCentre M60q Chromebox
+
+[boards/amd64/alderlake/brya/brask/kuldax]
+codename = kuldax
+hwid-match = ^KULDAX-DGSC.*
+name = ASUS Chromebox (Enterprise) 5 (CN67)
+
+[boards/amd64/alderlake/brya/brask/moli]
+codename = moli
+hwid-match = ^MOLI-.*
+name = Acer Chromebox CXI5
+
+[boards/amd64/alderlake/brya/crota]
+codename = crota
+hwid-match = ^CROTA-LPXP.*
+name = Dell Latitude 5430 Chromebook
+
+[boards/amd64/alderlake/brya/crota/crota360]
+codename = crota360
+hwid-match = ^CROTA360-QYFB.*
+name = Dell Latitude 5430 2-in-1 Chromebook
+
 [boards/amd64/alderlake/brya/felwinter]
 codename = felwinter
 hwid-match = ^FELWINTER-BDXJ.*
-name = ASUS Chromebook Flip CX5 / ASUS Chromebook Enterprise Flip CX5
+name = ASUS Chromebook (Enterprise) Flip CX5 (CX5601)
+
+[boards/amd64/alderlake/brya/gimble]
+codename = gimble
+hwid-match = ^GIMBLE-PVHI.*
+name = HP Chromebook x360 14 inch
 
 [boards/amd64/alderlake/brya/kano]
 codename = kano
+
+[boards/amd64/alderlake/brya/kano/0]
 hwid-match = ^KANO-VJXU.*
-name = Acer Chromebook Spin 714 (CP714-1WN) / Acer Chromebook Enterprise Spin 714 (CP714-1WN)
+name = Acer Chromebook (Enterprise) Spin 714 (CP714-1WN)
+
+[boards/amd64/alderlake/brya/kano/1]
+hwid-match = ^KANO-.*
+name = Acer Chromebook (Enterprise) Spin 714 (CP714-2WN)
+
+[boards/amd64/alderlake/brya/mithrax]
+codename = mithrax
+
+[boards/amd64/alderlake/brya/mithrax/0]
+hwid-match = ^MITHRAX-HKVS.*
+name = ASUS Chromebook (Enterprise) CX34, CB34 Flip (CX3401, CX3401FBA, CB3401)
+
+[boards/amd64/alderlake/brya/mithrax/1]
+hwid-match = ^MITHRAX-ISVS.*
+name = Asus Chromebook Vibe CX34 Flip (CX3401, CX3401FBA)
 
 [boards/amd64/alderlake/brya/osiris]
 codename = osiris
 hwid-match = ^OSIRIS-ATFE.*
 name = Acer Chromebook 516 GE (CBG516-1H)
 
 [boards/amd64/alderlake/brya/primus]
@@ -72,21 +127,101 @@
 codename = redrix
 hwid-match = ^REDRIX-CLQY .*
 name = HP Elite Dragonfly Chromebook
 
 [boards/amd64/alderlake/brya/taeko]
 codename = taeko
 hwid-match = ^TAEKO.*
-name = Lenovo IdeaPad Flex 5i Chromebook (14", 7)
+name = Lenovo (IdeaPad) Flex 5i Chromebook (14", 7)
+
+[boards/amd64/alderlake/brya/taniks]
+codename = taniks
+hwid-match = ^TANIKS.*
+name = Lenovo IdeaPad Gaming Chromebook 16
+
+[boards/amd64/alderlake/brya/tarlo]
+codename = tarlo
+hwid-match = ^TARLO[ |-].*
+name = Lenovo (IdeaPad) 5i Chromebook (16", 7)
+
+[boards/amd64/alderlake/brya/vell]
+codename = vell
+hwid-match = ^VELL-SVGZ .*
+name = HP Dragonfly Pro Chromebook
 
 [boards/amd64/alderlake/brya/volmar]
 codename = volmar
 hwid-match = ^VOLMAR-PGRU.*
 name = Acer Chromebook Vero 514
 
+[boards/amd64/alderlake/brya/volmar/zavala]
+codename = zavala
+hwid-match = ^ZAVALA-PSHU.*
+name = Acer Chromebook Vero 712 (CV872, CV872T)
+
+[boards/amd64/alderlake-n]
+codename = chipset-adln
+
+[boards/amd64/alderlake-n/nissa]
+codename = nissa
+image-format = zimage
+image-max-size = 512 MiB
+
+[boards/amd64/alderlake-n/nissa/craask]
+codename = craask
+hwid-match = ^CRAASK-HULX.*
+name = Acer Chromebook Spin 512 (R856T, R856T-TCO, R856TN, R856TN-TCO, R856LT, R856LT-TCO, R856LTN, R856LTN-TCO)
+
+[boards/amd64/alderlake-n/nissa/craask/craaskbowl]
+codename = craaskbowl
+hwid-match = ^CRAASKBOWL-GSKT.*
+name = Acer Chromebook Spin 511 (R756T, R756T-TCO, R756TN, R756TN-TCO, R756LT, R756LT-TCO, R756LTN, R756LTN-TCO)
+
+[boards/amd64/alderlake-n/nissa/craask/craaskvin]
+codename = craaskvin
+hwid-match = ^CRAASKVIN-HOWA.*
+name = Acer Chromebook 511 (C736, C736T, C736L, C736LT)
+
+[boards/amd64/alderlake-n/nissa/pujjo]
+codename = pujjo
+
+[boards/amd64/alderlake-n/nissa/pujjo/0]
+hwid-match = ^PUJJO-KTLR.*
+name = Lenovo 500e Yoga Chromebook Gen 4
+
+[boards/amd64/alderlake-n/nissa/pujjo/1]
+hwid-match = ^PUJJO-DCCV.*
+name = Lenovo (IdeaPad) Flex 3i Chromebook (12", 8)
+
+[boards/amd64/alderlake-n/nissa/pujjo/pujjoteen]
+codename = pujjoteen
+
+[boards/amd64/alderlake-n/nissa/pujjo/pujjoteen/0]
+hwid-match = ^PUJJOTEEN(15W)?[-| ].*
+name = Lenovo 14e Chromebook Gen 3 (15w)
+
+[boards/amd64/alderlake-n/nissa/pujjo/pujjoteen/1]
+hwid-match = ^PUJJOTEEN(15W)?[-| ].*
+name = Lenovo 14e Chromebook Gen 3 Chromebook
+
+[boards/amd64/alderlake-n/nissa/xivu]
+codename = xivu
+hwid-match = ^XIVU-YAZN.*
+name = ASUS Chromebook CR11 (CR1102C)
+
+[boards/amd64/alderlake-n/nissa/xivu/xivu360]
+codename = xivu360
+hwid-match = ^XIVU360-HRQS.*
+name = ASUS Chromebook CR11 (CR1102F)
+
+[boards/amd64/alderlake-n/nissa/yaviks]
+codename = yaviks
+hwid-match = ^YAVIKS-BVSW.*
+name = HP Chromebook 15.6”
+
 [boards/amd64/apollolake]
 codename = chipset-apl
 
 [boards/amd64/apollolake/coral]
 codename = coral
 image-max-size = 32 MiB
 
@@ -148,15 +283,15 @@
 name = Positivo Chromebook N2110
 
 [boards/amd64/apollolake/coral/blacktip360]
 codename = blacktip360
 
 [boards/amd64/apollolake/coral/blacktip360/0]
 hwid-match = ^BLACKTIP360 [A-Z0-9][A-Z0-9]B-([A-Z0-9\-])+
-name = CTL Chromebook NL7 / NL7T-360 / NL7TW-360
+name = CTL Chromebook NL7, NL7T-360, NL7TW-360
 
 [boards/amd64/apollolake/coral/blacktip360/1]
 hwid-match = ^BLACKTIP360 [A-Z0-9][A-Z0-9]C-([A-Z0-9\-])+
 name = Edxis Chromebook X11
 
 [boards/amd64/apollolake/coral/blacktip360/2]
 hwid-match = ^BLACKTIP360 [A-Z0-9][A-Z0-9]F-([A-Z0-9\-])+
@@ -238,15 +373,15 @@
 name = Acer Chromebook 11 (CB311-8H, CB311-8HT)
 
 [boards/amd64/apollolake/coral/whitetip]
 codename = whitetip
 
 [boards/amd64/apollolake/coral/whitetip/0]
 hwid-match = ^WHITETIP [A-Z0-9][A-Z0-9]D-([A-Z0-9\-])+
-name = CTL Chromebook J41 / J41T
+name = CTL Chromebook J41, J41T
 
 [boards/amd64/apollolake/coral/whitetip/1]
 hwid-match = ^WHITETIP [A-Z0-9][A-Z0-9]G-([A-Z0-9\-])+
 name = PCmerge Chromebook AL116
 
 [boards/amd64/apollolake/coral/whitetip/2]
 hwid-match = ^WHITETIP [A-Z0-9][A-Z0-9]E-([A-Z0-9\-])+
@@ -269,15 +404,15 @@
 
 [boards/amd64/apollolake/reef/0]
 hwid-match = ^REEF \w{3}-C\w{2}(-\w{3})*
 name = ASUS Chromebook Flip C213
 
 [boards/amd64/apollolake/reef/1]
 hwid-match = ^REEF \w{3}-B\w{2}(-\w{3})*
-name = Acer Chromebook Spin 11 (R751T / CP511)
+name = Acer Chromebook Spin 11 (R751T, CP511)
 
 [boards/amd64/apollolake/reef/pyro]
 codename = pyro
 hwid-match = ^PYRO .*
 name = Lenovo ThinkPad 11e 4th Gen Chromebook
 
 [boards/amd64/apollolake/reef/sand]
@@ -286,15 +421,15 @@
 name = Acer Chromebook 15 (CB515-1H, CB515-1HT)
 
 [boards/amd64/apollolake/reef/snappy]
 codename = snappy
 
 [boards/amd64/apollolake/reef/snappy/0]
 hwid-match = ^SNAPPY ([A-Z0-9])+-B[A-Z0-9][A-Z0-9]-([A-Z0-9])+-([A-Z0-9\-])+
-name = HP Chromebook 11 G6 EE / Chromebook 11a
+name = HP Chromebook 11/11a G6 EE
 
 [boards/amd64/apollolake/reef/snappy/1]
 hwid-match = ^SNAPPY ([A-Z0-9])+-C[A-Z0-9][A-Z0-9]-([A-Z0-9])+-([A-Z0-9\-])+
 name = HP Chromebook 14 G5
 
 [boards/amd64/apollolake/reef/snappy/2]
 hwid-match = ^SNAPPY ([A-Z0-9])+-[^BC].*
@@ -417,15 +552,15 @@
 hwid-match = ^HELI .*
 name = Haier Chromebook 11 G2
 
 [boards/amd64/baytrail/rambi/kip]
 codename = kip
 
 [boards/amd64/baytrail/rambi/kip/0]
-name = HP Chromebook 11 2100-2199 / HP Chromebook 11 G3
+name = HP Chromebook 11 2100-2199, 11 G3
 
 [boards/amd64/baytrail/rambi/kip/1]
 hwid-match = ^KIP [ABC].*
 name = HP Chromebook 11 G3/G4/G4 EE
 
 [boards/amd64/baytrail/rambi/kip/2]
 hwid-match = ^KIP [DE].*
@@ -567,15 +702,15 @@
 
 [boards/amd64/braswell/strago/terra/0]
 hwid-match = ^TERRA \w{3}-\w{3}-\w{3}-A.*
 name = ASUS Chromebook C202SA
 
 [boards/amd64/braswell/strago/terra/1]
 hwid-match = ^TERRA \w{3}-\w{3}-\w{3}-B.*
-name = ASUS Chromebook C300SA / C301SA
+name = ASUS Chromebook C300SA, C301SA
 
 [boards/amd64/braswell/strago/ultima]
 codename = ultima
 hwid-match = ^ULTIMA .*
 name = Lenovo ThinkPad 11e 3rd Gen Chromebook
 
 [boards/amd64/braswell/strago/wizpig]
@@ -617,14 +752,17 @@
 image-max-size = 16 MiB
 
 [boards/amd64/broadwell/auron/buddy]
 codename = buddy
 hwid-match = ^BUDDY .*
 name = Acer Chromebase 24
 
+[boards/amd64/broadwell/auron/buddy/cfm]
+codename = buddy-cfm
+
 [boards/amd64/broadwell/auron/gandof]
 codename = gandof
 hwid-match = ^GANDOF .*
 name = Toshiba Chromebook 2 (2015 Edition)
 
 [boards/amd64/broadwell/auron/lulu]
 codename = lulu
@@ -635,15 +773,14 @@
 codename = paine
 hwid-match = ^PAINE .*
 name = Acer Chromebook 11 (C740)
 
 [boards/amd64/broadwell/auron/samus]
 codename = samus
 hwid-match = ^SAMUS .*
-image-max-size = 16 MiB
 name = Google Chromebook Pixel (2015)
 
 [boards/amd64/broadwell/auron/yuna]
 codename = yuna
 hwid-match = ^YUNA .*
 name = Acer Chromebook 15 (CB5-571, C910)
 
@@ -652,18 +789,24 @@
 image-max-size = 16 MiB
 
 [boards/amd64/broadwell/jecht/guado]
 codename = guado
 hwid-match = ^GUADO .*
 name = ASUS Chromebox 2 (CN62)
 
+[boards/amd64/broadwell/jecht/guado/cfm]
+codename = guado-cfm
+
 [boards/amd64/broadwell/jecht/rikku]
 codename = rikku
 hwid-match = ^RIKKU .*
-name = Acer Chromebox CXI2 / CXV2
+name = Acer Chromebox CXI2, CXV2
+
+[boards/amd64/broadwell/jecht/rikku/cfm]
+codename = rikku-cfm
 
 [boards/amd64/broadwell/jecht/tidus]
 codename = tidus
 hwid-match = ^TIDUS .*
 name = Lenovo ThinkCentre Chromebox
 
 [boards/amd64/cezanne]
@@ -672,15 +815,15 @@
 [boards/amd64/cezanne/guybrush]
 codename = guybrush
 image-max-size = 512 MiB
 
 [boards/amd64/cezanne/guybrush/dewatt]
 codename = dewatt
 hwid-match = ^DEWATT[-| ].*
-name = Acer Chromebook Spin 514 [CP514-3H, CP514-3HH, CP514-3WH]
+name = Acer Chromebook Spin 514 (CP514-3H, CP514-3HH, CP514-3WH)
 
 [boards/amd64/cezanne/guybrush/nipperkin]
 codename = nipperkin
 hwid-match = ^NIPPERKIN[-| ].*
 name = HP Elite c645 G2 Chromebook
 
 [boards/amd64/cometlake]
@@ -701,40 +844,40 @@
 [boards/amd64/cometlake/hatch]
 codename = hatch
 image-max-size = 512 MiB
 
 [boards/amd64/cometlake/hatch/akemi]
 codename = akemi
 hwid-match = ^AKEMI-AOKF .*
-name = IdeaPad Flex 5i Chromebook (13", 5)
+name = Lenovo IdeaPad Flex 5i Chromebook (13", 5)
 
 [boards/amd64/cometlake/hatch/dragonair]
 codename = dragonair
 hwid-match = ^DRAGONAIR-.*
 name = HP Chromebook x360 14c
 
 [boards/amd64/cometlake/hatch/dratini]
 codename = dratini
 hwid-match = ^DRATINI-.*
-name = HP Pro c640 Chromebook / HP Pro c640 Chromebook Enterprise
+name = HP Pro c640 Chromebook (Enterprise)
 
 [boards/amd64/cometlake/hatch/helios]
 codename = helios
 hwid-match = ^HELIOS-.*
 name = ASUS Chromebook Flip C436FA
 
 [boards/amd64/cometlake/hatch/jinlon]
 codename = jinlon
 hwid-match = ^JINLON-YTGY .*
-name = HP Elite c1030 Chromebook / HP Chromebook x360 13c
+name = HP Elite c1030 Chromebook, HP Chromebook x360 13c
 
 [boards/amd64/cometlake/hatch/kindred]
 codename = kindred
 hwid-match = ^KINDRED-.*
-name = Acer Chromebook 712 [C871]
+name = Acer Chromebook 712 (C871)
 
 [boards/amd64/cometlake/hatch/kled]
 codename = kled
 hwid-match = ^KLED-.*
 name = Acer Chromebook Spin 713 (CP713-2W)
 
 [boards/amd64/cometlake/hatch/kohaku]
@@ -747,18 +890,48 @@
 hwid-match = ^NIGHTFURY[-| ].*
 name = Samsung Galaxy Chromebook 2
 
 [boards/amd64/cometlake/puff]
 codename = puff
 image-max-size = 512 MiB
 
+[boards/amd64/cometlake/puff/ambassador]
+codename = ambassador
+
+[boards/amd64/cometlake/puff/ambassador/0]
+hwid-match = ^AMBASSADOR-ANWJ.*
+name = ASUS Meet Compute System (Intel 10th Gen)
+
+[boards/amd64/cometlake/puff/ambassador/1]
+hwid-match = ^AMBASSADOR-NCZK.*
+name = CTL Meet Compute System (Intel 10th Gen)
+
+[boards/amd64/cometlake/puff/ambassador/2]
+hwid-match = ^AMBASSADOR-.*
+name = Meet Compute System (Intel 10th Gen)
+
+[boards/amd64/cometlake/puff/ambassador/genesis]
+codename = genesis
+hwid-match = ^GENESIS-.*
+name = Meet Compute System - Series One (Intel 10th Gen)
+
+[boards/amd64/cometlake/puff/ambassador/moonbuggy]
+codename = moonbuggy
+hwid-match = ^MOONBUGGY-.*
+name = Series One Board 65
+
+[boards/amd64/cometlake/puff/ambassador/scout]
+codename = scout
+hwid-match = ^SCOUT-.*
+name = Series One Desk 27
+
 [boards/amd64/cometlake/puff/dooly]
 codename = dooly
 hwid-match = ^DOOLY-SBGV.*
-name = HP Chromebase 21.5 inch All-in-One Desktop
+name = HP Chromebase 21.5" All-in-One Desktop
 
 [boards/amd64/cometlake/puff/duffy]
 codename = duffy
 hwid-match = ^DUFFY-.*
 name = ASUS Chromebox 4
 
 [boards/amd64/cometlake/puff/faffy]
@@ -777,15 +950,15 @@
 name = HP Chromebox G3
 
 [boards/amd64/cometlake/puff/wyvern]
 codename = wyvern
 
 [boards/amd64/cometlake/puff/wyvern/0]
 hwid-match = ^WYVERN-JLOF.*
-name = CTL Chromebox CBx2
+name = CTL Chromebox (Enterprise) CBx2
 
 [boards/amd64/cometlake/puff/wyvern/1]
 hwid-match = ^WYVERN-JOTV.*
 name = Promethean Chromebox 2
 
 [boards/amd64/cometlake/puff/wyvern/2]
 hwid-match = ^WYVERN-JRVR.*
@@ -801,25 +974,25 @@
 [boards/amd64/geminilake/octopus]
 codename = octopus
 image-max-size = 512 MiB
 
 [boards/amd64/geminilake/octopus/ampton]
 codename = ampton
 hwid-match = ^AMPTON .*
-name = ASUS Chromebook Flip C214 (EDU), ASUS Chromebook Flip C234 (CANADA CONSUMER)
+name = ASUS Chromebook Flip C214 (EDU), C234 (Canada)
 
 [boards/amd64/geminilake/octopus/apel]
 codename = apel
 hwid-match = ^APEL .*
 name = ASUS Chromebook C204
 
 [boards/amd64/geminilake/octopus/apele]
 codename = apele
 hwid-match = ^APELE .*
-name = CX1101CMA
+name = ASUS Chromebook CX1101 (CX1101CMA)
 
 [boards/amd64/geminilake/octopus/bloog]
 codename = bloog
 hwid-match = ^BLOOG .*
 name = HP Chromebook x360 12b
 
 [boards/amd64/geminilake/octopus/blooglet]
@@ -879,15 +1052,15 @@
 codename = dood
 hwid-match = ^DOOD .*
 name = NEC Chromebook Y2
 
 [boards/amd64/geminilake/octopus/dorp]
 codename = dorp
 hwid-match = ^DORP .*
-name = Chromebook 14 G6
+name = HP Chromebook 14 G6
 
 [boards/amd64/geminilake/octopus/droid]
 codename = droid
 
 [boards/amd64/geminilake/octopus/droid/0]
 hwid-match = ^DROID [D-F].*
 name = Acer Chromebook 314 (C933L/LT)
@@ -906,15 +1079,15 @@
 name = Dell Chromebook 3100
 
 [boards/amd64/geminilake/octopus/foob]
 codename = foob
 
 [boards/amd64/geminilake/octopus/foob/0]
 hwid-match = ^FOOB \w{3}-\w{3}-\w{3}-B\w{2}-.*
-name = CTL Chromebook VX11,  CTL Chromebook VX11T
+name = CTL Chromebook VX11, VX11T
 
 [boards/amd64/geminilake/octopus/foob/1]
 hwid-match = ^FOOB \w{3}-\w{3}-\w{3}-C\w{2}-.*
 name = Poin2 Chromebook 11P
 
 [boards/amd64/geminilake/octopus/foob360]
 codename = foob360
@@ -926,15 +1099,15 @@
 [boards/amd64/geminilake/octopus/foob360/1]
 hwid-match = ^FOOB360 \w{3}-\w{3}-\w{3}-C\w{2}-.*
 name = Poin2 Chromebook 11P
 
 [boards/amd64/geminilake/octopus/garfour]
 codename = garfour
 hwid-match = ^GARFOUR \w{3}-\w{3}-\w{3}-B\w{2}-.*
-name = CTL Chromebook NL81/NL81T
+name = CTL Chromebook NL81, NL81T
 
 [boards/amd64/geminilake/octopus/garg]
 codename = garg
 
 [boards/amd64/geminilake/octopus/garg/0]
 hwid-match = ^GARG \w{3}-\w{3}-\w{3}-L\w{2}-.*
 name = ADVAN Chromebook 116
@@ -993,15 +1166,15 @@
 
 [boards/amd64/geminilake/octopus/garg/14]
 hwid-match = ^GARG \w{3}-\w{3}-\w{3}-R\w{2}-.*
 name = XO Chromebook
 
 [boards/amd64/geminilake/octopus/garg/15]
 hwid-match = ^GARG \w{3}-\w{3}-\w{3}-N\w{2}-.*
-name = Zyrex Chromebook M432-1/M432-128 / Zyrex Chromebook 360-1
+name = Zyrex Chromebook (M432-1, M432-128), Zyrex Chromebook 360-1
 
 [boards/amd64/geminilake/octopus/garg360]
 codename = garg360
 
 [boards/amd64/geminilake/octopus/garg360/0]
 hwid-match = ^GARG360 \w{3}-\w{3}-\w{3}-L\w{2}-.*
 name = ADVAN Chromebook 116
@@ -1068,24 +1241,24 @@
 name = Dell Chromebook 3100 2-in-1
 
 [boards/amd64/geminilake/octopus/laser14]
 codename = laser14
 
 [boards/amd64/geminilake/octopus/laser14/0]
 hwid-match = ^LASER14 [D|E|G].{11}B.*
-name = IdeaPad 3 CB 14IGL05
+name = Lenovo IdeaPad 3 CB 14IGL05
 
 [boards/amd64/geminilake/octopus/laser14/1]
 hwid-match = ^LASER14 [ABC][A-Z0-9].*|^LASER14 [E].{11}A.*
-name = Lenovo Chromebook S340-14 and Lenovo Chromebook S340-14 Touch
+name = Lenovo Chromebook S340-14 (Touch)
 
 [boards/amd64/geminilake/octopus/lick]
 codename = lick
 hwid-match = ^LICK .*
-name = Ideapad 3 Chromebook
+name = Lenovo Ideapad 3 Chromebook 11IGL05
 
 [boards/amd64/geminilake/octopus/meep]
 codename = meep
 hwid-match = ^MEEP .*
 name = HP Chromebook x360 11 G2 EE
 
 [boards/amd64/geminilake/octopus/mimrock]
@@ -1109,23 +1282,23 @@
 name = Lenovo 100e Chromebook 2nd Gen
 
 [boards/amd64/geminilake/octopus/phaser360]
 codename = phaser360
 
 [boards/amd64/geminilake/octopus/phaser360/0]
 hwid-match = ^PHASER360 [G|H].{11}C.*
-name = IdeaPad Flex 3 CB 11IGL05
+name = Lenovo IdeaPad Flex 3 CB 11IGL05
 
 [boards/amd64/geminilake/octopus/phaser360/1]
 hwid-match = ^PHASER360 [ABCD][A-Z0-9].*|^PHASER360 [G|H|K|L|M].{11}B.*
 name = Lenovo 300e/500e Chromebook 2nd Gen
 
 [boards/amd64/geminilake/octopus/phaser360/2]
 hwid-match = ^PHASER360 [E|F][A-Z0-9].*|^PHASER360 [G|H|K|L|M|N].{11}C.*
-name = Lenovo Chromebook C340-11/300e/500e Chromebook 2nd Gen
+name = Lenovo Chromebook C340-11, 300e, 500e 2nd Gen
 
 [boards/amd64/geminilake/octopus/phaser360/3]
 hwid-match = ^PHASER360 [G|H|K].{11}A.*
 name = NEC Chromebook Y1
 
 [boards/amd64/geminilake/octopus/phaser360/4]
 hwid-match = ^PHASER360 [G|H|K|L|M].{11}D.*
@@ -1192,20 +1365,20 @@
 [boards/amd64/haswell/slippy]
 codename = slippy
 image-max-size = 16 MiB
 
 [boards/amd64/haswell/slippy/falco]
 codename = falco
 hwid-match = ^FALCO [ABC].*
-name = HP Chromebook 14 q000-q099 / HP Chromebook 14-SMB Atheros
+name = HP Chromebook 14 q000-q099, 14-SMB Atheros
 
 [boards/amd64/haswell/slippy/falco/li]
 codename = falco_li
 hwid-match = ^FALCO (D|LI-).*
-name = HP Chromebook 14 q000-q099 WP2 / HP Chromebook 14-SMB Intel Corp
+name = HP Chromebook 14 q000-q099 WP2, 14-SMB Intel Corp
 
 [boards/amd64/haswell/slippy/leon]
 codename = leon
 hwid-match = ^LEON .*
 name = Toshiba Chromebook
 
 [boards/amd64/haswell/slippy/peppy]
@@ -1250,30 +1423,30 @@
 codename = blipper
 hwid-match = ^BLIPPER-SBBR .*
 name = Lenovo 3i-15 Chromebook
 
 [boards/amd64/jasperlake/dedede/blipper/beetley]
 codename = beetley
 hwid-match = BEETLEY.*
-name = Lenovo Flex 3i Chromebook 15 IdeaPad Flex 3i Chromebook (15, 7)
+name = Lenovo (IdeaPad) Flex 3i Chromebook 15 (15, 7)
 
 [boards/amd64/jasperlake/dedede/boten]
 codename = boten
 hwid-match = ^BOTEN-YGHA.*
 name = Lenovo 500e Chromebook Gen 3
 
 [boards/amd64/jasperlake/dedede/boten/bookem]
 codename = bookem
 hwid-match = ^BOOKEM-LPEW.*
-name = 100e Chromebook Gen 3
+name = Lenovo 100e Chromebook Gen 3 (Intel)
 
 [boards/amd64/jasperlake/dedede/boten/botenflex]
 codename = botenflex
 hwid-match = ^BOTENFLEX.*
-name = Lenovo Flex 3i-11 Chromebook / IdeaPad Flex 3i Chromebook (11", 6)
+name = Lenovo (IdeaPad) Flex 3i-11 Chromebook (11", 6)
 
 [boards/amd64/jasperlake/dedede/bugzzy]
 codename = bugzzy
 hwid-match = ^BUGZZY.*
 name = Galaxy Chromebook 2 360
 
 [boards/amd64/jasperlake/dedede/cret]
@@ -1310,40 +1483,40 @@
 codename = galtic
 hwid-match = ^GALTIC-MOIP.*
 name = ASUS Chromebook CX1
 
 [boards/amd64/jasperlake/dedede/galtic/galith]
 codename = galith
 hwid-match = ^GALITH-HFKU.*
-name = ASUS Chromebook CX1500CKA
+name = ASUS Chromebook CX1500 (CX1500CKA)
 
 [boards/amd64/jasperlake/dedede/galtic/galith360]
 codename = galith360
 hwid-match = ^GALITH360-DSCL.*
-name = CX1500FKA
+name = ASUS Chromebook Flip CX1500 (CX1500FKA)
 
 [boards/amd64/jasperlake/dedede/galtic/gallop]
 codename = gallop
 hwid-match = ^GALLOP-FOBB.*
 name = ASUS Chromebook CX1700CKA
 
 [boards/amd64/jasperlake/dedede/galtic/galnat]
 codename = galnat
 hwid-match = ^GALNAT-RGDH.*
 name = ASUS Chromebook CX1 CX1102
 
 [boards/amd64/jasperlake/dedede/galtic/galnat360]
 codename = galnat360
-hwid-match = GALNAT360.*
-name = ASUS Chromebook Flip CX1 CX1102
+hwid-match = ^GALNAT360.*
+name = ASUS Chromebook Flip CX1 (CX1102)
 
 [boards/amd64/jasperlake/dedede/galtic/galtic360]
 codename = galtic360
 hwid-match = ^GALTIC360-RAKQ.*
-name = CX1400FKA
+name = ASUS Chromebook Flip CX1400 (CX1400FKA)
 
 [boards/amd64/jasperlake/dedede/kracko]
 codename = kracko
 hwid-match = ^KRACKO-WPBT .*
 name = CTL Chromebook NL72
 
 [boards/amd64/jasperlake/dedede/kracko/kracko360]
@@ -1351,15 +1524,15 @@
 
 [boards/amd64/jasperlake/dedede/kracko/kracko360/0]
 hwid-match = ^KRACKO360-BLXA .*
 name = CTL Chromebook NL72T
 
 [boards/amd64/jasperlake/dedede/kracko/kracko360/1]
 hwid-match = ^KRACKO360-LGAB .*
-name = LG Chromebook 11TC50Q/11TQ50Q
+name = LG Chromebook 11TC50Q, 11TQ50Q
 
 [boards/amd64/jasperlake/dedede/lantis]
 codename = lantis
 hwid-match = ^LANTIS-MEXL.*
 name = HP Chromebook 14a-na1
 
 [boards/amd64/jasperlake/dedede/lantis/landia]
@@ -1381,65 +1554,78 @@
 codename = magolor
 hwid-match = ^MAGOLOR-DUKI.*
 name = Acer Chromebook Spin 511 (R753T, R753TN, R752T-R)
 
 [boards/amd64/jasperlake/dedede/magolor/magister]
 codename = magister
 hwid-match = ^MAGISTER-RNPH.*
-name = Acer Chromebook Spin 314
+name = Acer Chromebook Spin 314 (CP314-1H, CP314-1HN)
 
 [boards/amd64/jasperlake/dedede/magolor/maglet]
 codename = maglet
 hwid-match = ^MAGLET-CFGF .*
 name = Acer Chromebook 512 (C852)
 
 [boards/amd64/jasperlake/dedede/magolor/maglia]
 codename = maglia
 hwid-match = ^MAGLIA-VYRC.*
 name = Acer Chromebook Spin 512 (R853TA, R853TNA)
 
 [boards/amd64/jasperlake/dedede/magolor/maglith]
 codename = maglith
 hwid-match = ^MAGLITH-STMU.*
-name = Acer Chromebook 511 (C734 , C734T, C733-R, C733T-R)
+name = Acer Chromebook 511 (C734, C734T, C733-R, C733T-R)
 
 [boards/amd64/jasperlake/dedede/magolor/magma]
 codename = magma
 hwid-match = ^MAGMA-QZPR.*
-name = Acer Chromebook 315 (CB315-4H , CB315-4HT)
+name = Acer Chromebook 315 (CB315-4H, CB315-4HT)
 
 [boards/amd64/jasperlake/dedede/magolor/magneto]
 codename = magneto
 
 [boards/amd64/jasperlake/dedede/magolor/magneto/0]
 hwid-match = ^MAGNETO-BWYB.*
-name = Acer Chromebook 314
+name = Acer Chromebook 314 (CB314-3H, CB314-3HT, C934, C934T)
 
 [boards/amd64/jasperlake/dedede/magolor/magneto/1]
 hwid-match = ^MAGNETO-SGGB.*
 name = Packard Bell Chromebook 314
 
+[boards/amd64/jasperlake/dedede/magolor/magneto/2]
+hwid-match = ^MAGNETO-SGGB.*
+name = Packard Bell Chromebook 314 (PCB314-2, PCB314-2T)
+
 [boards/amd64/jasperlake/dedede/magolor/magpie]
 codename = magpie
 hwid-match = ^MAGPIE-TQAU.*
 name = Acer Chromebook 317
 
 [boards/amd64/jasperlake/dedede/metaknight]
 codename = metaknight
 hwid-match = ^METAKNIGHT-GNDV.*
 name = NEC Chromebook Y3
 
+[boards/amd64/jasperlake/dedede/oscino]
+codename = oscino
+hwid-match = ^OSCINO-JZWV.*
+name = HP Fortis x360 11 G3 J Chromebook (Enterprise)
+
 [boards/amd64/jasperlake/dedede/pirika]
 codename = pirika
 
 [boards/amd64/jasperlake/dedede/pirika/0]
-hwid-match = ^PIRIKA-BMAD .*
-name = CTL Chromebook PX14E/PX14EX/PX14EXT
+hwid-match = ^PIRIKA-NPXS .*
+name = Axioo Chromebook P14
 
 [boards/amd64/jasperlake/dedede/pirika/1]
+hwid-match = ^PIRIKA-BMAD .*
+name = CTL Chromebook Enterprise, PX14E, PX14EX, PX14EXT
+
+[boards/amd64/jasperlake/dedede/pirika/2]
 hwid-match = ^PIRIKA-XAJY .*
 name = Gateway Chromebook 14
 
 [boards/amd64/jasperlake/dedede/pirika/pasara]
 codename = pasara
 hwid-match = ^PASARA-TZNR .*
 name = Gateway Chromebook 15
@@ -1464,33 +1650,54 @@
 name = Zyrex Chromebook M432-2
 
 [boards/amd64/jasperlake/dedede/sasuke]
 codename = sasuke
 hwid-match = ^SASUKE-.*
 name = Galaxy Chromebook Go
 
+[boards/amd64/jasperlake/dedede/sasukette]
+codename = sasukette
+hwid-match = ^SASUKETTE-QACT .*
+name = Galaxy Chromebook Go 11
+
 [boards/amd64/jasperlake/dedede/storo]
 codename = storo
 hwid-match = ^STORO-HIER.*
-name = ASUS Chromebook CR1100CKA
+name = ASUS Chromebook CR1100 (CR1100CKA)
 
 [boards/amd64/jasperlake/dedede/storo360]
 codename = storo360
 hwid-match = ^STORO360-JLGJ.*
-name = ASUS Chromebook Flip CR1100FKA
+name = ASUS Chromebook Flip CR1100 (CR1100FKA)
 
 [boards/amd64/kabylake]
 codename = chipset-kbl
 
 [boards/amd64/kabylake/fizz]
 codename = fizz
 hwid-match = ^FIZZ .*
 image-max-size = 32 MiB
 name = Chromebox Reference
 
+[boards/amd64/kabylake/fizz/endeavour]
+codename = endeavour
+hwid-match = ^ENDEAVOUR-HMDJ.*
+name = Meet Compute System - Series One
+
+[boards/amd64/kabylake/fizz/excelsior]
+codename = excelsior
+
+[boardsamd64//kabylake/fizz/excelsior/0]
+hwid-match = ^EXCELSIOR-URAR.*
+name = ASUS Meet Compute System
+
+[boardsamd64//kabylake/fizz/excelsior/1]
+hwid-match = ^EXCELSIOR-OOLH.*
+name = CTL Meet Compute System
+
 [boards/amd64/kabylake/fizz/jax]
 codename = jax
 
 [boards/amd64/kabylake/fizz/jax/0]
 hwid-match = ^JAX \w{3}-\w{3}-\w{1}4\w{1}(-\w{3})*
 name = AOpen Chromebox Commercial 2
 
@@ -1509,14 +1716,17 @@
 name = Acer Chromebox CXI3
 
 [boards/amd64/kabylake/fizz/teemo]
 codename = teemo
 hwid-match = ^TEEMO .*
 name = ASUS Chromebox 3 (CN65)
 
+[boards/amd64/kabylake/fizz/teemo/cfm]
+codename = fizz-cfm
+
 [boards/amd64/kabylake/fizz/wukong]
 codename = wukong
 
 [boards/amd64/kabylake/fizz/wukong/0]
 hwid-match = ^WUKONG [A-Z0-9][A-Z0-9]D.*
 name = CTL Chromebox CBx1
 
@@ -1541,14 +1751,17 @@
 image-max-size = 512 MiB
 
 [boards/amd64/kabylake/kalista/karma]
 codename = karma
 hwid-match = ^KARMA .*
 name = Acer Chromebase CA24I2
 
+[boards/amd64/kabylake/kalista/karma/cfm]
+codename = kalista-cfm
+
 [boards/amd64/kabylake/nami]
 codename = nami
 image-max-size = 32 MiB
 
 [boards/amd64/kabylake/nami/akali]
 codename = akali
 hwid-match = ^AKALI .*
@@ -1558,20 +1771,20 @@
 codename = akali360
 hwid-match = ^AKALI360 .*
 name = Acer Chromebook Spin 13 (CP713-1WN)
 
 [boards/amd64/kabylake/nami/bard]
 codename = bard
 hwid-match = ^BARD .*
-name = Acer Chromebook 715 (CB715-1W / CB715-1WT)
+name = Acer Chromebook 715 (CB715-1W, CB715-1WT)
 
 [boards/amd64/kabylake/nami/ekko]
 codename = ekko
 hwid-match = ^EKKO .*
-name = Acer Chromebook 714 (CB714-1W / CB714-1WT)
+name = Acer Chromebook 714 (CB714-1W, CB714-1WT)
 
 [boards/amd64/kabylake/nami/pantheon]
 codename = pantheon
 
 [boards/amd64/kabylake/nami/pantheon/0]
 hwid-match = ^PANTHEON [DEGHI][A-Z0-9].*
 name = Lenovo C340-15 Chromebook
@@ -1648,14 +1861,34 @@
 hwid-match = ^SHYVANA.* ...(-...){2}-..([DHLPTX37]-.*|[CGKOSW26]-([^A]|A(2A-A)*([^2].-.|.[^A]-.|..-[^A])).*)$
 name = ASUS Chromebook Flip C433
 
 [boards/amd64/kabylake/rammus/shyvana/1]
 hwid-match = ^SHYVANA.* ...((-...){0,3}|(-...){2}-..([ABEFIJMNQRUVYZ45].*|[CGKOSW26]-A(2A-A)*..))$
 name = ASUS Chromebook Flip C434
 
+[boards/amd64/mendocino]
+codename = chipset-mendocino
+
+[boards/amd64/mendocino/skyrim]
+codename = skyrim
+image-max-size = 512 MiB
+
+[boards/amd64/mendocino/skyrim/frostflow]
+codename = frostflow
+hwid-match = ^FROSTFLOW-INHJ.*
+name = ASUS Chromebook CM34 Flip
+
+[boards/amd64/mendocino/skyrim/winterhold]
+codename = winterhold
+
+[boards/amd64/mendocino/skyrim/winterhold/whiterun]
+codename = whiterun
+hwid-match = ^WHITERUN-WPKT.*
+name = Dell Latitude 3445 Chromebook
+
 [boards/amd64/picasso]
 codename = chipset-picasso
 
 [boards/amd64/picasso/zork]
 codename = zork
 image-max-size = 512 MiB
 
@@ -1668,30 +1901,30 @@
 codename = dirinboz
 hwid-match = ^DIRINBOZ-.*
 name = HP Chromebook 14a
 
 [boards/amd64/picasso/zork/ezkinil]
 codename = ezkinil
 hwid-match = ^EZKINIL-.*
-name = Acer Chromebook Spin 514  (CP514-1H, CP514-1W, CP514-1WH, CP514-1HH)
+name = Acer Chromebook Spin 514 (CP514-1H, CP514-1W, CP514-1WH, CP514-1HH)
 
 [boards/amd64/picasso/zork/gumboz]
 codename = gumboz
 hwid-match = ^GUMBOZ-JPUQ.*
 name = HP Chromebook x360 14a
 
 [boards/amd64/picasso/zork/jelboz360]
 codename = jelboz360
 hwid-match = ^JELBOZ360[-| ].*
-name = ASUS Chromebook Flip CM1
+name = ASUS Chromebook Flip CM1 (CM1400)
 
 [boards/amd64/picasso/zork/morphius]
 codename = morphius
 hwid-match = ^MORPHIUS[-| ].*
-name = Lenovo ThinkPad C13 Yoga Chromebook / Lenovo ThinkPad C13 Yoga Chromebook Enterprise
+name = Lenovo ThinkPad C13 Yoga Chromebook (Enterprise)
 
 [boards/amd64/picasso/zork/vilboz]
 codename = vilboz
 hwid-match = ^VILBOZ-LKSP.*
 name = Lenovo 100e Chromebook Gen 3
 
 [boards/amd64/picasso/zork/vilboz14]
@@ -1838,46 +2071,46 @@
 codename = aleena
 hwid-match = ^ALEENA[-| ].*
 name = Acer Chromebook 315 (CB315-2H)
 
 [boards/amd64/stoneyridge/grunt/barla]
 codename = barla
 hwid-match = ^BARLA[-| ].*
-name = HP Chromebook 11A G6 EE / HP Chromebook 11A G8 EE
+name = HP Chromebook 11A G6 EE, 11A G8 EE
 
 [boards/amd64/stoneyridge/grunt/careena]
 codename = careena
 hwid-match = ^CAREENA[-| ].*
-name = HP Chromebook 14 db0000-db0999 / HP Chromebook 14A G5
+name = HP Chromebook 14 db0000-db0999, 14A G5
 
 [boards/amd64/stoneyridge/grunt/kasumi]
 codename = kasumi
 hwid-match = ^KASUMI[-| ].*
 name = Acer Chromebook 311 (C721)
 
 [boards/amd64/stoneyridge/grunt/kasumi360]
 codename = kasumi360
 hwid-match = ^KASUMI360[-| ].*
 name = Acer Chromebook Spin 311 (R721T)
 
 [boards/amd64/stoneyridge/grunt/liara]
 codename = liara
 hwid-match = ^LIARA[-| ].*
-name = Lenovo 14e Chromebook, Lenovo Chromebook S345-14
+name = Lenovo 14e Chromebook, S345-14
 
 [boards/amd64/stoneyridge/grunt/treeya]
 codename = treeya
 
 [boards/amd64/stoneyridge/grunt/treeya/0]
 hwid-match = ^TREEYA .*|^TREEYA-BAUA .*
 name = Lenovo 100e Gen 2 AST
 
 [boards/amd64/stoneyridge/grunt/treeya/1]
 hwid-match = ^TREEYA-QCDF .*
-name = IdeaPad 3 Chromebook (11", 5)
+name = Lenovo IdeaPad 3 Chromebook (11", 5)
 
 [boards/amd64/stoneyridge/grunt/treeya360]
 codename = treeya360
 
 [boards/amd64/stoneyridge/grunt/treeya360/0]
 hwid-match = ^TREEYA360 .*|^TREEYA360-XFUX .*
 name = Lenovo 300e Gen 2 AST
@@ -1892,30 +2125,36 @@
 [boards/amd64/tigerlake/volteer]
 codename = volteer
 image-max-size = 512 MiB
 
 [boards/amd64/tigerlake/volteer/chronicler]
 codename = chronicler
 hwid-match = ^CHRONICLER-FYSO.*
-name = FMV Chromebook 14F, FMV Chromebook WM1/F3
+name = FMV Chromebook 14F, WM1/F3
 
 [boards/amd64/tigerlake/volteer/collis]
 codename = collis
 hwid-match = ^COLLIS-WMMD.*
 name = ASUS Chromebook Flip CX3
 
 [boards/amd64/tigerlake/volteer/copano]
 codename = copano
 hwid-match = ^COPANO-MRFF.*
 name = ASUS Chromebook Flip CX5 (CX5400)
 
 [boards/amd64/tigerlake/volteer/delbin]
 codename = delbin
+
+[boards/amd64/tigerlake/volteer/delbin/0]
 hwid-match = ^DELBIN-XHVI.*
-name = ASUS Chromebook Flip CX5 (CX5500), ASUS Chromebook Flip C536
+name = ASUS Chromebook Flip CX5 (CX5500), C536
+
+[boards/amd64/tigerlake/volteer/delbin/1]
+hwid-match = ^DELBIN-NHYA.*
+name = ASUS Chromebook Vibe CX55 Flip
 
 [boards/amd64/tigerlake/volteer/drobit]
 codename = drobit
 hwid-match = ^DROBIT-QSIM.*
 name = ASUS Chromebook CX9 (CX9400)
 
 [boards/amd64/tigerlake/volteer/eldrid]
@@ -1938,35 +2177,35 @@
 [boards/amd64/tigerlake/volteer/lindar/1]
 hwid-match = ^LINDAR-LCDF.*
 name = Lenovo Slim 5 Chromebook
 
 [boards/amd64/tigerlake/volteer/lindar/lillipup]
 codename = lillipup
 hwid-match = ^LILLIPUP-MQUZ.*
-name = IdeaPad Flex 5i Chromebook (13", 6)
+name = Lenovo IdeaPad Flex 5i Chromebook (13", 6)
 
 [boards/amd64/tigerlake/volteer/voema]
 codename = voema
 hwid-match = ^VOEMA-DHAS .*
 name = Acer Chromebook Spin 514 (CP514-2H)
 
 [boards/amd64/tigerlake/volteer/volet]
 codename = volet
 hwid-match = ^VOLET-XIYN.*|^VOLET-ZZCR.*
-name = Acer Chromebook 515 (CB515-1W/CB515-1WT)
+name = Acer Chromebook 515 (CB515-1W, CB515-1WT)
 
 [boards/amd64/tigerlake/volteer/voxel]
 codename = voxel
 hwid-match = ^VOXEL-GFMQ.*
 name = Acer Chromebook Spin 713 (CP713-3W)
 
 [boards/amd64/tigerlake/volteer/voxel/volta]
 codename = volta
 hwid-match = ^VOLTA-OIFF .*
-name = Acer Chromebook 514 (CB514-1W/CB514-1WT)
+name = Acer Chromebook 514 (CB514-1W, CB514-1WT)
 
 [boards/amd64/whiskeylake]
 codename = chipset-whl
 
 [boards/amd64/whiskeylake/sarien]
 codename = sarien
 hwid-match = ^SARIEN-.*
@@ -1992,53 +2231,55 @@
 
 [boards/arm/exynos5/daisy]
 codename = daisy
 dt-compatible = google,daisy
 image-max-size = 8 MiB
 image-start-address = 0x42000000
 fit-ramdisk-load-address = 0x50000000
+loads-dtb-off-by-one = True
 loads-fit-ramdisk = True
 
 [boards/arm/exynos5/daisy/skate]
 codename = skate
 dt-compatible = google,skate
 hwid-match = ^SKATE .*
 name = HP Chromebook 11 G2
 
 [boards/arm/exynos5/daisy/snow]
 codename = snow
 dt-compatible = google,snow
 hwid-match = ^SNOW .*
-name = Samsung Chromebook - XE303
+name = Samsung Chromebook (XE303C12)
 
 [boards/arm/exynos5/daisy/spring]
 codename = spring
 dt-compatible = google,spring
 hwid-match = ^SPRING .*
 name = HP Chromebook 11 G1
 
 [boards/arm/exynos5/peach]
 codename = peach
 dt-compatible = google,peach
 image-max-size = 8 MiB
 image-start-address = 0x20008000
 fit-ramdisk-load-address = 0x44000000
+loads-dtb-off-by-one = True
 loads-fit-ramdisk = True
 
 [boards/arm/exynos5/peach/pi]
 codename = pi
 dt-compatible = google,pi
 hwid-match = ^PI .*
-name = Samsung Chromebook 2 13"
+name = Samsung Chromebook 2 13" (XE503C32)
 
 [boards/arm/exynos5/peach/pit]
 codename = pit
 dt-compatible = google,pit
 hwid-match = ^PIT ([^TEST.*]).*
-name = Samsung Chromebook 2 11"
+name = Samsung Chromebook 2 11" (XE503C12)
 
 [boards/arm/ipq4019]
 codename = chipset-ipq4019
 dt-compatible = qcom,ipq4019
 
 [boards/arm/ipq4019/gale]
 codename = gale
@@ -2110,23 +2351,23 @@
 
 [boards/arm/rk3288/veyron/jerry]
 codename = jerry
 dt-compatible = google,veyron-jerry
 
 [boards/arm/rk3288/veyron/jerry/0]
 hwid-match = ^JERRY \w{3}-\w{3}-\w{3}-B\w{2}.*
-name = CTL J2 / J4 Chromebook
+name = CTL J2, J4 Chromebook
 
 [boards/arm/rk3288/veyron/jerry/1]
 hwid-match = ^JERRY \w{3}-\w{3}-\w{3}-D\w{2}(-\w{3})*$
 name = EduGear Chromebook K
 
 [boards/arm/rk3288/veyron/jerry/2]
 hwid-match = ^JERRY \w{3}-\w{3}-\w{3}-F\w{2}(-\w{3})*$
-name = Epik 11.6" Chromebook  ELB1101
+name = Epik 11.6" Chromebook ELB1101
 
 [boards/arm/rk3288/veyron/jerry/3]
 hwid-match = ^JERRY \w{3}-\w{3}-\w{3}-A\w{2}(-\w{3})*$
 name = HiSense Chromebook 11
 
 [boards/arm/rk3288/veyron/jerry/4]
 hwid-match = ^JERRY \w{3}-\w{3}-\w{3}-H\w{2}(-\w{3})*$
@@ -2306,15 +2547,15 @@
 
 [boards/arm64/mt8173/oak/hana/7]
 hwid-match = ^HANA ([A-Z0-9])+-([A-Z0-9])+-[A-Z0-9][A-Z0-9]B-([A-Z0-9\-])+
 name = Poin2 Chromebook 14
 
 [boards/arm64/mt8173/oak/hana/8]
 hwid-match = ^HANA ([A-Z0-9])+-([A-Z0-9])+-[A-Z0-9][A-Z0-9]G-([A-Z0-9\-])+
-name = Prowise Chromebook Eduline / Prowise Chromebook Eduline 360
+name = Prowise Chromebook Eduline (360)
 
 [boards/arm64/mt8183]
 codename = chipset-mt8183
 dt-compatible = mediatek,mt8183
 
 [boards/arm64/mt8183/kukui]
 codename = kukui
@@ -2342,30 +2583,30 @@
 hwid-match = ^DAMU.*
 name = ASUS Chromebook Flip CM3200FVA
 
 [boards/arm64/mt8183/kukui/jacuzzi/fennel]
 codename = fennel
 dt-compatible = google,fennel
 hwid-match = ^FENNEL-.*
-name = IdeaPad Flex 3 Chromebook
+name = Lenovo IdeaPad Flex 3 Chromebook
 
 [boards/arm64/mt8183/kukui/jacuzzi/fennel14]
 codename = fennel14
 dt-compatible = google,fennel
 hwid-match = ^FENNEL14-.*
-name = IdeaPad 3 Chromebook
+name = Lenovo IdeaPad 3 Chromebook
 
 [boards/arm64/mt8183/kukui/jacuzzi/icarus]
 codename = icarus
 
 [boards/arm64/mt8183/kukui/jacuzzi/icarus/cozmo]
 codename = cozmo
 dt-compatible = google,cozmo
 hwid-match = ^COZMO.*
-name = Acer Chromebook 314 (CB314-2H/CB314-2HT)
+name = Acer Chromebook 314 (CB314-2H, CB314-2HT)
 
 [boards/arm64/mt8183/kukui/jacuzzi/icarus/pico]
 codename = pico
 dt-compatible = google,pico
 hwid-match = ^PICO-EXEM.*
 name = Acer Chromebook Spin 311 - R722T
 
@@ -2400,27 +2641,27 @@
 
 [boards/arm64/mt8183/kukui/jacuzzi/willow]
 codename = willow
 dt-compatible = google,willow
 
 [boards/arm64/mt8183/kukui/jacuzzi/willow/0]
 hwid-match = ^WILLOW-ZZCR .*
-name = Acer Chromebook 311 (C722/C722T)
+name = Acer Chromebook 311 (C722, C722T)
 
 [boards/arm64/mt8183/kukui/jacuzzi/willow/1]
 hwid-match = ^WILLOW-TFIY .*
-name = Acer Chromebook 311 (C722/C722T)
+name = Acer Chromebook 311 (C722, C722T)
 
 [boards/arm64/mt8183/kukui/kakadu]
 codename = kakadu
 dt-compatible = google,kadaku
 hwid-match = ^KAKADU-WFIQ.*
 name = ASUS Chromebook Detachable CM3
 
-[boards/arm64/mt8183/kukui/kakadu/katsu]
+[boards/arm64/mt8183/kukui/katsu]
 codename = katsu
 dt-compatible = google,katsu
 hwid-match = ^KATSU.*
 name = ASUS Chromebook Detachable CZ1
 
 [boards/arm64/mt8183/kukui/kodama]
 codename = kodama
@@ -2428,15 +2669,49 @@
 hwid-match = ^KODAMA.*
 name = Lenovo 10e Chromebook Tablet
 
 [boards/arm64/mt8183/kukui/krane]
 codename = krane
 dt-compatible = google,krane
 hwid-match = ^KRANE-ZDKS .*
-name = Lenovo Chromebook Duet / Lenovo Ideapad Duet Chromebook
+name = Lenovo (IdeaPad) Chromebook Duet
+
+[boards/arm64/mt8186]
+codename = chipset-mt8186
+dt-compatible = mediatek,mt8186
+
+[boards/arm64/mt8186/corsola]
+codename = corsola
+dt-compatible = google,corsola
+image-max-size = 512 MiB
+
+[boards/arm64/mt8186/corsola/steelix]
+codename = steelix
+hwid-match = ^STEELIX-VZSZ.*
+name = Lenovo 300e Yoga Chromebook Gen 4
+
+[boards/arm64/mt8186/corsola/steelix/magneton]
+codename = magneton
+hwid-match = ^MAGNETON-LCKC.*
+name = Lenovo IP Slim 3 Chrome 14M868
+
+[boards/arm64/mt8186/corsola/steelix/rusty]
+codename = rusty
+hwid-match = ^RUSTY-ZNCE.*
+name = Lenovo 100e Chromebook Gen 4
+
+[boards/arm64/mt8186/corsola/tentacruel]
+codename = tentacruel
+hwid-match = ^TENTACRUEL-VAFH.*
+name = ASUS Chromebook CM14 Flip (CM1402F)
+
+[boards/arm64/mt8186/corsola/tentacruel/tentacool]
+codename = tentacool
+hwid-match = ^TENTACOOL-ZLJE.*
+name = ASUS Chromebook CM14 (CM1402C)
 
 [boards/arm64/mt8192]
 codename = chipset-mt8192
 dt-compatible = mediatek,mt8192
 
 [boards/arm64/mt8192/asurada]
 codename = asurada
@@ -2464,42 +2739,42 @@
 dt-compatible = google,cherry
 image-max-size = 512 MiB
 
 [boards/arm64/mt8195/cherry/dojo]
 codename = dojo
 dt-compatible = google,dojo
 hwid-match = ^DOJO-EJPG.*
-name = HP Chromebook x360 13.3" - 13b-ca0xxx
+name = HP Chromebook x360 13.3" (13b-ca0xxx)
 
 [boards/arm64/mt8195/cherry/tomato]
 codename = tomato
 dt-compatible = google,tomato
 hwid-match = ^TOMATO-LYVN.*
-name = ACER Chromebook Spin 513
+name = ACER Chromebook (Enterprise) Spin 513 (CP513-2H)
 
 [boards/arm64/qc7180]
 codename = chipset-qc7180
 dt-compatible = qcom,sc7180
 
 [boards/arm64/qc7180/trogdor]
 codename = trogdor
 dt-compatible = google,trogdor
 image-max-size = 512 MiB
 
 [boards/arm64/qc7180/trogdor/kingoftown]
 codename = kingoftown
 dt-compatible = google,kingoftown
 hwid-match = ^KINGOFTOWN-KDDA.*
-name = HP Fortis 11 G9 Q Chromebook / Chromebook Enterprise
+name = HP Fortis 11 G9 Q Chromebook (Enterprise)
 
 [boards/arm64/qc7180/trogdor/lazor]
 codename = lazor
 dt-compatible = google,lazor(-rev\d+)?(-sku[02])?
 hwid-match = ^LAZOR.*
-name = Acer Chromebook Spin 513, CP513-1H/1HL, R841T/LT
+name = Acer Chromebook Spin 513 (CP513-1H/1HL, R841T/LT)
 
 [boards/arm64/qc7180/trogdor/lazor/limozeen]
 codename = limozeen
 dt-compatible = google,lazor(-rev\d+)?(-sku[456])?
 hwid-match = ^LIMOZEEN.*
 name = Acer Chromebook 511 (C741L/C741LT)
 
@@ -2531,27 +2806,27 @@
 hwid-match = ^COACHZ.*
 name = HP Chromebook x2 11c
 
 [boards/arm64/qc7180/trogdor/strongbad/homestar]
 codename = homestar
 dt-compatible = google,homestar
 hwid-match = ^HOMESTAR-MBLE.*
-name = Lenovo Chromebook Duet 5 / IdeaPad Duet 5 Chromebook
-
-[boards/arm64/qc7180/trogdor/strongbad/wormdingler]
-codename = wormdingler
-dt-compatible = google,wormdingler
-hwid-match = ^WORMDINGLER-JQAO.*
-name = Lenovo Chromebook Duet 3 / IdeaPad Duet 3 Chromebook
+name = Lenovo (IdeaPad) Chromebook Duet 5
 
 [boards/arm64/qc7180/trogdor/strongbad/quackingstick]
 codename = quackingstick
 dt-compatible = google,quackingstick
 hwid-match = ^QUACKINGSTICK.*
-name = Acer Chromebook Tab 510 / Enterprise Tab 510
+name = Acer Chromebook (Enterprise) Tab 510
+
+[boards/arm64/qc7180/trogdor/strongbad/wormdingler]
+codename = wormdingler
+dt-compatible = google,wormdingler
+hwid-match = ^WORMDINGLER-JQAO.*
+name = Lenovo (IdeaPad) Chromebook Duet 3 (Education Edition)
 
 [boards/arm64/qcs404]
 codename = chipset-qcs404
 dt-compatible = qcom,qcs404
 
 [boards/arm64/qcs404/mistral]
 codename = mistral
@@ -2574,26 +2849,26 @@
 hwid-match = ^BOB .*
 name = ASUS Chromebook Flip C101PA
 
 [boards/arm64/rk3399/gru/kevin]
 codename = kevin
 dt-compatible = google,kevin
 hwid-match = ^KEVIN .*
-name = Samsung Chromebook Plus
+name = Samsung Chromebook Plus (XE513C24)
 
 [boards/arm64/rk3399/gru/scarlet]
 codename = scarlet
 dt-compatible = google,scarlet
 hwid-match = ^SCARLET .*
 name = Acer Chromebook Tab 10
 
 [boards/arm64/rk3399/gru/scarlet/dru]
 codename = dru
 hwid-match = ^DRU .*
-name = Acer Chromebook Tab 10 (D651N / D650N)
+name = Acer Chromebook Tab 10 (D651N, D650N)
 
 [boards/arm64/rk3399/gru/scarlet/druwl]
 codename = druwl
 
 [boards/arm64/rk3399/gru/scarlet/druwl/0]
 hwid-match = ^DRUWL [A-Z0-9][A-Z0-9]D.*
 name = AOpen Chromebook Commercial Tab
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/__init__.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl command
+# Copyright (C) 2020-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import collections
 import configparser
 import copy
 import glob
 import logging
@@ -35,14 +40,16 @@
 from depthcharge_tools.utils.platform import (
     Architecture,
     vboot_keys,
     cros_hwid,
     dt_compatibles,
     is_cros_boot,
     is_cros_libreboot,
+    kernel_cmdline,
+    proc_cmdline,
 )
 from depthcharge_tools.utils.string import (
     parse_bytesize,
 )
 
 
 class Board:
@@ -107,14 +114,18 @@
         return self._config.getboolean("loads-zimage-ramdisk", False)
 
     @property
     def loads_fit_ramdisk(self):
         return self._config.getboolean("loads-fit-ramdisk", False)
 
     @property
+    def loads_dtb_off_by_one(self):
+        return self._config.getboolean("loads-dtb-off-by-one", False)
+
+    @property
     def fit_ramdisk_load_address(self):
         addr = self._config.get("fit-ramdisk-load-address", None)
         return parse_bytesize(addr)
 
     @property
     def image_start_address(self):
         addr = self._config.get("image-start-address", None)
@@ -205,15 +216,15 @@
             for c in cmdline:
                 lhs, _, rhs = c.partition("=")
                 if lhs.lower() == "root":
                     root = rhs
 
             if root:
                 self.logger.info(
-                    "Using root '{}' set in user configured cmdline."
+                    "Using root '{}' set in cmdline."
                     .format(root)
                 )
                 return str(root)
 
             self.logger.info(
                 "Defaulting to current system root '/'."
             )
@@ -222,23 +233,29 @@
         if os.path.ismount(Path(root).resolve()):
             self.logger.info(
                 "Using root argument '{}' as the system to work on."
                 .format(root)
             )
             return Path(root).resolve()
 
-        self.logger.info(
-            "Using root argument '{}' as a device description."
-            .format(root)
-        )
+        if root in (None, "", "none", "None"):
+            self.logger.info(
+                "Using no root argument for the kernel cmdline."
+                .format(root)
+            )
+        else:
+            self.logger.info(
+                "Using root argument '{}' as a device description."
+                .format(root)
+            )
 
         return str(root)
 
     @global_options.add
-    @Argument("--root-mountpoint", nargs=1, help=argparse.SUPPRESS)
+    @Argument("--root-mountpoint", nargs=1, metavar="DIR")
     def root_mountpoint(self, mnt=None):
         """Root mountpoint of the system to work on."""
         if mnt:
             mnt = Path(mnt).resolve()
             self.logger.info(
                 "Using root mountpoint '{}' from given argument."
                 .format(mnt)
@@ -257,15 +274,15 @@
             key=lambda p: len(p.parents),
         )
 
         if len(mountpoints) > 1:
             mnt = mountpoints[0]
             self.logger.warning(
                 "Choosing '{}' from multiple root mountpoints: {}."
-                .format(mnt, mountpoints)
+                .format(mnt, ", ".join(str(m) for m in mountpoints))
             )
             return mnt
 
         elif mountpoints:
             mnt = mountpoints[0]
             if mnt != Path("/").resolve():
                 self.logger.info(
@@ -277,15 +294,15 @@
         self.logger.warning(
             "Couldn't find root mountpoint, falling back to '/'."
         )
 
         return Path("/").resolve()
 
     @global_options.add
-    @Argument("--boot-mountpoint", nargs=1, help=argparse.SUPPRESS)
+    @Argument("--boot-mountpoint", nargs=1, metavar="DIR")
     def boot_mountpoint(self, boot=None):
         """Boot mountpoint of the system to work on."""
         if boot:
             boot = Path(boot).resolve()
             self.logger.info(
                 "Using boot mountpoint '{}' from given argument."
                 .format(boot)
@@ -304,15 +321,15 @@
                 "Boot partition '{}' for specified root is not mounted."
                 .format(device)
             )
 
         if len(mountpoints) > 1:
             self.logger.warning(
                 "Choosing '{}' from multiple /boot mountpoints: {}."
-                .format(mountpoints[0], mountpoints)
+                .format(mountpoints[0], ", ".join(str(m) for m in mountpoints))
             )
 
         if mountpoints:
             return mountpoints[0]
 
         root = self.root_mountpoint
         boot = (root / "boot").resolve()
@@ -354,16 +371,41 @@
             'board': self.board.codename if self.board else "none",
             'images-dir': str(self.images_dir),
             'vboot-keyblock': str(self.vboot_keyblock),
             'vboot-public-key': str(self.vboot_public_key),
             'vboot-private-key': str(self.vboot_private_key),
             'kernel-cmdline': " ".join(self.kernel_cmdline),
             'ignore-initramfs': str(self.ignore_initramfs),
+            'zimage-initramfs-hack': str(self.zimage_initramfs_hack),
         })
 
+        if self.board is not None:
+            def pattern(regex):
+                try:
+                    return str(regex.pattern)
+                except:
+                    return "None"
+
+            self.config.update({
+                "arch": str(self.board.arch),
+                "codename": str(self.board.codename),
+                "boots-lz4-kernel": str(self.board.boots_lz4_kernel),
+                "boots-lzma-kernel": str(self.board.boots_lzma_kernel),
+                "dt-compatible": pattern(self.board.dt_compatible),
+                "fit-ramdisk-load-address": str(self.board.fit_ramdisk_load_address),
+                "hwid-match": pattern(self.board.hwid_match),
+                "image-format": str(self.board.image_format),
+                "image-max-size": str(self.board.image_max_size),
+                "image-start-address": str(self.board.image_start_address),
+                "loads-dtb-off-by-one": str(self.board.loads_dtb_off_by_one),
+                "loads-fit-ramdisk": str(self.board.loads_fit_ramdisk),
+                "loads-zimage-ramdisk": str(self.board.loads_zimage_ramdisk),
+                "name": str(self.board.name),
+            })
+
     @config_options.add
     @Argument("--config", nargs=1)
     def config(self, file_=None):
         """Additional configuration file to read"""
         if isinstance(file_, configparser.SectionProxy):
             parser = file_.parser
 
@@ -615,17 +657,15 @@
         # Use generic boards per cpu architecture, since we couldn't
         # detect this system as a proper board
         arch = platform.machine()
         if arch in Architecture.arm_32:
             sectname = "boards/arm"
         elif arch in Architecture.arm_64:
             sectname = "boards/arm64"
-        elif arch in Architecture.x86_32:
-            sectname = "boards/x86"
-        elif arch in Architecture.x86_64:
+        elif arch in Architecture.x86:
             sectname = "boards/amd64"
         board = boards.get(sectname, None)
         if board is not None:
             self.logger.warning(
                 "Assuming a generic board of architecture '{}'."
                 .format(board.arch)
             )
@@ -735,35 +775,70 @@
 
     @config_options.add
     @Argument("--kernel-cmdline", nargs="+", metavar="CMD")
     def kernel_cmdline(self, *cmds):
         """Command line options for the kernel"""
         # Break cyclic dependencies here
         yield []
+        cmdline_src = "given options"
 
         if len(cmds) == 0:
             cmdline = self.config.get("kernel-cmdline")
             if cmdline is not None:
                 cmds = shlex.split(cmdline)
+                cmdline_src = "configuration"
+
+        if len(cmds) == 0:
+            cmds = kernel_cmdline(self.root_mountpoint)
+            cmdline_src = "/etc/kernel/cmdline"
+
+        if len(cmds) == 0:
+            if self.root_mountpoint == Path("/").resolve():
+                cmds = [
+                    cmd for cmd in proc_cmdline()
+                    if cmd.split("=", 1)[0] not in (
+                        "root", "initrd", "kern_guid", "BOOT_IMAGE",
+                        "cros_secure", "cros_legacy", "cros_efi",
+                    )
+                ]
+                cmdline_src = "/proc/cmdline"
 
         flat_cmds = []
         for cmd in cmds:
             flat_cmds.extend(shlex.split(cmd))
 
+        if flat_cmds:
+            self.logger.info(
+                "Using kernel cmdline from {}: {}"
+                .format(cmdline_src, " ".join(flat_cmds))
+            )
+
         return flat_cmds
 
     @config_options.add
     @Argument("--ignore-initramfs", ignore=True)
     def ignore_initramfs(self, ignore=None):
         """Do not include initramfs in images"""
         if ignore is None:
             ignore = self.config.getboolean("ignore-initramfs", False)
 
         return ignore
 
+    @config_options.add
+    @Argument("--zimage-initramfs-hack", nargs=1, help=argparse.SUPPRESS)
+    def zimage_initramfs_hack(self, hack=None):
+        """Which initramfs support hack should be used for zimage format"""
+        if hack is None:
+            hack = self.config.get("zimage-initramfs-hack", "init-size")
+
+        if hack in ("None", "none"):
+            hack = None
+
+        return hack
+
     @Subparsers()
     def command(self, cmd):
         """Supported subcommands"""
 
     def __call__(self):
         if hasattr(type(self), "list"):
             self.logger.info("No subcommand given, defaulting to list")
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_bless.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_bless.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl bless subcommand
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 import subprocess
 
 from depthcharge_tools import __version__
 from depthcharge_tools.utils.argparse import (
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_build.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl build subcommand
+# Copyright (C) 2020-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import collections
 import configparser
 import logging
 import os
 import shlex
@@ -23,14 +28,15 @@
     Partition,
 )
 from depthcharge_tools.utils.pathlib import (
     copy,
 )
 from depthcharge_tools.utils.platform import (
     KernelEntry,
+    cpu_microcode,
     vboot_keys,
     installed_kernels,
     root_requires_initramfs,
 )
 from depthcharge_tools.utils.subprocess import (
     fdtget,
 )
@@ -127,14 +133,26 @@
         if board is None:
             raise ValueError(
                 "Cannot build depthcharge images when no board is specified.",
             )
 
         return board
 
+    @depthchargectl.zimage_initramfs_hack.copy()
+    def zimage_initramfs_hack(self, hack=None):
+        hack = super().zimage_initramfs_hack
+
+        if hack not in (None, "set-init-size", "pad-vmlinuz"):
+            raise ValueError(
+                "Unknown zimage initramfs support hack '{}'."
+                .format(hack)
+            )
+
+        return hack
+
     @Group
     def custom_kernel_options(self):
         """Custom kernel specification"""
 
     @custom_kernel_options.add
     @Argument("--kernel-release", nargs=1)
     def kernel_release(self, name=None):
@@ -161,45 +179,51 @@
 
         elif file_ is None:
             raise ValueError("No vmlinuz file found.")
 
         return Path(file_)
 
     @custom_kernel_options.add
-    @Argument("--initramfs", nargs=1)
-    def initrd(self, file_=None):
-        """Ramdisk image"""
+    @Argument("--initramfs", nargs='+')
+    def initrd(self, *files):
+        """Ramdisk images"""
         # Trigger more important errors first
         self.kernel
 
-        if file_ is None and self.kernel_version is not None:
+        if not files and self.kernel_version is not None:
             if self.kernel == self.kernel_version.kernel:
-                file_ = self.kernel_version.initrd
+                microcode = cpu_microcode(self.boot_mountpoint)
+                files = [*microcode, self.kernel_version.initrd]
 
         if self.ignore_initramfs:
-            self.logger.warning(
-                "Ignoring initramfs '{}' as configured."
-                .format(file_)
-            )
+            for file in files:
+                self.logger.warning(
+                    "Ignoring initramfs '{}' as configured."
+                    .format(file)
+                )
+            return None
+
+        if len(files) == 1 and files[0] in (None, "None", "none"):
+            self.logger.warning("Not using initramfs.")
             return None
 
         # Initramfs is optional.
-        if file_ is None and self.kernel_release is not None:
+        if not files and self.kernel_release is not None:
             self.logger.info(
                 "No initramfs file found for version '{}'."
                 .format(self.kernel_release)
             )
             return None
 
-        elif file_ is None:
+        elif not files:
             self.logger.info("No initramfs file found.")
             return None
 
         else:
-            return Path(file_)
+            return [Path(file) for file in files]
 
     @custom_kernel_options.add
     @Argument("--fdtdir", nargs=1)
     def fdtdir(self, dir_=None):
         """Directory to search device-tree binaries for the board"""
         if dir_ is None and self.kernel_version is not None:
             if self.kernel == self.kernel_version.kernel:
@@ -261,15 +285,15 @@
 
         if self.board.image_format == "zimage" and len(files) != 0:
             raise ValueError(
                 "Image format '{}' doesn't support dtb files."
                 .format(self.board.image_format)
             )
 
-        return files
+        return sorted(files, key=lambda f: f.name)
 
     @options.add
     @Argument("--description", nargs=1)
     def description(self, desc=None):
         """Human-readable description for the image"""
         if desc is None and self.kernel_version is not None:
             desc = self.kernel_version.description
@@ -340,14 +364,21 @@
             if lhs.lower() != "root":
                 continue
 
             if rhs == self.root:
                 append_root = False
                 continue
 
+            if self.root is None:
+                self.logger.warning(
+                    "Kernel cmdline has a root '{}', keeping it."
+                    .format(rhs)
+                )
+                continue
+
             self.logger.warning(
                 "Kernel cmdline has a different root '{}', removing it."
                 .format(rhs)
             )
             cmdline.remove(c)
 
         if append_root:
@@ -411,15 +442,18 @@
             if "SOURCE_DATE_EPOCH" in os.environ:
                 seconds = os.environ["SOURCE_DATE_EPOCH"]
 
         # Initramfs date is bound to be later than vmlinuz date, so
         # prefer that if possible.
         if seconds is None:
             if self.initrd is not None:
-                seconds = int(self.initrd.stat().st_mtime)
+                seconds = max(
+                    int(initrd.stat().st_mtime)
+                    for initrd in self.initrd
+                )
             else:
                 seconds = int(self.kernel.stat().st_mtime)
 
         if seconds is None:
             self.logger.error(
                 "Couldn't determine a timestamp from initramfs "
                 "nor vmlinuz."
@@ -457,30 +491,38 @@
 
         # Try to keep output reproducible.
         if self.timestamp is not None:
             os.environ["SOURCE_DATE_EPOCH"] = str(self.timestamp)
 
         # Error early if initramfs is absolutely too big to fit
         initrd_size = (
-            self.initrd.stat().st_size
+            sum(initrd.stat().st_size for initrd in self.initrd)
             if self.initrd is not None
             else 0
         )
         if initrd_size >= self.board.image_max_size:
             self.logger.error(
                 "Initramfs alone is larger than the maximum image size."
             )
             raise InitramfsSizeTooBigError()
 
+        # The earliest boards apparently have an off-by-one error while
+        # loading the chosen dtb, adding each file twice solves it.
+        dtbs = (
+            self.dtbs
+            if not self.board.loads_dtb_off_by_one else
+            [dtb for dtb in self.dtbs for _ in (0, 1)]
+        )
+
         # Skip compress="none" if inputs wouldn't fit max image size
         compress_list = self.compress
         inputs_size = sum([
             self.kernel.stat().st_size,
             initrd_size,
-            *(dtb.stat().st_size for dtb in self.dtbs),
+            *(dtb.stat().st_size for dtb in dtbs),
         ])
 
         if inputs_size > self.board.image_max_size and "none" in compress_list:
             self.logger.info(
                 "Inputs are too big, skipping uncompressed build."
             )
             compress_list.remove("none")
@@ -499,26 +541,29 @@
 
             if self.board.fit_ramdisk_load_address is not None:
                 image_format_opts["ramdisk_load_address"] = (
                     self.board.fit_ramdisk_load_address
                 )
 
         elif self.board.image_format == "zimage":
-            image_format_opts["pad_vmlinuz"] = not self.board.loads_zimage_ramdisk
+            if not self.board.loads_zimage_ramdisk:
+                hack = self.zimage_initramfs_hack
+                image_format_opts["pad_vmlinuz"] = (hack == "pad-vmlinuz")
+                image_format_opts["set_init_size"] = (hack == "set-init-size")
 
         for compress in compress_list:
             self.logger.info("Trying with compression '{}'.".format(compress))
             tmpdir = self.tmpdir / "mkdepthcharge-{}".format(compress)
 
             try:
                 mkdepthcharge(
                     arch=self.board.arch,
                     cmdline=self.kernel_cmdline,
                     compress=compress,
-                    dtbs=self.dtbs,
+                    dtbs=dtbs,
                     **image_format_opts,
                     kernel_start=self.board.image_start_address,
                     initramfs=self.initrd,
                     keyblock=self.vboot_keyblock,
                     output=outtmp,
                     signprivate=self.vboot_private_key,
                     signpubkey=self.vboot_public_key,
@@ -545,15 +590,21 @@
             # check if reducing the initramfs would make things fit.
             if outtmp.stat().st_size - initrd_size < self.board.image_max_size:
                 raise InitramfsSizeTooBigError()
             else:
                 raise SizeTooBigError()
 
         self.logger.info("Copying newly built image to output.")
-        copy(outtmp, self.output)
+        try:
+            copy(outtmp, self.output)
+        except PermissionError as err:
+            raise PermissionError(
+                "Couldn't copy to '{}', permission denied."
+                .format(self.output)
+            )
 
         self.logger.warning(
             "Built depthcharge image for kernel version '{}'."
             .format(self.kernel_release or "(unknown)")
         )
         return self.output
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_check.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl check subcommand
+# Copyright (C) 2020-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 
 from pathlib import Path
 
 from depthcharge_tools import __version__
@@ -114,14 +119,27 @@
         if board is None:
             raise ValueError(
                 "Cannot check depthcharge images when no board is specified.",
             )
 
         return board
 
+    @depthchargectl.zimage_initramfs_hack.copy()
+    def zimage_initramfs_hack(self, hack=None):
+        hack = super().zimage_initramfs_hack
+
+        if hack not in (None, "set-init-size", "pad-vmlinuz"):
+            raise ValueError(
+                "Unknown zimage initramfs support hack '{}'."
+                .format(hack)
+            )
+
+        return hack
+
+
     def __call__(self):
         image = self.image
 
         self.logger.warning(
             "Verifying depthcharge image for board '{}' ('{}')."
             .format(self.board.name, self.board.codename)
         )
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_config.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl config subcommand
+# Copyright (C) 2021-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 
 from depthcharge_tools import __version__
 from depthcharge_tools.utils.argparse import (
     Command,
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_list.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl list subcommand
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 import subprocess
 
 from depthcharge_tools import __version__
 from depthcharge_tools.utils.argparse import (
@@ -117,15 +122,18 @@
     def disks(self, *disks):
         """Disks to check for ChromeOS kernel partitions."""
 
         if self.all_disks:
             self.logger.info("Searching all disks.")
             disks = self.diskinfo.roots()
         elif disks:
-            self.logger.info("Searching real disks for {}.".format(disks))
+            self.logger.info(
+                "Searching real disks for {}."
+                .format(", ".join(str(d) for d in disks))
+            )
             images = []
             for d in disks:
                 if self.diskinfo.evaluate(d) is None:
                     try:
                         images.append(Disk(d))
                     except ValueError as err:
                         self.logger.warning(
@@ -142,15 +150,18 @@
             boot = (
                 self.diskinfo.by_mountpoint("/boot", fstab_only=True)
                 or self.diskinfo.by_mountpoint(self.boot_mountpoint)
             )
             disks = self.diskinfo.roots(root, boot)
 
         if disks:
-            self.logger.info("Using disks: {}.".format(disks))
+            self.logger.info(
+                "Using disks: {}."
+                .format(", ".join(str(d) for d in disks))
+            )
         else:
             raise ValueError("Could not find any matching disks.")
 
         return disks
 
     @Group
     def options(self):
@@ -246,15 +257,15 @@
                 columns=self.output,
             )
 
         if error_disks:
             return CommandExit(
                 message=(
                     "Couldn't get partitions for disks {}."
-                    .format(error_disks)
+                    .format(", ".join(str(d) for d in error_disks))
                 ),
                 output=output,
                 returncode=1,
             )
 
         return output
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_remove.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl remove subcommand
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 import subprocess
 
 from pathlib import Path
 
@@ -118,14 +123,16 @@
 
         # When called with --vblockonly vbutil_kernel creates a file of
         # size 64KiB == 0x10000.
         image_vblock = image.read_bytes()[:0x10000]
 
         partitions = depthchargectl.list(
             root=self.root,
+            root_mountpoint=self.root_mountpoint,
+            boot_mountpoint=self.boot_mountpoint,
             config=self.config,
             board=self.board,
             tmpdir=self.tmpdir / "list",
             images_dir=self.images_dir,
             vboot_keyblock=self.vboot_keyblock,
             vboot_public_key=self.vboot_public_key,
             vboot_private_key=self.vboot_private_key,
@@ -180,14 +187,16 @@
         for part in badparts:
             self.logger.info("Deactivating '{}'.".format(part))
             try:
                 depthchargectl.bless(
                     partition=part,
                     bad=True,
                     root=self.root,
+                    root_mountpoint=self.root_mountpoint,
+                    boot_mountpoint=self.boot_mountpoint,
                     config=self.config,
                     board=self.board,
                     tmpdir=self.tmpdir / "bless",
                     images_dir=self.images_dir,
                     vboot_keyblock=self.vboot_keyblock,
                     vboot_public_key=self.vboot_public_key,
                     vboot_private_key=self.vboot_private_key,
@@ -222,21 +231,21 @@
 
         output = badparts or None
 
         error_msg = []
         if error_disks:
             error_msg.append(
                 "Couldn't disable partitions for disks {}."
-                .format(error_disks)
+                .format(", ".join(str(d) for d in error_disks))
             )
 
         if error_parts:
             error_msg.append(
                 "Couldn't disable partitions {}."
-                .format(error_parts)
+                .format(", ".join(str(d) for d in error_parts))
             )
 
         if error_msg:
             return CommandExit(
                 message="\n".join(error_msg),
                 output=done_parts,
                 returncode=1,
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_target.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_target.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl target subcommand
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 import subprocess
 import sys
 import types
 
@@ -208,14 +213,16 @@
         # If no disks or partitions were given, search bootable disks.
         # Search all disks if explicitly asked.
         if disks or not partitions or self.all_disks:
             partitions += depthchargectl.list(
                 disks=disks,
                 all_disks=self.all_disks,
                 root=self.root,
+                root_mountpoint=self.root_mountpoint,
+                boot_mountpoint=self.boot_mountpoint,
                 config=self.config,
                 board=self.board,
                 tmpdir=self.tmpdir / "list",
                 images_dir=self.images_dir,
                 vboot_keyblock=self.vboot_keyblock,
                 vboot_public_key=self.vboot_public_key,
                 vboot_private_key=self.vboot_private_key,
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/depthchargectl/_write.py` & `depthcharge-tools-0.6.2/depthcharge_tools/depthchargectl/_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl write subcommand
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 import os
 import subprocess
 
 from pathlib import Path
@@ -191,14 +196,16 @@
 
         else:
             # No image given, try creating one.
             try:
                 image = depthchargectl.build_(
                     kernel_version=self.kernel_version,
                     root=self.root,
+                    root_mountpoint=self.root_mountpoint,
+                    boot_mountpoint=self.boot_mountpoint,
                     config=self.config,
                     board=self.board,
                     tmpdir=self.tmpdir / "build",
                     images_dir=self.images_dir,
                     vboot_keyblock=self.vboot_keyblock,
                     vboot_public_key=self.vboot_public_key,
                     vboot_private_key=self.vboot_private_key,
@@ -216,14 +223,16 @@
         self.logger.info("Searching disks for a target partition.")
         try:
             target = depthchargectl.target(
                 disks=[self.target] if self.target else [],
                 min_size=image.stat().st_size,
                 allow_current=self.allow_current,
                 root=self.root,
+                root_mountpoint=self.root_mountpoint,
+                boot_mountpoint=self.boot_mountpoint,
                 config=self.config,
                 board=self.board,
                 tmpdir=self.tmpdir / "target",
                 images_dir=self.images_dir,
                 vboot_keyblock=self.vboot_keyblock,
                 vboot_public_key=self.vboot_public_key,
                 vboot_private_key=self.vboot_private_key,
@@ -266,14 +275,16 @@
                 .format(target)
             )
             try:
                 depthchargectl.bless(
                     partition=target,
                     oneshot=True,
                     root=self.root,
+                    root_mountpoint=self.root_mountpoint,
+                    boot_mountpoint=self.boot_mountpoint,
                     config=self.config,
                     board=self.board,
                     tmpdir=self.tmpdir / "bless",
                     images_dir=self.images_dir,
                     vboot_keyblock=self.vboot_keyblock,
                     vboot_public_key=self.vboot_public_key,
                     vboot_private_key=self.vboot_private_key,
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/mkdepthcharge.py` & `depthcharge-tools-0.6.2/depthcharge_tools/mkdepthcharge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools mkdepthcharge program
+# Copyright (C) 2020-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import logging
 import os
 import platform
 import struct
 import subprocess
@@ -38,15 +43,15 @@
     fdtput,
 )
 
 
 class mkdepthcharge(
     Command,
     prog="mkdepthcharge",
-    usage="%(prog)s [options] -o FILE [--] [VMLINUZ] [INITRAMFS] [DTB ...]",
+    usage="%(prog)s [options] -o FILE [--] [VMLINUZ] [INITRAMFS ...] [DTB ...]",
     add_help=False,
 ):
     """Build boot images for the ChromeOS bootloader."""
 
     _logger = logging.getLogger(__name__)
 
     @property
@@ -200,35 +205,41 @@
             )
 
         vmlinuz = self._copy(files[0])
 
         return vmlinuz
 
     @input_files.add
-    @Argument("-i", "--initramfs", nargs=1)
-    def initramfs(self, initramfs=None):
-        """Ramdisk image"""
-        files = self.files["initramfs"]
+    @Argument("-i", "--initramfs", metavar="INITRAMFS", nargs="+")
+    def initramfs(self, *files):
+        """Ramdisk images"""
+        files = [
+            *(Path(f).resolve() for f in files if f is not None),
+            *self.files["initramfs"],
+        ]
 
-        if initramfs is not None:
-            initramfs = Path(initramfs).resolve()
+        for file in files:
             self.logger.info(
                 "Using file '{}' as an initramfs."
-                .format(initramfs)
+                .format(file)
             )
-            files = [initramfs, *files]
 
         if len(files) > 1:
-            raise ValueError(
-                "Can't build with multiple initramfs"
+            self.logger.info(
+                "Concatenating initramfs files as a single initramfs."
             )
+            initramfs = self._tempfile("merged-initramfs.img")
+            with initramfs.open('xb') as merge:
+                for file in files:
+                    merge.write(file.read_bytes())
 
-        if files:
+        elif len(files) == 1:
             initramfs = self._copy(files[0])
-        else:
+
+        elif not files:
             initramfs = None
 
         return initramfs
 
     @input_files.add
     @Argument("-b", "--dtbs", metavar="DTB", nargs="+")
     def dtbs(self, *dtbs):
@@ -377,14 +388,33 @@
         """Start of depthcharge kernel buffer in memory."""
         if addr is not None:
             return parse_bytesize(addr)
 
         if self.arch in Architecture.x86:
             return 0x100000
 
+    @options.add
+    @Argument(
+        "--no-pad-vmlinuz", pad=False,
+        help=argparse.SUPPRESS,
+    )
+    @Argument(
+        "--pad-vmlinuz", pad=True,
+        help="Pad vmlinuz for safe decompression.",
+    )
+    def pad_vmlinuz(self, pad=None):
+        """Pad vmlinuz for safe decompression."""
+        if pad is None:
+            pad = (
+                self.image_format == "fit"
+                and self.patch_dtbs
+            )
+
+        return bool(pad)
+
     @Group
     def fit_options(self):
         """FIT image options"""
 
     @fit_options.add
     @Argument("-C", "--compress", nargs=1)
     def compress(self, type_=None):
@@ -449,30 +479,30 @@
 
     @Group
     def zimage_options(self):
         """zImage format options"""
 
     @zimage_options.add
     @Argument(
-        "--no-pad-vmlinuz", pad=False,
-        help="Don't pad the vmlinuz file for safe decompression",
+        "--no-set-init-size", init_size=False,
+        help="Don't set init_size boot param.",
     )
     @Argument(
-        "--pad-vmlinuz", pad=True,
+        "--set-init-size", init_size=True,
         help=argparse.SUPPRESS,
     )
-    def pad_vmlinuz(self, pad=None):
-        """Pad vmlinuz for safe decompression"""
-        if pad is None:
+    def set_init_size(self, init_size=None):
+        """Set init_size boot param for safe decompression."""
+        if init_size is None:
             return (
                 self.image_format == "zimage"
                 and self.initramfs is not None
             )
 
-        return bool(pad)
+        return bool(init_size)
 
     @Group
     def vboot_options(self):
         """Depthcharge image options"""
 
         keydirs = []
         if self.keydir is not None:
@@ -675,14 +705,32 @@
 
         # vbutil_kernel --bootloader argument is mandatory, but it's
         # unused in depthcharge except as a multiboot ramdisk. Prepare
         # this empty file as its replacement where necessary.
         empty = self._tempfile("empty.bin")
         empty.write_bytes(bytes(512))
 
+        # The kernel decompression overwrites parts of the buffer we
+        # control while decompressing itself. We need to make sure we
+        # don't place initramfs in that range. For that, we need to know
+        # how offsets in file correspond to addresses in memory.
+
+        def addr_to_offs(addr, load_addr=self.kernel_start):
+            return addr - load_addr + 0x10000
+
+        def offs_to_addr(offs, load_addr=self.kernel_start):
+            return offs + load_addr - 0x10000
+
+        def align_up(size, align=0x1000):
+            return ((size + align - 1) // align) * align
+
+        # Size for a small padding, sometimes necessary in some
+        # places for unknown reasons, added and set empirically.
+        small_pad = 0x40000
+
         if self.image_format == "fit":
             fit_image = self._tempfile("depthcharge.fit")
 
             initramfs_args = []
             if initramfs is not None:
                 initramfs_args += ["-i", initramfs]
 
@@ -696,14 +744,82 @@
                     node = "/images/{}".format(subimage)
                     try:
                         if fdtget.get(fit_image, node, "type") == subimage_type:
                             return node
                     except:
                         continue
 
+            # On later 32-bit ARM Chromebooks, the KERNEL_START address
+            # can be very close to the where kernel decompresses itself
+            # that the process overwrites the initramfs. The device-tree
+            # is luckily copied away before then. We need to add some
+            # vmlinuz padding to prevent this.
+            if initramfs is not None and self.pad_vmlinuz:
+
+                # We need the decompressed kernel size, not easy to get.
+                # Try to find the compressed vmlinux inside vmlinuz,
+                # then try to decompress it.
+                data = vmlinuz.read_bytes()
+                vmlinuz_size = len(data)
+                decomp_size = -1
+
+                for fmt, magic in {
+                    "gzip":  b'\x1f\x8b\x08',
+                    "xz":    b'\xfd7zXZ\x00',
+                    "zstd":  b'(\xb5/\xfd',
+                    "lzma":  b'\x5d\x00\x00\x00',
+                    "lz4":   b'\02!L\x18',
+                    "bzip2": b'BZh',
+                    "lzop":  b'\x89\x4c\x5a',
+                }.items():
+                    offs = data.find(magic)
+                    while 0 < offs < vmlinuz_size:
+                        decomp = decompress(data[offs:], partial=True)
+                        if decomp:
+                            self.logger.info(
+                                "Found {} at {:#x} in vmlinuz, with size {:#x}."
+                                .format(fmt, offs, len(decomp))
+                            )
+                            decomp_size = max(decomp_size, len(decomp))
+                        offs = data.find(magic, offs + 1)
+
+                if decomp_size == -1:
+                    raise ValueError(
+                        "Couldn't find decompressed kernel inside vmlinuz."
+                    )
+
+                self.logger.info(
+                    "Vmlinuz size is {:#x}, {:#x} decompressed."
+                    .format(vmlinuz_size, decomp_size)
+                )
+
+                # Decompression starts at start of physical memory,
+                # calculated per AUTO_ZRELADDR. But first kernel copies
+                # itself after where the decompressed copy would end.
+                decomp_addr = self.kernel_start & 0xf8000000
+                safe_initrd_start = (
+                    decomp_addr + decomp_size + vmlinuz_size + small_pad
+                )
+                initrd_start = (
+                    self.kernel_start + vmlinuz_size
+                    + sum(dtb.stat().st_size for dtb in self.dtbs)
+                )
+
+                if initrd_start < safe_initrd_start:
+                    pad_to = align_up(
+                        vmlinuz_size
+                        + (safe_initrd_start - initrd_start)
+                    )
+                    self.logger.info(
+                        "Padding vmlinuz to {:#x}."
+                        .format(pad_to)
+                    )
+                    with vmlinuz.open("r+b") as f, mmap(f.fileno(), 0) as data:
+                        data.resize(pad_to)
+
             # The later 32-bit ARM Chromebooks use Depthcharge, but
             # their stock versions don't have the code to support FIT
             # ramdisks. But since we know the fixed KERNEL_START we can
             # deduce where the initramfs will be, and inject its address
             # into the DTBs the way Linux expects bootloaders to do.
             if initramfs is not None and self.patch_dtbs:
 
@@ -834,52 +950,44 @@
                 "--keyblock", self.keyblock,
                 "--signprivate", self.signprivate,
                 "--pack", self.output,
             )
             self.logger.info(proc.stdout)
 
         elif self.image_format == "zimage":
-            # The bzImage overwrites parts of the buffer we control
-            # while decompressing itself. We need to make sure we don't
-            # place initramfs in that range. For that, we need to know
-            # how offsets in file correspond to addresses in memory.
-
-            def addr_to_offs(addr, load_addr=self.kernel_start):
-                return addr - load_addr + 0x10000
-
-            def offs_to_addr(offs, load_addr=self.kernel_start):
-                return offs + load_addr - 0x10000
-
-            def align_up(size, align=0x1000):
-                return ((size + align - 1) // align) * align
-
             # bzImage header has the address the kernel will decompress
             # to, and the amount of memory it needs there to work.
             # See Documentation/x86/boot.rst in Linux tree for offsets.
             with vmlinuz.open("r+b") as f, mmap(f.fileno(), 0) as data:
                 if data[0x202:0x206] != b"HdrS":
                     raise ValueError(
                         "Vmlinuz file is not a Linux kernel bzImage."
                     )
 
                 pref_address, init_size = struct.unpack(
                     "<QI", data[0x258:0x264]
                 )
-                pad_to = align_up(addr_to_offs(pref_address + init_size))
+                self.logger.info(
+                    "Vmlinuz pref_address is {:#x}, with init_size {:#x}."
+                    .format(pref_address, init_size)
+                )
+
+                # Initramfs gets corrupted if it's too close to vmlinuz
+                pad_to = align_up(data.size()) + small_pad
 
-                # Custom kernels may have PHYSICAL_START high enough
-                # that we can squeeze the initramfs between vmlinuz and
-                # the preferred_address. Very unlikely, but saves space.
-                # Didn't work unless I padded the vmlinuz by 0x15000.
-                low_pad = 0x18000
-                low_usable = pref_address - align_up(data.size()) - low_pad
-                if initramfs.stat().st_size < low_usable:
-                    pad_to = align_up(data.size()) + low_pad
+                # KASLR takes care to avoid overwriting initramfs in
+                # self-decompression, but if that's disabled we need to
+                # put the initramfs outside the decompression buffer.
+                # But if the kernel and initramfs are small enough, they
+                # might fit before pref_address, where we can skip that.
+                low_usable = pref_address - align_up(data.size()) - small_pad
+                if self.pad_vmlinuz and initramfs.stat().st_size > low_usable:
+                    pad_to = align_up(addr_to_offs(pref_address + init_size))
 
-                if self.pad_vmlinuz and pad_to > data.size():
+                if pad_to > data.size():
                     self.logger.info(
                         "Padding vmlinuz to size {:#x}"
                         .format(pad_to)
                     )
                     data.resize(pad_to)
 
             # vbutil_kernel picks apart the vmlinuz in ways I don't
@@ -941,14 +1049,33 @@
 
                 # These get passed to the kernel unmodified by depthcharge.
                 # "initrdmem=addr,size" in the cmdline would work, but
                 # this looks like how bootloaders are supposed to do it.
                 data[p+0x218:p+0x21c] = struct.pack("<I", initramfs_addr)
                 data[p+0x21c:p+0x220] = struct.pack("<I", initramfs_size)
 
+                # Kernel self-decompression first copies vmlinuz to avoid
+                # overwriting itself, ending at pref_address + init_size
+                # or so. Increasing init_size in the boot params makes
+                # it avoid overwriting our initramfs. Also needs some
+                # small padding for unknown reasons.
+                if self.set_init_size:
+                    safe_copy_end = align_up(
+                        initramfs_addr + initramfs_size
+                        + small_pad
+                        + vmlinuz.stat().st_size
+                    )
+                    if pref_address + init_size < safe_copy_end:
+                        init_size = safe_copy_end - pref_address
+                        self.logger.info(
+                            "Setting init_size = {:#x}."
+                            .format(init_size)
+                        )
+                        data[p+0x260:p+0x264] = struct.pack("<I", init_size)
+
             self.logger.info("Re-signing edited temporary image.")
             proc = vbutil_kernel(
                 "--keyblock", self.keyblock,
                 "--signprivate", self.signprivate,
                 "--oldblob", temp_img,
                 "--repack", self.output,
             )
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/utils/argparse.py` & `depthcharge-tools-0.6.2/depthcharge_tools/utils/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools argparse utilities
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import argparse
 import copy
 import contextlib
 import functools
 import inspect
 import logging
@@ -850,14 +855,17 @@
                 retval = inst(*args, **kwargs)
         else:
             retval = instance(*args, **kwargs)
 
         if isinstance(retval, CommandExit):
             if raise_exit:
                 raise retval
+            elif retval.returncode != 0 and hasattr(instance, "_logger"):
+                instance._logger.warning(retval.message)
+                retval = retval.output
             else:
                 retval = retval.output
 
         return retval
 
     def __generator_call(cls, *args, **kwargs):
         instance = super().__call__()
@@ -868,14 +876,17 @@
                 retval = yield from inst(*args, **kwargs)
         else:
             retval = yield from instance(*args, **kwargs)
 
         if isinstance(retval, CommandExit):
             if raise_exit:
                 raise retval
+            elif retval.returncode != 0 and hasattr(instance, "_logger"):
+                instance._logger.warning(retval.message)
+                retval = retval.output
             else:
                 retval = retval.output
 
         return retval
 
     def main(cls, *argv):
         if len(argv) == 0:
@@ -900,36 +911,42 @@
 
         def log_error(err):
             is_debug_level = logger.isEnabledFor(logging.DEBUG)
             if not is_debug_level and err.__cause__ is not None:
                 log_error(err.__cause__)
             logger.error(err, exc_info=is_debug_level)
 
-        try:
-            output = command(__raise_CommandExit=True, **kwargs)
-
+        def print_out(output):
             if inspect.isgenerator(output):
                 try:
                     while True:
                         print(next(output))
                 except StopIteration as err:
                     output = err.value
 
-            if output is not None:
+            elif isinstance(output, list):
+                print(*output, sep="\n")
+
+            elif isinstance(output, tuple):
+                print(*output, sep="\n")
+
+            elif output is not None:
                 print(output)
 
+        try:
+            output = command(__raise_CommandExit=True, **kwargs)
+            print_out(output)
+
         except CommandExit as exit:
             if exit.returncode != 0:
                 log_error(exit)
             else:
                 logger.warning(exit)
 
-            if exit.output is not None:
-                print(exit.output)
-
+            print_out(exit.output)
             sys.exit(exit.returncode)
 
         except Exception as err:
             log_error(err)
             sys.exit(1)
 
     def items(cls):
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/utils/collections.py` & `depthcharge-tools-0.6.2/depthcharge_tools/utils/collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools collections utilities
+# Copyright (C) 2021-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import collections
 
 # Inheritance for config sections
 class ConfigDict(collections.OrderedDict):
     def __getitem__(self, key):
         super_ = super()
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/utils/os.py` & `depthcharge-tools-0.6.2/depthcharge_tools/utils/os.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools os utilities
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import collections
 import re
 import shlex
 
 from pathlib import Path
 
@@ -10,15 +15,15 @@
     DirectedGraph,
 )
 from depthcharge_tools.utils.pathlib import (
     iterdir,
     read_lines,
 )
 from depthcharge_tools.utils.platform import (
-    kernel_cmdline,
+    proc_cmdline,
 )
 from depthcharge_tools.utils.subprocess import (
     cgpt,
 )
 
 
 class Disks(DirectedGraph):
@@ -293,15 +298,15 @@
     def get_uuid(self, device):
         return self._get_dev_disk_info(device, "uuid")
 
     def get_partuuid(self, device):
         return self._get_dev_disk_info(device, "partuuid")
 
     def by_kern_guid(self):
-        for arg in kernel_cmdline():
+        for arg in proc_cmdline():
             lhs, _, rhs = arg.partition("=")
             if lhs == "kern_guid":
                 return self.by_partuuid(rhs)
 
     def add_edge(self, node, child):
         node = self.evaluate(node)
         child = self.evaluate(child)
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/utils/platform.py` & `depthcharge-tools-0.6.2/depthcharge_tools/utils/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools platform utilities
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import collections
 import glob
 import platform
 import re
 import shlex
 
@@ -75,15 +80,32 @@
         for line in os_release_f.read_text().splitlines():
             lhs, _, rhs = line.partition("=")
             os_release[lhs] = rhs.strip('\'"')
 
     return os_release
 
 
-def kernel_cmdline():
+def kernel_cmdline(root=None):
+    cmdline = ""
+
+    if root is None:
+        root = "/"
+    root = Path(root).resolve()
+
+    cmdline_f = root / "etc" / "kernel" / "cmdline"
+    if not cmdline_f.exists():
+        cmdline_f = root / "usr" / "lib" / "kernel" / "cmdline"
+
+    if cmdline_f.exists():
+        cmdline = cmdline_f.read_text().rstrip("\n")
+
+    return shlex.split(cmdline)
+
+
+def proc_cmdline():
     cmdline = ""
 
     cmdline_f = Path("/proc/cmdline")
     if cmdline_f.exists():
         cmdline = cmdline_f.read_text().rstrip("\n")
 
     return shlex.split(cmdline)
@@ -91,15 +113,15 @@
 
 def is_cros_boot():
     dt_cros_firmware = Path("/proc/device-tree/firmware/chromeos")
     if dt_cros_firmware.is_dir():
         return True
 
     # Chrome OS firmware injects this into the kernel cmdline.
-    if "cros_secure" in kernel_cmdline():
+    if "cros_secure" in proc_cmdline():
         return True
 
     return False
 
 
 def is_cros_libreboot():
     fwid = cros_fwid()
@@ -143,14 +165,15 @@
     if len(keydirs) == 0 or system:
         if root is None:
             root = "/"
         root = Path(root).resolve()
 
         keydirs = (
             *keydirs,
+            root / "etc" / "depthcharge-tools",
             root / "usr" / "share" / "vboot" / "devkeys",
             root / "usr" / "local" / "share" / "vboot" / "devkeys",
         )
 
     for keydir in keydirs:
         keydir = Path(keydir)
         if not keydir.is_dir():
@@ -169,14 +192,45 @@
 
         if keyblock or signprivate or signpubkey:
             return keydir, keyblock, signprivate, signpubkey
 
     return None, None, None, None
 
 
+def cpu_microcode(boot=None):
+    microcode = []
+
+    for f in (
+        *boot.glob("amd-ucode.img"),
+        *boot.glob("amd-uc.img"),
+    ):
+        if f.is_file():
+            microcode.append(f)
+            break
+
+    for f in (
+        *boot.glob("intel-ucode.img"),
+        *boot.glob("intel-uc.img"),
+    ):
+        if f.is_file():
+            microcode.append(f)
+            break
+
+    if not microcode:
+        for f in (
+            *boot.glob("early_ucode.cpio"),
+            *boot.glob("microcode.cpio"),
+        ):
+            if f.is_file():
+                microcode.append(f)
+                break
+
+    return microcode
+
+
 def installed_kernels(root=None, boot=None):
     kernels = {}
     initrds = {}
     fdtdirs = {}
 
     if root is None:
         root = "/"
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/utils/string.py` & `depthcharge-tools-0.6.2/depthcharge_tools/utils/string.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools string utilities
+# Copyright (C) 2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import ast
 import re
 
 def bytesize_suffixes():
     def long_forms(x):
         formats = ("{}", "{}byte", "{} byte", "{}bytes", "{} bytes")
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools/utils/subprocess.py` & `depthcharge-tools-0.6.2/depthcharge_tools/utils/subprocess.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #! /usr/bin/env python3
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools subprocess utilities
+# Copyright (C) 2020-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 import contextlib
 import logging
 import re
 import subprocess
 import shlex
 
@@ -49,15 +54,31 @@
             if isinstance(stderr, str):
                 stderr = Path(stderr)
             if isinstance(stderr, Path):
                 kwargs["stderr"] = ctx.enter_context(stderr.open("x"))
             if stderr is None:
                 kwargs["stderr"] = subprocess.PIPE
 
-            return subprocess.run(args, **kwargs)
+            try:
+                return subprocess.run(args, **kwargs)
+            except subprocess.CalledProcessError as err:
+                our_err = self._parse_subprocess_error(err)
+                if our_err is None:
+                    return subprocess.CompletedProcess(
+                        args=err.cmd,
+                        returncode=err.returncode,
+                        stdout=err.stdout,
+                        stderr=err.stderr,
+                    )
+                if our_err is not err:
+                    raise our_err
+                raise
+
+    def _parse_subprocess_error(self, err):
+        return err
 
 
 class GzipRunner(ProcessRunner):
     def __init__(self):
         super().__init__("gzip", encoding=None)
 
     def compress(self, src, dest=None):
@@ -253,14 +274,33 @@
         # https://bugs.chromium.org/p/chromium/issues/detail?id=463414
         mid = len(lines) // 2
         if lines[:mid] == lines[mid:]:
             proc.stdout = "\n".join(lines[:mid])
 
         return proc
 
+    def _parse_subprocess_error(self, err):
+        # Exits with nonzero status if it finds no partitions of
+        # given type even if the disk has a valid partition table
+        if not err.stderr:
+            return None
+
+        m = re.fullmatch(
+            "ERROR: Can't open (.*): Permission denied\n",
+            err.stderr,
+        )
+        if m:
+            return PermissionError(
+                "Couldn't open '{}', permission denied."
+                .format(m.groups()[0])
+            )
+
+        return err
+
+
     def get_raw_attribute(self, disk, partno):
         proc = self("show", "-A", "-i", str(partno), str(disk))
         attribute = int(proc.stdout, 16)
         return attribute
 
     def set_raw_attribute(self, disk, partno, attribute):
         self("add", "-A", hex(attribute), "-i", str(partno), str(disk))
@@ -305,23 +345,15 @@
         if type is None:
             # cgpt find needs at least one of -t, -u, -l
             proc = self("show", "-q", "-n", disk)
             lines = proc.stdout.splitlines()
             partnos = [int(shlex.split(line)[2]) for line in lines]
 
         else:
-            # Exits with nonzero status if it finds no partitions of
-            # given type even if the disk has a valid partition table
-            try:
-                proc = self("find", "-n", "-t", type, disk)
-            except subprocess.CalledProcessError as err:
-                if err.stderr:
-                    raise
-                return []
-
+            proc = self("find", "-n", "-t", type, disk)
             partnos = [int(n) for n in proc.stdout.splitlines()]
 
         return partnos
 
     def prioritize(self, disk, partno):
         self("prioritize", "-i", str(partno), str(disk))
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools.egg-info/PKG-INFO` & `depthcharge-tools-0.6.2/depthcharge_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-tools
-Version: 0.6.1
+Version: 0.6.2
 Summary: Tools to manage the Chrome OS bootloader
 Home-page: https://github.com/alpernebbi/depthcharge-tools
 Author: Alper Nebi Yasak
 Author-email: alpernebiyasak@gmail.com
 License: GPL2+
 Keywords: ChromeOS ChromiumOS depthcharge vboot vbutil_kernel
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Boot
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+License-File: COPYRIGHT
+
+.. SPDX-License-Identifier: GPL-2.0-or-later
+
+.. depthcharge-tools README file
+.. Copyright (C) 2019-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+.. See COPYRIGHT and LICENSE files for full copyright information.
 
 =================
 Depthcharge-Tools
 =================
 This project is a collection of tools that ease and automate interacting
 with depthcharge_, the Chrome OS bootloader.
 
@@ -30,28 +37,28 @@
 `the format depthcharge expects`_. These tools are about the latter.
 
 Right now these are developed on and tested with only a few boards,
 but everything will attempt to work on other boards based on my best
 guesses.
 
 .. _depthcharge: https://chromium.googlesource.com/chromiumos/platform/depthcharge
-.. _the format depthcharge expects: https://www.chromium.org/chromium-os/chromiumos-design-docs/disk-format#TOC-Google-Chrome-OS-devices
+.. _the format depthcharge expects: https://chromium.googlesource.com/chromiumos/docs/+/HEAD/disk_format.md#Google-ChromeOS-devices
 .. _Debian: https://www.debian.org/
 
 
 mkdepthcharge
 =============
 The mkdepthcharge_ tool is intended to wrap mkimage_ and vbutil_kernel_
 to provide reasonable defaults to them, hide their idiosyncrasies and
 automate creating a depthcharge-bootable partition image appropriate for
 the running architecture. An example invocation on a Samsung Chromebook
 Plus (v1, arm64) could be::
 
     $ mkdepthcharge -o depthcharge.img --compress lzma \
-        --cmdline "console=tty1 root=/dev/mmcblk0p2 rootwait" \
+        --cmdline "console=tty1 root=/dev/mmcblk0p2 rootwait" -- \
         /boot/vmlinuz.gz /boot/initrd.img rk3399-gru-kevin.dtb
 
 Here, mkdepthcharge would automatically extract and recompress the
 kernel, create a FIT image, put command line parameters into a file,
 create an empty bootloader, and provide defaults for vboot keys and
 other arguments while building the partition image.
 
@@ -100,24 +107,46 @@
 the ``mkdepthcharge.rst`` and ``depthchargectl.rst`` files to manual
 pages. However, this is not automated here and has to be done manually.
 
 This project (or at least ``depthchargectl``) is meant to be integrated
 into your operating system by its maintainers, and the best way to
 install it is through your OS' package manager whenever possible.
 
+
 Debian
 ------
-An unofficial Debian package is available in the releases_ page, with
-it's packaging source tracked in salsa_. After downloading, you can
-install with::
+An official `depthcharge-tools Debian package`_ is available upstream,
+since Debian 12 (bookworm). You can install it like any other package::
+
+    $ sudo apt install depthcharge-tools
+
+It includes the necessary system hooks and services to make and keep
+your Chromebook bootable, enabled by default. These however do not
+trigger on the depthcharge-tools installation, but on kernel and
+initramfs changes. To trigger these hooks manually, run::
+
+    $ sudo update-initramfs -u
+
+.. _depthcharge-tools Debian package: https://packages.debian.org/sid/depthcharge-tools
+
 
-    $ sudo apt install ./depthcharge-tools_*.deb
+Alpine Linux
+------------
+Thanks to the efforts in supporting `postmarketOS on ChromeOS Devices`_,
+there is an official `depthcharge-tools package for Alpine Linux`_. You
+should be able to install it as::
+
+    $ sudo apk add depthcharge-tools
+
+However, this doesn't include any system hooks or services to keep your
+Chromebook bootable.
+
+.. _postmarketOS on ChromeOS Devices: https://wiki.postmarketos.org/wiki/Chrome_OS_devices
+.. _depthcharge-tools package for Alpine Linux: https://pkgs.alpinelinux.org/package/edge/testing/x86/depthcharge-tools
 
-.. _releases: https://github.com/alpernebbi/depthcharge-tools/releases
-.. _salsa: https://salsa.debian.org/alpernebbi/depthcharge-tools
 
 Pip
 ---
 Python binary wheels are uploaded to PyPI_, and it should be possible to
 install the python package using `pip`. However, this does not install
 the manual pages, bash/zsh completions, systemd/init.d service files,
 and OS-specific kernel/initramfs hooks.
@@ -155,14 +184,15 @@
     vboot-public-key: The public key for (.vbpubk) verifying images
 
     [depthchargectl]
     board: Codename of a board to build and check images for
     ignore-initramfs: Do not include an initramfs in the image
     images-dir: Directory to store built images
     kernel-cmdline: Kernel commandline parameters to use
+    zimage-initramfs-hack = How to support initramfs on x86 boards
 
 For longer explanations check the manual pages of each command for
 options named the same as these.
 
 .. |CONFIG_FILE| replace:: ``/etc/depthcharge-tools/config``
 .. |CONFIGD_DIR| replace:: ``/etc/depthcharge-tools/config.d``
 .. _config.ini: https://github.com/alpernebbi/depthcharge-tools/blob/master/depthcharge_tools/config.ini
@@ -192,29 +222,38 @@
 
     $ depthchargectl list /dev/mmcblk0
     S  P  T  PATH
     1  2  0  /dev/mmcblk0p2
     1  1  0  /dev/mmcblk0p4
     0  0  15 /dev/mmcblk0p6
 
+Or you can add a similar invocation to the /usr/local/bin files, so that
+it's available to both normal users and root::
 
-Contributing
-============
-I only own two chromebooks, so I need your help to make it work with all
-others. Pull requests, bug reports, or even pointers in the right
-direction for existing issues are all welcome.
+    $ sudo tee /usr/local/bin/depthchargectl <<EOF
+    #!/bin/sh
+    export PYTHONDONTWRITEBYTECODE=1
+    export PYTHONPATH=/path/to/depthcharge-tools
+    exec python3 -m depthcharge_tools.depthchargectl "\$@"
+    EOF
+
+    $ sudo chmod +x /usr/local/bin/depthchargectl
 
 
 License
 =======
+Copyright (C) 2019-2023 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+
 This program is free software; you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation; either version 2 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <https://www.gnu.org/licenses/>
+
+See COPYRIGHT and LICENSE files for full copyright information.
```

### Comparing `depthcharge-tools-0.6.1/depthcharge_tools.egg-info/SOURCES.txt` & `depthcharge-tools-0.6.2/depthcharge_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 depthchargectl.rst
 mkdepthcharge.rst
 setup.py
 completions/_depthchargectl.bash
```

### Comparing `depthcharge-tools-0.6.1/depthchargectl.rst` & `depthcharge-tools-0.6.2/depthchargectl.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+.. SPDX-License-Identifier: GPL-2.0-or-later
+
+.. depthcharge-tools depthchargectl(1) manual page
+.. Copyright (C) 2019-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+.. See COPYRIGHT and LICENSE files for full copyright information.
+
 ==============
 depthchargectl
 ==============
 
 --------------------------------------------------
 Manage the ChromeOS bootloader and its boot images
 --------------------------------------------------
 
-:date: 2022-11-24
-:version: v0.6.1
+:date: 2023-06-30
+:version: v0.6.2
 :manual_section: 1
 :manual_group: depthcharge-tools
 
 .. |mkdepthcharge| replace:: *mkdepthcharge*\ (1)
 .. |cgpt| replace:: *cgpt*\ (1)
 .. |vbutil_kernel| replace:: *vbutil_kernel*\ (1)
 
+.. |CONFIG_DIR| replace:: **/etc/depthcharge-tools**
 .. |CONFIG_FILE| replace:: **/etc/depthcharge-tools/config**
 .. |CONFIGD_DIR| replace:: **/etc/depthcharge-tools/config.d**
 .. |IMAGES_DIR| replace:: **/boot/depthcharge**
-.. |VBOOT_KEYBLOCK| replace:: **/usr/share/vboot/kernel.keyblock**
-.. |VBOOT_PUBLIC_KEY| replace:: **/usr/share/vboot/kernel_subkey.vbpubk**
-.. |VBOOT_PRIVATE_KEY| replace:: **/usr/share/vboot/kernel_data_key.vbprivk**
-.. |KERNEL_CMDLINE| replace:: **"console=tty0 quiet splash"**
 .. |INITD_DIR| replace:: **/etc/init.d**
 .. |SYSTEMD_DIR| replace:: **/usr/lib/systemd/system**
+.. |USR_CMDLINE_FILE| replace:: **/usr/lib/kernel/cmdline**
+.. |ETC_CMDLINE_FILE| replace:: **/etc/kernel/cmdline**
+.. |PROC_CMDLINE_FILE| replace:: **/proc/cmdline**
+.. |VBOOT_DEVKEYS| replace:: **/usr/share/vboot/devkeys**
+.. |USR_KI_DIR| replace:: **/usr/lib/kernel/install.d**
+.. |ETC_KI_CONF| replace:: **/etc/kernel/install.conf**
 
 
 SYNOPSIS
 ========
 **depthchargectl** [options] *COMMAND* ...
 
 **depthchargectl bless** [options] [*PARTITION* | *DISK*]
@@ -93,21 +102,21 @@
 for the kernel are automatically tried as necessary, when the firmware
 supports them.
 
 depthchargectl config
 ---------------------
 Retrieves the configured value for a given configuration key, primarily
 for use in scripts that integrate **depthchargectl** with the system
-upgrade process.
+upgrade process. Can also query information about boards.
 
 depthchargectl check
 --------------------
 Checks if a file is a depthcharge image that can be booted on this
 board. **depthchargectl** also keeps track of restrictions on images
-for each board. For example, most ChromeOS board can boot images
+for each board. For example, earlier ChromeOS board can boot images
 up to a specific size, e.g. 32MiB. It checks if its input is in a format
 the ChromeOS bootloader expects and satisfies these restrictions.
 
 depthchargectl list
 -------------------
 Prints a table of ChromeOS kernel partitions and their bootloader
 specific GPT flags (i.e. Successful, Priority, Tries). By default, it
@@ -154,14 +163,21 @@
     Print program version and exit.
 
 --root ROOT
     Root device or mountpoint of the system to work on. If a mounted
     device is given, its mountpoint is used. Defaults to the currently
     booted system's root.
 
+--root-mountpoint DIR, --boot-mountpoint DIR
+    Root and boot mountpoints of the system to work on. If not given,
+    deduced from the **--root** argument. These are helpful because the
+    **--root** argument is overloaded by the **build** subcommand, which
+    adds it as a kernel command line argument, and it can be desirable
+    to avoid that while building an image for a chroot.
+
 --tmpdir DIR
     Directory to keep temporary files. Normally **depthchargectl**
     creates a temporary directory by itself and removes it when it
     quits. However, if a temporary directory is specified with this
     option any temporary files will be created under it and will not be
     deleted.
 
@@ -184,38 +200,47 @@
 
 --images-dir DIR
     Directory to store and look for built depthcharge images. By
     default, set to |IMAGES_DIR|.
 
 --vboot-keyblock KEYBLOCK
     The kernel keyblock file required to sign and verify images. By
-    default, set to |VBOOT_KEYBLOCK|.
+    default, **depthchargectl** searches for these keys in |CONFIG_DIR|
+    and |VBOOT_DEVKEYS| directories.
 
 --vboot-public-key SIGNPUBKEY
     The public key required to verify images, in .vbpubk format. By
-    default, set to |VBOOT_PUBLIC_KEY|.
+    default, **depthchargectl** searches for these keys in |CONFIG_DIR|
+    and |VBOOT_DEVKEYS| directories.
 
 --vboot-private-key SIGNPRIVATE
     The private key necessary to sign images, in .vbprivk format. By
-    default, set to |VBOOT_PRIVATE_KEY|.
+    default, **depthchargectl** searches for these keys in |CONFIG_DIR|
+    and |VBOOT_DEVKEYS| directories.
 
 --kernel-cmdline *CMD* [*CMD* ...]
-    Command-line parameters for the kernel. By default, set to
-    |KERNEL_CMDLINE|.  **depthchargectl** and |mkdepthcharge| append
-    some other values to this: an appropriate **root=**\ *ROOT*, the
-    **kern_guid=%U** parameter required for the **bless** subcommand,
-    **noinitrd** if **--ignore-initramfs** is given.
+    Command-line parameters for the kernel. By default, these are read
+    from |ETC_CMDLINE_FILE|, |USR_CMDLINE_FILE| or |PROC_CMDLINE_FILE|.
+    **depthchargectl** and |mkdepthcharge| may append some other values
+    to this: an appropriate **root=**\ *ROOT*, the **kern_guid=%U**
+    parameter required for the **bless** subcommand, **noinitrd** if
+    **--ignore-initramfs** is given.
 
 --ignore-initramfs
-    Do not include *initramfs* in the built images. For some boards,
-    **depthchargectl** cannot build an image that includes an initramfs
-    so it exits with an error if your OS kernel has a corresponding one.
-    If you know that your OS kernel can boot on this board without an
-    initramfs, you can specify this option to build an initramfs-less
-    image.
+    Do not include *initramfs* in the built images, ignore the initramfs
+    checks for the **root=**\ *ROOT* argument, and add **noinitrd** to
+    the kernel cmdline. If you know that your OS kernel can boot on this
+    board without an initramfs (perhaps because it has a built-in one),
+    you can specify this option to build an initramfs-less image.
+
+--zimage-initramfs-hack
+    Choose which initramfs support hack will be used for the zimage
+    format. Either **set-init-size** (the default), **pad-vmlinuz**
+    for kernels without **KASLR**, or **none** if depthcharge ever
+    gets native support for safely loading zimage initramfs.
 
 depthchargectl bless options
 ----------------------------
 --bad
     Set the specified partition as unbootable. This sets all three of
     the *Successful*, *Priority*, *Tries* flags to 0.
 
@@ -235,15 +260,15 @@
     Human-readable description for the image. By default, a string that
     describes your system with the specified kernel release name, like
     "Debian GNU/Linux, with Linux 5.10.0-6-arm64".
 
 --root ROOT
     Root device to add to kernel cmdline. By default, this is acquired
     from **/etc/fstab** or a filesystem UUID is derived from the mounted
-    root. If "none" is passed, no root parameter is added.
+    root. If **none** is passed, no root parameter is added.
 
 --compress *TYPE* [*TYPE* ...]
     Compression types to attempt. By default, all compression types that
     the board supports based on **depthchargectl** configuration are
     attempted from lowest to highest compression.
 
 --timestamp SECONDS
@@ -262,17 +287,18 @@
     Release name for the kernel to be used in image filename under the
     images-dir (unless **--output** is specified).
 
 --kernel FILE
     Kernel executable. Usually **/boot/vmlinuz-**\ *VERSION* by default,
     but depends on your OS.
 
---initramfs FILE
+--initramfs *FILE* [*FILE* ...]
     Ramdisk image. Usually **/boot/initrd.img-**\ *VERSION* by default,
-    but depends on your OS.
+    but depends on your OS. If **none** is passed, no initramfs is
+    added.
 
 --fdtdir DIR
     Directory to search device-tree binaries for the board. Usually
     **/boot/dtbs** or a directory like **/usr/lib/linux-image-**\
     *VERSION*, depends on your OS. *dtb* files in this dir are searched
     to find ones matching your board's device-tree compatible string set
     in configuration.
@@ -431,31 +457,49 @@
 
 7
     The *partition* is smaller than the **--min-size** argument.
 
 
 FILES
 =====
+|CONFIG_DIR|
+    Configuration directory. **depthchargectl** searches this directory
+    for configuration files and ChromiumOS verified boot keys.
+
 |CONFIG_FILE|
     System configuration file. The "Configuration options" explained
     above can be set here to have them as long-term defaults. It's also
     possible to modify board properties or add new boards here.
 
 |CONFIGD_DIR|/*\ **
     These files are considered appended to the **config** file.
 
-|SYSTEMD_DIR|/depthchargectl-bless.service
-    A systemd service that runs the **depthchargectl bless** on
-    successful boots.
+|ETC_CMDLINE_FILE|, |USR_CMDLINE_FILE|, |PROC_CMDLINE_FILE|
+    Files from which **depthchargectl** may deduce a default kernel
+    command line.
 
-|INITD_DIR|/depthchargectl-bless
+|SYSTEMD_DIR|\ **/depthchargectl-bless.service**
+    A systemd service that runs **depthchargectl bless** on successful
+    boots.
+
+|USR_KI_DIR|\ **/90-depthcharge-tools.install**
+    A systemd kernel-install plugin that can automatically manage your
+    system if **layout=depthcharge-tools** is set in |ETC_KI_CONF|.
+
+|INITD_DIR|\ **/depthchargectl-bless**
     An init service that runs **depthchargectl bless** on successful
     boots.
 
-|IMAGES_DIR|/*\ **.img
+|VBOOT_DEVKEYS|
+    A directory containing test keys which should have been installed by
+    |vbutil_kernel|. **depthchargectl** also searches this directory if
+    no verified boot keys are set in configuration or found in config
+    directories.
+
+|IMAGES_DIR|/*\ **\ **.img**
     The most recently built images for each kernel version.
 
 
 EXAMPLES
 ========
 **depthchargectl** **list** **-n** **-o** *PATH*
     Get a list of partitions **depthchargectl** will act on by default.
```

### Comparing `depthcharge-tools-0.6.1/init.d/depthchargectl-bless` & `depthcharge-tools-0.6.2/init.d/depthchargectl-bless`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/bin/sh
+# SPDX-License-Identifier: GPL-2.0-or-later
+
+# depthcharge-tools depthchargectl-bless sysvinit service
+# Copyright (C) 2020-2021 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
 
 ### BEGIN INIT INFO
 # Provides:          depthchargectl-bless
 # Required-Start:    $remote_fs
 # Required-Stop:
 # Default-Start:     2 3 4 5
 # Default-Stop:
```

### Comparing `depthcharge-tools-0.6.1/mkdepthcharge.rst` & `depthcharge-tools-0.6.2/mkdepthcharge.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+.. SPDX-License-Identifier: GPL-2.0-or-later
+
+.. depthcharge-tools mkdepthcharge(1) manual page
+.. Copyright (C) 2019-2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+.. See COPYRIGHT and LICENSE files for full copyright information.
+
 =============
 mkdepthcharge
 =============
 
 ---------------------------------------------
 Build boot images for the ChromeOS bootloader
 ---------------------------------------------
 
-:date: 2022-11-24
-:version: v0.6.1
+:date: 2023-06-30
+:version: v0.6.2
 :manual_section: 1
 :manual_group: depthcharge-tools
 
 .. |depthchargectl| replace:: *depthchargectl*\ (1)
 .. |mkimage| replace:: *mkimage*\ (1)
 .. |vbutil_kernel| replace:: *vbutil_kernel*\ (1)
 .. |futility| replace:: *futility*\ (1)
 
-.. |VBOOT_DEVKEYS| replace:: /usr/share/vboot/devkeys
-.. |VBOOT_KEYBLOCK| replace:: |VBOOT_DEVKEYS|/kernel.keyblock
-.. |VBOOT_SIGNPUBKEY| replace:: |VBOOT_DEVKEYS|/kernel_subkey.vbpubk
-.. |VBOOT_SIGNPRIVATE| replace:: |VBOOT_DEVKEYS|/kernel_data_key.vbprivk
+.. |CONFIG_DIR| replace:: **/etc/depthcharge-tools**
+.. |CONFIG_FILE| replace:: **/etc/depthcharge-tools/config**
+.. |CONFIGD_DIR| replace:: **/etc/depthcharge-tools/config.d**
+.. |VBOOT_DEVKEYS| replace:: **/usr/share/vboot/devkeys**
+.. |VBOOT_KEYBLOCK| replace:: **kernel.keyblock**
+.. |VBOOT_SIGNPUBKEY| replace:: **kernel_subkey.vbpubk**
+.. |VBOOT_SIGNPRIVATE| replace:: **kernel_data_key.vbprivk**
 
 SYNOPSIS
 ========
-**mkdepthcharge** **-o** *FILE* [options] [*VMLINUZ*] [*INITRAMFS*] [*DTB* ...]
+**mkdepthcharge** **-o** *FILE* [options] [*VMLINUZ*] [*INITRAMFS* ...] [*DTB* ...]
 
 
 DESCRIPTION
 ===========
 **mkdepthcharge** wraps the |mkimage| and |vbutil_kernel|
 programs with reasonable defaults to package its inputs into the
 format the ChromeOS bootloader expects. It also automates preprocessing
@@ -52,16 +61,17 @@
 Input files
 -----------
 
 -d VMLINUZ, --vmlinuz VMLINUZ
     Kernel executable. If a compressed file is given here, it is
     decompressed and its contents are used in its place.
 
--i INITRAMFS, --initramfs INITRAMFS
-    Ramdisk image.
+-i *INITRAMFS* [*INITRAMFS* ...], --initramfs *INITRAMFS* [*INITRAMFS* ...]
+    Ramdisk image. If multiple files are given (e.g. for CPU microcode
+    updates), they are concatenated and used as a single file.
 
 -b *DTB* [*DTB* ...], --dtbs *DTB* [*DTB* ...]
     Device-tree binary files.
 
 Global options
 --------------
 -A ARCH, --arch ARCH
@@ -100,14 +110,20 @@
     architecture.
 
 -o FILE, --output FILE
     Write the image to *FILE*. The image isn't generated at the output,
     but copied to it from a temporary working directory. This option is
     mandatory.
 
+--pad-vmlinuz, --no-pad-vmlinuz
+    Pad the *VMLINUZ* file so that the kernel's self-decompression has
+    enough space to avoid overwriting the *INITRAMFS* file during boot.
+    This has different defaults and behaviour depending on the image
+    format, see explanations in their respective sections.
+
 --tmpdir DIR
     Create and keep temporary files in *DIR*. If not given, a temporary
     **mkdepthcharge-\*** directory is created in **/tmp** and removed at
     exit.
 
 -v, --verbose
     Print info messages, |mkimage| output and |vbutil_kernel| output to
@@ -122,14 +138,29 @@
     Compress the *VMLINUZ* before packaging it into a FIT image, either
     with **lz4** or **lzma**. **none** is also accepted, but does
     nothing.
 
 -n DESC, --name DESC
     Description of the *VMLINUZ* to put in the FIT image.
 
+--pad-vmlinuz, --no-pad-vmlinuz
+    Pad the *VMLINUZ* file so that the kernel's self-decompression has
+    enough space to avoid overwriting the *INITRAMFS* file during boot.
+    The necessary padding is calculated based on compressed and
+    decompressed kernel sizes and the **--kernel-start** argument.
+
+    On earliest boards U-Boot moves the *INITRAMFS* away to a safe place
+    before running the *VMLINUZ*, and on ARM64 boards Depthcharge itself
+    decompresses the *VMLINUZ* to a safe place. But 32-bit ARM boards
+    with Depthcharge lack FIT ramdisk support and run the *VMLINUZ*
+    in-place, so this initramfs support hack is necessary on those.
+
+    This option is enabled by default when **--patch-dtbs** is given,
+    use the **--no-pad-vmlinuz** argument to disable it.
+
 --patch-dtbs, --no-patch-dtbs
     Add **linux,initrd-start** and **linux,initrd-end** properties to
     the *DTB* files' **/chosen** nodes. Their values are based on the
     **--kernel-start** or the **--ramdisk-load-address** argument, one
     of which is required if this argument is given.
 
     These properties are normally added by Depthcharge, but 32-bit ARM
@@ -157,17 +188,38 @@
     total) they may fit between **--kernel-start** and the start of the
     decompression buffer. In this case the padding is unnecessary and
     not added.
 
     The padding is usually larger than the decompressed version of the
     kernel, so it results in unbootable images for older boards with
     small image size limits. For these, it is usually necessary to use
-    custom kernels to make the parts fit as described above.
+    **--set-init-size**, or custom kernels to make the parts fit as
+    described above.
 
-    This is enabled by default, use the **--no-pad-vmlinuz** argument to
+    This is disabled by default in favour of **--set-init-size**, use
+    the **--pad-vmlinuz** argument to enable it.
+
+--set-init-size, --no-set-init-size
+    Increase the **init_size** kernel boot parameter so that the
+    kernel's self-decompression does not overwrite the *INITRAMFS* file
+    during boot. The modified value is calculated based on values in the
+    zImage header and the **--kernel-start** argument.
+
+    This only works if the kernel has **KASLR** enabled (as is the
+    default), because then the kernel itself tries to avoid overwriting
+    the *INITRAMFS* during decompression. However it does not do this
+    when first copying the *VMLINUZ* to the end of the decompression
+    buffer. Increasing **init_size** shifts copy this upwards to avoid
+    it overlapping *INITRAMFS*.
+
+    If the *VMLINUZ* and *INITRAMFS* are small enough, they may fit
+    before the first compressed copy's start. In this case changing the
+    value is unnecessary and skipped.
+
+    This is enabled by default, use the **--no-set-init-size** argument to
     disable it.
 
 Depthcharge image options
 -------------------------
 --bootloader FILE
     Bootloader stub for the very first Chromebooks that use H2C as their
     firmware. Beyond those, this field is ignored on the firmware side
@@ -187,56 +239,66 @@
     the root partition to the one after the booted partition.
 
     As knowing the currently booted partition is generally useful,
     **mkdepthcharge** prepends **kern_guid=%U** to the given kernel
     command line parameters to capture it. Use **--no-kern-guid** to
     disable this.
 
---keydir DIR
-    Directory containing developer keys to use. Equivalent to using
-    **--keyblock** "*DIR*\ **/kernel.keyblock**", **--signprivate**
-    "*DIR*\ **/kernel_data_key.vbprivk**", and **--signpubkey**
-    "*DIR*\ **/kernel_subkey.vbpubk**".
-
---keyblock FILE
-    Kernel key block file. If not given, the test key files distributed
-    with |vbutil_kernel| are used.
-
 --kern-guid, --no-kern-guid
     Prepend **kern_guid=%U** to kernel command-line parameters. This is
     enabled by default, use the **--no-kern-guid** argument to disable
     it.
 
---signprivate FILE
-    Private keys in .vbprivk format. If not given, the test key files
-    distributed with |vbutil_kernel| are used.
-
---signpubkey FILE
-    Public keys in .vbpubk format. If not given, the test key files
-    distributed with |vbutil_kernel| are used.
+--keydir KEYDIR
+    Directory containing verified boot keys to use. Equivalent to using
+    **--keyblock** *KEYDIR*\/|VBOOT_KEYBLOCK|, **--signprivate**
+    *KEYDIR*\/|VBOOT_SIGNPRIVATE|, and **--signpubkey** *KEYDIR*\
+    /|VBOOT_SIGNPUBKEY|.
+
+--keyblock FILE, --signprivate FILE, --signpubkey FILE
+    ChromiumOS verified boot keys. More specifically: kernel key block,
+    private keys in .vbprivk format, and public keys in .vbpubk format.
+
+    If not given, defaults to files set in **depthcharge-tools**
+    configuration. If those are not set, **mkdepthcharge** searches for
+    these keys in |CONFIG_DIR| and |VBOOT_DEVKEYS| directories, the
+    latter being test keys that may be distributed with |vbutil_kernel|.
+
+    You can set these in **depthcharge-tools** configuration by the
+    **vboot-keyblock**, **vboot-private-key** and **vboot-public-key**
+    options under a **depthcharge-tools** config section.
 
 
 EXIT STATUS
 ===========
 In general, exits with zero on success and non-zero on failure.
 
 
 FILES
 =====
+|CONFIG_FILE|, |CONFIGD_DIR|/*\ **
+    The **depthcharge-tools** configuration files. These might be used
+    to specify locations of the ChromiumOS verified boot keys as system
+    configuration.
+
+|CONFIG_DIR|
+    The **depthcharge-tools** configuration directory. **mkdepthcharge**
+    searches this directory for verified boot keys.
+
 |VBOOT_DEVKEYS|
-    Default devkeys directory containing test keys which might have
-    been installed by |vbutil_kernel|.
+    A directory containing test keys which should have been installed by
+    |vbutil_kernel|.
 
-|VBOOT_KEYBLOCK|
+*KEYDIR*/|VBOOT_KEYBLOCK|
     Default kernel key block file used for signing the image.
 
-|VBOOT_SIGNPUBKEY|
+*KEYDIR*/|VBOOT_SIGNPUBKEY|
     Default public key used to verify signed images.
 
-|VBOOT_SIGNPRIVATE|
+*KEYDIR*/|VBOOT_SIGNPRIVATE|
     Default private key used for signing the image.
 
 
 EXAMPLES
 ========
 **mkdepthcharge** **-o** *depthcharge.img* */boot/vmlinuz*
     The simplest invocation possible. If tried on an ARM board, the
@@ -251,16 +313,17 @@
 
 **mkdepthcharge** **-o** *veyron.img* **-c** *"root=LABEL=ROOT gpt"* **--kernel-start** *0x2000000* **--patch-dtbs** **--** */boot/vmlinuz* */boot/initramfs-linux.img* */boot/dtbs/rk3288-veyron-\*.dtb*
     Build an image intended to work on veyron boards like ASUS
     Chromebook C201PA and Chromebook Flip C100PA. The stock Depthcharge
     on these boards doesn't process the FIT ramdisk, so the dtbs needs
     to be patched to boot with initramfs.
 
-**mkdepthcharge** **-o** *peach-pit.img* **-c** *"console=null"* **--ramdisk-load-address** *0x44000000* **--** *vmlinuz* *initramfs* *exynos5420-peach-pit.dtb*
+**mkdepthcharge** **-o** *peach-pit.img* **-c** *"console=null"* **--ramdisk-load-address** *0x44000000* **--** *vmlinuz* *initramfs* *exynos5420-peach-pit.dtb* *exynos5420-peach-pit.dtb*
     Build an image intended to work on a Samsung Chromebook 2 (11").
     This board uses a custom U-Boot, so needs an explicit ramdisk load
-    address.
+    address. Its firmware has a bug with loading the device-tree file,
+    so needs the file twice for the result to be actually bootable.
 
 SEE ALSO
 ========
 |depthchargectl|, |mkimage|, |vbutil_kernel|, |futility|
```

### Comparing `depthcharge-tools-0.6.1/systemd/90-depthcharge-tools.install` & `depthcharge-tools-0.6.2/systemd/90-depthcharge-tools.install`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #!/bin/sh
 # SPDX-License-Identifier: LGPL-2.1-or-later
-#
+
+# depthcharge-tools kernel-install plugin
+# Copyright (C) 2022 Alper Nebi Yasak <alpernebiyasak@gmail.com>
+# See COPYRIGHT and LICENSE files for full copyright information.
+
 # This is a modified copy of 90-loaderentry.install from systemd.
 #
 # systemd is free software; you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation; either version 2.1 of the License, or
 # (at your option) any later version.
 #
```

