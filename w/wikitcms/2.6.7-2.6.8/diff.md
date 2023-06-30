# Comparing `tmp/wikitcms-2.6.7.tar.gz` & `tmp/wikitcms-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikitcms-2.6.7.tar", last modified: Fri Dec 16 18:08:46 2022, max compression
+gzip compressed data, was "wikitcms-2.6.8.tar", last modified: Fri Jun 30 18:23:34 2023, max compression
```

## Comparing `wikitcms-2.6.7.tar` & `wikitcms-2.6.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 adamw     (1001) adamw     (1001)        0 2022-12-16 18:08:46.917522 wikitcms-2.6.7/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       73 2020-05-12 20:42:40.000000 wikitcms-2.6.7/.pylintrc
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    25422 2022-12-16 18:06:16.000000 wikitcms-2.6.7/CHANGELOG.md
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    35147 2007-07-01 22:55:35.000000 wikitcms-2.6.7/COPYING
--rw-r--r--   0 adamw     (1001) adamw     (1001)    11417 2022-12-16 18:08:46.917522 wikitcms-2.6.7/PKG-INFO
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    10910 2020-05-12 20:42:40.000000 wikitcms-2.6.7/README.md
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       38 2020-05-12 20:42:40.000000 wikitcms-2.6.7/ci.requires
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       63 2019-11-14 01:38:23.000000 wikitcms-2.6.7/install.requires
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      365 2020-05-12 20:42:40.000000 wikitcms-2.6.7/pyproject.toml
--rwxrwxr-x   0 adamw     (1001) adamw     (1001)      749 2022-12-16 18:07:49.000000 wikitcms-2.6.7/release.sh
--rw-r--r--   0 adamw     (1001) adamw     (1001)       38 2022-12-16 18:08:46.918522 wikitcms-2.6.7/setup.cfg
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     1789 2022-12-16 18:08:21.000000 wikitcms-2.6.7/setup.py
-drwxr-xr-x   0 adamw     (1001) adamw     (1001)        0 2022-12-16 18:08:46.897521 wikitcms-2.6.7/src/
-drwxr-xr-x   0 adamw     (1001) adamw     (1001)        0 2022-12-16 18:08:46.906521 wikitcms-2.6.7/src/wikitcms/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      862 2022-12-16 18:08:21.000000 wikitcms-2.6.7/src/wikitcms/__init__.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    16152 2022-01-27 01:05:13.000000 wikitcms-2.6.7/src/wikitcms/event.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     1351 2021-06-01 19:48:49.000000 wikitcms-2.6.7/src/wikitcms/exceptions.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     9369 2021-06-01 19:48:49.000000 wikitcms-2.6.7/src/wikitcms/helpers.py
--rw-r--r--   0 adamw     (1001) adamw     (1001)    15163 2022-12-16 18:05:38.000000 wikitcms-2.6.7/src/wikitcms/listing.py
--rw-r--r--   0 adamw     (1001) adamw     (1001)    35183 2022-12-16 18:05:38.000000 wikitcms-2.6.7/src/wikitcms/page.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     2173 2021-06-01 19:48:49.000000 wikitcms-2.6.7/src/wikitcms/release.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    21263 2021-06-01 19:48:49.000000 wikitcms-2.6.7/src/wikitcms/result.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    34813 2022-01-27 00:52:51.000000 wikitcms-2.6.7/src/wikitcms/wiki.py
-drwxr-xr-x   0 adamw     (1001) adamw     (1001)        0 2022-12-16 18:08:46.912521 wikitcms-2.6.7/src/wikitcms.egg-info/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    11417 2022-12-16 18:08:46.000000 wikitcms-2.6.7/src/wikitcms.egg-info/PKG-INFO
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     1514 2022-12-16 18:08:46.000000 wikitcms-2.6.7/src/wikitcms.egg-info/SOURCES.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)        1 2022-12-16 18:08:46.000000 wikitcms-2.6.7/src/wikitcms.egg-info/dependency_links.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       63 2022-12-16 18:08:46.000000 wikitcms-2.6.7/src/wikitcms.egg-info/requires.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)        9 2022-12-16 18:08:46.000000 wikitcms-2.6.7/src/wikitcms.egg-info/top_level.txt
-drwxr-xr-x   0 adamw     (1001) adamw     (1001)        0 2022-12-16 18:08:46.913521 wikitcms-2.6.7/tests/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     4030 2021-06-01 19:48:55.000000 wikitcms-2.6.7/tests/conftest.py
-drwxr-xr-x   0 adamw     (1001) adamw     (1001)        0 2022-12-16 18:08:46.917522 wikitcms-2.6.7/tests/data/
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    27890 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     1863 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    61816 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Fedora-32-20200312.0.images.json
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    11495 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    12456 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     8425 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Day:2013-11-05_Printing.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    20634 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    20535 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Day:2016-10-24_Cloud.txt
--rw-r--r--   0 adamw     (1001) adamw     (1001)     3296 2020-05-21 22:11:13.000000 wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json
--rw-r--r--   0 adamw     (1001) adamw     (1001)    12476 2020-05-21 22:09:03.000000 wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     6971 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    22861 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     3843 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     4081 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    23892 2022-01-27 01:05:13.000000 wikitcms-2.6.7/tests/test_event.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     6290 2022-01-27 01:05:13.000000 wikitcms-2.6.7/tests/test_helpers.py
--rw-r--r--   0 adamw     (1001) adamw     (1001)    18059 2022-12-16 18:05:38.000000 wikitcms-2.6.7/tests/test_listing.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    42241 2021-06-01 19:48:55.000000 wikitcms-2.6.7/tests/test_page.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)     3221 2021-06-01 19:48:55.000000 wikitcms-2.6.7/tests/test_release.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    26439 2022-01-27 01:05:13.000000 wikitcms-2.6.7/tests/test_result.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)    29575 2021-06-01 19:48:55.000000 wikitcms-2.6.7/tests/test_wiki.py
--rw-rw-r--   0 adamw     (1001) adamw     (1001)       22 2020-05-12 20:42:40.000000 wikitcms-2.6.7/tests.requires
--rw-rw-r--   0 adamw     (1001) adamw     (1001)      488 2021-11-12 19:49:43.000000 wikitcms-2.6.7/tox.ini
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.178209 wikitcms-2.6.8/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       73 2023-03-02 16:57:00.000000 wikitcms-2.6.8/.pylintrc
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    25619 2023-06-30 18:22:37.000000 wikitcms-2.6.8/CHANGELOG.md
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    35147 2023-03-02 16:57:00.000000 wikitcms-2.6.8/COPYING
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    11417 2023-06-30 18:23:34.178209 wikitcms-2.6.8/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    10910 2023-03-02 16:57:00.000000 wikitcms-2.6.8/README.md
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-03-02 16:57:00.000000 wikitcms-2.6.8/ci.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       63 2023-03-02 16:57:00.000000 wikitcms-2.6.8/install.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      366 2023-05-05 20:38:09.000000 wikitcms-2.6.8/pyproject.toml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      749 2023-03-02 16:57:00.000000 wikitcms-2.6.8/release.sh
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-06-30 18:23:34.178209 wikitcms-2.6.8/setup.cfg
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1789 2023-06-30 18:23:10.000000 wikitcms-2.6.8/setup.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.175209 wikitcms-2.6.8/src/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.176209 wikitcms-2.6.8/src/wikitcms/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      862 2023-06-30 18:23:10.000000 wikitcms-2.6.8/src/wikitcms/__init__.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    16152 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/event.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1351 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/exceptions.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     9369 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    15163 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/listing.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    35320 2023-06-30 18:19:26.000000 wikitcms-2.6.8/src/wikitcms/page.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2173 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/release.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    21263 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/result.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    34813 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/wiki.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.176209 wikitcms-2.6.8/src/wikitcms.egg-info/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    11417 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1514 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/SOURCES.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)        1 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/dependency_links.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       63 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/requires.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)        9 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/top_level.txt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.177209 wikitcms-2.6.8/tests/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4030 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/conftest.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.177209 wikitcms-2.6.8/tests/data/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27890 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1863 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    61816 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.images.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    11495 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    12456 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     8425 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Day:2013-11-05_Printing.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    20634 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    20535 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3296 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    12476 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     6971 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    22861 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3843 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4081 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    23892 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_event.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     6290 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    18059 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_listing.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    42241 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_page.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3221 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_release.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    26439 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_result.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    29575 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_wiki.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       22 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      488 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tox.ini
```

### Comparing `wikitcms-2.6.7/CHANGELOG.md` & `wikitcms-2.6.8/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ## Changelog
 
