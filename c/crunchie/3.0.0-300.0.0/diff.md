# Comparing `tmp/crunchie-3.0.0.tar.gz` & `tmp/crunchie-300.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunchie-3.0.0.tar", last modified: Fri Jun 30 12:32:50 2023, max compression
+gzip compressed data, was "crunchie-300.0.0.tar", last modified: Fri Jun 30 08:37:19 2023, max compression
```

## Comparing `crunchie-3.0.0.tar` & `crunchie-300.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 12:32:50.947893 crunchie-3.0.0/
--rw-r--r--   0 kali      (1000) kali      (1000)      160 2023-06-30 12:32:50.947893 crunchie-3.0.0/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 12:32:50.943893 crunchie-3.0.0/crunchie/
--rwxr-x---   0 kali      (1000) kali      (1000)      477 2023-06-30 12:32:35.000000 crunchie-3.0.0/crunchie/flake.py
--rwxr-x---   0 kali      (1000) kali      (1000)      157 2023-06-30 08:46:04.000000 crunchie-3.0.0/crunchie/main.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 12:32:50.947893 crunchie-3.0.0/crunchie.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      160 2023-06-30 12:32:50.000000 crunchie-3.0.0/crunchie.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      171 2023-06-30 12:32:50.000000 crunchie-3.0.0/crunchie.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-30 12:32:50.000000 crunchie-3.0.0/crunchie.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-06-30 12:32:50.000000 crunchie-3.0.0/crunchie.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-06-30 12:32:50.947893 crunchie-3.0.0/setup.cfg
--rwxr-x---   0 kali      (1000) kali      (1000)      631 2023-06-30 08:44:53.000000 crunchie-3.0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 08:37:19.339141 crunchie-300.0.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)      162 2023-06-30 08:37:19.331137 crunchie-300.0.0/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 08:37:19.323133 crunchie-300.0.0/crunchie/
+-rwxr-x---   0 kali      (1000) kali      (1000)      841 2023-06-29 05:42:56.000000 crunchie-300.0.0/crunchie/chomp.py
+-rwxr-x---   0 kali      (1000) kali      (1000)      433 2023-06-29 05:42:32.000000 crunchie-300.0.0/crunchie/flake.py
+-rwxr-x---   0 kali      (1000) kali      (1000)      463 2023-06-28 13:47:28.000000 crunchie-300.0.0/crunchie/main.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 08:37:19.331137 crunchie-300.0.0/crunchie.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      162 2023-06-30 08:37:19.000000 crunchie-300.0.0/crunchie.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      189 2023-06-30 08:37:19.000000 crunchie-300.0.0/crunchie.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-30 08:37:19.000000 crunchie-300.0.0/crunchie.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-06-30 08:37:19.000000 crunchie-300.0.0/crunchie.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-06-30 08:37:19.339141 crunchie-300.0.0/setup.cfg
+-rwxr-x---   0 kali      (1000) kali      (1000)     1083 2023-06-28 07:36:38.000000 crunchie-300.0.0/setup.py
```

