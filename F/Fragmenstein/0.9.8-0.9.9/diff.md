# Comparing `tmp/Fragmenstein-0.9.8.tar.gz` & `tmp/Fragmenstein-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fragmenstein-0.9.8.tar", last modified: Wed Jun  8 15:38:11 2022, max compression
+gzip compressed data, was "Fragmenstein-0.9.9.tar", last modified: Wed Jun  8 16:03:41 2022, max compression
```

## Comparing `Fragmenstein-0.9.8.tar` & `Fragmenstein-0.9.9.tar`

### file list

```diff
@@ -1,681 +1,681 @@
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.257278 Fragmenstein-0.9.8/
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:10.625102 Fragmenstein-0.9.8/Fragmenstein.egg-info/
--rw-r--r--   0 matteo     (501) staff       (20)    23486 2022-06-08 15:38:09.000000 Fragmenstein-0.9.8/Fragmenstein.egg-info/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)    27884 2022-06-08 15:38:10.000000 Fragmenstein-0.9.8/Fragmenstein.egg-info/SOURCES.txt
--rw-r--r--   0 matteo     (501) staff       (20)        1 2022-06-08 15:38:09.000000 Fragmenstein-0.9.8/Fragmenstein.egg-info/dependency_links.txt
--rw-r--r--   0 matteo     (501) staff       (20)       55 2022-06-08 15:38:09.000000 Fragmenstein-0.9.8/Fragmenstein.egg-info/entry_points.txt
--rw-r--r--   0 matteo     (501) staff       (20)      320 2022-06-08 15:38:10.000000 Fragmenstein-0.9.8/Fragmenstein.egg-info/requires.txt
--rw-r--r--   0 matteo     (501) staff       (20)       19 2022-06-08 15:38:10.000000 Fragmenstein-0.9.8/Fragmenstein.egg-info/top_level.txt
--rw-r--r--   0 matteo     (501) staff       (20)     1069 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/LICENSE
--rw-r--r--   0 matteo     (501) staff       (20)      317 2022-05-27 17:06:07.000000 Fragmenstein-0.9.8/MANIFEST.in
--rw-r--r--   0 matteo     (501) staff       (20)    23486 2022-06-08 15:38:11.256009 Fragmenstein-0.9.8/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)    22658 2022-06-01 16:23:10.000000 Fragmenstein-0.9.8/README.md
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:10.630380 Fragmenstein-0.9.8/fragmenstein/
--rw-r--r--   0 matteo     (501) staff       (20)     1455 2022-06-01 10:09:11.000000 Fragmenstein-0.9.8/fragmenstein/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     1189 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/branding.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:10.630928 Fragmenstein-0.9.8/fragmenstein/cli/
--rw-r--r--   0 matteo     (501) staff       (20)     4919 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/cli/__init__.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:10.632108 Fragmenstein-0.9.8/fragmenstein/demo/
--rw-r--r--   0 matteo     (501) staff       (20)     2034 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     4035 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/_base_dataset_holder.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:10.781622 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/
--rw-r--r--   0 matteo     (501) staff       (20)        0 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/__init__.py
--rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1592 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1317 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1592 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)      998 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1597 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1164 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      736 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1317 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1343 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1164 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      819 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1343 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      736 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      736 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      998 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      902 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)      902 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      570 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)      570 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      557 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      915 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      915 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)      915 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1605 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1505 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0115.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0116.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1186 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0123.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0124.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1601 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0131.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0132.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0137.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0138.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0139.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1531 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0142.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1614 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0148.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1518 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0159.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1601 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0161.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0163.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0178.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0179.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0180.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0182.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0188.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0190.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1243 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0193.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0204.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0206.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1243 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0212.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0213.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0223.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0224.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0226.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0227.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0228.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0231.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0255.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0263.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0271.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0277.mol
--rw-r--r--   0 matteo     (501) staff       (20)      841 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0282.mol
--rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0283.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0284.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0301.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1243 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0302.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0303.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0305.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0306.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0309.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0319.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0321.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0326.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0328.mol
--rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0333.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0337.mol
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0338.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0341.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0343.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0344.mol
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0345.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0346.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0347.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0348.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0354.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0357.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0358.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0360.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0361.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0365.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2073 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0371.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0373.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0375.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0378.mol
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0379.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0380.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0381.mol
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0385.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0387.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0392.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0394.mol
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0396.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0397.mol
--rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0398.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0402.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0404.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0411.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0412.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0415.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0417.mol
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0433.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0436.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0437.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0439.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1505 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0441.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0444.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0451.mol
--rw-r--r--   0 matteo     (501) staff       (20)      745 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0453.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0455.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0472.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0482.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1671 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0496.mol
--rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0509.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0510.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0511.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0522.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0527.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0546.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0555.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1269 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0564.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0565.mol
--rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0567.mol
--rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0568.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0570.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0572.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0576.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1352 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0582.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1614 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0584.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1326 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0587.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0588.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3121 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0590.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x1493.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1933 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x1494.mol
--rw-r--r--   0 matteo     (501) staff       (20)   208424 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/template.pdb
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.169345 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/
--rw-r--r--   0 matteo     (501) staff       (20)     2850 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6lze.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2933 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2933 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6w63.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol
--rw-r--r--   0 matteo     (501) staff       (20)      723 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol
--rw-r--r--   0 matteo     (501) staff       (20)      723 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol
--rw-r--r--   0 matteo     (501) staff       (20)      723 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol
--rw-r--r--   0 matteo     (501) staff       (20)      819 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol
--rw-r--r--   0 matteo     (501) staff       (20)      404 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xbg.mol
--rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol
--rw-r--r--   0 matteo     (501) staff       (20)      819 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol
--rw-r--r--   0 matteo     (501) staff       (20)      972 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xch.mol
--rw-r--r--   0 matteo     (501) staff       (20)      806 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2920 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol
--rw-r--r--   0 matteo     (501) staff       (20)      640 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3527 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol
--rw-r--r--   0 matteo     (501) staff       (20)      832 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol
--rw-r--r--   0 matteo     (501) staff       (20)      505 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6yz6.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6zru.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2230 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7aku.mol
--rw-r--r--   0 matteo     (501) staff       (20)      754 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7brp.mol
--rw-r--r--   0 matteo     (501) staff       (20)      806 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7buy.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol
--rw-r--r--   0 matteo     (501) staff       (20)      142 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8b.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3820 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7com.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol
--rw-r--r--   0 matteo     (501) staff       (20)      142 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7d1m.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2850 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3527 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol
--rw-r--r--   0 matteo     (501) staff       (20)      391 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7jr4.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3112 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7k40.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0072.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0104.mol
--rw-r--r--   0 matteo     (501) staff       (20)      990 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0107.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1239 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0161.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0165.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0177.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0194.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0195.mol
--rw-r--r--   0 matteo     (501) staff       (20)      990 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0305.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1322 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0336.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0350.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0354.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1597 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0376.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0387.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1597 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0390.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1252 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0395.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0397.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0398.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1348 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0425.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0426.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0434.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0464.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1322 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0478.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0499.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0540.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1252 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0669.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0678.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0689.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0691.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0692.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0705.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0708.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0731.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1693 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0734.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0736.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0748.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0749.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0752.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0755.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0759.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0769.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0770.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0771.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0774.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0786.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0820.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1846 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0830.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0831.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0874.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0887.mol
--rw-r--r--   0 matteo     (501) staff       (20)      990 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0946.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1737 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0967.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1309 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0978.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1392 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0981.mol
--rw-r--r--   0 matteo     (501) staff       (20)      479 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0991.mol
--rw-r--r--   0 matteo     (501) staff       (20)      658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0995.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1930 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10019.mol
--rw-r--r--   0 matteo     (501) staff       (20)      658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1002.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1502 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10022.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10049.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2160 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10082.mol
--rw-r--r--   0 matteo     (501) staff       (20)      658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1012.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2179 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10150.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10155.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1323 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10172.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10178.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1502 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10201.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2179 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10236.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2179 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10237.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10247.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1585 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10248.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10296.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10306.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1668 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10314.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10322.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1943 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10324.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10327.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10329.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1668 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10334.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10338.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10355.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1585 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10359.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1930 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10371.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10377.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10387.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1764 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10392.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10395.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10396.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10403.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1585 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10417.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10419.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1751 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10421.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1751 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10422.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10423.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10466.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10473.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1400 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10474.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10476.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10478.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10484.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10488.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10494.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10506.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10513.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10525.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10535.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10555.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10559.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10565.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10566.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10575.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10598.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10604.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10606.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10610.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10626.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10638.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10645.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10678.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10679.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10700.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10710.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10723.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10728.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10733.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10756.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1077.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10787.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10789.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10800.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10801.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10812.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2352 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10820.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10834.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10856.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1086.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10862.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2697 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10870.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10871.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2435 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10876.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10888.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10889.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10898.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10899.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10900.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10906.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1093.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10942.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10959.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10976.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10995.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10996.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11001.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2593 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1101.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11011.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11013.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11025.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11041.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11044.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1854 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11159.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2518 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11164.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1854 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11186.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1119.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11204.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11208.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1675 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11212.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11223.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11225.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11231.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11233.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11254.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11258.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11271.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11294.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11313.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11317.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11318.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1132.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11339.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11346.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11354.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2269 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11366.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11368.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11372.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11417.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11424.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11426.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11427.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11428.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11431.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11432.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11454.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11458.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11473.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11475.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11485.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11488.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11493.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11498.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11499.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11541.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11562.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11564.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11579.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11587.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11612.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1163.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11642.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11723.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11743.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11764.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2518 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11790.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2435 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11797.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11798.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11801.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11809.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11831.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1187.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11894.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2269 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x12025.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2186 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x12073.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x12080.mol
--rw-r--r--   0 matteo     (501) staff       (20)      907 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1226.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1235.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1252 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1237.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1249.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1308.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1311.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1334.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1336.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1348.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1351.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1358.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1374.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1375.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1380.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1239 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1382.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1384.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1385.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1386.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1392.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1402.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1412.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1418.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1425.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1488 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1458.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1073 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1478.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1493.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2052.mol
--rw-r--r--   0 matteo     (501) staff       (20)      824 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2097.mol
--rw-r--r--   0 matteo     (501) staff       (20)      741 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2119.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2193.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2497 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2540.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1929 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2562.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2563.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2569.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2572.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1929 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2581.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2600.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2608.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2643.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2646.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2649.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2659.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2925 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2694.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2925 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2703.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2925 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2705.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2754.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2764.mol
--rw-r--r--   0 matteo     (501) staff       (20)     3008 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2776.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2779.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2908.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2910.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2912.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1846 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2929.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2964.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2971.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3077.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2261 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3080.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3108.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2829 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3110.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2663 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3113.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2580 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3115.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2759 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3117.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2331 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3124.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2427 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3298.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3303.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2261 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3305.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1322 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3324.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3325.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1488 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3333.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3348.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3351.mol
--rw-r--r--   0 matteo     (501) staff       (20)     2414 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3359.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3366.mol
--rw-r--r--   0 matteo     (501) staff       (20)        0 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)   379172 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/template.pdb
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.181894 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/
--rw-r--r--   0 matteo     (501) staff       (20)    17574 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/5SB7_mergers.sdf
--rw-r--r--   0 matteo     (501) staff       (20)     1254 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/F584.mol
--rw-r--r--   0 matteo     (501) staff       (20)        0 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/__init__.py
--rwxr-xr-x   0 matteo     (501) staff       (20)   467127 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/apo_example1.pdb
--rwxr-xr-x   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/mac-x0138.mol
--rwxr-xr-x   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/mac-x0398.mol
--rw-r--r--   0 matteo     (501) staff       (20)     4580 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/placed_example1.mol
--rw-r--r--   0 matteo     (501) staff       (20)      753 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/rototoluene.mol
--rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/toluene.mol
--rw-r--r--   0 matteo     (501) staff       (20)      758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/transtoluene.mol
--rw-r--r--   0 matteo     (501) staff       (20)      763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/transtoluene2.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/x0032_0A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     1421 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/demo/test_mols/x0103_0A.mol
--rw-r--r--   0 matteo     (501) staff       (20)     6426 2022-06-01 15:02:03.000000 Fragmenstein-0.9.8/fragmenstein/display.py
--rw-r--r--   0 matteo     (501) staff       (20)    56342 2022-05-17 14:51:19.000000 Fragmenstein-0.9.8/fragmenstein/divergent_colors.json
--rw-r--r--   0 matteo     (501) staff       (20)     3842 2022-06-08 11:10:28.000000 Fragmenstein-0.9.8/fragmenstein/extraction_funs.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.186085 Fragmenstein-0.9.8/fragmenstein/igor/
--rw-r--r--   0 matteo     (501) staff       (20)     2412 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/igor/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)      788 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/igor/_igor_base.py
--rw-r--r--   0 matteo     (501) staff       (20)     6669 2022-05-09 11:21:43.000000 Fragmenstein-0.9.8/fragmenstein/igor/_igor_init.py
--rw-r--r--   0 matteo     (501) staff       (20)    18705 2022-06-08 10:27:15.000000 Fragmenstein-0.9.8/fragmenstein/igor/_igor_min.py
--rw-r--r--   0 matteo     (501) staff       (20)     9344 2022-06-08 10:27:15.000000 Fragmenstein-0.9.8/fragmenstein/igor/_igor_utils.py
--rw-r--r--   0 matteo     (501) staff       (20)     1101 2022-06-01 16:48:41.000000 Fragmenstein-0.9.8/fragmenstein/igor/pyrosetta_import.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.190571 Fragmenstein-0.9.8/fragmenstein/laboratory/
--rw-r--r--   0 matteo     (501) staff       (20)      797 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/laboratory/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     6859 2022-05-27 17:06:10.000000 Fragmenstein-0.9.8/fragmenstein/laboratory/_base.py
--rw-r--r--   0 matteo     (501) staff       (20)     2346 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/laboratory/_combine.py
--rw-r--r--   0 matteo     (501) staff       (20)     3639 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/laboratory/_place.py
--rw-r--r--   0 matteo     (501) staff       (20)     1014 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/legacy.py
--rw-r--r--   0 matteo     (501) staff       (20)    15283 2022-05-31 12:46:27.000000 Fragmenstein-0.9.8/fragmenstein/m_rmsd.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.200791 Fragmenstein-0.9.8/fragmenstein/monster/
--rw-r--r--   0 matteo     (501) staff       (20)     6457 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     7932 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/_base.py
--rw-r--r--   0 matteo     (501) staff       (20)    52217 2022-05-27 17:06:10.000000 Fragmenstein-0.9.8/fragmenstein/monster/_collapse_ring.py
--rw-r--r--   0 matteo     (501) staff       (20)     3741 2022-04-25 12:04:35.000000 Fragmenstein-0.9.8/fragmenstein/monster/_combine.py
--rw-r--r--   0 matteo     (501) staff       (20)    18773 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/monster/_communal.py
--rw-r--r--   0 matteo     (501) staff       (20)     6058 2022-04-25 12:34:03.000000 Fragmenstein-0.9.8/fragmenstein/monster/_join_neighboring.py
--rw-r--r--   0 matteo     (501) staff       (20)    16292 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/monster/_merge.py
--rw-r--r--   0 matteo     (501) staff       (20)     1582 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/monster/_modification_logging.py
--rw-r--r--   0 matteo     (501) staff       (20)     7956 2022-06-08 15:26:31.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.208957 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/
--rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     9551 2022-06-08 15:36:38.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_expand.py
--rw-r--r--   0 matteo     (501) staff       (20)     1106 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_full.py
--rw-r--r--   0 matteo     (501) staff       (20)     8275 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_make_chimera.py
--rw-r--r--   0 matteo     (501) staff       (20)     9671 2022-06-01 13:27:36.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_mappings.py
--rw-r--r--   0 matteo     (501) staff       (20)     8156 2022-06-08 15:36:38.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_no_blending.py
--rw-r--r--   0 matteo     (501) staff       (20)     9864 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_partial.py
--rw-r--r--   0 matteo     (501) staff       (20)     6957 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_refine.py
--rw-r--r--   0 matteo     (501) staff       (20)     7213 2022-06-07 17:18:37.000000 Fragmenstein-0.9.8/fragmenstein/monster/_util_compare.py
--rw-r--r--   0 matteo     (501) staff       (20)    16904 2022-06-08 10:27:15.000000 Fragmenstein-0.9.8/fragmenstein/monster/_utility.py
--rw-r--r--   0 matteo     (501) staff       (20)     1939 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/monster/bond_provenance.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.212513 Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/
--rw-r--r--   0 matteo     (501) staff       (20)      342 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)    10974 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/compare_atom.py
--rw-r--r--   0 matteo     (501) staff       (20)     1127 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/types.py
--rw-r--r--   0 matteo     (501) staff       (20)     5354 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/utils.py
--rw-r--r--   0 matteo     (501) staff       (20)     5087 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/monster/positional_mapping.py
--rw-r--r--   0 matteo     (501) staff       (20)    20872 2022-06-08 13:36:38.000000 Fragmenstein-0.9.8/fragmenstein/monster/unmerge_mapper.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.213822 Fragmenstein-0.9.8/fragmenstein/mpro/
--rw-r--r--   0 matteo     (501) staff       (20)     6188 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/mpro/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     1439 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/mpro/dataframe.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.214957 Fragmenstein-0.9.8/fragmenstein/multivictor/
--rw-r--r--   0 matteo     (501) staff       (20)       70 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/multivictor/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     3266 2022-05-30 16:48:53.000000 Fragmenstein-0.9.8/fragmenstein/multivictor/multivictor.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.233953 Fragmenstein-0.9.8/fragmenstein/victor/
--rw-r--r--   0 matteo     (501) staff       (20)     6125 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/victor/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)      802 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/victor/_loggerwriter.py
--rw-r--r--   0 matteo     (501) staff       (20)     8431 2022-06-08 13:32:27.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_base.py
--rw-r--r--   0 matteo     (501) staff       (20)     6579 2022-06-08 11:49:56.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_combine.py
--rw-r--r--   0 matteo     (501) staff       (20)    17182 2022-06-08 10:27:15.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_common.py
--rw-r--r--   0 matteo     (501) staff       (20)     5315 2022-06-08 11:14:33.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_igor.py
--rw-r--r--   0 matteo     (501) staff       (20)     4154 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_journal.py
--rw-r--r--   0 matteo     (501) staff       (20)      829 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_overridables.py
--rw-r--r--   0 matteo     (501) staff       (20)     8312 2022-06-07 15:22:34.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_place.py
--rw-r--r--   0 matteo     (501) staff       (20)     6764 2022-06-07 15:13:41.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_plonk.py
--rw-r--r--   0 matteo     (501) staff       (20)     1792 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_safety.py
--rw-r--r--   0 matteo     (501) staff       (20)     6170 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_show.py
--rw-r--r--   0 matteo     (501) staff       (20)     4674 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_store.py
--rw-r--r--   0 matteo     (501) staff       (20)    22017 2022-06-08 11:10:28.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_utils.py
--rw-r--r--   0 matteo     (501) staff       (20)     2139 2022-06-07 18:00:18.000000 Fragmenstein-0.9.8/fragmenstein/victor/_victor_validate.py
--rw-r--r--   0 matteo     (501) staff       (20)     5650 2022-06-07 15:38:18.000000 Fragmenstein-0.9.8/fragmenstein/victor/minimalPDB.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.243442 Fragmenstein-0.9.8/fragmenstein/walton/
--rw-r--r--   0 matteo     (501) staff       (20)     2279 2022-05-31 12:46:27.000000 Fragmenstein-0.9.8/fragmenstein/walton/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     8226 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/fragmenstein/walton/_advmoves.py
--rw-r--r--   0 matteo     (501) staff       (20)     3214 2022-06-01 13:21:20.000000 Fragmenstein-0.9.8/fragmenstein/walton/_art.py
--rw-r--r--   0 matteo     (501) staff       (20)     3829 2022-05-31 15:49:08.000000 Fragmenstein-0.9.8/fragmenstein/walton/_base.py
--rw-r--r--   0 matteo     (501) staff       (20)     7289 2022-05-31 12:46:27.000000 Fragmenstein-0.9.8/fragmenstein/walton/_movements.py
--rw-r--r--   0 matteo     (501) staff       (20)     1693 2022-04-20 16:14:21.000000 Fragmenstein-0.9.8/fragmenstein/walton/_polygon.py
--rw-r--r--   0 matteo     (501) staff       (20)      862 2022-06-01 14:09:35.000000 Fragmenstein-0.9.8/requirements.txt
--rw-r--r--   0 matteo     (501) staff       (20)       38 2022-06-08 15:38:11.257471 Fragmenstein-0.9.8/setup.cfg
--rw-r--r--   0 matteo     (501) staff       (20)     3212 2022-06-08 15:37:07.000000 Fragmenstein-0.9.8/setup.py
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 15:38:11.253073 Fragmenstein-0.9.8/tests/
--rw-r--r--   0 matteo     (501) staff       (20)     1490 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/MPro_combine.py
--rw-r--r--   0 matteo     (501) staff       (20)     4350 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/MPro_place.py
--rw-r--r--   0 matteo     (501) staff       (20)      378 2022-06-08 11:31:28.000000 Fragmenstein-0.9.8/tests/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     4606 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/internals.py
--rw-r--r--   0 matteo     (501) staff       (20)     5599 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/mapping.py
--rw-r--r--   0 matteo     (501) staff       (20)     4321 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/monster_combine.py
--rw-r--r--   0 matteo     (501) staff       (20)     9082 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/monster_place.py
--rw-r--r--   0 matteo     (501) staff       (20)     1323 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/multivictor.py
--rw-r--r--   0 matteo     (501) staff       (20)     4064 2022-05-27 17:05:56.000000 Fragmenstein-0.9.8/tests/problems.py
--rw-r--r--   0 matteo     (501) staff       (20)     4068 2022-05-31 12:46:27.000000 Fragmenstein-0.9.8/tests/walton.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.657345 Fragmenstein-0.9.9/
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:40.874379 Fragmenstein-0.9.9/Fragmenstein.egg-info/
+-rw-r--r--   0 matteo     (501) staff       (20)    23486 2022-06-08 16:03:39.000000 Fragmenstein-0.9.9/Fragmenstein.egg-info/PKG-INFO
+-rw-r--r--   0 matteo     (501) staff       (20)    27884 2022-06-08 16:03:40.000000 Fragmenstein-0.9.9/Fragmenstein.egg-info/SOURCES.txt
+-rw-r--r--   0 matteo     (501) staff       (20)        1 2022-06-08 16:03:39.000000 Fragmenstein-0.9.9/Fragmenstein.egg-info/dependency_links.txt
+-rw-r--r--   0 matteo     (501) staff       (20)       55 2022-06-08 16:03:40.000000 Fragmenstein-0.9.9/Fragmenstein.egg-info/entry_points.txt
+-rw-r--r--   0 matteo     (501) staff       (20)      320 2022-06-08 16:03:40.000000 Fragmenstein-0.9.9/Fragmenstein.egg-info/requires.txt
+-rw-r--r--   0 matteo     (501) staff       (20)       19 2022-06-08 16:03:40.000000 Fragmenstein-0.9.9/Fragmenstein.egg-info/top_level.txt
+-rw-r--r--   0 matteo     (501) staff       (20)     1069 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/LICENSE
+-rw-r--r--   0 matteo     (501) staff       (20)      317 2022-05-27 17:06:07.000000 Fragmenstein-0.9.9/MANIFEST.in
+-rw-r--r--   0 matteo     (501) staff       (20)    23486 2022-06-08 16:03:41.656761 Fragmenstein-0.9.9/PKG-INFO
+-rw-r--r--   0 matteo     (501) staff       (20)    22658 2022-06-01 16:23:10.000000 Fragmenstein-0.9.9/README.md
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:40.881974 Fragmenstein-0.9.9/fragmenstein/
+-rw-r--r--   0 matteo     (501) staff       (20)     1455 2022-06-01 10:09:11.000000 Fragmenstein-0.9.9/fragmenstein/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1189 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/branding.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:40.882760 Fragmenstein-0.9.9/fragmenstein/cli/
+-rw-r--r--   0 matteo     (501) staff       (20)     4919 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/cli/__init__.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:40.884377 Fragmenstein-0.9.9/fragmenstein/demo/
+-rw-r--r--   0 matteo     (501) staff       (20)     2034 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4035 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/_base_dataset_holder.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.156875 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/
+-rw-r--r--   0 matteo     (501) staff       (20)        0 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/__init__.py
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1592 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1317 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1592 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)      998 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1597 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1164 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      736 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1247 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1317 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1343 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1164 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      819 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1343 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1234 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      736 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      736 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      998 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      902 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      902 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      570 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      570 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      557 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      915 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      915 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1068 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      915 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1605 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1505 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0115.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0116.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1186 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0123.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0124.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1601 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0131.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0132.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0137.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0138.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0139.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1531 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0142.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1614 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0148.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1518 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0159.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1601 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0161.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0163.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0178.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0179.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0180.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0182.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0188.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0190.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1243 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0193.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0204.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0206.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1243 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0212.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0213.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0223.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0224.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0226.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0227.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0228.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0231.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0255.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0263.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0271.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0277.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      841 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0282.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0283.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0284.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0301.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1243 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0302.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0303.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0305.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0306.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0309.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0319.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0321.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0326.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0328.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0333.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0337.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0338.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0341.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0343.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0344.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0345.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0346.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0347.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0348.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0354.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0357.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0358.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0360.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0361.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0365.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2073 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0371.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0373.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0375.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0378.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0379.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0380.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0381.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0385.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0387.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0392.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0394.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0396.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0397.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0398.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0402.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0404.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1160 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0411.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0412.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0415.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0417.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0433.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0436.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0437.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0439.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1505 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0441.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0444.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0451.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      745 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0453.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1077 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0455.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:55.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0472.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0482.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1671 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0496.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0509.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0510.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0511.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0522.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1422 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0527.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0546.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0555.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1269 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0564.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0565.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0567.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0568.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0570.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0572.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0576.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1352 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0582.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1614 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0584.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1326 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0587.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1435 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0588.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3121 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0590.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x1493.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1933 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x1494.mol
+-rw-r--r--   0 matteo     (501) staff       (20)   208424 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/template.pdb
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.516774 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/
+-rw-r--r--   0 matteo     (501) staff       (20)     2850 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6lze.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2933 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2933 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6w63.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      723 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      723 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      723 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      819 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      404 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xbg.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      985 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      819 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      972 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xch.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      806 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2920 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      640 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3527 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      832 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      505 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6yz6.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6zru.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2230 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7aku.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      754 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7brp.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      806 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7buy.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      142 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8b.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3820 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2492 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7com.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      142 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7d1m.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2850 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3527 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      391 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7jr4.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3112 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7k40.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0072.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0104.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      990 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0107.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1239 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0161.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0165.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0177.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0194.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0195.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      990 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0305.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1322 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0336.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0350.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0354.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1597 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0376.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0387.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1597 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0390.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1252 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0395.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0397.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0398.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1348 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0425.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0426.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0434.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0464.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1322 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0478.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0499.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0540.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1252 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0669.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0678.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0689.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0691.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0692.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0705.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0708.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0731.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1693 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0734.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0736.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0748.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0749.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0752.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0755.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0759.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0769.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0770.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0771.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0774.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0786.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0820.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1846 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0830.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0831.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0874.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0887.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      990 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0946.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1737 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0967.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1309 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0978.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1392 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0981.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      479 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0991.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0995.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1930 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10019.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1002.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1502 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10022.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10049.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2160 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10082.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      658 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1012.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2179 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10150.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10155.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1323 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10172.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10178.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1502 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10201.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2179 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10236.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2179 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10237.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10247.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1585 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10248.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10296.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10306.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1668 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10314.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10322.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1943 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10324.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10327.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10329.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1668 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10334.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10338.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10355.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1585 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10359.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1930 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10371.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10377.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10387.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1764 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10392.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10395.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10396.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2013 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10403.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1585 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10417.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10419.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1751 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10421.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1751 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10422.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1834 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10423.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10466.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10473.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1400 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10474.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10476.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10478.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10484.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10488.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10494.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10506.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10513.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10525.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10535.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10555.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10559.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10565.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10566.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10575.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10598.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10604.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10606.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10610.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10626.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10638.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10645.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10678.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10679.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10700.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10710.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10723.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10728.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10733.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10756.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1077.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10787.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10789.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10800.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10801.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1081 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10812.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2352 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10820.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10834.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10856.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1086.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10862.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2697 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10870.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10871.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2435 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10876.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10888.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10889.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10898.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10899.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10900.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10906.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1093.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10942.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10959.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10976.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10995.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10996.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11001.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2593 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1101.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11011.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11013.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11025.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11041.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11044.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1854 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11159.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2518 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11164.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1854 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11186.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1119.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11204.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11208.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1675 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11212.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11223.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11225.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11231.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1937 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11233.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11254.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11258.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11271.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11294.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11313.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11317.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11318.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1132.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1330 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11339.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11346.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11354.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2269 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11366.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11368.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11372.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1745 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11417.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11424.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1413 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11426.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1662 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11427.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11428.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11431.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11432.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11454.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1924 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11458.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1496 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11473.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11475.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1579 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11485.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11488.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11493.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11498.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11499.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11541.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11562.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2339 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11564.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1911 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11579.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11587.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11612.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1163.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11642.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2256 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11723.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11743.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2173 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11764.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2518 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11790.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2435 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11797.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2601 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11798.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11801.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1841 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11809.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2103 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11831.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1335 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1187.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11894.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2269 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x12025.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2186 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x12073.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x12080.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      907 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1226.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1235.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1252 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1237.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1249.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1308.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1311.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1334.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1336.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1348.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1351.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1358.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1374.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1375.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1380.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1239 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1382.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1384.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1385.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1386.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1392.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1402.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1501 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1412.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1418.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1425.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1488 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1458.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1073 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1478.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1156 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1493.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2052.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      824 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2097.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      741 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2119.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2193.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2497 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2540.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1929 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2562.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2563.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2569.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2572.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1929 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2581.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2600.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2608.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2643.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2646.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2649.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2659.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2925 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2694.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2925 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2703.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2925 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2705.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2754.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1667 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2764.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     3008 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2776.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1418 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2779.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2908.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2178 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2910.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1750 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2912.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1846 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2929.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1584 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2964.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2971.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1680 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3077.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2261 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3080.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1833 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3108.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2829 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3110.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2663 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3113.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2580 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3115.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2759 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3117.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2331 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3124.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2427 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3298.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2191 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3303.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2261 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3305.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1322 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3324.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1151 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3325.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1488 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3333.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2007 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3348.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1169 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3351.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     2414 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3359.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3366.mol
+-rw-r--r--   0 matteo     (501) staff       (20)        0 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)   379172 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/template.pdb
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.561243 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/
+-rw-r--r--   0 matteo     (501) staff       (20)    17574 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/5SB7_mergers.sdf
+-rw-r--r--   0 matteo     (501) staff       (20)     1254 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/F584.mol
+-rw-r--r--   0 matteo     (501) staff       (20)        0 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/__init__.py
+-rwxr-xr-x   0 matteo     (501) staff       (20)   467127 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/apo_example1.pdb
+-rwxr-xr-x   0 matteo     (501) staff       (20)     1090 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/mac-x0138.mol
+-rwxr-xr-x   0 matteo     (501) staff       (20)      994 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/mac-x0398.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     4580 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/placed_example1.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      753 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/rototoluene.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      653 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/toluene.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      758 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/transtoluene.mol
+-rw-r--r--   0 matteo     (501) staff       (20)      763 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/transtoluene2.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1509 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/x0032_0A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     1421 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/demo/test_mols/x0103_0A.mol
+-rw-r--r--   0 matteo     (501) staff       (20)     6426 2022-06-01 15:02:03.000000 Fragmenstein-0.9.9/fragmenstein/display.py
+-rw-r--r--   0 matteo     (501) staff       (20)    56342 2022-05-17 14:51:19.000000 Fragmenstein-0.9.9/fragmenstein/divergent_colors.json
+-rw-r--r--   0 matteo     (501) staff       (20)     3842 2022-06-08 11:10:28.000000 Fragmenstein-0.9.9/fragmenstein/extraction_funs.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.568198 Fragmenstein-0.9.9/fragmenstein/igor/
+-rw-r--r--   0 matteo     (501) staff       (20)     2412 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/igor/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)      788 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/igor/_igor_base.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6669 2022-05-09 11:21:43.000000 Fragmenstein-0.9.9/fragmenstein/igor/_igor_init.py
+-rw-r--r--   0 matteo     (501) staff       (20)    18705 2022-06-08 10:27:15.000000 Fragmenstein-0.9.9/fragmenstein/igor/_igor_min.py
+-rw-r--r--   0 matteo     (501) staff       (20)     9344 2022-06-08 10:27:15.000000 Fragmenstein-0.9.9/fragmenstein/igor/_igor_utils.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1101 2022-06-01 16:48:41.000000 Fragmenstein-0.9.9/fragmenstein/igor/pyrosetta_import.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.571824 Fragmenstein-0.9.9/fragmenstein/laboratory/
+-rw-r--r--   0 matteo     (501) staff       (20)      797 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/laboratory/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6859 2022-05-27 17:06:10.000000 Fragmenstein-0.9.9/fragmenstein/laboratory/_base.py
+-rw-r--r--   0 matteo     (501) staff       (20)     2346 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/laboratory/_combine.py
+-rw-r--r--   0 matteo     (501) staff       (20)     3639 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/laboratory/_place.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1014 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/legacy.py
+-rw-r--r--   0 matteo     (501) staff       (20)    15283 2022-05-31 12:46:27.000000 Fragmenstein-0.9.9/fragmenstein/m_rmsd.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.588339 Fragmenstein-0.9.9/fragmenstein/monster/
+-rw-r--r--   0 matteo     (501) staff       (20)     6457 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     7932 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/_base.py
+-rw-r--r--   0 matteo     (501) staff       (20)    52217 2022-05-27 17:06:10.000000 Fragmenstein-0.9.9/fragmenstein/monster/_collapse_ring.py
+-rw-r--r--   0 matteo     (501) staff       (20)     3741 2022-04-25 12:04:35.000000 Fragmenstein-0.9.9/fragmenstein/monster/_combine.py
+-rw-r--r--   0 matteo     (501) staff       (20)    18773 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/monster/_communal.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6058 2022-04-25 12:34:03.000000 Fragmenstein-0.9.9/fragmenstein/monster/_join_neighboring.py
+-rw-r--r--   0 matteo     (501) staff       (20)    16292 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/monster/_merge.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1582 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/monster/_modification_logging.py
+-rw-r--r--   0 matteo     (501) staff       (20)     7956 2022-06-08 15:26:31.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.595544 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/
+-rw-r--r--   0 matteo     (501) staff       (20)      828 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     9551 2022-06-08 15:36:38.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_expand.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1106 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_full.py
+-rw-r--r--   0 matteo     (501) staff       (20)     8275 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_make_chimera.py
+-rw-r--r--   0 matteo     (501) staff       (20)     9671 2022-06-01 13:27:36.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_mappings.py
+-rw-r--r--   0 matteo     (501) staff       (20)     8156 2022-06-08 15:36:38.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_no_blending.py
+-rw-r--r--   0 matteo     (501) staff       (20)     9864 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_partial.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6957 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_refine.py
+-rw-r--r--   0 matteo     (501) staff       (20)     7213 2022-06-07 17:18:37.000000 Fragmenstein-0.9.9/fragmenstein/monster/_util_compare.py
+-rw-r--r--   0 matteo     (501) staff       (20)    16904 2022-06-08 10:27:15.000000 Fragmenstein-0.9.9/fragmenstein/monster/_utility.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1939 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/monster/bond_provenance.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.602577 Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/
+-rw-r--r--   0 matteo     (501) staff       (20)      342 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)    10974 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/compare_atom.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1127 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/types.py
+-rw-r--r--   0 matteo     (501) staff       (20)     5354 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/utils.py
+-rw-r--r--   0 matteo     (501) staff       (20)     5087 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/monster/positional_mapping.py
+-rw-r--r--   0 matteo     (501) staff       (20)    21192 2022-06-08 15:55:12.000000 Fragmenstein-0.9.9/fragmenstein/monster/unmerge_mapper.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.605477 Fragmenstein-0.9.9/fragmenstein/mpro/
+-rw-r--r--   0 matteo     (501) staff       (20)     6188 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/mpro/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1439 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/mpro/dataframe.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.607170 Fragmenstein-0.9.9/fragmenstein/multivictor/
+-rw-r--r--   0 matteo     (501) staff       (20)       70 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/multivictor/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     3266 2022-05-30 16:48:53.000000 Fragmenstein-0.9.9/fragmenstein/multivictor/multivictor.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.631856 Fragmenstein-0.9.9/fragmenstein/victor/
+-rw-r--r--   0 matteo     (501) staff       (20)     6125 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/victor/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)      802 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/victor/_loggerwriter.py
+-rw-r--r--   0 matteo     (501) staff       (20)     8431 2022-06-08 13:32:27.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_base.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6579 2022-06-08 11:49:56.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_combine.py
+-rw-r--r--   0 matteo     (501) staff       (20)    17182 2022-06-08 10:27:15.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_common.py
+-rw-r--r--   0 matteo     (501) staff       (20)     5315 2022-06-08 11:14:33.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_igor.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4154 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_journal.py
+-rw-r--r--   0 matteo     (501) staff       (20)      829 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_overridables.py
+-rw-r--r--   0 matteo     (501) staff       (20)     8312 2022-06-07 15:22:34.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_place.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6764 2022-06-07 15:13:41.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_plonk.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1792 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_safety.py
+-rw-r--r--   0 matteo     (501) staff       (20)     6170 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_show.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4674 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_store.py
+-rw-r--r--   0 matteo     (501) staff       (20)    22017 2022-06-08 11:10:28.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_utils.py
+-rw-r--r--   0 matteo     (501) staff       (20)     2139 2022-06-07 18:00:18.000000 Fragmenstein-0.9.9/fragmenstein/victor/_victor_validate.py
+-rw-r--r--   0 matteo     (501) staff       (20)     5650 2022-06-07 15:38:18.000000 Fragmenstein-0.9.9/fragmenstein/victor/minimalPDB.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.637150 Fragmenstein-0.9.9/fragmenstein/walton/
+-rw-r--r--   0 matteo     (501) staff       (20)     2279 2022-05-31 12:46:27.000000 Fragmenstein-0.9.9/fragmenstein/walton/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     8226 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/fragmenstein/walton/_advmoves.py
+-rw-r--r--   0 matteo     (501) staff       (20)     3214 2022-06-01 13:21:20.000000 Fragmenstein-0.9.9/fragmenstein/walton/_art.py
+-rw-r--r--   0 matteo     (501) staff       (20)     3829 2022-05-31 15:49:08.000000 Fragmenstein-0.9.9/fragmenstein/walton/_base.py
+-rw-r--r--   0 matteo     (501) staff       (20)     7289 2022-05-31 12:46:27.000000 Fragmenstein-0.9.9/fragmenstein/walton/_movements.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1693 2022-04-20 16:14:21.000000 Fragmenstein-0.9.9/fragmenstein/walton/_polygon.py
+-rw-r--r--   0 matteo     (501) staff       (20)      862 2022-06-01 14:09:35.000000 Fragmenstein-0.9.9/requirements.txt
+-rw-r--r--   0 matteo     (501) staff       (20)       38 2022-06-08 16:03:41.657529 Fragmenstein-0.9.9/setup.cfg
+-rw-r--r--   0 matteo     (501) staff       (20)     3212 2022-06-08 16:03:34.000000 Fragmenstein-0.9.9/setup.py
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2022-06-08 16:03:41.655678 Fragmenstein-0.9.9/tests/
+-rw-r--r--   0 matteo     (501) staff       (20)     1490 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/MPro_combine.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4350 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/MPro_place.py
+-rw-r--r--   0 matteo     (501) staff       (20)      378 2022-06-08 11:31:28.000000 Fragmenstein-0.9.9/tests/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4606 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/internals.py
+-rw-r--r--   0 matteo     (501) staff       (20)     5599 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/mapping.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4321 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/monster_combine.py
+-rw-r--r--   0 matteo     (501) staff       (20)     9082 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/monster_place.py
+-rw-r--r--   0 matteo     (501) staff       (20)     1323 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/multivictor.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4064 2022-05-27 17:05:56.000000 Fragmenstein-0.9.9/tests/problems.py
+-rw-r--r--   0 matteo     (501) staff       (20)     4068 2022-05-31 12:46:27.000000 Fragmenstein-0.9.9/tests/walton.py
```

### Comparing `Fragmenstein-0.9.8/Fragmenstein.egg-info/PKG-INFO` & `Fragmenstein-0.9.9/Fragmenstein.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fragmenstein
-Version: 0.9.8
+Version: 0.9.9
 Summary: Scaffold hopping between bound compounds by stitching them together like a reanimated corpse
 Home-page: https://github.com/matteoferla/Fragmenstein
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Fragmenstein-0.9.8/Fragmenstein.egg-info/SOURCES.txt` & `Fragmenstein-0.9.9/Fragmenstein.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/LICENSE` & `Fragmenstein-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/PKG-INFO` & `Fragmenstein-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fragmenstein
-Version: 0.9.8
+Version: 0.9.9
 Summary: Scaffold hopping between bound compounds by stitching them together like a reanimated corpse
 Home-page: https://github.com/matteoferla/Fragmenstein
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Fragmenstein-0.9.8/README.md` & `Fragmenstein-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/branding.py` & `Fragmenstein-0.9.9/fragmenstein/branding.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/cli/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/_base_dataset_holder.py` & `Fragmenstein-0.9.9/fragmenstein/demo/_base_dataset_holder.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0091_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0104_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0128_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0142_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0158_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0159_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0173_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0216_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0228_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0253_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0259_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0282_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0290_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0299_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0301_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0334_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0371_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0380_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0417_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0421_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0423_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0436_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0438_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0465_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0469_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0471_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0496_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0516_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0524_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0548_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0548_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0574_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0587_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0591_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0592_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0598_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0600_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0626_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0628_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0631_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0655_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0662_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0676_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0681_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0685_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0689_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0711_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0722_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0724_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0727_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0729_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0737_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0742_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0766_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0792_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0796_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0797_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0805_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0814_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0822_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0837_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0844_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0849_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0852_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0855_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0864_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0895_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0900_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0905_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0905_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0910_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0918_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0926_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0933_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0950_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0962_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0967_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x0969_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1012_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1015_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1018_A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/diamond-x1092_B.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0115.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0115.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0116.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0116.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0123.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0123.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0124.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0124.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0131.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0131.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0132.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0132.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0137.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0137.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0138.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0138.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0139.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0139.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0142.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0142.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0148.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0148.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0159.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0159.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0161.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0161.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0163.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0163.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0178.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0178.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0179.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0179.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0180.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0180.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0182.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0182.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0188.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0188.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0190.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0190.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0193.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0193.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0204.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0204.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0206.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0206.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0212.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0212.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0213.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0213.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0223.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0223.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0224.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0224.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0226.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0226.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0227.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0227.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0228.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0228.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0231.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0231.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0255.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0255.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0263.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0263.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0271.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0271.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0277.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0277.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0282.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0282.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0283.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0283.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0284.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0284.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0301.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0301.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0302.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0302.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0303.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0303.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0305.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0306.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0306.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0309.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0309.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0319.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0319.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0321.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0321.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0326.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0326.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0328.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0328.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0333.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0333.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0337.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0337.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0338.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0338.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0341.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0341.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0343.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0343.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0344.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0344.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0345.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0345.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0346.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0346.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0347.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0347.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0348.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0354.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0357.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0357.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0358.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0358.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0360.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0360.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0361.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0361.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0365.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0365.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0371.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0371.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0373.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0373.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0375.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0375.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0378.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0378.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0379.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0379.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0380.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0380.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0381.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0381.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0385.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0385.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0387.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0392.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0394.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0394.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0396.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0396.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0397.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0397.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0398.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0402.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0402.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0404.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0404.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0411.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0411.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0412.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0412.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0415.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0415.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0417.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0433.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0433.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0436.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0436.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0437.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0437.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0439.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0439.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0441.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0441.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0444.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0444.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0451.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0451.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0453.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0453.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0455.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0455.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0472.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0472.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0482.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0482.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0496.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0496.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0509.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0509.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0510.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0510.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0511.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0511.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0522.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0522.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0527.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0527.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0546.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0546.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0555.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0555.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0564.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0564.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0565.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0565.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0567.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0567.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0568.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0568.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0570.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0570.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0572.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0572.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0576.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0576.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0582.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0582.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0584.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0584.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0587.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0587.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0588.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0588.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x0590.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x0590.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x1493.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x1493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/mac-x1494.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/mac-x1494.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mac1_mols/template.pdb` & `Fragmenstein-0.9.9/fragmenstein/demo/mac1_mols/template.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6lze.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6lze.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6m0k.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6m2n.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6w63.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6w63.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wnp.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wtj.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wtk.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6wtt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xa4.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xb0.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xb1.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xb2.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xbh.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xbi.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xch.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xch.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xfn.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xhm.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xkf.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xmk.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xqs.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xqt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xqu.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6xr3.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6y2f.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6y2g.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6ynq.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6yt8.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6yvf.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6zrt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-6zru.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-6zru.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7aku.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7aku.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7bqy.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7brp.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7brp.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7buy.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7buy.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c6s.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c6u.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c7p.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8r.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8t.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7c8u.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7cbt.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7com.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7com.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7cx9.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7d1o.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7d3i.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7jkv.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7ju7.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7jyc.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7k40.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7k40.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7k6d.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7k6e.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-7kfj.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0072.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0072.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0104.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0104.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0107.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0107.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0161.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0161.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0165.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0165.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0177.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0177.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0194.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0194.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0195.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0195.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0305.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0336.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0336.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0350.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0350.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0354.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0376.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0376.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0387.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0390.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0390.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0395.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0395.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0397.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0397.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0398.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0425.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0425.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0426.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0426.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0434.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0434.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0464.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0464.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0478.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0499.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0499.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0540.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0540.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0669.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0669.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0678.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0678.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0689.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0689.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0691.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0691.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0692.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0692.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0705.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0705.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0708.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0708.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0731.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0731.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0734.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0734.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0736.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0736.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0748.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0748.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0749.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0749.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0752.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0752.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0755.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0755.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0759.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0759.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0769.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0769.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0770.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0770.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0771.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0771.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0774.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0774.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0786.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0786.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0820.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0820.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0830.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0830.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0831.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0831.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0874.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0874.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0887.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0887.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0946.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0946.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0967.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0967.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0978.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0978.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0981.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0981.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x0995.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x0995.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10019.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10019.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1002.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1002.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10022.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10022.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10049.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10049.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10082.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10082.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1012.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1012.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10150.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10150.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10155.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10155.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10172.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10172.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10178.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10178.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10201.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10201.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10236.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10236.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10237.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10237.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10247.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10247.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10248.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10248.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10296.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10296.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10306.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10306.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10314.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10314.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10322.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10322.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10324.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10324.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10327.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10327.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10329.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10329.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10334.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10334.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10338.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10338.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10355.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10355.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10359.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10359.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10371.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10371.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10377.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10377.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10387.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10387.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10392.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10395.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10395.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10396.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10396.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10403.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10403.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10417.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10419.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10419.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10421.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10421.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10422.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10422.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10423.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10423.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10466.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10466.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10473.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10473.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10474.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10474.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10476.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10476.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10478.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10484.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10484.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10488.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10488.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10494.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10494.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10506.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10506.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10513.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10513.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10525.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10525.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10535.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10535.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10555.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10555.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10559.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10559.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10565.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10565.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10566.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10566.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10575.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10575.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10598.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10598.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10604.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10604.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10606.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10606.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10610.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10610.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10626.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10626.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10638.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10638.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10645.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10645.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10678.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10678.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10679.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10679.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10700.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10700.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10710.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10710.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10723.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10723.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10728.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10728.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10733.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10733.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10756.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10756.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1077.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1077.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10787.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10787.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10789.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10789.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10800.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10800.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10801.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10801.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10812.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10812.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10820.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10820.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10834.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10834.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10856.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10856.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1086.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1086.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10862.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10862.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10870.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10870.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10871.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10871.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10876.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10876.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10888.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10888.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10889.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10889.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10898.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10898.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10899.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10899.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10900.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10900.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10906.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10906.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1093.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1093.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10942.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10942.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10959.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10959.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10976.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10976.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10995.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10995.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x10996.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x10996.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11001.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11001.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1101.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1101.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11011.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11011.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11013.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11013.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11025.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11025.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11041.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11041.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11044.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11044.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11159.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11159.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11164.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11164.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11186.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11186.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1119.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1119.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11204.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11204.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11208.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11208.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11212.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11212.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11223.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11223.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11225.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11225.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11231.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11231.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11233.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11233.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11254.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11254.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11258.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11258.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11271.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11271.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11294.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11294.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11313.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11313.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11317.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11317.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11318.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11318.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1132.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1132.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11339.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11339.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11346.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11346.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11354.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11354.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11366.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11366.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11368.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11368.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11372.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11372.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11417.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11417.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11424.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11424.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11426.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11426.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11427.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11427.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11428.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11428.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11431.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11431.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11432.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11432.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11454.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11454.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11458.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11458.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11473.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11473.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11475.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11475.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11485.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11485.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11488.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11488.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11493.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11498.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11498.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11499.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11499.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11541.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11541.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11562.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11562.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11564.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11564.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11579.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11579.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11587.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11587.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11612.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11612.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1163.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1163.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11642.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11642.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11723.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11723.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11743.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11743.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11764.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11764.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11790.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11790.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11797.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11797.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11798.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11798.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11801.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11801.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11809.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11809.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11831.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11831.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1187.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1187.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x11894.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x11894.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x12025.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x12025.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x12073.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x12073.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x12080.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x12080.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1226.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1226.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1235.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1235.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1237.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1237.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1249.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1249.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1308.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1308.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1311.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1311.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1334.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1334.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1336.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1336.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1348.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1351.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1351.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1358.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1358.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1374.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1374.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1375.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1375.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1380.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1380.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1382.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1382.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1384.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1384.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1385.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1385.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1386.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1386.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1392.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1392.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1402.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1402.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1412.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1412.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1418.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1418.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1425.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1425.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1458.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1458.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1478.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1478.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x1493.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x1493.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2052.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2052.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2097.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2097.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2119.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2119.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2193.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2193.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2540.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2540.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2562.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2562.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2563.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2563.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2569.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2569.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2572.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2572.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2581.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2581.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2600.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2600.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2608.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2608.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2643.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2643.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2646.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2646.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2649.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2649.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2659.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2659.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2694.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2694.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2703.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2703.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2705.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2705.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2754.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2754.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2764.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2764.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2776.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2776.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2779.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2779.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2908.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2908.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2910.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2910.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2912.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2912.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2929.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2929.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2964.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2964.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x2971.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x2971.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3077.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3077.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3080.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3080.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3108.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3108.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3110.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3110.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3113.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3113.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3115.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3115.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3117.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3117.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3124.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3124.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3298.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3298.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3303.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3303.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3305.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3305.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3324.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3324.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3325.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3325.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3333.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3333.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3348.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3348.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3351.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3351.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3359.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3359.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/Mpro-x3366.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/Mpro-x3366.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/mpro_mols/template.pdb` & `Fragmenstein-0.9.9/fragmenstein/demo/mpro_mols/template.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/5SB7_mergers.sdf` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/5SB7_mergers.sdf`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/F584.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/F584.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/apo_example1.pdb` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/apo_example1.pdb`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/mac-x0138.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/mac-x0138.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/mac-x0398.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/mac-x0398.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/placed_example1.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/placed_example1.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/rototoluene.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/rototoluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/toluene.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/toluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/transtoluene.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/transtoluene.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/transtoluene2.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/transtoluene2.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/x0032_0A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/x0032_0A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/demo/test_mols/x0103_0A.mol` & `Fragmenstein-0.9.9/fragmenstein/demo/test_mols/x0103_0A.mol`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/display.py` & `Fragmenstein-0.9.9/fragmenstein/display.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/divergent_colors.json` & `Fragmenstein-0.9.9/fragmenstein/divergent_colors.json`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/extraction_funs.py` & `Fragmenstein-0.9.9/fragmenstein/extraction_funs.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/igor/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/igor/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/igor/_igor_base.py` & `Fragmenstein-0.9.9/fragmenstein/igor/_igor_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/igor/_igor_init.py` & `Fragmenstein-0.9.9/fragmenstein/igor/_igor_init.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/igor/_igor_min.py` & `Fragmenstein-0.9.9/fragmenstein/igor/_igor_min.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/igor/_igor_utils.py` & `Fragmenstein-0.9.9/fragmenstein/igor/_igor_utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/igor/pyrosetta_import.py` & `Fragmenstein-0.9.9/fragmenstein/igor/pyrosetta_import.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/laboratory/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/laboratory/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/laboratory/_base.py` & `Fragmenstein-0.9.9/fragmenstein/laboratory/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/laboratory/_combine.py` & `Fragmenstein-0.9.9/fragmenstein/laboratory/_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/laboratory/_place.py` & `Fragmenstein-0.9.9/fragmenstein/laboratory/_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/legacy.py` & `Fragmenstein-0.9.9/fragmenstein/legacy.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/m_rmsd.py` & `Fragmenstein-0.9.9/fragmenstein/m_rmsd.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/monster/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_base.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_collapse_ring.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_collapse_ring.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_combine.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_communal.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_communal.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_join_neighboring.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_join_neighboring.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_merge.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_merge.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_modification_logging.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_modification_logging.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_expand.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_expand.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_full.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_full.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_make_chimera.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_make_chimera.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_mappings.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_mappings.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_no_blending.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_no_blending.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_partial.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_partial.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_place_modes/_refine.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_place_modes/_refine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_util_compare.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_util_compare.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/_utility.py` & `Fragmenstein-0.9.9/fragmenstein/monster/_utility.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/bond_provenance.py` & `Fragmenstein-0.9.9/fragmenstein/monster/bond_provenance.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/compare_atom.py` & `Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/compare_atom.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/types.py` & `Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/types.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/mcs_mapping/utils.py` & `Fragmenstein-0.9.9/fragmenstein/monster/mcs_mapping/utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/positional_mapping.py` & `Fragmenstein-0.9.9/fragmenstein/monster/positional_mapping.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/monster/unmerge_mapper.py` & `Fragmenstein-0.9.9/fragmenstein/monster/unmerge_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,24 +376,29 @@
             return {}
         elif not self.check_possible_distances(other, possible_map, combined, combined_map,
                                                cutoff=self.distance_cutoff):
             return {}
         else:
             return possible_map
 
