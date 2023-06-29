# Comparing `tmp/pipettor-0.8.0.tar.gz` & `tmp/pipettor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipettor-0.8.0.tar", last modified: Mon Feb  6 05:13:28 2023, max compression
+gzip compressed data, was "pipettor-1.0.0.tar", last modified: Thu Jun 29 23:20:34 2023, max compression
```

## Comparing `pipettor-0.8.0.tar` & `pipettor-1.0.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:28.143951 pipettor-0.8.0/
--rw-rw-r--   0 markd     (1376) genecats  (1305)      122 2015-11-08 04:56:28.000000 pipettor-0.8.0/AUTHORS.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)     3297 2020-12-25 23:35:42.000000 pipettor-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)     1245 2023-02-06 05:09:24.000000 pipettor-0.8.0/HISTORY.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)     1081 2015-11-02 22:32:59.000000 pipettor-0.8.0/LICENSE
--rw-rw-r--   0 markd     (1376) genecats  (1305)      263 2018-07-14 18:31:31.000000 pipettor-0.8.0/MANIFEST.in
--rw-rw-r--   0 markd     (1376) genecats  (1305)     3218 2023-02-06 05:13:28.144951 pipettor-0.8.0/PKG-INFO
--rw-rw-r--   0 markd     (1376) genecats  (1305)      967 2022-07-14 20:42:02.000000 pipettor-0.8.0/README.rst
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:27.985946 pipettor-0.8.0/docs/
--rw-rw-r--   0 markd     (1376) genecats  (1305)     6384 2020-12-25 23:35:42.000000 pipettor-0.8.0/docs/Makefile
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2015-11-02 22:32:59.000000 pipettor-0.8.0/docs/authors.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)     8453 2018-07-14 18:31:26.000000 pipettor-0.8.0/docs/conf.py
--rw-rw-r--   0 markd     (1376) genecats  (1305)       33 2015-11-02 22:32:59.000000 pipettor-0.8.0/docs/contributing.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)      704 2020-12-25 23:35:42.000000 pipettor-0.8.0/docs/design.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2015-11-02 22:32:59.000000 pipettor-0.8.0/docs/history.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)      364 2020-12-25 23:35:42.000000 pipettor-0.8.0/docs/index.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)      154 2018-07-14 18:31:26.000000 pipettor-0.8.0/docs/installation.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)      864 2018-07-14 18:31:26.000000 pipettor-0.8.0/docs/library.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)       27 2015-11-02 22:32:59.000000 pipettor-0.8.0/docs/readme.rst
--rw-rw-r--   0 markd     (1376) genecats  (1305)     2417 2018-07-14 18:31:26.000000 pipettor-0.8.0/docs/usage.rst
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:27.953945 pipettor-0.8.0/lib/
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:27.990946 pipettor-0.8.0/lib/pipettor/
--rw-rw-r--   0 markd     (1376) genecats  (1305)     4931 2023-02-06 05:12:21.000000 pipettor-0.8.0/lib/pipettor/__init__.py
--rw-rw-r--   0 markd     (1376) genecats  (1305)     8240 2023-02-06 04:52:31.000000 pipettor-0.8.0/lib/pipettor/devices.py
--rw-rw-r--   0 markd     (1376) genecats  (1305)     1891 2020-12-25 23:35:42.000000 pipettor-0.8.0/lib/pipettor/exceptions.py
--rw-rw-r--   0 markd     (1376) genecats  (1305)    25979 2023-02-06 04:52:31.000000 pipettor-0.8.0/lib/pipettor/processes.py
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:27.998946 pipettor-0.8.0/lib/pipettor.egg-info/
--rw-rw-r--   0 markd     (1376) genecats  (1305)     3218 2023-02-06 05:13:27.000000 pipettor-0.8.0/lib/pipettor.egg-info/PKG-INFO
--rw-rw-r--   0 markd     (1376) genecats  (1305)     1575 2023-02-06 05:13:27.000000 pipettor-0.8.0/lib/pipettor.egg-info/SOURCES.txt
--rw-rw-r--   0 markd     (1376) genecats  (1305)        1 2023-02-06 05:13:27.000000 pipettor-0.8.0/lib/pipettor.egg-info/dependency_links.txt
--rw-rw-r--   0 markd     (1376) genecats  (1305)        9 2023-02-06 05:13:27.000000 pipettor-0.8.0/lib/pipettor.egg-info/top_level.txt
--rw-rw-r--   0 markd     (1376) genecats  (1305)        1 2022-11-16 23:04:24.000000 pipettor-0.8.0/lib/pipettor.egg-info/zip-safe
--rw-rw-r--   0 markd     (1376) genecats  (1305)      293 2023-02-06 05:13:28.146951 pipettor-0.8.0/setup.cfg
--rw-rw-r--   0 markd     (1376) genecats  (1305)     1551 2023-02-06 05:12:21.000000 pipettor-0.8.0/setup.py
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:28.004946 pipettor-0.8.0/tests/
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:28.009947 pipettor-0.8.0/tests/.emacs.bak/
--rw-rw-r--   0 markd     (1376) genecats  (1305)    20949 2018-02-25 08:49:26.000000 pipettor-0.8.0/tests/.emacs.bak/pipettorTests.py.~1~
--rwxrwxr-x   0 markd     (1376) genecats  (1305)      159 2020-12-25 08:50:01.000000 pipettor-0.8.0/tests/.emacs.bak/progWithError.~1~
--rw-rw-r--   0 markd     (1376) genecats  (1305)        0 2016-08-09 23:57:36.000000 pipettor-0.8.0/tests/__init__.py
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:28.132951 pipettor-0.8.0/tests/expected/
--rw-rw-r--   0 markd     (1376) genecats  (1305)      123 2016-08-09 23:57:36.000000 pipettor-0.8.0/tests/expected/file.binary.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.FunctionTests.testWriteFile.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       70 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.FunctionTests.testWriteFileLex.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.FunctionsTests.testWriteFile.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       56 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PipelineTests.testAppendFile.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PipelineTests.testReadFile.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       14 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PipelineTests.testStdinMem.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PipelineTests.testWriteFile.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PopenTests.testRead.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)        8 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PopenTests.testReadMult.wc
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PopenTests.testWrite.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PopenTests.testWriteFile.out
--rw-rw-r--   0 markd     (1376) genecats  (1305)        8 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/expected/test_pipettor.PopenTests.testWriteMult.wc
-drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-02-06 05:13:28.141951 pipettor-0.8.0/tests/input/
--rw-rw-r--   0 markd     (1376) genecats  (1305)      123 2016-08-09 23:57:36.000000 pipettor-0.8.0/tests/input/file.binary
--rw-rw-r--   0 markd     (1376) genecats  (1305)       61 2018-07-14 18:31:31.000000 pipettor-0.8.0/tests/input/nonAscii.txt
--rw-rw-r--   0 markd     (1376) genecats  (1305)       34 2018-07-14 18:31:31.000000 pipettor-0.8.0/tests/input/simple1.dos.txt
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2018-07-14 18:31:31.000000 pipettor-0.8.0/tests/input/simple1.mac.txt
--rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2016-08-09 23:57:36.000000 pipettor-0.8.0/tests/input/simple1.txt
--rwxrwxr-x   0 markd     (1376) genecats  (1305)      220 2023-01-07 06:58:05.000000 pipettor-0.8.0/tests/progWithError
--rw-rw-r--   0 markd     (1376) genecats  (1305)     8255 2020-12-25 23:35:42.000000 pipettor-0.8.0/tests/testCaseBase.py
--rw-rw-r--   0 markd     (1376) genecats  (1305)    21371 2023-02-06 04:52:31.000000 pipettor-0.8.0/tests/test_pipettor.py
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.298792 pipettor-1.0.0/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      122 2015-11-08 04:56:28.000000 pipettor-1.0.0/AUTHORS.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     3297 2020-12-25 23:35:42.000000 pipettor-1.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     1481 2023-06-29 23:08:48.000000 pipettor-1.0.0/HISTORY.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     1081 2015-11-02 22:32:59.000000 pipettor-1.0.0/LICENSE
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      263 2018-07-14 18:31:31.000000 pipettor-1.0.0/MANIFEST.in
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     3454 2023-06-29 23:20:34.299792 pipettor-1.0.0/PKG-INFO
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      967 2022-07-14 20:42:02.000000 pipettor-1.0.0/README.rst
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.240790 pipettor-1.0.0/docs/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     6384 2020-12-25 23:35:42.000000 pipettor-1.0.0/docs/Makefile
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2015-11-02 22:32:59.000000 pipettor-1.0.0/docs/authors.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     8453 2018-07-14 18:31:26.000000 pipettor-1.0.0/docs/conf.py
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       33 2015-11-02 22:32:59.000000 pipettor-1.0.0/docs/contributing.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2015-11-02 22:32:59.000000 pipettor-1.0.0/docs/history.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      354 2023-06-29 22:55:35.000000 pipettor-1.0.0/docs/index.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      154 2018-07-14 18:31:26.000000 pipettor-1.0.0/docs/installation.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      864 2018-07-14 18:31:26.000000 pipettor-1.0.0/docs/library.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       27 2015-11-02 22:32:59.000000 pipettor-1.0.0/docs/readme.rst
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     2417 2018-07-14 18:31:26.000000 pipettor-1.0.0/docs/usage.rst
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.196788 pipettor-1.0.0/lib/
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.246790 pipettor-1.0.0/lib/pipettor/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     4931 2023-06-29 23:19:30.000000 pipettor-1.0.0/lib/pipettor/__init__.py
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     8240 2023-02-06 04:52:31.000000 pipettor-1.0.0/lib/pipettor/devices.py
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     1891 2020-12-25 23:35:42.000000 pipettor-1.0.0/lib/pipettor/exceptions.py
+-rw-rw-r--   0 markd     (1376) genecats  (1305)    25054 2023-06-29 22:55:35.000000 pipettor-1.0.0/lib/pipettor/processes.py
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.254790 pipettor-1.0.0/lib/pipettor.egg-info/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     3454 2023-06-29 23:20:34.000000 pipettor-1.0.0/lib/pipettor.egg-info/PKG-INFO
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     1591 2023-06-29 23:20:34.000000 pipettor-1.0.0/lib/pipettor.egg-info/SOURCES.txt
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        1 2023-06-29 23:20:34.000000 pipettor-1.0.0/lib/pipettor.egg-info/dependency_links.txt
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        9 2023-06-29 23:20:34.000000 pipettor-1.0.0/lib/pipettor.egg-info/top_level.txt
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        1 2022-11-16 23:04:24.000000 pipettor-1.0.0/lib/pipettor.egg-info/zip-safe
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      293 2023-06-29 23:20:34.300792 pipettor-1.0.0/setup.cfg
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     1551 2023-06-29 23:19:30.000000 pipettor-1.0.0/setup.py
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.260790 pipettor-1.0.0/tests/
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.264791 pipettor-1.0.0/tests/.emacs.bak/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)    20949 2018-02-25 08:49:26.000000 pipettor-1.0.0/tests/.emacs.bak/pipettorTests.py.~1~
+-rwxrwxr-x   0 markd     (1376) genecats  (1305)      159 2020-12-25 08:50:01.000000 pipettor-1.0.0/tests/.emacs.bak/progWithError.~1~
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        1 2023-06-29 23:00:08.000000 pipettor-1.0.0/tests/.emacs.bak/sigTest.py.~1~
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        0 2016-08-09 23:57:36.000000 pipettor-1.0.0/tests/__init__.py
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.288792 pipettor-1.0.0/tests/expected/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      123 2016-08-09 23:57:36.000000 pipettor-1.0.0/tests/expected/file.binary.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.FunctionTests.testWriteFile.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       70 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.FunctionTests.testWriteFileLex.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.FunctionsTests.testWriteFile.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       56 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PipelineTests.testAppendFile.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PipelineTests.testReadFile.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       14 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PipelineTests.testStdinMem.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PipelineTests.testWriteFile.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PopenTests.testRead.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        8 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PopenTests.testReadMult.wc
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PopenTests.testWrite.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PopenTests.testWriteFile.out
+-rw-rw-r--   0 markd     (1376) genecats  (1305)        8 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/expected/test_pipettor.PopenTests.testWriteMult.wc
+drwxrwxr-x   0 markd     (1376) genecats  (1305)        0 2023-06-29 23:20:34.297792 pipettor-1.0.0/tests/input/
+-rw-rw-r--   0 markd     (1376) genecats  (1305)      123 2016-08-09 23:57:36.000000 pipettor-1.0.0/tests/input/file.binary
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       61 2018-07-14 18:31:31.000000 pipettor-1.0.0/tests/input/nonAscii.txt
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       34 2018-07-14 18:31:31.000000 pipettor-1.0.0/tests/input/simple1.dos.txt
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2018-07-14 18:31:31.000000 pipettor-1.0.0/tests/input/simple1.mac.txt
+-rw-rw-r--   0 markd     (1376) genecats  (1305)       28 2016-08-09 23:57:36.000000 pipettor-1.0.0/tests/input/simple1.txt
+-rwxrwxr-x   0 markd     (1376) genecats  (1305)      220 2023-01-07 06:58:05.000000 pipettor-1.0.0/tests/progWithError
+-rw-rw-r--   0 markd     (1376) genecats  (1305)     8255 2020-12-25 23:35:42.000000 pipettor-1.0.0/tests/testCaseBase.py
+-rw-rw-r--   0 markd     (1376) genecats  (1305)    21371 2023-02-06 04:52:31.000000 pipettor-1.0.0/tests/test_pipettor.py
```

### Comparing `pipettor-0.8.0/CONTRIBUTING.rst` & `pipettor-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/HISTORY.rst` & `pipettor-1.0.0/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 .. :changelog:
 
 History
 =======
 
