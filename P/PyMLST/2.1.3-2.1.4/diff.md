# Comparing `tmp/PyMLST-2.1.3.tar.gz` & `tmp/PyMLST-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMLST-2.1.3.tar", last modified: Mon Jun 13 11:05:00 2022, max compression
+gzip compressed data, was "PyMLST-2.1.4.tar", last modified: Fri Jun 30 13:08:43 2023, max compression
```

## Comparing `PyMLST-2.1.3.tar` & `PyMLST-2.1.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.931489 PyMLST-2.1.3/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      301 2021-09-30 14:06:39.000000 PyMLST-2.1.3/MANIFEST.in
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    15580 2022-06-13 11:05:00.931489 PyMLST-2.1.3/PKG-INFO
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.799488 PyMLST-2.1.3/PyMLST.egg-info/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    15580 2022-06-13 11:05:00.000000 PyMLST-2.1.3/PyMLST.egg-info/PKG-INFO
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1616 2022-06-13 11:05:00.000000 PyMLST-2.1.3/PyMLST.egg-info/SOURCES.txt
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        1 2022-06-13 11:05:00.000000 PyMLST-2.1.3/PyMLST.egg-info/dependency_links.txt
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      104 2022-06-13 11:05:00.000000 PyMLST-2.1.3/PyMLST.egg-info/entry_points.txt
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      213 2022-06-13 11:05:00.000000 PyMLST-2.1.3/PyMLST.egg-info/requires.txt
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        7 2022-06-13 11:05:00.000000 PyMLST-2.1.3/PyMLST.egg-info/top_level.txt
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    11949 2022-06-13 08:50:45.000000 PyMLST-2.1.3/README.md
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.819489 PyMLST-2.1.3/pymlst/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      309 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/__init__.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.831489 PyMLST-2.1.3/pymlst/cla/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/cla/__init__.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.855489 PyMLST-2.1.3/pymlst/cla/commands/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/cla/commands/__init__.py
--rwxrwx---   0 bvalot3   (1003) 2b2s      (1006)     1038 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/cla/commands/create.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2521 2021-10-25 14:40:39.000000 PyMLST-2.1.3/pymlst/cla/commands/import.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      680 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/cla/commands/remove.py
--rwxrwx---   0 bvalot3   (1003) 2b2s      (1006)     1190 2021-10-26 08:44:21.000000 PyMLST-2.1.3/pymlst/cla/commands/search.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1429 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/cla/commands/search2.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    24535 2022-02-24 08:56:40.000000 PyMLST-2.1.3/pymlst/cla/core.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      525 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/cla/model.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2645 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/cmd.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.875489 PyMLST-2.1.3/pymlst/common/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/common/__init__.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1892 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/common/blat.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.875489 PyMLST-2.1.3/pymlst/common/commands/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/common/commands/__init__.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1734 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/common/commands/configure.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      773 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/common/exceptions.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      190 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/common/flag.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     4761 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/common/kma.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1377 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/common/mafft.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     7428 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/common/psl.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     3879 2022-05-11 12:21:41.000000 PyMLST-2.1.3/pymlst/common/utils.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     8247 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/common/web.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1967 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/config.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.759488 PyMLST-2.1.3/pymlst/data/
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.887489 PyMLST-2.1.3/pymlst/data/alembic/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2305 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/alembic.ini
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.891489 PyMLST-2.1.3/pymlst/data/alembic/cla/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2393 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/cla/env.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      494 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/cla/script.py.mako
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.891489 PyMLST-2.1.3/pymlst/data/alembic/cla/versions/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1561 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/cla/versions/21efe503d07d_initial.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.891489 PyMLST-2.1.3/pymlst/data/alembic/wg/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2392 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/wg/env.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      494 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/wg/script.py.mako
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.891489 PyMLST-2.1.3/pymlst/data/alembic/wg/versions/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2179 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/data/alembic/wg/versions/52ae99cb5f33_initial.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      294 2022-06-13 09:44:50.000000 PyMLST-2.1.3/pymlst/version.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.911489 PyMLST-2.1.3/pymlst/wg/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)       72 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/__init__.py
-drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2022-06-13 11:05:00.923489 PyMLST-2.1.3/pymlst/wg/commands/
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/__init__.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      999 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/add.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1173 2022-01-06 11:51:35.000000 PyMLST-2.1.3/pymlst/wg/commands/add2.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1368 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/create.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      850 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/distance.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      824 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/gene.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2341 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/import.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      971 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/mlst.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1113 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/msa.py
--rwxrwx---   0 bvalot3   (1003) 2b2s      (1006)      731 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/recombinaison.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1436 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/remove.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1109 2022-01-11 12:46:47.000000 PyMLST-2.1.3/pymlst/wg/commands/sequence.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      542 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/stats.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      984 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/commands/strain.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      941 2022-03-08 08:04:09.000000 PyMLST-2.1.3/pymlst/wg/commands/subgraph.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    32362 2022-05-11 12:25:59.000000 PyMLST-2.1.3/pymlst/wg/core.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    10479 2022-01-11 12:45:40.000000 PyMLST-2.1.3/pymlst/wg/extractors.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      681 2021-09-30 14:06:39.000000 PyMLST-2.1.3/pymlst/wg/model.py
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)       76 2022-06-13 11:05:00.931489 PyMLST-2.1.3/setup.cfg
--rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     3321 2021-09-30 14:06:39.000000 PyMLST-2.1.3/setup.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.822093 PyMLST-2.1.4/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      301 2021-09-30 14:06:39.000000 PyMLST-2.1.4/MANIFEST.in
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    15595 2023-06-30 13:08:43.822093 PyMLST-2.1.4/PKG-INFO
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.618092 PyMLST-2.1.4/PyMLST.egg-info/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    15595 2023-06-30 13:08:43.000000 PyMLST-2.1.4/PyMLST.egg-info/PKG-INFO
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1616 2023-06-30 13:08:43.000000 PyMLST-2.1.4/PyMLST.egg-info/SOURCES.txt
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        1 2023-06-30 13:08:43.000000 PyMLST-2.1.4/PyMLST.egg-info/dependency_links.txt
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      104 2023-06-30 13:08:43.000000 PyMLST-2.1.4/PyMLST.egg-info/entry_points.txt
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      195 2023-06-30 13:08:43.000000 PyMLST-2.1.4/PyMLST.egg-info/requires.txt
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        7 2023-06-30 13:08:43.000000 PyMLST-2.1.4/PyMLST.egg-info/top_level.txt
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    11964 2023-03-02 15:18:39.000000 PyMLST-2.1.4/README.md
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.650092 PyMLST-2.1.4/pymlst/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      309 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/__init__.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.678093 PyMLST-2.1.4/pymlst/cla/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/cla/__init__.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.702093 PyMLST-2.1.4/pymlst/cla/commands/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/cla/commands/__init__.py
+-rwxrwx---   0 bvalot3   (1003) 2b2s      (1006)     1038 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/cla/commands/create.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2521 2021-10-25 14:40:39.000000 PyMLST-2.1.4/pymlst/cla/commands/import.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      680 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/cla/commands/remove.py
+-rwxrwx---   0 bvalot3   (1003) 2b2s      (1006)     1190 2021-10-26 08:44:21.000000 PyMLST-2.1.4/pymlst/cla/commands/search.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1429 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/cla/commands/search2.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    24535 2022-02-24 08:56:40.000000 PyMLST-2.1.4/pymlst/cla/core.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      525 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/cla/model.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2645 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/cmd.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.762093 PyMLST-2.1.4/pymlst/common/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/common/__init__.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1892 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/common/blat.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.762093 PyMLST-2.1.4/pymlst/common/commands/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/common/commands/__init__.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1734 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/common/commands/configure.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      817 2023-03-10 16:04:26.000000 PyMLST-2.1.4/pymlst/common/exceptions.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      190 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/common/flag.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     4761 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/common/kma.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1377 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/common/mafft.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     7428 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/common/psl.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     3879 2022-05-11 12:21:41.000000 PyMLST-2.1.4/pymlst/common/utils.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     8247 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/common/web.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1967 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/config.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.614092 PyMLST-2.1.4/pymlst/data/
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.778093 PyMLST-2.1.4/pymlst/data/alembic/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2305 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/alembic.ini
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.778093 PyMLST-2.1.4/pymlst/data/alembic/cla/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2393 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/cla/env.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      494 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/cla/script.py.mako
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.778093 PyMLST-2.1.4/pymlst/data/alembic/cla/versions/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1561 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/cla/versions/21efe503d07d_initial.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.782093 PyMLST-2.1.4/pymlst/data/alembic/wg/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2392 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/wg/env.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      494 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/wg/script.py.mako
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.782093 PyMLST-2.1.4/pymlst/data/alembic/wg/versions/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2179 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/data/alembic/wg/versions/52ae99cb5f33_initial.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      294 2023-06-30 13:00:17.000000 PyMLST-2.1.4/pymlst/version.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.782093 PyMLST-2.1.4/pymlst/wg/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)       72 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/__init__.py
+drwxrwx---   0 bvalot3   (1003) 2b2s      (1006)        0 2023-06-30 13:08:43.806093 PyMLST-2.1.4/pymlst/wg/commands/
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)        0 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/__init__.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      999 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/add.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1173 2022-01-06 11:51:35.000000 PyMLST-2.1.4/pymlst/wg/commands/add2.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1372 2023-03-10 16:13:27.000000 PyMLST-2.1.4/pymlst/wg/commands/create.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      850 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/distance.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      823 2023-03-10 12:56:34.000000 PyMLST-2.1.4/pymlst/wg/commands/gene.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     2341 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/import.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      971 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/mlst.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1113 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/msa.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      731 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/recombinaison.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1436 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/remove.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     1109 2022-01-11 12:46:47.000000 PyMLST-2.1.4/pymlst/wg/commands/sequence.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      542 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/stats.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      984 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/commands/strain.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      941 2022-03-08 08:04:09.000000 PyMLST-2.1.4/pymlst/wg/commands/subgraph.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    32564 2023-03-10 16:08:19.000000 PyMLST-2.1.4/pymlst/wg/core.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)    10553 2023-03-10 13:25:14.000000 PyMLST-2.1.4/pymlst/wg/extractors.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)      681 2021-09-30 14:06:39.000000 PyMLST-2.1.4/pymlst/wg/model.py
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)       76 2023-06-30 13:08:43.822093 PyMLST-2.1.4/setup.cfg
+-rw-rw----   0 bvalot3   (1003) 2b2s      (1006)     3303 2023-03-02 14:07:42.000000 PyMLST-2.1.4/setup.py
```

### Comparing `PyMLST-2.1.3/PKG-INFO` & `PyMLST-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyMLST
-Version: 2.1.3
+Version: 2.1.4
 Summary: python Mlst Local Search Tool
 Home-page: https://github.com/bvalot/pyMLST.git
 Author: Benoit Valot
 Author-email: benoit.valot@univ-fcomte.fr
 License: GPLv3