-    def check_possible_distances(self, other, possible_map, combined, combined_map, cutoff=3):
+    def check_possible_distances(self, other, possible_map, combined, combined_map, cutoff=2.5):
         for i, offset_o in possible_map.items():
             unoffset_o = offset_o - combined.GetNumAtoms()
             atom = self.followup.GetAtomWithIdx(i)
             for neigh in atom.GetNeighbors():
                 ni = neigh.GetIdx()
                 if ni in possible_map:
                     pass  # assuming the inspiration compound was not janky
                 elif ni in combined_map:
-                    if self.get_inter_distance(other, combined, unoffset_o, combined_map[ni]) > cutoff:
+                    separation = self.get_inter_distance(other, combined, unoffset_o, combined_map[ni])
+                    # removing the distance cutoff is a bad idea as the next atoms along with be stretched
+                    # but on others it is fine.
+                    if separation > cutoff * 2:  # very bad.
+                        return False
+                    elif separation > cutoff:  # moderately bad.
                         self.poisonous_indices.append(i)
                         self.poisonous_indices.append(ni)
                         return False
                 else:
                     pass  # unmapped neighbor
         return True
```

### Comparing `Fragmenstein-0.9.8/fragmenstein/mpro/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/mpro/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/mpro/dataframe.py` & `Fragmenstein-0.9.9/fragmenstein/mpro/dataframe.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/multivictor/multivictor.py` & `Fragmenstein-0.9.9/fragmenstein/multivictor/multivictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/victor/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_loggerwriter.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_loggerwriter.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_base.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_combine.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_common.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_common.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_igor.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_igor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_journal.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_journal.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_overridables.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_overridables.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_place.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_plonk.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_plonk.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_safety.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_safety.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_show.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_show.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_store.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_store.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_utils.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_utils.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/_victor_validate.py` & `Fragmenstein-0.9.9/fragmenstein/victor/_victor_validate.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/victor/minimalPDB.py` & `Fragmenstein-0.9.9/fragmenstein/victor/minimalPDB.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/walton/__init__.py` & `Fragmenstein-0.9.9/fragmenstein/walton/__init__.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/walton/_advmoves.py` & `Fragmenstein-0.9.9/fragmenstein/walton/_advmoves.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/walton/_art.py` & `Fragmenstein-0.9.9/fragmenstein/walton/_art.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/walton/_base.py` & `Fragmenstein-0.9.9/fragmenstein/walton/_base.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/walton/_movements.py` & `Fragmenstein-0.9.9/fragmenstein/walton/_movements.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/fragmenstein/walton/_polygon.py` & `Fragmenstein-0.9.9/fragmenstein/walton/_polygon.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/requirements.txt` & `Fragmenstein-0.9.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/setup.py` & `Fragmenstein-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 if not util.find_spec('pymol2'):
     warn('The module pymol2 is optionally required (conda or apt-get installable).')
 
 
 
 setup(
     name='Fragmenstein',
-    version='0.9.8',
+    version='0.9.9',
     description='Scaffold hopping between bound compounds by stitching them together like a reanimated corpse',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.7',
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
```

### Comparing `Fragmenstein-0.9.8/tests/MPro_combine.py` & `Fragmenstein-0.9.9/tests/MPro_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/MPro_place.py` & `Fragmenstein-0.9.9/tests/MPro_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/internals.py` & `Fragmenstein-0.9.9/tests/internals.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/mapping.py` & `Fragmenstein-0.9.9/tests/mapping.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/monster_combine.py` & `Fragmenstein-0.9.9/tests/monster_combine.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/monster_place.py` & `Fragmenstein-0.9.9/tests/monster_place.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/multivictor.py` & `Fragmenstein-0.9.9/tests/multivictor.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/problems.py` & `Fragmenstein-0.9.9/tests/problems.py`

 * *Files identical despite different names*

### Comparing `Fragmenstein-0.9.8/tests/walton.py` & `Fragmenstein-0.9.9/tests/walton.py`

 * *Files identical despite different names*

