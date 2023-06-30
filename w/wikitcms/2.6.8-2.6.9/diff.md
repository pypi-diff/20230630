# Comparing `tmp/wikitcms-2.6.8.tar.gz` & `tmp/wikitcms-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikitcms-2.6.8.tar", last modified: Fri Jun 30 18:23:34 2023, max compression
+gzip compressed data, was "wikitcms-2.6.9.tar", last modified: Fri Jun 30 19:09:10 2023, max compression
```

## Comparing `wikitcms-2.6.8.tar` & `wikitcms-2.6.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.178209 wikitcms-2.6.8/
--rw-r--r--   0 adamw     (1000) adamw     (1000)       73 2023-03-02 16:57:00.000000 wikitcms-2.6.8/.pylintrc
--rw-r--r--   0 adamw     (1000) adamw     (1000)    25619 2023-06-30 18:22:37.000000 wikitcms-2.6.8/CHANGELOG.md
--rw-r--r--   0 adamw     (1000) adamw     (1000)    35147 2023-03-02 16:57:00.000000 wikitcms-2.6.8/COPYING
--rw-r--r--   0 adamw     (1000) adamw     (1000)    11417 2023-06-30 18:23:34.178209 wikitcms-2.6.8/PKG-INFO
--rw-r--r--   0 adamw     (1000) adamw     (1000)    10910 2023-03-02 16:57:00.000000 wikitcms-2.6.8/README.md
--rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-03-02 16:57:00.000000 wikitcms-2.6.8/ci.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)       63 2023-03-02 16:57:00.000000 wikitcms-2.6.8/install.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)      366 2023-05-05 20:38:09.000000 wikitcms-2.6.8/pyproject.toml
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)      749 2023-03-02 16:57:00.000000 wikitcms-2.6.8/release.sh
--rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-06-30 18:23:34.178209 wikitcms-2.6.8/setup.cfg
--rw-r--r--   0 adamw     (1000) adamw     (1000)     1789 2023-06-30 18:23:10.000000 wikitcms-2.6.8/setup.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.175209 wikitcms-2.6.8/src/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.176209 wikitcms-2.6.8/src/wikitcms/
--rw-r--r--   0 adamw     (1000) adamw     (1000)      862 2023-06-30 18:23:10.000000 wikitcms-2.6.8/src/wikitcms/__init__.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    16152 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/event.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     1351 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/exceptions.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     9369 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    15163 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/listing.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    35320 2023-06-30 18:19:26.000000 wikitcms-2.6.8/src/wikitcms/page.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     2173 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/release.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    21263 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/result.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    34813 2023-03-02 16:57:00.000000 wikitcms-2.6.8/src/wikitcms/wiki.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.176209 wikitcms-2.6.8/src/wikitcms.egg-info/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    11417 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/PKG-INFO
--rw-r--r--   0 adamw     (1000) adamw     (1000)     1514 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/SOURCES.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)        1 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/dependency_links.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)       63 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/requires.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)        9 2023-06-30 18:23:34.000000 wikitcms-2.6.8/src/wikitcms.egg-info/top_level.txt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.177209 wikitcms-2.6.8/tests/
--rw-r--r--   0 adamw     (1000) adamw     (1000)     4030 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/conftest.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 18:23:34.177209 wikitcms-2.6.8/tests/data/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27890 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)     1863 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    61816 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.images.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    11495 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext
--rw-r--r--   0 adamw     (1000) adamw     (1000)    12456 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext
--rw-r--r--   0 adamw     (1000) adamw     (1000)     8425 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Day:2013-11-05_Printing.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)    20634 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)    20535 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)     3296 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    12476 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)     6971 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    22861 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)     3843 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)     4081 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt
--rw-r--r--   0 adamw     (1000) adamw     (1000)    23892 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_event.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     6290 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    18059 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_listing.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    42241 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_page.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     3221 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_release.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    26439 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_result.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    29575 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests/test_wiki.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)       22 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tests.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)      488 2023-03-02 16:57:00.000000 wikitcms-2.6.8/tox.ini
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 19:09:10.914469 wikitcms-2.6.9/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       73 2023-03-02 16:57:00.000000 wikitcms-2.6.9/.pylintrc
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    25811 2023-06-30 19:08:34.000000 wikitcms-2.6.9/CHANGELOG.md
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    35147 2023-03-02 16:57:00.000000 wikitcms-2.6.9/COPYING
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    11417 2023-06-30 19:09:10.914469 wikitcms-2.6.9/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    10910 2023-03-02 16:57:00.000000 wikitcms-2.6.9/README.md
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-03-02 16:57:00.000000 wikitcms-2.6.9/ci.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       63 2023-03-02 16:57:00.000000 wikitcms-2.6.9/install.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      366 2023-05-05 20:38:09.000000 wikitcms-2.6.9/pyproject.toml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      749 2023-03-02 16:57:00.000000 wikitcms-2.6.9/release.sh
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-06-30 19:09:10.914469 wikitcms-2.6.9/setup.cfg
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1789 2023-06-30 19:08:47.000000 wikitcms-2.6.9/setup.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 19:09:10.907469 wikitcms-2.6.9/src/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 19:09:10.910469 wikitcms-2.6.9/src/wikitcms/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      862 2023-06-30 19:08:47.000000 wikitcms-2.6.9/src/wikitcms/__init__.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    16152 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/event.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1351 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/exceptions.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     9369 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    15163 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/listing.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    35310 2023-06-30 19:06:28.000000 wikitcms-2.6.9/src/wikitcms/page.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2173 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/release.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    21263 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/result.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    34813 2023-03-02 16:57:00.000000 wikitcms-2.6.9/src/wikitcms/wiki.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 19:09:10.910469 wikitcms-2.6.9/src/wikitcms.egg-info/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    11417 2023-06-30 19:09:10.000000 wikitcms-2.6.9/src/wikitcms.egg-info/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1514 2023-06-30 19:09:10.000000 wikitcms-2.6.9/src/wikitcms.egg-info/SOURCES.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)        1 2023-06-30 19:09:10.000000 wikitcms-2.6.9/src/wikitcms.egg-info/dependency_links.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       63 2023-06-30 19:09:10.000000 wikitcms-2.6.9/src/wikitcms.egg-info/requires.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)        9 2023-06-30 19:09:10.000000 wikitcms-2.6.9/src/wikitcms.egg-info/top_level.txt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 19:09:10.911469 wikitcms-2.6.9/tests/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4030 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/conftest.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-30 19:09:10.913469 wikitcms-2.6.9/tests/data/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27890 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1863 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    61816 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Fedora-32-20200312.0.images.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    11508 2023-06-30 19:07:24.000000 wikitcms-2.6.9/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    12456 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     8425 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Day:2013-11-05_Printing.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    20634 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    20535 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Day:2016-10-24_Cloud.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3296 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    12476 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     6971 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    22861 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3843 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     4081 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    23892 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_event.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     6290 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    18059 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_listing.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    42241 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_page.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     3221 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_release.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    26439 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_result.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    29575 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests/test_wiki.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       22 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tests.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      488 2023-03-02 16:57:00.000000 wikitcms-2.6.9/tox.ini
```

### Comparing `wikitcms-2.6.8/CHANGELOG.md` & `wikitcms-2.6.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ## Changelog
 
