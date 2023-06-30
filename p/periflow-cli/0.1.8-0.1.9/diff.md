# Comparing `tmp/periflow-cli-0.1.8.tar.gz` & `tmp/periflow-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow-cli-0.1.8.tar", last modified: Fri Nov 25 06:13:37 2022, max compression
+gzip compressed data, was "periflow-cli-0.1.9.tar", last modified: Wed Nov 30 01:12:34 2022, max compression
```

## Comparing `periflow-cli-0.1.8.tar` & `periflow-cli-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.566959 periflow-cli-0.1.8/
--rw-r--r--   0 yunmokoo   (501) staff       (20)    11357 2022-07-01 01:38:21.000000 periflow-cli-0.1.8/LICENSE
--rw-r--r--   0 yunmokoo   (501) staff       (20)       16 2022-07-01 01:38:21.000000 periflow-cli-0.1.8/MANIFEST.in
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7656 2022-11-25 06:13:37.566795 periflow-cli-0.1.8/PKG-INFO
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7242 2022-11-25 06:07:11.000000 periflow-cli-0.1.8/README.md
--rw-r--r--   0 yunmokoo   (501) staff       (20)        6 2022-11-25 06:07:11.000000 periflow-cli-0.1.8/VERSION
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.558723 periflow-cli-0.1.8/periflow_cli.egg-info/
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7656 2022-11-25 06:13:37.000000 periflow-cli-0.1.8/periflow_cli.egg-info/PKG-INFO
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1154 2022-11-25 06:13:37.000000 periflow-cli-0.1.8/periflow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 yunmokoo   (501) staff       (20)        1 2022-11-25 06:13:37.000000 periflow-cli-0.1.8/periflow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 yunmokoo   (501) staff       (20)       33 2022-11-25 06:13:37.000000 periflow-cli-0.1.8/periflow_cli.egg-info/entry_points.txt
--rw-r--r--   0 yunmokoo   (501) staff       (20)      412 2022-11-25 06:13:37.000000 periflow-cli-0.1.8/periflow_cli.egg-info/requires.txt
--rw-r--r--   0 yunmokoo   (501) staff       (20)        6 2022-11-25 06:13:37.000000 periflow-cli-0.1.8/periflow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.561854 periflow-cli-0.1.8/pfcli/
--rw-r--r--   0 yunmokoo   (501) staff       (20)      105 2022-07-01 01:38:21.000000 periflow-cli-0.1.8/pfcli/__init__.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1554 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/artifact.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     4394 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/billing.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     8516 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/checkpoint.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1086 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/context.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     8948 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/credential.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)    13278 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/dataset.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7762 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/deployment.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     3843 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/group.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)    22635 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/job.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7095 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/main.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7133 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/project.py
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.562762 periflow-cli-0.1.8/pfcli/service/
--rw-r--r--   0 yunmokoo   (501) staff       (20)     8202 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/__init__.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     3457 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/auth.py
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.564821 periflow-cli-0.1.8/pfcli/service/client/
--rw-r--r--   0 yunmokoo   (501) staff       (20)     5534 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/client/__init__.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     5753 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/client/base.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1316 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/client/billing.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     3174 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/client/checkpoint.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1887 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/client/credential.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)    13615 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/client/data.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1036 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/client/deployment.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7145 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/client/group.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)    10203 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/client/job.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     2619 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/client/metrics.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     6086 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/client/project.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     4058 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/client/user.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     4430 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/cloud.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)    20079 2022-11-25 02:46:07.000000 periflow-cli-0.1.8/pfcli/service/config.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     7812 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/service/formatter.py
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.566325 periflow-cli-0.1.8/pfcli/utils/
--rw-r--r--   0 yunmokoo   (501) staff       (20)        0 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/__init__.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     2724 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/format.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     5166 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/fs.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)      554 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/prompt.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1923 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/request.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1213 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/url.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     1846 2022-11-25 02:38:33.000000 periflow-cli-0.1.8/pfcli/utils/validate.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)     8166 2022-11-25 06:07:11.000000 periflow-cli-0.1.8/pfcli/vm.py
--rw-r--r--   0 yunmokoo   (501) staff       (20)       38 2022-11-25 06:13:37.567002 periflow-cli-0.1.8/setup.cfg
--rw-r--r--   0 yunmokoo   (501) staff       (20)     2292 2022-09-07 07:03:51.000000 periflow-cli-0.1.8/setup.py
-drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-25 06:13:37.566603 periflow-cli-0.1.8/test/
--rw-r--r--   0 yunmokoo   (501) staff       (20)        0 2022-07-01 01:38:21.000000 periflow-cli-0.1.8/test/test_utils.py
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.573608 periflow-cli-0.1.9/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    11357 2022-07-01 01:38:21.000000 periflow-cli-0.1.9/LICENSE
+-rw-r--r--   0 yunmokoo   (501) staff       (20)       16 2022-07-01 01:38:21.000000 periflow-cli-0.1.9/MANIFEST.in
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7656 2022-11-30 01:12:34.573420 periflow-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7242 2022-11-25 06:07:11.000000 periflow-cli-0.1.9/README.md
+-rw-r--r--   0 yunmokoo   (501) staff       (20)        6 2022-11-30 01:10:58.000000 periflow-cli-0.1.9/VERSION
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.564964 periflow-cli-0.1.9/periflow_cli.egg-info/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7656 2022-11-30 01:12:34.000000 periflow-cli-0.1.9/periflow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1154 2022-11-30 01:12:34.000000 periflow-cli-0.1.9/periflow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 yunmokoo   (501) staff       (20)        1 2022-11-30 01:12:34.000000 periflow-cli-0.1.9/periflow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 yunmokoo   (501) staff       (20)       33 2022-11-30 01:12:34.000000 periflow-cli-0.1.9/periflow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 yunmokoo   (501) staff       (20)      412 2022-11-30 01:12:34.000000 periflow-cli-0.1.9/periflow_cli.egg-info/requires.txt
+-rw-r--r--   0 yunmokoo   (501) staff       (20)        6 2022-11-30 01:12:34.000000 periflow-cli-0.1.9/periflow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.568425 periflow-cli-0.1.9/pfcli/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)      105 2022-07-01 01:38:21.000000 periflow-cli-0.1.9/pfcli/__init__.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1554 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/artifact.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     4394 2022-11-25 02:46:07.000000 periflow-cli-0.1.9/pfcli/billing.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     8997 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/checkpoint.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1086 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/context.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     8948 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/credential.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    13403 2022-11-25 08:06:02.000000 periflow-cli-0.1.9/pfcli/dataset.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    11059 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/deployment.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     3938 2022-11-30 00:24:39.000000 periflow-cli-0.1.9/pfcli/group.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    22639 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/job.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7089 2022-11-30 00:24:39.000000 periflow-cli-0.1.9/pfcli/main.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7686 2022-11-30 00:24:39.000000 periflow-cli-0.1.9/pfcli/project.py
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.569374 periflow-cli-0.1.9/pfcli/service/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     8361 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/service/__init__.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     3457 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/auth.py
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.571821 periflow-cli-0.1.9/pfcli/service/client/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     5918 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/service/client/__init__.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     5753 2022-11-25 07:50:28.000000 periflow-cli-0.1.9/pfcli/service/client/base.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1316 2022-11-25 02:46:07.000000 periflow-cli-0.1.9/pfcli/service/client/billing.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     3174 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/client/checkpoint.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1887 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/client/credential.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    13615 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/client/data.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1956 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/service/client/deployment.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7145 2022-11-25 02:46:07.000000 periflow-cli-0.1.9/pfcli/service/client/group.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    10203 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/client/job.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     2619 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/client/metrics.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     6125 2022-11-25 08:06:02.000000 periflow-cli-0.1.9/pfcli/service/client/project.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     4325 2022-11-30 00:24:39.000000 periflow-cli-0.1.9/pfcli/service/client/user.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     4430 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/cloud.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)    19660 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/service/config.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     7812 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/service/formatter.py
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.573059 periflow-cli-0.1.9/pfcli/utils/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)        0 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/utils/__init__.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     2680 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/utils/format.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     5166 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/utils/fs.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)      554 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/utils/prompt.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1923 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/utils/request.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1225 2022-11-30 01:06:07.000000 periflow-cli-0.1.9/pfcli/utils/url.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     1846 2022-11-25 02:38:33.000000 periflow-cli-0.1.9/pfcli/utils/validate.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     8166 2022-11-25 06:07:11.000000 periflow-cli-0.1.9/pfcli/vm.py
+-rw-r--r--   0 yunmokoo   (501) staff       (20)       38 2022-11-30 01:12:34.573655 periflow-cli-0.1.9/setup.cfg
+-rw-r--r--   0 yunmokoo   (501) staff       (20)     2292 2022-09-07 07:03:51.000000 periflow-cli-0.1.9/setup.py
+drwxr-xr-x   0 yunmokoo   (501) staff       (20)        0 2022-11-30 01:12:34.573212 periflow-cli-0.1.9/test/
+-rw-r--r--   0 yunmokoo   (501) staff       (20)        0 2022-07-01 01:38:21.000000 periflow-cli-0.1.9/test/test_utils.py
```

### Comparing `periflow-cli-0.1.8/LICENSE` & `periflow-cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/PKG-INFO` & `periflow-cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: PeriFlow CLI
 Home-page: https://github.com/friendliai/periflow-cli
 Author: FriendliAI
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
```

### Comparing `periflow-cli-0.1.8/README.md` & `periflow-cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/periflow_cli.egg-info/PKG-INFO` & `periflow-cli-0.1.9/periflow_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: PeriFlow CLI
 Home-page: https://github.com/friendliai/periflow-cli
 Author: FriendliAI
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
```

### Comparing `periflow-cli-0.1.8/periflow_cli.egg-info/SOURCES.txt` & `periflow-cli-0.1.9/periflow_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/artifact.py` & `periflow-cli-0.1.9/pfcli/artifact.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/billing.py` & `periflow-cli-0.1.9/pfcli/billing.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/checkpoint.py` & `periflow-cli-0.1.9/pfcli/checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2021 FriendliAI
 
 """CLI for Checkpoint"""
 
 import os
