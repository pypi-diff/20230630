# Comparing `tmp/Replidec-0.2.3.1.tar.gz` & `tmp/Replidec-0.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Replidec-0.2.3.1.tar", last modified: Thu Aug 11 21:31:54 2022, max compression
+gzip compressed data, was "Replidec-0.3.1.1.tar", last modified: Fri Jun 30 16:32:42 2023, max compression
```

## Comparing `Replidec-0.2.3.1.tar` & `Replidec-0.3.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)        0 2022-08-11 21:31:54.000000 Replidec-0.2.3.1/
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     1067 2022-08-03 14:50:07.000000 Replidec-0.2.3.1/LICENSE
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)      253 2022-08-08 23:31:07.000000 Replidec-0.2.3.1/MANIFEST.in
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     6033 2022-08-11 21:31:54.000000 Replidec-0.2.3.1/PKG-INFO
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     5437 2022-08-09 08:41:43.000000 Replidec-0.2.3.1/README.rst
-drwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)        0 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec/
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    23622 2022-08-11 21:24:55.000000 Replidec-0.2.3.1/Replidec/Replidec.py
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     5521 2022-08-09 08:03:16.000000 Replidec-0.2.3.1/Replidec/Replidec_cmdline.py
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     9430 2022-08-09 08:01:57.000000 Replidec-0.2.3.1/Replidec/Replidec_multi.py
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)      563 2022-08-08 20:31:42.000000 Replidec-0.2.3.1/Replidec/__init__.py
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     5143 2022-08-03 14:50:07.000000 Replidec-0.2.3.1/Replidec/cli.py
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)      514 2022-07-15 20:04:35.000000 Replidec-0.2.3.1/Replidec/utility.py
-drwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)        0 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     6033 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/PKG-INFO
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     2286 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/SOURCES.txt
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)        1 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/dependency_links.txt
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)       60 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/entry_points.txt
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)       31 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/requires.txt
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)        9 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/Replidec.egg-info/top_level.txt
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)        1 2022-08-08 20:32:04.000000 Replidec-0.2.3.1/Replidec.egg-info/zip-safe
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)      380 2022-08-11 21:31:54.000000 Replidec-0.2.3.1/setup.cfg
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     1141 2022-08-11 21:31:29.000000 Replidec-0.2.3.1/setup.py
-drwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)        0 2022-08-11 21:31:53.000000 Replidec-0.2.3.1/test/
-drwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)        0 2022-08-11 21:31:54.000000 Replidec-0.2.3.1/test/example/
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     1302 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/example.list
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)      600 2022-07-16 00:37:59.000000 Replidec-0.2.3.1/test/example/example.small.list
-drwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)        0 2022-08-11 21:31:54.000000 Replidec-0.2.3.1/test/example/genome_test/
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)     1657 2022-07-17 10:19:10.000000 Replidec-0.2.3.1/test/example/genome_test/generate.sh
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    54156 2022-07-17 10:19:17.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)   146988 2022-07-17 10:19:17.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaab
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)   132469 2022-07-17 10:19:17.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaac
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    13750 2022-07-17 10:19:18.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaad
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     6768 2022-07-17 10:19:18.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaae
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    13628 2022-07-17 10:19:18.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaf
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    61742 2022-07-17 10:19:18.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaag
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    14120 2022-07-17 10:19:19.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaah
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     8995 2022-07-17 10:19:19.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaai
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)   116893 2022-07-17 10:19:19.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaj
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     3350 2022-07-17 10:19:20.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaak
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     8172 2022-07-17 10:19:20.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaal
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     8558 2022-07-17 10:19:20.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaam
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    68228 2022-07-17 10:19:20.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaan
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    31259 2022-07-17 10:19:20.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaao
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)   226244 2022-07-17 10:19:21.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaap
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    63450 2022-07-17 10:19:21.000000 Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaq
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)      739 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/genome_test.index
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)      431 2022-07-15 23:48:19.000000 Replidec-0.2.3.1/test/example/genome_test.small.index
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)      841 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/mock_data_single_lifestyleBC.py
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     1427 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.1.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    20940 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.10.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     7202 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.11.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    24497 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.12.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    17577 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.13.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    13692 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.14.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    18149 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.15.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    22149 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.16.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    43963 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.17.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     1803 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.18.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     3914 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.19.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     1629 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.2.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    20724 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.20.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    21581 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.21.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    21808 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.22.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    35102 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.3.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    12601 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.4.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     9328 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.5.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     2584 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.6.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     7003 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.7.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)     8411 2022-07-15 20:04:21.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.8.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)    31389 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/simulate_art_sample1.9.faa
--rwxr-xr-x   0 xue.peng (143757) OG-VIRO-User (47000)   699219 2022-07-15 20:04:22.000000 Replidec-0.2.3.1/test/example/test.contig.small.fa
--rw-r--r--   0 xue.peng (143757) OG-VIRO-User (47000)      323 2022-07-17 18:17:32.000000 Replidec-0.2.3.1/test/example.sh
+drwxr-xr-x   0 pengxue    (501) staff       (20)        0 2023-06-30 16:32:42.027812 Replidec-0.3.1.1/
+-rw-r--r--   0 pengxue    (501) staff       (20)     1067 2022-08-03 14:38:39.000000 Replidec-0.3.1.1/LICENSE
+-rw-r--r--   0 pengxue    (501) staff       (20)      253 2022-08-09 10:23:53.000000 Replidec-0.3.1.1/MANIFEST.in
+-rw-r--r--   0 pengxue    (501) staff       (20)     5977 2023-06-30 16:32:42.027996 Replidec-0.3.1.1/PKG-INFO
+-rw-r--r--   0 pengxue    (501) staff       (20)     5361 2023-06-30 10:48:03.000000 Replidec-0.3.1.1/README.rst
+drwxr-xr-x   0 pengxue    (501) staff       (20)        0 2023-06-30 16:32:41.995391 Replidec-0.3.1.1/Replidec/
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    24300 2023-06-30 16:31:17.000000 Replidec-0.3.1.1/Replidec/Replidec.py
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     5950 2023-06-30 16:03:18.000000 Replidec-0.3.1.1/Replidec/Replidec_cmdline.py
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     9590 2023-06-30 13:50:44.000000 Replidec-0.3.1.1/Replidec/Replidec_multi.py
+-rwxr-xr-x   0 pengxue    (501) staff       (20)      563 2022-08-09 10:23:53.000000 Replidec-0.3.1.1/Replidec/__init__.py
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     5143 2022-08-03 14:38:39.000000 Replidec-0.3.1.1/Replidec/cli.py
+-rwxr-xr-x   0 pengxue    (501) staff       (20)      514 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/Replidec/utility.py
+drwxr-xr-x   0 pengxue    (501) staff       (20)        0 2023-06-30 16:32:41.998457 Replidec-0.3.1.1/Replidec.egg-info/
+-rw-r--r--   0 pengxue    (501) staff       (20)     5977 2023-06-30 16:32:41.000000 Replidec-0.3.1.1/Replidec.egg-info/PKG-INFO
+-rw-r--r--   0 pengxue    (501) staff       (20)     2286 2023-06-30 16:32:41.000000 Replidec-0.3.1.1/Replidec.egg-info/SOURCES.txt
+-rw-r--r--   0 pengxue    (501) staff       (20)        1 2023-06-30 16:32:41.000000 Replidec-0.3.1.1/Replidec.egg-info/dependency_links.txt
+-rw-r--r--   0 pengxue    (501) staff       (20)       61 2023-06-30 16:32:41.000000 Replidec-0.3.1.1/Replidec.egg-info/entry_points.txt
+-rw-r--r--   0 pengxue    (501) staff       (20)       31 2023-06-30 16:32:41.000000 Replidec-0.3.1.1/Replidec.egg-info/requires.txt
+-rw-r--r--   0 pengxue    (501) staff       (20)        9 2023-06-30 16:32:41.000000 Replidec-0.3.1.1/Replidec.egg-info/top_level.txt
+-rw-r--r--   0 pengxue    (501) staff       (20)        1 2023-06-30 14:19:15.000000 Replidec-0.3.1.1/Replidec.egg-info/zip-safe
+-rw-r--r--   0 pengxue    (501) staff       (20)      382 2023-06-30 16:32:42.028687 Replidec-0.3.1.1/setup.cfg
+-rw-r--r--   0 pengxue    (501) staff       (20)     1141 2023-06-30 14:18:02.000000 Replidec-0.3.1.1/setup.py
+drwxr-xr-x   0 pengxue    (501) staff       (20)        0 2023-06-30 16:32:41.999147 Replidec-0.3.1.1/test/
+drwxr-xr-x   0 pengxue    (501) staff       (20)        0 2023-06-30 16:32:42.013634 Replidec-0.3.1.1/test/example/
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     1302 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/example.list
+-rw-r--r--   0 pengxue    (501) staff       (20)      600 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/example.small.list
+drwxr-xr-x   0 pengxue    (501) staff       (20)        0 2023-06-30 16:32:42.027237 Replidec-0.3.1.1/test/example/genome_test/
+-rw-r--r--   0 pengxue    (501) staff       (20)     1657 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/generate.sh
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    54156 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)   146988 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaab
+-rwxr-xr-x   0 pengxue    (501) staff       (20)   132469 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaac
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    13750 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaad
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     6768 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaae
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    13628 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaf
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    61742 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaag
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    14120 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaah
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     8995 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaai
+-rwxr-xr-x   0 pengxue    (501) staff       (20)   116893 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaj
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     3350 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaak
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     8172 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaal
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     8558 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaam
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    68228 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaan
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    31259 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaao
+-rwxr-xr-x   0 pengxue    (501) staff       (20)   226244 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaap
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    63450 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaq
+-rwxr-xr-x   0 pengxue    (501) staff       (20)      739 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test.index
+-rw-r--r--   0 pengxue    (501) staff       (20)      431 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/genome_test.small.index
+-rwxr-xr-x   0 pengxue    (501) staff       (20)      841 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/mock_data_single_lifestyleBC.py
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     1427 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.1.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    20940 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.10.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     7202 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.11.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    24497 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.12.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    17577 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.13.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    13692 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.14.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    18149 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.15.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    22149 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.16.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    43963 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.17.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     1803 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.18.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     3914 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.19.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     1629 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.2.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    20724 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.20.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    21581 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.21.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    21808 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.22.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    35102 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.3.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    12601 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.4.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     9328 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.5.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     2584 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.6.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     7003 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.7.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)     8411 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.8.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)    31389 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/simulate_art_sample1.9.faa
+-rwxr-xr-x   0 pengxue    (501) staff       (20)   699219 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example/test.contig.small.fa
+-rw-r--r--   0 pengxue    (501) staff       (20)      323 2022-08-03 14:34:55.000000 Replidec-0.3.1.1/test/example.sh
```

### Comparing `Replidec-0.2.3.1/LICENSE` & `Replidec-0.3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/PKG-INFO` & `Replidec-0.3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Replidec
-Version: 0.2.3.1
+Version: 0.3.1.1
 Summary: Replication Cycle Detector for Phages
 Home-page: https://github.com/deng-lab/Replidec
 Author: Xue Peng
 Author-email: xue.peng@helmholtz-muenchen.de
 License: MIT license
 Keywords: Replidec
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -25,34 +26,32 @@
 
 ## Aim
 
 Use bayes classifier combine with homology search to predict virus replication cycle
 
 ## Install
 
