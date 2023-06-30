# Comparing `tmp/crewmate-0.0.0.4.tar.gz` & `tmp/crewmate-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewmate-0.0.0.4.tar", last modified: Fri May 26 04:33:37 2023, max compression
+gzip compressed data, was "crewmate-0.0.0.5.tar", last modified: Fri Jun 30 04:33:15 2023, max compression
```

## Comparing `crewmate-0.0.0.4.tar` & `crewmate-0.0.0.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.597859 crewmate-0.0.0.4/
--rw-rw-rw-   0        0        0      178 2023-05-26 04:33:37.597859 crewmate-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-05-26 04:28:27.000000 crewmate-0.0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 04:33:37.599103 crewmate-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-05-26 04:33:34.000000 crewmate-0.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.589186 crewmate-0.0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.592888 crewmate-0.0.0.4/src/crewmate/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:10:04.000000 crewmate-0.0.0.4/src/crewmate/__init__.py
--rw-rw-rw-   0        0        0     3527 2023-05-26 04:31:10.000000 crewmate-0.0.0.4/src/crewmate/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 04:33:37.596852 crewmate-0.0.0.4/src/crewmate.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 04:33:37.000000 crewmate-0.0.0.4/src/crewmate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.817556 crewmate-0.0.0.5/
+-rw-rw-rw-   0        0        0      178 2023-06-30 04:33:15.816540 crewmate-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-05-26 09:14:10.000000 crewmate-0.0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 04:33:15.817556 crewmate-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-06-30 04:33:07.000000 crewmate-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.803276 crewmate-0.0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.810526 crewmate-0.0.0.5/src/crewmate/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:10:04.000000 crewmate-0.0.0.5/src/crewmate/__init__.py
+-rw-rw-rw-   0        0        0     1269 2023-05-26 07:31:14.000000 crewmate-0.0.0.5/src/crewmate/cost_functions.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 04:55:14.000000 crewmate-0.0.0.5/src/crewmate/fit.py
+-rw-rw-rw-   0        0        0     9933 2023-06-30 03:53:53.000000 crewmate-0.0.0.5/src/crewmate/qctrl.py
+-rw-rw-rw-   0        0        0     6134 2023-06-30 04:31:27.000000 crewmate-0.0.0.5/src/crewmate/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 04:33:15.815032 crewmate-0.0.0.5/src/crewmate.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 04:33:15.000000 crewmate-0.0.0.5/src/crewmate.egg-info/top_level.txt
```

