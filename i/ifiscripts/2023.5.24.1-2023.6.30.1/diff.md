# Comparing `tmp/ifiscripts-2023.5.24.1.tar.gz` & `tmp/ifiscripts-2023.6.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifiscripts-2023.5.24.1.tar", last modified: Wed May 24 12:26:30 2023, max compression
+gzip compressed data, was "ifiscripts-2023.6.30.1.tar", last modified: Fri Jun 30 17:05:40 2023, max compression
```

## Comparing `ifiscripts-2023.5.24.1.tar` & `ifiscripts-2023.6.30.1.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:26:30.639515 ifiscripts-2023.5.24.1/
--rw-rw-rw-   0        0        0   970313 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/26_XYZ-22_Rec709.cube
--rw-rw-rw-   0        0        0     1116 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/LICENSE.txt
--rw-rw-rw-   0        0        0       70 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1130 2023-05-24 12:26:30.638512 ifiscripts-2023.5.24.1/PKG-INFO
--rw-rw-rw-   0        0        0     4611 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/README.rst
--rw-rw-rw-   0        0        0     5029 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/film_scan_aip_documentation.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 12:26:30.548983 ifiscripts-2023.5.24.1/ifiscripts.egg-info/
--rw-rw-rw-   0        0        0     1130 2023-05-24 12:26:30.000000 ifiscripts-2023.5.24.1/ifiscripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1666 2023-05-24 12:26:30.000000 ifiscripts-2023.5.24.1/ifiscripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:26:30.000000 ifiscripts-2023.5.24.1/ifiscripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-24 12:26:30.000000 ifiscripts-2023.5.24.1/ifiscripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-24 12:26:30.000000 ifiscripts-2023.5.24.1/ifiscripts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 12:26:30.573983 ifiscripts-2023.5.24.1/legacy_scripts/
--rw-rw-rw-   0        0        0     2872 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/batchfixity.py
--rw-rw-rw-   0        0        0     1599 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/db_cleaning.py
--rw-rw-rw-   0        0        0    11222 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/dpxonly.py
--rw-rw-rw-   0        0        0     5019 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/dvsip.py
--rw-rw-rw-   0        0        0     1004 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/giffer.py
--rw-rw-rw-   0        0        0      989 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/loopline.py
--rw-rw-rw-   0        0        0    11528 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/makedpx.py
--rw-rw-rw-   0        0        0      851 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/mezzaninecheck.py
--rw-rw-rw-   0        0        0     1720 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/oeremove.py
--rw-rw-rw-   0        0        0     3803 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/pg.py
--rw-rw-rw-   0        0        0     3065 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/playerseq.py
--rw-rw-rw-   0        0        0    21971 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/premisgui.py
--rw-rw-rw-   0        0        0     2658 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/qctools.py
--rw-rw-rw-   0        0        0    15738 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/rawbatch.py
--rw-rw-rw-   0        0        0      421 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/renumber.py
--rw-rw-rw-   0        0        0    67554 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/revtmd.py
--rw-rw-rw-   0        0        0     1316 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/legacy_scripts/sha512deep.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:26:30.637512 ifiscripts-2023.5.24.1/scripts/
--rw-rw-rw-   0        0        0   123258 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/Objects.py
--rw-rw-rw-   0        0        0    12189 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/accession.py
--rw-rw-rw-   0        0        0     3710 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/accession_register.py
--rw-rw-rw-   0        0        0     8952 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/as11fixity.py
--rw-rw-rw-   0        0        0    16639 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/batchaccession.py
--rw-rw-rw-   0        0        0     3623 2023-05-24 12:13:49.000000 ifiscripts-2023.5.24.1/scripts/batchmakeshell.py
--rw-rw-rw-   0        0        0     6005 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/batchsipcreator.py
--rw-rw-rw-   0        0        0     9396 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/bitc.py
--rw-rw-rw-   0        0        0    10479 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/concat.py
--rw-rw-rw-   0        0        0    32639 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/copyit.py
--rw-rw-rw-   0        0        0    23142 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/dcpaccess.py
--rw-rw-rw-   0        0        0    13705 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/dcpfixity.py
--rw-rw-rw-   0        0        0     4813 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/deletefiles.py
--rw-rw-rw-   0        0        0    68625 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/dfxml.py
--rw-rw-rw-   0        0        0      804 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/durationcheck.py
--rw-rw-rw-   0        0        0     7327 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/ffv1mkvvalidate.py
--rw-rw-rw-   0        0        0     1903 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/framemd5.py
--rw-rw-rw-   0        0        0    77808 2023-05-24 12:13:49.000000 ifiscripts-2023.5.24.1/scripts/ififuncs.py
--rw-rw-rw-   0        0        0    12437 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/loopline_repackage.py
--rw-rw-rw-   0        0        0     3668 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/make_mediaconch.py
--rw-rw-rw-   0        0        0     1628 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/makedfxml.py
--rw-rw-rw-   0        0        0     3680 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/makedip.py
--rw-rw-rw-   0        0        0    12126 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/makeffv1.py
--rw-rw-rw-   0        0        0    32173 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/makepbcore.py
--rw-rw-rw-   0        0        0      300 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/makeuuid.py
--rw-rw-rw-   0        0        0     3414 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/makezip.py
--rw-rw-rw-   0        0        0     6947 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/manifest.py
--rw-rw-rw-   0        0        0     5708 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/masscopy.py
--rw-rw-rw-   0        0        0      971 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/massqc.py
--rw-rw-rw-   0        0        0      755 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/mergepbcore.py
--rw-rw-rw-   0        0        0     1983 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/multicopy.py
--rw-rw-rw-   0        0        0    10584 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/normalise.py
--rw-rw-rw-   0        0        0     2695 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/order.py
--rw-rw-rw-   0        0        0     6649 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/package_update.py
--rw-rw-rw-   0        0        0     3853 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/packagecheck.py
--rw-rw-rw-   0        0        0     4935 2023-02-09 14:21:08.000000 ifiscripts-2023.5.24.1/scripts/prores.py
--rw-rw-rw-   0        0        0    15431 2023-05-24 12:13:49.000000 ifiscripts-2023.5.24.1/scripts/seq2ffv1.py
--rw-rw-rw-   0        0        0    27444 2023-05-24 12:13:52.000000 ifiscripts-2023.5.24.1/scripts/sipcreator.py
--rw-rw-rw-   0        0        0     8153 2023-05-23 19:17:50.000000 ifiscripts-2023.5.24.1/scripts/strongbox_fixity.py
--rw-rw-rw-   0        0        0     2682 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/subfolders.py
--rw-rw-rw-   0        0        0     3927 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/testfiles.py
--rw-rw-rw-   0        0        0     9842 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/validate.py
--rw-rw-rw-   0        0        0     7154 2023-01-09 12:53:28.000000 ifiscripts-2023.5.24.1/scripts/walk_to_dfxml.py
--rw-rw-rw-   0        0        0       42 2023-05-24 12:26:30.639515 ifiscripts-2023.5.24.1/setup.cfg
--rw-rw-rw-   0        0        0     3040 2023-05-24 12:15:00.000000 ifiscripts-2023.5.24.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:05:40.045359 ifiscripts-2023.6.30.1/
+-rw-rw-rw-   0        0        0   970313 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/26_XYZ-22_Rec709.cube
+-rw-rw-rw-   0        0        0     1116 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       70 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1189 2023-06-30 17:05:40.044356 ifiscripts-2023.6.30.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4589 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/README.rst
+-rw-rw-rw-   0        0        0     5015 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/film_scan_aip_documentation.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 17:05:39.948924 ifiscripts-2023.6.30.1/ifiscripts.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-06-30 17:05:39.000000 ifiscripts-2023.6.30.1/ifiscripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2023-06-30 17:05:39.000000 ifiscripts-2023.6.30.1/ifiscripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:05:39.000000 ifiscripts-2023.6.30.1/ifiscripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-30 17:05:39.000000 ifiscripts-2023.6.30.1/ifiscripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-30 17:05:39.000000 ifiscripts-2023.6.30.1/ifiscripts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 17:05:39.971920 ifiscripts-2023.6.30.1/legacy_scripts/
+-rw-rw-rw-   0        0        0     2872 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/batchfixity.py
+-rw-rw-rw-   0        0        0     1599 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/db_cleaning.py
+-rw-rw-rw-   0        0        0    11222 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/dpxonly.py
+-rw-rw-rw-   0        0        0     5019 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/dvsip.py
+-rw-rw-rw-   0        0        0     1004 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/giffer.py
+-rw-rw-rw-   0        0        0      989 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/loopline.py
+-rw-rw-rw-   0        0        0    11528 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/makedpx.py
+-rw-rw-rw-   0        0        0      851 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/mezzaninecheck.py
+-rw-rw-rw-   0        0        0     1720 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/oeremove.py
+-rw-rw-rw-   0        0        0     3803 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/pg.py
+-rw-rw-rw-   0        0        0     3065 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/playerseq.py
+-rw-rw-rw-   0        0        0    21971 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/premisgui.py
+-rw-rw-rw-   0        0        0     2658 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/qctools.py
+-rw-rw-rw-   0        0        0    15738 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/rawbatch.py
+-rw-rw-rw-   0        0        0      421 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/renumber.py
+-rw-rw-rw-   0        0        0    67528 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/legacy_scripts/revtmd.py
+-rw-rw-rw-   0        0        0     1316 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/legacy_scripts/sha512deep.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:05:40.043353 ifiscripts-2023.6.30.1/scripts/
+-rw-rw-rw-   0        0        0   123258 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/Objects.py
+-rw-rw-rw-   0        0        0     3729 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/accession_register.py
+-rw-rw-rw-   0        0        0    12517 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/aipcreator.py
+-rw-rw-rw-   0        0        0     9815 2023-06-30 16:49:28.000000 ifiscripts-2023.6.30.1/scripts/as11fixity.py
+-rw-rw-rw-   0        0        0    16950 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/batchaipcreator.py
+-rw-rw-rw-   0        0        0     6149 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/batchdiff_framemd5.py
+-rw-rw-rw-   0        0        0     3618 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/batchmakeshell.py
+-rw-rw-rw-   0        0        0     6005 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/batchsipcreator.py
+-rw-rw-rw-   0        0        0     9396 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/bitc.py
+-rw-rw-rw-   0        0        0    10479 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/concat.py
+-rw-rw-rw-   0        0        0    32639 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/copyit.py
+-rw-rw-rw-   0        0        0    23142 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/dcpaccess.py
+-rw-rw-rw-   0        0        0    13705 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/dcpfixity.py
+-rw-rw-rw-   0        0        0     4814 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/deletefiles.py
+-rw-rw-rw-   0        0        0    68625 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/dfxml.py
+-rw-rw-rw-   0        0        0      804 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/durationcheck.py
+-rw-rw-rw-   0        0        0     7327 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/ffv1mkvvalidate.py
+-rw-rw-rw-   0        0        0     1946 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/framemd5.py
+-rw-rw-rw-   0        0        0    77085 2023-06-30 16:55:48.000000 ifiscripts-2023.6.30.1/scripts/ififuncs.py
+-rw-rw-rw-   0        0        0    12425 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/loopline_repackage.py
+-rw-rw-rw-   0        0        0     3668 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/make_mediaconch.py
+-rw-rw-rw-   0        0        0     1628 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/makedfxml.py
+-rw-rw-rw-   0        0        0     3680 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/makedip.py
+-rw-rw-rw-   0        0        0    12126 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/makeffv1.py
+-rw-rw-rw-   0        0        0    32016 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/makepbcore.py
+-rw-rw-rw-   0        0        0      300 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/makeuuid.py
+-rw-rw-rw-   0        0        0     3414 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/makezip.py
+-rw-rw-rw-   0        0        0     6947 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/manifest.py
+-rw-rw-rw-   0        0        0     5708 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/masscopy.py
+-rw-rw-rw-   0        0        0      971 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/massqc.py
+-rw-rw-rw-   0        0        0      757 2023-06-01 15:32:45.000000 ifiscripts-2023.6.30.1/scripts/mergepbcore.py
+-rw-rw-rw-   0        0        0     1983 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/multicopy.py
+-rw-rw-rw-   0        0        0    10584 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/normalise.py
+-rw-rw-rw-   0        0        0     2689 2023-06-30 16:49:24.000000 ifiscripts-2023.6.30.1/scripts/order.py
+-rw-rw-rw-   0        0        0     6649 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/package_update.py
+-rw-rw-rw-   0        0        0     3853 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/packagecheck.py
+-rw-rw-rw-   0        0        0     4935 2023-02-09 14:21:08.000000 ifiscripts-2023.6.30.1/scripts/prores.py
+-rw-rw-rw-   0        0        0    15431 2023-05-24 12:13:49.000000 ifiscripts-2023.6.30.1/scripts/seq2ffv1.py
+-rw-rw-rw-   0        0        0    28617 2023-06-30 16:49:28.000000 ifiscripts-2023.6.30.1/scripts/sipcreator.py
+-rw-rw-rw-   0        0        0     8153 2023-05-23 19:17:50.000000 ifiscripts-2023.6.30.1/scripts/strongbox_fixity.py
+-rw-rw-rw-   0        0        0     2682 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/subfolders.py
+-rw-rw-rw-   0        0        0     3927 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/testfiles.py
+-rw-rw-rw-   0        0        0     9842 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/validate.py
+-rw-rw-rw-   0        0        0     7154 2023-01-09 12:53:28.000000 ifiscripts-2023.6.30.1/scripts/walk_to_dfxml.py
+-rw-rw-rw-   0        0        0       42 2023-06-30 17:05:40.045359 ifiscripts-2023.6.30.1/setup.cfg
+-rw-rw-rw-   0        0        0     3152 2023-06-30 16:55:20.000000 ifiscripts-2023.6.30.1/setup.py
```

### Comparing `ifiscripts-2023.5.24.1/26_XYZ-22_Rec709.cube` & `ifiscripts-2023.6.30.1/26_XYZ-22_Rec709.cube`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/LICENSE.txt` & `ifiscripts-2023.6.30.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/PKG-INFO` & `ifiscripts-2023.6.30.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: ifiscripts
-Version: 2023.5.24.1
+Version: 2023.6.30.1
 Summary: Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive
 Author: Kieran O'Leary
 Author-email: kieran.o.leary@gmail.com
+Maintainer: Yazhou He
+Maintainer-email: yhe@irishfilm.ie
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Scripts for use in the IFI Irish Film Archive. Scripts have been tested in OSX/Windows 7/10 and Ubuntu 18.04. The aim is to make cross-platform scripts, but please get in touch with any issues. It is best to download all scripts, as some of them share code.
 
 Most scripts take either a file or a directory as their input, for example makeffv1.py filename.mov or premis.py path/to/folder_of_stuff. (It's best to just drag and drop the folder or filename into the terminal)
```