+from click import secho
 from dateutil.parser import parse
 from typing import Optional, List
 from uuid import UUID
 
 import typer
 
 from pfcli.service import (
@@ -78,14 +79,31 @@
         "Iteration",
         "Format",
         "Created At",
     ],
 )
 tree_formatter = TreeFormatter(name="Files")
 
+model_info_panel = PanelFormatter(
+    name="Model Info",
+    fields=[
+        "head_size",
+        "num_heads",
+        "num_layers",
+        "max_length",
+        "vocab_size",
+    ],
+    headers=[
+        "Head Size",
+        "#Heads",
+        "#Layers",
+        "Max Length",
+        "Vocab Size",
+    ]
+)
 
 @app.command()
 def list(
     category: Optional[CheckpointCategory] = typer.Option(
         None,
         "--category",
         "-c",
@@ -115,14 +133,19 @@
     client: CheckpointClientService = build_client(ServiceType.CHECKPOINT)
     ckpt = client.get_checkpoint(checkpoint_id)
     for form in ckpt["forms"]:
         form["vendor"] = storage_type_map_inv[form["vendor"]].value
     ckpt["created_at"] = datetime_to_pretty_str(parse(ckpt["created_at"]))
 
     panel_formatter.render([ckpt])
+
+    # serving model info.
+    if "attributes" in ckpt and "head_size" in ckpt["attributes"]:
+        model_info_panel.render(ckpt["attributes"])
+
     tree_formatter.render(ckpt["forms"][0]["files"])
 
 
 @app.command()
 def create(
     name: str = typer.Option(
         ..., "--name", "-n", help="Name of your checkpoint to create."
```

### Comparing `periflow-cli-0.1.8/pfcli/context.py` & `periflow-cli-0.1.9/pfcli/context.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/credential.py` & `periflow-cli-0.1.9/pfcli/credential.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/dataset.py` & `periflow-cli-0.1.9/pfcli/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,22 @@
     if metadata_file is not None:
         try:
             metadata = yaml.safe_load(metadata_file)
         except yaml.YAMLError as exc:
             secho_error_and_exit(f"Error occurred while parsing metadata file... {exc}")
 
     dataset = project_client.create_dataset(
-        name, StorageType.FAI, "", "", None, metadata, [], False
+        name=name,
+        vendor=StorageType.FAI,
+        region="",
+        storage_name="",
+        credential_id=None,
+        metadata=metadata,
+        files=[],
+        active=False,
     )
     dataset_id = dataset["id"]
 
     try:
         typer.echo(f"Start uploading objects to dataset ({name})...")
         spu_targets = expand_paths(src_path, expand, FileSizeType.SMALL)
         mpu_targets = expand_paths(src_path, expand, FileSizeType.LARGE)
```

### Comparing `periflow-cli-0.1.8/pfcli/deployment.py` & `periflow-cli-0.1.9/pfcli/deployment.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,39 @@
 
 from dateutil.parser import parse
 from typing import Optional
 
 import ruamel.yaml
 import typer
 import yaml
-from click import Choice
+from uuid import UUID
+import datetime
 
 from pfcli.service import (
+    DeploymentType,
     ServiceType,
     GpuType,
     CloudType,
     EngineType,
 )
 from pfcli.service.client import (
     DeploymentClientService,
     build_client,
 )
+from pfcli.context import get_current_project_id
+from pfcli.service.client.deployment import (
+    DeploymentMetricsClientService,
+    PFSProjectUsageClientService,
+)
 from pfcli.service.config import build_deployment_configurator
 from pfcli.service.formatter import PanelFormatter, TableFormatter
-from pfcli.utils.format import datetime_to_pretty_str, secho_error_and_exit
+from pfcli.utils.format import (
+    datetime_to_pretty_str,
+    secho_error_and_exit,
+)
 from pfcli.utils.prompt import get_default_editor, open_editor
 
 
 app = typer.Typer(
     no_args_is_help=True,
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
@@ -36,26 +46,37 @@
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
 )
 
 app.add_typer(template_app, name="template", help="Manage deployment templates.")
 
 deployment_panel = PanelFormatter(
-    name="Overview",
+    name="Deployment Overview",
     fields=[
         "id",
         "config.name",
+        "config.deployment_type",
         "status",
         "vms",
         "config.gpu_type",
         "config.total_gpus",
         "start",
         "endpoint",
     ],
-    headers=["ID", "Name", "Status", "VM", "Device", "Device Cnt", "Start", "Endpoint"],
+    headers=[
+        "ID",
+        "Name",
+        "Type",
+        "Status",
+        "VM Type",
+        "GPU Type",
+        "#GPUs",
+        "Start",
+        "Endpoint",
+    ],
     extra_fields=["error"],
     extra_headers=["error"],
 )
 
 deployment_table = TableFormatter(
     name="Deployments",
     fields=[
@@ -63,19 +84,42 @@
         "config.name",
         "status",
         "vms",
         "config.gpu_type",
         "config.total_gpus",
         "start",
     ],
-    headers=["ID", "Name", "Status", "VM", "Device", "Device Cnt", "Start"],
+    headers=["ID", "Name", "Status", "VM Type", "GPU Type", "#GPUs", "Start"],
+    extra_fields=["error"],
+    extra_headers=["error"],
+)
+
+deployment_metrics_table = TableFormatter(
+    name="Deployment Metrics",
+    fields=[
+        "id",
+        "latency",
+        "throughput",
+        "time_window",
+    ],
+    headers=["ID", "Latency(ms)", "Throughput(req/s)", "Time Window(sec)"],
     extra_fields=["error"],
     extra_headers=["error"],
 )
 
+deployment_usage_table = TableFormatter(
+    name="Deployment Usage",
+    fields=[
+        "id",
+        "type",
+        "duration",
+    ],
+    headers=["ID", "Type", "Total Usage (days, HH:MM:SS)"],
+)
+
 deployment_panel.add_substitution_rule("waiting", "[bold]waiting")
 deployment_panel.add_substitution_rule("enqueued", "[bold cyan]enqueued")
 deployment_panel.add_substitution_rule("running", "[bold blue]running")
 deployment_panel.add_substitution_rule("success", "[bold green]success")
 deployment_panel.add_substitution_rule("failed", "[bold red]failed")
 deployment_panel.add_substitution_rule("terminated", "[bold yellow]terminated")
 deployment_panel.add_substitution_rule("terminating", "[bold magenta]terminating")
@@ -86,36 +130,53 @@
 deployment_table.add_substitution_rule("running", "[bold blue]running")
 deployment_table.add_substitution_rule("success", "[bold green]success")
 deployment_table.add_substitution_rule("failed", "[bold red]failed")
 deployment_table.add_substitution_rule("terminated", "[bold yellow]terminated")
 deployment_table.add_substitution_rule("terminating", "[bold magenta]terminating")
 deployment_table.add_substitution_rule("cancelling", "[bold magenta]cancelling")
 
+deployment_metrics_table.add_substitution_rule("waiting", "[bold]waiting")
+deployment_metrics_table.add_substitution_rule("enqueued", "[bold cyan]enqueued")
+deployment_metrics_table.add_substitution_rule("running", "[bold blue]running")
+deployment_metrics_table.add_substitution_rule("success", "[bold green]success")
+deployment_metrics_table.add_substitution_rule("failed", "[bold red]failed")
+deployment_metrics_table.add_substitution_rule("terminated", "[bold yellow]terminated")
+deployment_metrics_table.add_substitution_rule(
+    "terminating", "[bold magenta]terminating"
+)
+deployment_metrics_table.add_substitution_rule("cancelling", "[bold magenta]cancelling")
+
 
 @app.command()
 def list(
     tail: Optional[int] = typer.Option(
         None, "--tail", help="The number of deployment list to view at the tail"
     ),
     head: Optional[int] = typer.Option(
         None, "--head", help="The number of deployment list to view at the head"
     ),
 ):
     """List all deployments."""
+    project_id = get_current_project_id()
+    if project_id is None:
+        secho_error_and_exit("Failed to identify project... Please set project again.")
+
     client: DeploymentClientService = build_client(ServiceType.DEPLOYMENT)
-    deployments = client.list_deployments()["deployments"]
+    deployments = client.list_deployments(str(project_id))["deployments"]
 
     for deployment in deployments:
         started_at = deployment.get("start")
         if started_at is not None:
             start = datetime_to_pretty_str(parse(started_at))
         else:
             start = None
         deployment["start"] = start
-        deployment["vms"] = deployment["vms"][0]["name"]
+        deployment["vms"] = (
+            deployment["vms"][0]["name"] if deployment["vms"] else "None"
+        )
 
     if tail is not None or head is not None:
         target_deployment_list = []
         if tail:
             target_deployment_list.extend(deployments[:tail])
         if head:
             target_deployment_list.extend(deployments[-head:])
@@ -126,14 +187,18 @@
 
 
 @app.command()
 def delete(deployment_id: str = typer.Argument(..., help="ID of deployment to delete")):
     """Delete deployment."""
     client: DeploymentClientService = build_client(ServiceType.DEPLOYMENT)
     client.delete_deployment(deployment_id)
+    typer.secho(
+        f"Deleted Deployment ({deployment_id}) successfully.",
+        fg=typer.colors.BLUE,
+    )
 
 
 @app.command()
 def view(
     deployment_id: str = typer.Argument(..., help="deployment id to inspect detail.")
 ):
     """Show details of a deployment."""
@@ -142,29 +207,62 @@
 
     started_at = deployment.get("start")
     if started_at is not None:
         start = datetime_to_pretty_str(parse(started_at))
     else:
         start = None
     deployment["start"] = start
-    deployment["vms"] = deployment["vms"][0]["name"]
+    deployment["vms"] = deployment["vms"][0]["name"] if deployment["vms"] else "None"
     deployment_panel.render([deployment])
 
 
 @app.command()
-def create(
-    project_id: str = typer.Option(
-        ..., "--project-id", "-pid", help="Project to deploy."
+def metrics(
+    deployment_id: str = typer.Argument(..., help="Deployment id to inspect detail."),
+    time_window: int = typer.Option(
+        60, "--time-window", "-t", help="Time window of metrics in seconds."
     ),
+):
+    """Show metrics of a deployment."""
+    metrics_client: DeploymentMetricsClientService = build_client(
+        ServiceType.DEPLOYMENT_METRICS, deployment_id=deployment_id
+    )
+    metrics = metrics_client.get_metrics(
+        deployment_id=deployment_id, time_window=time_window
+    )
+    metrics["id"] = metrics["deployment_id"]
+    # ns => ms
+    metrics["latency"] = "{:.3f}".format(metrics["latency"] / 1000000) if "latency" in metrics else None
+    metrics["throughput"] = "{:.3f}".format(metrics["throughput"]) if "throughput" in metrics else None
+    deployment_metrics_table.render([metrics])
+
+
+@app.command()
+def usage():
+    """Show total usage of deployments in project."""
+    client: PFSProjectUsageClientService = build_client(ServiceType.PFS_PROJECT_USAGE)
+    usages = client.get_deployment_usage()
+
+    deployments = [
+        {"id": id, "type": info["deployment_type"] , "duration": datetime.timedelta(seconds=int(info["duration"]))}
+        for id, info in usages.items()
+    ]
+    deployment_usage_table.render(deployments)
+
+@app.command()
+def create(
     checkpoint_id: str = typer.Option(
         ..., "--checkpoint-id", "-id", help="Checkpoint id to deploy."
     ),
     deployment_name: str = typer.Option(
         ..., "--name", "-n", help="The name of deployment. "
     ),
+    deployment_type: DeploymentType = typer.Option(
+        ..., "--type", "-t", help="Type of deployment(dev/prod)."
+    ),
     gpu_type: GpuType = typer.Option(
         ..., "--gpu-type", "-g", help="The GPU type where the deployment is deployed."
     ),
     cloud: CloudType = typer.Option(
         ..., "--cloud", "-c", help="Type of cloud(aws, azure, gcp)."
     ),
     region: str = typer.Option(..., "--region", "-r", help="Region of cloud."),
@@ -172,56 +270,59 @@
         EngineType.ORCA, "--engine", "-e", help="Type of engine(orca or triton)."
     ),
     config_file: typer.FileText = typer.Option(
         ..., "--config-file", "-f", help="Path to configuration file."
     ),
 ):
     """Create a deployment object by using model checkpoint."""
+    project_id = get_current_project_id()
+    if project_id is None:
+        secho_error_and_exit("Failed to identify project... Please set project again.")
+
     if engine is not EngineType.ORCA:
         secho_error_and_exit("Only ORCA is supported!")
 
     try:
+        UUID(checkpoint_id)
+    except ValueError:
+        secho_error_and_exit("Checkpoint ID should be in UUID format.")
+
+    try:
         config: dict = yaml.safe_load(config_file)
     except yaml.YAMLError as e:
         secho_error_and_exit(f"Error occurred while parsing engine config file... {e}")
 
     request_data = {
-        "project_id": project_id,
+        "project_id": str(project_id),
         "model_id": checkpoint_id,
+        "deployment_type": deployment_type,
         "name": deployment_name,
         "gpu_type": gpu_type,
         "cloud": cloud,
         "region": region,
         **config,
     }
-    typer.secho(f"request_data: {request_data}")
     client: DeploymentClientService = build_client(ServiceType.DEPLOYMENT)
-    typer.secho(f"deployment url:{client.url_kwargs}")
     deployment = client.create_deployment(request_data)
 
     typer.secho(
-        f"Deployment ({deployment['id']}) started successfully. Use 'pf deployment view <id>' to see the deployment details.\n"
-        f"Run 'curl {deployment['endpoint']}' for inference request",
+        f"Deployment ({deployment['id']}) started successfully. Use 'pf deployment view {deployment['id']}' to see the deployment details.\n"
+        f"Send inference requests to '{deployment['endpoint']}'.",
         fg=typer.colors.BLUE,
     )
 
 
 @template_app.command("create")
-def template_crate(
+def template_create(
     save_path: typer.FileTextWrite = typer.Option(
         ..., "--save-path", "-s", help="Path to save job YAML configruation file."
     )
 ):
     """Create a deployment engine configuration YAML file."""
-    engine_type = typer.prompt(
-        "What kind of engine type do you want?\n",
-        type=Choice([e.value for e in EngineType]),
-        prompt_suffix="\n>> ",
-    )
-    configurator = build_deployment_configurator(engine_type)
+    configurator = build_deployment_configurator(EngineType.ORCA)
     yaml_str = configurator.render()
 
     yaml = ruamel.yaml.YAML()
     code = yaml.load(yaml_str)
     yaml.dump(code, save_path)
 
     continue_edit = typer.confirm(
```

### Comparing `periflow-cli-0.1.8/pfcli/group.py` & `periflow-cli-0.1.9/pfcli/group.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,25 +45,27 @@
 
     org = get_current_org()
 
     if org["privilege_level"] != "owner":
         secho_error_and_exit("Only the owner of the organization can invite/set-role.")
 
     group_client.invite_to_group(org["id"], email)
-    typer.secho("Invitation Successfully Sent!")
+    typer.echo("Invitation Successfully Sent!")
 
 
 @app.command("accept-invite", help="accept invitation")
 def accept_invite(
-    token: str = typer.Option(..., prompt="Enter verification code"),
+    token: str = typer.Option(..., prompt="Enter email token"),
     key: str = typer.Option(..., prompt="Enter verification key"),
 ):
     group_client: GroupClientService = build_client(ServiceType.GROUP)
     group_client.accept_invite(token, key)
-    typer.secho("Verification Success!")
+    typer.echo("Verification Success!")
+    typer.echo("Please login again with: ", nl=False)
+    typer.secho("pf login", fg=typer.colors.BLUE)
 
 
 @app.command("set-role", help="set organization role of the user")
 def set_role(
     username: str = typer.Argument(..., help="Username to set role"),
     role: GroupRole = typer.Argument(..., help="Organization role"),
 ):
@@ -74,15 +76,15 @@
     if org["privilege_level"] != "owner":
         secho_error_and_exit(
             "Only the owner of the organization can invite/set-privilege."
         )
 
     user_id = _get_org_user_id_by_name(org["id"], username)
     user_client.set_group_privilege(org["id"], user_id, role)
-    typer.secho(
+    typer.echo(
         f"Organization role for user ({username}) successfully updated to {role.value}!"
     )
 
 
 def _get_org_user_id_by_name(org_id: UUID, username: str) -> UUID:
     group_client: GroupClientService = build_client(ServiceType.GROUP)
     users = group_client.get_users(org_id, username)
```

### Comparing `periflow-cli-0.1.8/pfcli/job.py` & `periflow-cli-0.1.9/pfcli/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,19 +353,19 @@
         started_at = job.get("started_at")
         finished_at = job.get("finished_at")
         if started_at is not None:
             start = datetime_to_pretty_str(parse(job["started_at"]))
         else:
             start = None
         if started_at is not None and finished_at is not None:
-            duration = timedelta_to_pretty_str(parse(started_at), parse(finished_at))
+            duration = timedelta_to_pretty_str(parse(finished_at) - parse(started_at))
         elif started_at is not None and job["status"] == JobStatus.RUNNING:
             start_time = parse(started_at)
             curr_time = datetime.now(start_time.tzinfo)
-            duration = timedelta_to_pretty_str(start_time, curr_time)
+            duration = timedelta_to_pretty_str(curr_time - start_time)
         else:
             duration = None
 
         job["started_at"] = start
         job["duration"] = duration
         job["data_name"] = (
             job["data_store"]["name"] if job["data_store"] is not None else None
@@ -441,19 +441,19 @@
     started_at = job.get("started_at")
     finished_at = job.get("finished_at")
     if started_at is not None:
         start = datetime_to_pretty_str(parse(job["started_at"]))
     else:
         start = None
     if started_at is not None and finished_at is not None:
-        duration = timedelta_to_pretty_str(parse(started_at), parse(finished_at))
+        duration = timedelta_to_pretty_str(parse(finished_at) - parse(started_at))
     elif started_at is not None and job["status"] == JobStatus.RUNNING:
         start_time = parse(started_at)
         curr_time = datetime.now(start_time.tzinfo)
-        duration = timedelta_to_pretty_str(start_time, curr_time)
+        duration = timedelta_to_pretty_str(curr_time - start_time)
     else:
         duration = None
 
     job["started_at"] = start
     job["duration"] = duration
     job["data_name"] = (
         job["data_store"]["name"] if job["data_store"] is not None else None
```

### Comparing `periflow-cli-0.1.8/pfcli/main.py` & `periflow-cli-0.1.9/pfcli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     client.change_password(old_password, new_password)
 
     typer.secho("Password is changed successfully!", fg=typer.colors.BLUE)
 
 
 def _verify(
     _,
-    token: str = typer.Option(..., prompt="Enter verification code"),
+    token: str = typer.Option(..., prompt="Enter email token"),
     key: str = typer.Option(..., prompt="Enter verification key"),
 ):
     client: UserSignUpService = build_client(ServiceType.SIGNUP)
     client.verify(token, key)
 
     typer.echo("\n\nVerified!")
     typer.echo("Sign up success! Please sign in.")
```

### Comparing `periflow-cli-0.1.8/pfcli/project.py` & `periflow-cli-0.1.9/pfcli/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,15 +176,31 @@
 ):
     user_client: UserClientService = build_client(ServiceType.USER)
 
     org_id, project_id = _check_project_and_get_id()
     user_id = _get_org_user_id_by_name(org_id, username)
 
     user_client.add_to_project(user_id, project_id, role)
-    typer.secho(f"User successfully added to project")
+    typer.secho(f"User is successfully added to project", fg=typer.colors.BLUE)
+
+
+@app.command("delete-user", help="delete user from project")
+def delete_user(
+    username: str = typer.Argument(
+        ...,
+        help="Username to delete from the current working project",
+    ),
+):
+    user_client: UserClientService = build_client(ServiceType.USER)
+
+    org_id, project_id = _check_project_and_get_id()
+    user_id = _get_org_user_id_by_name(org_id, username)
+
+    user_client.delete_from_project(user_id, project_id)
+    typer.secho(f"User is successfully deleted from project", fg=typer.colors.BLUE)
 
 
 @app.command("set-role", help="set project role for a user")
 def set_role(
     username: str = typer.Argument(
         ...,
         help="Username to set project role",
```

### Comparing `periflow-cli-0.1.8/pfcli/service/__init__.py` & `periflow-cli-0.1.9/pfcli/service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     CREDENTIAL_TYPE = "CREDENTIAL_TYPE"
     DATA = "DATA"
     PROJECT_DATA = "PROJECT_DATA"
     CHECKPOINT = "CHECKPOINT"
     GROUP_PROJECT_CHECKPOINT = "GROUP_PROJECT_CHECKPOINT"
     JOB_WS = "JOB_WS"
     DEPLOYMENT = "DEPLOYMENT"
+    DEPLOYMENT_METRICS = "DEPLOYMENT_METRICS"
+    PFS_PROJECT_USAGE = "PFS_PROJECT_USAGE"
     PFT_BILLING_SUMMARY = "BILLING_SUMMARY"
     METRICS = "METRICS"
 
 
 class GroupRole(str, Enum):
     OWNER = "owner"
     MEMBER = "member"
@@ -151,23 +153,27 @@
     MEGATRON = "MEGATRON"
     ORCA = "ORCA"
     HF = "HF"
     ETC = "ETC"
 
 
 class GpuType(str, Enum):
-    T4 = "t4"
-    V100 = "v100"
+    A10G = "a10g"
 
 
 class EngineType(str, Enum):
     ORCA = "orca"
     TRITON = "triton"
 
 
+class DeploymentType(str, Enum):
+    DEVELOPMENT = "dev"
+    PRODUCTION = "prod"
+
+
 storage_type_map: Dict[StorageType, str] = {
     StorageType.S3: "aws",
     StorageType.BLOB: "azure.blob",
     StorageType.GCS: "gcp",
     StorageType.FAI: "fai",
 }
```

### Comparing `periflow-cli-0.1.8/pfcli/service/auth.py` & `periflow-cli-0.1.9/pfcli/service/auth.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/__init__.py` & `periflow-cli-0.1.9/pfcli/service/client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,19 @@
 from pfcli.service.client.project import (
     ProjectClientService,
     ProjectCredentialClientService,
     ProjectDataClientService,
     PFTProjectVMConfigClientService,
     PFTProjectVMQuotaClientService,
 )
-from pfcli.service.client.deployment import DeploymentClientService
+from pfcli.service.client.deployment import (
+    DeploymentClientService,
+    DeploymentMetricsClientService,
+    PFSProjectUsageClientService,
+)
 from pfcli.service.client.user import (
     UserClientService,
     UserGroupClientService,
     UserGroupProjectClientService,
     UserMFAService,
     UserSignUpService,
 )
@@ -131,14 +135,22 @@
         Template(get_uri("group/$group_id/vm_config/")),
     ),
     ServiceType.JOB_WS: (JobWebSocketClientService, Template(get_wss_uri("job/"))),
     ServiceType.DEPLOYMENT: (
         DeploymentClientService,
         Template(get_pfs_uri("deployment/")),
     ),
+    ServiceType.DEPLOYMENT_METRICS: (
+        DeploymentMetricsClientService,
+        Template(get_pfs_uri("deployment/$deployment_id/metrics/")),
+    ),
+    ServiceType.PFS_PROJECT_USAGE: (
+        PFSProjectUsageClientService,
+        Template(get_pfs_uri("usage/project/$project_id/duration")),
+    ),
     ServiceType.PFT_BILLING_SUMMARY: (
         PFTBillingClientService,
         Template(get_meter_uri("training/instances/price/")),
     ),
     ServiceType.METRICS: (
         MetricsClientService,
         Template(get_observatory_uri("graphql")),
```

### Comparing `periflow-cli-0.1.8/pfcli/service/client/base.py` & `periflow-cli-0.1.9/pfcli/service/client/base.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/billing.py` & `periflow-cli-0.1.9/pfcli/service/client/billing.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/checkpoint.py` & `periflow-cli-0.1.9/pfcli/service/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/credential.py` & `periflow-cli-0.1.9/pfcli/service/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/data.py` & `periflow-cli-0.1.9/pfcli/service/client/data.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/group.py` & `periflow-cli-0.1.9/pfcli/service/client/group.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/job.py` & `periflow-cli-0.1.9/pfcli/service/client/job.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/metrics.py` & `periflow-cli-0.1.9/pfcli/service/client/metrics.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/client/project.py` & `periflow-cli-0.1.9/pfcli/service/client/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         vendor_name = storage_type_map[vendor]
         request_data = {
             "name": name,
             "vendor": vendor_name,
             "region": region,
             "storage_name": storage_name,
-            "credential_id": str(credential_id),
+            "credential_id": str(credential_id) if credential_id is not None else None,
             "metadata": metadata,
             "files": files,
             "active": active,
         }
         response = safe_request(
             self.post, err_prefix="Failed to create a new dataset."
         )(json=request_data)
```

### Comparing `periflow-cli-0.1.8/pfcli/service/client/user.py` & `periflow-cli-0.1.9/pfcli/service/client/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,14 +76,22 @@
         self, pf_user_id: UUID, pf_project_id: UUID, access_level: ProjectRole
     ) -> None:
         safe_request(self.post, err_prefix="Failed to add user to project")(
             path=f"{pf_user_id}/pf_project/{pf_project_id}",
             json={"access_level": access_level.value},
         )
 
+    def delete_from_project(
+        self, pf_user_id: UUID, pf_project_id: UUID,
+    ) -> None:
+        safe_request(self.delete, err_prefix="Failed to remove user from proejct")(
+            pk=pf_user_id,
+            path=f"pf_project/{pf_project_id}",
+        )
+
     def set_project_privilege(
         self, pf_user_id: UUID, pf_project_id: UUID, access_level: ProjectRole
     ) -> None:
         safe_request(
             self.partial_update,
             err_prefix="Failed to update privilege level in project",
         )(
```

### Comparing `periflow-cli-0.1.8/pfcli/service/cloud.py` & `periflow-cli-0.1.9/pfcli/service/cloud.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/service/config.py` & `periflow-cli-0.1.9/pfcli/service/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,26 +602,14 @@
 @dataclass
 class OrcaDeploymentConfigService(DeploymentConfigService):
     """Orca deployment template configuration service"""
 
     use_scaler: bool = False
 
     def start_interaction(self):
-        self.use_specific_image = typer.confirm(
-            "Will you use specific orca docker image?",
-            prompt_suffix="\n>> ",
-        )
-        self.use_ckpt_config = typer.confirm(
-            "Will you use checkpoint config?",
-            prompt_suffix="\n>> ",
-        )
-        self.use_scaler = typer.confirm(
-            "Will you use keda autoscaler?",
-            prompt_suffix="\n>> ",
-        )
         self.ready = True
 
     def render(self) -> str:
         assert self.ready
 
         yaml_str = ORCA_CONFIG
         yaml_str += self._render()
```

### Comparing `periflow-cli-0.1.8/pfcli/service/formatter.py` & `periflow-cli-0.1.9/pfcli/service/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/utils/format.py` & `periflow-cli-0.1.9/pfcli/utils/format.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,15 @@
             return f"{round((delta.seconds % 3600) / 60)} mins ago"
         elif delta < timedelta(days=1):
             return f"{round(delta.seconds / 3600)} hours ago"
         else:
             return f"{delta.days + round(delta.seconds / (3600 * 24))} days ago"
 
 
-def timedelta_to_pretty_str(start: datetime, finish: datetime, long_list: bool = False):
-    delta = finish - start
+def timedelta_to_pretty_str(delta: timedelta, long_list: bool = False):
     if long_list:
         if delta < timedelta(minutes=1):
             return f"{(delta.seconds % 60)}s"
         if delta < timedelta(hours=1):
             return f"{(delta.seconds % 3600) // 60}m {(delta.seconds % 60)}s"
         elif delta < timedelta(days=1):
             return f"{delta.seconds // 3600}h {(delta.seconds % 3600) // 60}m {(delta.seconds % 60)}s"
```

### Comparing `periflow-cli-0.1.8/pfcli/utils/fs.py` & `periflow-cli-0.1.9/pfcli/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/utils/prompt.py` & `periflow-cli-0.1.9/pfcli/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/utils/request.py` & `periflow-cli-0.1.9/pfcli/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/utils/url.py` & `periflow-cli-0.1.9/pfcli/utils/url.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from urllib.parse import urljoin
 
 periflow_api_server = "https://api-staging.friendli.ai/api/"
 periflow_ws_server = "wss://api-ws-staging.friendli.ai/ws/"
 periflow_discuss_url = "https://discuss.friendli.ai/"
 periflow_mr_server = "https://pfmodelregistry-staging.friendli.ai/"
-periflow_serve_server = "http://0.0.0.0:8000/"
+periflow_serve_server = "https://pfs-staging.friendli.ai/"
 periflow_auth_server = "https://pfauth-staging.friendli.ai/"
 periflow_meter_server = "https://pfmeter-staging.friendli.ai/"
 periflow_observatory_server = "https://pfo-staging.friendli.ai/"
 
 
 def get_auth_uri(path: str) -> str:
     return urljoin(periflow_auth_server, path)
```

### Comparing `periflow-cli-0.1.8/pfcli/utils/validate.py` & `periflow-cli-0.1.9/pfcli/utils/validate.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/pfcli/vm.py` & `periflow-cli-0.1.9/pfcli/vm.py`

 * *Files identical despite different names*

### Comparing `periflow-cli-0.1.8/setup.py` & `periflow-cli-0.1.9/setup.py`

 * *Files identical despite different names*