+1.0.0 (2023-06-29)
+-----------------
+* Don't use a process group; as it caused signals to not get propagated.  Processes are explicitly waited for by pid, so this will not consume the exit of other process not create by this module.
+  
+
 0.8.0 (2023-02-05)
 -----------------
 * make most optional arguments require keyword form to help prevent errors, especially if open() options are assumed
 * added more functions to make Popen objects file-like objects
 
 0.7.0 (2023-01-06)
 -----------------
 * don't fail if invalid UTF-8 characters are written to capture stderr
 
 0.6.0 (2022-11-16)
 -----------------
 * remove use of deprecated pipes module
 
-
 0.5.0 (2020-12-25)
 -----------------
 * Removed Python-2 support.
 * Switch to using subprocess as a base rather interface directly
   with Unix system calls.  This lets subprocess deal with
   various issues dealing with the Python interpreter environment.
```

### Comparing `pipettor-0.8.0/LICENSE` & `pipettor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/PKG-INFO` & `pipettor-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipettor
-Version: 0.8.0
+Version: 1.0.0
 Summary: pipettor - robust, easy to use Unix process pipelines
 Home-page: https://github.com/diekhans/pipettor
 Author: Mark Diekhans
 Author-email: markd@ucsc.edu
 License: MIT
 Keywords: Unix,process,pipe
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,28 +50,32 @@
 
 
 
 
 History
 =======
 
