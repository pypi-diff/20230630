# Comparing `tmp/remotemanager-0.8.0.tar.gz` & `tmp/remotemanager-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.8.0.tar", last modified: Tue Jun 27 13:28:04 2023, max compression
+gzip compressed data, was "remotemanager-0.8.1.tar", last modified: Fri Jun 30 20:01:15 2023, max compression
```

## Comparing `remotemanager-0.8.0.tar` & `remotemanager-0.8.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-27 13:28:04.534990 remotemanager-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-27 06:55:16.000000 remotemanager-0.8.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.526990 remotemanager-0.8.0/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-27 06:55:16.000000 remotemanager-0.8.0/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.526990 remotemanager-0.8.0/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.0/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12847 2023-06-26 12:50:24.000000 remotemanager-0.8.0/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.0/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.0/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.0/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.0/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25581 2023-06-26 08:49:48.000000 remotemanager-0.8.0/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47377 2023-06-27 06:55:16.000000 remotemanager-0.8.0/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     4029 2023-06-26 08:49:48.000000 remotemanager-0.8.0/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    23856 2023-06-27 12:51:29.000000 remotemanager-0.8.0/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4920 2023-06-26 12:50:24.000000 remotemanager-0.8.0/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.0/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.0/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.0/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.530990 remotemanager-0.8.0/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.0/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.0/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.0/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.0/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.0/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.0/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9435 2023-06-26 08:49:48.000000 remotemanager-0.8.0/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.534990 remotemanager-0.8.0/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.0/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:28:04.526990 remotemanager-0.8.0/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 13:28:04.000000 remotemanager-0.8.0/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-27 13:28:04.534990 remotemanager-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-30 20:01:15.851386 remotemanager-0.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-30 09:39:29.000000 remotemanager-0.8.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.843386 remotemanager-0.8.1/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-30 09:39:29.000000 remotemanager-0.8.1/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.1/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-29 14:39:51.000000 remotemanager-0.8.1/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.1/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.1/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.1/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.1/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25581 2023-06-26 08:49:48.000000 remotemanager-0.8.1/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48600 2023-06-30 14:09:28.000000 remotemanager-0.8.1/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-06-26 08:49:48.000000 remotemanager-0.8.1/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    24686 2023-06-30 13:14:43.000000 remotemanager-0.8.1/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4920 2023-06-26 12:50:24.000000 remotemanager-0.8.1/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.1/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.1/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.1/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.1/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.1/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.1/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.1/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.1/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9435 2023-06-26 08:49:48.000000 remotemanager-0.8.1/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 20:01:15.851386 remotemanager-0.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.1/setup.py
```

### Comparing `remotemanager-0.8.0/LICENSE` & `remotemanager-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/PKG-INFO` & `remotemanager-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.0
+Version: 0.8.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.0/README.md` & `remotemanager-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/pyproject.toml` & `remotemanager-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.8.0"
+current_version = "0.8.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.8.0/remotemanager/connection/cmd.py` & `remotemanager-0.8.1/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/connection/computers/base.py` & `remotemanager-0.8.1/remotemanager/connection/computers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,17 @@
 
         if len(optional) > 0:
             spec["optional_resources"] = optional
 
         if len(defaults) > 0:
             spec["optional_defaults"] = defaults
 
+        # avoids a strange error where the parser source cant be found.
+        # likely loads it into memory where `inspect` can access it
+        self.parser
         if isinstance(self._parser, Function):
             spec["resource_parser"] = self._parser
         else:
             spec["resource_parser"] = Function(self.parser)
 
         return spec
 