+### 2.6.9 - 2023-06-30
+
+*   [wikitcms-2.6.9.tar.gz](https://files.pythonhosted.org/packages/source/w/wikitcms/wikitcms-2.6.9.tar.gz)
+
+1.  Expand "gp3" not "standard" by default in AMI tables
+
 ### 2.6.8 - 2023-06-30
 
 *   [wikitcms-2.6.8.tar.gz](https://files.pythonhosted.org/packages/source/w/wikitcms/wikitcms-2.6.8.tar.gz)
 
 1.  Handle "gp3" volume type in the AMI table generation code
 
 ### 2.6.7 - 2022-12-16
```

### Comparing `wikitcms-2.6.8/COPYING` & `wikitcms-2.6.9/COPYING`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/PKG-INFO` & `wikitcms-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikitcms
-Version: 2.6.8
+Version: 2.6.9
 Summary: Fedora QA wiki test management library
 Home-page: https://pagure.io/fedora-qa/python-wikitcms
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora qa mediawiki validation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wikitcms-2.6.8/README.md` & `wikitcms-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/release.sh` & `wikitcms-2.6.9/release.sh`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/setup.py` & `wikitcms-2.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     LONGDESC = f.read()
 
 setup(
     name="wikitcms",
-    version="2.6.8",
+    version="2.6.9",
     author="Adam Williamson",
     author_email="awilliam@redhat.com",
     description="Fedora QA wiki test management library",
     license="GPLv3+",
     keywords="fedora qa mediawiki validation",
     url="https://pagure.io/fedora-qa/python-wikitcms",
     packages=["wikitcms"],
```

### Comparing `wikitcms-2.6.8/src/wikitcms/__init__.py` & `wikitcms-2.6.9/src/wikitcms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 #
 # Author:   Adam Williamson <awilliam@redhat.com>
 
 """Library for interacting with Fedora release validation and test day
 wiki pages.
 """
 
-__version__ = "2.6.8"
+__version__ = "2.6.9"
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `wikitcms-2.6.8/src/wikitcms/event.py` & `wikitcms-2.6.9/src/wikitcms/event.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms/exceptions.py` & `wikitcms-2.6.9/src/wikitcms/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms/helpers.py` & `wikitcms-2.6.9/src/wikitcms/helpers.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms/listing.py` & `wikitcms-2.6.9/src/wikitcms/listing.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms/page.py` & `wikitcms-2.6.9/src/wikitcms/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -698,16 +698,16 @@
             url += f"region={destination}#LaunchInstanceWizard:ami={ami}"
             return f"| {destination}\n| {ami}\n| [{url} Launch in EC2]\n|-\n"
 
         def _table(arch, virttype, voltype):
             """Convenience function for adding a table."""
             ret = f"== {arch} {virttype} {voltype} AMIs ==\n\n"
             ret += '{| class="wikitable sortable mw-collapsible'
-            if arch != "x86_64" or virttype != "hvm" or voltype != "standard":
-                # we expand the x86_64 hvm standard table by default
+            if arch != "x86_64" or virttype != "hvm" or voltype != "gp3":
+                # we expand the x86_64 hvm gp3 table by default
                 ret += " mw-collapsed"
             ret += '" width=100%\n|-\n'
             ret += "! Region !! AMI ID !! Direct launch link\n|-\n"
             # find the right messages for this arch and types
             relevants = [
                 msg
                 for msg in ours
```

### Comparing `wikitcms-2.6.8/src/wikitcms/release.py` & `wikitcms-2.6.9/src/wikitcms/release.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms/result.py` & `wikitcms-2.6.9/src/wikitcms/result.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms/wiki.py` & `wikitcms-2.6.9/src/wikitcms/wiki.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/src/wikitcms.egg-info/PKG-INFO` & `wikitcms-2.6.9/src/wikitcms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikitcms
-Version: 2.6.8
+Version: 2.6.9
 Summary: Fedora QA wiki test management library
 Home-page: https://pagure.io/fedora-qa/python-wikitcms
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora qa mediawiki validation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wikitcms-2.6.8/src/wikitcms.egg-info/SOURCES.txt` & `wikitcms-2.6.9/src/wikitcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/conftest.py` & `wikitcms-2.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json` & `wikitcms-2.6.9/tests/data/Fedora-32-20200312.0.ami.dgdata.1.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json` & `wikitcms-2.6.9/tests/data/Fedora-32-20200312.0.ami.dgdata.2.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Fedora-32-20200312.0.images.json` & `wikitcms-2.6.9/tests/data/Fedora-32-20200312.0.images.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext` & `wikitcms-2.6.9/tests/data/Template:Fedora 32 Beta 1.2 AMI.seedtext`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 == x86_64 hvm standard AMIs ==
 
-{| class="wikitable sortable mw-collapsible" width=100%
+{| class="wikitable sortable mw-collapsible mw-collapsed" width=100%
 |-
 ! Region !! AMI ID !! Direct launch link
 |-
 | ap-northeast-1
 | ami-053db6774d7445008
 | [https://redirect.fedoraproject.org/console.aws.amazon.com/ec2/v2/home?region=ap-northeast-1#LaunchInstanceWizard:ami=ami-053db6774d7445008 Launch in EC2]
 |-
```

### Comparing `wikitcms-2.6.8/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext` & `wikitcms-2.6.9/tests/data/Template:Fedora 32 Beta 1.2 Download.seedtext`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Day:2013-11-05_Printing.txt` & `wikitcms-2.6.9/tests/data/Test_Day:2013-11-05_Printing.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt` & `wikitcms-2.6.9/tests/data/Test_Day:2016-10-24_Cloud.longrefs.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Day:2016-10-24_Cloud.txt` & `wikitcms-2.6.9/tests/data/Test_Day:2016-10-24_Cloud.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json` & `wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.sections.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt` & `wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Desktop.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json` & `wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.sections.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt` & `wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Installation.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json` & `wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.sections.json`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt` & `wikitcms-2.6.9/tests/data/Test_Results:Fedora_32_Branched_20200322.n.0_Server.txt`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_event.py` & `wikitcms-2.6.9/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_helpers.py` & `wikitcms-2.6.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_listing.py` & `wikitcms-2.6.9/tests/test_listing.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_page.py` & `wikitcms-2.6.9/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_release.py` & `wikitcms-2.6.9/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_result.py` & `wikitcms-2.6.9/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `wikitcms-2.6.8/tests/test_wiki.py` & `wikitcms-2.6.9/tests/test_wiki.py`

 * *Files identical despite different names*