+1.0.0 (2023-06-29)
+-----------------
+* Don't use a process group; as it caused signals to not get propagated.  Processes are explicitly waited for by pid, so this will not consume the exit of other process not create by this module.
+  
+
 0.8.0 (2023-02-05)
 -----------------
 * make most optional arguments require keyword form to help prevent errors, especially if open() options are assumed
 * added more functions to make Popen objects file-like objects
 
 0.7.0 (2023-01-06)
 -----------------
 * don't fail if invalid UTF-8 characters are written to capture stderr
 
 0.6.0 (2022-11-16)
 -----------------
 * remove use of deprecated pipes module
 
-
 0.5.0 (2020-12-25)
 -----------------
 * Removed Python-2 support.
 * Switch to using subprocess as a base rather interface directly
   with Unix system calls.  This lets subprocess deal with
   various issues dealing with the Python interpreter environment.
```

### Comparing `pipettor-0.8.0/README.rst` & `pipettor-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/docs/Makefile` & `pipettor-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/docs/conf.py` & `pipettor-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/docs/library.rst` & `pipettor-1.0.0/docs/library.rst`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/docs/usage.rst` & `pipettor-1.0.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/lib/pipettor/__init__.py` & `pipettor-1.0.0/lib/pipettor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Robust, easy to use Unix process pipelines.
 """
 import shlex
 from pipettor.exceptions import PipettorException, ProcessException
 from pipettor.devices import DataReader, DataWriter, File
 from pipettor.processes import Pipeline, Popen, setDefaultLogger, getDefaultLogger, setDefaultLogLevel, getDefaultLogLevel, setDefaultLogging
 
-__version__ = "0.8.0"
+__version__ = "1.0.0"
 
 
 def run(cmds, stdin=None, stdout=None, stderr=DataReader, logger=None, logLevel=None):
     """Construct and run an process pipeline. If any of the processes fail,
     a ProcessException is throw.
 
     `cmds` is either a list of arguments for a single process, or a list of
```