@@ -389,19 +392,14 @@
             None
         """
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def resources_block(self, **kwargs):
 
-        if "name" in kwargs:
-            # Dataset `name` param detected, use as a default
-            if not hasattr(self, "jobname") or "jobname" not in kwargs:
-                kwargs["jobname"] = kwargs.pop("name")
-
         self.update_resources(**kwargs)
 
         if not self.valid:
             raise RuntimeError(f"missing required arguments: {self.missing}")
 
         if self._parser is None:
             return []
```

### Comparing `remotemanager-0.8.0/remotemanager/connection/computers/example.py` & `remotemanager-0.8.1/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/connection/computers/options.py` & `remotemanager-0.8.1/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/connection/computers/parsers.py` & `remotemanager-0.8.1/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/connection/testing_object.py` & `remotemanager-0.8.1/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/connection/url.py` & `remotemanager-0.8.1/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/dataset/dataset.py` & `remotemanager-0.8.1/remotemanager/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,25 +91,27 @@
         self._global_run_args.update(global_run_args)
 
         # dataset uuid is equal to Function uuid for now
         self._name = name or "dataset"
         self._uuid = generate_uuid(self._function.uuid + self.name)
         self._logger.info(f"uuid is {self.uuid}")
 
-        self._script = script or "#!/bin/bash"
+        self._script = script or ""
         self._extra_files = {
             "send": ensure_list(extra_files_send)
             if extra_files_send is not None
             else [],
             "recv": ensure_list(extra_files_recv)
             if extra_files_recv is not None
             else [],
         }
         self._add_newline = add_newline
 
+        self._last_run = -1
+
         self._url = None
         self._transport = None
         self._computer = False
         self._serialiser = None
         self._dbfile_override = dbfile
         self._dependency = None
         self._do_not_recurse = False
@@ -454,15 +456,15 @@
             quiet (bool):
                 disable printing for this append if True
             skip (bool):
                 ignores checks for an existing runner if set to False
             run_args:
                 any extra arguments to pass to runner
         """
-        self._logger.debug("Dataset append_run called")
+        self._logger.debug("#### Dataset append_run called")
         Quiet.state = quiet
         if args is None and arguments is not None:
             args = arguments
 
         if verbose is None:
             verbose = self.verbose.value
 
@@ -628,14 +630,16 @@
             runner.clear_result()
 
     def _collect_files(self, attribute: str) -> list:
         """
         Collects attribute `attribute` from both Dataset and each runner,
         returning a list.
 
+        Used primarily for deleting those files.
+
         Used for file collection via `_collect_files('remote_dir')`,
         for example
 
         Args:
             attribute (str):
                 attribute to collect
         Returns:
@@ -1029,14 +1033,20 @@
                 state to check for
 
         Returns (bool):
             all(states)
         """
         return all([r == state for r in self.get_all_runner_states()])
 