-Download database from https://zenodo.org/record/6857082/files/db.tar.gz
-
-### Method 1: using Docker (recommended)
+### Method 1: using Conda
 
 ```bash
-docker pull denglab/replidec
+conda create -n replidec
+conda activate replidec
+conda install -c denglab -c conda-forge -c bioconda replidec
 ```
 
-If you want to use `Replidec` on an HPC, singularity is recommended. You can create a singularity image using following command,
+### Method 2: using Docker
 
 ```bash
-singularity pull replidec.sif docker://denglab/replidec
+docker pull denglab/replidec
 ```
 
-### Method 2: using Conda
+If you want to use `Replidec` on an HPC, singularity is recommended. You can create a singularity image using following command,
 
 ```bash
-conda create -n replidec
-conda activate replidec
-conda install -c denglab -c conda-forge replidec
+singularity pull replidec.sif docker://denglab/replidec
 ```
 
 ### Method 3: using pip
 
 If you install using pip, please make sure that `mmseqs`, `hmmsearch` and `blastp` is set to $PATH, these software can equal or higher than version list below
 
 - MMseqs2 Version: 13.45111
@@ -163,7 +162,9 @@
 ## test passed - multiSeqEachAsOne
 Replidec -p multiSeqEachAsOne -i example/test.contig.small.fa -w multiSeqEachAsOne
 
 ## test passed - batch
 Replidec -p batch -i example/example.small.list -w batch
 ```
 
+
+
```