-Download-URL: https://github.com/bvalot/pyMLST/archive/refs/tags/2.1.3.tar.gz
+Download-URL: https://github.com/bvalot/pyMLST/archive/refs/tags/2.1.4.tar.gz
 Description: # PyMLST
         A Python Mlst Local Search Tool.
         
         ## Purpose
         Typing bacteria is an important public health task in hospital. 
         The use of next generation sequencing to analyse or survey epidimic strain is rising.
         For this purpose, core or whole genome Multilocus Sequence Typing (cgMLST / wgMLST) has become the new standard.
@@ -37,15 +37,15 @@
         - A configuration file for defined PATH to external tools.
         - An easy installation with pypi repository.
         
         
         ## Automatic Installation
         
         ```
-        conda install -c bioconda pymlst
+        conda install -c bioconda -c conda-forge pymlst
         ```
         
         ## Manual Installation
         ### From pypi repository
         
         ```
         pip install pymlst
@@ -149,15 +149,15 @@
         The scheme is a multi-fasta file containing sequences of genes in nucleotide format.
         You can obtained scheme for:
         	- Core genome analysis in publications.
         	- Whole genome analysis by using annoted genes of a publish genome close to your strains.
         
         ```
         wgMLST create --help
-        Usage: wgMLST create [OPTIONS] COREGENE DATABASE
+        Usage: wgMLST create [OPTIONS] DATABASE COREGENE
         
           Create a wgMLST DATABASE from a template COREGENE.
         
         Options:
           -f, --force        Override alrealdy existing DATABASE
           -c, --concatenate  Automatically concatenate genes with duplicated sequences
           -r, --remove       Automatically remove genes with duplicated sequences
