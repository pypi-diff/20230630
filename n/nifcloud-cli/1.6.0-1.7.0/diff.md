# Comparing `tmp/nifcloud-cli-1.6.0.tar.gz` & `tmp/nifcloud-cli-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifcloud-cli-1.6.0.tar", last modified: Thu Apr 20 07:41:54 2023, max compression
+gzip compressed data, was "nifcloud-cli-1.7.0.tar", last modified: Fri Jun 30 02:13:47 2023, max compression
```

## Comparing `nifcloud-cli-1.6.0.tar` & `nifcloud-cli-1.7.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/bin/nifcloud
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 07:41:54.000000 nifcloud-cli-1.6.0/nifcloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/clidriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/customizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/addmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/customizations/waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/_retry.json
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/cli.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.496480 nifcloud-cli-1.6.0/nifcloudcli/data/computing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/
--rw-r--r--   0 runner    (1001) docker     (123)   753203 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.496480 nifcloud-cli-1.6.0/nifcloudcli/data/dns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/endpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/ess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/
--rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/
--rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/nas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/
--rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/
--rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/script/2015-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/script/2015-09-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/2020-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.500480 nifcloud-cli-1.6.0/nifcloudcli/data/storage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/data/storage/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/data/storage/2006-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/nifcloudcli/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/nifcloudcli/topics/topic-tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-20 07:41:54.504480 nifcloud-cli-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-20 07:41:43.000000 nifcloud-cli-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/bin/nifcloud
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-30 02:13:47.000000 nifcloud-cli-1.7.0/nifcloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-30 02:13:47.000000 nifcloud-cli-1.7.0/nifcloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 02:13:47.000000 nifcloud-cli-1.7.0/nifcloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 02:13:47.000000 nifcloud-cli-1.7.0/nifcloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 02:13:47.000000 nifcloud-cli-1.7.0/nifcloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.533947 nifcloud-cli-1.7.0/nifcloudcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/clidriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.533947 nifcloud-cli-1.7.0/nifcloudcli/customizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.533947 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/addmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/customizations/waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.533947 nifcloud-cli-1.7.0/nifcloudcli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/_retry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/cli.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/computing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.533947 nifcloud-cli-1.7.0/nifcloudcli/data/computing/3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   756272 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/computing/3.0/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/computing/3.0/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/dns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/endpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/ess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    22706 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/hatoba/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/hatoba/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)   107780 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/hatoba/v1/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/hatoba/v1/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/nas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/nas/N2016-02-24/
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/nas/N2016-02-24/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/rdb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/
+-rw-r--r--   0 runner    (1001) docker     (123)   134534 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/script/2015-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/script/2015-09-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/service-activity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/service-activity/2020-11-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.529947 nifcloud-cli-1.7.0/nifcloudcli/data/storage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/data/storage/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    89861 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/data/storage/2006-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/nifcloudcli/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/nifcloudcli/topics/topic-tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 02:13:47.537947 nifcloud-cli-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-30 02:13:36.000000 nifcloud-cli-1.7.0/setup.py
```

### Comparing `nifcloud-cli-1.6.0/LICENSE` & `nifcloud-cli-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/PKG-INFO` & `nifcloud-cli-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: nifcloud-cli
-Version: 1.6.0
+Version: 1.7.0
 Summary: NIFCLOUD Command-Line Tools
 Home-page: https://github.com/nifcloud/nifcloud-cli
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nifcloud-cli
 
 [![Test](https://github.com/nifcloud/nifcloud-cli/workflows/Test/badge.svg)](https://github.com/nifcloud/nifcloud-cli/actions?query=workflow%3ATest)
 [![PyPI](https://badge.fury.io/py/nifcloud-cli.svg)](https://pypi.org/project/nifcloud-cli)
```

### Comparing `nifcloud-cli-1.6.0/README.md` & `nifcloud-cli-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloud_cli.egg-info/PKG-INFO` & `nifcloud-cli-1.7.0/nifcloud_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: nifcloud-cli
-Version: 1.6.0
+Version: 1.7.0
 Summary: NIFCLOUD Command-Line Tools
 Home-page: https://github.com/nifcloud/nifcloud-cli
 Author: FUJITSU CLOUD TECHNOLOGIES
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nifcloud-cli
 
 [![Test](https://github.com/nifcloud/nifcloud-cli/workflows/Test/badge.svg)](https://github.com/nifcloud/nifcloud-cli/actions?query=workflow%3ATest)
 [![PyPI](https://badge.fury.io/py/nifcloud-cli.svg)](https://pypi.org/project/nifcloud-cli)
```

### Comparing `nifcloud-cli-1.6.0/nifcloud_cli.egg-info/SOURCES.txt` & `nifcloud-cli-1.7.0/nifcloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/clidriver.py` & `nifcloud-cli-1.7.0/nifcloudcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/commands.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/commands.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/addmodel.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/addmodel.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/configure.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/configure.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/get.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/get.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/list.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/list.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/configure/set.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/configure/set.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/customizations/waiters.py` & `nifcloud-cli-1.7.0/nifcloudcli/customizations/waiters.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/_retry.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/cli.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/computing/3.0/service-2.json`

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

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/computing/3.0/waiters-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/computing/3.0/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/dns/2012-12-12N2013-12-16/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/endpoints.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/endpoints.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/ess/2010-12-01N2014-05-28/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/hatoba/v1/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/hatoba/v1/waiters-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/hatoba/v1/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/nas/N2016-02-24/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/nas/N2016-02-24/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/rdb/2013-05-15N2013-12-16/waiters-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/script/2015-09-01/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/script/2015-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/service-activity/2020-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/data/storage/2006-03-01/service-2.json` & `nifcloud-cli-1.7.0/nifcloudcli/data/storage/2006-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/nifcloudcli/link.py` & `nifcloud-cli-1.7.0/nifcloudcli/link.py`

 * *Files identical despite different names*

### Comparing `nifcloud-cli-1.6.0/setup.py` & `nifcloud-cli-1.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,23 +52,25 @@
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='FUJITSU CLOUD TECHNOLOGIES',
     url='https://github.com/nifcloud/nifcloud-cli',
     packages=find_packages(exclude=['tests*']),
     package_data={'nifcloudcli': ['data/*.json', 'topics/*.json']},
     include_package_data=True,
-    install_requires=['nifcloud==1.6.0', 'awscli==1.20.43'],
+    install_requires=['nifcloud==1.7.0', 'awscli==1.20.43'],
     license='Apache License 2.0',
     classifiers=(
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ),
     scripts=['bin/nifcloud'],
     **cx_freeze_opts,
 )
```