### Comparing `Replidec-0.2.3.1/README.rst` & `Replidec-0.3.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,32 @@
 
 ## Aim
 
 Use bayes classifier combine with homology search to predict virus replication cycle
 
 ## Install
 
-Download database from https://zenodo.org/record/6857082/files/db.tar.gz
-
-### Method 1: using Docker (recommended)
+### Method 1: using Conda
 
 ```bash
-docker pull denglab/replidec
+conda create -n replidec
+conda activate replidec
+conda install -c denglab -c conda-forge -c bioconda replidec
 ```
 
-If you want to use `Replidec` on an HPC, singularity is recommended. You can create a singularity image using following command,
+### Method 2: using Docker
 
 ```bash
-singularity pull replidec.sif docker://denglab/replidec
+docker pull denglab/replidec
 ```
 
-### Method 2: using Conda
+If you want to use `Replidec` on an HPC, singularity is recommended. You can create a singularity image using following command,
 
 ```bash
-conda create -n replidec
-conda activate replidec
-conda install -c denglab -c conda-forge replidec
+singularity pull replidec.sif docker://denglab/replidec
 ```
 
 ### Method 3: using pip
 
 If you install using pip, please make sure that `mmseqs`, `hmmsearch` and `blastp` is set to $PATH, these software can equal or higher than version list below
 
 - MMseqs2 Version: 13.45111