### Comparing `ifiscripts-2023.5.24.1/README.rst` & `ifiscripts-2023.6.30.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -50,21 +50,21 @@
 
 * All of these preservation events are logged in a log file located in the ``logs`` directory. This log file tries to use ``PREMIS (PREservation Metadata Implementation Strategies)`` terminology as much as possible.
 
 * Even though the package has yet to be accessioned, temporary backups are required. ``copyit.py`` will generate backups, and it will use the checksum manifest generated by ``sipcreator.py`` to verify the integrity of the file transfer.
 
 * If the package contains FFV1 or Matroska files, perhaps ``ffv1mkvvalidate.py`` could run, which uses ``mediaconch`` to verify the compliance of the files, and stores the information in the logfile.
 
-* If the package passes our Quality Control Procedures, then it will be accessioned. ``accession.py`` will generate an accession number, rename the OE number with the accession number, generate a SHA-512 manifest and update the log file to document these new preservation events.
+* If the package passes our Quality Control Procedures, then it will be accessioned. ``aipcreator.py`` will generate an accession number, rename the OE number with the accession number, generate a SHA-512 manifest and update the log file to document these new preservation events.
 
-* A large batch of items can be accessioned using ``batchaccession.py``. If the ``-pbcore`` command line argument is used with the accessioning scripts, technical metadata based on the PBCore standard will be generated in CSV format. This process can be run seperately by using ``makepbcore.py``. CSV was chosen instead of XML as this allows us to immediately import the CSV into our database system so that we have item level records.
+* A large batch of items can be AIPed using ``batchaipcreator.py``. If the ``-pbcore`` command line argument is used with the aipcreator scripts, technical metadata based on the PBCore standard will be generated in CSV format. This process can be run seperately by using ``makepbcore.py``. CSV was chosen instead of XML as this allows us to immediately import the CSV into our database system so that we have item level records.
 
 * Access copies may be needed, so low-res watermarked proxies can be generated with ``bitc.py``, or high res mezzanines with ``prores.py``.
 
-* The accessioned package can then be written to preservation storage, again using the ``copyit.py`` command.
+* The AIP can then be written to preservation storage, again using the ``copyit.py`` command.
 
 So this is just one way of using the scripts from acquisition to preservation storage, but there are many other scripts for specific workflows, which you can investigate further down in the documentation.
 
 
 
 Table of Contents
 -----------------
