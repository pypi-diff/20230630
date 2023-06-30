# Comparing `tmp/drive_ibd-1.0.0.tar.gz` & `tmp/drive_ibd-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-1.0.0.tar", max compression
+gzip compressed data, was "drive_ibd-2.0.2.tar", max compression
```

## Comparing `drive_ibd-1.0.0.tar` & `drive_ibd-2.0.2.tar`

### file list

```diff
@@ -1,6 +1,37 @@
--rw-r--r--   0        0        0        0 2023-03-29 18:09:05.948006 drive_ibd-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-03-29 18:09:05.980005 drive_ibd-1.0.0/drive/__init__.py
--rw-r--r--   0        0        0     8857 2023-03-30 22:13:28.644929 drive_ibd-1.0.0/drive/drive.py
--rw-r--r--   0        0        0     1125 2023-03-30 22:21:54.759542 drive_ibd-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 drive_ibd-1.0.0/setup.py
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 drive_ibd-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-02 16:23:38.534742 drive_ibd-2.0.2/README.md
+-rw-r--r--   0        0        0       23 2023-05-08 17:12:27.774702 drive_ibd-2.0.2/drive/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-04 19:56:44.572942 drive_ibd-2.0.2/drive/cluster/__init__.py
+-rw-r--r--   0        0        0    17869 2023-05-23 17:27:33.288051 drive_ibd-2.0.2/drive/cluster/cluster.py
+-rw-r--r--   0        0        0    10145 2023-06-26 19:00:49.383493 drive_ibd-2.0.2/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-04-11 15:57:06.666606 drive_ibd-2.0.2/drive/factory/__init__.py
+-rw-r--r--   0        0        0     1515 2023-05-03 21:40:36.665638 drive_ibd-2.0.2/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-05-03 21:40:36.649638 drive_ibd-2.0.2/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-06-22 19:24:49.749173 drive_ibd-2.0.2/drive/filters/__init__.py
+-rw-r--r--   0        0        0    17183 2023-06-27 18:29:28.100126 drive_ibd-2.0.2/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.0.2/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.0.2/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.0.2/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.0.2/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.0.2/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.0.2/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6230 2023-06-22 19:16:27.189955 drive_ibd-2.0.2/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.0.2/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     4240 2023-05-23 17:27:33.148055 drive_ibd-2.0.2/drive/log/logger.py
+-rw-r--r--   0        0        0      248 2023-06-21 16:46:23.320291 drive_ibd-2.0.2/drive/models/__init__.py
+-rw-r--r--   0        0        0      503 2023-06-21 16:46:16.772455 drive_ibd-2.0.2/drive/models/choices.py
+-rw-r--r--   0        0        0      694 2023-05-04 22:02:59.468876 drive_ibd-2.0.2/drive/models/data_container.py
+-rw-r--r--   0        0        0     4493 2023-06-27 18:13:44.556344 drive_ibd-2.0.2/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-05-04 16:45:00.827439 drive_ibd-2.0.2/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-04-13 21:14:00.109726 drive_ibd-2.0.2/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:34:54.522918 drive_ibd-2.0.2/drive/plugins/__init__.py
+-rw-r--r--   0        0        0     4352 2023-06-27 18:14:16.239555 drive_ibd-2.0.2/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    10084 2023-05-23 17:30:22.059715 drive_ibd-2.0.2/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0       59 2023-05-03 21:40:36.641638 drive_ibd-2.0.2/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0     1520 2023-05-03 21:40:36.657638 drive_ibd-2.0.2/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2222 2023-05-02 19:24:58.309743 drive_ibd-2.0.2/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-05-03 21:42:41.142428 drive_ibd-2.0.2/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0     9196 2023-05-23 17:27:33.204053 drive_ibd-2.0.2/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-05-04 20:29:24.747764 drive_ibd-2.0.2/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2145 2023-06-30 15:31:09.902368 drive_ibd-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 drive_ibd-2.0.2/setup.py
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 drive_ibd-2.0.2/PKG-INFO
```