```

### Comparing `Replidec-0.2.3.1/Replidec/Replidec.py` & `Replidec-0.3.1.1/Replidec/Replidec.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,26 +306,28 @@
         if os.path.exists("%s/db"%scriptPos):
             cmd = "mv %s/db discarded_db"%scriptPos
             obj = Popen(cmd,shell=True)
             obj.wait()
 
     if not os.path.exists(os.path.join(scriptPos,"db")):
         print("db not exist! download database ...")
-        url="https://zenodo.org/record/6975142/files/db_v0.2.3.tar.gz"
+        #url="https://zenodo.org/record/6975142/files/db_v0.2.3.tar.gz"
+        url="https://zenodo.org/record/8101942/files/db_v0.3.1.tar.gz"
         file=os.path.split(url)[-1]
         cmd = "wget {0} -P {1} && cd {1} && tar -zxvf {2} && rm -rf {2}".format(url, scriptPos, file)
         obj = Popen(cmd,shell=True, stdout=PIPE)
         obj.wait()
 
         check_db_md5(scriptPos)
     else:
         print("db exist!")
 
 
 def bayes_classifier_single(inputfile, prefix, wd,
+        db_name="prokaryte",
         hmm_creteria=1e-5, mmseqs_creteria=1e-5, blastp_creteria=1e-3,
         blastp_para="-num_threads 3",
         hmmer_para="--noali --cpu 3",
         mmseqs_para="-s 7 --max-seqs 1 --alignment-mode 3 --alignment-output-mode 0 --min-aln-len 40  --cov-mode 0 --greedy-best-hits 1 --threads 3"):
     '''
     Aim: single predict lifestyle
 
@@ -378,23 +380,37 @@
     if inte_label or excision_label:
         #pfam_label = "Lysogenic"
         pfam_label = "Temperate"
     # print(prefix,inte_label,excision_label,pfam_label)
 
     # phase 2 bayes classifier
     # run mmseqs search
-    bc_mmseqsDB = os.path.join(fileDir, "db/bayes_mmseqs_index/all.protein")
+    if db_name == "all":
+        print("Using prokaryote and eukaryote protein as DB")
+        bc_mmseqsDB = os.path.join(fileDir, "db/bayes_mmseqs_index/all.protein")
+    elif db_name == "prokaryote":
+        print("Using only prokaryote protein as DB")
+        bc_mmseqsDB = os.path.join(fileDir, "db/bayes_mmseqs_index/prokaryote_only")
+    else:
+        print("Please check parameter -D")
+
     mmseqs_wd = os.path.join(wd, "BC_mmseqs")
     mmseqs_prefix = "%s.BC_mmseqs" % prefix
     mmseq_opt = runMmseqsEasysearch(inputfile, mmseqs_prefix, mmseqs_wd, bc_mmseqsDB,
                                     otherPara = mmseqs_para)
     # print(mmseq_opt)
 
     # load score file
-    score_file = os.path.join(fileDir, "db/score.tsv")
+    if db_name == "all":
+        score_file = os.path.join(fileDir, "db/all_mmseq2_linclust_cluster.stat.scoreOpt.tsv")
+    elif db_name == "prokaryote":
+        score_file = os.path.join(fileDir, "db/prokaryote_only_mmseq2_linclust_cluster.stat.scoreOpt.tsv")
+    else:
+        print("Please check parameter -D")
+
     member2scoreD = load_scoreD(score_file)
 
     # read mmseqs easy search file
     p_total_temperate, p_total_lytic, bc_label, match_gene_number = calcaulate_score(
         mmseq_opt, member2scoreD, creteria = mmseqs_creteria)
     print(prefix, inte_label, excision_label, pfam_label,
           p_total_temperate, p_total_lytic, bc_label)
```

### Comparing `Replidec-0.2.3.1/Replidec/Replidec_cmdline.py` & `Replidec-0.3.1.1/Replidec/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 from Replidec.Replidec_multi import bayes_classifier_batch,bayes_classifier_contig,bayes_classifier_genomes
 from argparse import RawTextHelpFormatter,ArgumentParser
-from Replidec.Replidec import checkdb_and_download
-from Replidec.utility import mkdirs
+
 
 current_work_dir = os.path.dirname(os.path.realpath(__file__))
 
 parser = ArgumentParser(description="replication cycle detector", formatter_class=RawTextHelpFormatter)
 parser.add_argument('--version', action='version', version='Replidec v0.2.1')
 
 parser.add_argument("-p","--program", default='multiSeqEachAsOne', required=True,
@@ -45,25 +44,18 @@
                     default="-s 7 --max-seqs 1 --alignment-mode 3 --alignment-output-mode 0 --min-aln-len 40 --cov-mode 0 --greedy-best-hits 1 --threads 3",
                     help="Parameter used for mmseqs")
 
 parser.add_argument("-b", "--bc",default=1e-5, type=float, dest="blastp_creteria", help="Creteria to filter blast result")
 
 parser.add_argument("-B", "--bp",default="-num_threads 3", dest="blastp_parameter", help="Parameter used for blastp")
 
-parser.add_argument("-d", "--db",action='store_true',default=False,dest="db_redownload", help="remove db and redownload")
-
 args = parser.parse_args()
 
 
 def main():
-    if args.db_redownload:
-        print("Check db")
-        fileDir = os.path.dirname(os.path.abspath(__file__))
-        checkdb_and_download(fileDir,redownload=True)
-
     print("Using %s"%args.program)
     if args.program == "multiSeqAsOne":
         bayes_classifier_genomes(args.input_file, args.workdir, summaryfile=args.summary, threads=args.threads,
                                 hmm_creteria=args.hmmer_creteria, mmseqs_creteria=args.mmseqs_creteria, blastp_creteria=args.blastp_creteria,
                                 hmmer_para=args.hmmer_parameter, mmseqs_para=args.mmseqs_parameter, blastp_para=args.blastp_parameter)
     elif args.program == "multiSeqEachAsOne":
         bayes_classifier_contig(args.input_file, args.workdir, summaryfile=args.summary, threads=args.threads,
```

### Comparing `Replidec-0.2.3.1/Replidec/Replidec_multi.py` & `Replidec-0.3.1.1/Replidec/Replidec_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from Bio import Seq,SeqIO
 import time
 from subprocess import Popen
 
 
 
-def bayes_classifier_batch(inputfile, wd, summaryfile="BC_predict.summary",threads=10,
+def bayes_classifier_batch(inputfile, wd, db_name="prokaryte", summaryfile="BC_predict.summary",threads=10,
          hmm_creteria=1e-5, mmseqs_creteria=1e-5, blastp_creteria=1e-5,
          blastp_para="-num_threads 3",
          hmmer_para="--noali --cpu 3",
          mmseqs_para="-s 7 --max-seqs 1 --alignment-mode 3\
                      --alignment-output-mode 0 --min-aln-len 40 --cov-mode 0 --greedy-best-hits 1 --threads 3"):
 
     '''