### Comparing `pipettor-0.8.0/lib/pipettor/devices.py` & `pipettor-1.0.0/lib/pipettor/devices.py`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/lib/pipettor/exceptions.py` & `pipettor-1.0.0/lib/pipettor/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/lib/pipettor/processes.py` & `pipettor-1.0.0/lib/pipettor/processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 from pipettor.devices import DataReader
 from pipettor.devices import _SiblingPipe
 from pipettor.devices import File
 from pipettor.exceptions import PipettorException
 from pipettor.exceptions import ProcessException
 from pipettor.exceptions import _warn_error_during_error_handling
 
-# FIXME: C-c problems:
-# http://code.activestate.com/recipes/496735-workaround-for-missed-sigint-in-multithreaded-prog/
-# http://bugs.python.org/issue21822
-# FIXME above handled by subprocess??
-
 _defaultLogger = None
 _defaultLogLevel = logging.DEBUG
 
 def setDefaultLogger(logger):
     """Set the default pipettor logger used in logging command and errors.
     If None, there is no default logging.  The logger can be the name of
     a logger or the logger itself.  Standard value is None"""
@@ -102,15 +97,14 @@
         self.stdin = self._stdio_assoc(stdin, "r")
         self.stdout = self._stdio_assoc(stdout, "w")
         if stderr == DataReader:
             stderr = DataReader(errors='backslashreplace')
         self.stderr = self._stdio_assoc(stderr, "w")
         self.popen = None
         self.pid = None
