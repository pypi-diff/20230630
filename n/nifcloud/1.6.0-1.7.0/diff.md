# Comparing `tmp/nifcloud-1.6.0.tar.gz` & `tmp/nifcloud-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifcloud-1.6.0.tar", last modified: Thu Apr 20 07:28:35 2023, max compression
+gzip compressed data, was "nifcloud-1.7.0.tar", last modified: Fri Jun 30 01:56:48 2023, max compression
```

## Comparing `nifcloud-1.6.0.tar` & `nifcloud-1.7.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-20 07:28:24.000000 nifcloud-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-20 07:28:35.541945 nifcloud-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-20 07:28:24.000000 nifcloud-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/configprovider.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/_retry.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.533945 nifcloud-1.6.0/nifcloud/data/computing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/computing/3.0/
--rw-r--r--   0 runner    (1001) docker     (123)   753203 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/computing/3.0/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/computing/3.0/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.533945 nifcloud-1.6.0/nifcloud/data/dns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/dns/2012-12-12N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/endpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.533945 nifcloud-1.6.0/nifcloud/data/ess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/ess/2010-12-01N2014-05-28/
--rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.533945 nifcloud-1.6.0/nifcloud/data/hatoba/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/data/hatoba/v1/
--rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/hatoba/v1/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/hatoba/v1/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.533945 nifcloud-1.6.0/nifcloud/data/nas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/data/nas/N2016-02-24/
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/nas/N2016-02-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/nas/N2016-02-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/rdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/data/rdb/2013-05-15N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/data/script/2015-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/script/2015-09-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/service-activity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/data/service-activity/2020-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/service-activity/2020-11-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud/data/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/data/storage/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/data/storage/2006-03-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.541945 nifcloud-1.6.0/nifcloud/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-20 07:28:24.000000 nifcloud-1.6.0/nifcloud/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:28:35.537945 nifcloud-1.6.0/nifcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-20 07:28:35.000000 nifcloud-1.6.0/nifcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-20 07:28:35.000000 nifcloud-1.6.0/nifcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:28:35.000000 nifcloud-1.6.0/nifcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 07:28:35.000000 nifcloud-1.6.0/nifcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 07:28:35.000000 nifcloud-1.6.0/nifcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-20 07:28:35.541945 nifcloud-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-20 07:28:24.000000 nifcloud-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 01:56:39.000000 nifcloud-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-30 01:56:48.695919 nifcloud-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-30 01:56:39.000000 nifcloud-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/configprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/_retry.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/computing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/computing/3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   756272 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/computing/3.0/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/computing/3.0/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/dns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/dns/2012-12-12N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/endpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/ess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/ess/2010-12-01N2014-05-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/hatoba/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/hatoba/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/hatoba/v1/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/hatoba/v1/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.687919 nifcloud-1.7.0/nifcloud/data/nas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/rdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/script/2015-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/script/2015-09-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/service-activity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/service-activity/2020-11-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/service-activity/2020-11-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud/data/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/data/storage/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/data/storage/2006-03-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.695919 nifcloud-1.7.0/nifcloud/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-30 01:56:39.000000 nifcloud-1.7.0/nifcloud/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:56:48.691919 nifcloud-1.7.0/nifcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 01:56:48.000000 nifcloud-1.7.0/nifcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 01:56:48.695919 nifcloud-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-30 01:56:39.000000 nifcloud-1.7.0/setup.py
```

### Comparing `nifcloud-1.6.0/LICENSE.txt` & `nifcloud-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/PKG-INFO` & `nifcloud-1.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifcloud
-Version: 1.6.0
+Version: 1.7.0
 Summary: Data-driven NIFCLOUD SDK for Python
 Home-page: https://github.com/nifcloud/nifcloud-sdk-python
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,14 +16,18 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NIFCLOUD SDK for Python
 
 [![Test](https://github.com/nifcloud/nifcloud-sdk-python/workflows/Test/badge.svg)](https://github.com/nifcloud/nifcloud-sdk-python/actions?query=workflow%3ATest)
 [![Documentation](https://readthedocs.org/projects/nifcloud-sdk-python/badge)](https://nifcloud-sdk-python.readthedocs.io/en/latest/)
```

### Comparing `nifcloud-1.6.0/README.md` & `nifcloud-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/_retry.json` & `nifcloud-1.7.0/nifcloud/data/_retry.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/computing/3.0/service-2.json` & `nifcloud-1.7.0/nifcloud/data/computing/3.0/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992310919822988%*

 * *Differences: {"'shapes'": "{'Expectation': {'members': {'HttpCode': {'shape': 'String'}}}, 'NetworkInterfaces': "*

 * *             "{'members': {'SystemIpAddresses': OrderedDict([('locationName', "*

 * *             "'SystemIpAddresses'), ('shape', 'ListOfSystemIpAddresses')])}}, "*

 * *             "'NiftyReplaceElasticLoadBalancerLatestVersionRequest': {'members': "*

 * *             "{'NetworkInterface': OrderedDict([('locationName', 'NetworkInterface'), ('shape', "*

 * *             "'ListOfRequestNetworkInterfaceOfNiftyReplaceElasticLoadB […]*

```diff
@@ -9146,15 +9146,15 @@
             "name": "EncryptionAlgorithmOfNiftyIpsecConfigurationForCreateVpnConnection",
             "type": "string"
         },
         "Expectation": {
             "members": {
                 "HttpCode": {
                     "locationName": "HttpCode",
-                    "shape": "Integer"
+                    "shape": "String"
                 }
             },
             "name": "Expectation",
             "type": "structure"
         },
         "ExtendVolumeSizeRequest": {
             "members": {
@@ -9492,14 +9492,25 @@
                     "locationName": "UnhealthyThreshold",
                     "shape": "Integer"
                 }
             },
             "name": "HealthCheckOfNiftyDescribeElasticLoadBalancers",
             "type": "structure"
         },
+        "HttpCodeOfListenersForNiftyCreateElasticLoadBalancer": {
+            "enum": [
+                "1xx",
+                "2xx",
+                "3xx",
+                "4xx",
+                "5xx"
+            ],
+            "name": "HttpCodeOfListenersForNiftyCreateElasticLoadBalancer",
+            "type": "string"
+        },
         "IPAddresses": {
             "members": {
                 "IPAddress": {
                     "locationName": "IPAddress",
                     "shape": "String"
                 }
             },
@@ -13646,14 +13657,22 @@
             "member": {
                 "locationName": "member",
                 "shape": "RequestExpectation"
             },
             "name": "ListOfRequestExpectation",
             "type": "list"
         },
+        "ListOfRequestExpectationOfNiftyCreateElasticLoadBalancer": {
+            "member": {
+                "locationName": "member",
+                "shape": "RequestExpectationOfNiftyCreateElasticLoadBalancer"
+            },
+            "name": "ListOfRequestExpectationOfNiftyCreateElasticLoadBalancer",
+            "type": "list"
+        },
         "ListOfRequestFilter": {
             "member": {
                 "shape": "RequestFilter"
             },
             "name": "ListOfRequestFilter",
             "type": "list"
         },
@@ -14085,14 +14104,21 @@
         "ListOfRequestNetworkInterfaceOfNiftyCreateRouter": {
             "member": {
                 "shape": "RequestNetworkInterfaceOfNiftyCreateRouter"
             },
             "name": "ListOfRequestNetworkInterfaceOfNiftyCreateRouter",
             "type": "list"
         },
+        "ListOfRequestNetworkInterfaceOfNiftyReplaceElasticLoadBalancerLatestVersion": {
+            "member": {
+                "shape": "RequestNetworkInterfaceOfNiftyReplaceElasticLoadBalancerLatestVersion"
+            },
+            "name": "ListOfRequestNetworkInterfaceOfNiftyReplaceElasticLoadBalancerLatestVersion",
+            "type": "list"
+        },
         "ListOfRequestNetworkInterfaceOfNiftyUpdateRouterNetworkInterfaces": {
             "member": {
                 "shape": "RequestNetworkInterfaceOfNiftyUpdateRouterNetworkInterfaces"
             },
             "name": "ListOfRequestNetworkInterfaceOfNiftyUpdateRouterNetworkInterfaces",
             "type": "list"
         },
@@ -14323,14 +14349,21 @@
         "ListOfRequestSnapshotName": {
             "member": {
                 "shape": "String"
             },
             "name": "ListOfRequestSnapshotName",
             "type": "list"
         },
+        "ListOfRequestSystemIpAddresses": {
+            "member": {
+                "shape": "RequestSystemIpAddresses"
+            },
+            "name": "ListOfRequestSystemIpAddresses",
+            "type": "list"
+        },
         "ListOfRequestTenancy": {
             "member": {
                 "shape": "String"
             },
             "name": "ListOfRequestTenancy",
             "type": "list"
         },
@@ -14611,14 +14644,22 @@
             "member": {
                 "locationName": "item",
                 "shape": "StoppedScaleOutOsSet"
             },
             "name": "ListOfStoppedScaleOutOsSet",
             "type": "list"
         },
+        "ListOfSystemIpAddresses": {
+            "member": {
+                "locationName": "member",
+                "shape": "SystemIpAddresses"
+            },
+            "name": "ListOfSystemIpAddresses",
+            "type": "list"
+        },
         "ListOfTagSet": {
             "member": {
                 "locationName": "item",
                 "shape": "TagSet"
             },
             "name": "ListOfTagSet",
             "type": "list"
@@ -17167,14 +17208,18 @@
                 "NetworkId": {
                     "locationName": "NetworkId",
                     "shape": "String"
                 },
                 "NetworkName": {
                     "locationName": "NetworkName",
                     "shape": "String"
+                },
+                "SystemIpAddresses": {
+                    "locationName": "SystemIpAddresses",
+                    "shape": "ListOfSystemIpAddresses"
                 }
             },
             "name": "NetworkInterfaces",
             "type": "structure"
         },
         "NextMonthAccountingType": {
             "members": {
@@ -20491,14 +20536,18 @@
                 "ElasticLoadBalancerId": {
                     "locationName": "ElasticLoadBalancerId",
                     "shape": "String"
                 },
                 "ElasticLoadBalancerName": {
                     "locationName": "ElasticLoadBalancerName",
                     "shape": "String"
+                },
+                "NetworkInterface": {
+                    "locationName": "NetworkInterface",
+                    "shape": "ListOfRequestNetworkInterfaceOfNiftyReplaceElasticLoadBalancerLatestVersion"
                 }
             },
             "name": "NiftyReplaceElasticLoadBalancerLatestVersionRequest",
             "type": "structure"
         },
         "NiftyReplaceElasticLoadBalancerLatestVersionResultWrapper": {
             "members": {
@@ -23600,20 +23649,30 @@
             "name": "RequestElasticLoadBalancers",
             "type": "structure"
         },
         "RequestExpectation": {
             "members": {
                 "HttpCode": {
                     "locationName": "HttpCode",
-                    "shape": "Integer"
+                    "shape": "String"
                 }
             },
             "name": "RequestExpectation",
             "type": "structure"
         },
+        "RequestExpectationOfNiftyCreateElasticLoadBalancer": {
+            "members": {
+                "HttpCode": {
+                    "locationName": "HttpCode",
+                    "shape": "HttpCodeOfListenersForNiftyCreateElasticLoadBalancer"
+                }
+            },
+            "name": "RequestExpectationOfNiftyCreateElasticLoadBalancer",
+            "type": "structure"
+        },
         "RequestFilter": {
             "members": {
                 "ListOfRequestValue": {
                     "locationName": "Value",
                     "shape": "ListOfRequestValue"
                 },
                 "Name": {
@@ -23928,15 +23987,15 @@
             "members": {
                 "Interval": {
                     "locationName": "Interval",
                     "shape": "Integer"
                 },
                 "ListOfRequestExpectation": {
                     "locationName": "Expectation",
-                    "shape": "ListOfRequestExpectation"
+                    "shape": "ListOfRequestExpectationOfNiftyCreateElasticLoadBalancer"
                 },
                 "Path": {
                     "locationName": "Path",
                     "shape": "String"
                 },
                 "Target": {
                     "locationName": "Target",
@@ -24552,14 +24611,18 @@
                     "locationName": "IpAddress",
                     "shape": "String"
                 },
                 "IsVipNetwork": {
                     "locationName": "IsVipNetwork",
                     "shape": "Boolean"
                 },
+                "ListOfRequestSystemIpAddresses": {
+                    "locationName": "SystemIpAddresses",
+                    "shape": "ListOfRequestSystemIpAddresses"
+                },
                 "NetworkId": {
                     "locationName": "NetworkId",
                     "shape": "String"
                 },
                 "NetworkName": {
                     "locationName": "NetworkName",
                     "shape": "String"
@@ -24602,14 +24665,28 @@
                     "locationName": "NetworkName",
                     "shape": "String"
                 }
             },
             "name": "RequestNetworkInterfaceOfNiftyCreateRouter",
             "type": "structure"
         },
+        "RequestNetworkInterfaceOfNiftyReplaceElasticLoadBalancerLatestVersion": {
+            "members": {
+                "ListOfRequestSystemIpAddresses": {
+                    "locationName": "SystemIpAddresses",
+                    "shape": "ListOfRequestSystemIpAddresses"
+                },
+                "NetworkId": {
+                    "locationName": "NetworkId",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestNetworkInterfaceOfNiftyReplaceElasticLoadBalancerLatestVersion",
+            "type": "structure"
+        },
         "RequestNetworkInterfaceOfNiftyUpdateRouterNetworkInterfaces": {
             "members": {
                 "DeviceIndex": {
                     "locationName": "DeviceIndex",
                     "shape": "Integer"
                 },
                 "Dhcp": {
@@ -25322,14 +25399,24 @@
                     "locationName": "Method",
                     "shape": "MethodOfLoadBalancerAttributesForNiftyModifyElasticLoadBalancerAttributes"
                 }
             },
             "name": "RequestStickinessPolicyOfNiftyModifyElasticLoadBalancerAttributes",
             "type": "structure"
         },
+        "RequestSystemIpAddresses": {
+            "members": {
+                "SystemIpAddress": {
+                    "locationName": "SystemIpAddress",
+                    "shape": "String"
+                }
+            },
+            "name": "RequestSystemIpAddresses",
+            "type": "structure"
+        },
         "RequestTimeZone": {
             "members": {
                 "EndingTimeZone": {
                     "locationName": "EndingTimeZone",
                     "shape": "String"
                 },
                 "StartingTimeZone": {
@@ -27132,14 +27219,24 @@
             "name": "StoppedScaleOutOsSet",
             "type": "structure"
         },
         "String": {
             "name": "String",
             "type": "string"
         },
+        "SystemIpAddresses": {
+            "members": {
+                "SystemIpAddress": {
+                    "locationName": "SystemIpAddress",
+                    "shape": "String"
+                }
+            },
+            "name": "SystemIpAddresses",
+            "type": "structure"
+        },
         "TStamp": {
             "name": "TStamp",
             "type": "timestamp"
         },
         "TagSet": {
             "members": {
                 "Key": {
```

### Comparing `nifcloud-1.6.0/nifcloud/data/computing/3.0/waiters-2.json` & `nifcloud-1.7.0/nifcloud/data/computing/3.0/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json` & `nifcloud-1.7.0/nifcloud/data/dns/2012-12-12N2013-12-16/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/endpoints.json` & `nifcloud-1.7.0/nifcloud/data/endpoints.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json` & `nifcloud-1.7.0/nifcloud/data/ess/2010-12-01N2014-05-28/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/hatoba/v1/service-2.json` & `nifcloud-1.7.0/nifcloud/data/hatoba/v1/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/hatoba/v1/waiters-2.json` & `nifcloud-1.7.0/nifcloud/data/hatoba/v1/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/nas/N2016-02-24/service-2.json` & `nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/nas/N2016-02-24/waiters-2.json` & `nifcloud-1.7.0/nifcloud/data/nas/N2016-02-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json` & `nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json` & `nifcloud-1.7.0/nifcloud/data/rdb/2013-05-15N2013-12-16/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/script/2015-09-01/service-2.json` & `nifcloud-1.7.0/nifcloud/data/script/2015-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/service-activity/2020-11-25/service-2.json` & `nifcloud-1.7.0/nifcloud/data/service-activity/2020-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/data/storage/2006-03-01/service-2.json` & `nifcloud-1.7.0/nifcloud/data/storage/2006-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/docs/__init__.py` & `nifcloud-1.7.0/nifcloud/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/parsers.py` & `nifcloud-1.7.0/nifcloud/parsers.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/serialize.py` & `nifcloud-1.7.0/nifcloud/serialize.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud/session.py` & `nifcloud-1.7.0/nifcloud/session.py`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/nifcloud.egg-info/PKG-INFO` & `nifcloud-1.7.0/nifcloud.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifcloud
-Version: 1.6.0
+Version: 1.7.0
 Summary: Data-driven NIFCLOUD SDK for Python
 Home-page: https://github.com/nifcloud/nifcloud-sdk-python
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,14 +16,18 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NIFCLOUD SDK for Python
 
 [![Test](https://github.com/nifcloud/nifcloud-sdk-python/workflows/Test/badge.svg)](https://github.com/nifcloud/nifcloud-sdk-python/actions?query=workflow%3ATest)
 [![Documentation](https://readthedocs.org/projects/nifcloud-sdk-python/badge)](https://nifcloud-sdk-python.readthedocs.io/en/latest/)
```

### Comparing `nifcloud-1.6.0/nifcloud.egg-info/SOURCES.txt` & `nifcloud-1.7.0/nifcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifcloud-1.6.0/setup.py` & `nifcloud-1.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,9 +49,13 @@
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ),
 )
```