@@ -37,15 +37,16 @@
 
     header = "sample_name\tintegrase_number\texcisionase_number\tpfam_label\tbc_temperate\tbc_virulent\tbc_label\tfinal_label\tmatch_gene_number\tpath\n"
     opt.write(header)
 
     executor = ThreadPoolExecutor(max_workers=threads)
     all_task = []
     kwargsD={"hmm_creteria":hmm_creteria, "mmseqs_creteria":mmseqs_creteria, "blastp_creteria":blastp_creteria,
-             "blastp_para":blastp_para,"hmmer_para":hmmer_para,"mmseqs_para":mmseqs_para}
+             "blastp_para":blastp_para,"hmmer_para":hmmer_para,"mmseqs_para":mmseqs_para,
+             "db_name":db_name}
 
     ## n is try to control the sceond job will be submit after the first, cause some env or dir will be confilct when run all jobs at same time
     n=0
     with open(inputfile) as f:
         for line in f:
             n+=1
             sample_name, path = line.strip("\n").split("\t")
@@ -58,15 +59,15 @@
         for future in as_completed(all_task):
             res = future.result()
             res.append(path)
             opt.write("\t".join([str(i) for i in res])+"\n")
             #opt.flush()
     opt.close()
 
-def bayes_classifier_contig(inputfile, wd, summaryfile="BC_predict.summary",threads=10,
+def bayes_classifier_contig(inputfile, wd, db_name="prokaryte",summaryfile="BC_predict.summary",threads=10,
           hmm_creteria=1e-5, mmseqs_creteria=1e-5, blastp_creteria=1e-5,
           blastp_para="-num_threads 3",
           hmmer_para="--noali --cpu 3",
           mmseqs_para="-s 7 --max-seqs 1 --alignment-mode 3\
                       --alignment-output-mode 0 --min-aln-len 40 --cov-mode 0 --greedy-best-hits 1 --threads 3"):
 
     '''
@@ -91,15 +92,17 @@
     opt = open(os.path.join(wd, summaryfile), "w")
     header = "sample_name\tintegrase_number\texcisionase_number\tpfam_label\tbc_temperate\tbc_virulent\tbc_label\tfinal_label\tmatch_gene_number\tpath\n"
     opt.write(header)
 
     executor = ThreadPoolExecutor(max_workers=threads)
     all_task = []
     kwargsD={"hmm_creteria":hmm_creteria, "mmseqs_creteria":mmseqs_creteria, "blastp_creteria":blastp_creteria,
-              "blastp_para":blastp_para,"hmmer_para":hmmer_para,"mmseqs_para":mmseqs_para}
+              "blastp_para":blastp_para,"hmmer_para":hmmer_para,"mmseqs_para":mmseqs_para,
+              "db_name":db_name}
+
     faaDict = {}
     for seq in SeqIO.parse(inputfile,"fasta"):
         tmpfile="./%s.tmp"%seq.id
         SeqIO.write(seq,tmpfile,"fasta")
         faaFile = runProdigal(tmpfile, seq.id, "%s/BC_prodigal"%wd, program="meta", otherPara="-g 11")
         faaDict[seq.id] = faaFile
         #res = ["sample_name"] + ['NA']*6 + [0]
@@ -122,15 +125,15 @@
         res.append(faaFile)
         opt.write("\t".join([str(i) for i in res])+"\n")
         #opt.flush()
         os.remove(tmpfile)
     opt.close()
 
 
-def bayes_classifier_genomes(inputfile, wd, summaryfile="BC_predict.summary",threads=10,
+def bayes_classifier_genomes(inputfile, wd, db_name="prokaryte",summaryfile="BC_predict.summary",threads=10,
            hmm_creteria=1e-5, mmseqs_creteria=1e-5, blastp_creteria=1e-5,
            blastp_para="-num_threads 3",
            hmmer_para="--noali --cpu 3",
            mmseqs_para="-s 7 --max-seqs 1 --alignment-mode 3\
                        --alignment-output-mode 0 --min-aln-len 40 --cov-mode 0 --greedy-best-hits 1 --threads 3"):
     '''
     Aim: predict lifestyle for one genome file which contain multiple seq
@@ -156,15 +159,16 @@
     opt = open(os.path.join(wd, summaryfile), "w")
     header = "sample_name\tintegrase_number\texcisionase_number\tpfam_label\tbc_temperate\tbc_virulent\tbc_label\tfinal_label\tmatch_gene_number\tpath\n"
     opt.write(header)
 
     executor = ThreadPoolExecutor(max_workers=threads)
     all_task = []
     kwargsD={"hmm_creteria":hmm_creteria, "mmseqs_creteria":mmseqs_creteria, "blastp_creteria":blastp_creteria,
-              "blastp_para":blastp_para,"hmmer_para":hmmer_para,"mmseqs_para":mmseqs_para}
+              "blastp_para":blastp_para,"hmmer_para":hmmer_para,"mmseqs_para":mmseqs_para,
+              "db_name":db_name}
     faaDict = {}
 
     with open(inputfile) as f:
         for line in f:
             sample_name, path = line.strip("\n").split("\t")
             faaFile = runProdigal(path, sample_name, "%s/BC_prodigal"%wd, program="meta", otherPara="-g 11")
             #res = [sample_name] + ['NA']*6 + [0]