```

### Comparing `ifiscripts-2023.5.24.1/film_scan_aip_documentation.txt` & `ifiscripts-2023.6.30.1/film_scan_aip_documentation.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 This textfile - Generic description of the features of the Archival Information Package.
 Changelog: v1.1 - temporary manifests removed from logs_directory.
 
 parent_directory - either OE (oe##### - Object_Entry Spectrum Collections Management( Identifier or Accession Number (aaa####)
 ├── uuid_directory - this directory contains the AIP. The identifier is  for the entire representation/package.
 │   ├── logs - logs that are generated via IFIscripts. This can include process logs for FFmpeg/rawcooked and other tools.
 │   │   └── uuid_sip_log.log - the most important log - this is a rolling log for all processes that IFIscripts will execute.
-│   ├── metadata - for AV objects - mediainfo and mediatrace XML files. For non-AV objects, Siegfried/PRONOM and EXIFTOOL JSON reports. Once the package is accessioned, there will be a Digital Forensics XML minus the hashes. This will also contain PBCore/Technical metadata CSV and IFI Filmographic CSV in the accessioned package.
+│   ├── metadata - for AV objects - mediainfo and mediatrace XML files. For non-AV objects, Siegfried/PRONOM and EXIFTOOL JSON reports. Once the AIP is created it will contain a Digital Forensics XML minus the hashes. It will also contain PBCore/Technical metadata CSV and IFI Filmographic CSV.
 │   │   └── supplemental - For normalised objects, checksum manifests, mediainfo, mediatrace and Digital Forensics XML regarding the source object.
 │   └── objects - the actual focus of preservation. 
 └── uuid_directory_manifest.md5 - MD5 manifest for entire package.
-└── uuid_directory_manifest-sha512.txt - This will only be generated at the accessioning phase. SHA512 manifest for the entire package.
+└── uuid_directory_manifest-sha512.txt - This will only be generated with AIPCREATOR.py/BATCHAIPCREATOR.py. SHA512 manifest for the entire package.
 
 Example tree structure and explanation for a film scan normalised to FFV1/Matroska via seq2ffv1.py. 
-Additional files appear when the accession/batchaccession process runs.
+Additional files appear when the aipcreator/batchaipcreator process runs.
 
 oe0001 | parent_directory
 ├── da990f5e-9846-4a8c-9792-3ee677d50591 |uuid_directory
 │   ├── logs | directory for logs generated via IFIscripts
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel3.mkv_rawcooked.log | rawcooked_log via ffmpeg
 │   │   └── da990f5e-9846-4a8c-9792-3ee677d50591_sip_log.log | central log for all IFIscripts processes
 │   ├── metadata | directory for metadata
-│   │   ├── aaa0001_pbcore.csv | ONLY APPEARS WITH ACCESSION.py/BATCHACCESSION.py - CSV containing metadata ready for ingest into IFI technical database. Loosely based on PBCore, with many custom IFI legacy fields.
-│   │   ├── AF12345_filmographic.csv | ONLY APPEARS WITH ACCESSION.py/BATCHACCESSION.py - CSV containing descriptive metadata ready for ingest into IFI Filmographic/descriptive database. Loosely based on the original FIAF cataloguing guidelines.
-│   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_dfxml.xml | ONLY APPEARS WITH ACCESSION.py/BATCHACCESSION.py - file system metadata in Digital Forensics XML format for all files within the package.
+│   │   ├── aaa0001_pbcore.csv | ONLY APPEARS WITH AIPCREATOR.py/BATCHAIPCREATOR.py - CSV containing metadata ready for ingest into IFI technical database. Loosely based on PBCore, with many custom IFI legacy fields.
+│   │   ├── AF12345_filmographic.csv | ONLY APPEARS WITH AIPCREATOR.py/BATCHAIPCREATOR.py - CSV containing descriptive metadata ready for ingest into IFI Filmographic/descriptive database. Loosely based on the original FIAF cataloguing guidelines.
+│   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_dfxml.xml | ONLY APPEARS WITH AIPCREATOR.py/BATCHAIPCREATOR.py - file system metadata in Digital Forensics XML format for all files within the package.
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel1.mkv_mediainfo.xml | technical metadata in XML format via mediainfo
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel1.mkv_mediatrace.xml | granular technical metadata in XML format via mediainfo
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel2.mkv_mediainfo.xml | technical metadata in XML format via mediainfo
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel2.mkv_mediatrace.xml granular technical metadata in XML format via mediainfo
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel3.mkv_mediainfo.xml | technical metadata in XML format via mediainfo
 │   │   ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel3.mkv_mediatrace.xml | granular technical metadata in XML format via mediainfo
 │   │   └── supplemental | directory for metadata for the source object, prior to normalisation
@@ -36,10 +36,10 @@
 │   │       ├── da990f5e-9846-4a8c-9792-3ee677d50591_source_mediatrace.xml | granulartechnical metadata in XML format for the source DPX sequence.
 │   │       └── multi_reel_manifest-md5.txt | md5 checksum manifest for the source DPX sequence
 │   └── objects | directory for the preservation
 │       ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel1.mkv | FFV1/Matroska normalisation of image sequence.
 │       ├── da990f5e-9846-4a8c-9792-3ee677d50591_reel2.mkv | FFV1/Matroska normalisation of image sequence.
 │       └── da990f5e-9846-4a8c-9792-3ee677d50591_reel3.mkv | FFV1/Matroska normalisation of image sequence.
 ├── da990f5e-9846-4a8c-9792-3ee677d50591_manifest.md5 | MD5 checksum manifest for the whole package.
-└── da990f5e-9846-4a8c-9792-3ee677d50591_manifest-sha512.txt |  ONLY APPEARS WITH ACCESSION.py/BATCHACCESSION.py SHA512 checksum manifest for the whole package.
+└── da990f5e-9846-4a8c-9792-3ee677d50591_manifest-sha512.txt |  ONLY APPEARS WITH AIPCREATOR.py/BATCHAIPCREATOR.py SHA512 checksum manifest for the whole package.
```

### Comparing `ifiscripts-2023.5.24.1/ifiscripts.egg-info/PKG-INFO` & `ifiscripts-2023.6.30.1/ifiscripts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: ifiscripts
-Version: 2023.5.24.1
+Version: 2023.6.30.1
 Summary: Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive
 Author: Kieran O'Leary
 Author-email: kieran.o.leary@gmail.com
+Maintainer: Yazhou He
+Maintainer-email: yhe@irishfilm.ie
 License: MIT
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 
 Scripts for use in the IFI Irish Film Archive. Scripts have been tested in OSX/Windows 7/10 and Ubuntu 18.04. The aim is to make cross-platform scripts, but please get in touch with any issues. It is best to download all scripts, as some of them share code.
 
 Most scripts take either a file or a directory as their input, for example makeffv1.py filename.mov or premis.py path/to/folder_of_stuff. (It's best to just drag and drop the folder or filename into the terminal)
```

### Comparing `ifiscripts-2023.5.24.1/ifiscripts.egg-info/SOURCES.txt` & `ifiscripts-2023.6.30.1/ifiscripts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 legacy_scripts/premisgui.py
 legacy_scripts/qctools.py
 legacy_scripts/rawbatch.py
 legacy_scripts/renumber.py
 legacy_scripts/revtmd.py
 legacy_scripts/sha512deep.py
 scripts/Objects.py
-scripts/accession.py
 scripts/accession_register.py
+scripts/aipcreator.py
 scripts/as11fixity.py
-scripts/batchaccession.py
+scripts/batchaipcreator.py
+scripts/batchdiff_framemd5.py
 scripts/batchmakeshell.py
 scripts/batchsipcreator.py
 scripts/bitc.py
 scripts/concat.py
 scripts/copyit.py
 scripts/dcpaccess.py
 scripts/dcpfixity.py
```

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/batchfixity.py` & `ifiscripts-2023.6.30.1/legacy_scripts/batchfixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/db_cleaning.py` & `ifiscripts-2023.6.30.1/legacy_scripts/db_cleaning.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/dpxonly.py` & `ifiscripts-2023.6.30.1/legacy_scripts/dpxonly.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/dvsip.py` & `ifiscripts-2023.6.30.1/legacy_scripts/dvsip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/giffer.py` & `ifiscripts-2023.6.30.1/legacy_scripts/giffer.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/loopline.py` & `ifiscripts-2023.6.30.1/legacy_scripts/loopline.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/makedpx.py` & `ifiscripts-2023.6.30.1/legacy_scripts/makedpx.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/mezzaninecheck.py` & `ifiscripts-2023.6.30.1/legacy_scripts/mezzaninecheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/oeremove.py` & `ifiscripts-2023.6.30.1/legacy_scripts/oeremove.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/pg.py` & `ifiscripts-2023.6.30.1/legacy_scripts/pg.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/playerseq.py` & `ifiscripts-2023.6.30.1/legacy_scripts/playerseq.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/premisgui.py` & `ifiscripts-2023.6.30.1/legacy_scripts/premisgui.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/qctools.py` & `ifiscripts-2023.6.30.1/legacy_scripts/qctools.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/rawbatch.py` & `ifiscripts-2023.6.30.1/legacy_scripts/rawbatch.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/revtmd.py` & `ifiscripts-2023.6.30.1/legacy_scripts/revtmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,15 +661,15 @@
                "Dean Kavanagh", "Raelene Casey", 
            "Anja Mahler", "Eoin O'Donohoe", "Brian Cash","Unknown"]
     user = choicebox(msg, title, choices)
 
     msg = "Fill out these things please"
     title = "blablablabl"
     fieldNames = ["Source Accession Number",
-                  "Filmographic Reference Number", 
+                  "Filmographic URN", 
                   "Identifier-Object Entry/Accession Number:"]
       # we start with blanks for the values
     fieldValues = multenterbox(msg,title, fieldNames)
 
     # make sure that none of the fields was left blank
     while 1:
             if fieldValues == None: break
@@ -772,15 +772,15 @@
         fo.write('<revtmd:role/>\n')
         fo.write('</revtmd:organization_main>\n')
         fo.write('<revtmd:organization_division>\n')
         fo.write('<revtmd:name>Irish Film Archive</revtmd:name>\n')
         fo.write('</revtmd:organization_division>\n')
         fo.write('</revtmd:organization>\n')
         fo.write('<revtmd:identifier type="Object Entry">%s</revtmd:identifier>\n' % fieldValues[2])
-        fo.write('<revtmd:identifier type="Inmagic DB Textworks Filmographic Reference Number">%s</revtmd:identifier>\n' % fieldValues[1])
+        fo.write('<revtmd:identifier type="Inmagic DB Textworks Filmographic URN">%s</revtmd:identifier>\n' % fieldValues[1])
         
         fo.write('<revtmd:duration>%s</revtmd:duration>\n' % container_duration)
         fo.write('<revtmd:language/>\n')
         fo.write('<revtmd:size>%s</revtmd:size>\n' % container_size)
         fo.write('<revtmd:datarate>%s</revtmd:datarate>\n' % overall_bitrate)
         fo.write('<revtmd:use>Preservation Master</revtmd:use>\n')
         fo.write('<revtmd:color/>\n')
```

### Comparing `ifiscripts-2023.5.24.1/legacy_scripts/sha512deep.py` & `ifiscripts-2023.6.30.1/legacy_scripts/sha512deep.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/Objects.py` & `ifiscripts-2023.6.30.1/scripts/Objects.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/accession.py` & `ifiscripts-2023.6.30.1/scripts/aipcreator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #! /usr/bin/env python3
 '''
-Runs (Spectrum) accessioning procedures on packages
-that have been through the Object Entry process
+Creates AIPs for the Irish Film Institute collections
 Written by Kieran O'Leary
 MIT License
 '''
 
 import sys
 import os
 import argparse
@@ -43,43 +42,43 @@
 
 
 def parse_args(args_):
     '''
     Parse command line arguments.
     '''
     parser = argparse.ArgumentParser(
-        description='Accessions objects into the Irish Film Institute collection'
+        description='Creates AIPs for the Irish Film Institute collections'
         'Completes the transformation of a SIP into an AIP.'
         ' Written by Kieran O\'Leary.'
     )
     parser.add_argument(
         'input', help='Input directory'
     )
     parser.add_argument(
         '-user',
         help='Declare who you are. If this is not set, you will be prompted.')
     parser.add_argument(
-        '-number',
+        '-accession_number',
         help='Enter the Accession number for the representation.The parent Object Entry number will be replaced with this name.'
     )
     parser.add_argument(
         '-force',
-        help='Renames OE with accession number without confirmation.', action='store_true'
+        help='Renames OE with Accession number without confirmation.', action='store_true'
     )
     parser.add_argument(
         '-pbcore',
         help='launches makepbcore and updates AIP', action='store_true'
     )
     parser.add_argument(
-        '-reference',
-        help='Enter the Filmographic reference number for the representation. This is only relevant when used with -pbcore. For multiple works that are represented, seperate each reference number with a + sign eg AF1234+AC456'
+        '-filmo_number',
+        help='Enter the Filmographic URN for the representation. This is only relevant when used with -pbcore. For multiple works that are represented, seperate each Filmographic URN with a + sign eg AF1234+AC456'
     )
     parser.add_argument(
         '-register',
-        help='Path of accessions register CSV file. Mostly to be used by batchaccession.py'
+        help='Path of accessions register CSV file. Mostly to be used by batchaipcreator.py'
     )
     parser.add_argument(
         '-filmo_csv',
         help='Enter the path to the Filmographic CSV so that the metadata will be stored within the package.'
     )
     parser.add_argument(
         '-parent',
@@ -114,66 +113,66 @@
     Adds Digital Forensics XML to metadata folder and updates manifests.
     '''
     metadata = os.path.join(new_uuid_path, 'metadata')
     dfxml = os.path.join(metadata, uuid + '_dfxml.xml')
     makedfxml.main([new_uuid_path, '-n', '-o', dfxml])
     return dfxml
 
-def insert_filmographic(filmographic_csv, Reference_Number, package_filmographic):
+def insert_filmographic(filmographic_csv, filmographic_number, package_filmographic):
     '''
-    Should this be done at the accession.py level?
+    Should this be done at the aipcreator.py level?
     yes, as it extracts the title.
     And it should be done after the args.pbcore bit as
-    that is what extracts the reference number.
-    filmographic_csv=source filmographic csv with reference numbers
-    Reference_Number=the specific reference number that you would like to extract
+    that is what extracts the filmographic URN.
+    filmographic_csv=source filmographic csv with filmo numbers
+    Filmo_Number=the specific filmographic URN that you would like to extract
     package_filmographic = the full path of the filmographic to be instered in /metadata
     '''
     csv_dict = ififuncs.extract_metadata(filmographic_csv)
     for items in csv_dict:
         for x in items:
             if type(x) in [collections.OrderedDict, dict]:
-                if Reference_Number in x['Filmographic URN'].upper():
+                if filmographic_number in x['Filmographic URN'].upper():
                     with open(package_filmographic, 'w', encoding='utf-8') as csvfile:
                         fieldnames = csv_dict[1]
                         writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
                         writer.writeheader()
                         writer.writerow(x)
 def main(args_):
     '''
-    Launches the various functions that will accession a package
+    Launches the various functions that will turn the SIP into an AIP.
     '''
     args = parse_args(args_)
     source = args.input
     uuid_directory = ififuncs.check_for_sip([source])
     if uuid_directory is not None:
         oe_path = os.path.dirname(uuid_directory)
         oe_number = os.path.basename(oe_path)
         if args.user:
             user = args.user
         else:
             user = ififuncs.get_user()
-        if args.number:
-            if args.number[:3] != 'aaa':
+        if args.accession_number:
+            if args.accession_number[:3] != 'aaa':
                 print('First three characters must be \'aaa\' and last four characters must be four digits')
                 accession_number = ififuncs.get_accession_number()
-            elif len(args.number[3:]) != 4:
+            elif len(args.accession_number[3:]) != 4:
                 accession_number = ififuncs.get_accession_number()
                 print('First three characters must be \'aaa\' and last four characters must be four digits')
-            elif not args.number[3:].isdigit():
+            elif not args.accession_number[3:].isdigit():
                 accession_number = ififuncs.get_accession_number()
                 print('First three characters must be \'aaa\' and last four characters must be four digits')
             else:
-                accession_number = args.number
+                accession_number = args.accession_number
         else:
             accession_number = ififuncs.get_accession_number()
-        if args.reference:
-            Reference_Number = args.reference.upper()
+        if args.filmo_number:
+            filmo_number = args.filmo_number.upper()
         else:
-            Reference_Number = ififuncs.get_reference_number()
+            filmo_number = ififuncs.get_filmo_number()
         if args.acquisition_type:        
             acquisition_type = ififuncs.get_acquisition_type(args.acquisition_type)
             print(acquisition_type)
         accession_path = os.path.join(
             os.path.dirname(oe_path), accession_number
         )
         uuid = os.path.basename(uuid_directory)
@@ -191,19 +190,19 @@
         if args.register:
             register = args.register
         else:
             register = make_register()
         ififuncs.append_csv(register, (oe_number.upper()[:2] + '-' + oe_number[2:], accession_number, '','','','','', ''))
         ififuncs.generate_log(
             sipcreator_log,
-            'EVENT = accession.py started'
+            'EVENT = aipcreator.py started'
         )
         ififuncs.generate_log(
             sipcreator_log,
-            'eventDetail=accession.py %s' % ififuncs.get_script_version('accession.py')
+            'eventDetail=aipcreator.py %s' % ififuncs.get_script_version('aipcreator.py')
         )
         ififuncs.generate_log(
             sipcreator_log,
             'Command line arguments: %s' % args
         )
         ififuncs.generate_log(
             sipcreator_log,
@@ -213,18 +212,28 @@
             sipcreator_log,
             'EVENT = eventType=Identifier assignment,'
             ' eventIdentifierType=accession number, value=%s'
             % accession_number
         )
         ififuncs.generate_log(
             sipcreator_log,
-            'EVENT = eventType=accession,'
+            'EVENT = eventType=Accession,'
             ' eventIdentifierType=accession number, value=%s'
             % accession_number
         )
+        ififuncs.generate_log(
+            sipcreator_log,
+            'EVENT = eventType=Information package creation'
+        )
+        '''
+        ififuncs.generate_log(
+            sipcreator_log,
+            'EVENT = eventType=Information package creation, eventOutcomeDetailNote=Archival information package'
+        )
+        '''
         sip_manifest = os.path.join(
             accession_path, uuid
             ) + '_manifest.md5'
         sha512_log = manifest.main([new_uuid_path, '-sha512', '-s'])
         sha512_manifest = os.path.join(
             os.path.dirname(new_uuid_path), uuid + '_manifest-sha512.txt'
         )
@@ -240,45 +249,45 @@
             )
         except UnicodeDecodeError:
             ififuncs.generate_log(
                 sipcreator_log,
                 'EVENT = Metadata extraction - eventDetail=File system metadata extraction using Digital Forensics XML, eventOutcome=FAILURE due to UnicodeDecodeError, agentName=makedfxml'
             )
             dfxml_check = False
-        # this is inefficient. The script should not have to ask for reference
+        # this is inefficient. The script should not have to ask for filmographic
         # number twice if someone wants to insert the filmographic but do not
         # want to make the pbcore csv, perhaps because the latter already exists.
         if args.filmo_csv:
             metadata_dir = os.path.join(new_uuid_path, 'metadata')
-            if '+' in Reference_Number:
-                reference_list = Reference_Number.split('+')
+            if '+' in filmo_number:
+                filmo_list = filmo_number.split('+')
             else:
-                reference_list = [Reference_Number]
-            for ref in reference_list:
-                package_filmographic = os.path.join(metadata_dir, ref + '_filmographic.csv')
-                insert_filmographic(args.filmo_csv, ref , package_filmographic)
+                filmo_list = [filmo_number]
+            for filmo in filmo_list:
+                package_filmographic = os.path.join(metadata_dir, filmo + '_filmographic.csv')
+                insert_filmographic(args.filmo_csv, filmo , package_filmographic)
                 ififuncs.generate_log(
                     sipcreator_log,
-                    'EVENT = Metadata extraction - eventDetail=Filmographic descriptive metadata added to metadata folder, eventOutcome=%s, agentName=accession.py' % (package_filmographic)
+                    'EVENT = Metadata extraction - eventDetail=Filmographic descriptive metadata added to metadata folder, eventOutcome=%s, agentName=aipcreator.py' % (package_filmographic)
                 )
                 ififuncs.manifest_update(sip_manifest, package_filmographic)
                 ififuncs.sha512_update(sha512_manifest, package_filmographic)
                 print('Filmographic descriptive metadata added to metadata folder')
         ififuncs.generate_log(
             sipcreator_log,
-            'EVENT = accession.py finished'
+            'EVENT = aipcreator.py finished'
         )
         ififuncs.checksum_replace(sip_manifest, sipcreator_log, 'md5')
         ififuncs.checksum_replace(sha512_manifest, sipcreator_log, 'sha512')
         if dfxml_check is True:
             ififuncs.manifest_update(sip_manifest, dfxml)
             ififuncs.sha512_update(sha512_manifest, dfxml)
         if args.pbcore:
-            for ref in reference_list:
-                makepbcore_cmd = [accession_path, '-p', '-user', user, '-reference', ref]
+            for filmo in filmo_list:
+                makepbcore_cmd = [accession_path, '-p', '-user', user, '-filmo_number', filmo]
                 if args.parent:
                     makepbcore_cmd.extend(['-parent', args.parent])
                 if args.acquisition_type:
                     makepbcore_cmd.extend(['-acquisition_type', args.acquisition_type])
                 if args.donor:
                     makepbcore_cmd.extend(['-donor', args.donor])
                 if args.donor:
```

### Comparing `ifiscripts-2023.5.24.1/scripts/accession_register.py` & `ifiscripts-2023.6.30.1/scripts/accession_register.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     )
     parser.add_argument(
         '-pbcore_csv',
         help='Path to technical/PBCore CSV.'
     )
     parser.add_argument(
         '-filmo_csv',
-        help='Path to Filmographic CSV. Must contain reference numbers.'
+        help='Path to Filmographic CSV. Must contain Filmographic URN.'
     )
     parsed_args = parser.parse_args(args_)
     return parsed_args
 
 
 def find_checksums(csv_file, identifier):
     '''
@@ -54,17 +54,17 @@
     Launches functions that will generate a helper accessions register
     '''
     args = parse_args(args_)
     sorted_csv_dict = ififuncs.extract_metadata(args.sorted_csv)[0]
     pbcore_csv_dict = ififuncs.extract_metadata(args.pbcore_csv)[0]
     filmo_csv_dict = ififuncs.extract_metadata(args.filmo_csv)[0]
     for accession in sorted_csv_dict:
-        number = accession['accession number']
+        accession_number = accession['accession number']
         for technical_record in pbcore_csv_dict:
-            if technical_record['Accession Number'] == number:
+            if technical_record['Accession Number'] == accession_number:
                 accession['acquisition method'] = technical_record['Type Of Deposit']
                 accession['acquired from'] = technical_record['Donor']
                 accession['date acquired'] = technical_record['Date Of Donation']
                 for filmographic_record in filmo_csv_dict:
                     if filmographic_record['Filmographic URN'] == technical_record['Reference Number']:
                         if filmographic_record['Title/Name'] == '':
                             title = filmographic_record['Series Title'] + '; ' + filmographic_record['Episode No']
```

### Comparing `ifiscripts-2023.5.24.1/scripts/as11fixity.py` & `ifiscripts-2023.6.30.1/scripts/as11fixity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 #!/usr/bin/env python3
 '''
-WORK IN PROGRESS WORKSHOP SCRIPT!!!
+VALIDATE AS-11 UK DPP MXF BY COMPARING 
+ITS CHECKSUMS FROM BOTH PACKAGE MANIFEST
+AND DPP XML <MediaChecksumValue>
 '''
 
 import sys
 import os
 import csv
 import hashlib
 from datetime import datetime
 from lxml import etree
 import unidecode
-
-
-def create_csv(csv_file, *args):
-    f = open(csv_file, 'w', encoding='utf8', newline='')
-    try:
-        writer = csv.writer(f)
-        writer.writerow(*args)
-    finally:
-        f.close()
-
-
-def append_csv(csv_file, *args):
-    f = open(csv_file, 'a', encoding='utf-8', newline='')
-    try:
-        writer = csv.writer(f)
-        writer.writerow(*args)
-    finally:
-        f.close()
-
+import ififuncs
 
 def digest_with_progress(filename, chunk_size):
     read_size = 0
     last_percent_done = 0
     digest = hashlib.md5()
     total_size = os.path.getsize(filename)
     data = True
-    f = open(filename, 'rb')
+    f = open(filename, 'rb', encoding= 'utf-8')
     while data:
         # Read and update digest.
         data = f.read(chunk_size)
         read_size += len(data)
         digest.update(data)
         # Calculate progress.
         percent_done = 100 * read_size / total_size
@@ -55,16 +39,16 @@
     dicto = {}
     previous_oe = ''
     for dirpath, dirss, filenames in os.walk(starting_dir):
         oe = False
         aaa = False
         try:
             current_oe = dirpath.split('oe')[1][:5]
-            if current_oe[-1] == '/':
-                current_oe = current_oe[:4]
+            if current_oe[-1] == '/' or current_oe[-1] == '\\':
+                current_oe = current_oe[:-1]
             oe = True
         except IndexError:
             try:
                 current_oe = dirpath.split('aaa')[1][:4]
                 aaa = True
             except IndexError:
                 continue
@@ -81,152 +65,161 @@
         elif aaa:
             dicto['aaa' + previous_oe] = [filename_counter, dir_counter]
         ''''
         except KeyError:
             print 'hi'
             dicto['aaa' + previous_oe] = [filename_counter, dir_counter]
         '''
-    print(dicto)
+    print('SIP/AIP found:')
+    for i in dicto:
+        print(i, " | filecount: ", dicto[i][0], " | folder_count: ", dicto[i][1])
+    print()
     return dicto
+
 def main():
     starting_dir = sys.argv[1]
     dicto = count_files(starting_dir)
-    print(dicto, 12312312123)
     startTime = datetime.now()
     csv_report_filename = os.path.basename(starting_dir) + "_report"
     csv_report = os.path.expanduser("~/Desktop/%s.csv") % csv_report_filename
     checkfile = os.path.isfile(csv_report)
-    counter = 0
-    create_csv(
+    if checkfile is True:
+        print("CSV file already exists.\nThis will overwrite the existed CSV.\n")
+    ififuncs.create_csv(
         csv_report,
         (
             'ID',
             'oe',
             'accessionnumber',
             'files_count',
             'directory_count',
             'Filename',
             'Series_Title',
             'Prog_Title',
             'Episode_Number',
             'Md5_From_Xml',
             'Md5_from_Mxf',
             'Checksum_Result'
-            )
         )
-    if checkfile is True:
-        print("CSV file already exists.")
+    )
+    
+    xml_flag = 0
     for dirpath, dirss, filenames in sorted(os.walk(starting_dir)):
-        for filename in filenames:
-            if filename.endswith('.xml'):
-                if os.path.basename(dirpath) == 'supplemental':
+        if len(os.path.basename(dirpath)) == 36:
+            uuid_dir = dirpath
+            logs_dir = os.path.join(uuid_dir, 'logs')
+            log = os.path.join(logs_dir, os.path.basename(uuid_dir) + '_sip_log.log')
+            objects_dir = os.path.join(uuid_dir, 'objects')
+            objects_list = os.listdir(objects_dir)
+            manifest_basename = os.path.basename(uuid_dir) + '_manifest.md5'
+            manifest = os.path.join(os.path.dirname(uuid_dir), manifest_basename)
+        if os.path.basename(dirpath) == 'supplemental':
+            for filename in filenames:
+                if filename.endswith('.xml') and not filename.endswith('_MediaConchReport.xml'):
                     full_xml_path = os.path.join(dirpath, filename)
-                else:
-                    continue
-                uuid_dir = os.path.dirname(os.path.dirname(dirpath))
-                objects_dir = os.path.join(uuid_dir, 'objects')
-                logs_dir = os.path.join(uuid_dir, 'logs')
-                log = os.path.join(logs_dir, os.path.basename(uuid_dir) + '_sip_log.log')
-                
-                objects_list = os.listdir(objects_dir)
-
-                manifest_basename = os.path.basename(uuid_dir) + '_manifest.md5'
-                manifest = os.path.join(os.path.dirname(uuid_dir), manifest_basename)
-                with open(manifest, 'r', encoding='utf-8') as fo:
-                    manifest_lines = fo.readlines()
-                    for line in manifest_lines:
-                        if line.lower().replace('\n', '').endswith('.mxf'):
-                        
-                            mxf_checksum = line[:32]
-                            print(mxf_checksum)
-                #mxf_checksum = str(digest_with_progress(mxf, 1024))
-                try:
-                    dpp_xml_parse = etree.parse(full_xml_path)
-                    dpp_xml_namespace = dpp_xml_parse.xpath('namespace-uri(.)')
-                    #parsed values
-                    series_title = dpp_xml_parse.findtext(
-                        '//ns:SeriesTitle',
-                        namespaces={'ns':dpp_xml_namespace}
-                    )
-                    prog_title = dpp_xml_parse.findtext(
-                        '//ns:ProgrammeTitle',
-                        namespaces={'ns':dpp_xml_namespace}
-                    )
-                    ep_num = dpp_xml_parse.findtext(
-                        '//ns:EpisodeTitleNumber',
-                        namespaces={'ns':dpp_xml_namespace}
-                    )
-                    checksum = dpp_xml_parse.findtext(
-                        '//ns:MediaChecksumValue',
-                        namespaces={'ns':dpp_xml_namespace}
-                    )
-                    accession_number_id = ''
-                    print('Generating Report....  \n')
-                    if os.path.isfile(log):
-                        print(log)
-                        with open(log, 'r', encoding='utf-8') as log_object:
-                            log_lines = log_object.readlines()
-                            for lines in log_lines:
-                                if 'eventIdentifierType=object entry,' in lines:
-                                    source_oe = lines.split('=')[-1].replace('\n', '')
-                                if 'eventIdentifierType=accession number,' in lines:
-                                    accession_number_id = lines.split('=')[-1].replace('\n', '')
-                    if mxf_checksum == checksum:
-                        print(dicto,7897897897)
-                        append_csv(
-                            csv_report,
-                            (
-                                os.path.basename(os.path.dirname(uuid_dir)),
-                                source_oe,
-                                accession_number_id,
-                                dicto[os.path.basename(os.path.dirname(uuid_dir))][0],
-                                dicto[os.path.basename(os.path.dirname(uuid_dir))][1],
-                                filename,
-                                unidecode.unidecode(series_title),
-                                unidecode.unidecode(prog_title),
-                                unidecode.unidecode(ep_num),
-                                checksum,
-                                mxf_checksum,
-                                'CHECKSUM MATCHES!'
-                                )
+                    xml_flag = 1
+                    with open(manifest, 'r', encoding='utf-8') as fo:
+                        manifest_lines = fo.readlines()
+                        for line in manifest_lines:
+                            if line.lower().replace('\n', '').endswith('.mxf'):
+                                mxf_checksum = line[:32]
+                                #mxf_checksum = str(digest_with_progress(mxf, 1024))
+                                print(mxf_checksum + ' - mxf checksum from package manifest')
+                    try:
+                        dpp_xml_parse = etree.parse(full_xml_path)
+                        dpp_xml_namespace = dpp_xml_parse.xpath('namespace-uri(.)')
+                        #parsed values from dpp xml
+                        series_title = dpp_xml_parse.findtext(
+                            '//ns:SeriesTitle',
+                            namespaces={'ns':dpp_xml_namespace}
+                        )
+                        prog_title = dpp_xml_parse.findtext(
+                            '//ns:ProgrammeTitle',
+                            namespaces={'ns':dpp_xml_namespace}
+                        )
+                        ep_num = dpp_xml_parse.findtext(
+                            '//ns:EpisodeTitleNumber',
+                            namespaces={'ns':dpp_xml_namespace}
+                        )
+                        checksum = dpp_xml_parse.findtext(
+                            '//ns:MediaChecksumValue',
+                            namespaces={'ns':dpp_xml_namespace}
                         )
-                    else:
-                        append_csv(
+                        print(checksum + ' - mxf checksum from DPP XML')
+                        accession_number_id = ''
+                        if os.path.isfile(log):
+                            with open(log, 'r', encoding='utf-8') as log_object:
+                                log_lines = log_object.readlines()
+                                for lines in log_lines:
+                                    if 'eventIdentifierType=object entry,' in lines:
+                                        source_oe = lines.split('=')[-1].replace('\n', '')
+                                    if 'eventIdentifierType=accession number,' in lines:
+                                        accession_number_id = lines.split('=')[-1].replace('\n', '')
+                        print('Generating Report.... ')
+                        if mxf_checksum == checksum:
+                            print(source_oe + 'Checksum MATCHES!\n---')
+                            ififuncs.append_csv(
+                                csv_report,
+                                (
+                                    os.path.basename(os.path.dirname(uuid_dir)),
+                                    source_oe,
+                                    accession_number_id,
+                                    dicto[os.path.basename(os.path.dirname(uuid_dir))][0],
+                                    dicto[os.path.basename(os.path.dirname(uuid_dir))][1],
+                                    filename,
+                                    unidecode.unidecode(series_title),
+                                    unidecode.unidecode(prog_title),
+                                    unidecode.unidecode(ep_num),
+                                    checksum,
+                                    mxf_checksum,
+                                    'CHECKSUM MATCHES!'
+                                    )
+                            )
+                        else:
+                            print(source_oe + 'Checksum does NOT MATCH!\n---'),
+                            ififuncs.append_csv(
+                                csv_report,
+                                (
+                                    os.path.basename(os.path.dirname(uuid_dir)),
+                                    source_oe,
+                                    accession_number_id,
+                                    dicto[os.path.basename(os.path.dirname(uuid_dir))][0],
+                                    dicto[os.path.basename(os.path.dirname(uuid_dir))][1],
+                                    filename,
+                                    unidecode.unidecode(series_title),
+                                    unidecode.unidecode(prog_title),
+                                    unidecode.unidecode(ep_num),
+                                    checksum,
+                                    mxf_checksum,
+                                    'CHECKSUM DOES NOT MATCH!'
+                                    )
+                            )
+                    except AttributeError:
+                        print(source_oe + 'Checksum does NOT MATCH or wrong source!\n---')
+                        ififuncs.append_csv(
                             csv_report,
                             (
                                 os.path.basename(os.path.dirname(uuid_dir)),
                                 source_oe,
                                 accession_number_id,
                                 dicto[os.path.basename(os.path.dirname(uuid_dir))][0],
                                 dicto[os.path.basename(os.path.dirname(uuid_dir))][1],
                                 filename,
-                                unidecode.unidecode(series_title),
-                                unidecode.unidecode(prog_title),
-                                unidecode.unidecode(ep_num),
-                                checksum,
-                                mxf_checksum,
-                                'CHECKSUM DOES NOT MATCH!'
+                                'error',
+                                'error',
+                                'error',
+                                'error',
+                                'error',
+                                'CHECKSUM DOES NOT MATCH or WRONG SOURCE!'
                                 )
-                        )
-                except AttributeError:
-                    append_csv(
-                        csv_report,
-                        (
-                            os.path.basename(os.path.dirname(uuid_dir)),
-                            source_oe,
-                            accession_number_id,
-                            dicto[os.path.basename(os.path.dirname(uuid_dir))][0],
-                            dicto[os.path.basename(os.path.dirname(uuid_dir))][1],
-                            filename,
-                            'error',
-                            'error',
-                            'error',
-                            'error',
-                            'error',
-                            'CHECKSUM DOES NOT MATCH!'
                             )
-                        )
-    print("Report complete - Time elaspsed : ", datetime.now() - startTime)
+                else:
+                    continue
+            if xml_flag == 0:
+                print(dirpath + '\n*****There is no metadata xml file in the supplement directory!\n*****Check if the structure is correct.\n---')
+                continue
+    print("Report complete\nTime elaspsed : ", datetime.now() - startTime)
+    print("Location: " + csv_report)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ifiscripts-2023.5.24.1/scripts/batchaccession.py` & `ifiscripts-2023.6.30.1/scripts/batchaipcreator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/env python3
 '''
-Batch process packages by running accession.py and makepbcore.py
+Batch process packages by running aipcreator.py and makepbcore.py
 The outcome will be:
-* Packages are accessioned
+* AIP is created
 * Filmographic records can be ingested to DB TEXTWORKS
 * Technical records can be ingested to DB TEXTWORKS
-* Skeleton accession record can be also be made available.
-
-NOTE - this is almost done, you just need to find when to_accession[package] == 3, then
-add an arg to the accession commmand that will declare the package as a reproduction.
+* Skeleton accession register record can be also be made available.
 '''
 import argparse
 import sys
 import csv
 import os
 import re
 import time
 import ififuncs
-import accession
+import aipcreator
 import copyit
 import order
 
 '''
 the following two functions for natural sorting are stolen from
 https://stackoverflow.com/questions/5967500/how-to-correctly-sort-a-string-with-a-number-inside?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa
 '''
@@ -43,97 +40,97 @@
     metadata and store in a single file for the purposes of batch import into
     the DB TEXTWORKS technical database.
     '''
     metadata = []
     for root, _, filenames in sorted(os.walk(source)):
         for filename in filenames:
             if filename.endswith('pbcore.csv'):
-                with open(os.path.join(root,filename), 'r') as csv_file:
+                with open(os.path.join(root,filename), 'r', encoding='utf-8') as csv_file:
                     csv_rows = csv_file.readlines()
                 if metadata:
                     metadata.append([csv_rows[1]])
                 else:
                     metadata.append([csv_rows[0]])
                     metadata.append([csv_rows[1]])
     collated_pbcore = os.path.join(
         ififuncs.make_desktop_logs_dir(),
         time.strftime("%Y-%m-%dT%H_%M_%S_pbcore.csv")
     )
-    with open(collated_pbcore, 'w') as fo:
+    with open(collated_pbcore, 'w', encoding='utf-8') as fo:
         for i in metadata:
             fo.write(i[0])
     return collated_pbcore
 
 
-def initial_check(args, accession_digits, oe_list, reference_number):
+def initial_check(args, accession_digits, oe_list, filmo_number):
     '''
-    Tells the user which packages will be accessioned and what their accession
+    Tells the user which AIPs will be created and what their accession
     numbers will be.
     '''
     to_accession = {}
     wont_accession = []
     # accession = 'af' + str(accession_digits)
-    ref = reference_number
-    reference_digits = int(ref[2:])
+    ref = filmo_number
+    filmo_digits = int(ref[2:])
     # so just reverse this - loop through the csv first.
-    # this will break the non CSV usage of batchaccession for now.
+    # this will break the non CSV usage of batchaipcreator for now.
     for thingies in oe_list:
         for root, _, _ in sorted(os.walk(args.input)):
             if os.path.basename(root)[:2] == 'oe' and len(os.path.basename(root)[2:]) >= 4:
                 if copyit.check_for_sip(root) is None:
                     wont_accession.append(root)
                 else:
-                    # this is just batchaccessioning if no csv is supplied
+                    # this is just batchaipcreator if no csv is supplied
                     # this is pretty pointless at the moment seeing as this is loopline through oe_list :(
                     if not oe_list:
                         to_accession[root] = 'aaa' + str(accession_digits).zfill(4)
                         accession_digits += 1
                     else:
                         # gets parent info
                         if os.path.basename(root) == thingies:
                             to_accession[
                                 os.path.join(os.path.dirname(root),
                                              order.main(root))
                             ] = [
                                 'aaa' + str(accession_digits).zfill(4),
-                                ref[:2] + str(reference_digits).zfill(4)
+                                ref[:2] + str(filmo_digits).zfill(4)
                             ]
                             if root in to_accession:
                                 # If a single file is found, this prevents the file being
                                 # processed twice, with a skip in the number run
-                                reference_digits += 1
+                                filmo_digits += 1
                                 accession_digits += 1
                                 continue
                             accession_digits += 1
                             # gets reproduction info
-                            to_accession[root] = ['aaa' + str(accession_digits).zfill(4), ref[:2] + str(reference_digits), 'reproduction']
-                            reference_digits += 1
+                            to_accession[root] = ['aaa' + str(accession_digits).zfill(4), ref[:2] + str(filmo_digits), 'reproduction']
+                            filmo_digits += 1
                             accession_digits += 1
     for fails in wont_accession:
         print('%s looks like it is not a fully formed SIP. Perhaps loopline_repackage.py should proccess it?' % fails)
     for success in sorted(to_accession.keys()):
-        print('%s will be accessioned as %s' %  (success, to_accession[success]))
+        print('%s will be AIPed as %s' %  (success, to_accession[success]))
     return to_accession
 
 def get_filmographic_titles(to_accession, filmographic_dict):
     '''
-    Retrieves filmographic titles of packages to be accessioned for QC purposes
+    Retrieves filmographic titles of packages to be AIPed for QC purposes
     '''
     for ids in to_accession:
         oe_number = os.path.basename(ids)
         oe = oe_number[:2].upper() + '-' + oe_number[2:]
         for record in filmographic_dict:
             if record['Object Entry'] == oe:
                 print(record['Title'])
 def parse_args(args_):
     '''
     Parse command line arguments.
     '''
     parser = argparse.ArgumentParser(
-        description='Batch process packages by running accession.py and makepbcore.py'
+        description='Batch process packages by running aipcreator.py and makepbcore.py'
         ' Written by Kieran O\'Leary.'
     )
     parser.add_argument(
         'input', help='Input directory'
     )
     parser.add_argument(
         '-start_number',
@@ -144,36 +141,36 @@
         help='Enter the path to the Filmographic CSV'
     )
     parser.add_argument(
         '-oe_csv',
         help='Enter the path to the Object Entry CSV'
     )
     parser.add_argument(
-        '-reference',
-        help='Enter the starting Filmographic reference number for the representation. This is not required when using the -oe_csv option'
+        '-filmo_number',
+        help='Enter the starting Filmographic URN for the representation. This is not required when using the -oe_csv option'
     )
     parser.add_argument(
         '-dryrun', action='store_true',
         help='The script will reveal which identifiers will be assigned but will not actually perform any actions.'
     )
     parsed_args = parser.parse_args(args_)
     return parsed_args
 
 
-def get_filmographic_number(number):
+def get_filmographic_number(filmo_number):
     '''
     This check is not sustainable, will have to be made more flexible!
     '''
-    if len(number) == 7:
-        if number[:3] != 'af1':
-            number = ififuncs.get_reference_number()
-        return number.upper()
+    if len(filmo_number) == 7:
+        if filmo_number[:3] != 'af1':
+            filmo_number = ififuncs.get_filmo_number()
+        return filmo_number.upper()
     else:
-        number = ififuncs.get_reference_number()
-        return number.upper()
+        filmo_number = ififuncs.get_filmo_number()
+        return filmo_number.upper()
 
 
 def get_number(args):
     '''
     Figure out the first accession number and how to increment per package.
     '''
     if args.start_number:
@@ -202,33 +199,33 @@
         try:
             dictionary = {}
             dictionary['Object Entry'] = record['OE No.']
             dictionary['format'] = record['Format']
             dictionary['donation_date'] = record['Date Received']
             dictionary['normalised_oe_number']  = dictionary['Object Entry'][:2].lower() + dictionary['Object Entry'][3:]
             dictionary['source_path'] = os.path.join(source_path, dictionary['normalised_oe_number'])
-            dictionary['reference number'] = record['Additional Information'].split('Representation of ')[1].split('|')[0].rstrip()
+            dictionary['Filmographic URN'] = record['Additional Information'].split('Representation of ')[1].split('|')[0].rstrip()
             oe_dicts.append(dictionary)
         except IndexError:
             continue
         try:
             dictionary['parent'] = record['Additional Information'].split('Reproduction of ')[1].split('|')[0].rstrip()
         except IndexError:
             dictionary['parent'] = 'n/a'
     return oe_dicts
 
 def main(args_):
     '''
-    Batch process packages by running accession.py and makepbcore.py
+    Batch process packages by running aipcreator.py and makepbcore.py
     '''
     args = parse_args(args_)
     oe_list = []
     if args.oe_csv:
         if not args.filmo_csv:
-            print(' - batchaccession.py - ERROR\n - No -filmographic argument supplied. This is mandatory when using the -oe_csv option. \n - Exiting..')
+            print(' - batchaipcreator.py - ERROR\n - No -filmographic argument supplied. This is mandatory when using the -oe_csv option. \n - Exiting..')
             sys.exit()
         oe_csv_extraction = ififuncs.extract_metadata(args.oe_csv)
         initial_oe_list = oe_csv_extraction[0]
         oe_dicts = process_oe_csv(oe_csv_extraction, args.input)
         # temp hack while we're performing both workflows
         helper_csv = args.oe_csv
     elif args.filmo_csv:
@@ -241,41 +238,41 @@
                 oe_number = line_item['Object Entry'].lower()
             except KeyError:
                 oe_number = line_item['OE No.'].lower()
             # this transforms OE-#### to oe####
             transformed_oe = oe_number[:2] + oe_number[3:]
             oe_list.append(transformed_oe)
     if not args.oe_csv:
-        # No need to ask for the reference number if the OE csv option is supplied.
-        # The assumption here is that the OE csv contains the reference numbers though.
-        if args.reference:
-            reference_number = get_filmographic_number(args.reference)
+        # No need to ask for the Filmographic URN if the OE csv option is supplied.
+        # The assumption here is that the OE csv contains the Filmographic URN though.
+        if args.filmo_number:
+            filmo_number = get_filmographic_number(args.filmo_number)
         else:
-            reference_number = ififuncs.get_reference_number()
+            filmo_number = ififuncs.get_filmo_number()
     donor = ififuncs.ask_question('Who is the source of acquisition, as appears on the donor agreement? This will not affect Reproductions.')
     depositor_reference = ififuncs.ask_question('What is the donor/depositor number? This will not affect Reproductions.')
     reproduction_creator = ififuncs.ask_question('Who is the reproduction creator? This will not affect acquisitions. Enter n/a if not applicable')
     acquisition_type = ififuncs.get_acquisition_type('')
     user = ififuncs.get_user()
     accession_number = get_number(args)
     accession_digits = int(accession_number[3:])
     if not args.oe_csv:
-        to_accession = initial_check(args, accession_digits, oe_list, reference_number)
+        to_accession = initial_check(args, accession_digits, oe_list, filmo_number)
     else:
         to_accession = {}
         print('\nIngested info from CSVs: Please check the following if an error occurs')
         for oe_record in oe_dicts:
             print(oe_record)
             if os.path.isdir(oe_record['source_path']):
-                to_accession[oe_record['source_path']] = ['aaa' + str(accession_digits).zfill(4), oe_record['reference number'], oe_record['parent'], oe_record['donation_date']]
+                to_accession[oe_record['source_path']] = ['aaa' + str(accession_digits).zfill(4), oe_record['Filmographic URN'], oe_record['parent'], oe_record['donation_date']]
                 accession_digits += 1
         print('\n')
     for success in sorted(to_accession.keys()):
-        print('%s will be accessioned as %s' %  (success, to_accession[success]))
-    register = accession.make_register()
+        print('%s will be AIPed as %s' %  (success, to_accession[success]))
+    register = aipcreator.make_register()
     if args.filmo_csv:
         desktop_logs_dir = ififuncs.make_desktop_logs_dir()
         if args.dryrun:
             new_csv_filename = time.strftime("%Y-%m-%dT%H_%M_%S_DRYRUN_SHEET_PLEASE_DO_NOT_INGEST_JUST_IGNORE_COMPLETELY") + os.path.basename(args.filmo_csv)
         else:
             new_csv_filename = time.strftime("%Y-%m-%dT%H_%M_%S_") + os.path.basename(args.filmo_csv)
         new_csv = os.path.join(desktop_logs_dir, new_csv_filename)
@@ -290,66 +287,74 @@
                 fieldnames = headers
                 # Removes Object Entry from headings as it's not needed in database.
                 del fieldnames[1]
                 writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
                 writer.writeheader()
                 for i in filmographic_dict:
                     i.pop('Object Entry', None)
-                    # Only include records that have reference numbers
+                    # Only include records that have Filmographic URN
                     if not i['Filmographic URN'] == '':
                         writer.writerow(i)
     if not to_accession:
         print('`/*** Exiting as there is no data to process. This is usually because:\n* Your OE register does not match the values\n* OR your "representation of: " values in the Object entry do not match to values in your filmographic CSV\n* OR your filmographic CSV does not contain values that match to the representation of values in the Object Entry CSV')
         sys.exit()
     filmographic_dict, headers = ififuncs.extract_metadata(args.filmo_csv)
     for package in to_accession:
-        filmo = False
-        filmo_ref = to_accession[package][1]
+        filmo_match = False
+        filmo_lower = []
+        filmo_number_oe_csv = to_accession[package][1]
         for record in filmographic_dict:
-            if filmo_ref.upper() == record["Filmographic URN"]:
-                filmo = True
-        if filmo is False:
-            print('\n*** WARNING it appears that %s is not present in your filmographic CSV - proceeding will probably result in a crash' % filmo_ref)
+            if filmo_number_oe_csv.upper() == record["Filmographic URN"]:
+                filmo_match = True
+            if filmo_number_oe_csv.lower() == record["Filmographic URN"]:
+                filmo_match = False
+                filmo_lower.append(filmo_number_oe_csv)
+        if filmo_match is False:
+            print('\n*** WARNING it appears that %s is not present in your filmographic CSV - proceeding will probably result in a crash' % filmo_number_oe_csv)
+        if filmo_lower:
+            print('\n*** These Filmographic URN(s) in the filmographic CSV are in lower case: ')
+            print(filmo_lower, sep=', ')
     if args.dryrun:
         sys.exit()
     proceed = ififuncs.ask_yes_no(
         'Do you want to proceed?'
     )
     if args.oe_csv:
         new_csv = args.filmo_csv
     if proceed == 'Y':
         for package in sorted(to_accession.keys(), key=natural_keys):
             accession_cmd = [
                 package, '-user', user,
                 '-force',
-                '-number', to_accession[package][0],
-                '-reference', to_accession[package][1],
+                '-accession_number', to_accession[package][0],
+                '-filmo_number', to_accession[package][1],
                 '-register', register,
                 '-filmo_csv', new_csv
             ]
             for oe_record in oe_dicts:
                 if oe_record['source_path'] == package:
                     if not oe_record['format'].lower() == 'dcdm':
                         accession_cmd.append('-pbcore')
             if len(to_accession[package]) == 4:
                 if not to_accession[package][2] == 'n/a':
-                    accession_cmd.extend(['-acquisition_type', '13'])
+                    # acquisition_type target to the index of reproduction
+                    accession_cmd.extend(['-acquisition_type', '4'])
                     if args.oe_csv:
                         accession_cmd.extend(['-parent', to_accession[package][2]])
                         accession_cmd.extend(['-reproduction_creator', reproduction_creator])
                     else:
                         accession_cmd.extend(['-parent', order.main(package)])
                 else:
                     accession_cmd.extend(['-donor', donor])
                     accession_cmd.extend(['-depositor_reference', depositor_reference])
                     accession_cmd.extend(['-acquisition_type', acquisition_type[2]])
                     print(to_accession[package][3])
                     accession_cmd.extend(['-donation_date', to_accession[package][3]])
             print(accession_cmd)
-            accession.main(accession_cmd)
+            aipcreator.main(accession_cmd)
     collated_pbcore = gather_metadata(args.input)
     sorted_filepath = ififuncs.sort_csv(register, 'accession number')
     print('\nA helper accessions register has been generated in order to help with registration - located here: %s' % sorted_filepath)
-    print('\nA modified filmographic CSV has been generated with added reference numbers - located here: %s' % new_csv)
+    print('\nA modified filmographic CSV has been generated with added Filmographic URN - located here: %s' % new_csv)
     print('\nA collated CSV consisting of each PBCore report has been generated for batch database import - located here: %s' % collated_pbcore)
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.5.24.1/scripts/batchmakeshell.py` & `ifiscripts-2023.6.30.1/scripts/batchmakeshell.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 import shutil
 
 
 def set_options():
     parser = argparse.ArgumentParser(
-        description='IFI Irish Film Institute accession shell creator.'
+        description='IFI Irish Film Institute AIPs shell creator.'
                     ' Written by Yazhou He.'
     )
     parser.add_argument(
         'input'
     )
     parser.add_argument(
         '-as11',
```

### Comparing `ifiscripts-2023.5.24.1/scripts/batchsipcreator.py` & `ifiscripts-2023.6.30.1/scripts/batchsipcreator.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/bitc.py` & `ifiscripts-2023.6.30.1/scripts/bitc.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/concat.py` & `ifiscripts-2023.6.30.1/scripts/concat.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/copyit.py` & `ifiscripts-2023.6.30.1/scripts/copyit.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/dcpaccess.py` & `ifiscripts-2023.6.30.1/scripts/dcpaccess.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/dcpfixity.py` & `ifiscripts-2023.6.30.1/scripts/dcpfixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/deletefiles.py` & `ifiscripts-2023.6.30.1/scripts/deletefiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 '''
-Deletes files after sipcreator has been run, but before accession.py has been run.
+Deletes files after sipcreator has been run, but before aipcreator.py has been run.
 Manifests are updated and metadata is deleted.
 '''
 import os
 import argparse
 import sys
 import datetime
 import ififuncs
```

### Comparing `ifiscripts-2023.5.24.1/scripts/dfxml.py` & `ifiscripts-2023.6.30.1/scripts/dfxml.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/durationcheck.py` & `ifiscripts-2023.6.30.1/scripts/durationcheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/ffv1mkvvalidate.py` & `ifiscripts-2023.6.30.1/scripts/ffv1mkvvalidate.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/framemd5.py` & `ifiscripts-2023.6.30.1/scripts/framemd5.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #!/usr/bin/env python3
 '''
 Creates framemd5 sidecars on all mov/mkv files in all subfolders beneath your input.
 If the input is a file, then framemd5.py will just generate a sidecar for this one file.
 '''
 import subprocess
 import os
+import sys
 import argparse
 import ififuncs
 
-def parse_args():
+def parse_args(args_):
     '''
     Parse command line arguments.
     '''
     parser = argparse.ArgumentParser(
         description='Creates framemd5 sidecars on all mov/mkv files in all subfolders beneath your input.'
         ' If the input is a file, then framemd5.py will just generate a sidecar for this one file.'
     )
     parser.add_argument(
         '-i',
         help='full path of input file or directory', required=True
     )
-    parsed_args = parser.parse_args()
+    parsed_args = parser.parse_args(args_)
     return parsed_args
 
-def main():
+def main(args_):
     '''
     Simple recursive process that makes framemd5 sidecar reports.
     '''
     ififuncs.check_existence(['ffmpeg'])
-    args = parse_args()
+    args = parse_args(args_)
     source = args.i
     fmd5 = source + '_source.framemd5'
     if os.path.isfile(source):
         cmd = [
             'ffmpeg',
             '-i',
             source,
@@ -57,9 +58,9 @@
                             '-an',
                             full_path + '_source.framemd5'
                             ]
                         subprocess.call(cmd)
 
 
 if __name__ == '__main__':
-    main()
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.5.24.1/scripts/ififuncs.py` & `ifiscripts-2023.6.30.1/scripts/ififuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,24 +548,24 @@
         with open(manifest2check, "r") as fo:
             manifest_lines = [line.split(',') for line in fo.readlines()]
             count_in_manifest = len(manifest_lines)
     return count_in_manifest
 
 
 def create_csv(csv_file, *args):
-    f = open(csv_file, 'w', newline='')
+    f = open(csv_file, 'w', encoding='utf-8', newline='')
     try:
         writer = csv.writer(f)
         writer.writerow(*args)
     finally:
         f.close()
 
 
 def append_csv(csv_file, *args):
-    f = open(csv_file, 'a', newline='')
+    f = open(csv_file, 'a', encoding='utf-8', newline='')
     try:
         writer = csv.writer(f)
         writer.writerow(*args)
     finally:
         f.close()
 
 def sort_csv(csv_file, key):
@@ -739,37 +739,39 @@
     
 def get_user():
     '''
     Asks user who they are. Returns a string with their name
     '''
     user_list = ['Allison McGrail',
                 'Caroline Crowther',
+                'Cody Farren',
                 'Emma Battlebury',
                 'Gavin Martin',
                 'Mark Keleghan',
+                'Matheus Almeida',
                 'Niall Anderson',
                 'Raelene Casey',
                 'Raven Cooke',
                 'Yazhou He']
     user = ''
     if user not in user_list:
         print('\n\n**** Who are you?\nEnter the number before your name (ie. 1)\n\n')
         i = 1
         for user_item in user_list:
             print(str(i) + '.\t' + user_item)
             i = i + 1
-        print('\n\n(User list was last updated on 2023-05-23)\n')
+        print('\n\n(User list was last updated on 2023-06-30)\n')
         i = int(input())
         while i > len(user_list) or i < 1:
             print('\n\n**** Who are you?\Enter the number before your name (ie. 1)\n\n')
             i = 1
             for user_item in user_list:
                 print(str(i) + '.\t' + user_item)
                 i = i + 1
-            print('\n\n(User list was last updated on 2023-05-23)\n')
+            print('\n\n(User list was last updated on 2023-06-30)\n')
             i = int(input())
     user = user_list[i-1]
     print('\nUser selected: ' + user)
     time.sleep(1)
     return user
 
 
@@ -785,47 +787,42 @@
     return user
 
 
 def get_acquisition_type(acquisition_type):
     '''
     Asks user for the type of acquisition
     '''
-    if acquisition_type not in ('1', '2', '4', '5', '7', '8', '13', '14'):
+    if acquisition_type not in ('1', '2', '3', '4', '5', '6'):
         acquisition_type = input(
-            '\n\n**** What is the type of acquisition? - This will not affect Reproductions that have been auto-detected.\nPress 1,2,4,5,7,8,13,14\n\n1. IFB -  deposited  in compliance with IFB delivery requirements\n2. BAI  - deposited  in compliance with BAI delivery requirements\n4. Deposit\n5. Purchased for collection\n7. Unknown at present\n8. Arts Council- deposited in compliance with Arts council delivery requirements\n13. Reproduction\n14. Donation\n'
+            '\n\n**** What is the type of acquisition? - This will not affect Reproductions that have been auto-detected.\nPress 1,2,3,4,5,6\n\n1. Deposit\n2. Deposit via overarching agreements\n3. Donation\n4. Reproduction\n5. Purchased for collection\n6. Unknown at present\n'
         )
-        while acquisition_type not in ('1', '2', '4', '5', '7', '8', '13', '14'):
+        while acquisition_type not in ('1', '2', '3', '4', '5', '6'):
             acquisition_type = input(
-                '\n\n**** What is the type of acquisition? - This will not affect Reproductions that have been auto-detected.\nPress 1,2,4,5,7,8,13,14\n\n1. IFB -  deposited  in compliance with IFB delivery requirements\n2. BAI  - deposited  in compliance with BAI delivery requirements\n4. Deposit\n5. Purchased for collection\n7. Unknown at present\n8. Arts Council- deposited in compliance with Arts council delivery requirements\n13. Reproduction\n14. Donation\n'
+                '\n\n**** What is the type of acquisition? - This will not affect Reproductions that have been auto-detected.\nPress 1,2,3,4,5,6\n\n1. Deposit\n2. Deposit via overarching agreements\n3. Donation\n4. Reproduction\n5. Purchased for collection\n6. Unknown at present\n'
             )
     if acquisition_type == '1':
-        acquisition_type = ['1. IFB -  deposited  in compliance with IFB delivery requirements', 'Deposit', '1']
+        acquisition_type = ['Deposit', 'Deposit', '1']
         time.sleep(1)
     elif acquisition_type == '2':
-        acquisition_type = ['2. BAI  - deposited  in compliance with BAI delivery requirements', 'Deposit', '2']
+        acquisition_type = ['Deposit via overarching agreements', 'Deposit', '2']
+        time.sleep(1)
+    elif acquisition_type == '3':
+        acquisition_type = ['Donation', 'Donation', '3']
         time.sleep(1)
     elif acquisition_type == '4':
-        acquisition_type = ['4. Deposit', 'Deposit', '4']
+        acquisition_type = ['Reproduction', 'Reproduction', '4']
         time.sleep(1)
     elif acquisition_type == '5':
-        acquisition_type = ['5. Purchased for collection', 'Purchase', '5']
-        time.sleep(1)
-    elif acquisition_type == '7':
-        acquisition_type = ['7. Unknown at present', 'Unknown', '7']
-        time.sleep(1)
-    elif acquisition_type == '8':
-        acquisition_type = ['Arts Council- deposited in compliance with Arts council delivery requirements', 'Deposit', '8']
-        time.sleep(1)
-    elif acquisition_type == '13':
-        acquisition_type = ['Reproduction', 'Reproduction', '13']
-        time.sleep(1)
-    elif acquisition_type == '14':
-        acquisition_type = ['Donation', 'Donation', '14']
+        acquisition_type = ['Purchased for collection', 'Purchase', '5']
         time.sleep(1)
+    elif acquisition_type == '6':
+        acquisition_type = ['Unknown at present', 'Unknown', '6']
+        time.sleep(1)        
     return acquisition_type
+
 def sort_manifest(manifest_textfile):
     '''
     Sorts an md5 manifest in alphabetical order.
     Some scripts like moveit.py will require a manifest to be ordered like this.
     '''
     with open(manifest_textfile, "r", encoding='utf-8') as fo:
         manifest_lines = fo.readlines()
@@ -1002,23 +999,23 @@
             print(' - First three characters must be \'aaa\' and last four characters must be four digits')
         elif not accession_number[3:].isdigit():
             accession_number = False
             print(' - First three characters must be \'aaa\' and last four characters must be four digits')
         else:
             return accession_number
 
-def get_reference_number():
+def get_filmo_number():
     '''
-    Asks user for a Filmographic reference number. Due to the variety of reference numbers, validation
-    will be removed for now.
+    Asks user for a Filmographic URN. Due to the variety 
+    of Filmographic URN, validation will be removed for now.
     '''
-    reference_number = input(
-        '\n\n**** Please enter the Filmographic reference number of the representation- if there is more than one work that is represented, seperate them with an ampersand, eg af1234&aa675\n\n'
+    get_filmo_number = input(
+        '\n\n**** Please enter the Filmographic URN of the representation- if there is more than one work that is represented, seperate them with an ampersand, eg af1234&aa675\n\n'
     )
-    return reference_number.upper()
+    return get_filmo_number.upper()
 
 def get_contenttitletext(cpl):
     '''
     Returns the <ContentTitleText> element text from a DCP CPL.xml
     '''
     cpl_parse = etree.parse(cpl)
     cpl_namespace = cpl_parse.xpath('namespace-uri(.)')
@@ -1423,15 +1420,15 @@
     groups a uuid with its parent uuid in a dictionary
     '''
     uuid_oe_dict = {}
     for root, dirnames, _ in os.walk(source):
         if os.path.basename(root)[:2] == 'oe':
             if validate_uuid4(dirnames[0]) is not False:
                 uuid_oe_dict[os.path.basename(root)] = dirnames[0]
-        # check for accessioned packages
+        # check for AIPs
         elif os.path.basename(root)[:3] == 'aaa':
             if validate_uuid4(dirnames[0]) is not False:
                 uuid_oe_dict[os.path.basename(root)] = dirnames[0]
     return uuid_oe_dict
 
 def convert_ms2frames(fps, ms):
     # taken from https://github.com/atvKumar/Scene_Cut_Detection/blob/93622d250dc38907ee7d3ee8d925c4bfb76129b6/timecode_utils.py'
```

### Comparing `ifiscripts-2023.5.24.1/scripts/loopline_repackage.py` & `ifiscripts-2023.6.30.1/scripts/loopline_repackage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 '''
 Retrospectively updates older FFV1/DV packages in order to meet our current
-packaging requirements. This should allow accession.py and makepbcore.py to run as
+packaging requirements. This should allow aipcreator.py and makepbcore.py to run as
 expected. This script should work on files created by:
 makeffv1.py
 dvsip.py
 loopline.py
 '''
 import argparse
 import sys
@@ -17,15 +17,15 @@
 def parse_args(args_):
     '''
     Parse command line arguments.
     '''
     parser = argparse.ArgumentParser(
         description='Retrospectively updates older FFV1/DV packages in order to'
         'meet our current packaging requirements. This should allow'
-        ' accession.py and makepbcore.py to run as expected.'
+        ' aipcreator.py and makepbcore.py to run as expected.'
         ' Written by Kieran O\'Leary.'
     )
     parser.add_argument(
         'input', help='Input directory'
     )
     parser.add_argument(
         '-start_number',
@@ -33,33 +33,33 @@
     )
     parser.add_argument(
         '-technical',
         help='Path to technical/PBCore CSV.'
     )
     parser.add_argument(
         '-filmographic',
-        help='Path to Filmographic CSV. Must contain reference numbers.'
+        help='Path to Filmographic CSV. Must contain Filmographic URN.'
     )
     parsed_args = parser.parse_args(args_)
     return parsed_args
 
 def get_numbers(args):
     '''
     Figure out the first OE number and how to increment per package.
     '''
     if args.start_number:
         if args.start_number[:2] != 'oe':
-            print 'First two characters must be \'oe\' and last four characters must be four digits'
+            print('First two characters must be \'oe\' and last four characters must be four digits')
             object_entry = ififuncs.get_object_entry()
         elif len(args.start_number[2:]) not in range(4, 6):
-            print 'First two characters must be \'oe\' and last four characters must be four digits'
+            print('First two characters must be \'oe\' and last four characters must be four digits')
             object_entry = ififuncs.get_object_entry()
         elif not args.start_number[2:].isdigit():
             object_entry = ififuncs.get_object_entry()
-            print 'First two characters must be \'oe\' and last four characters must be four digits'
+            print('First two characters must be \'oe\' and last four characters must be four digits')
         else:
             object_entry = args.start_number
     else:
         object_entry = ififuncs.get_object_entry()
     object_entry_digits = int(object_entry[2:])
     new_object_entry = 'oe' + str(object_entry_digits)
     return new_object_entry
@@ -211,15 +211,15 @@
                         log = os.path.join(log_dir, files)
                 manifest = os.path.join(
                     os.path.dirname(root),
                     old_oe + '_manifest.md5'
                     )
                 uuid = ififuncs.create_uuid()
                 uuid_event = (
-                    'EVENT = eventType=Identifier assignement,'
+                    'EVENT = eventType=Identifier assignment,'
                     ' eventIdentifierType=UUID, value=%s, module=uuid.uuid4'
                 ) % uuid
                 ififuncs.generate_log(
                     log,
                     'EVENT = loopline_repackage.py started'
                 )
                 ififuncs.generate_log(
@@ -236,22 +236,22 @@
                 )
                 ififuncs.generate_log(
                     log,
                     uuid_event
                 )
                 ififuncs.generate_log(
                     log,
-                    'EVENT = eventType=Identifier assignement,'
+                    'EVENT = eventType=Identifier assignment,'
                     ' eventIdentifierType=object entry, value=%s'
                     % new_object_entry
                 )
                 ififuncs.generate_log(
                     log,
-                    'EVENT = eventType=Identifier assignement,'
-                    ' eventIdentifierType=Filmographic reference number , value=%s'
+                    'EVENT = eventType=Identifier assignment,'
+                    ' eventIdentifierType=Filmographic URN , value=%s'
                     % oe_package['filmographic_reference_number']
                 )
                 oe_package['new_object_entry'] = new_object_entry
                 print('Transforming %s into %s' % (oe_package['old_oe'], oe_package['new_object_entry']))
                 ififuncs.generate_log(
                         log,
                         'Relationship, derivation, has source=%s' % oe_package['source_accession_number']
```

### Comparing `ifiscripts-2023.5.24.1/scripts/make_mediaconch.py` & `ifiscripts-2023.6.30.1/scripts/make_mediaconch.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/makedfxml.py` & `ifiscripts-2023.6.30.1/scripts/makedfxml.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/makedip.py` & `ifiscripts-2023.6.30.1/scripts/makedip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/makeffv1.py` & `ifiscripts-2023.6.30.1/scripts/makeffv1.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/makepbcore.py` & `ifiscripts-2023.6.30.1/scripts/makepbcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,20 +144,16 @@
         'input', help='Input directory'
     )
     parser.add_argument(
         '-user',
         help='Declare who you are. If this is not set, you will be prompted.'
     )
     parser.add_argument(
-        '-accession',
-        help='Enter the Accession number for the representation.'
-    )
-    parser.add_argument(
-        '-reference',
-        help='Enter the Filmographic reference number for the representation.'
+        '-filmo_number',
+        help='Enter the Filmographic URN for the representation.'
     )
     parser.add_argument(
         '-p', action='store_true',
         help='Adds the PBCore CSV to the metadata folder'
     )
     parser.add_argument(
         '-parent',
@@ -185,37 +181,37 @@
     )
     parsed_args = parser.parse_args(args_)
     return parsed_args
 
 
 def get_accession_number(source):
     '''
-    Checks if the package has been accessioned.
+    Checks if the AIP has been created.
     Returns the accession number if this is the case, otherwise the script exits.
     '''
     basename = os.path.basename(source)
     if len(basename) == 7:
         if basename[:3] == 'aaa':
             return basename
     else:
-        print('looks like your package has not been accessioned? Exiting!')
-        return 'not_accessioned'
+        print('looks like your AIP has not been created? Exiting!')
+        return 'not_AIPed'
 
 
-def get_reference_number(source):
+def get_filmo_number(source):
     '''
-    Checks if the reference number is in the folder path.
+    Checks if the filmographic URN is in the folder path.
     This check is not sustainable, will have to be made more flexible!
     '''
     basename = os.path.basename(os.path.dirname(source))
     if len(basename) == 7:
         if basename[:3] == 'af1':
             return basename
     else:
-        basename = ififuncs.get_reference_number()
+        basename = ififuncs.get_filmo_number()
         return basename
 
 
 def make_csv(csv_filename):
     '''
     Writes a CSV with IFI database headings.
     '''
@@ -361,18 +357,18 @@
     if args.acquisition_type:
         acquisition_type = ififuncs.get_acquisition_type(args.acquisition_type)[0]
     instantiationIdentif = ''
     for dirs in os.listdir(args.input):
         if ififuncs.validate_uuid4(dirs) is None:
             instantiationIdentif = dirs
     Accession_Number = get_accession_number(args.input)
-    if args.reference:
-        Reference_Number = args.reference.upper()
+    if args.filmo_number:
+        Reference_Number = args.filmo_number.upper()
     else:
-        Reference_Number = get_reference_number(args.input)
+        Reference_Number = get_filmo_number(args.input)
     if args.p:
         for root, _, filenames in os.walk(args.input):
             if os.path.basename(root) == 'metadata':
                 metadata_dir = root
             elif os.path.basename(root) == 'logs':
                 logs_dir = root
         csv_filename = os.path.join(metadata_dir, Accession_Number + '_%s_pbcore.csv' % Reference_Number)
```

### Comparing `ifiscripts-2023.5.24.1/scripts/makezip.py` & `ifiscripts-2023.6.30.1/scripts/makezip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/manifest.py` & `ifiscripts-2023.6.30.1/scripts/manifest.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/masscopy.py` & `ifiscripts-2023.6.30.1/scripts/masscopy.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/massqc.py` & `ifiscripts-2023.6.30.1/scripts/massqc.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/mergepbcore.py` & `ifiscripts-2023.6.30.1/scripts/mergepbcore.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 '''
 Just a helper script that collates PBCore CSV files from packages
 '''
 import argparse
-import batchaccession
+import batchaipcreator
 
 def parse_args():
     '''
     Parse command line arguments.
     '''
     parser = argparse.ArgumentParser(
         description='Collates PBCore CSV files from archival packages and stores in the Desktop logs folder'
@@ -18,13 +18,13 @@
     )
     parsed_args = parser.parse_args()
     return parsed_args
 
 def main():
     args = parse_args()
     source = args.input
-    collated_pbcore = batchaccession.gather_metadata(source)
+    collated_pbcore = batchaipcreator.gather_metadata(source)
     print('Merged PBCore CSV is stored in %s' % collated_pbcore)
 if __name__ == '__main__':
     main()
```

### Comparing `ifiscripts-2023.5.24.1/scripts/multicopy.py` & `ifiscripts-2023.6.30.1/scripts/multicopy.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/normalise.py` & `ifiscripts-2023.6.30.1/scripts/normalise.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/order.py` & `ifiscripts-2023.6.30.1/scripts/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 '''
 Audits logfiles to determine the parent of a derivative package.
 This script can aid in automating large accessioning procedures that involve
-the accessioning of derivatives along with masters, eg a Camera Card and
+the AIPing of derivatives along with masters, eg a Camera Card and
 a concatenated derivative, or a master file and a mezzanine.
 
 order.py will be able to determine if something is a reproduction,
 but it won't be able to tell if acquisitions are deposits, purchases or donations.
 So leave it blank in the latter instances.
 '''
 import sys
```

### Comparing `ifiscripts-2023.5.24.1/scripts/package_update.py` & `ifiscripts-2023.6.30.1/scripts/package_update.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/packagecheck.py` & `ifiscripts-2023.6.30.1/scripts/packagecheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/prores.py` & `ifiscripts-2023.6.30.1/scripts/prores.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/seq2ffv1.py` & `ifiscripts-2023.6.30.1/scripts/seq2ffv1.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/sipcreator.py` & `ifiscripts-2023.6.30.1/scripts/sipcreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 import shutil
 import datetime
 import time
 import atexit
 import copyit
 import ififuncs
 import package_update
-import accession
+import aipcreator
 import manifest
 import makezip
-import accession
 from masscopy import analyze_log
 try:
     from clairmeta.utils.xml import prettyprint_xml
     from clairmeta import DCP
     import dicttoxml
 except ImportError:
     print('Clairmeta is not installed. DCP options will not function!')
@@ -37,16 +36,17 @@
     desktop_manifest_dir = os.path.expanduser("~/Desktop/moveit_manifests")
     old_manifest_dir = os.path.join(desktop_manifest_dir, 'old_manifests')
     for i in os.listdir(desktop_manifest_dir):
         o = os.path.join(old_manifest_dir, i)
         i = os.path.join(desktop_manifest_dir, i)
         if i.endswith('.md5'):
             print('**** Found existing manifest: ' + i)
-            shutil.move(i, o)
-            print('**** Moved to old_manifest folder')
+            if i.endswith('objects_manifest.md5'):
+                shutil.move(i, o)
+                print('**** Moved object_manifest.md5 to old_manifest folder in case of content overlap. \n**** Check if other manifests are in use in other scripts before move them manually.')
 
 def make_folder_path(path, args, object_entry):
     '''
     Generates objects/logs/metadata/UUID folder structure in output directory.
     Asks user for UUID if it's not supplied in an arg.
     Adds a workaround for special collections workflows.
     Returns the path.
@@ -234,16 +234,16 @@
         help='special collections workflow'
     )
     parser.add_argument(
         '-zip', action='store_true',
         help='Uses makezip.py to store the objects in an uncompressed ZIP'
     )
     parser.add_argument(
-        '-accession', action='store_true',
-        help='Launches accession.py immediately after sipcreator.py finishes. This is only useful if the SIP has already passed QC and will definitely be accessioned and ingested.'
+        '-aipcreator', action='store_true',
+        help='Launches aipcreator.py immediately after sipcreator.py finishes. This is only useful if the SIP has already passed QC and will definitely be AIPed and ingested.'
     )
     parser.add_argument(
         '-filmo_csv',
         help='Enter the path to the Filmographic CSV so that the metadata will be stored within the package.'
     )
     parser.add_argument(
         '-oe',
@@ -335,29 +335,29 @@
     Validates a UUID to use as the SIP identifier.
     UNITTEST = validate the existing validations.
     '''
     if args.u:
         if ififuncs.validate_uuid4(args.u) is None:
             uuid = args.u
             uuid_event = (
-                'EVENT = eventType=Identifier assignement,'
+                'EVENT = eventType=Identifier assignment,'
                 ' eventIdentifierType=UUID, value=%s, module=uuid.uuid4'
             ) % uuid
         else:
             print('exiting due to invalid UUID')
             sys.exit()
     else:
         uuid = os.path.basename(sip_path)
         uuid_event = (
-            'EVENT = eventType=Identifier assignement,'
+            'EVENT = eventType=Identifier assignment,'
             ' eventIdentifierType=UUID, value=%s, module=uuid.uuid4'
         ) % uuid
     return uuid, uuid_event
 
-def process_dcp(sip_path, content_title, args, new_manifest_textfile, new_log_textfile, metadata_dir, clairmeta_version):
+def process_dcp(sip_path, content_title, args, new_manifest_textfile, new_log_textfile, txt_name_source, metadata_dir, clairmeta_version):
     '''
     Runs DCP specific functions.
     '''
     objects_dir = os.path.join(sip_path, 'objects')
     cpl = ififuncs.find_cpl(objects_dir)
     dcp_dirname = os.path.dirname(cpl)
     os.chdir(os.path.dirname(dcp_dirname))
@@ -375,14 +375,18 @@
     '''
     dcp = DCP(absolute_dcp_path)
     dcp_dict = dcp.parse()
     # json_str = json.dumps(dcp_dict , sort_keys=True, indent=2, separators=(',', ': '))
     xml_str = dicttoxml.dicttoxml(dcp_dict, custom_root='ClairmetaProbe', ids=False, attr_type=False)
     xml_pretty = prettyprint_xml(xml_str)
     status, report = dcp.check()
+    # print clairmeta result to ifiscripts_log/$oe_clairmeta_outcome_$datetime.txt
+    with open(txt_name_source, 'a') as file:
+        file.write(report.pretty_str())
+    print('\n\nClairmeta outcome has exported to' + txt_name_source)
     ififuncs.generate_log(
         new_log_textfile,
         'EVENT = eventType=validation, eventOutcome=%s, eventDetail=%s, agentName=Clairmeta version %s' % (
             status, report, clairmeta_version
         )
     )
     clairmeta_xml = os.path.join(metadata_dir, '%s_clairmeta.xml' % content_title)
@@ -390,16 +394,14 @@
         new_log_textfile,
         'EVENT = Metadata extraction - eventDetail=Clairmeta DCP metadata extraction, eventOutcome=%s, agentName=Clairmeta version %s' % (clairmeta_xml, clairmeta_version)
     )
     with open(clairmeta_xml, 'w') as fo:
         fo.write(xml_pretty)
     ififuncs.checksum_replace(new_manifest_textfile, new_log_textfile, 'md5')
     ififuncs.manifest_update(new_manifest_textfile, clairmeta_xml)
-    print(status)
-    print(report)
 
 def make_oe_register():
     '''
     This sends a placeholder oe register to the desktop logs directory.
     This should get rid of some of the more painful, repetitive identifier matching.
     '''
     desktop_logs_dir = ififuncs.make_desktop_logs_dir()
@@ -469,24 +471,34 @@
     ififuncs.generate_log(
         new_log_textfile,
         uuid_event
     )
     if not args.sc:
         ififuncs.generate_log(
             new_log_textfile,
-            'EVENT = eventType=Identifier assignement,'
-            ' eventIdentifierType=object entry, value=%s'
+            'EVENT = eventType=Identifier assignment,'
+            ' eventIdentifierType=object entry number, value=%s'
             % object_entry
         )
+        ififuncs.generate_log(
+            new_log_textfile,
+            'EVENT = eventType=Information package creation'
+        )
+        '''
+        ififuncs.generate_log(
+            new_log_textfile,
+            'EVENT = eventType=Information package creation, eventOutcomeDetailNote=Submission information package'
+        )
+        '''
     metadata_dir = os.path.join(sip_path, 'metadata')
     supplemental_dir = os.path.join(metadata_dir, 'supplemental')
     logs_dir = os.path.join(sip_path, 'logs')
-    if args.accession:
+    if args.aipcreator:
         accession_number = ififuncs.get_accession_number()
-        reference_number = ififuncs.get_reference_number()
+        filmo_number = ififuncs.get_filmo_number()
         parent = ififuncs.ask_question('What is the parent record? eg MV 1234. Enter n/a if this is a born digital acquisition with no parent.')
         donor = ififuncs.ask_question('Who is the source of acquisition, as appears on the donor agreement? This will not affect Reproductions.')
         reproduction_creator = ififuncs.ask_question('Who is the reproduction creator? This will not affect acquisitions. Enter n/a if not applicable')
         depositor_reference = ififuncs.ask_question('What is the donor/depositor number? This will not affect Reproductions.')
         acquisition_type = ififuncs.get_acquisition_type('')
         donation_date = ififuncs.ask_question('When was the donation date in DD/MM/YYYY format? Eg. 31/12/1999 - Unfortunately this is NOT using ISO 8601.')
     if args.zip:
@@ -567,15 +579,15 @@
         package_update.main(supplement_cmd)
     if args.zip:
         os.makedirs(supplemental_dir)
         supplement_cmd = ['-i', [inputxml, inputtracexml, dfxml, source_manifest], '-user', user, '-new_folder', supplemental_dir, os.path.dirname(sip_path), '-copy']
         package_update.main(supplement_cmd)
     if args.sc:
         print('Generating Digital Forensics XML')
-        dfxml = accession.make_dfxml(args, sip_path, uuid)
+        dfxml = aipcreator.make_dfxml(args, sip_path, uuid)
         ififuncs.generate_log(
             new_log_textfile,
             'EVENT = Metadata extraction - eventDetail=File system metadata extraction using Digital Forensics XML, eventOutcome=%s, agentName=makedfxml' % (dfxml)
         )
         ififuncs.manifest_update(new_manifest_textfile, dfxml)
         sha512_log = manifest.main([sip_path, '-sha512', '-s'])
         sha512_manifest = os.path.join(
@@ -587,42 +599,47 @@
     ififuncs.sort_manifest(new_manifest_textfile)
     if not args.quiet:
         if 'log_names' in locals():
             log_report(log_names)
     finish = datetime.datetime.now()
     print('\n- %s ran this script at %s and it finished at %s' % (user, start, finish))
     if args.d:
-        process_dcp(sip_path, content_title, args, new_manifest_textfile, new_log_textfile, metadata_dir, clairmeta_version)
-    if args.accession:
-        register = accession.make_register()
+        # print clairmeta result to ifiscripts_log/$oe_clairmeta_outcome_$datetime.txt
+        desktop_logs_dir = ififuncs.make_desktop_logs_dir()
+        txt_name_filename = object_entry + "_clairmeta_outcome" + time.strftime("_%Y_%m_%dT%H_%M_%S")
+        txt_name_source = "%s/%s.txt" % (desktop_logs_dir, txt_name_filename)
+        ififuncs.generate_txt(txt_name_source, 'Target Directory: %s' % inputs)
+        process_dcp(sip_path, content_title, args, new_manifest_textfile, new_log_textfile, txt_name_source, metadata_dir, clairmeta_version)
+    if args.aipcreator:
+        register = aipcreator.make_register()
         filmographic_dict = ififuncs.extract_metadata(args.filmo_csv)[0]
         for filmographic_record in filmographic_dict:
-            if filmographic_record['Reference Number'].lower() == reference_number.lower():
-                if filmographic_record['Title'] == '':
-                    title = filmographic_record['TitleSeries'] + '; ' + filmographic_record['EpisodeNo']
+            if filmographic_record['Filmographic URN'].lower() == filmo_number.lower():
+                if filmographic_record['Title/Name'] == '':
+                    title = filmographic_record['Series Title'] + '; ' + filmographic_record['Episode No']
                 else:
-                    title = filmographic_record['Title']
+                    title = filmographic_record['Title/Name']
         oe_register = make_oe_register()
-        ififuncs.append_csv(oe_register, (object_entry.upper()[:2] + '-' + object_entry[2:], donation_date, '1','',title,donor,acquisition_type[1], accession_number, 'Representation of %s|Reproduction of %s' % (reference_number, parent), ''))
+        ififuncs.append_csv(oe_register, (object_entry.upper()[:2] + '-' + object_entry[2:], donation_date, '1','',title,donor,acquisition_type[1], accession_number, 'Representation of %s|Reproduction of %s' % (filmo_number, parent), ''))
         accession_cmd = [
             os.path.dirname(sip_path), '-user', user,
             '-force',
-            '-number', accession_number,
-            '-reference', reference_number,
+            '-accession_number', accession_number,
+            '-filmo_number', filmo_number,
             '-register', register,
             '-filmo_csv', args.filmo_csv,
             '-pbcore'
         ]
         if not parent.lower() == 'n/a':
             accession_cmd.extend(['-parent', parent])
         accession_cmd.extend(['-donor', donor])
         accession_cmd.extend(['-depositor_reference', depositor_reference])
         accession_cmd.extend(['-acquisition_type', acquisition_type[2]])
         accession_cmd.extend(['-donation_date', donation_date])
         accession_cmd.extend(['-reproduction_creator', reproduction_creator])
         print(accession_cmd)
-        accession.main(accession_cmd)
+        aipcreator.main(accession_cmd)
     return new_log_textfile, new_manifest_textfile
 
 
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.5.24.1/scripts/strongbox_fixity.py` & `ifiscripts-2023.6.30.1/scripts/strongbox_fixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/subfolders.py` & `ifiscripts-2023.6.30.1/scripts/subfolders.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/testfiles.py` & `ifiscripts-2023.6.30.1/scripts/testfiles.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/validate.py` & `ifiscripts-2023.6.30.1/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/scripts/walk_to_dfxml.py` & `ifiscripts-2023.6.30.1/scripts/walk_to_dfxml.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.5.24.1/setup.py` & `ifiscripts-2023.6.30.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 
 if sys.version_info < (3, 8):
     print("Python 3.8 or higher is required - earlier python 3 versions may work but were not tested.")
     sys.exit(1)
 setup(
     author='Kieran O\'Leary',
     author_email='kieran.o.leary@gmail.com',
+    maintainer='Yazhou He',
+    maintainer_email='yhe@irishfilm.ie',
     description="Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive",
     long_description=("""\
 Scripts for use in the IFI Irish Film Archive. Scripts have been tested in OSX/Windows 7/10 and Ubuntu 18.04. The aim is to make cross-platform scripts, but please get in touch with any issues. It is best to download all scripts, as some of them share code.
 
 Most scripts take either a file or a directory as their input, for example makeffv1.py filename.mov or premis.py path/to/folder_of_stuff. (It's best to just drag and drop the folder or filename into the terminal)
 
 Note: Documentation template has been copied from mediamicroservices
 
 NOTE: Objects.py has been copied from https://github.com/simsong/dfxml. walk_to_dfxml.py has also been copied but has been customised in order to add command line arguments for optionally turning off checksum generation. For more context, see https://github.com/simsong/dfxml/pull/28
 """),
     scripts=[
-        'scripts/Objects.py',
-        'scripts/accession.py',
         'scripts/accession_register.py',
+        'scripts/aipcreator.py',
         'scripts/as11fixity.py',
-        'scripts/batchaccession.py',
+        'scripts/batchaipcreator.py',
+        'scripts/batchdiff_framemd5.py',
         'scripts/batchmakeshell.py',
         'scripts/batchsipcreator.py',
         'scripts/bitc.py',
         'scripts/concat.py',
         'scripts/copyit.py',
         'scripts/dcpaccess.py',
         'scripts/dcpfixity.py',
@@ -48,14 +50,15 @@
         'scripts/makezip.py',
         'scripts/manifest.py',
         'scripts/masscopy.py',
         'scripts/massqc.py',
         'scripts/mergepbcore.py',
         'scripts/multicopy.py',
         'scripts/normalise.py',
+        'scripts/Objects.py',
         'scripts/order.py',
         'scripts/package_update.py',
         'scripts/packagecheck.py',
         'scripts/prores.py',
         'scripts/seq2ffv1.py',
         'scripts/sipcreator.py',
         'scripts/strongbox_fixity.py',
@@ -71,10 +74,10 @@
         'dicttoxml',
         'future',
         'clairmeta'
     ],
     data_files=[('', ['film_scan_aip_documentation.txt', '26_XYZ-22_Rec709.cube'])],
     include_package_data=True,
     name='ifiscripts',
-    version='2023.05.24.1',
+    version='2023.06.30.1',
     python_requires='>=3.8'
 )
```