-        self.pgid = None
         self.returncode = None  # exit code, or -signal
         # FIXME: should this just be exception for the users??
         self.procExcept = None  # exception because of failed process
         self.state = State.PREINIT
         self.forced = False    # force termination during error cleanup
 
     def __str__(self):
@@ -140,43 +134,32 @@
             return spec
         elif isinstance(spec, Dev):
             return spec.read_fd if stdfd == 0 else spec.write_fd
         else:
             # this should have been detected earlier
             raise PipettorException("_get_child_stdio logic error: {} {}".format(type(spec), stdfd))
 
-    def _start_process(self, pgid):
-        """Do work of starting the process.  If pgid is None, this process
-        becomes group leader, otherwise this process is added to group pgid."""
+    def _start_process(self):
+        """Do work of starting the process"""
         self.state = State.STARTUP    # do first to prevent restarts on error
 
-        # standard dance to get process group set
-        # preexec_fn will go away: https://bugs.python.org/issue38435
-        if pgid is None:
-            preexecFn = lambda: os.setpgid(os.getpid(), os.getpid())  # noqa
-        else:
-            preexecFn = lambda: os.setpgid(os.getpid(), pgid)  # noqa
-
         try:
             self.popen = subprocess.Popen(self.cmd,
                                           stdin=self._get_child_stdio(self.stdin, 0),
                                           stdout=self._get_child_stdio(self.stdout, 1),
-                                          stderr=self._get_child_stdio(self.stderr, 2),
-                                          preexec_fn=preexecFn)
+                                          stderr=self._get_child_stdio(self.stderr, 2))
         except Exception as ex:
             raise ProcessException(str(self)) from ex
         self.pid = self.popen.pid
-        self.pgid = self.pid if pgid is None else pgid
         self.state = State.RUNNING
 
-    def _start(self, pgid):
-        """Start the process,  If pgid is None, this process
-        becomes group leader."""
+    def _start(self):
+        """Start the process,"""
         try:
-            self._start_process(pgid)
+            self._start_process()
         except BaseException as ex:
             self.procExcept = ex
         if self.procExcept is not None:
             raise self.procExcept
 
     @property
     def running(self):
@@ -277,15 +260,14 @@
                  logger=None, logLevel=None):
         self.lock = RLock()
         self.stdin = stdin
         self.stdout = stdout
         self.stderr = stderr
         self.procs = []
         self.devs = set()
-        self.pgid = None       # process group leader
         self.bypid = dict()    # indexed by pid
         self.state = State.PREINIT
         self.logger = _getLoggerToUse(logger)
         self.logLevel = _getLogLevelToUse(logLevel)
 
         if isinstance(cmds[0], str):
             cmds = [cmds]  # one-process pipeline