```

### Comparing `Replidec-0.2.3.1/Replidec/__init__.py` & `Replidec-0.3.1.1/Replidec/__init__.py`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/Replidec/cli.py` & `Replidec-0.3.1.1/Replidec/Replidec_cmdline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 from Replidec.Replidec_multi import bayes_classifier_batch,bayes_classifier_contig,bayes_classifier_genomes
 from argparse import RawTextHelpFormatter,ArgumentParser
-
+from Replidec.Replidec import checkdb_and_download
+from Replidec.utility import mkdirs
 
 current_work_dir = os.path.dirname(os.path.realpath(__file__))
 
 parser = ArgumentParser(description="replication cycle detector", formatter_class=RawTextHelpFormatter)
 parser.add_argument('--version', action='version', version='Replidec v0.2.1')
 
 parser.add_argument("-p","--program", default='multiSeqEachAsOne', required=True,
@@ -44,29 +45,42 @@
                     default="-s 7 --max-seqs 1 --alignment-mode 3 --alignment-output-mode 0 --min-aln-len 40 --cov-mode 0 --greedy-best-hits 1 --threads 3",
                     help="Parameter used for mmseqs")
 
 parser.add_argument("-b", "--bc",default=1e-5, type=float, dest="blastp_creteria", help="Creteria to filter blast result")
 
 parser.add_argument("-B", "--bp",default="-num_threads 3", dest="blastp_parameter", help="Parameter used for blastp")
 
+parser.add_argument("-d", "--db",action='store_true',default=False,dest="db_redownload", help="remove db and redownload")
+
+parser.add_argument("-D", "--databaseN",default="prokaryote",choices=["all","prokaryote"],dest="db_name", 
+                    help="specific which database will use. all contain protein from prokaryote and eukaryote; prokaryote contain protein only from prokaryote")
+
 args = parser.parse_args()
 
 
 def main():
+    if args.db_redownload:
+        print("Check db")
+        fileDir = os.path.dirname(os.path.abspath(__file__))
+        checkdb_and_download(fileDir,redownload=True)
+
     print("Using %s"%args.program)
     if args.program == "multiSeqAsOne":
-        bayes_classifier_genomes(args.input_file, args.workdir, summaryfile=args.summary, threads=args.threads,
+        bayes_classifier_genomes(args.input_file, args.workdir,db_name=args.db_name, 
+                                summaryfile=args.summary, threads=args.threads,
                                 hmm_creteria=args.hmmer_creteria, mmseqs_creteria=args.mmseqs_creteria, blastp_creteria=args.blastp_creteria,
                                 hmmer_para=args.hmmer_parameter, mmseqs_para=args.mmseqs_parameter, blastp_para=args.blastp_parameter)
     elif args.program == "multiSeqEachAsOne":
-        bayes_classifier_contig(args.input_file, args.workdir, summaryfile=args.summary, threads=args.threads,
+        bayes_classifier_contig(args.input_file, args.workdir,db_name=args.db_name, 
+                               summaryfile=args.summary, threads=args.threads,
                                hmm_creteria=args.hmmer_creteria, mmseqs_creteria=args.mmseqs_creteria, blastp_creteria=args.blastp_creteria,
                                hmmer_para=args.hmmer_parameter, mmseqs_para=args.mmseqs_parameter, blastp_para=args.blastp_parameter)
     elif args.program == "batch":
-        bayes_classifier_batch(args.input_file, args.workdir, summaryfile=args.summary, threads=args.threads,
+        bayes_classifier_batch(args.input_file, args.workdir,db_name=args.db_name, 
+                               summaryfile=args.summary, threads=args.threads,
                               hmm_creteria=args.hmmer_creteria, mmseqs_creteria=args.mmseqs_creteria, blastp_creteria=args.blastp_creteria,
                               hmmer_para=args.hmmer_parameter, mmseqs_para=args.mmseqs_parameter, blastp_para=args.blastp_parameter)
     #elif args.program == "test_multiSeqAsOne":
     #    bayes_classifier_genomes("%s/example/genome_test.index"%current_work_dir, "./test_multiSeqAsOne",
     #                            summaryfile="BC_predict.summary",threads=10)
     #elif args.program == "test_multiSeqEachAsOne":
     #    bayes_classifier_contig("%s/example/test.contig.small.fa"%current_work_dir, "./test_multiSeqEachAsOne",
```