+### 2.6.8 - 2023-06-30
+
+*   [wikitcms-2.6.8.tar.gz](https://files.pythonhosted.org/packages/source/w/wikitcms/wikitcms-2.6.8.tar.gz)
+
+1.  Handle "gp3" volume type in the AMI table generation code
+
 ### 2.6.7 - 2022-12-16
 
 *   [wikitcms-2.6.7.tar.gz](https://files.pythonhosted.org/packages/source/w/wikitcms/wikitcms-2.6.7.tar.gz)
 
 1.  Treat matrix template pages as result pages
 
 ### 2.6.6 - 2022-01-26
```

### Comparing `wikitcms-2.6.7/COPYING` & `wikitcms-2.6.8/COPYING`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/PKG-INFO` & `wikitcms-2.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikitcms
-Version: 2.6.7
+Version: 2.6.8
 Summary: Fedora QA wiki test management library
 Home-page: https://pagure.io/fedora-qa/python-wikitcms
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora qa mediawiki validation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wikitcms-2.6.7/README.md` & `wikitcms-2.6.8/README.md`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/release.sh` & `wikitcms-2.6.8/release.sh`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/setup.py` & `wikitcms-2.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     LONGDESC = f.read()
 
 setup(
     name="wikitcms",
-    version="2.6.7",
+    version="2.6.8",
     author="Adam Williamson",
     author_email="awilliam@redhat.com",
     description="Fedora QA wiki test management library",
     license="GPLv3+",
     keywords="fedora qa mediawiki validation",
     url="https://pagure.io/fedora-qa/python-wikitcms",
     packages=["wikitcms"],
```

### Comparing `wikitcms-2.6.7/src/wikitcms/__init__.py` & `wikitcms-2.6.8/src/wikitcms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 #
 # Author:   Adam Williamson <awilliam@redhat.com>
 
 """Library for interacting with Fedora release validation and test day
 wiki pages.
 """
 
-__version__ = "2.6.7"
+__version__ = "2.6.8"
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `wikitcms-2.6.7/src/wikitcms/event.py` & `wikitcms-2.6.8/src/wikitcms/event.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms/exceptions.py` & `wikitcms-2.6.8/src/wikitcms/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms/helpers.py` & `wikitcms-2.6.8/src/wikitcms/helpers.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms/listing.py` & `wikitcms-2.6.8/src/wikitcms/listing.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms/page.py` & `wikitcms-2.6.8/src/wikitcms/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,26 +711,30 @@
             relevants = [
                 msg
                 for msg in ours
                 if msg["architecture"] == arch
                 and msg["extra"]["virt_type"] == virttype
                 and msg["extra"]["vol_type"] == voltype
             ]
+            if not relevants:
+                return ""
             # sort the messages by region so the table is easier to scan
             relevants.sort(key=lambda x: x["destination"])
             for msg in relevants:
                 ret += _table_line(msg)
             ret += "|}\n\n"
             return ret
 
         # now let's create and populate the tables
         for arch in ("x86_64", "arm64"):
             for virttype in ("hvm",):
-                for voltype in ("standard", "gp2"):
-                    text += _table(arch, virttype, voltype)
+                for voltype in ("standard", "gp2", "gp3"):
+                    newtext = _table(arch, virttype, voltype)
+                    if newtext:
+                        text += newtext
 
         return text
 
 
 class TestDayPage(Page):
     """A Test Day results page. Usually contains table(s) with test
     cases as the column headers and users as the rows - each row is
```

### Comparing `wikitcms-2.6.7/src/wikitcms/release.py` & `wikitcms-2.6.8/src/wikitcms/release.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms/result.py` & `wikitcms-2.6.8/src/wikitcms/result.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms/wiki.py` & `wikitcms-2.6.8/src/wikitcms/wiki.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/src/wikitcms.egg-info/PKG-INFO` & `wikitcms-2.6.8/src/wikitcms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikitcms
-Version: 2.6.7
+Version: 2.6.8
 Summary: Fedora QA wiki test management library
 Home-page: https://pagure.io/fedora-qa/python-wikitcms
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora qa mediawiki validation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wikitcms-2.6.7/src/wikitcms.egg-info/SOURCES.txt` & `wikitcms-2.6.8/src/wikitcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/conftest.py` & `wikitcms-2.6.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json` & `wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json` & `wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Fedora-32-20200312.0.images.json` & `wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.images.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext` & `wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext` & `wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Day:2013-11-05_Printing.txt` & `wikitcms-2.6.8/tests/data/Test_Day:2013-11-05_Printing.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt` & `wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Day:2016-10-24_Cloud.txt` & `wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json` & `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt` & `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json` & `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt` & `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json` & `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt` & `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_event.py` & `wikitcms-2.6.8/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_helpers.py` & `wikitcms-2.6.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_listing.py` & `wikitcms-2.6.8/tests/test_listing.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_page.py` & `wikitcms-2.6.8/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_release.py` & `wikitcms-2.6.8/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_result.py` & `wikitcms-2.6.8/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.7/tests/test_wiki.py` & `wikitcms-2.6.8/tests/test_wiki.py`

 * *Files identical despite different names*