+    @property
+    def last_run(self):
+        if self._last_run > 0:
+            return self._last_run
+        return None
+
     def run(
         self,
         force: bool = False,
         dry_run: bool = False,
         quiet: bool = False,
         avoid_nodes: bool = False,
         **run_args,
@@ -1052,15 +1062,14 @@
             avoid_nodes (bool):
                 if True, will attempt to avoid running on avoid_nodes using a standard
                 'bash' submission
             run_args:
                 any arguments to pass to the runners during this run.
                 will override any "global" arguments set at Dataset init
         """
-        self._logger.debug("Dataset run called")
         Quiet.state = quiet
 
         if os.name == "nt" and self.url.is_local:
             raise RuntimeError(localwinerror)
         if self.is_parent:
             self._logger.warning(f"dataset {self} is a parent, skipping run")
             Quiet.state = quiet
@@ -1086,15 +1095,18 @@
         **run_args,
     ) -> None:
         """
         Seperation of run and _run allows for dependency runs. Any
         functionality intended for run that does not interact with
         dependencies should be placed here
         """
-        self._logger.debug("Dataset _run called")
+        self.avoid_runtime()
+        runtime = int(time.time())
+        self._logger.runtime(f"#### Dataset _run called at {runtime}")
+        self._last_run = runtime
         self._run_cmds = []
         self._repo_files = []
         self._master_scripts = []
         # initial run args
         if len(run_args) != 0:
             self._logger.info(f"extra run args: {format_iterable(run_args)}")
         temp_args = {"force": force}
@@ -1176,17 +1188,17 @@
 
         if not dry_run:
             self.transport.transfer()
             self.set_runner_states("files copied to remote", runners_to_update)
             if self.is_child:
                 self._logger.info(f"{self} is child, returning")
                 return self._run_finalise()
+            self.set_runner_states(Runner._submit_status["final"], runners_to_update)
             for cmd in cmds:
                 self._run_cmds.append(self.url.cmd(cmd, asynchronous=asynchronous))
-            self.set_runner_states(Runner._submit_status["final"], runners_to_update)
         else:
             self.transport.wipe_transfers()
             for cmd in cmds:
                 self._logger.important(f"launch command: {cmd}")
             self.set_runner_states("dry run", runners_to_update)
 
         self._run_finalise()
@@ -1300,25 +1312,30 @@
             raise_if_not_finished (bool):
                 raise an error if all calculations not finished
 
         Returns:
             None
         """
         Quiet.state = quiet
+        self._logger.runtime("#### Dataset fetch_results called")
+        self.avoid_runtime()
 
         result_mtimes, error_mtimes = self._check_for_runner_outputs()
 
         # no reason to continue if we don't have any files, find out if that's the case
         valid_results = [t for t in result_mtimes.values() if t is not None]
         valid_errors = [t for t in error_mtimes.values() if t is not None]
         if len(valid_results) + len(valid_errors) == 0:
             self._logger.info("no valid results or errors found, exiting early")
             Quiet.state = False
             return
 
+        self._logger.info(f"found {len(valid_results)} valid result files")
+        self._logger.info(f"found {len(valid_errors)} valid error files")
+
         self._logger.info("present result files:")
         self._logger.info(format_iterable(result_mtimes))
         for runner in self.runners:
             if result_mtimes[runner.resultfile.remote]:
                 self.transport.queue_for_pull(
                     os.path.split(runner.resultfile.remote)[1],
                     runner.local_dir,
@@ -1362,14 +1379,18 @@
         Args:
             verbose (bool):
                 disables printing if False
 
         Returns (list):
             boolean list corresponding to the Runner order
         """
+        checktime = int(time.time())
+        self._logger.runtime(f"#### Dataset _is_finished called at {checktime}")
+        self.avoid_runtime()
+
         if not verbose:
             Quiet.state = True
         # initialise an empty return dict
         ret = {r.uuid: None for r in self.runners}
         # if we're skipping, check in with the runners
         # since runner.is_finished = True will be valid...
         for runner in self.runners:
@@ -1459,18 +1480,35 @@
     def results(self) -> list:
         """
         Access the results of the runners
 
         Returns (list):
             runner.result for each runner
         """
+        self._logger.runtime("#### Dataset results called")
         return [r.result for r in self.runners]
 
     @property
     def errors(self) -> list:
         """
         Access the errors of the runners
 
         Returns (list):
             runner.result for each runner
         """
+        self._logger.runtime("#### Dataset errors called")
         return [r.error for r in self.runners]
+
+    def avoid_runtime(self) -> None:
+        """
+        Call for last_runtime sensitive operations such as is_finished and fetch_results
+
+        Waits for 1s if we're too close to the saved _last_run time
+
+        Returns:
+            None
+        """
+        checktime = int(time.time())
+
+        if checktime <= self._last_run:
+            self._logger.runtime("call is too soon after last run, sleeping for 1s")
+            time.sleep(1)
```

### Comparing `remotemanager-0.8.0/remotemanager/dataset/dependency.py` & `remotemanager-0.8.1/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/dataset/runner.py` & `remotemanager-0.8.1/remotemanager/dataset/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,40 +356,67 @@
         """
         Returns the extra files set for this runner
         """
         return self._extra_files
 
     def read_local_files(self):
         self._logger.runtime("reading local runner files")
-        result = False
-        if os.path.isfile(self.resultfile.local):
-            self._logger.info("reading locally discovered runfile")
-            result = self.parent.serialiser.load(self.resultfile.local)
-
-            timestamp = int(os.path.getmtime(self.resultfile.local))
-            if timestamp < self.last_submitted and not self.is_finished:
-                self._logger.warning(f"{self}: calculation not completed yet")
 
+        def check_file_mtime(path: str) -> int:
+            """
+            Checks if a file at `path` exists, and is part of the current run
+
+            Args:
+                path:
+                    filepath to check
+            Returns:
+                (int) timestamp if valid, -1 otherwise
+            """
+            self._logger.runtime(f"checking file {path}")
+            # check if the file exists
+            if not os.path.isfile(path):
+                self._logger.runtime("file not found")
+                return -1
+            # check if the file is from after the most recent submission
+            timestamp = int(os.path.getmtime(path))
+            self._logger.runtime(
+                f"checking mtime {timestamp} vs " f"submit time {self.last_submitted}"
+            )
+            if timestamp < self.last_submitted:
+                self._logger.runtime("file is outdated")
+                return -1
+
+            return timestamp
+
+        finished = False
+        # first try read results
+        timestamp = check_file_mtime(self.resultfile.local)
+        if timestamp > 0:
             mtime = datetime.fromtimestamp(timestamp)
             self.insert_history(mtime, "resultfile created remotely")
 
-            self.result = result
-            result = True
+            self.result = self.parent.serialiser.load(self.resultfile.local)
+            finished = True
+
+        # do the same for the error
+        timestamp = check_file_mtime(self.errorfile.local)
+        if timestamp > 0:
+            mtime = datetime.fromtimestamp(timestamp)
+            self.insert_history(mtime, "errorfile created remotely")
 
-        try:
             with open(self.errorfile.local, "r") as o:
                 error = o.read().strip()
 
-                if error != "":
-                    self._logger.runtime("valid error found, storing")
-                    self.error = error.split("\n")[-1]
-        except FileNotFoundError:
-            self._logger.runtime("no error file found")
+            if error != "":
+                self._logger.runtime("valid error found, storing")
+                self.error = error.split("\n")[-1]
+
+            finished = True
 
-        return result
+        return finished
 
     @property
     def result(self):
         """
         Result (If available)
         """
         if os.path.isfile(self.resultfile.local):
@@ -568,15 +595,15 @@
         self._history[timekey] = newstate
 
     def run(self, dry_run: bool = False, **kwargs) -> None:
         """
         Perform a manual run
 
         .. warning::
-            This method should be used sparingly, as it creates a Datset
+            This method should be used sparingly, as it creates a Dataset
             object within the function from the Database. This is a costly
             process and potentially unstable.
 
         Args:
             dry_run (bool):
                 create files, but do not run
         """
@@ -586,15 +613,14 @@
         if not self._assess_run(**self._run_options):
             return None
 
         if os.name == "nt" and parent.url.is_local:
             raise RuntimeError(localwinerror)
 
         self._manual_run = True  # set internal flag for a manual run
-        self._run_options.update(kwargs)
         self.state = Runner._submit_status["initial"]
         self._write_runfile(parent)
 
         parent.transport.queue_for_push(
             self.runfile.name, self.local_dir, self.remote_dir
         )
```

### Comparing `remotemanager-0.8.0/remotemanager/jupyter/magic.py` & `remotemanager-0.8.1/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/logging/__init__.py` & `remotemanager-0.8.1/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/logging/log.py` & `remotemanager-0.8.1/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/logging/utils.py` & `remotemanager-0.8.1/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/logging/verbosity.py` & `remotemanager-0.8.1/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/serialisation/__init__.py` & `remotemanager-0.8.1/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/serialisation/serial.py` & `remotemanager-0.8.1/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.8.1/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.8.1/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/storage/database.py` & `remotemanager-0.8.1/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/storage/function.py` & `remotemanager-0.8.1/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/storage/remotefunction.py` & `remotemanager-0.8.1/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/storage/sendablemixin.py` & `remotemanager-0.8.1/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/storage/trackedfile.py` & `remotemanager-0.8.1/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/transport/cp.py` & `remotemanager-0.8.1/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/transport/rsync.py` & `remotemanager-0.8.1/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/transport/scp.py` & `remotemanager-0.8.1/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/transport/transport.py` & `remotemanager-0.8.1/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/utils/__init__.py` & `remotemanager-0.8.1/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/utils/flags.py` & `remotemanager-0.8.1/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager/utils/version.py` & `remotemanager-0.8.1/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.0/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.8.1/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.0
+Version: 0.8.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.0/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.8.1/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