### Comparing `Replidec-0.2.3.1/Replidec/utility.py` & `Replidec-0.3.1.1/Replidec/utility.py`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/Replidec.egg-info/PKG-INFO` & `Replidec-0.3.1.1/Replidec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Replidec
-Version: 0.2.3.1
+Version: 0.3.1.1
 Summary: Replication Cycle Detector for Phages
 Home-page: https://github.com/deng-lab/Replidec
 Author: Xue Peng
 Author-email: xue.peng@helmholtz-muenchen.de
 License: MIT license
 Keywords: Replidec
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -25,34 +26,32 @@
 
 ## Aim
 
 Use bayes classifier combine with homology search to predict virus replication cycle
 
 ## Install
 
-Download database from https://zenodo.org/record/6857082/files/db.tar.gz
-
-### Method 1: using Docker (recommended)
+### Method 1: using Conda
 
 ```bash
-docker pull denglab/replidec
+conda create -n replidec
+conda activate replidec
+conda install -c denglab -c conda-forge -c bioconda replidec
 ```
 
-If you want to use `Replidec` on an HPC, singularity is recommended. You can create a singularity image using following command,
+### Method 2: using Docker
 
 ```bash
-singularity pull replidec.sif docker://denglab/replidec
+docker pull denglab/replidec
 ```
 