@@ -368,17 +350,16 @@
         if self.stderr == DataReader:
             desc += " 2>[DataReader]"  # instance made in Process
         elif self.stderr not in (None, 2):
             desc += " 2>" + str(self.stderr)
         return desc
 
     def _start_process(self, proc):
-        proc._start(self.pgid)
+        proc._start()
         self.bypid[proc.pid] = proc
-        self.pgid = proc.pgid
 
     def _start_processes(self):
         for proc in self.procs:
             self._start_process(proc)
 
     def _post_start_parent(self):
         for d in self.devs:
```

### Comparing `pipettor-0.8.0/lib/pipettor.egg-info/PKG-INFO` & `pipettor-1.0.0/lib/pipettor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipettor
-Version: 0.8.0
+Version: 1.0.0
 Summary: pipettor - robust, easy to use Unix process pipelines
 Home-page: https://github.com/diekhans/pipettor
 Author: Mark Diekhans
 Author-email: markd@ucsc.edu
 License: MIT
 Keywords: Unix,process,pipe
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,28 +50,32 @@
 
 
 
 
 History
 =======
 
+1.0.0 (2023-06-29)
+-----------------
+* Don't use a process group; as it caused signals to not get propagated.  Processes are explicitly waited for by pid, so this will not consume the exit of other process not create by this module.
+  
+
 0.8.0 (2023-02-05)
 -----------------
 * make most optional arguments require keyword form to help prevent errors, especially if open() options are assumed
 * added more functions to make Popen objects file-like objects
 
 0.7.0 (2023-01-06)
 -----------------
 * don't fail if invalid UTF-8 characters are written to capture stderr
 
 0.6.0 (2022-11-16)
 -----------------
 * remove use of deprecated pipes module
 
-
 0.5.0 (2020-12-25)
 -----------------
 * Removed Python-2 support.
 * Switch to using subprocess as a base rather interface directly
   with Unix system calls.  This lets subprocess deal with
   various issues dealing with the Python interpreter environment.
```

### Comparing `pipettor-0.8.0/lib/pipettor.egg-info/SOURCES.txt` & `pipettor-1.0.0/lib/pipettor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
-docs/design.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/library.rst
 docs/readme.rst
 docs/usage.rst
 lib/pipettor/__init__.py
@@ -28,14 +27,15 @@
 lib/pipettor.egg-info/zip-safe
 tests/__init__.py
 tests/progWithError
 tests/testCaseBase.py
 tests/test_pipettor.py
 tests/.emacs.bak/pipettorTests.py.~1~
 tests/.emacs.bak/progWithError.~1~
+tests/.emacs.bak/sigTest.py.~1~
 tests/expected/file.binary.out
 tests/expected/test_pipettor.FunctionTests.testWriteFile.out
 tests/expected/test_pipettor.FunctionTests.testWriteFileLex.out
 tests/expected/test_pipettor.FunctionsTests.testWriteFile.out
 tests/expected/test_pipettor.PipelineTests.testAppendFile.out
 tests/expected/test_pipettor.PipelineTests.testReadFile.out
 tests/expected/test_pipettor.PipelineTests.testStdinMem.out
```

### Comparing `pipettor-0.8.0/setup.py` & `pipettor-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     history = history_file.read().replace('.. :changelog:', '')
 
 requirements = [
 ]
 
 setuptools.setup(
     name = 'pipettor',
-    version = '0.8.0',
+    version = '1.0.0',
     description = "pipettor - robust, easy to use Unix process pipelines",
     long_description = readme + '\n\n' + history,
     long_description_content_type="text/markdown",
     author = "Mark Diekhans",
     author_email = 'markd@ucsc.edu',
     url = 'https://github.com/diekhans/pipettor',
     packages = [
```

### Comparing `pipettor-0.8.0/tests/.emacs.bak/pipettorTests.py.~1~` & `pipettor-1.0.0/tests/.emacs.bak/pipettorTests.py.~1~`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/tests/testCaseBase.py` & `pipettor-1.0.0/tests/testCaseBase.py`

 * *Files identical despite different names*

### Comparing `pipettor-0.8.0/tests/test_pipettor.py` & `pipettor-1.0.0/tests/test_pipettor.py`

 * *Files identical despite different names*