@@ -167,15 +167,15 @@
         
         Next, you need to add your strain iteratively to the database. 
         A draft genome can be used (we recommend to use [Spades](http://cab.spbu.ru/software/spades/) for assembly).
         You can also add reference genome for comparison.
         
         ```
         wgMLST add --help
-        Usage: wgMLST add [OPTIONS] GENOME DATABASE
+        Usage: wgMLST add [OPTIONS] DATABASE GENOME
         
           Add a strain GENOME to the wgMLST DATABASE.
         
         Options:
           -s, --strain TEXT     Name of the strain (default:genome name)
           -i, --identity FLOAT  Minimum identity to search gene (default=0.95)
           -c, --coverage FLOAT  Minimum coverage to search gene (default=0.9)
```

### Comparing `PyMLST-2.1.3/PyMLST.egg-info/PKG-INFO` & `PyMLST-2.1.4/PyMLST.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyMLST
-Version: 2.1.3
+Version: 2.1.4
 Summary: python Mlst Local Search Tool
 Home-page: https://github.com/bvalot/pyMLST.git
 Author: Benoit Valot
 Author-email: benoit.valot@univ-fcomte.fr
 License: GPLv3
-Download-URL: https://github.com/bvalot/pyMLST/archive/refs/tags/2.1.3.tar.gz
+Download-URL: https://github.com/bvalot/pyMLST/archive/refs/tags/2.1.4.tar.gz
 Description: # PyMLST
         A Python Mlst Local Search Tool.
         
         ## Purpose
         Typing bacteria is an important public health task in hospital. 
         The use of next generation sequencing to analyse or survey epidimic strain is rising.
         For this purpose, core or whole genome Multilocus Sequence Typing (cgMLST / wgMLST) has become the new standard.
@@ -37,15 +37,15 @@
         - A configuration file for defined PATH to external tools.
         - An easy installation with pypi repository.
         
         
         ## Automatic Installation
         
         ```
-        conda install -c bioconda pymlst
+        conda install -c bioconda -c conda-forge pymlst
         ```
         
         ## Manual Installation
         ### From pypi repository
         
         ```
         pip install pymlst
@@ -149,15 +149,15 @@
         The scheme is a multi-fasta file containing sequences of genes in nucleotide format.
         You can obtained scheme for:
         	- Core genome analysis in publications.
         	- Whole genome analysis by using annoted genes of a publish genome close to your strains.
         
         ```
         wgMLST create --help
-        Usage: wgMLST create [OPTIONS] COREGENE DATABASE
+        Usage: wgMLST create [OPTIONS] DATABASE COREGENE
         
           Create a wgMLST DATABASE from a template COREGENE.
         
         Options:
           -f, --force        Override alrealdy existing DATABASE
           -c, --concatenate  Automatically concatenate genes with duplicated sequences
           -r, --remove       Automatically remove genes with duplicated sequences
@@ -167,15 +167,15 @@
         
         Next, you need to add your strain iteratively to the database. 
         A draft genome can be used (we recommend to use [Spades](http://cab.spbu.ru/software/spades/) for assembly).
         You can also add reference genome for comparison.
         
         ```
         wgMLST add --help
-        Usage: wgMLST add [OPTIONS] GENOME DATABASE
+        Usage: wgMLST add [OPTIONS] DATABASE GENOME
         
           Add a strain GENOME to the wgMLST DATABASE.
         
         Options:
           -s, --strain TEXT     Name of the strain (default:genome name)
           -i, --identity FLOAT  Minimum identity to search gene (default=0.95)
           -c, --coverage FLOAT  Minimum coverage to search gene (default=0.9)
```

### Comparing `PyMLST-2.1.3/PyMLST.egg-info/SOURCES.txt` & `PyMLST-2.1.4/PyMLST.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/README.md` & `PyMLST-2.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 - A configuration file for defined PATH to external tools.
 - An easy installation with pypi repository.
 
 
 ## Automatic Installation
 
 ```
-conda install -c bioconda pymlst
+conda install -c bioconda -c conda-forge pymlst
 ```
 
 ## Manual Installation
 ### From pypi repository
 
 ```
 pip install pymlst
@@ -140,15 +140,15 @@
 The scheme is a multi-fasta file containing sequences of genes in nucleotide format.
 You can obtained scheme for:
 	- Core genome analysis in publications.
 	- Whole genome analysis by using annoted genes of a publish genome close to your strains.
 
 ```
 wgMLST create --help
-Usage: wgMLST create [OPTIONS] COREGENE DATABASE
+Usage: wgMLST create [OPTIONS] DATABASE COREGENE
 
   Create a wgMLST DATABASE from a template COREGENE.
 
 Options:
   -f, --force        Override alrealdy existing DATABASE
   -c, --concatenate  Automatically concatenate genes with duplicated sequences
   -r, --remove       Automatically remove genes with duplicated sequences
@@ -158,15 +158,15 @@
 
 Next, you need to add your strain iteratively to the database. 
 A draft genome can be used (we recommend to use [Spades](http://cab.spbu.ru/software/spades/) for assembly).
 You can also add reference genome for comparison.
 
 ```
 wgMLST add --help
-Usage: wgMLST add [OPTIONS] GENOME DATABASE
+Usage: wgMLST add [OPTIONS] DATABASE GENOME
 
   Add a strain GENOME to the wgMLST DATABASE.
 
 Options:
   -s, --strain TEXT     Name of the strain (default:genome name)
   -i, --identity FLOAT  Minimum identity to search gene (default=0.95)
   -c, --coverage FLOAT  Minimum coverage to search gene (default=0.9)
```

### Comparing `PyMLST-2.1.3/pymlst/cla/commands/create.py` & `PyMLST-2.1.4/pymlst/cla/commands/create.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cla/commands/import.py` & `PyMLST-2.1.4/pymlst/cla/commands/import.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cla/commands/remove.py` & `PyMLST-2.1.4/pymlst/cla/commands/remove.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cla/commands/search.py` & `PyMLST-2.1.4/pymlst/cla/commands/search.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cla/commands/search2.py` & `PyMLST-2.1.4/pymlst/cla/commands/search2.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cla/core.py` & `PyMLST-2.1.4/pymlst/cla/core.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cla/model.py` & `PyMLST-2.1.4/pymlst/cla/model.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/cmd.py` & `PyMLST-2.1.4/pymlst/cmd.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/blat.py` & `PyMLST-2.1.4/pymlst/common/blat.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/commands/configure.py` & `PyMLST-2.1.4/pymlst/common/commands/configure.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/exceptions.py` & `PyMLST-2.1.4/pymlst/common/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,7 +55,10 @@
 
 class NothingToRemove(PyMLSTError):
     pass
 
 
 class UndefinedExportType(PyMLSTError):
     pass
+
+class EmptyDatabase(PyMLSTError):
+    pass
```

### Comparing `PyMLST-2.1.3/pymlst/common/kma.py` & `PyMLST-2.1.4/pymlst/common/kma.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/mafft.py` & `PyMLST-2.1.4/pymlst/common/mafft.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/psl.py` & `PyMLST-2.1.4/pymlst/common/psl.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/utils.py` & `PyMLST-2.1.4/pymlst/common/utils.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/common/web.py` & `PyMLST-2.1.4/pymlst/common/web.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/config.py` & `PyMLST-2.1.4/pymlst/config.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/data/alembic/alembic.ini` & `PyMLST-2.1.4/pymlst/data/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/data/alembic/cla/env.py` & `PyMLST-2.1.4/pymlst/data/alembic/cla/env.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/data/alembic/cla/versions/21efe503d07d_initial.py` & `PyMLST-2.1.4/pymlst/data/alembic/cla/versions/21efe503d07d_initial.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/data/alembic/wg/env.py` & `PyMLST-2.1.4/pymlst/data/alembic/wg/env.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/data/alembic/wg/versions/52ae99cb5f33_initial.py` & `PyMLST-2.1.4/pymlst/data/alembic/wg/versions/52ae99cb5f33_initial.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/add.py` & `PyMLST-2.1.4/pymlst/wg/commands/add.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/add2.py` & `PyMLST-2.1.4/pymlst/wg/commands/add2.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/create.py` & `PyMLST-2.1.4/pymlst/wg/commands/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,8 +33,8 @@
         with pymlst.open_wg(os.path.abspath(database)) as mlst:
             mlst.create(**utils.clean_kwargs(kwargs))
 
     except exceptions.DuplicatedGeneSequence as err:
         raise click.UsageError('{}, use -c or -r options to manage it'
                                .format(str(err)))
     except exceptions.PyMLSTError as err:
-        raise click.UsageError(str(err))
+        raise click.ClickException(str(err))
```

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/distance.py` & `PyMLST-2.1.4/pymlst/wg/commands/distance.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/gene.py` & `PyMLST-2.1.4/pymlst/wg/commands/gene.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pymlst
 from pymlst.common import utils, exceptions
 from pymlst.wg.extractors import GeneExtractor, TableExtractorCommand
 
 @click.command(name='gene', cls=TableExtractorCommand)
 @click.option('--output', '-o',
               type=click.File('w'),
-              help='Export MLST table to (default=stdout).')
+              help='Export GENE list to (default=stdout).')
 @click.argument('database', type=click.Path(exists=True))
 def cli(database, **kwargs):
     """Extract an genes list from a wgMLST DATABASE."""
 
     tab_kwargs,out_kwargs = utils.get_output(utils.clean_kwargs(kwargs))
 
     try:
```

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/import.py` & `PyMLST-2.1.4/pymlst/wg/commands/import.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/mlst.py` & `PyMLST-2.1.4/pymlst/wg/commands/mlst.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/msa.py` & `PyMLST-2.1.4/pymlst/wg/commands/msa.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/recombinaison.py` & `PyMLST-2.1.4/pymlst/wg/commands/recombinaison.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/remove.py` & `PyMLST-2.1.4/pymlst/wg/commands/remove.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/sequence.py` & `PyMLST-2.1.4/pymlst/wg/commands/sequence.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/stats.py` & `PyMLST-2.1.4/pymlst/wg/commands/stats.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/strain.py` & `PyMLST-2.1.4/pymlst/wg/commands/strain.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/commands/subgraph.py` & `PyMLST-2.1.4/pymlst/wg/commands/subgraph.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/pymlst/wg/core.py` & `PyMLST-2.1.4/pymlst/wg/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,14 +494,18 @@
 
             if rc_genes:
                 logging.info('Reverse-complemented genes: %s', str(rc_genes))
 
             if invalid_genes:
                 logging.info('Skipped invalid genes: %s', str(invalid_genes))
 
+            if len(self.__database.get_core_genes()) == 0:
+                raise exceptions.InvalidGeneName("No valid gene found\n" + \
+                    "You probably load genome instead of genes")
+
             logging.info('Database initialized')
 
     def add_strain(self, genome, strain=None, identity=0.95, coverage=0.90):
         """Adds a genome strain to the database.
 
         How it works:
```

### Comparing `PyMLST-2.1.3/pymlst/wg/extractors.py` & `PyMLST-2.1.4/pymlst/wg/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,20 +249,22 @@
         self.form = form
 
     def extract(self, base, output):
         valid_shema = super().get_valid_shema(base)
         strains = base.get_all_strains()
         mlst = base.get_mlst(valid_shema)
         table = pd.DataFrame(columns=["#GeneId"] + strains)
+        rows = []
         for gene in valid_shema:
             row = {"#GeneId": gene}
             mlstg = mlst.get(gene, {})
             for strain in strains:
                 row[strain] = mlstg.get(strain, None)
-            table = table.append(row, ignore_index=True)
+            rows.append(row)
+        table = pd.concat([table, pd.DataFrame.from_dict(rows)], ignore_index=True)
         table = table.set_index('#GeneId')
         
         if self.form == 'grapetree':
             if self.duplicate:
                 logging.warnings("Export grapetree table " +
                              "using duplicate genes is not recommended.")
             table = table.fillna(-1)
```

### Comparing `PyMLST-2.1.3/pymlst/wg/model.py` & `PyMLST-2.1.4/pymlst/wg/model.py`

 * *Files identical despite different names*

### Comparing `PyMLST-2.1.3/setup.py` & `PyMLST-2.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,27 +47,27 @@
     long_description_content_type='text/markdown',
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     version=version,
     setup_requires=['wheel'],
     install_requires=[
         # Include dependencies here
-        'biopython~=1.78',
-        'click~=7.1.2',
-        'pytest~=6.2.2',
-        'sqlalchemy~=1.4.15',
-        'networkx~=2.5',
-        'decorator~=4.4.2',
-        'requests~=2.23.0',
-        'pandas~=1.2.1',
-        'numpy~=1.20.0',
-        'beautifulsoup4~=4.9.3',
-        'questionary~=1.9.0',
-        'setuptools~=44.0.0',
-        'alembic~=1.6.2'
+        'biopython>=1.78',
+        'click>=7.1',
+        'pytest>=6.2',
+        'sqlalchemy>=1.4,<2',
+        'networkx>=2.5',
+        'decorator>=4.4',
+        'requests>=2.23',
+        'pandas>=1.2',
+        'numpy>=1.20.0',
+        'beautifulsoup4>=4.9',
+        'questionary>=1.9',
+        'setuptools>=44.0',
+        'alembic>=1.6'
     ],
     entry_points="""
     [console_scripts]
     pyMLST=pymlst.cmd:py
     wgMLST=pymlst.cmd:wg
     claMLST=pymlst.cmd:cla
     """,
```