-### Method 2: using Conda
+If you want to use `Replidec` on an HPC, singularity is recommended. You can create a singularity image using following command,
 
 ```bash
-conda create -n replidec
-conda activate replidec
-conda install -c denglab -c conda-forge replidec
+singularity pull replidec.sif docker://denglab/replidec
 ```
 
 ### Method 3: using pip
 
 If you install using pip, please make sure that `mmseqs`, `hmmsearch` and `blastp` is set to $PATH, these software can equal or higher than version list below
 
 - MMseqs2 Version: 13.45111
@@ -163,7 +162,9 @@
 ## test passed - multiSeqEachAsOne
 Replidec -p multiSeqEachAsOne -i example/test.contig.small.fa -w multiSeqEachAsOne
 
 ## test passed - batch
 Replidec -p batch -i example/example.small.list -w batch
 ```
 
+
+
```

### Comparing `Replidec-0.2.3.1/Replidec.egg-info/SOURCES.txt` & `Replidec-0.3.1.1/Replidec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/setup.py` & `Replidec-0.3.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 requirements = ["biopython>=1.77",
                 "future>=0.18.2",]
 
 
 setup(
     name='Replidec',
-    version='0.2.3.1',
+    version='0.3.1.1',
     author="Xue Peng",
     author_email='xue.peng@helmholtz-muenchen.de',
     keywords='Replidec',
     description='Replication Cycle Detector for Phages',
     long_description=readme,
     long_description_content_type="text/markdown",
     url='https://github.com/deng-lab/Replidec',
```

### Comparing `Replidec-0.2.3.1/test/example/example.list` & `Replidec-0.3.1.1/test/example/example.list`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/example.small.list` & `Replidec-0.3.1.1/test/example/example.small.list`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/generate.sh` & `Replidec-0.3.1.1/test/example/genome_test/generate.sh`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaa` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaab` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaab`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaac` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaac`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaad` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaad`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaae` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaae`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaf` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaf`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaag` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaag`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaah` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaah`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaai` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaai`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaj` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaj`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaak` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaak`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaal` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaal`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaam` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaam`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaan` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaan`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaao` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaao`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaap` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaap`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test/genome.test.fnaaq` & `Replidec-0.3.1.1/test/example/genome_test/genome.test.fnaaq`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/genome_test.index` & `Replidec-0.3.1.1/test/example/genome_test.index`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/mock_data_single_lifestyleBC.py` & `Replidec-0.3.1.1/test/example/mock_data_single_lifestyleBC.py`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.1.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.1.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.10.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.10.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.11.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.11.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.12.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.12.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.13.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.13.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.14.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.14.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.15.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.15.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.16.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.16.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.17.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.17.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.18.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.18.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.19.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.19.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.2.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.2.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.20.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.20.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.21.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.21.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.22.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.22.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.3.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.3.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.4.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.4.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.5.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.5.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.6.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.6.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.7.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.7.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.8.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.8.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/simulate_art_sample1.9.faa` & `Replidec-0.3.1.1/test/example/simulate_art_sample1.9.faa`

 * *Files identical despite different names*

### Comparing `Replidec-0.2.3.1/test/example/test.contig.small.fa` & `Replidec-0.3.1.1/test/example/test.contig.small.fa`

 * *Files identical despite different names*

