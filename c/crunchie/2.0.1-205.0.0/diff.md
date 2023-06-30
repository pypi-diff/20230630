# Comparing `tmp/crunchie-2.0.1.tar.gz` & `tmp/crunchie-205.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunchie-2.0.1.tar", last modified: Fri Jun 30 07:41:33 2023, max compression
+gzip compressed data, was "crunchie-205.0.0.tar", last modified: Tue Jun 27 10:19:19 2023, max compression
```

## Comparing `crunchie-2.0.1.tar` & `crunchie-205.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 07:41:33.094993 crunchie-2.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)      160 2023-06-30 07:41:33.094993 crunchie-2.0.1/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 07:41:33.094993 crunchie-2.0.1/crunchie/
--rwxr-x---   0 kali      (1000) kali      (1000)      153 2023-06-27 12:01:27.000000 crunchie-2.0.1/crunchie/main.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-30 07:41:33.094993 crunchie-2.0.1/crunchie.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      160 2023-06-30 07:41:32.000000 crunchie-2.0.1/crunchie.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      153 2023-06-30 07:41:32.000000 crunchie-2.0.1/crunchie.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-30 07:41:32.000000 crunchie-2.0.1/crunchie.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-06-30 07:41:32.000000 crunchie-2.0.1/crunchie.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-06-30 07:41:33.094993 crunchie-2.0.1/setup.cfg
--rwxr-x---   0 kali      (1000) kali      (1000)     1080 2023-06-30 07:41:24.000000 crunchie-2.0.1/setup.py
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 10:19:19.845670 crunchie-205.0.0/
+-rwxrwx---   0 root         (0) vboxsf     (998)      220 2023-06-27 10:19:19.841670 crunchie-205.0.0/PKG-INFO
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 10:19:19.821670 crunchie-205.0.0/crunchie/
+-rwxrwx---   0 root         (0) vboxsf     (998)      155 2023-06-27 09:58:43.000000 crunchie-205.0.0/crunchie/main.py
+drwxrwx---   0 root         (0) vboxsf     (998)        0 2023-06-27 10:19:19.841670 crunchie-205.0.0/crunchie.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (998)      220 2023-06-27 10:19:19.000000 crunchie-205.0.0/crunchie.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (998)      153 2023-06-27 10:19:19.000000 crunchie-205.0.0/crunchie.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)        1 2023-06-27 10:19:19.000000 crunchie-205.0.0/crunchie.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)        9 2023-06-27 10:19:19.000000 crunchie-205.0.0/crunchie.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (998)       38 2023-06-27 10:19:19.845670 crunchie-205.0.0/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (998)      660 2023-06-27 10:00:37.000000 crunchie-205.0.0/setup.py
```

