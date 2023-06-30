# Comparing `tmp/gallon-0.0.0.tar.gz` & `tmp/gallon-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallon-0.0.0.tar", max compression
+gzip compressed data, was "gallon-0.0.1.tar", max compression
```

## Comparing `gallon-0.0.0.tar` & `gallon-0.0.1.tar`

### file list

```diff
@@ -1,4 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.0/gallon/__init__.py
--rw-r--r--   0        0        0      272 2023-06-30 01:57:31.056668 gallon-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 gallon-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 01:56:31.790908 gallon-0.0.1/README.md
+-rw-r--r--   0        0        0      257 2023-06-30 03:06:40.530018 gallon-0.0.1/gallon/__init__.py
+-rw-r--r--   0        0        0     4023 2023-06-30 03:03:11.079145 gallon-0.0.1/gallon/client.py
+-rw-r--r--   0        0        0     9668 2023-06-30 03:02:57.075552 gallon-0.0.1/gallon/data.py
+-rw-r--r--   0        0        0     1975 2023-06-30 03:02:44.091937 gallon-0.0.1/gallon/helpers.py
+-rw-r--r--   0        0        0     3589 2023-06-30 03:02:55.375602 gallon-0.0.1/gallon/objects.py
+-rw-r--r--   0        0        0     3989 2023-06-30 02:42:16.528905 gallon-0.0.1/gallon/server.py
+-rw-r--r--   0        0        0      272 2023-06-30 03:07:08.149456 gallon-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 gallon-0.0.1/PKG-INFO
```

