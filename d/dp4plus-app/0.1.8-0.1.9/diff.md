# Comparing `tmp/dp4plus_app-0.1.8.tar.gz` & `tmp/dp4plus_app-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp4plus_app-0.1.8.tar", last modified: Tue Jun 13 14:01:12 2023, max compression
+gzip compressed data, was "dp4plus_app-0.1.9.tar", last modified: Wed Jun 28 17:27:58 2023, max compression
```

## Comparing `dp4plus_app-0.1.8.tar` & `dp4plus_app-0.1.9.tar`

### file list

```diff
@@ -1,146 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:12.228048 dp4plus_app-0.1.8/
--rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.8/LICENCE
--rw-rw-rw-   0        0        0     7497 2023-06-13 14:01:12.228048 dp4plus_app-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6903 2023-06-13 13:58:55.000000 dp4plus_app-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 14:01:12.228048 dp4plus_app-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1990 2023-06-13 13:59:20.000000 dp4plus_app-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.009713 dp4plus_app-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.447221 dp4plus_app-0.1.8/src/dp4plus_app/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.650350 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/
--rw-rw-rw-   0        0        0  1983578 2023-06-05 16:41:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.docx
--rw-rw-rw-   0        0        0  2040794 2023-06-05 16:42:18.000000 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.pdf
--rw-rw-rw-   0        0        0   765044 2023-05-31 15:25:45.000000 dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
--rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.8/src/dp4plus_app/__init__.py
--rw-rw-rw-   0        0        0     9508 2023-06-02 17:21:15.000000 dp4plus_app-0.1.8/src/dp4plus_app/bugs_a_warning_module.py
--rw-rw-rw-   0        0        0     9896 2023-06-07 19:08:21.000000 dp4plus_app-0.1.8/src/dp4plus_app/correlation_module.py
--rw-rw-rw-   0        0        0    19040 2023-06-02 19:18:30.000000 dp4plus_app-0.1.8/src/dp4plus_app/custom_gui_module.py
--rw-rw-rw-   0        0        0     8702 2023-06-02 17:39:19.000000 dp4plus_app-0.1.8/src/dp4plus_app/custom_module.py
--rw-rw-rw-   0        0        0    13608 2023-06-01 17:06:25.000000 dp4plus_app-0.1.8/src/dp4plus_app/data_base_Custom.xlsx
--rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/data_base_MM.xlsx
--rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.8/src/dp4plus_app/data_base_QM.xlsx
--rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/dp4_module.py
--rw-rw-rw-   0        0        0    73188 2023-03-07 17:33:34.000000 dp4plus_app-0.1.8/src/dp4plus_app/logo_CONICET.png
--rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.8/src/dp4plus_app/logo_INGEBIO.png
--rw-rw-rw-   0        0        0     3710 2023-05-31 18:15:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/main.py
--rw-rw-rw-   0        0        0    19424 2023-06-02 19:17:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/main_gui_module.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.712852 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/
--rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
--rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:10.009734 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/
--rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
--rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
--rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
--rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:10.400369 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/
--rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
--rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
--rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
--rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:12.212422 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/
--rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a - copia.xlsx
--rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    10836 2023-06-01 16:54:02.000000 dp4plus_app-0.1.8/src/dp4plus_app/output_module.py
--rw-rw-rw-   0        0        0     5375 2023-06-02 17:47:02.000000 dp4plus_app-0.1.8/src/dp4plus_app/validation_module.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:01:09.494098 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/
--rw-rw-rw-   0        0        0     7497 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7047 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 14:01:08.000000 dp4plus_app-0.1.8/src/dp4plus_app.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:58.368435 dp4plus_app-0.1.9/
+-rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.9/LICENCE
+-rw-rw-rw-   0        0        0     7497 2023-06-28 17:27:58.354033 dp4plus_app-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6903 2023-06-13 13:58:55.000000 dp4plus_app-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-28 17:27:58.368435 dp4plus_app-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2021 2023-06-28 15:22:12.000000 dp4plus_app-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.111525 dp4plus_app-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.397643 dp4plus_app-0.1.9/src/dp4plus_app/
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.592498 dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/
+-rw-rw-rw-   0        0        0  1983578 2023-06-05 16:41:59.000000 dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/UserGuide.docx
+-rw-rw-rw-   0        0        0  2040794 2023-06-05 16:42:18.000000 dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/UserGuide.pdf
+-rw-rw-rw-   0        0        0   765044 2023-05-31 15:25:45.000000 dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
+-rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.9/src/dp4plus_app/__init__.py
+-rw-rw-rw-   0        0        0     9508 2023-06-02 17:21:15.000000 dp4plus_app-0.1.9/src/dp4plus_app/bugs_a_warning_module.py
+-rw-rw-rw-   0        0        0     9896 2023-06-07 19:08:21.000000 dp4plus_app-0.1.9/src/dp4plus_app/correlation_module.py
+-rw-rw-rw-   0        0        0    19065 2023-06-28 17:26:42.000000 dp4plus_app-0.1.9/src/dp4plus_app/custom_gui_module.py
+-rw-rw-rw-   0        0        0     8774 2023-06-28 17:11:40.000000 dp4plus_app-0.1.9/src/dp4plus_app/custom_module.py
+-rw-rw-rw-   0        0        0    15931 2023-06-28 17:26:01.000000 dp4plus_app-0.1.9/src/dp4plus_app/data_base_Custom.xlsx
+-rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.9/src/dp4plus_app/data_base_MM.xlsx
+-rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.9/src/dp4plus_app/data_base_QM.xlsx
+-rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.9/src/dp4plus_app/dp4_module.py
+-rw-rw-rw-   0        0        0    49515 2023-06-28 16:54:34.000000 dp4plus_app-0.1.9/src/dp4plus_app/logo_CONICET.png
+-rw-rw-rw-   0        0        0    44371 2023-06-28 16:35:01.000000 dp4plus_app-0.1.9/src/dp4plus_app/logo_DP4app.png
+-rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.9/src/dp4plus_app/logo_INGEBIO.png
+-rw-rw-rw-   0        0        0     4534 2023-06-28 17:24:36.000000 dp4plus_app-0.1.9/src/dp4plus_app/main.py
+-rw-rw-rw-   0        0        0    19029 2023-06-28 17:08:45.000000 dp4plus_app-0.1.9/src/dp4plus_app/main_gui_module.py
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.712626 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/
+-rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
+-rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.817577 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/
+-rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
+-rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
+-rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
+-rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.902568 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/
+-rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
+-rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
+-rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
+-rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:58.354033 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/
+-rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a - copia.xlsx
+-rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    10912 2023-06-28 17:08:03.000000 dp4plus_app-0.1.9/src/dp4plus_app/output_module.py
+-rw-rw-rw-   0        0        0     5375 2023-06-02 17:47:02.000000 dp4plus_app-0.1.9/src/dp4plus_app/validation_module.py
+drwxrwxrwx   0        0        0        0 2023-06-28 17:27:55.477723 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/
+-rw-rw-rw-   0        0        0     7497 2023-06-28 17:27:54.000000 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7079 2023-06-28 17:27:54.000000 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-28 17:27:54.000000 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-06-28 17:27:54.000000 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      132 2023-06-28 17:27:54.000000 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-28 17:27:54.000000 dp4plus_app-0.1.9/src/dp4plus_app.egg-info/top_level.txt
```

### Comparing `dp4plus_app-0.1.8/LICENCE` & `dp4plus_app-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/PKG-INFO` & `dp4plus_app-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp4plus_app
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to simplify your DP4+ calculations
 Home-page: https://github.com/RosarioCCLab/DP4plus-App
 Author: Bruno A. Franco
 Author-email: bruno.agustin.franco@gmail.com
 License: MIT
 Keywords: nmr
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dp4plus_app-0.1.8/README.md` & `dp4plus_app-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/setup.py` & `dp4plus_app-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md') as file:         #sirve para incluir el REEDME
     long_description = file.read()
 
 short_description = 'A tool to simplify your DP4+ calculations'
 
 setup(
     name='dp4plus_app',
-    version='0.1.8',
+    version='0.1.9',
     
     author='Bruno A. Franco',
     author_email='bruno.agustin.franco@gmail.com',
     url='https://github.com/RosarioCCLab/DP4plus-App',
     description =short_description	,
     long_description = long_description,
     long_description_content_type ="text/markdown",
@@ -38,14 +38,15 @@
                     'openpyxl', 
                     'xlsxwriter',
                     'pandas',
                     'pathlib', 
                     'scikit-learn', 
                     'scipy', 
                     'tk',
+                    'Pillow',
                     'odfpy'],
     
     entry_points={ 'gui_scripts': ['dp4plus = dp4plus_app.main:main'],
                     'console_scripts':['dp4plus-exe = dp4plus_app.main:create_exe'],},
                  
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.docx` & `dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/UserGuide.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuide.pdf` & `dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/UserGuide.pdf`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/UserGuide/UserGuideFigures.pptx` & `dp4plus_app-0.1.9/src/dp4plus_app/UserGuide/UserGuideFigures.pptx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/bugs_a_warning_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/bugs_a_warning_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/correlation_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/correlation_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/custom_gui_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/custom_gui_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 
 def custom_input ():
     ''' Main function of the application
     Contains the settings of the application widgets
     '''
     global custom_app
-    custom_app = tk.Tk()
+    custom_app = tk.Toplevel()
     custom_app.wm_title("Custom: New Level")
-    custom_app.geometry("600x300") #(width x height)
+    custom_app.geometry("650x350") #(width x height)
 
     #-----------------------------------------------------------------
     label = tk.Label(custom_app, 
                      text='Reparametrization module')
     label.config(font = ("Arial Bold", "14"))
     label.grid(row=0,column=0,columnspan=2,sticky='W', padx=10)
     custom_app.columnconfigure(1, pad = 20)
@@ -61,15 +61,15 @@
     TMS_frame = tk.Frame(custom_app)
 
     #-----------------------------------------------------------------
     #"Load" widgets (wg)
     global files_frame
     files_frame = tk.Frame(custom_app)
     
-    custom_app.mainloop()
+    custom_app.wait_window()
     
     if 'Input' in mode_list.get():
         return {'mode': mode,
                 'name': name, 
                 'C_TMS': C_TMS, 
                 'H_TMS': H_TMS, 
                 'param': table }
@@ -167,15 +167,15 @@
             
     return
 
 def download(): 
     '''Configuration and applications, from the download window to 
     parameterize with G09 calculations
     '''
-    down_add = tk.Tk()
+    down_add = tk.Toplevel()
     down_add.wm_title("DP4+ App")
     
     tk.Label (down_add, text = 'Optimization Theory Level: ').grid(row=0,column=0,
                                                           pady=10, sticky='we',
                                                           columnspan=2)
     
     down_selec = tk.StringVar(down_add,'')
@@ -242,15 +242,15 @@
         shutil.copy((Path(__file__).parent / "nmr_custom"/'custom_molecules_set.docx').as_posix(), 
                     dst_folder)
         shutil.copy((Path(__file__).parent / "nmr_custom"/'Data_traning_set.xlsx').as_posix(), 
                     dst_folder)
         
         custom_app.destroy()
 
-        examp_add = tk.Tk()
+        examp_add = tk.Toplevel()
         examp_add.wm_title("DP4+ App")
         tk.Label(examp_add,text = u' Folder Copy \u2713', 
                  font = ("Arial Black", "12")).grid(row=0)
         tk.Label(examp_add,text ='"nmr_custom" has been created in your desktop', 
                  font = ("Arial Bold", "10")).grid(row=1, pady=10)
         tk.Label(examp_add,text ='The program will restarts. Follow the user guide instructions to process the data', 
                  font = ("Arial Bold", "10")).grid(row=2, padx=10)
@@ -258,15 +258,15 @@
                   command= exit).grid(row=3, pady=5 )
         return
         
     tk.Button(down_add, text=u'Download files \u21E9 ',
               command= copy_and_exit).grid(row=4, column = 0, pady = (5,10), columnspan=2)
     down_add.rowconfigure(5, minsize=30)
 
-    down_add.mainloop()
+    down_add.wait_window()
     return
 
 def select_xlsx():
     '''Select xlsx file with experimental data and asignation labels. 
     '''    
     custom_app.xlsx = filedialog.askopenfilename(title='Select Excel',
                                    filetypes=[('Excel files','*.xlsx'),
@@ -445,15 +445,15 @@
         mode = mode_list.get()
         name = name_entry.get()
 
         #close widget    
         l_end['text'] = 'Processing . . .'
         button_final['state'] = 'disable'
     
-        custom_app.after(1000, custom_app.quit())
+        custom_app.after(1000, custom_app.destroy)
 
         return 
     #----------------------------------------------------------------     
     def change_name(): 
         warn_add.destroy()
         l_end['text'] = 'Choose other name'
         return
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/custom_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/custom_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     
     param.loc['Csp2'] = st.t.fit(e_vectors['Csp2'])
     param.loc['Csp3'] = st.t.fit(e_vectors['Csp3'])
     
     param.loc['Hsp2'] = st.t.fit(e_vectors['Hsp2'])
     param.loc['Hsp3'] = st.t.fit(e_vectors['Hsp3']) 
     
+    param.loc['Csca','m'] = 0.0
+    param.loc['Hsca','m'] = 0.0
+    
     return param
 
 def get_command():
     '''saves the command line of 10% of the files used in the 
     parameterization
     '''    
     files = []
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/data_base_Custom.xlsx` & `dp4plus_app-0.1.9/src/dp4plus_app/data_base_Custom.xlsx`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-00000000: 504b 0304 1400 0600 0800 0000 2100 bac4  PK..........!...
-00000010: 8506 7901 0000 9805 0000 1300 0802 5b43  ..y...........[C
+00000000: 504b 0304 1400 0600 0800 0000 2100 8756  PK..........!..V
+00000010: e132 8601 0000 9906 0000 1300 0802 5b43  .2............[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
 00000030: 6c20 a204 0228 a000 0200 0000 0000 0000  l ...(..........
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -29,42 +29,42 @@
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 00ac 94cb 6ec2 3010  ............n.0.
-00000240: 45f7 95fa 0f91 b755 6260 5155 1581 451f  E......Ub`QU..E.
-00000250: cb16 a954 ead6 8d07 62e1 973c 0385 bfaf  ...T....b..<....
-00000260: 631e aaaa 148a c226 56e2 997b cf8c e319  c......&V..{....
-00000270: 8ed7 4667 2b08 a89c 2d59 bfe8 b10c 6ce5  ..Fg+...-Y....l.
-00000280: a4b2 f392 bd4f 9ff3 3b96 2109 2b85 7616  .....O..;.!.+.v.
-00000290: 4ab6 0164 e3d1 f5d5 70ba f180 59cc b658  J..d....p...Y..X
-000002a0: b29a c8df 738e 550d 4660 e13c d8b8 3373  ....s.U.F`.<..3s
-000002b0: c108 8aaf 61ce bda8 1662 0e7c d0eb ddf2  ....a....b.|....
-000002c0: ca59 024b 3935 1a6c 347c 8499 586a ca9e  .Y.K95.l4|..Xj..
-000002d0: d6f1 f396 2480 4696 3d6c 031b af92 09ef  ....$.F.=l......
-000002e0: b5aa 0445 52be b2f2 974b be73 2862 668a  ...ER....K.s(bf.
-000002f0: c15a 79bc 8918 8cb7 3a34 3b7f 1bec f25e  .Zy.....:4;....^
-00000300: 636b 8292 904d 44a0 1761 2206 5f6b fee5  ck...MD..a"._k..
-00000310: c2e2 d3b9 4571 5ca4 85d2 cd66 aa02 e9aa  ....Eq\....f....
-00000320: a589 1d28 d007 1012 6b00 32ba 486b 6184  ...(....k.2.Hka.
-00000330: b27b ee23 fe29 1879 5afa 1706 69ea 4bc2  .{.#.).yZ...i.K.
-00000340: 2738 289e 37f0 f4ec 8e90 644e 1822 6d34  '8(.7.....dN."m4
-00000350: e0a5 db9e 444f 39d7 2280 7ca3 106f c6c5  ....DO9.".|..o..
-00000360: 017e 6a1f e3a8 9648 ce7c 18cd 1581 9904  .~j....H.|......
-00000370: e7b1 7bdf 0fa2 8d1e 0452 70b8 366d bf5f  ..{......Rp.6m._
-00000380: 0bc3 a0f3 819c c910 ef4f 2a3e 4e92 00e7  .........O*>N...
-00000390: 9bef 4745 939d fb7f 557d 708c 53a8 73b5  ..GE....U}p.S.s.
-000003a0: d0cc 3909 b2c5 9ba7 b93a fa06 0000 ffff  ..9......:......
-000003b0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000003c0: b555 3023 f400 0000 4c02 0000 0b00 0802  .U0#....L.......
-000003d0: 5f72 656c 732f 2e72 656c 7320 a204 0228  _rels/.rels ...(
-000003e0: a000 0200 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 00bc 954d 4b03 3110  ...........MK.1.
+00000240: 86ef 82ff 61c9 55ba 692b 8848 b73d f871  ....a.U.i+.H.=.q
+00000250: d482 15bc c6cd b41b 9a2f 32d3 dafe 7bb3  ........./2...{.
+00000260: e907 226b 6bd9 e265 c36e 32ef fb64 6633  .."kk..e.n2..df3
+00000270: 198c 5646 674b 08a8 9c2d 582f efb2 0c6c  ..VFgK...-X/...l
+00000280: e9a4 b2b3 82bd 4d9e 3ab7 2c43 1256 0aed  ......M.:.,C.V..
+00000290: 2c14 6c0d c846 c3cb 8bc1 64ed 01b3 186d  ,.l..F....d....m
+000002a0: b160 1591 bfe3 1ccb 0a8c c0dc 79b0 7166  .`..........y.qf
+000002b0: ea82 1114 5fc3 8c7b 51ce c50c 78bf dbbd  ...._..{Q...x...
+000002c0: e1a5 b304 963a 546b b0e1 e001 a662 a129  .....:Tk.....b.)
+000002d0: 7b5c c5cf 1b92 001a 5976 bf59 587b 154c  {\......Yv.YX{.L
+000002e0: 78af 5529 2892 f2a5 953f 5c3a 5b87 3c46  x.U)(....?\:[.<F
+000002f0: a635 5829 8f57 1183 f146 877a e677 836d  .5X).W...F.z.w.m
+00000300: dc4b 4c4d 5012 b2b1 08f4 2c4c c4e0 2bcd  .KLMP.....,L..+.
+00000310: 3f5d 987f 3837 cf0f 8b34 50ba e954 9520  ?]..87...4P..T. 
+00000320: 5db9 3031 0339 fa00 4262 0540 46e7 69cc  ].01.9..Bb.@F.i.
+00000330: 8d50 76c7 7dc0 3f2d 469e 86de 9941 eafd  .Pv.}.?-F....A..
+00000340: 25e1 231c 14eb 0d3c 3ddb 2324 9923 8648  %.#....<=.#$.#.H
+00000350: 6b0d 78ee b427 d163 ce95 0820 5f29 c493  k.x..'.c... _)..
+00000360: 7176 80ef da87 38ca 0592 33ef 4673 4560  qv....8...3.FsE`
+00000370: c6c1 796c 9ff7 bd68 ad07 8114 ec8f 4dd3  ..yl...h......M.
+00000380: efd7 c0d0 6f5d 90f6 0cd7 ffcd 10cf 702a  ....o]........p*
+00000390: 40ec 6601 4e37 dfb5 ab3a bae3 ff94 f9bd  @.f.N7...:......
+000003a0: 63ec 84ad 770b 75af 9520 4ff5 de54 ea4c  c...w.u.. O..T.L
+000003b0: c96e 30e7 e962 197e 0100 00ff ff03 0050  .n0..b.~.......P
+000003c0: 4b03 0414 0006 0008 0000 0021 0013 5ebe  K..........!..^.
+000003d0: 6502 0100 00df 0200 000b 0008 025f 7265  e............_re
+000003e0: 6c73 2f2e 7265 6c73 20a2 0402 28a0 0002  ls/.rels ...(...
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -88,764 +88,909 @@
 00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005e0: 0000 00ac 924d 4fc3 300c 86ef 48fc 87c8  .....MO.0...H...
-000005f0: f7d5 dd90 1042 4b77 4148 bb21 547e 8049  .....BKwAH.!T~.I
-00000600: dc0f b58d a324 1bdd bf27 1c10 541a 8303  .....$...'..T...
-00000610: 477f bd7e fcca dbdd 3c8d eac8 21f6 e234  G..~....<...!..4
-00000620: ac8b 1214 3b23 b677 ad86 97fa 7175 072a  ....;#.w....qu.*
-00000630: 2672 9646 71ac e1c4 1176 d5f5 d5f6 9947  &r.Fq....v.....G
-00000640: 4a79 2876 bd8f 2aab b8a8 a14b c9df 2346  Jy(v..*....K..#F
-00000650: d3f1 44b1 10cf 2e57 1a09 13a5 1c86 163d  ..D....W.......=
-00000660: 9981 5ac6 4d59 de62 f8ae 01d5 4253 edad  ..Z.MY.b....BS..
-00000670: 86b0 b737 a0ea 93cf 9b7f d796 a6e9 0d3f  ...7...........?
-00000680: 8839 4cec d299 15c8 7362 67d9 ae7c c86c  .9L.....sbg..|.l
-00000690: 21f5 f91a 5553 6839 69b0 629e 723a 2279  !...USh9i.b.r:"y
-000006a0: 5f64 6cc0 f344 9bbf 13fd 7c2d 4e9c c852  _dl..D....|-N..R
-000006b0: 2234 12f8 32cf 47c7 25a0 f57f 5ab4 34f1  "4..2.G.%...Z.4.
-000006c0: cb9d 79c4 3709 c3ab c8f0 c982 8b1f a8de  ..y.7...........
-000006d0: 0100 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000006e0: 0000 0021 009e 81d4 5011 0100 00d6 0300  ...!....P.......
-000006f0: 001a 0008 0178 6c2f 5f72 656c 732f 776f  .....xl/_rels/wo
-00000700: 726b 626f 6f6b 2e78 6d6c 2e72 656c 7320  rkbook.xml.rels 
-00000710: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
-00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: ac92 4d4b 0331 1086 ef82 ff21 ccbd 3bdb  ..MK.1.....!..;.
+00000600: 2a22 d26c 2f45 e84d 64fd 0131 99fd 6037  *".l/E.Md..1..`7
+00000610: 9990 a4ba fdf7 4641 74a1 b61e 7a9c af77  ......FAt...z..w
+00000620: 9e79 99f5 66b2 a378 a310 7b76 1296 4509  .y..f..x..{v..E.
+00000630: 829c 66d3 bb56 c24b fdb8 b807 1193 7246  ..f..V.K......rF
+00000640: 8dec 48c2 8122 6caa ebab f533 8d2a e5a1  ..H.."l....3.*..
+00000650: d8f5 3e8a ace2 a284 2e25 ff80 1875 4756  ..>......%...uGV
+00000660: c582 3db9 5c69 3858 9572 185a f44a 0faa  ..=.\i8X.r.Z.J..
+00000670: 255c 95e5 1d86 df1a 50cd 34c5 ce48 083b  %\......P.4..H.;
+00000680: 7303 a23e f8bc f9bc 3637 4daf 69cb 7a6f  s..>....67M.i.zo
+00000690: c9a5 232b 90a6 44ce 9059 f890 d942 eaf3  ..#+..D..Y...B..
+000006a0: 35a2 56a1 a524 c1b0 7eca e988 cafb 2263  5.V..$..~....."c
+000006b0: 031e 275a fd9f e8ef 6bd1 5252 4625 859a  ..'Z....k.RRF%..
+000006c0: 039d e6f9 ec38 05b4 bca4 4573 137f dc99  .....8....Es....
+000006d0: 467c e730 bc32 0fa7 586e 2fc9 a2f7 31b1  F|.0.2..Xn/...1.
+000006e0: 3d63 ce57 cf37 12ce deb2 fa00 0000 ffff  =c.W.7..........
+000006f0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00000700: dfa4 6728 1a01 0000 6404 0000 1a00 0801  ..g(....d.......
+00000710: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
+00000720: 6b2e 786d 6c2e 7265 6c73 20a2 0401 28a0  k.xml.rels ...(.
+00000730: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000810: 0000 0000 0000 00bc 534d 4bc4 3010 bd0b  ........SMK.0...
-00000820: fe87 3077 9bb6 ea22 b2e9 5e44 d8ab 56f0  ..0w..."..^D..V.
-00000830: 1ada e907 db24 2533 abf6 df1b 2a76 bbb0  .....$%3....*v..
-00000840: d44b f112 9837 e4bd 9797 99ed eecb 74e2  .K...7........t.
-00000850: 033d b5ce 2a48 a218 04da c295 adad 15bc  .=..*H..........
-00000860: e5cf 370f 2088 b52d 75e7 2c2a 1890 6097  ..7. ..-u.,*..`.
-00000870: 5d5f 6d5f b0d3 1c2e 51d3 f624 028b 2505  ]_m_....Q..$..%.
-00000880: 0d73 ff28 2515 0d1a 4d91 ebd1 864e e5bc  .s.(%...M....N..
-00000890: d11c 4a5f cb5e 1707 5da3 4ce3 7823 fd9c  ..J_.^..].L.x#..
-000008a0: 03b2 334e b12f 15f8 7d79 0b22 1ffa a0fc  ..3N./..}y."....
-000008b0: 37b7 abaa b6c0 2757 1c0d 5abe 2021 8987  7.....'W..Z. !..
-000008c0: 2e3c 40e4 dad7 c80a 7eea 2878 0479 593e  .<@.....~.(x.yY>
-000008d0: 5d53 9e43 2c78 521f 4b39 9ec9 9287 644d  ]S.C,xR.K9....dM
-000008e0: 0f9f ce1f a841 e493 8f09 2239 7616 cd6c  .....A...."9v..l
-000008f0: d634 531c 899d 790f f14f 5f12 4572 4265  .4S...y..O_.ErBe
-00000900: cb68 d2a5 68ee ffdb cd62 3677 abce 6aa3  .h..h....b6w..j.
-00000910: 3d96 afec c32a ce47 760e ff46 23cf b631  =....*.Gv..F#..1
-00000920: fb06 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00000930: 0800 0000 2100 e619 1dd3 2302 0000 4104  ....!.....#...A.
-00000940: 0000 0f00 0000 786c 2f77 6f72 6b62 6f6f  ......xl/workboo
-00000950: 6b2e 786d 6ca4 53cb 6edb 3010 bc17 e83f  k.xml.S.n.0....?
-00000960: 10bc 1631 2dd7 111a c372 e038 7d04 480b  ...1-....r.8}.H.
-00000970: 234d 9363 b126 d716 11be 4a52 b5f3 f75d  #M.c.&....JR...]
-00000980: 4955 9a34 9714 bd88 bbe4 6ac8 9d99 9d9f  IU.4......j.....
-00000990: 1eac 613f 3126 ed5d c58b d198 3374 d22b  ..a?1&.]....3t.+
-000009a0: ed76 15ff 76fd e1e8 1d67 2983 5360 bcc3  .v..v....g).S`..
-000009b0: 8adf 63e2 a78b d7af e67b 1fef 36de df31  ..c......{..6..1
-000009c0: 0270 a9e2 75ce 6126 4492 355a 4823 1fd0  .p..u.a&D.5ZH#..
-000009d0: d1c9 d647 0b99 d2b8 1329 4404 956a c46c  ...G.....)D..j.l
-000009e0: 8d98 8cc7 a5b0 a01d ef11 66f1 2518 7ebb  ..........f.%.~.
-000009f0: d512 cfbd 6c2c badc 8344 3490 e9f9 a9d6  ....l,...D4.....
-00000a00: 210d 6856 be04 ce42 bc6b c291 f436 10c4  !.hV...B.k...6..
-00000a10: 461b 9def 3b50 ceac 9c5d ec9c 8fb0 31d4  F...;P...]....1.
-00000a20: f6a1 381e 9029 7c06 6db5 8c3e f96d 1e11  ..8..)|.m..>.m..
-00000a30: 94e8 1ff9 acdf 622c 8aa2 6f79 31df 6a83  ......b,..oy1.j.
-00000a40: 373d ed0c 42f8 02b6 bdc5 7066 20e5 f74a  7=..B.....pf ..J
-00000a50: 6754 152f 29f5 7b7c b211 9b70 d668 43a7  gT./).{|...p.hC.
-00000a60: c574 3a19 73b1 7890 621d 99c2 2d34 265f  .t:.s.x.b...-4&_
-00000a70: 9308 033c 154e a693 49d9 5652 534b 9331  ...<.N..I.VRSK.1
-00000a80: 3ac8 b8f2 2e13 87bf d9ff 5fbe 3aec 55ed  :........._.:.U.
-00000a90: 491d 7685 3f1a 1d91 4cd1 d2b6 98d3 17e4  I.v.?...L.......
-00000aa0: 0c36 690d b966 4d34 3d7f 89ec d248 f06f  .6i..fM4=....H.o
-00000ab0: cbe3 51aa 2162 f0da f50c 26ea 3f89 ab33  ..Q.!b....&.?..3
-00000ac0: ed57 ab4b d888 4170 9f58 a755 cc5a f924  .W.K..Ap.X.U.Z.$
-00000ad0: 3ea2 c308 469c afa7 6fd8 3204 b13c fa4a  >...F...o.2..<.J
-00000ae0: 22ec 094b a830 0da6 49df 895c 91a2 7c92  "..K.0..I..\..|.
-00000af0: 3f92 129e fbe4 1fc4 04d9 b22a 88d6 bef5  ?..........*....
-00000b00: 3efe 9be2 c5bc 1d94 1b8d fbf4 47ac 3665  >...........G.6e
-00000b10: 875b ed94 df57 7c32 a5c1 bb1f b2d6 6cfb  .[...W|2......l.
-00000b20: eee4 56ab 5c93 82e5 f8e4 61ef 13ea 5d9d  ..V.\.....a...].
-00000b30: 2b7e 5296 9dfc e211 7a37 5d74 4bb7 32d7  +~R.....z7]tK.2.
-00000b40: b9aa 1fdf a868 90db d9bb 68ad c359 9c69  .....h....h..Y.i
-00000b50: 0ae2 852a ba16 861f 2518 493e 6a97 b690  ...*....%.I>j...
-00000b60: 5ed5 869f bd22 7b5a 700d 98ae 7c98 fec5  ^...."{Zp...|...
-00000b70: 2f00 0000 ffff 0300 504b 0304 1400 0600  /.......PK......
-00000b80: 0800 0000 2100 9c63 914c aa00 0000 ea00  ....!..c.L......
-00000b90: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
-00000ba0: 7472 696e 6773 2e78 6d6c 5cce c10a c230  trings.xml\....0
-00000bb0: 0cc6 f1bb e03b 94dc 5da7 8888 b4dd 6122  .....;..].....a"
-00000bc0: 5ebc e903 942d 6e85 359d 4b26 faf6 4e44  ^....-n.5.K&..ND
-00000bd0: 108f ff5f f820 a678 c44e dd71 e090 c8c2  ..._. .x.N.q....
-00000be0: 32cb 4121 55a9 0ed4 58b8 9c0f 8b2d 2816  2.A!U...X....-(.
-00000bf0: 4fb5 ef12 a185 2732 146e 3e33 cca2 a62d  O.....'2.n>3...-
-00000c00: b185 56a4 df69 cd55 8bd1 7396 7aa4 e972  ..V..i.U..s.z..r
-00000c10: 4d43 f432 e5d0 68ee 07f4 35b7 8812 3bbd  MC.2..h...5...;.
-00000c20: caf3 8d8e 3e10 a82a 8d24 16d6 a046 0ab7  ....>..*.$...F..
-00000c30: 11cb 6f3b c3c1 1971 a5d1 e28c 7ec7 078e  ..o;...q....~...
-00000c40: ffb0 f782 ff76 4af5 8fe9 e957 f702 0000  .....vJ....W....
-00000c50: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00000c60: 2100 1ae8 a8b7 9106 0000 e51b 0000 1300  !...............
-00000c70: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
-00000c80: 312e 786d 6cec 59cd 6e1b 3710 be17 e83b  1.xml.Y.n.7....;
-00000c90: 107b 4f2c d992 6319 9103 4b96 e236 7162  .{O,..c...K..6qb
-00000ca0: d84a 8a1c a915 b5cb 98bb 5c90 941d dd8a  .J........\.....
-00000cb0: e458 a040 d1b4 e8a5 406f 3d14 6d03 2440  .X.@....@o=.m.$@
-00000cc0: 2fe9 d3b8 4dd1 a640 5ea1 4372 2591 1615  /...M..@^.Cr%...
-00000cd0: db89 81fe c506 6c89 fb71 6638 3f1f 87dc  ......l..qf8?...
-00000ce0: abd7 1e64 0c1d 1221 29cf 9b51 f572 2542  ...d...!)..Q.r%B
-00000cf0: 248f f980 e649 33ba d3eb 5e5a 8b90 5438  $....I3...^Z..T8
-00000d00: 1f60 c673 d28c c644 46d7 36de 7fef 2a5e  .`.s...DF.6...*^
-00000d10: 5729 c908 82f9 b95c c7cd 2855 aa58 5f5a  W).....\..(U.X_Z
-00000d20: 9231 0c63 7999 1724 8767 432e 32ac e0ab  .1.cy..$.gC.2...
-00000d30: 4896 0602 1f81 dc8c 2d2d 572a ab4b 19a6  H.......--W*.K..
-00000d40: 7984 729c 81d8 1ecc 4103 826e 0f87 3426  y.r.....A..n..4&
-00000d50: d1c6 447c 8781 8e5c 493d 1033 b1af 8593  ..D|...\I=.3....
-00000d60: 728e 831d 1c54 3542 8e65 9b09 7488 5933  r....T5B.e..t.Y3
-00000d70: 024d 037e d423 0f54 8418 960a 1e34 a38a  .M.~.#.T.....4..
-00000d80: f989 9636 ae2e e1f5 7212 530b e63a f3ba  ...6....r.S..:..
-00000d90: e6a7 9c57 4e18 1c2c 1b9d 22e9 4f95 56bb  ...WN..,..".O.V.
-00000da0: b5c6 95ad a97c 0360 6a1e d7e9 74da 9dea  .....|.`j...t...
-00000db0: 549e 01e0 3886 955a 5b5c 99b5 ee5a b535  T...8..Z[\...Z.5
-00000dc0: 91e9 80ec c779 d9ed 4abd 52f3 f18e fc95  .....y..J.R.....
-00000dd0: 399b 1bad 56ab de28 6db1 420d c87e accd  9...V..(m.B..~..
-00000de0: e1d7 2aab b5cd 650f 6f40 165f 9fc3 d75a  ..*...e.o@._...Z
-00000df0: 9bed f6aa 8737 208b 5f9d c377 af34 566b  .....7 ._..w.4Vk
-00000e00: 3ede 8052 46f3 8339 b40e 68b7 5b4a 9f42  >..RF..9..h.[J.B
-00000e10: 869c 6d07 e16b 005f ab94 f019 0ab2 619a  ..m..k._......a.
-00000e20: 5d5a c590 e76a 51ae 65f8 3e17 5d00 6820  ]Z...jQ.e.>.].h 
-00000e30: c38a e648 8d0b 32c4 31e4 711b 677d 4171  ...H..2.1.q.g}Aq
-00000e40: 840a 9c73 0903 95e5 4ab7 b202 7ff5 6fcd  ...s....J.....o.
-00000e50: 7caa 69f5 789d 6067 9e1d 8ae5 dc90 b604  |.i.x.`g........
-00000e60: c958 d042 35a3 0f41 6ae4 405e 3dff fed5  .X.B5..Aj.@^=...
-00000e70: f3a7 e8d5 f327 c70f 9f1d 3ffc e9f8 d1a3  .....'....?.....
-00000e80: e387 3f5a 59de c46d 9c27 eec4 97df 7ef6  ..?ZY..m.'....~.
-00000e90: e7d7 1fa3 3f9e 7ef3 f2f1 1761 bc74 f1bf  ....?.~....a.t..
-00000ea0: fef0 c92f 3f7f 1e06 427d cdd6 ffe2 cb27  .../?...B}.....'
-00000eb0: bf3d 7bf2 e2ab 4f7f ffee 7100 be29 70df  .={...O...q..)p.
-00000ec0: 85f7 6846 24ba 458e d01e cf60 6dc6 31be  ..hF$.E....`m.1.
-00000ed0: e5a4 2fce 37a3 9762 eacd c029 c80e 88ee  ../.7..b...)....
-00000ee0: a8d4 03de 1a63 16c2 b588 efbc bb02 a825  .....c.........%
-00000ef0: 04bc 3eba efd9 ba9f 8a91 a201 cd37 d2cc  ..>..........7..
-00000f00: 03ee 70ce 5a5c 041d 7043 eb72 3cdc 1be5  ..p.Z\..pC.r<...
-00000f10: 4958 b918 b9b8 3d8c 0f43 badb 38f7 42db  IX....=..C..8.B.
-00000f20: 1915 c0a9 90b2 f3be 6fa7 c433 7397 e15c  ........o..3s..\
-00000f30: e184 e444 21fd 8c1f 1012 9876 8f52 cfaf  ...D!......v.R..
-00000f40: 3b34 165c f2a1 42f7 286a 611a 7449 8ff6  ;4.\..B.(ja.tI..
-00000f50: bd44 9a4d daa6 19c4 651c 3210 42ed f966  .D.M....e.2.B..f
-00000f60: e72e 6a71 165a f516 39f4 9150 1098 058c  ..jq.Z..9..P....
-00000f70: ef11 e6b9 f13a 1e29 9c85 44f6 70c6 5c87  .....:.)..D.p.\.
-00000f80: dfc4 2a0d 19b9 3f16 b18b eb48 0591 4e08  ..*...?....H..N.
-00000f90: e3a8 3320 5286 e6dc 16b0 5e27 e837 30b0  ..3 R.....^'.70.
-00000fa0: 5930 ec3b 6c9c f948 a1e8 4148 e64d ccb9  Y0.;l..H..AH.M..
-00000fb0: 8bdc e207 ed14 6745 d066 9aa7 2ef6 0379  ......gE.f.....y
-00000fc0: 0029 8ad1 2e57 21f8 0ef7 2b44 7f87 38e0  .)...W!...+D..8.
-00000fd0: 7c61 b8ef 52e2 85fb 7422 b843 13cf a459  |a..R...t".C...Y
-00000fe0: 82e8 2723 1188 e575 c2fd 7a1c b321 2686  ..'#...u..z..!&.
-00000ff0: 6580 f03d 1ecf 68fe 3a52 6714 58fd 04a9  e..=..h.:Rg.X...
-00001000: d7df 91ba dd95 4e92 fa26 6c80 a1d2 da3e  ......N..&l....>
-00001010: 41e5 8b70 ff42 02df c2a3 7c97 40cd cc93  A..p.B....|.@...
-00001020: e83b fe7e c7df d17f 9ebf 17d5 f2c5 b3f6  .;.~............
-00001030: 8ca8 81c3 677d bae9 dab3 854d fb90 32b6  ....g}.....M..2.
-00001040: afc6 8cdc 94a6 6f97 b03d 0dba 3068 0e14  ......o..=..0h..
-00001050: e654 393d c415 297c 2c8f 081e 2e11 d8cc  .T9=..)|,.......
-00001060: 4182 ab8f a84a f753 5c40 8b5f 35c7 d544  A....J.S\@._5..D
-00001070: 96a2 1389 0a2e a1f3 37c3 e638 4c4e c836  ........7..8LN.6
-00001080: c75b 0a8d bd39 a9d6 f519 c632 87c4 6a87  .[...9.....2..j.
-00001090: 0fec f08a 7b56 9d8a 3127 d7c4 9c87 278a  ....{V..1'....'.
-000010a0: 56b4 80b3 2a5b b9f2 76ca aad6 aa85 6ef3  V...*[..v.....n.
-000010b0: 9756 35a6 1952 f496 365d 32c4 707e 6930  .V5..R..6]2.p~i0
-000010c0: 38f5 26f4 3d08 ba25 f0f2 2a5c 1a68 dbe1  8.&.=..%..*\.h..
-000010d0: 3484 1919 68bf db73 fc24 2c5a f585 8648  4...h..s.$,Z...H
-000010e0: a618 ae24 6c8c f4ba e763 5435 419a e4ca  ...$l....cT5A...
-000010f0: 248d 0231 d2e7 ce53 62e4 686b 68b1 6fa1  $..1...Sb.hkh.o.
-00001100: ed2c 4172 d5d5 16a8 9b44 ef6d a234 396c  .,Ar.....D.m.49l
-00001110: cfa2 a4eb f644 39b2 dc2d 4e96 a3a3 66d4  .....D9..-N...f.
-00001120: a82f d723 14e3 a219 0de1 980d 1fb3 02a2  ./.#............
-00001130: 2e75 ab89 5902 b755 b112 36ed 4f2d 6693  .u..Y..U..6.O-f.
-00001140: aeb3 6836 c269 5985 9b13 ebf7 b905 7b3c  ..h6.iY.......{<
-00001150: 5008 a9b6 b04c 6d6a 9847 650a b0dc 5c0a  P....Lmj.Ge...\.
-00001160: 18fb 97eb e0d6 8b5a 80cd f437 b062 650d  .......Z...7.be.
-00001170: 92e1 6fb3 02fc e887 960c 8724 566e b09d  ..o........$Vn..
-00001180: 1173 2b62 0025 95f2 9122 623f 1d1c a13e  .s+b.%..."b?...>
-00001190: 1b89 3d0c e1d7 a90a eb19 5009 f721 8611  ..=.......P..!..
-000011a0: f417 b8da d3de 368f 7c72 2e8b cebd 5033  ......6.|r....P3
-000011b0: 383b 8e59 91e2 926e 7589 4e2a d9c2 4d1d  8;.Y...nu.N*..M.
-000011c0: 4f6d 30df acb5 c63c 585b d076 b3b8 f32f  Om0....<X[.v.../
-000011d0: c594 fc05 2dc5 4de3 ffd9 52f4 7e02 1714  ....-.M...R.~...
-000011e0: 2b03 1d81 18ee 9605 46ba 5e9b 1117 2ae5  +.......F.^...*.
-000011f0: c042 454a e3ae 806b 35c3 1d90 2d70 3d0c  .BEJ...k5...-p=.
-00001200: 8f21 a9e0 86db fc17 e450 ffb7 3567 6598  .!.......P..5ge.
-00001210: b286 73a6 daa3 0912 14f6 2395 0a42 7681  ..s.......#..Bv.
-00001220: 964c f69d 22ac 5aee 5d56 242b 0599 8c72  .L..".Z.]V$+...r
-00001230: cc95 8535 bb4f 0e09 eb69 0e5c d57b 7b84  ...5.O...i.\.{{.
-00001240: 5248 75c3 2625 0d18 dcc9 fcf3 bf97 15d4  RHu.&%..........
-00001250: 4f74 93f3 4fed 7c6c 319f b73d d0dd 816d  Ot..O.|l1..=...m
-00001260: b1ec fc33 f622 3587 f49d ada0 11dc fb4c  ...3."5........L
-00001270: 4f35 a583 d76c ece7 dc6a 2d63 cdad 78b9  O5...l...j-c..x.
-00001280: 7ee6 adb6 806b 26b8 5d56 9013 3115 31b3  ~....k&.]V..1.1.
-00001290: 2f4b f486 dae3 7bc0 ad08 de7d d8f6 0a41  /K....{....}...A
-000012a0: 565f b28d 07d2 0469 e9b1 0f8d 931d b4c9  V_.....i........
-000012b0: a445 d986 a5ec 6e2f bc8d 821b f2b2 d39d  .E....n/........
-000012c0: ea85 2a7d 934e f79c ce9e 3667 be3a af16  ..*}.N....6g.:..
-000012d0: 5fdf 7d9e cfd9 a587 3d5f bb9d 6ec0 d550  _.}.....=_..n..P
-000012e0: b427 4b54 b747 9383 8c09 8c79 cfe6 be08  .'KT.G.....y....
-000012f0: e3fd fb10 e82d 78e5 3062 4ada 9709 0fe0  .....-x.0bJ.....
-00001300: 5211 4e19 f6a5 0514 bf0d ae99 baf1 1700  R.N.............
-00001310: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00001320: 0000 2100 e97d fce0 0e03 0000 1e08 0000  ..!..}..........
-00001330: 0d00 0000 786c 2f73 7479 6c65 732e 786d  ....xl/styles.xm
-00001340: 6cb4 555b 4fdb 3014 7e9f b4ff 60f9 3de4  l.U[O.0.~...`.=.
-00001350: 42d3 b555 1244 5b22 2131 3409 26ed d54d  B..U.D["!14.&..M
-00001360: 9cd6 c297 c871 59ca b4ff bee3 386d 038c  .....qY.....8m..
-00001370: 8db1 eda5 b58f edef 5cbe ef9c 2467 ade0  ........\...$g..
-00001380: e89e ea86 2999 e2f0 24c0 88ca 4295 4cae  ....)...$...B.L.
-00001390: 53fc f936 f726 1835 86c8 9270 2569 8a77  S..6.&.5...p%i.w
-000013a0: b4c1 67d9 fb77 4963 769c de6c 2835 0820  ..g..wIcv..l(5. 
-000013b0: 6493 e28d 31f5 ccf7 9b62 4305 694e 544d  d...1....bC.iNTM
-000013c0: 259c 544a 0b62 60ab d77e 536b 4aca c63e  %.TJ.b`..~SkJ..>
-000013d0: 12dc 8f82 60ec 0bc2 2476 0833 51bc 0644  ....`...$v.3Q..D
-000013e0: 107d b7ad bd42 899a 18b6 629c 995d 8785  .}...B....b..]..
-000013f0: 9128 6697 6ba9 3459 7108 b50d 47a4 406d  .(f.k.4Yq...G.@m
-00001400: 38d6 d1de 4367 7ae6 44b0 42ab 4655 e604  8...Cgz.D.B.FU..
-00001410: 407d 5555 aca0 cf63 9dfa 539f 1447 2480  @}UU...c..S..G$.
-00001420: 7d1b 5218 fb41 e412 cf12 b915 b930 0d2a  }.R..A.......0.*
-00001430: d456 1a20 00ef 4dc8 9d5c 9660 1c8f 3072  .V. ..M..\.`..0r
-00001440: 755c a812 320b 4e82 20c0 7e96 f8fd f32c  u\..2.N. .~....,
-00001450: a994 3ca2 d87c 6df2 b33b a9be cadc 1e39  ..<..|m..;.....9
-00001460: 687b 2b4b 9a07 744f 3858 428b 5128 ae34  h{+K..tO8XB.Q(.4
-00001470: 3240 1a20 7716 4904 7537 1684 b395 66f6  2@. w.I.u7....f.
-00001480: 5a45 04e3 3b67 8eac a1e3 b9bf 2718 54bd  ZE..;g......'.T.
-00001490: 0bc8 7978 e2a7 8bf5 7ff8 f1bb b421 38c6  ..yx.........!8.
-000014a0: f9a1 8611 d4d0 1ab2 0404 62a8 9639 6c50  ..........b..9lP
-000014b0: bfbe ddd5 90a6 042d bb70 bb7b bfb9 bdd6  .......-.p.{....
-000014c0: 6417 46f1 e081 df39 cc92 95d2 25f4 ce90  d.F....9....%...
-000014d0: 3d67 ca12 4e2b 0355 d26c bdb1 ff46 d5f0  =g..N+.U.l...F..
-000014e0: bb52 c680 c4b2 a464 64ad 24e1 96c3 fd8b  .R.....dd.$.....
-000014f0: 7ed1 0025 94f3 1bdb 5f5f aa47 d86d 3550  ~..%....__.G.m5P
-00001500: 0574 aacd de0a c42e 2191 7ee9 f0dc c6e2  .t......!.~.....
-00001510: 0fd1 1cf6 0076 04c5 fa73 58d4 5607 fc97  .....v...sX.V...
-00001520: 5e87 2f06 7578 8d48 5df3 9dd5 67af bc7f  ^./.ux.H]...g...
-00001530: 86e5 90cf 395b 4b41 f78d 0562 765b b451  ....9[KA...bv[.Q
-00001540: 9a3d 805b db05 059c 5327 deb6 7a52 8cbe  .=.[....S'..zR..
-00001550: f35c 955f 9dd0 f556 aca8 cebb c167 137b  .\._...V.....g.{
-00001560: 9ce6 db43 eb98 04ee 0602 7924 8f03 d1c8  ...C......y$....
-00001570: 7670 8aaf 6d04 1c66 414f 165a 6d19 374c  vp..m..fAO.Zm.7L
-00001580: fe44 1a80 59b6 47b1 750d 6bec 18ed 6478  .D..Y.G.u.k...dx
-00001590: f002 422b 6945 b6dc dc1e 0e53 7c5c 7fa4  ..B+iE.....S|\..
-000015a0: 25db 8ae9 e1d6 2776 af4c 0791 e2e3 faca  %.....'v.L......
-000015b0: f644 38b6 fd44 5b73 d5c0 4882 7fb4 d52c  .D8..D[s..H....,
-000015c0: c5df 2ee6 1fa6 cb8b 3cf2 26c1 7ce2 8d4e  ........<.&.|..N
-000015d0: 69ec 4de3 f9d2 8b47 8bf9 7299 4f83 2858  i.M....G..r.O.(X
-000015e0: 7c1f ccf3 bf98 e6dd b707 180f 47b3 86c3  |...........G...
-000015f0: ccd7 7db2 7d8a 3747 5b8a 071b 177e 370d  ..}.}.7G[....~7.
-00001600: 20ec 61ec d368 1c9c c761 e0e5 a741 e88d   .a..h...a...A..
-00001610: c664 e24d c6a7 b197 c761 b41c 8fe6 1771  .d.M.....a.....q
-00001620: 1e0f 628f dff8 fd08 fc30 dc7f 3fda 309e  ..b......0..?.0.
-00001630: 1926 2867 72cf d59e a1a1 1548 82ed 2f92  .&(gr......H../.
-00001640: f0f7 4cf8 c70f 7bf6 0300 00ff ff03 0050  ..L...{........P
-00001650: 4b03 0414 0006 0008 0000 0021 00bf 6024  K..........!..`$
-00001660: 7b98 0200 00ad 0500 0018 0000 0078 6c2f  {............xl/
-00001670: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00001680: 312e 786d 6c8c 945b 4fdb 3014 c7df 27ed  1.xml..[O.0...'.
-00001690: 3b58 7e27 374a 69ab a648 d0c1 90b6 695a  ;X~'7Ji..H....iZ
-000016a0: 7779 769c 93c6 22c9 c96c b7a5 7cfa 1d3b  wyv..."..l..|..;
-000016b0: 490b 2a43 bcc4 767c fc3b ff73 b1e7 578f  I.*C..v|.;.s..W.
-000016c0: 75c5 b6a0 8dc2 26e5 7110 7106 8dc4 5c35  u.....&.q.q...\5
-000016d0: eb94 fffa 797b 36e1 cc58 d1e4 a2c2 0652  ....y{6..X.....R
-000016e0: be07 c3af 161f 3fcc 77a8 1f4c 0960 1911  ......?.w..L.`..
-000016f0: 1a93 f2d2 da76 1686 4696 500b 1360 0b0d  .....v..F.P..`..
-00001700: ed14 a86b 6169 a9d7 a169 3588 dc1f aaab  ...kai...i5.....
-00001710: 3089 a271 580b d5f0 8e30 d3ef 6160 5128  0..qX....0..a`Q(
-00001720: 094b 949b 1a1a db41 3454 c292 7e53 aad6  .K.....A4T..~S..
-00001730: 0cb4 5abe 0757 0bfd b069 cf24 d62d 2132  ..Z..W...i.$.-!2
-00001740: 5529 bbf7 50ce 6a39 bb5f 37a8 4556 51dc  U)..P.j9._7.EVQ.
-00001750: 8ff1 48c8 81ed 1727 f85a 498d 060b 1b10  ..H....'.ZI.....
-00001760: 2eec 849e c63c 0da7 2191 16f3 5c51 042e  .....<..!...\Q..
-00001770: ed4c 4391 f2eb 78f6 29e6 e162 eef3 f35b  .LC...x.)..b...[
-00001780: c1ce 3c9b 3353 e2ee 4eab fc8b 6a80 924d  ..<.3S..N...j..M
-00001790: 65b2 225b 4105 d242 4e85 e3ec 09b1 5e49  e."[A..BN.....^I
-000017a0: e1c4 c6f1 c5b3 f537 5782 aaff ebca 9621  .......7W......!
-000017b0: 3e38 07f7 7430 2225 c663 9c12 21ad dac2  >8..t0"%.c..!...
-000017c0: 0d54 647e 17bb d2ff f5e2 dc9c a485 076d  .Td~...........m
-000017d0: cfe7 83ce 5b5f eaef 9a65 c2c0 0d56 7f54  ....[_...e...V.T
-000017e0: 6e4b 724b 5a73 28c4 a6b2 c79f d320 1e45  nKrKZs(...... .E
-000017f0: e384 64f6 5b3f 70f7 19d4 bab4 7420 092e  ..d.[?p.....t ..
-00001800: 69c3 2779 96ef 9760 2495 9aa4 0689 1321  i.'y...`$......!
-00001810: b122 8ff4 65b5 722d 4b95 128f 7edc f50e  ."..e.r-K...~...
-00001820: c707 b8b1 7b9f 0fce e4c6 58ac 0749 3da7  ....{.....X..I=.
-00001830: 2324 3de1 9cb3 8110 05a3 e4e2 7212 3b81  #$=.........r.;.
-00001840: 3d83 76df 608c 7a06 8d03 830e f447 c9c1  =.v.`.z......G..
-00001850: 1b47 c985 0f80 c6e1 e8c5 2b01 6460 ecad  .G........+.d`..
-00001860: 72e9 7993 361e 841c 71c7 5cbf 2b1d a301  r.y.6...q.\.+...
-00001870: 118f cf27 c778 5ea1 b88e e8aa e1fb 6229  ...'.x^.......b)
-00001880: ac58 cc35 ee18 dd64 5269 5ae1 de85 64f6  .X.5...dRiZ...d.
-00001890: bf62 5215 9de9 b5b3 253b 6ae9 941b eac7  .bR.....%;j.....
-000018a0: ed22 9a87 5b07 ef2d 6e4e 2de2 9716 cb53  ."..[..-nN-....S
-000018b0: 8be4 a505 5d2e e785 be07 2fe7 078b 9054  ....]...../....T
-000018c0: 0f2d dd85 d18a 357c 157a ad1a c32a 287c  .-....5|.z...*(|
-000018d0: fb5d 72a6 bb16 8d02 9a5b 6c5d 53ba 5ecd  .]r......[l]S.^.
-000018e0: d052 770d ab92 5e39 a0c0 a280 7aa0 40b4  .Rw...^9....z.@.
-000018f0: c382 12e6 b82b b09b 96b5 a205 bd52 4f74  .....+.......ROt
-00001900: 5fa7 9ca1 56d4 e4fe 194b 798b da6a a1ac  _...V....Ky..j..
-00001910: bf73 8787 76f1 0f00 00ff ff03 0050 4b03  .s..v........PK.
-00001920: 0414 0006 0008 0000 0021 005e 7e59 7cbd  .........!.^~Y|.
-00001930: 0100 007d 0400 0018 0028 0063 7573 746f  ...}.....(.custo
-00001940: 6d58 6d6c 2f69 7465 6d50 726f 7073 322e  mXml/itemProps2.
-00001950: 786d 6c20 a224 0028 a020 0000 0000 0000  xml .$.(. ......
-00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001970: 0000 0000 0000 0000 0000 00b4 945b 6bdc  .............[k.
-00001980: 3010 85df 0bfd 0f46 efb2 e48b 7c09 f186  0......F....|...
-00001990: cd2e 0b81 064a 9b42 5ec7 b2b4 6b6a 4946  .....J.B^...kjIF
-000019a0: 92bb 2da5 ffbd b293 52d2 6cd8 96b6 4ff6  ..-.....R.l...O.
-000019b0: d8cc 3933 c79f 7c79 f559 0dd1 2761 5d6f  ..93..|y.Y..'a]o
-000019c0: 7483 9298 a248 686e ba5e ef1b f4e1 6e87  t....Hhn.^....n.
-000019d0: 2b14 390f ba83 c168 d120 6dd0 d5ea f5ab  +.9....h. m.....
-000019e0: cbce 5d74 e0c1 7963 c58d 172a 0a0f fa70  ..]t..yc...*...p
-000019f0: bdd9 36e8 eb8e aeb7 eb7a c3f0 26ad 4b9c  ..6......z..&.K.
-00001a00: d775 86d7 f98e e1f4 9a55 05bb deee 3675  .u.......U....6u
-00001a10: fa0d 45c1 5a07 19d7 a083 f7e3 0521 8e1f  ..E.Z........!..
-00001a20: 8402 179b 51e8 f052 1aab c087 d2ee 8991  ....Q..R........
-00001a30: b2e7 626b f8a4 84f6 24a5 b420 7c0a f6ea  ..bk....$.. |...
-00001a40: 5e0d 6835 cff3 d0fd 4e48 f7b4 9c47 9b6c  ^.h5....NH...G.l
-00001a50: ffcc 45f5 dc1a 67a4 8fb9 518f 060f c24a  ..E...g...Q....J
-00001a60: 7898 b723 dc68 1fec eebe 8c02 917f a63a  x..#.h.........:
-00001a70: dab0 a0f5 bd70 6476 5a7b 6ffb 76f2 c29d  .....pdvZ{o.v...
-00001a80: f338 1e8f f131 5bf2 0801 24e4 fef6 cdfb  .8...1[...$.....
-00001a90: 25b2 ff32 dc8b a26d 490b 2864 8669 295b  %..2...mI.(d.i)[
-00001aa0: 9cb7 5985 2b46 1986 b264 05af 92ba cde1  ..Y.+F...d......
-00001ab0: c566 9a54 0974 acc4 ac66 29ce 69b8 0309  .f.T.t...f).i...
-00001ac0: 1297 3483 2ea5 590d bcfa fb75 ba47 506e  ..4...Y....u.GPn
-00001ad0: 41c3 5e2c c8f8 f011 cf26 fc83 c093 6cf4  A.^,.....&....l.
-00001ae0: 5a9a 11fc 6186 a424 6fc1 7a2d ec26 2062  Z...a..$o.z-.& b
-00001af0: cdf0 dbca 27d8 1e81 7f0c 533e 63cf 0afc  ....'.....S>c...
-00001b00: 1395 7399 8c93 1d16 323a 4ec4 b0ac ec48  ..s.....2:N....H
-00001b10: 1227 e44f 1abd b0ca 9ded 381d 521f 8e8a  .'.O......8.R...
-00001b20: d530 10d3 76b3 27f9 e548 cef5 935f c6ea  .0..v.'..H..._..
-00001b30: 3b00 0000 ffff 0300 504b 0304 1400 0600  ;.......PK......
-00001b40: 0800 0000 2100 5c96 2722 c300 0000 2801  ....!.\.'"....(.
-00001b50: 0000 1e00 0801 6375 7374 6f6d 586d 6c2f  ......customXml/
-00001b60: 5f72 656c 732f 6974 656d 322e 786d 6c2e  _rels/item2.xml.
-00001b70: 7265 6c73 20a2 0401 28a0 0001 0000 0000  rels ...(.......
-00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c70: 0000 0000 0000 0000 0000 0000 84cf c16a  ...............j
-00001c80: c330 0c06 e07b a1ef 6074 5f9c f630 4a89  .0...{..`t_..0J.
-00001c90: d34b 19e4 3646 0bbd 1a47 494c 63cb 584a  .K..6F...GILc.XJ
-00001ca0: 69df 7ea6 a716 063b 4a42 df2f 3587 7b98  i.~....;JB./5.{.
-00001cb0: d50d 337b 8a06 3655 0d0a a3a3 dec7 d1c0  ..3{..6U........
-00001cc0: f9f4 f5b1 03c5 6263 6f67 8a68 e081 0c87  ......bcog.h....
-00001cd0: 76bd 6a7e 70b6 5296 78f2 8955 5122 1b98  v.j~p.R.x..UQ"..
-00001ce0: 44d2 5e6b 7613 06cb 1525 8c65 3250 0e56  D.^kv....%.e2P.V
-00001cf0: 4a99 479d acbb da11 f5b6 ae3f 757e 35a0  J.G........?u~5.
-00001d00: 7d33 55d7 1bc8 5dbf 0175 7aa4 92fc bf4d  }3U...]..uz....M
-00001d10: c3e0 1d1e c92d 01a3 fc11 a1dd c242 e112  .....-.......B..
-00001d20: e6ef 4c89 8b6c f388 62c0 0b86 676b 5b95  ..L..l..b...gk[.
-00001d30: 7b41 b78d 7efb affd 0500 00ff ff03 0050  {A..~..........P
-00001d40: 4b03 0414 0006 0008 0000 0021 0074 3f39  K..........!.t?9
-00001d50: 7ac2 0000 0028 0100 001e 0008 0163 7573  z....(.......cus
-00001d60: 746f 6d58 6d6c 2f5f 7265 6c73 2f69 7465  tomXml/_rels/ite
-00001d70: 6d31 2e78 6d6c 2e72 656c 7320 a204 0128  m1.xml.rels ...(
-00001d80: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e80: 0000 0084 cfc1 8a02 310c 06e0 bbe0 3b94  ........1.....;.
-00001e90: dc9d ce78 1091 e978 5916 bc89 b8e0 b574  ...x...xY......t
-00001ea0: 3233 c569 539a 28fa f616 4f2b 2cec 3109  23.iS.(...O+,.1.
-00001eb0: f9fe a4dd 3fc2 acee 98d9 5334 d054 3528  ....?.....S4.T5(
-00001ec0: 8c8e 7a1f 4703 3fe7 efd5 1614 8b8d bd9d  ..z.G.?.........
-00001ed0: 29a2 8127 32ec bbe5 a23d e16c a52c f1e4  )..'2....=.l.,..
-00001ee0: 13ab a244 3630 89a4 9dd6 ec26 0c96 2b4a  ...D60.....&..+J
-00001ef0: 18cb 64a0 1cac 9432 8f3a 5977 b523 ea75  ..d....2.:Yw.#.u
-00001f00: 5d6f 74fe 6d40 f761 aa43 6f20 1ffa 06d4  ]ot.m@.a.Co ....
-00001f10: f999 4af2 ff36 0d83 77f8 45ee 1630 ca1f  ..J..6..w.E..0..
-00001f20: 11da dd58 285c c27c cc94 b8c8 368f 2806  ...X(\.|....6.(.
-00001f30: bc60 78b7 9aaa dc0b ba6b f5c7 7fdd 0b00  .`x......k......
-00001f40: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00001f50: 0021 00bd 8462 2390 0000 00db 0000 0013  .!...b#.........
-00001f60: 0028 0063 7573 746f 6d58 6d6c 2f69 7465  .(.customXml/ite
-00001f70: 6d31 2e78 6d6c 20a2 2400 28a0 2000 0000  m1.xml .$.(. ...
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f90: 0000 0000 0000 0000 0000 0000 0000 6c8e  ..............l.
-00001fa0: 3b0e c230 1005 af82 d293 2de8 d0e2 3481  ;..0......-...4.
-00001fb0: 0a51 e502 c638 8aa5 acd7 f22e 1fdf 1e07  .Q...8..........
-00001fc0: 4181 947a 9e66 1e76 24bc 751c d547 1d4a  A..z.f.v$.u..G.J
-00001fd0: f29d c113 671a 3ca5 d9aa 97cd 8be6 2887  ....g.<.......(.
-00001fe0: 6652 4d7b 0071 9327 2b2d 0597 5978 d4d6  fRM{.q.'+-..Yx..
-00001ff0: 3181 4c36 fbc4 212a 3c76 f0b5 69b5 c158  1.L6..!*<v..i..X
-00002000: 5dd2 18ec 8354 5f31 3dbb 3bd5 d439 5cb3  ]....T_1=.;..9\.
-00002010: cd65 4921 fc20 1e6f 41d7 271f 8217 ff5c  .eI!. .oA.'....\
-00002020: c70b 40f8 3b6e de00 0000 ffff 0300 504b  ..@.;n........PK
-00002030: 0304 1400 0600 0800 0000 2100 1118 db79  ..........!....y
-00002040: f400 0000 4f01 0000 1800 2800 6375 7374  ....O.....(.cust
-00002050: 6f6d 586d 6c2f 6974 656d 5072 6f70 7331  omXml/itemProps1
-00002060: 2e78 6d6c 20a2 2400 28a0 2000 0000 0000  .xml .$.(. .....
-00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002080: 0000 0000 0000 0000 0000 0000 6490 416b  ............d.Ak
-00002090: 8340 1085 ef85 fe07 d9bb ae6b 6cac 410d  .@.........kl.A.
-000020a0: 498c 906b 69a1 d765 1de3 82bb 23bb 6368  I..ki..e....#.ch
-000020b0: 29fd ef5d e929 ed69 78f3 98f7 3da6 da7f  )..].).ix...=...
-000020c0: 9829 ba81 f31a 6dcd 4492 b208 acc2 5edb  .)....m.D.....^.
-000020d0: 6bcd de5e bbf8 9945 9ea4 ede5 8416 6a66  k..^...E......jf
-000020e0: 91ed 9bc7 87aa f7bb 5e92 f484 0e2e 0426  ........^......&
-000020f0: 0a0b 1de6 a5ad d957 763c 9799 1022 2e8e  .......Wv<..."..
-00002100: 6511 e7e7 d329 3e6c f22e dee6 6527 9eb2  e....)>l....e'..
-00002110: 8328 d2f6 9b45 016d 438c afd9 4834 ef38  .(...E.mC...H4.8
-00002120: f76a 0423 7d82 33d8 600e e88c a420 dd95  .j.#}.3.`.... ..
-00002130: e330 6805 2daa c580 259e a5e9 96ab 25e0  .0h.-...%.....%.
-00002140: cdbb 9958 b3f6 f9bd 7e81 c1df cbb5 dae2  ...X....~.......
-00002150: f43f 8ad1 caa1 c781 1285 86fb 513a 9851  .?..........Q:.Q
-00002160: 87f0 db86 2bb4 1438 f439 035f 6b78 c69b  ....+..8.9._kx..
-00002170: 8aff 81ac faee 09cd 0f00 0000 ffff 0300  ................
-00002180: 504b 0304 1400 0600 0800 0000 2100 a05a  PK..........!..Z
-00002190: 864d 8a01 0000 0703 0000 1000 0801 646f  .M............do
-000021a0: 6350 726f 7073 2f61 7070 2e78 6d6c 20a2  cProps/app.xml .
-000021b0: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022b0: 0000 0000 0000 9c92 c16e 1331 1086 ef48  .........n.1...H
-000022c0: bc83 e57b e34d 4115 8abc ae50 0bca 0144  ...{.MA....P...D
-000022d0: a4a4 bd1b 7b36 3138 f6ca 3359 25bc 0dcf  ....{618..3Y%...
-000022e0: c28b 31bb aba6 9b96 13b7 99f9 67ff fdfc  ..1.........g...
-000022f0: dbfa f6b8 8fa2 8382 21a7 5ace 6795 1490  ........!.Z.g...
-00002300: 5cf6 216d 6bf9 b0f9 7cf5 410a 249b bc8d  \.!mk...|.A.$...
-00002310: 3941 2d4f 80f2 d6bc 7da3 5725 b750 2800  9A-O....}.W%.P(.
-00002320: 0ab6 4858 cb1d 51bb 500a dd0e f616 672c  ..HX..Q.P.....g,
-00002330: 2756 9a5c f696 b82d 5b95 9b26 38b8 cfee  'V.\...-[..&8...
-00002340: b087 44ea baaa 6e14 1c09 9207 7fd5 9e0d  ..D...n.........
-00002350: e5e8 b8e8 e87f 4d7d 763d 1f3e 6e4e 2d03  ......M}v=.>nN-.
-00002360: 1bfd b16d 6370 96f8 94e6 6b70 2563 6e48  ...mcp....kp%cnH
-00002370: 7c3a 3a88 5a4d 45cd 746b 7087 12e8 642a  |::.ZME.tkp...d*
-00002380: ada6 ad5e 3b1b e18e 8d4d 6323 8256 cf03  ...^;....Mc#.V..
-00002390: bd04 db87 b6b2 a1a0 d11d 2d3a 7094 8bc0  ..........-:p...
-000023a0: f08b 63bb 96e2 bb45 e871 6ad9 d912 6c22  ..c....E.qj...l"
-000023b0: c6ea d7c6 66a8 638b 54cc 32ff b028 3c08  ....f.c.T.2..(<.
-000023c0: f7e7 7774 8798 b5e2 bd51 1bca e927 d33a  ..wt.....Q...'.:
-000023d0: bc37 f361 818b cbc5 de60 e461 e192 7413  .7.a.....`.a..t.
-000023e0: 2802 7e6b 56b6 d03f c0e7 53f0 8161 c41e  (.~kV..?..S..a..
-000023f0: 71c6 9751 fc2b c2e1 ecfc af17 ee5f 42fa  q..Q.+......._B.
-00002400: 890f ed26 df5b 82a7 102f 877a bdb3 053c  ...&.[.../.z...<
-00002410: e77e 0ef9 3cd0 4bce afc4 dee4 6e67 d316  .~..<.K.....ng..
-00002420: fcd3 ce6b a1bf f2c7 f15d 9bf9 cdac 7a57  ...k.....]....zW
-00002430: f16d 4e66 5a3d bf60 f317 0000 ffff 0300  .mNfZ=.`........
-00002440: 504b 0304 1400 0600 0800 0000 2100 c8fa  PK..........!...
-00002450: e105 4801 0000 6902 0000 1100 0801 646f  ..H...i.......do
-00002460: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
-00002470: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
-00002480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000024f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000830: 0000 bc94 4d6b c330 0c86 ef83 fd07 e3fb  ....Mk.0........
+00000840: a224 ddba 32ea f432 06bd 6e19 ec6a 1ce5  .$..2..2..n..j..
+00000850: 83c6 76b0 d56d f9f7 3319 4b53 28d9 25f4  ..v..m..3.KS(.%.
+00000860: 6290 84df f7b1 84bc dd7d eb96 7da2 f38d  b........}..}...
+00000870: 3582 2751 cc19 1a65 8bc6 5482 bfe7 2f77  5.'Q...e..T.../w
+00000880: 1bce 3c49 53c8 d61a 14bc 47cf 77d9 edcd  ..<IS.....G.w...
+00000890: f615 5b49 e192 af9b ceb3 a062 bce0 3551  ..[I.......b..5Q
+000008a0: f704 e055 8d5a fac8 7668 42a5 b44e 4b0a  ...U.Z..vhB..NK.
+000008b0: a1ab a093 ea20 2b84 348e d7e0 a61a 3c3b  ..... +.4.....<;
+000008c0: d364 fb42 70b7 2f56 9ce5 7d17 9cff d7b6  .d.Bp./V..}.....
+000008d0: 65d9 287c b6ea a8d1 d005 0bf0 d4b7 e101  e.(|............
+000008e0: 2c97 ae42 12fc 378e 0223 87cb f68f 4bda  ,..B..7..#....K.
+000008f0: aba3 27ab 3f82 db48 1045 3066 a121 d4ab  ..'.?..H.E0f.!..
+00000900: 399a 7449 1a0a 43c2 13c9 10c2 7026 730c  9.tI..C.....p&s.
+00000910: c992 0c5f d61d 7c8d 4827 8e31 e561 a8cc  ..._..|.H'.1.a..
+00000920: c2ac af3d 9e74 ae35 0fd7 a699 edcd fda2  ...=.t.5........
+00000930: 9b53 4b87 c51b b9f0 314c 1768 9afe 6b0d  .SK.....1L.h..k.
+00000940: 9cfd 0dd9 0f00 0000 ffff 0300 504b 0304  ............PK..
+00000950: 1400 0600 0800 0000 2100 e619 1dd3 2302  ........!.....#.
+00000960: 0000 4104 0000 0f00 0000 786c 2f77 6f72  ..A.......xl/wor
+00000970: 6b62 6f6f 6b2e 786d 6ca4 53cb 6edb 3010  kbook.xml.S.n.0.
+00000980: bc17 e83f 10bc 1631 2dd7 111a c372 e038  ...?...1-....r.8
+00000990: 7d04 480b 234d 9363 b126 d716 11be 4a52  }.H.#M.c.&....JR
+000009a0: b5f3 f75d 4955 9a34 9714 bd88 bbe4 6ac8  ...]IU.4......j.
+000009b0: 9d99 9d9f 1eac 613f 3126 ed5d c58b d198  ......a?1&.]....
+000009c0: 3374 d22b ed76 15ff 76fd e1e8 1d67 2983  3t.+.v..v....g).
+000009d0: 5360 bcc3 8adf 63e2 a78b d7af e67b 1fef  S`....c......{..
+000009e0: 36de df31 0270 a9e2 75ce 6126 4492 355a  6..1.p..u.a&D.5Z
+000009f0: 4823 1fd0 d1c9 d647 0b99 d2b8 1329 4404  H#.....G.....)D.
+00000a00: 956a c46c 8d98 8cc7 a5b0 a01d ef11 66f1  .j.l..........f.
+00000a10: 2518 7ebb d512 cfbd 6c2c badc 8344 3490  %.~.....l,...D4.
+00000a20: e9f9 a9d6 210d 6856 be04 ce42 bc6b c291  ....!.hV...B.k..
+00000a30: f436 10c4 461b 9def 3b50 ceac 9c5d ec9c  .6..F...;P...]..
+00000a40: 8fb0 31d4 f6a1 381e 9029 7c06 6db5 8c3e  ..1...8..)|.m..>
+00000a50: f96d 1e11 94e8 1ff9 acdf 622c 8aa2 6f79  .m........b,..oy
+00000a60: 31df 6a83 373d ed0c 42f8 02b6 bdc5 7066  1.j.7=..B.....pf
+00000a70: 20e5 f74a 6754 152f 29f5 7b7c b211 9b70   ..JgT./).{|...p
+00000a80: d668 43a7 c574 3a19 73b1 7890 621d 99c2  .hC..t:.s.x.b...
+00000a90: 2d34 265f 9308 033c 154e a693 49d9 5652  -4&_...<.N..I.VR
+00000aa0: 534b 9331 3ac8 b8f2 2e13 87bf d9ff 5fbe  SK.1:........._.
+00000ab0: 3aec 55ed 491d 7685 3f1a 1d91 4cd1 d2b6  :.U.I.v.?...L...
+00000ac0: 98d3 17e4 0c36 690d b966 4d34 3d7f 89ec  .....6i..fM4=...
+00000ad0: d248 f06f cbe3 51aa 2162 f0da f50c 26ea  .H.o..Q.!b....&.
+00000ae0: 3f89 ab33 ed57 ab4b d888 4170 9f58 a755  ?..3.W.K..Ap.X.U
+00000af0: cc5a f924 3ea2 c308 469c afa7 6fd8 3204  .Z.$>...F...o.2.
+00000b00: b13c fa4a 22ec 094b a830 0da6 49df 895c  .<.J"..K.0..I..\
+00000b10: 91a2 7c92 3f92 129e fbe4 1fc4 04d9 b22a  ..|.?..........*
+00000b20: 88d6 bef5 3efe 9be2 c5bc 1d94 1b8d fbf4  ....>...........
+00000b30: 47ac 3665 875b ed94 df57 7c32 a5c1 bb1f  G.6e.[...W|2....
+00000b40: b2d6 6cfb eee4 56ab 5c93 82e5 f8e4 61ef  ..l...V.\.....a.
+00000b50: 13ea 5d9d 2b7e 5296 9dfc e211 7a37 5d74  ..].+~R.....z7]t
+00000b60: 4bb7 32d7 b9aa 1fdf a868 90db d9bb 68ad  K.2......h....h.
+00000b70: c359 9c69 0ae2 852a ba16 861f 2518 493e  .Y.i...*....%.I>
+00000b80: 6a97 b690 5ed5 869f bd22 7b5a 700d 98ae  j...^...."{Zp...
+00000b90: 7c98 fec5 2f00 0000 ffff 0300 504b 0304  |.../.......PK..
+00000ba0: 1400 0600 0800 0000 2100 9c63 914c aa00  ........!..c.L..
+00000bb0: 0000 ea00 0000 1400 0000 786c 2f73 6861  ..........xl/sha
+00000bc0: 7265 6453 7472 696e 6773 2e78 6d6c 5cce  redStrings.xml\.
+00000bd0: c10a c230 0cc6 f1bb e03b 94dc 5da7 8888  ...0.....;..]...
+00000be0: b4dd 6122 5ebc e903 942d 6e85 359d 4b26  ..a"^....-n.5.K&
+00000bf0: faf6 4e44 108f ff5f f820 a678 c44e dd71  ..ND..._. .x.N.q
+00000c00: e090 c8c2 32cb 4121 55a9 0ed4 58b8 9c0f  ....2.A!U...X...
+00000c10: 8b2d 2816 4fb5 ef12 a185 2732 146e 3e33  .-(.O.....'2.n>3
+00000c20: cca2 a62d b185 56a4 df69 cd55 8bd1 7396  ...-..V..i.U..s.
+00000c30: 7aa4 e972 4d43 f432 e5d0 68ee 07f4 35b7  z..rMC.2..h...5.
+00000c40: 8812 3bbd caf3 8d8e 3e10 a82a 8d24 16d6  ..;.....>..*.$..
+00000c50: a046 0ab7 11cb 6f3b c3c1 1971 a5d1 e28c  .F....o;...q....
+00000c60: 7ec7 078e ffb0 f782 ff76 4af5 8fe9 e957  ~........vJ....W
+00000c70: f702 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00000c80: 0800 0000 2100 1ae8 a8b7 9106 0000 e51b  ....!...........
+00000c90: 0000 1300 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
+00000ca0: 6865 6d65 312e 786d 6cec 59cd 6e1b 3710  heme1.xml.Y.n.7.
+00000cb0: be17 e83b 107b 4f2c d992 6319 9103 4b96  ...;.{O,..c...K.
+00000cc0: e236 7162 d84a 8a1c a915 b5cb 98bb 5c90  .6qb.J........\.
+00000cd0: 941d dd8a e458 a040 d1b4 e8a5 406f 3d14  .....X.@....@o=.
+00000ce0: 6d03 2440 2fe9 d3b8 4dd1 a640 5ea1 4372  m.$@/...M..@^.Cr
+00000cf0: 2591 1615 db89 81fe c506 6c89 fb71 6638  %.........l..qf8
+00000d00: 3f1f 87dc abd7 1e64 0c1d 1221 29cf 9b51  ?......d...!)..Q
+00000d10: f572 2542 248f f980 e649 33ba d3eb 5e5a  .r%B$....I3...^Z
+00000d20: 8b90 5438 1f60 c673 d28c c644 46d7 36de  ..T8.`.s...DF.6.
+00000d30: 7fef 2a5e 5729 c908 82f9 b95c c7cd 2855  ..*^W).....\..(U
+00000d40: aa58 5f5a 9231 0c63 7999 1724 8767 432e  .X_Z.1.cy..$.gC.
+00000d50: 32ac e0ab 4896 0602 1f81 dc8c 2d2d 572a  2...H.......--W*
+00000d60: ab4b 19a6 7984 729c 81d8 1ecc 4103 826e  .K..y.r.....A..n
+00000d70: 0f87 3426 d1c6 447c 8781 8e5c 493d 1033  ..4&..D|...\I=.3
+00000d80: b1af 8593 728e 831d 1c54 3542 8e65 9b09  ....r....T5B.e..
+00000d90: 7488 5933 024d 037e d423 0f54 8418 960a  t.Y3.M.~.#.T....
+00000da0: 1e34 a38a f989 9636 ae2e e1f5 7212 530b  .4.....6....r.S.
+00000db0: e63a f3ba e6a7 9c57 4e18 1c2c 1b9d 22e9  .:.....WN..,..".
+00000dc0: 4f95 56bb b5c6 95ad a97c 0360 6a1e d7e9  O.V......|.`j...
+00000dd0: 74da 9dea 549e 01e0 3886 955a 5b5c 99b5  t...T...8..Z[\..
+00000de0: ee5a b535 91e9 80ec c779 d9ed 4abd 52f3  .Z.5.....y..J.R.
+00000df0: f18e fc95 399b 1bad 56ab de28 6db1 420d  ....9...V..(m.B.
+00000e00: c87e accd e1d7 2aab b5cd 650f 6f40 165f  .~....*...e.o@._
+00000e10: 9fc3 d75a 9bed f6aa 8737 208b 5f9d c377  ...Z.....7 ._..w
+00000e20: af34 566b 3ede 8052 46f3 8339 b40e 68b7  .4Vk>..RF..9..h.
+00000e30: 5b4a 9f42 869c 6d07 e16b 005f ab94 f019  [J.B..m..k._....
+00000e40: 0ab2 619a 5d5a c590 e76a 51ae 65f8 3e17  ..a.]Z...jQ.e.>.
+00000e50: 5d00 6820 c38a e648 8d0b 32c4 31e4 711b  ].h ...H..2.1.q.
+00000e60: 677d 4171 840a 9c73 0903 95e5 4ab7 b202  g}Aq...s....J...
+00000e70: 7ff5 6fcd 7caa 69f5 789d 6067 9e1d 8ae5  ..o.|.i.x.`g....
+00000e80: dc90 b604 c958 d042 35a3 0f41 6ae4 405e  .....X.B5..Aj.@^
+00000e90: 3dff fed5 f3a7 e8d5 f327 c70f 9f1d 3ffc  =........'....?.
+00000ea0: e9f8 d1a3 e387 3f5a 59de c46d 9c27 eec4  ......?ZY..m.'..
+00000eb0: 97df 7ef6 e7d7 1fa3 3f9e 7ef3 f2f1 1761  ..~.....?.~....a
+00000ec0: bc74 f1bf fef0 c92f 3f7f 1e06 427d cdd6  .t...../?...B}..
+00000ed0: ffe2 cb27 bf3d 7bf2 e2ab 4f7f ffee 7100  ...'.={...O...q.
+00000ee0: be29 70df 85f7 6846 24ba 458e d01e cf60  .)p...hF$.E....`
+00000ef0: 6dc6 31be e5a4 2fce 37a3 9762 eacd c029  m.1.../.7..b...)
+00000f00: c80e 88ee a8d4 03de 1a63 16c2 b588 efbc  .........c......
+00000f10: bb02 a825 04bc 3eba efd9 ba9f 8a91 a201  ...%..>.........
+00000f20: cd37 d2cc 03ee 70ce 5a5c 041d 7043 eb72  .7....p.Z\..pC.r
+00000f30: 3cdc 1be5 4958 b918 b9b8 3d8c 0f43 badb  <...IX....=..C..
+00000f40: 38f7 42db 1915 c0a9 90b2 f3be 6fa7 c433  8.B.........o..3
+00000f50: 7397 e15c e184 e444 21fd 8c1f 1012 9876  s..\...D!......v
+00000f60: 8f52 cfaf 3b34 165c f2a1 42f7 286a 611a  .R..;4.\..B.(ja.
+00000f70: 7449 8ff6 bd44 9a4d daa6 19c4 651c 3210  tI...D.M....e.2.
+00000f80: 42ed f966 e72e 6a71 165a f516 39f4 9150  B..f..jq.Z..9..P
+00000f90: 1098 058c ef11 e6b9 f13a 1e29 9c85 44f6  .........:.)..D.
+00000fa0: 70c6 5c87 dfc4 2a0d 19b9 3f16 b18b eb48  p.\...*...?....H
+00000fb0: 0591 4e08 e3a8 3320 5286 e6dc 16b0 5e27  ..N...3 R.....^'
+00000fc0: e837 30b0 5930 ec3b 6c9c f948 a1e8 4148  .70.Y0.;l..H..AH
+00000fd0: e64d ccb9 8bdc e207 ed14 6745 d066 9aa7  .M........gE.f..
+00000fe0: 2ef6 0379 0029 8ad1 2e57 21f8 0ef7 2b44  ...y.)...W!...+D
+00000ff0: 7f87 38e0 7c61 b8ef 52e2 85fb 7422 b843  ..8.|a..R...t".C
+00001000: 13cf a459 82e8 2723 1188 e575 c2fd 7a1c  ...Y..'#...u..z.
+00001010: b321 2686 6580 f03d 1ecf 68fe 3a52 6714  .!&.e..=..h.:Rg.
+00001020: 58fd 04a9 d7df 91ba dd95 4e92 fa26 6c80  X.........N..&l.
+00001030: a1d2 da3e 41e5 8b70 ff42 02df c2a3 7c97  ...>A..p.B....|.
+00001040: 40cd cc93 e83b fe7e c7df d17f 9ebf 17d5  @....;.~........
+00001050: f2c5 b3f6 8ca8 81c3 677d bae9 dab3 854d  ........g}.....M
+00001060: fb90 32b6 afc6 8cdc 94a6 6f97 b03d 0dba  ..2.......o..=..
+00001070: 3068 0e14 e654 393d c415 297c 2c8f 081e  0h...T9=..)|,...
+00001080: 2e11 d8cc 4182 ab8f a84a f753 5c40 8b5f  ....A....J.S\@._
+00001090: 35c7 d544 96a2 1389 0a2e a1f3 37c3 e638  5..D........7..8
+000010a0: 4c4e c836 c75b 0a8d bd39 a9d6 f519 c632  LN.6.[...9.....2
+000010b0: 87c4 6a87 0fec f08a 7b56 9d8a 3127 d7c4  ..j.....{V..1'..
+000010c0: 9c87 278a 56b4 80b3 2a5b b9f2 76ca aad6  ..'.V...*[..v...
+000010d0: aa85 6ef3 9756 35a6 1952 f496 365d 32c4  ..n..V5..R..6]2.
+000010e0: 707e 6930 38f5 26f4 3d08 ba25 f0f2 2a5c  p~i08.&.=..%..*\
+000010f0: 1a68 dbe1 3484 1919 68bf db73 fc24 2c5a  .h..4...h..s.$,Z
+00001100: f585 8648 a618 ae24 6c8c f4ba e763 5435  ...H...$l....cT5
+00001110: 419a e4ca 248d 0231 d2e7 ce53 62e4 686b  A...$..1...Sb.hk
+00001120: 68b1 6fa1 ed2c 4172 d5d5 16a8 9b44 ef6d  h.o..,Ar.....D.m
+00001130: a234 396c cfa2 a4eb f644 39b2 dc2d 4e96  .49l.....D9..-N.
+00001140: a3a3 66d4 a82f d723 14e3 a219 0de1 980d  ..f../.#........
+00001150: 1fb3 02a2 2e75 ab89 5902 b755 b112 36ed  .....u..Y..U..6.
+00001160: 4f2d 6693 aeb3 6836 c269 5985 9b13 ebf7  O-f...h6.iY.....
+00001170: b905 7b3c 5008 a9b6 b04c 6d6a 9847 650a  ..{<P....Lmj.Ge.
+00001180: b0dc 5c0a 18fb 97eb e0d6 8b5a 80cd f437  ..\........Z...7
+00001190: b062 650d 92e1 6fb3 02fc e887 960c 8724  .be...o........$
+000011a0: 566e b09d 1173 2b62 0025 95f2 9122 623f  Vn...s+b.%..."b?
+000011b0: 1d1c a13e 1b89 3d0c e1d7 a90a eb19 5009  ...>..=.......P.
+000011c0: f721 8611 f417 b8da d3de 368f 7c72 2e8b  .!........6.|r..
+000011d0: cebd 5033 383b 8e59 91e2 926e 7589 4e2a  ..P38;.Y...nu.N*
+000011e0: d9c2 4d1d 4f6d 30df acb5 c63c 585b d076  ..M.Om0....<X[.v
+000011f0: b3b8 f32f c594 fc05 2dc5 4de3 ffd9 52f4  .../....-.M...R.
+00001200: 7e02 1714 2b03 1d81 18ee 9605 46ba 5e9b  ~...+.......F.^.
+00001210: 1117 2ae5 c042 454a e3ae 806b 35c3 1d90  ..*..BEJ...k5...
+00001220: 2d70 3d0c 8f21 a9e0 86db fc17 e450 ffb7  -p=..!.......P..
+00001230: 3567 6598 b286 73a6 daa3 0912 14f6 2395  5ge...s.......#.
+00001240: 0a42 7681 964c f69d 22ac 5aee 5d56 242b  .Bv..L..".Z.]V$+
+00001250: 0599 8c72 cc95 8535 bb4f 0e09 eb69 0e5c  ...r...5.O...i.\
+00001260: d57b 7b84 5248 75c3 2625 0d18 dcc9 fcf3  .{{.RHu.&%......
+00001270: bf97 15d4 4f74 93f3 4fed 7c6c 319f b73d  ....Ot..O.|l1..=
+00001280: d0dd 816d b1ec fc33 f622 3587 f49d ada0  ...m...3."5.....
+00001290: 11dc fb4c 4f35 a583 d76c ece7 dc6a 2d63  ...LO5...l...j-c
+000012a0: cdad 78b9 7ee6 adb6 806b 26b8 5d56 9013  ..x.~....k&.]V..
+000012b0: 3115 31b3 2f4b f486 dae3 7bc0 ad08 de7d  1.1./K....{....}
+000012c0: d8f6 0a41 565f b28d 07d2 0469 e9b1 0f8d  ...AV_.....i....
+000012d0: 931d b4c9 a445 d986 a5ec 6e2f bc8d 821b  .....E....n/....
+000012e0: f2b2 d39d ea85 2a7d 934e f79c ce9e 3667  ......*}.N....6g
+000012f0: be3a af16 5fdf 7d9e cfd9 a587 3d5f bb9d  .:.._.}.....=_..
+00001300: 6ec0 d550 b427 4b54 b747 9383 8c09 8c79  n..P.'KT.G.....y
+00001310: cfe6 be08 e3fd fb10 e82d 78e5 3062 4ada  .........-x.0bJ.
+00001320: 9709 0fe0 5211 4e19 f6a5 0514 bf0d ae99  ....R.N.........
+00001330: baf1 1700 0000 ffff 0300 504b 0304 1400  ..........PK....
+00001340: 0600 0800 0000 2100 e97d fce0 0e03 0000  ......!..}......
+00001350: 1e08 0000 0d00 0000 786c 2f73 7479 6c65  ........xl/style
+00001360: 732e 786d 6cb4 555b 4fdb 3014 7e9f b4ff  s.xml.U[O.0.~...
+00001370: 60f9 3de4 42d3 b555 1244 5b22 2131 3409  `.=.B..U.D["!14.
+00001380: 26ed d54d 9cd6 c297 c871 59ca b4ff bee3  &..M.....qY.....
+00001390: 386d 038c 8db1 eda5 b58f edef 5cbe ef9c  8m..........\...
+000013a0: 2467 ade0 e89e ea86 2999 e2f0 24c0 88ca  $g......)...$...
+000013b0: 4295 4cae 53fc f936 f726 1835 86c8 9270  B.L.S..6.&.5...p
+000013c0: 2569 8a77 b4c1 67d9 fb77 4963 769c de6c  %i.w..g..wIcv..l
+000013d0: 2835 0820 6493 e28d 31f5 ccf7 9b62 4305  (5. d...1....bC.
+000013e0: 694e 544d 259c 544a 0b62 60ab d77e 536b  iNTM%.TJ.b`..~Sk
+000013f0: 4aca c63e 12dc 8f82 60ec 0bc2 2476 0833  J..>....`...$v.3
+00001400: 51bc 0644 107d b7ad bd42 899a 18b6 629c  Q..D.}...B....b.
+00001410: 995d 8785 9128 6697 6ba9 3459 7108 b50d  .]...(f.k.4Yq...
+00001420: 47a4 406d 38d6 d1de 4367 7ae6 44b0 42ab  G.@m8...Cgz.D.B.
+00001430: 4655 e604 407d 5555 aca0 cf63 9dfa 539f  FU..@}UU...c..S.
+00001440: 1447 2480 7d1b 5218 fb41 e412 cf12 b915  .G$.}.R..A......
+00001450: b930 0d2a d456 1a20 00ef 4dc8 9d5c 9660  .0.*.V. ..M..\.`
+00001460: 1c8f 3072 755c a812 320b 4e82 20c0 7e96  ..0ru\..2.N. .~.
+00001470: f8fd f32c a994 3ca2 d87c 6df2 b33b a9be  ...,..<..|m..;..
+00001480: cadc 1e39 687b 2b4b 9a07 744f 3858 428b  ...9h{+K..tO8XB.
+00001490: 5128 ae34 3240 1a20 7716 4904 7537 1684  Q(.42@. w.I.u7..
+000014a0: b395 66f6 5a45 04e3 3b67 8eac a1e3 b9bf  ..f.ZE..;g......
+000014b0: 2718 54bd 0bc8 7978 e2a7 8bf5 7ff8 f1bb  '.T...yx........
+000014c0: b421 38c6 f9a1 8611 d4d0 1ab2 0404 62a8  .!8...........b.
+000014d0: 9639 6c50 bfbe ddd5 90a6 042d bb70 bb7b  .9lP.......-.p.{
+000014e0: bfb9 bdd6 6417 46f1 e081 df39 cc92 95d2  ....d.F....9....
+000014f0: 25f4 ce90 3d67 ca12 4e2b 0355 d26c bdb1  %...=g..N+.U.l..
+00001500: ff46 d5f0 bb52 c680 c4b2 a464 64ad 24e1  .F...R.....dd.$.
+00001510: 96c3 fd8b 7ed1 0025 94f3 1bdb 5f5f aa47  ....~..%....__.G
+00001520: d86d 3550 0574 aacd de0a c42e 2191 7ee9  .m5P.t......!.~.
+00001530: f0dc c6e2 0fd1 1cf6 0076 04c5 fa73 58d4  .........v...sX.
+00001540: 5607 fc97 5e87 2f06 7578 8d48 5df3 9dd5  V...^./.ux.H]...
+00001550: 67af bc7f 86e5 90cf 395b 4b41 f78d 0562  g.......9[KA...b
+00001560: 765b b451 9a3d 805b db05 059c 5327 deb6  v[.Q.=.[....S'..
+00001570: 7a52 8cbe f35c 955f 9dd0 f556 aca8 cebb  zR...\._...V....
+00001580: c167 137b 9ce6 db43 eb98 04ee 0602 7924  .g.{...C......y$
+00001590: 8f03 d1c8 7670 8aaf 6d04 1c66 414f 165a  ....vp..m..fAO.Z
+000015a0: 6d19 374c fe44 1a80 59b6 47b1 750d 6bec  m.7L.D..Y.G.u.k.
+000015b0: 18ed 6478 f002 422b 6945 b6dc dc1e 0e53  ..dx..B+iE.....S
+000015c0: 7c5c 7fa4 25db 8ae9 e1d6 2776 af4c 0791  |\..%.....'v.L..
+000015d0: e2e3 faca f644 38b6 fd44 5b73 d5c0 4882  .....D8..D[s..H.
+000015e0: 7fb4 d52c c5df 2ee6 1fa6 cb8b 3cf2 26c1  ...,........<.&.
+000015f0: 7ce2 8d4e 69ec 4de3 f9d2 8b47 8bf9 7299  |..Ni.M....G..r.
+00001600: 4f83 2858 7c1f ccf3 bf98 e6dd b707 180f  O.(X|...........
+00001610: 47b3 86c3 ccd7 7db2 7d8a 3747 5b8a 071b  G.....}.}.7G[...
+00001620: 177e 370d 20ec 61ec d368 1c9c c761 e0e5  .~7. .a..h...a..
+00001630: a741 e88d c664 e24d c6a7 b197 c761 b41c  .A...d.M.....a..
+00001640: 8fe6 1771 1e0f 628f dff8 fd08 fc30 dc7f  ...q..b......0..
+00001650: 3fda 309e 1926 2867 72cf d59e a1a1 1548  ?.0..&(gr......H
+00001660: 82ed 2f92 f0f7 4cf8 c70f 7bf6 0300 00ff  ../...L...{.....
+00001670: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001680: 0039 2bb5 e89a 0200 00ad 0500 0018 0000  .9+.............
+00001690: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+000016a0: 6865 6574 312e 786d 6c8c 945b 6fdb 2014  heet1.xml..[o. .
+000016b0: c7df 27ed 3b20 deeb 5bd3 b489 9254 6ab3  ..'.; ..[....Tj.
+000016c0: 6c93 b669 5a76 79c6 f838 4635 3e1e 90a4  l..iZvy..8F5>...
+000016d0: e9a7 df01 db69 ab74 555f 0c98 c3ef fccf  .....i.tU_......
+000016e0: 0566 d7f7 ba66 3b30 5661 33e7 6994 7006  .f...f;0Va3.i.p.
+000016f0: 8dc4 4235 9b39 fff5 7375 76c5 9975 a229  ..B5.9..suv..u.)
+00001700: 448d 0dcc f901 2cbf 5ebc 7f37 dba3 b9b3  D.....,.^..7....
+00001710: 1580 6344 68ec 9c57 ceb5 d338 b6b2 022d  ..cDh..W...8...-
+00001720: 6c84 2d34 b453 a2d1 c2d1 d26c 62db 1a10  l.-4.S.....lb...
+00001730: 4538 a4eb 384b 9271 ac85 6a78 4798 9ab7  E8..8K.q..jxG...
+00001740: 30b0 2c95 8425 caad 86c6 7510 03b5 70a4  0.,..%....u...p.
+00001750: df56 aab5 034d cbb7 e0b4 3077 dbf6 4ca2  .V...M....0w..L.
+00001760: 6e09 91ab 5ab9 4380 72a6 e5f4 f3a6 4123  n...Z.C.r.....A#
+00001770: f29a e2be 4f47 420e ecb0 38c1 6b25 0d5a  ....OGB...8.k%.Z
+00001780: 2c5d 44b8 b813 7a1a f324 9ec4 445a cc0a  ,]D...z..$..DZ..
+00001790: 4511 f8b4 3303 e59c dfa4 d30f 298f 17b3  E...3.......)...
+000017a0: 909f df0a f6f6 c99c d90a f71f 8d2a bea8  .............*..
+000017b0: 0628 d954 2627 f235 d420 1d14 5438 ce1e  .(.T&'.5. ..T8..
+000017c0: 10f5 5a0a 2f36 4d2f 9eac bff9 12d4 fd5f  ..Z./6M/......._
+000017d0: 5fb6 1cf1 ce3b f84c 0713 5262 03c6 2b11  _....;.L..Rb..+.
+000017e0: d2a9 1ddc 424d e6ab d497 fe6f 10e7 e724  ....BM.....o...$
+000017f0: 2d3e 6a7b 3a1f 74ae 42a9 bf1b 960b 0bb7  ->j{:.t.B.......
+00001800: 58ff 5185 abc8 2d69 2da0 14db da3d fe9c  X.Q...-i-....=..
+00001810: 44e9 2819 6724 b3df fa81 fb4f a036 95a3  D.(.g$.....O.6..
+00001820: 0359 7449 1b21 c9d3 e2b0 042b a9d4 2435  .YtI.!.....+..$5
+00001830: cabc 0889 3579 a42f d3ca b72c 554a dc87  ....5y./...,UJ..
+00001840: 71df 3b1c 1fe1 d61d 423e 3893 5beb 500f  q.;.....B>8.[.P.
+00001850: 927a 4e47 c87a c239 6703 2189 46d9 c5e5  .zNG.z.9g.!.F...
+00001860: 55ea 05f6 0cda 7d85 31ea 1934 0e0c 3ad0  U.....}.1..4..:.
+00001870: 1f25 07af 1c25 1721 001a 87a3 172f 0490  .%...%.!...../..
+00001880: 8375 2be5 d3f3 2a6d 3c08 b93c e21e 73fd  .u+...*m<..<..s.
+00001890: a674 8ca8 ec5d 46c7 e757 8ff1 bc40 f11d  .t...]F..W...@..
+000018a0: d155 23f4 c552 38b1 9819 dc33 bac9 a4d2  .U#..R8....3....
+000018b0: b6c2 bf0b d9f4 7fc5 a42a 7ad3 1b6f 4b76  .........*z..oKv
+000018c0: d4d2 736e a91f 778b 6416 ef3c bcb7 b83d  ..sn..w.d..<...=
+000018d0: b548 9f5b 2c4f 2db2 e716 74b9 bc17 fa1e  .H.[,O-...t.....
+000018e0: bd9c 1f2d 6252 3db4 7417 462b 36f0 5598  ...-bR=.t.F+6.U.
+000018f0: 8d6a 2cab a10c ed47 2935 5d8b 2611 cd1d  .j,....G)5].&...
+00001900: b6be 297d afe6 e8a8 bb86 5545 af1c 5060  ..)}......UE..P`
+00001910: 4944 3d50 22ba 6141 09f3 dc35 b86d cb5a  ID=P".aA...5.m.Z
+00001920: d182 59ab 07ba af13 ced0 286a f2f0 8ccd  ..Y.......(j....
+00001930: 798b c619 a15c b873 c787 76f1 0f00 00ff  y....\.s..v.....
+00001940: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001950: 00e9 253b 38f3 0000 004f 0100 0018 0028  ..%;8....O.....(
+00001960: 0063 7573 746f 6d58 6d6c 2f69 7465 6d50  .customXml/itemP
+00001970: 726f 7073 322e 786d 6c20 a224 0028 a020  rops2.xml .$.(. 
+00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019a0: 0064 90c1 6ac3 3010 44ef 85fc 83d1 dd96  .d..j.0.D.......
+000019b0: 92b8 691d 6c07 27aa 21d7 d240 af42 5ec7  ..i.l.'.!..@.B^.
+000019c0: 024b 6bb4 7268 29fd f7ca f494 f6b4 cc0e  .Kk.rh).........
+000019d0: 3b6f d8f2 f061 c7e4 069e 0cba 8aad 33c1  ;o...a........3.
+000019e0: 1270 1a3b e3ae 15bb bcb5 e933 4b28 28d7  .p.;.......3K((.
+000019f0: a911 1d54 cc21 3bd4 ab87 b2a3 7da7 82a2  ...T.!;.....}...
+00001a00: 801e ce01 6c12 1726 ceb3 acd8 57fb d41c  ....l..&....W...
+00001a10: 8b62 27d2 75b3 1169 2ee4 296d 1e65 9ebe  .b'.u..i..)m.e..
+00001a20: c85c 88a2 d8b6 b23d 7db3 24a2 5d8c a18a  .\.....=}.$.]...
+00001a30: 0d21 4c7b ce49 0f60 1565 3881 8b66 8fde  .!L{.I.`.e8..f..
+00001a40: aa10 a5bf 72ec 7ba3 41a2 9e2d b8c0 3742  ....r.{.A..-..7B
+00001a50: ecb8 9e23 debe db91 d54b 9fdf eb57 e8e9  ...#.....K...W..
+00001a60: 5e2e d566 6ffe 51ac d11e 09fb 9069 b49c  ^..fo.Q......i..
+00001a70: 06e5 6142 13c3 6f5b aed1 85c8 099f 13f0  ..aB..o[........
+00001a80: a506 315e 97fc 0f64 d177 4fa8 7f00 0000  ..1^...d.wO.....
+00001a90: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00001aa0: 2100 559f 35f5 d409 0000 8c30 0000 1300  !.U.5......0....
+00001ab0: 2800 6375 7374 6f6d 586d 6c2f 6974 656d  (.customXml/item
+00001ac0: 312e 786d 6c20 a224 0028 a020 0000 0000  1.xml .$.(. ....
+00001ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ae0: 0000 0000 0000 0000 0000 0000 00ec 5bdd  ..............[.
+00001af0: 929b 4616 be4f 55de 81d2 5e33 8040 0254  ..F..OU...^3.@.T
+00001b00: 9653 638d bdeb 8a1d bb32 daec dea5 9aa6  .Sc......2......
+00001b10: 19b1 4680 e966 4653 a97d a47d 8abc 584e  ..F..fFS.}.}..XN
+00001b20: 77f3 8f7e 004d 36a9 ad4d 2e32 9238 a74f  w..~.M6..M.2.8.O
+00001b30: 9fff f31d f2ea bbc3 3e52 1e49 46c3 245e  ........>R.IF.$^
+00001b40: cf8c 1b7d a690 1827 7e18 3fac 6739 0b54  ...}...'~.?.g9.T
+00001b50: 67f6 ddeb 5798 ad70 1233 12b3 ed73 4aee  g...W..p.3...sJ.
+00001b60: f18e ec91 025f febc 9ecd 943d aafe db78  ....._.....=...x
+00001b70: e807 b427 ebd9 5d82 f33d 9025 e2b1 c6cf  ...'..]..=.%....
+00001b80: efef d633 fda0 1bf0 affe ce34 0dc3 7db3  ...3.......4..}.
+00001b90: 9c6f 4c7b 6159 ae7b 676f de59 cead bbb9  .oL{aY.{go.Y....
+00001ba0: 7396 ce62 d9a5 fda9 12d7 e8fe 7447 28ce  s..b........tG(.
+00001bb0: c294 89db 6c32 8232 25ce c963 a2f8 a520  ....l2.2%..c... 
+00001bc0: 375d 927b 9ca4 20a9 f8ba 5004 17ce 70e6  7].{.. ...P...p.
+00001bd0: fe7c ae9b ba67 064b d35d ce1d 8275 ec2c  .|...g.K.]...u.,
+00001be0: dc39 b65c dd01 3d81 e662 bac2 6c3d db31  .9.\..=..b..l=.1
+00001bf0: 96ae 348d 0abd d09b 7d88 b384 2601 bbc1  ..4.....}...&...
+00001c00: c95e 4b82 20c4 449b ebfa 52db 1386 7cc4  .^K. .D...R...|.
+00001c10: 90d6 d044 c968 8fa6 304a 3390 3e63 21a1  ...D.h..0J3.>c!.
+00001c20: 82f9 2d63 59e8 e58c d0d9 eb6f bf79 75a0  ..-cY......o.yu.
+00001c30: fe4a 4aa5 3094 3d10 c6ad 4253 84e1 c2e3  .JJ.0.=...BS....
+00001c40: 85ae cf12 caca 9204 eece b29c 888f 4148  ..............AH
+00001c50: 229f 0abb 9aae 6393 00e9 a66b 390b cf31  ".....c....k9..1
+00001c60: 75dd f43d ecba f3b9 4d40 a733 25a6 73e9  u..=....M@.3%.s.
+00001c70: 3331 35e5 1f52 9920 6f25 d8d3 d3d3 cd93  315..R. o%......
+00001c80: 7993 640f 5c77 86f6 cf8f 1fa4 e395 0a3b  y.d.\w.........;
+00001c90: d0e1 cfa6 d7de 57ca 0772 af67 9ead 2fd1  ......W..r.g../.
+00001ca0: 3230 55dd 0e3c d5f2 4c47 7516 fa42 45b6  20U..<..LGu..BE.
+00001cb0: bd58 62c7 703d 0b95 32c2 fdc0 cf0d c740  .Xb.p=..2......@
+00001cc0: fec2 5617 ee62 ae5a 3afc 8502 14a8 b66e  ..V..b.Z:......n
+00001cd0: 221f 5ccc 45d8 a9cc 15ee d324 634a 5c1b  ".\.E......$cJ\.
+00001ce0: 6ad0 795a 69ee 3efd a0e3 2b7a 1211 1eb0  j.yZi.>...+z....
+00001cf0: 4280 f5ac 61f2 f200 f0e9 3422 079e 082a  B...a.....4"...*
+00001d00: 1723 5f73 c81a d5e7 368f 32f4 3ea2 183d  .#_s....6.2.>..=
+00001d10: 08e6 d565 8ff0 4251 54b2 2dd9 6424 58cf  ...e..BQT.-.d$X.
+00001d20: b8cb 7c24 7e88 ee49 f608 01f5 b108 25f0  ..|$~..I......%.
+00001d30: bd30 fe84 719e 813b e8b3 de3d 8e12 bf43  .0..q..;...=...C
+00001d40: 945d c5e0 1e32 0bde 7dae 826f b014 110e  .]...2..}..o....
+00001d50: ec65 602c 1698 f896 ef63 cfd2 5ddb 30ad  .e`,.....c..].0.
+00001d60: 2030 b169 ce83 818c ccd5 161d 3688 e1dd   0.i........6...
+00001d70: 6d14 4d52 c1a7 cd8f 93e8 fe4a 6292 219e  m.MR.......Jb.!.
+00001d80: 60b7 e19e 47fe 78ed bf7d 0407 fb1b a2bb  `...G.x..}......
+00001d90: 4de2 0fe5 60ae ee77 2823 fe3f 42b6 fb3b  M...`..w(#.?B..;
+00001da0: 8502 3058 5135 dd1d b84c 181d a5d4 78a6  ..0XQ5...L....x.
+00001db0: 2c5c 4ffc ddf1 4cf1 5de1 8fdc 3dc5 67da  ,\O...L.]...=.g.
+00001dc0: 70fb e144 a248 5c4a cec3 724c 21d0 bb24  p..D.H\J..rL!..$
+00001dd0: dbdf 41be cd23 c8c7 5f73 1485 908b fd3a  ..A..#.._s.....:
+00001de0: 4dfe 4e39 d5df d709 f872 e9eb 6701 8d41  M.N9.....r..g..A
+00001df0: 0a01 6bc8 d49a e261 293a 8c83 2445 6cc7  ..k....a):..$El.
+00001e00: 8b82 ad7d 4619 037f dc40 7392 2560 dad3  ...}F....@s.%`..
+00001e10: 5970 70b9 3b29 e899 143b 84f9 79c1 4fe4  Ypp.;)...;..y.O.
+00001e20: df13 190f adc2 d827 87f5 cc81 5a1a 4611  .......'....Z.F.
+00001e30: f222 a8e8 5529 f643 9a46 e859 b660 2759  ."..U).C.F.Y.`'Y
+00001e40: ec42 df27 d0f4 5564 2174 7859 8ca2 0b74  .B.'..Ud!txY...t
+00001e50: d055 f99f e2e8 b9a0 ac5c 192a 4f44 9a65  .U.......\.*OD.e
+00001e60: 2123 14ba 11cc 7385 e221 0a12 82cb ac7e  !#....s..!.....~
+00001e70: 4818 9169 5a06 518b ac1b 673c 2cdb d5a4  H..iZ.Q...g<,...
+00001e80: 799d 4e1a afb4 e28e d34a 8fcd 08cd f468  y.N......J.....h
+00001e90: ff3c da39 52a3 2a0d 19bc 091b e138 4779  .<.9R.*......8Gy
+00001ea0: 8d50 d351 fa3f 5655 032a 71ad aef9 5175  .P.Q.?VU.*q...Qu
+00001eb0: 3174 48e2 645f 4602 9f84 da31 34e8 8c92  1tH.d_F....14...
+00001ec0: cb3b de40 f763 effd 1eba a62d 7ae0 750b  .;.@.c.....-z.u.
+00001ed0: ad5a a1fd 9685 d078 3144 159f 2821 7f2e  .Z.....x1D..(!..
+00001ee0: 969d 7915 a101 8a68 a33d 7f0f a5e0 9745  ..y....h.=.....E
+00001ef0: d182 a8bc 0751 7913 a2f2 2e44 6db6 21ff  .....Qy....Dm.!.
+00001f00: 167c 4ac9 3e42 6509 1b89 82d2 9473 b2bd  .|J.>Be......s..
+00001f10: 856e 3b84 a8ae eb41 238c 3d5d 45c4 7655  .n;....A#.=]E.vU
+00001f20: 7f1e 58c4 b47d 3770 2cc9 8764 fb7b c238  ..X..}7p,..d.{.8
+00001f30: 8dee 3a86 857d 535d 2c1d a206 c4d5 55fe  ..:..}S],.....U.
+00001f40: 8dea f8cb b911 044e e015 3428 c6bb 24e3  .......N..4(..$.
+00001f50: 2481 8716 56e0 992a 3689 0124 8ec1 5bed  $...V..*6..$..[.
+00001f60: a58a 91e5 2d5d c372 b005 c50e 7403 9350  ....-].r....t..P
+00001f70: 2b9d d1ef c9f3 5392 7116 420d 133a 58d1  +.....S.q.B..:X.
+00001f80: 3da6 78b5 851b 741b 0738 f250 369e c6ec  =.x...t..8.P6...
+00001f90: b5ec 09ae ed11 ce27 3cd9 b4d5 6e09 eabd  .......'<...n...
+00001fa0: 14c5 6f0f 2c43 9811 5fd9 9203 137a 3a9d  ..o.,C.._....z:.
+00001fb0: e74b fe2f 1199 a5b6 414b 1f48 fcc0 76ca  .K./....AK.H..v.
+00001fc0: 238a 7228 02f3 c5a2 91ff 1b45 a26e acae  #.r(.......E.n..
+00001fd0: a809 bdfe b4d6 d662 5cce 3bc2 6944 c63b  .......b\.;.iD.;
+00001fe0: 427d a556 85fd 449f 7075 e1ec 76e0 b58e  B}.V..D.pu..v...
+00001ff0: 006c 1953 17fa 8c46 a8a8 4ffc dfd4 9054  .l.S...F..O....T
+00002000: e2a0 6e7c d004 adfc bf1b ff5f efc6 db33  ..n|......._...3
+00002010: 771d 34e6 e5a0 0152 d12a 2862 6857 606a  w.4....R.*(bhW`j
+00002020: 5736 4994 ef65 c1ee 054d 1452 98e5 7e31  W6I..e...M.R..~1
+00002030: 6cdd d603 ecab 73db 41aa 45a0 647a 4bc3  l.....s.A.E.dzK.
+00002040: 531d 2f98 07b6 6f99 b6b5 90a5 ba9d d3bb  S./...o.........
+00002050: 82d2 5df2 24da 8bf5 ac04 0dee 0086 14d5  ..].$...........
+00002060: e089 7823 21aa 23a8 4df1 159f c360 b6af  ..x#!.#.M....`..
+00002070: 009c 037c e2c8 72a3 fd17 bdc4 6697 0084  ...|..r.....f...
+00002080: f321 49be e469 0d54 9e45 917e e2c5 63a6  .!I..i.T.E.~..c.
+00002090: f099 51ce 1105 75b3 0ae7 b197 e430 18f1  ..Q...u......0..
+000020a0: 76a0 094b 7453 5a23 8976 4778 a891 52e4  v..KtSZ#.vGx..R.
+000020b0: aa18 f5af 3664 d6ef d7f1 3e7e 513b 907d  ....6d....>~Q;.}
+000020c0: d981 3600 bbc1 b01b fa89 02e0 f191 3a7e  ..6...........:~
+000020d0: 8cff 897c 7a95 0139 fa22 8c38 d070 fcf9  ...|z..9.".8.p..
+000020e0: f730 b477 6dd2 e89e 6abb 4d06 19ef ea91  .0.wm...j.M.....
+000020f0: b774 1201 7ec3 001a 3f5c c28a 38d8 ba9e  .t..~...?\..8...
+00002100: dd62 0cde 035d 6ad3 cb84 f483 fca9 6ff1  .b...]j.......o.
+00002110: 8221 1f89 87c9 7405 aaf4 47f8 718d a7d5  .!....t...G.q...
+00002120: 9e3c 0090 e064 5144 c4d0 9253 eece a567  .<...dQD...S...g
+00002130: 9ff5 eae6 697f eafe 7444 63d1 c18d f800  ....i...tDc.....
+00002140: 0368 5800 781e 6254 ac3e 6057 f305 e6ba  .hX.x.bT.>`W....
+00002150: defa 2823 6a73 1d73 a1f7 40e5 5aa8 0515  ..(#js.s..@.Z...
+00002160: e671 032c f4a2 047f a950 c4bf 8085 0a64  .q.,.....P.....d
+00002170: ae07 cb4d 9772 d292 0706 cf42 4d27 3742  ...M.r.....BM'7B
+00002180: 6a18 5306 0323 8499 3cc2 afc1 c434 cf22  j.S..#..<....4."
+00002190: a149 1f6b 8596 a866 dc18 5afd 2ca0 5e0d  .I.k...f..Z.,.^.
+000021a0: 28b3 4920 7ea9 9e4c 001a bc00 5296 6558  (.I ~..L....R.eX
+000021b0: 4b3c ff32 1879 4636 09a8 7e48 b080 daab  K<.2.yF6..~H....
+000021c0: 53fd dc8b 42d8 cf66 44dc a980 5d35 b835  S...B..fD...]5.5
+000021d0: d5be c20d 0114 3535 ddd2 f4b9 e6e3 1b48  ......55.......H
+000021e0: 49f5 42a4 bf18 2ad4 7aec c22f 71bc 505e  I.B...*.z../q.P^
+000021f0: 5b86 3694 c7af d15c a1c8 dabe d9fe dcf9  [.6....\........
+00002200: a1c2 461b 75ab d84f f51f 2e2b c8a9 3d92  ..F.u..O...+..=.
+00002210: 8f57 18d2 074b b233 05c9 38b1 47f2 6190  .W...K.3..8.G.a.
+00002220: 065f 911c fa6d 460b 1038 be89 82e3 4340  ._...mF..8....C@
+00002230: 5d19 87e8 474a 20ab 546b 73dc ee72 5ac7  ]...GJ .Tks..rZ.
+00002240: 179d 52ab 0856 691a d0bf 2e96 b40d 53d8  ..R..Vi.......S.
+00002250: 9213 de5c 4007 046d c649 15ac 58c8 a2ee  ...\@..m.I..X...
+00002260: dea6 0d86 4824 4c20 d412 016a c156 db5f  ....H$L ...j.V._
+00002270: ffc3 f2e8 cc01 34f7 fe45 3007 2b5a 5ddc  ......4..E0.+Z].
+00002280: 30f5 faf5 2b00 e318 48fd 7e91 98d1 79b0  0...+...H.~...y.
+00002290: a7af dc93 d68e 50fc 9043 069f 220b 043f  ......P..C.."..?
+000022a0: 7948 b2e7 b3b4 0364 9137 2b5e 6e78 1966  yH.....d.7+^nx.f
+000022b0: 1979 0c79 673f 925b 159d 719c 3091 daca  .y.yg?.[..q.0...
+000022c0: 6fca b54b f9a5 72e2 9fed 2ea4 1249 5260  o..K..r......IR`
+000022d0: 0712 7215 5185 ed08 bce7 b1f7 48a6 2481  ..r.Q.......H.$.
+000022e0: 42d1 237c 9764 4a29 24bd 51b6 f004 4ad3  B.#|.dJ)$.Q...J.
+000022f0: 8813 f081 0498 00f2 9426 309e c0ee 4481  .........&0...D.
+00002300: 92ab e429 bc9a 01dd 2270 ab8e 4001 04bc  ...)...."p..@...
+00002310: 4210 de55 cc6e befd e698 6812 feeb de42  B..U.n....h....B
+00002320: 7e8b 5ab7 bdbc e388 f87a 1ade c1e1 6bbc  ~.Z......z....k.
+00002330: 3757 5b5f 6098 65e6 da17 6c27 b9a3 9cee  7W[_`.e...l'....
+00002340: eec1 70f9 a4f8 18b4 6595 a547 bac5 552f  ..p.....e..G..U/
+00002350: af9c 5fb8 5d82 6b06 b44c 2fb9 b82c 1a97  .._.].k..L/..,..
+00002360: 41ef b414 ba69 17d3 cfb0 1387 702c 7eeb  A....i......p,~.
+00002370: 4d78 abe6 b2fa 40ab a55a 0970 b7e6 a756  Mx....@..Z.p...V
+00002380: da15 c076 f97c e7e8 92ba 313a 4da5 9553  ...v.|....1:M..S
+00002390: d279 6af0 9fd6 3df8 e7fe a2fe 84ac 3209  .yj...=.......2.
+000023a0: 1e9d 1357 7c4f 0963 e2b9 ab9e 9811 b944  ...W|O.c.......D
+000023b0: 2389 dbf3 e070 f237 779b 5b4a 131c 42ca  #....p.7w.[J..B.
+000023c0: f3df 420b c19e 279b 1b78 151c 4ed7 d8c6  ..B...'..x..N...
+000023d0: 54ce d358 53ad 5d43 c0af 55bc 40a2 84d7  T..XS.]C..U.@...
+000023e0: 7560 6722 0fa8 de38 2bb4 5b3d 57b8 d239  u`g"...8+.[=W..9
+000023f0: bac1 24f7 cf94 91fd fb62 0ae0 470e 262d  ..$......b..G.&-
+00002400: 550a 45e1 14dd 2037 abef 213d a57b fbaa  U.E... 7..!=.{..
+00002410: 4cb7 0d7e 5a1d 5d36 3584 308e c311 dd4c  L..~Z.]65.0....L
+00002420: 94a5 abaa 816c da79 aaf6 bca9 a94a 6af6  .....l.y.....Jj.
+00002430: ba84 2579 940e f323 0948 c65f 60eb 54c5  ..%y...#.H._`.T.
+00002440: 21a9 afe0 e4f3 5751 9bdd ea18 5ad8 2e4f  !.....WQ....Z..O
+00002450: a605 ec79 322d efcd a7ca 0ccb b4df 3d59  ...y2-........=Y
+00002460: 1fb1 b49c 11c7 64dd 93a6 9ecc 8adb 7a3a  ......d.......z:
+00002470: 3118 7b3a 3158 7b3a 3198 7b3a 31d8 7b3c  1.{:1X{:1.{:1.{<
+00002480: b15c 9b4f 0d74 4e3d 1c39 be54 a326 340b  .\.O.tN=.9.T.&4.
+00002490: 9500 d7dc 4054 95f1 7126 ceee 02cf bda4  ....@T..q&......
+000024a0: f202 1d11 3f48 ca38 cdbe 355e 7e26 2a85  ....?H.8..5^~&*.
+000024b0: 9cd5 ae55 3bf6 ff13 bcfe 0d00 00ff ff03  ...U;...........
+000024c0: 0050 4b03 0414 0006 0008 0000 0021 0074  .PK..........!.t
+000024d0: 3f39 7ac2 0000 0028 0100 001e 0008 0163  ?9z....(.......c
+000024e0: 7573 746f 6d58 6d6c 2f5f 7265 6c73 2f69  ustomXml/_rels/i
+000024f0: 7465 6d31 2e78 6d6c 2e72 656c 7320 a204  tem1.xml.rels ..
+00002500: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
 00002510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002570: 0000 0000 0000 0084 925d 4bc3 3018 85ef  .........]K.0...
-00002580: 05ff 43c9 7d9b b6d3 4e43 dbc1 945d 3910  ..C.}...NC...]9.
-00002590: dc50 bc0b c9bb add8 7c90 6476 fbf7 a6ed  .P......|.dv....
-000025a0: 56ab 1384 dc24 e7e4 c939 2fc9 6707 5107  V....$...9/.g.Q.
-000025b0: 9f60 6ca5 6481 9228 4601 48a6 7825 b705  .`l.d..(F.H.x%..
-000025c0: 5aaf 16e1 1d0a aca3 92d3 5a49 28d0 112c  Z.........ZI(..,
-000025d0: 9a95 d757 39d3 8429 03cf 4669 30ae 021b  ...W9..)..Fi0...
-000025e0: 7892 b484 e902 ed9c d304 63cb 7620 a88d  x.........c.v ..
-000025f0: bc43 7a71 a38c a0ce 6fcd 166b ca3e e816  .Czq....o..k.>..
-00002600: 701a c719 16e0 28a7 8ee2 1618 ea81 884e  p.....(........N
-00002610: 48ce 06a4 de9b ba03 7086 a106 01d2 599c  H.......p.....Y.
-00002620: 4409 fef6 3a30 c2fe 79a1 5346 4e51 b9a3  D...:0..y.SFNQ..
-00002630: f69d 4e71 c76c ce7a 7170 1f6c 3518 9ba6  ..Nq.l.zqp.l5...
-00002640: 899a 4917 c3e7 4ff0 dbf2 e9a5 ab1a 56b2  ..I...O.......V.
-00002650: 9d15 0354 e69c 1166 803a 65ca b9d9 4b15  ...T...f.:e...K.
-00002660: 2c8c 5754 8e47 423b c49a 5ab7 f4f3 de54  ,.WT.GB;..Z....T
-00002670: c0e7 c75f de4b dd73 bb1a 3d1c 78e0 8391  ..._.K.s..=.x...
-00002680: bec6 5979 9d3c 3cae 16a8 4ce3 7412 c67e  ..Yy.<<...L.t..~
-00002690: 65ab 644a 6eee 4932 7d6f 9fff 71bf 0dda  e.dJn.I2}o..q...
-000026a0: 1f88 5388 7f89 5918 272d 31ce 487a 3b22  ..S...Y.'-1.Hz;"
-000026b0: 9e01 658e 2f3e 47f9 0500 00ff ff03 0050  ..e./>G........P
-000026c0: 4b03 0414 0006 0008 0000 0021 0055 9f35  K..........!.U.5
-000026d0: f5d4 0900 008c 3000 0013 0028 0063 7573  ......0....(.cus
-000026e0: 746f 6d58 6d6c 2f69 7465 6d32 2e78 6d6c  tomXml/item2.xml
-000026f0: 20a2 2400 28a0 2000 0000 0000 0000 0000   .$.(. .........
-00002700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002710: 0000 0000 0000 0000 ec5b dd92 9b46 16be  .........[...F..
-00002720: 4f55 de81 d25e 3380 4002 5496 5363 8dbd  OU...^3.@.T.Sc..
-00002730: eb8a 1dbb 32da ecde a59a a619 b146 80e9  ....2........F..
-00002740: 6646 53a9 7da4 7d8a bc58 4e77 f38f 7e00  fFS.}.}..XNw..~.
-00002750: 4d36 a9ad 4d2e 3292 38a7 4f9f fff3 1df2  M6..M.2.8.O.....
-00002760: eabb c33e 521e 4946 c324 5ecf 8c1b 7da6  ...>R.IF.$^...}.
-00002770: 9018 277e 183f ac67 390b 5467 f6dd eb57  ..'~.?.g9.Tg...W
-00002780: 98ad 7012 3312 b3ed 734a eef1 8eec 9102  ..p.3...sJ......
-00002790: 5ffe bc9e cd94 3daa fedb 78e8 07b4 27eb  _.....=...x...'.
-000027a0: d95d 82f3 3d90 25e2 b1c6 cfef efd6 33fd  .]..=.%.......3.
-000027b0: a01b f0af fece 340d c37d b39c 6f4c 7b61  ......4..}..oL{a
-000027c0: 59ae 7b67 6fde 59ce adbb b973 96ce 62d9  Y.{go.Y....s..b.
-000027d0: a5fd a912 d7e8 fe74 4728 cec2 9489 db6c  .......tG(.....l
-000027e0: 3282 3225 cec9 63a2 f8a5 2037 5d92 7b9c  2.2%..c... 7].{.
-000027f0: a420 a9f8 ba50 0417 ce70 e6fe 7cae 9bba  . ...P...p..|...
-00002800: 6706 4bd3 5dce 1d82 75ec 2cdc 39b6 5cdd  g.K.]...u.,.9.\.
-00002810: 013d 81e6 62ba c26c 3ddb 3196 ae34 8d0a  .=..b..l=.1..4..
-00002820: bdd0 9b7d 88b3 8426 01bb c1c9 5e4b 8220  ...}...&....^K. 
-00002830: c444 9beb fa52 db13 867c c490 d6d0 44c9  .D...R...|....D.
-00002840: 688f a630 4a33 903e 6321 a182 f92d 6359  h..0J3.>c!...-cY
-00002850: e8e5 8cd0 d9eb 6fbf 7975 a0fe 4a4a a530  ......o.yu..JJ.0
-00002860: 943d 10c6 ad42 5384 e1c2 e385 aecf 12ca  .=...BS.........
-00002870: ca92 04ee ceb2 9c88 8f41 4822 9f0a bb9a  .........AH"....
-00002880: ae63 9300 e9a6 6b39 0bcf 3175 ddf4 3dec  .c....k9..1u..=.
-00002890: baf3 b94d 40a7 3325 a673 e933 3135 e51f  ...M@.3%.s.315..
-000028a0: 5299 206f 25d8 d3d3 d3cd 9379 9364 0f5c  R. o%......y.d.\
-000028b0: 7786 f6cf 8f1f a4e3 950a 3bd0 e1cf a6d7  w.........;.....
-000028c0: de57 ca07 72af 679e ad2f d132 3055 dd0e  .W..r.g../.20U..
-000028d0: 3cd5 f24c 4775 16fa 4245 b6bd 5862 c770  <..LGu..BE..Xb.p
-000028e0: 3d0b 9532 c2fd c0cf 0dc7 40fe c256 17ee  =..2......@..V..
-000028f0: 62ae 5a3a fc85 0214 a8b6 6e22 1f5c cc45  b.Z:......n".\.E
-00002900: d8a9 cc15 eed3 2463 4a5c 1b6a d079 5a69  ......$cJ\.j.yZi
-00002910: ee3e fda0 e32b 7a12 111e b042 80f5 ac61  .>...+z....B...a
-00002920: f2f2 00f0 e934 2207 9e08 2a17 235f 73c8  .....4"...*.#_s.
-00002930: 1ad5 e736 8f32 f43e a218 3d08 e6d5 658f  ...6.2.>..=...e.
-00002940: f042 5154 b22d d964 2458 cfb8 cb7c 247e  .BQT.-.d$X...|$~
-00002950: 88ee 49f6 0801 f5b1 0825 f0bd 30fe 8471  ..I......%..0..q
-00002960: 9e81 3be8 b3de 3d8e 12bf 4394 5dc5 e01e  ..;...=...C.]...
-00002970: 320b de7d ae82 6fb0 1411 0eec 6560 2c16  2..}..o.....e`,.
-00002980: 98f8 96ef 63cf d25d db30 ad20 30b1 69ce  ....c..].0. 0.i.
-00002990: 8381 8ccc d516 1d36 88e1 dd6d 144d 52c1  .......6...m.MR.
-000029a0: a7cd 8f93 e8fe 4a62 9221 9e60 b7e1 9e47  ......Jb.!.`...G
-000029b0: fe78 edbf 7d04 07fb 1ba2 bb4d e20f e560  .x..}......M...`
-000029c0: aeee 7728 23fe 3f42 b6fb 3b85 0230 5851  ..w(#.?B..;..0XQ
-000029d0: 35dd 1db8 4c18 1da5 d478 a62c 5c4f fcdd  5...L....x.,\O..
-000029e0: f14c f15d e18f dc3d c567 da70 fbe1 44a2  .L.]...=.g.p..D.
-000029f0: 485c 4ace c372 4c21 d0bb 24db df41 becd  H\J..rL!..$..A..
-00002a00: 23c8 c75f 7314 8590 8bfd 3a4d fe4e 39d5  #.._s.....:M.N9.
-00002a10: dfd7 09f8 72e9 eb67 018d 410a 016b c8d4  ....r..g..A..k..
-00002a20: 9ae2 6129 3a8c 8324 456c c78b 82ad 7d46  ..a):..$El....}F
-00002a30: 1903 7fdc 4073 9225 60da d359 7070 b93b  ....@s.%`..Ypp.;
-00002a40: 29e8 9914 3b84 f979 c14f e4df 1319 0fad  )...;..y.O......
-00002a50: c2d8 2787 f5cc 815a 1a46 11f2 22a8 e855  ..'....Z.F.."..U
-00002a60: 29f6 439a 46e8 59b6 6027 59ec 42df 27d0  ).C.F.Y.`'Y.B.'.
-00002a70: f455 6421 7478 598c a20b 74d0 55f9 9fe2  .Ud!txY...t.U...
-00002a80: e8b9 a0ac 5c19 2a4f 449a 6521 2314 ba11  ....\.*OD.e!#...
-00002a90: cc73 85e2 210a 1282 cbac 7e48 1891 695a  .s..!.....~H..iZ
-00002aa0: 0651 8bac 1b67 3c2c dbd5 a479 9d4e 1aaf  .Q...g<,...y.N..
-00002ab0: b4e2 8ed3 4a8f cd08 cdf4 68ff 3cda 3952  ....J.....h.<.9R
-00002ac0: a32a 0d19 bc09 1be1 3847 798d 50d3 51fa  .*......8Gy.P.Q.
-00002ad0: 3f56 5503 2a71 adae f951 7531 7448 e264  ?VU.*q...Qu1tH.d
-00002ae0: 5f46 029f 84da 3134 e88c 92cb 3bde 40f7  _F....14....;.@.
-00002af0: 63ef fd1e baa6 2d7a e075 0bad 5aa1 fd96  c.....-z.u..Z...
-00002b00: 85d0 7831 4415 9f28 217f 2e96 9d79 15a1  ..x1D..(!....y..
-00002b10: 018a 68a3 3d7f 0fa5 e097 45d1 82a8 bc07  ..h.=.....E.....
-00002b20: 5179 13a2 f22e 446d b621 ff16 7c4a c93e  Qy....Dm.!..|J.>
-00002b30: 4265 091b 8982 d294 73b2 bd85 6e3b 84a8  Be......s...n;..
-00002b40: aeeb 4123 8c3d 5d45 c476 557f 1e58 c4b4  ..A#.=]E.vU..X..
-00002b50: 7d37 702c c987 64fb 7bc2 388d ee3a 8685  }7p,..d.{.8..:..
-00002b60: 7d53 5d2c 1da2 06c4 d555 fe8d eaf8 cbb9  }S],.....U......
-00002b70: 1104 4ee0 1534 28c6 bb24 e324 8187 1656  ..N..4(..$.$...V
-00002b80: e099 2a36 8901 248e c15b eda5 8a91 e52d  ..*6..$..[.....-
-00002b90: 5dc3 72b0 05c5 0e74 0393 502b 9dd1 efc9  ].r....t..P+....
-00002ba0: f353 9271 1642 0d13 3a58 d13d a678 b585  .S.q.B..:X.=.x..
-00002bb0: 1b74 1b07 38f2 5036 9ec6 ecb5 ec09 aeed  .t..8.P6........
-00002bc0: 11ce 273c d9b4 d56e 09ea bd14 c56f 0f2c  ..'<...n.....o.,
-00002bd0: 4398 115f d992 0313 7a3a 9de7 4bfe 2f11  C.._....z:..K./.
-00002be0: 99a5 b641 4b1f 48fc c076 ca23 8a72 2802  ...AK.H..v.#.r(.
-00002bf0: f3c5 a291 ff1b 45a2 6eac aea8 09bd feb4  ......E.n.......
-00002c00: d6d6 625c ce3b c269 44c6 3b42 7da5 5685  ..b\.;.iD.;B}.V.
-00002c10: fd44 9f70 75e1 ec76 e0b5 8e00 6c19 5317  .D.pu..v....l.S.
-00002c20: fa8c 46a8 a84f fcdf d490 54e2 a06e 7cd0  ..F..O....T..n|.
-00002c30: 04ad fcbf 1bff 5fef c6db 3377 1d34 e6e5  ......_...3w.4..
-00002c40: a001 52d1 2a28 6268 5760 6a57 3649 94ef  ..R.*(bhW`jW6I..
-00002c50: 65c1 ee05 4d14 5298 e57e 316c ddd6 03ec  e...M.R..~1l....
-00002c60: ab73 db41 aa45 a064 7a4b c353 1d2f 9807  .s.A.E.dzK.S./..
-00002c70: b66f 99b6 b590 a5ba 9dd3 bb82 d25d f224  .o...........].$
-00002c80: da8b f5ac 040d ee00 8614 d5e0 8978 2321  .............x#!
-00002c90: aa23 a84d f115 9fc3 60b6 af00 9c03 7ce2  .#.M....`.....|.
-00002ca0: c872 a3fd 17bd c466 9700 84f3 2149 bee4  .r.....f....!I..
-00002cb0: 690d 549e 4591 7ee2 c563 a6f0 9951 ce11  i.T.E.~..c...Q..
-00002cc0: 0575 b30a e7b1 97e4 3018 f176 a009 4b74  .u......0..v..Kt
-00002cd0: 535a 2389 7647 78a8 9152 e4aa 18f5 af36  SZ#.vGx..R.....6
-00002ce0: 64d6 efd7 f13e 7e51 3b90 7dd9 8136 00bb  d....>~Q;.}..6..
-00002cf0: c1b0 1bfa 8902 e0f1 913a 7e8c ff89 7c7a  .........:~...|z
-00002d00: 9501 39fa 228c 38d0 70fc f9f7 30b4 776d  ..9.".8.p...0.wm
-00002d10: d2e8 9e6a bb4d 0619 efea 91b7 7412 017e  ...j.M......t..~
-00002d20: c300 1a3f 5cc2 8a38 d8ba 9edd 620c de03  ...?\..8....b...
-00002d30: 5d6a d3cb 84f4 83fc a96f f182 211f 8987  ]j.......o..!...
-00002d40: c974 05aa f447 f871 8da7 d59e 3c00 90e0  .t...G.q....<...
-00002d50: 6451 44c4 d092 53ee cea5 679f f5ea e669  dQD...S...g....i
-00002d60: 7fea fe74 4463 d1c1 8df8 0003 6858 0078  ...tDc......hX.x
-00002d70: 1e62 54ac 3e60 57f3 05e6 bade fa28 236a  .bT.>`W......(#j
-00002d80: 731d 73a1 f740 e55a a805 15e6 7103 2cf4  s.s..@.Z....q.,.
-00002d90: a204 7fa9 50c4 bf80 850a 64ae 07cb 4d97  ....P.....d...M.
-00002da0: 72d2 9207 06cf 424d 2737 426a 1853 0603  r.....BM'7Bj.S..
-00002db0: 2384 993c c2af c1c4 34cf 22a1 491f 6b85  #..<....4.".I.k.
-00002dc0: 96a8 66dc 185a fd2c a05e 0d28 b349 207e  ..f..Z.,.^.(.I ~
-00002dd0: a99e 4c00 1abc 0052 9665 584b 3cff 3218  ..L....R.eXK<.2.
-00002de0: 7946 3609 a87e 48b0 80da ab53 fddc 8b42  yF6..~H....S...B
-00002df0: d8cf 6644 dca9 805d 35b8 35d5 bec2 0d01  ..fD...]5.5.....
-00002e00: 1435 35dd d2f4 b9e6 e31b 4849 f542 a4bf  .55.......HI.B..
-00002e10: 182a d47a ecc2 2f71 bc50 5e5b 8636 94c7  .*.z../q.P^[.6..
-00002e20: afd1 5ca1 c8da bed9 fedc f9a1 c246 1b75  ..\..........F.u
-00002e30: abd8 4ff5 1f2e 2bc8 a93d 928f 5718 d207  ..O...+..=..W...
-00002e40: 4bb2 3305 c938 b147 f261 9006 5f91 1cfa  K.3..8.G.a.._...
-00002e50: 6d46 0b10 38be 8982 e343 405d 1987 e847  mF..8....C@]...G
-00002e60: 4a20 ab54 6b73 dcee 725a c717 9d52 ab08  J .Tks..rZ...R..
-00002e70: 5669 1ad0 bf2e 96b4 0d53 d892 13de 5c40  Vi.......S....\@
-00002e80: 0704 6dc6 4915 ac58 c8a2 eede a60d 8648  ..m.I..X.......H
-00002e90: 244c 20d4 1201 6ac1 56db 5fff c3f2 e8cc  $L ...j.V._.....
-00002ea0: 0134 f7fe 4530 072b 5a5d dc30 f5fa f52b  .4..E0.+Z].0...+
-00002eb0: 00e3 1848 fd7e 9198 d179 b0a7 afdc 93d6  ...H.~...y......
-00002ec0: 8e50 fc90 4306 9f22 0b04 3f79 48b2 e7b3  .P..C.."..?yH...
-00002ed0: b403 6491 372b 5e6e 7819 6619 790c 7967  ..d.7+^nx.f.y.yg
-00002ee0: 3f92 5b15 9d71 9c30 91da ca6f cab5 4bf9  ?.[..q.0...o..K.
-00002ef0: a572 e29f ed2e a412 4952 6007 1272 1551  .r......IR`..r.Q
-00002f00: 85ed 08bc e7b1 f748 a624 8142 d123 7c97  .......H.$.B.#|.
-00002f10: 644a 2924 bd51 b6f0 044a d388 13f0 8104  dJ)$.Q...J......
-00002f20: 9800 f294 2630 9ec0 ee44 8192 abe4 29bc  ....&0...D....).
-00002f30: 9a01 dd22 70ab 8e40 0104 bc42 10de 55cc  ..."p..@...B..U.
-00002f40: 6ebe fde6 9868 12fe ebde 427e 8b5a b7bd  n....h....B~.Z..
-00002f50: bce3 88f8 7a1a dec1 e16b bc37 575b 5f60  ....z....k.7W[_`
-00002f60: 9865 e6da 176c 27b9 a39c eeee c170 f9a4  .e...l'......p..
-00002f70: f818 b465 95a5 47ba c555 2faf 9c5f b85d  ...e..G..U/.._.]
-00002f80: 826b 06b4 4c2f b9b8 2c1a 9741 efb4 14ba  .k..L/..,..A....
-00002f90: 6917 d3cf b013 8770 2c7e eb4d 78ab e6b2  i......p,~.Mx...
-00002fa0: fa40 aba5 5a09 70b7 e6a7 56da 15c0 76f9  .@..Z.p...V...v.
-00002fb0: 7ce7 e892 ba31 3a4d a595 53d2 796a f09f  |....1:M..S.yj..
-00002fc0: d63d f8e7 fea2 fe84 ac32 091e 9d13 577c  .=.......2....W|
-00002fd0: 4f09 63e2 b9ab 9e98 11b9 4423 89db f3e0  O.c.......D#....
-00002fe0: 70f2 3777 9b5b 4a13 1c42 caf3 df42 0bc1  p.7w.[J..B...B..
-00002ff0: 9e27 9b1b 7815 1c4e d7d8 c654 ced3 5853  .'..x..N...T..XS
-00003000: ad5d 43c0 af55 bc40 a284 d775 6067 220f  .]C..U.@...u`g".
-00003010: a8de 382b b45b 3d57 b8d2 39ba c124 f7cf  ..8+.[=W..9..$..
-00003020: 9491 fdfb 620a e047 0e26 2d55 0a45 e114  ....b..G.&-U.E..
-00003030: dd20 37ab ef21 3da5 7bfb aa4c b70d 7e5a  . 7..!=.{..L..~Z
-00003040: 1d5d 3635 8430 8ec3 11dd 4c94 a5ab aa81  .]65.0....L.....
-00003050: 6cda 79aa f6bc a9a9 4a6a f6ba 8425 7994  l.y.....Jj...%y.
-00003060: 0ef3 2309 48c6 5f60 eb54 c521 a9af e0e4  ..#.H._`.T.!....
-00003070: f357 519b ddea 185a d82e 4fa6 05ec 7932  .WQ....Z..O...y2
-00003080: 2def cda7 ca0c cbb4 df3d 591f b1b4 9c11  -........=Y.....
-00003090: c764 dd93 a69e cc8a db7a 3a31 187b 3a31  .d.......z:1.{:1
-000030a0: 587b 3a31 987b 3a31 d87b 3cb1 5c9b 4f0d  X{:1.{:1.{<.\.O.
-000030b0: 744e 3d1c 39be 54a3 2634 0b95 00d7 dc40  tN=.9.T.&4.....@
-000030c0: 5495 f171 26ce ee02 cfbd a4f2 021d 113f  T..q&..........?
-000030d0: 48ca 38cd be35 5e7e 262a 859c d5ae 553b  H.8..5^~&*....U;
-000030e0: f6ff 13bc fe0d 0000 ffff 0300 504b 0102  ............PK..
-000030f0: 2d00 1400 0600 0800 0000 2100 bac4 8506  -.........!.....
-00003100: 7901 0000 9805 0000 1300 0000 0000 0000  y...............
-00003110: 0000 0000 0000 0000 0000 5b43 6f6e 7465  ..........[Conte
-00003120: 6e74 5f54 7970 6573 5d2e 786d 6c50 4b01  nt_Types].xmlPK.
-00003130: 022d 0014 0006 0008 0000 0021 00b5 5530  .-.........!..U0
-00003140: 23f4 0000 004c 0200 000b 0000 0000 0000  #....L..........
-00003150: 0000 0000 0000 00b2 0300 005f 7265 6c73  ..........._rels
-00003160: 2f2e 7265 6c73 504b 0102 2d00 1400 0600  /.relsPK..-.....
-00003170: 0800 0000 2100 9e81 d450 1101 0000 d603  ....!....P......
-00003180: 0000 1a00 0000 0000 0000 0000 0000 0000  ................
-00003190: d706 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
-000031a0: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 504b  kbook.xml.relsPK
-000031b0: 0102 2d00 1400 0600 0800 0000 2100 e619  ..-.........!...
-000031c0: 1dd3 2302 0000 4104 0000 0f00 0000 0000  ..#...A.........
-000031d0: 0000 0000 0000 0000 2809 0000 786c 2f77  ........(...xl/w
-000031e0: 6f72 6b62 6f6f 6b2e 786d 6c50 4b01 022d  orkbook.xmlPK..-
-000031f0: 0014 0006 0008 0000 0021 009c 6391 4caa  .........!..c.L.
-00003200: 0000 00ea 0000 0014 0000 0000 0000 0000  ................
-00003210: 0000 0000 0078 0b00 0078 6c2f 7368 6172  .....x...xl/shar
-00003220: 6564 5374 7269 6e67 732e 786d 6c50 4b01  edStrings.xmlPK.
-00003230: 022d 0014 0006 0008 0000 0021 001a e8a8  .-.........!....
-00003240: b791 0600 00e5 1b00 0013 0000 0000 0000  ................
-00003250: 0000 0000 0000 0054 0c00 0078 6c2f 7468  .......T...xl/th
-00003260: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
-00003270: 0102 2d00 1400 0600 0800 0000 2100 e97d  ..-.........!..}
-00003280: fce0 0e03 0000 1e08 0000 0d00 0000 0000  ................
-00003290: 0000 0000 0000 0000 1613 0000 786c 2f73  ............xl/s
-000032a0: 7479 6c65 732e 786d 6c50 4b01 022d 0014  tyles.xmlPK..-..
-000032b0: 0006 0008 0000 0021 00bf 6024 7b98 0200  .......!..`${...
-000032c0: 00ad 0500 0018 0000 0000 0000 0000 0000  ................
-000032d0: 0000 004f 1600 0078 6c2f 776f 726b 7368  ...O...xl/worksh
-000032e0: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
-000032f0: 4b01 022d 0014 0006 0008 0000 0021 005e  K..-.........!.^
-00003300: 7e59 7cbd 0100 007d 0400 0018 0000 0000  ~Y|....}........
-00003310: 0000 0000 0000 0000 001d 1900 0063 7573  .............cus
-00003320: 746f 6d58 6d6c 2f69 7465 6d50 726f 7073  tomXml/itemProps
-00003330: 322e 786d 6c50 4b01 022d 0014 0006 0008  2.xmlPK..-......
-00003340: 0000 0021 005c 9627 22c3 0000 0028 0100  ...!.\.'"....(..
-00003350: 001e 0000 0000 0000 0000 0000 0000 0038  ...............8
-00003360: 1b00 0063 7573 746f 6d58 6d6c 2f5f 7265  ...customXml/_re
-00003370: 6c73 2f69 7465 6d32 2e78 6d6c 2e72 656c  ls/item2.xml.rel
-00003380: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-00003390: 0074 3f39 7ac2 0000 0028 0100 001e 0000  .t?9z....(......
-000033a0: 0000 0000 0000 0000 0000 003f 1d00 0063  ...........?...c
-000033b0: 7573 746f 6d58 6d6c 2f5f 7265 6c73 2f69  ustomXml/_rels/i
-000033c0: 7465 6d31 2e78 6d6c 2e72 656c 7350 4b01  tem1.xml.relsPK.
-000033d0: 022d 0014 0006 0008 0000 0021 00bd 8462  .-.........!...b
-000033e0: 2390 0000 00db 0000 0013 0000 0000 0000  #...............
-000033f0: 0000 0000 0000 0045 1f00 0063 7573 746f  .......E...custo
-00003400: 6d58 6d6c 2f69 7465 6d31 2e78 6d6c 504b  mXml/item1.xmlPK
-00003410: 0102 2d00 1400 0600 0800 0000 2100 1118  ..-.........!...
-00003420: db79 f400 0000 4f01 0000 1800 0000 0000  .y....O.........
-00003430: 0000 0000 0000 0000 2e20 0000 6375 7374  ......... ..cust
-00003440: 6f6d 586d 6c2f 6974 656d 5072 6f70 7331  omXml/itemProps1
-00003450: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00003460: 0000 2100 a05a 864d 8a01 0000 0703 0000  ..!..Z.M........
-00003470: 1000 0000 0000 0000 0000 0000 0000 8021  ...............!
-00003480: 0000 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
-00003490: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-000034a0: 2100 c8fa e105 4801 0000 6902 0000 1100  !.....H...i.....
-000034b0: 0000 0000 0000 0000 0000 0000 4024 0000  ............@$..
-000034c0: 646f 6350 726f 7073 2f63 6f72 652e 786d  docProps/core.xm
-000034d0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000034e0: 0055 9f35 f5d4 0900 008c 3000 0013 0000  .U.5......0.....
-000034f0: 0000 0000 0000 0000 0000 00bf 2600 0063  ............&..c
-00003500: 7573 746f 6d58 6d6c 2f69 7465 6d32 2e78  ustomXml/item2.x
-00003510: 6d6c 504b 0506 0000 0000 1000 1000 2604  mlPK..........&.
-00003520: 0000 ec30 0000 0000                      ...0....
+00002570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000025f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002600: 0000 0000 0084 cfc1 8a02 310c 06e0 bbe0  ..........1.....
+00002610: 3b94 dc9d ce78 1091 e978 5916 bc89 b8e0  ;....x...xY.....
+00002620: b574 3233 c569 539a 28fa f616 4f2b 2cec  .t23.iS.(...O+,.
+00002630: 3109 f9fe a4dd 3fc2 acee 98d9 5334 d054  1.....?.....S4.T
+00002640: 3528 8c8e 7a1f 4703 3fe7 efd5 1614 8b8d  5(..z.G.?.......
+00002650: bd9d 29a2 8127 32ec bbe5 a23d e16c a52c  ..)..'2....=.l.,
+00002660: f1e4 13ab a244 3630 89a4 9dd6 ec26 0c96  .....D60.....&..
+00002670: 2b4a 18cb 64a0 1cac 9432 8f3a 5977 b523  +J..d....2.:Yw.#
+00002680: ea75 5d6f 74fe 6d40 f761 aa43 6f20 1ffa  .u]ot.m@.a.Co ..
+00002690: 06d4 f999 4af2 ff36 0d83 77f8 45ee 1630  ....J..6..w.E..0
+000026a0: ca1f 11da dd58 285c c27c cc94 b8c8 368f  .....X(\.|....6.
+000026b0: 2806 bc60 78b7 9aaa dc0b ba6b f5c7 7fdd  (..`x......k....
+000026c0: 0b00 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+000026d0: 0000 0021 005c 9627 22c3 0000 0028 0100  ...!.\.'"....(..
+000026e0: 001e 0008 0163 7573 746f 6d58 6d6c 2f5f  .....customXml/_
+000026f0: 7265 6c73 2f69 7465 6d32 2e78 6d6c 2e72  rels/item2.xml.r
+00002700: 656c 7320 a204 0128 a000 0100 0000 0000  els ...(........
+00002710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000027a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000027b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000027c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000027d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000027e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000027f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002800: 0000 0000 0000 0000 0000 0084 cfc1 6ac3  ..............j.
+00002810: 300c 06e0 7ba1 ef60 745f 9cf6 304a 89d3  0...{..`t_..0J..
+00002820: 4b19 e436 460b bd1a 4749 4c63 cb58 4a69  K..6F...GILc.XJi
+00002830: df7e a6a7 1606 3b4a 42df 2f35 877b 98d5  .~....;JB./5.{..
+00002840: 0d33 7b8a 0636 550d 0aa3 a3de c7d1 c0f9  .3{..6U.........
+00002850: f4f5 b103 c562 636f 678a 68e0 810c 8776  .....bcog.h....v
+00002860: bd6a 7e70 b652 9678 f289 5551 221b 9844  .j~p.R.x..UQ"..D
+00002870: d25e 6b76 1306 cb15 258c 6532 500e 564a  .^kv....%.e2P.VJ
+00002880: 9947 9dac bbda 11f5 b6ae 3f75 7e35 a07d  .G........?u~5.}
+00002890: 3355 d71b c85d bf01 757a a492 fcbf 4dc3  3U...]..uz....M.
+000028a0: e01d 1ec9 2d01 a3fc 11a1 ddc2 42e1 12e6  ....-.......B...
+000028b0: ef4c 898b 6cf3 8862 c00b 8667 6b5b 957b  .L..l..b...gk[.{
+000028c0: 41b7 8d7e fbaf fd05 0000 ffff 0300 504b  A..~..........PK
+000028d0: 0304 1400 0600 0800 0000 2100 7bf3 02a3  ..........!.{...
+000028e0: c300 0000 2801 0000 1e00 0801 6375 7374  ....(.......cust
+000028f0: 6f6d 586d 6c2f 5f72 656c 732f 6974 656d  omXml/_rels/item
+00002900: 332e 786d 6c2e 7265 6c73 20a2 0401 28a0  3.xml.rels ...(.
+00002910: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00002920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a10: 0000 84cf c16a c330 0c06 e07b 61ef 6074  .....j.0...{a.`t
+00002a20: 5f9c 7430 4a89 d3cb 28e4 3646 07bb 1a47  _.t0J...(.6F...G
+00002a30: 71cc 62cb 58ea 58df 7ea6 a716 063d 4a42  q.b.X.X.~....=JB
+00002a40: df2f f587 dfb8 aa1f 2c1c 2819 e89a 1614  ./......,.(.....
+00002a50: 2647 5348 dec0 e7e9 f8bc 03c5 62d3 6457  &GSH........b.dW
+00002a60: 4a68 e082 0c87 e169 d37f e06a a52e f112  Jh.....i...j....
+00002a70: 32ab aa24 36b0 88e4 bdd6 ec16 8c96 1bca  2..$6...........
+00002a80: 98ea 64a6 12ad d4b2 789d adfb b61e f5b6  ..d.....x.......
+00002a90: 6d5f 75b9 3560 b833 d538 1928 e3d4 813a  m_u.5`.3.8.(...:
+00002aa0: 5d72 4d7e 6cd3 3c07 876f e4ce 1193 fc13  ]rM~l.<..o......
+00002ab0: a1dd 9985 e257 5cdf 0b65 aeb2 2d1e c540  .....W\..e..-..@
+00002ac0: 108c d7d6 4b53 ef05 3df4 faee bfe1 0f00  ....KS..=.......
+00002ad0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00002ae0: 0021 0010 9525 c0bc 0100 007d 0400 0018  .!...%.....}....
+00002af0: 0028 0063 7573 746f 6d58 6d6c 2f69 7465  .(.customXml/ite
+00002b00: 6d50 726f 7073 312e 786d 6c20 a224 0028  mProps1.xml .$.(
+00002b10: a020 0000 0000 0000 0000 0000 0000 0000  . ..............
+00002b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002b30: 0000 00b4 945f 6bdb 3014 c5df 07fb 0e46  ....._k.0......F
+00002b40: efb2 e4f8 7fa9 53d2 a481 c20a 63eb a0af  ......S.....c...
+00002b50: d7b2 9488 5992 91e4 6563 ecbb 4f76 3b46  ....Y...ec..Ov;F
+00002b60: d794 6cac 7db2 afcd 3de7 dee3 9f7c 7ef1  ..l.}...=....|~.
+00002b70: 55f5 d117 6e9d 34ba 4149 4c51 c435 339d  U...n.4.AILQ.53.
+00002b80: d4bb 067d badd e20a 45ce 83ee a037 9a37  ...}....E....7.7
+00002b90: 481b 74b1 7cfb e6bc 7367 1d78 70de 587e  H.t.|...sg.xp.X~
+00002ba0: edb9 8ac2 0319 aed7 9b06 7d2f 92cd 55b1  ..........}/..U.
+00002bb0: a12b 9cd1 7a8d b3cb d51a af2e 698d e996  .+..z.......i...
+00002bc0: 96d5 627b 9564 dbea 078a 82b5 0e32 ae41  ..b{.d.......2.A
+00002bd0: 7bef 8733 421c db73 052e 3603 d7e1 a530  {..3B..s..6....0
+00002be0: 5681 0fa5 dd11 2384 647c 63d8 a8b8 f664  V.....#.d|c....d
+00002bf0: 4169 41d8 18ec d59d ead1 729a e7be fb03  AiA.......r.....
+00002c00: 17ee 7139 8d36 5af9 c445 4966 8d33 c2c7  ..q9.6Z..EIf.3..
+00002c10: cca8 0783 7b61 c53d 4cdb 1166 b40f 76b7  ....{a.=L..f..v.
+00002c20: df06 8ec8 8ba9 0e36 2c68 bde4 8e4c 4e2b  .......6,h...LN+
+00002c30: efad 6c47 cfdd 298f c3e1 101f d239 8f10  ..lG..)......9..
+00002c40: 4042 ee6e de7d 9c23 7b95 e19e 156d 4b5a  @B.n.}.#{....mKZ
+00002c50: 4021 524c 4bd1 e2ac 4d2b 5ce5 34c7 5096  @!RLK...M+\.4.P.
+00002c60: 79c1 aaa4 6e33 78b6 9926 5502 5d5e e2bc  y...n3x..&U.]^..
+00002c70: ce17 0190 7007 0204 2e69 0add 82a6 35b0  ....p....i....5.
+00002c80: eaff d7e9 1e40 b901 0d3b 3e23 e3c3 473c  .....@...;>#..G<
+00002c90: 99f0 2f02 8fb2 21b5 3003 f8fd 0449 49de  ../...!.0....II.
+00002ca0: 83f5 9adb 7540 c49a feaf 958f b03d 00fb  ....u@.......=..
+00002cb0: 1ca6 7cc2 9ee5 f837 2aa7 3219 46db cf64  ..|....7*.2.F..d
+00002cc0: 748c f07e 5ed9 9124 4ec8 bf34 7a6e 953b  t..~^..$N..4zn.;
+00002cd0: d971 3c24 198e 8ad5 d013 d376 9327 f9e3  .q<$.......v.'..
+00002ce0: 484e f5a3 5fc6 f227 0000 00ff ff03 0050  HN.._..'.......P
+00002cf0: 4b03 0414 0006 0008 0000 0021 007a 0991  K..........!.z..
+00002d00: 930e 0100 0092 0100 0013 0008 0164 6f63  .............doc
+00002d10: 5072 6f70 732f 6375 7374 6f6d 2e78 6d6c  Props/custom.xml
+00002d20: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
+00002d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e20: 0000 0000 0000 0000 9cd0 c96e 8330 1006  ...........n.0..
+00002e30: e07b a5be 83e5 bb63 b363 0444 c104 a9b7  .{.....c.c.D....
+00002e40: 1ed2 de11 9804 092f c20e 0daa faee 35ea  ......./......5.
+00002e50: 927b 8ea3 99f9 f4cf e4fb 9b98 c0c2 6733  .{............g3
+00002e60: 2a59 406f 4720 e0b2 53fd 28cf 057c 3b35  *Y@oG ..S.(..|;5
+00002e70: 2885 c0d8 56f6 eda4 242f e0ca 0ddc 97cf  (...V...$/......
+00002e80: 4ff9 ebac 349f edc8 0d70 8434 05bc 58ab  O...4....p.4..X.
+00002e90: 338c 4d77 e1a2 353b d796 ae33 a859 b4d6  3.Mw..5;...3.Y..
+00002ea0: 95f3 19ab 6118 3b5e abee 2ab8 b4d8 2724  ....a.;^..*...'$
+00002eb0: c6dd d558 2590 fee7 e08f 972d f651 b257  ...X%......-.Q.W
+00002ec0: dd96 cebc 9f56 ede2 96f9 2fbe 8241 d8b1  .....V..../..A..
+00002ed0: 2fe0 671d b1ba 8e48 84fc 2365 c823 5e85  /.g....H..#e.#^.
+00002ee0: 6840 1344 5242 fcca 670d 3d1c bf20 d0db  h@.DRB..g.=.. ..
+00002ef0: b00f 816c 853b 9d29 695d ec0d 7de9 9dba  ...l.;.)i]..}...
+00002f00: d86c d21f c6ce 25b9 1167 10d2 0481 e7d1  .l....%..g......
+00002f10: 2af6 5990 4461 4869 9db0 264c 0f94 d569  *.Y.DaHi..&L...i
+00002f20: 9c46 718e ef3b 39fe 4b55 e6f8 fecc f21b  .Fq..;9.KU......
+00002f30: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00002f40: 0000 2100 a05a 864d 8a01 0000 0703 0000  ..!..Z.M........
+00002f50: 1000 0801 646f 6350 726f 7073 2f61 7070  ....docProps/app
+00002f60: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
+00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003060: 0000 0000 0000 0000 0000 0000 9c92 c16e  ...............n
+00003070: 1331 1086 ef48 bc83 e57b e34d 4115 8abc  .1...H...{.MA...
+00003080: ae50 0bca 0144 a4a4 bd1b 7b36 3138 f6ca  .P...D....{618..
+00003090: 3359 25bc 0dcf c28b 31bb aba6 9b96 13b7  3Y%.....1.......
+000030a0: 99f9 67ff fdfc dbfa f6b8 8fa2 8382 21a7  ..g...........!.
+000030b0: 5ace 6795 1490 5cf6 216d 6bf9 b0f9 7cf5  Z.g...\.!mk...|.
+000030c0: 410a 249b bc8d 3941 2d4f 80f2 d6bc 7da3  A.$...9A-O....}.
+000030d0: 5725 b750 2800 0ab6 4858 cb1d 51bb 500a  W%.P(...HX..Q.P.
+000030e0: dd0e f616 672c 2756 9a5c f696 b82d 5b95  ....g,'V.\...-[.
+000030f0: 9b26 38b8 cfee b087 44ea baaa 6e14 1c09  .&8.....D...n...
+00003100: 9207 7fd5 9e0d e5e8 b8e8 e87f 4d7d 763d  ............M}v=
+00003110: 1f3e 6e4e 2d03 1bfd b16d 6370 96f8 94e6  .>nN-....mcp....
+00003120: 6b70 2563 6e48 7c3a 3a88 5a4d 45cd 746b  kp%cnH|::.ZME.tk
+00003130: 7087 12e8 642a ada6 ad5e 3b1b e18e 8d4d  p...d*...^;....M
+00003140: 6323 8256 cf03 bd04 db87 b6b2 a1a0 d11d  c#.V............
+00003150: 2d3a 7094 8bc0 f08b 63bb 96e2 bb45 e871  -:p.....c....E.q
+00003160: 6ad9 d912 6c22 c6ea d7c6 66a8 638b 54cc  j...l"....f.c.T.
+00003170: 32ff b028 3c08 f7e7 7774 8798 b5e2 bd51  2..(<...wt.....Q
+00003180: 1bca e927 d33a bc37 f361 818b cbc5 de60  ...'.:.7.a.....`
+00003190: e461 e192 7413 2802 7e6b 56b6 d03f c0e7  .a..t.(.~kV..?..
+000031a0: 53f0 8161 c41e 71c6 9751 fc2b c2e1 ecfc  S..a..q..Q.+....
+000031b0: af17 ee5f 42fa 890f ed26 df5b 82a7 102f  ..._B....&.[.../
+000031c0: 877a bdb3 053c e77e 0ef9 3cd0 4bce afc4  .z...<.~..<.K...
+000031d0: dee4 6e67 d316 fcd3 ce6b a1bf f2c7 f15d  ..ng.....k.....]
+000031e0: 9bf9 cdac 7a57 f16d 4e66 5a3d bf60 f317  ....zW.mNfZ=.`..
+000031f0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00003200: 0000 2100 12cf 9127 4801 0000 6902 0000  ..!....'H...i...
+00003210: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
+00003220: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
+00003230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000032f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003320: 0000 0000 0000 0000 0000 0000 0084 925d  ...............]
+00003330: 4bc3 3018 85ef 05ff 43c9 7d9b b693 6e86  K.0.....C.}...n.
+00003340: b683 29bb 7220 3899 7817 9277 5bb1 f920  ..).r 8.x..w[.. 
+00003350: c9ec f6ef 4ddb ad56 2708 b949 cec9 9373  ....M..V'..I...s
+00003360: 5e92 cf8f a20e 3ec1 d84a c902 2551 8c02  ^.....>..J..%Q..
+00003370: 904c f14a ee0a f4ba 5e86 3314 5847 25a7  .L.J....^.3.XG%.
+00003380: b592 50a0 1358 342f 6f6f 72a6 0953 069e  ..P..X4/oor..S..
+00003390: 8dd2 605c 0536 f024 6909 d305 da3b a709  ..`\.6.$i....;..
+000033a0: c696 ed41 501b 7987 f4e2 5619 419d df9a  ...AP.y...V.A...
+000033b0: 1dd6 947d d01d e034 8e33 2cc0 514e 1dc5  ...}...4.3,.QN..
+000033c0: 2d30 d403 119d 919c 0d48 7d30 7507 e00c  -0.......H}0u...
+000033d0: 430d 02a4 b338 8912 fced 7560 84fd f342  C....8....u`...B
+000033e0: a78c 9ca2 7227 ed3b 9de3 8ed9 9cf5 e2e0  ....r'.;........
+000033f0: 3eda 6a30 364d 1335 932e 86cf 9fe0 b7d5  >.j06M.5........
+00003400: d34b 5735 ac64 3b2b 06a8 cc39 23cc 0075  .KW5.d;+...9#..u
+00003410: ca94 0b73 902a 581a afa8 1c8f 8476 8835  ...s.*X......v.5
+00003420: b56e e5e7 bdad 802f 4ebf bcd7 bae7 7635  .n...../N.....v5
+00003430: 7a38 f0c0 0723 7d8d 8bb2 993c 3cae 97a8  z8...#}....<<...
+00003440: 4ce3 7412 c67e 65eb 644a eeee 4932 7d6f  L.t..~e.dJ..I2}o
+00003450: 9fff 71bf 0dda 1f88 7388 7f89 5998 ce5a  ..q.....s...Y..Z
+00003460: 629a 9138 1911 2f80 32c7 579f a3fc 0200  b..8../.2.W.....
+00003470: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00003480: 0021 0073 3226 f9a0 0100 00ba 0300 0018  .!.s2&..........
+00003490: 0028 0063 7573 746f 6d58 6d6c 2f69 7465  .(.customXml/ite
+000034a0: 6d50 726f 7073 332e 786d 6c20 a224 0028  mProps3.xml .$.(
+000034b0: a020 0000 0000 0000 0000 0000 0000 0000  . ..............
+000034c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000034d0: 0000 0094 535d 6bdb 3014 7d1f ec3f 18bd  ....S]k.0.}..?..
+000034e0: cb92 e34f 953a 25c4 1914 5618 6385 bede  ...O.:%...V.c...
+000034f0: c857 8999 2519 4959 36c6 fefb e4b4 1bb4  .W..%.IY6.......
+00003500: b44b f624 5f99 7bcf 39f7 1c5d df7c d763  .K.$_.{.9..].|.c
+00003510: f20d 9d1f ac69 4996 7292 a091 b61f ccae  .....iI.r.......
+00003520: 25f7 5f3e d086 243e 80e9 61b4 065b 622c  %._>..$>..a..[b,
+00003530: b959 be7f 77dd fbab 1e02 f860 1dde 06d4  .Y..w......`....
+00003540: 49bc 18e2 79db b5e4 27af 3a91 358b 9a76  I...y...'.:.5..v
+00003550: 42ac 69b1 2a37 54e4 794e 45b5 5915 ab55  B.i.*7T.yNE.Y..U
+00003560: b729 d6f9 2f92 4468 13c7 f896 ec43 98ae  .)../.Dh.....C..
+00003570: 18f3 728f 1a7c 6a27 34f1 a7b2 4e43 88a5  ..r..|j'4...NC..
+00003580: db31 abd4 20b1 b3f2 a0d1 04b6 e0bc 62f2  .1.. .........b.
+00003590: 10e1 f583 1ec9 72e6 f3d8 fd19 957f 5ece  ......r.......^.
+000035a0: d40e 6ef8 8b32 1ddc 789a d94b d64b 3d84  ..n..2..x..K.K=.
+000035b0: 1f13 32c2 2e6f c211 6712 9e65 6976 b6f1  ..2..o..g..eiv..
+000035c0: 8f26 3d48 67bd 5521 9556 3fc9 7994 a131  .&=Hg.U!.V?.y..1
+000035d0: c0bc 4b36 b928 dc85 01fd ffb0 09e8 b4bf  ..K6.(..........
+000035e0: 98c6 2bab 9d40 7e85 1dbe 2023 a3b1 f472  ..+..@~... #...r
+000035f0: 46ff 9439 1865 2708 fb19 a266 9fc0 0583  F..9.e'....f....
+00003600: 6e6d 4d70 763c abf5 fc02 fba7 54dc 8189  nmMpv<......T...
+00003610: 3a4e f998 3d7d 7b32 cf9a 0cfa b2a6 a528  :N..=}{2.......(
+00003620: 17b4 e0f1 0b14 285a f31c fa05 cf05 c8e6  ......(Z........
+00003630: 4d0b b635 afa0 5239 e5b5 dad2 629b 37b4  M..5..R9....b.7.
+00003640: 2979 49a1 aecb 4a36 99d8 1670 cebf e3f1  )yI...J6...p....
+00003650: 981e f353 081f ee3e b24c 8886 19d0 e8a3  ...S...>.L......
+00003660: 1738 37b3 1779 9eeb 67ef 6df9 1b00 00ff  .87..y..g.m.....
+00003670: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00003680: 0084 4c3d 2e36 0100 003c 0200 0013 0028  ..L=.6...<.....(
+00003690: 0063 7573 746f 6d58 6d6c 2f69 7465 6d33  .customXml/item3
+000036a0: 2e78 6d6c 20a2 2400 28a0 2000 0000 0000  .xml .$.(. .....
+000036b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036c0: 0000 0000 0000 0000 0000 0000 ac92 4b6f  ..............Ko
+000036d0: 8330 1084 ff4a e4bb b1c1 8021 02a2 2ad7  .0...J.....!..*.
+000036e0: 46aa d41c 7a5d fc08 96c0 46b6 53f2 f34b  F...z]....F.S..K
+000036f0: d2f4 71a8 d41e 7a9b c3ce b7b3 a36d 7697  ..q...z......mv.
+00003700: 69dc bc2a 1f8c b32d 4a13 8a36 ca0a 278d  i..*...-J..6..'.
+00003710: 3db5 e81c 35ae d0ae 6be6 edec ddac 7c34  =...5...k.....|4
+00003720: 2a6c 5687 0ddb b945 438c f396 9020 0635  *lV....EC.... .5
+00003730: 4148 2623 bc0b 4ec7 44b8 8938 ad8d 5024  AH&#..N.D..8..P$
+00003740: a3b4 2493 8a20 2102 f9a2 a03b e612 cc27  ..$.. !....;...'
+00003750: 6859 9664 6189 f3a7 ab2d 252f 87c7 e71b  hY.da....-%/....
+00003760: 1b1b 1b22 58a1 3e5c b3f8 db76 63b5 9b21  ..."X.>\...vc..!
+00003770: 0e57 1e27 4fe0 a355 7eef 6cf4 6e0c a86b  .W.'O..U~.l.n..k
+00003780: a413 e749 d978 000b 2775 555d 7384 cb1e  ...I.x..'uU]s...
+00003790: a218 1ec6 f13d 638b 685a a520 0b8e 8bba  .....=c.hZ. ....
+000037a0: c870 4e57 051a 34e6 9481 cc28 ab41 5488  .pNW..4....(.AT.
+000037b0: 74cd 2834 2f75 5a14 42c9 5c4a d1e7 b4e6  t.(4/uZ.B.\J....
+000037c0: 29cb b566 82b1 4c7f f07a 4e4b 2835 c394  )..f..L..zNK(5..
+000037d0: eb1e e73d ab70 55d0 0203 e745 29aa b4ee  ...=.pU....E)...
+000037e0: 7358 d31d 959f ee75 ffcf b9e4 46ec 1af2  sX.....u....F...
+000037f0: 5bd0 75e4 a76a c8f7 3fe8 de00 0000 ffff  [.u..j..?.......
+00003800: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00003810: bd84 6223 9000 0000 db00 0000 1300 2800  ..b#..........(.
+00003820: 6375 7374 6f6d 586d 6c2f 6974 656d 322e  customXml/item2.
+00003830: 786d 6c20 a224 0028 a020 0000 0000 0000  xml .$.(. ......
+00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003850: 0000 0000 0000 0000 0000 006c 8e3b 0ec2  ...........l.;..
+00003860: 3010 05af 82d2 932d e8d0 e234 810a 51e5  0......-...4..Q.
+00003870: 02c6 388a a5ac d7f2 2e1f df1e 0741 8194  ..8..........A..
+00003880: 7a9e 661e 7624 bc75 1cd5 471d 4af2 9dc1  z.f.v$.u..G.J...
+00003890: 1367 1a3c a5d9 aa97 cd8b e628 8766 524d  .g.<.......(.fRM
+000038a0: 7b00 7193 272b 2d05 9759 78d4 d631 814c  {.q.'+-..Yx..1.L
+000038b0: 36fb c421 2a3c 76f0 b569 b5c1 585d d218  6..!*<v..i..X]..
+000038c0: ec83 545f 313d bb3b d5d4 395c b3cd 6549  ..T_1=.;..9\..eI
+000038d0: 21fc 201e 6f41 d727 1f82 17ff 5cc7 0b40  !. .oA.'....\..@
+000038e0: f83b 6ede 0000 00ff ff03 0050 4b01 022d  .;n........PK..-
+000038f0: 0014 0006 0008 0000 0021 0087 56e1 3286  .........!..V.2.
+00003900: 0100 0099 0600 0013 0000 0000 0000 0000  ................
+00003910: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
+00003920: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
+00003930: 2d00 1400 0600 0800 0000 2100 135e be65  -.........!..^.e
+00003940: 0201 0000 df02 0000 0b00 0000 0000 0000  ................
+00003950: 0000 0000 0000 bf03 0000 5f72 656c 732f  .........._rels/
+00003960: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00003970: 0000 0021 00df a467 281a 0100 0064 0400  ...!...g(....d..
+00003980: 001a 0000 0000 0000 0000 0000 0000 00f2  ................
+00003990: 0600 0078 6c2f 5f72 656c 732f 776f 726b  ...xl/_rels/work
+000039a0: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
+000039b0: 022d 0014 0006 0008 0000 0021 00e6 191d  .-.........!....
+000039c0: d323 0200 0041 0400 000f 0000 0000 0000  .#...A..........
+000039d0: 0000 0000 0000 004c 0900 0078 6c2f 776f  .......L...xl/wo
+000039e0: 726b 626f 6f6b 2e78 6d6c 504b 0102 2d00  rkbook.xmlPK..-.
+000039f0: 1400 0600 0800 0000 2100 9c63 914c aa00  ........!..c.L..
+00003a00: 0000 ea00 0000 1400 0000 0000 0000 0000  ................
+00003a10: 0000 0000 9c0b 0000 786c 2f73 6861 7265  ........xl/share
+00003a20: 6453 7472 696e 6773 2e78 6d6c 504b 0102  dStrings.xmlPK..
+00003a30: 2d00 1400 0600 0800 0000 2100 1ae8 a8b7  -.........!.....
+00003a40: 9106 0000 e51b 0000 1300 0000 0000 0000  ................
+00003a50: 0000 0000 0000 780c 0000 786c 2f74 6865  ......x...xl/the
+00003a60: 6d65 2f74 6865 6d65 312e 786d 6c50 4b01  me/theme1.xmlPK.
+00003a70: 022d 0014 0006 0008 0000 0021 00e9 7dfc  .-.........!..}.
+00003a80: e00e 0300 001e 0800 000d 0000 0000 0000  ................
+00003a90: 0000 0000 0000 003a 1300 0078 6c2f 7374  .......:...xl/st
+00003aa0: 796c 6573 2e78 6d6c 504b 0102 2d00 1400  yles.xmlPK..-...
+00003ab0: 0600 0800 0000 2100 392b b5e8 9a02 0000  ......!.9+......
+00003ac0: ad05 0000 1800 0000 0000 0000 0000 0000  ................
+00003ad0: 0000 7316 0000 786c 2f77 6f72 6b73 6865  ..s...xl/workshe
+00003ae0: 6574 732f 7368 6565 7431 2e78 6d6c 504b  ets/sheet1.xmlPK
+00003af0: 0102 2d00 1400 0600 0800 0000 2100 e925  ..-.........!..%
+00003b00: 3b38 f300 0000 4f01 0000 1800 0000 0000  ;8....O.........
+00003b10: 0000 0000 0000 0000 4319 0000 6375 7374  ........C...cust
+00003b20: 6f6d 586d 6c2f 6974 656d 5072 6f70 7332  omXml/itemProps2
+00003b30: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00003b40: 0000 2100 559f 35f5 d409 0000 8c30 0000  ..!.U.5......0..
+00003b50: 1300 0000 0000 0000 0000 0000 0000 941a  ................
+00003b60: 0000 6375 7374 6f6d 586d 6c2f 6974 656d  ..customXml/item
+00003b70: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
+00003b80: 0000 0021 0074 3f39 7ac2 0000 0028 0100  ...!.t?9z....(..
+00003b90: 001e 0000 0000 0000 0000 0000 0000 00c1  ................
+00003ba0: 2400 0063 7573 746f 6d58 6d6c 2f5f 7265  $..customXml/_re
+00003bb0: 6c73 2f69 7465 6d31 2e78 6d6c 2e72 656c  ls/item1.xml.rel
+00003bc0: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
+00003bd0: 005c 9627 22c3 0000 0028 0100 001e 0000  .\.'"....(......
+00003be0: 0000 0000 0000 0000 0000 00c7 2600 0063  ............&..c
+00003bf0: 7573 746f 6d58 6d6c 2f5f 7265 6c73 2f69  ustomXml/_rels/i
+00003c00: 7465 6d32 2e78 6d6c 2e72 656c 7350 4b01  tem2.xml.relsPK.
+00003c10: 022d 0014 0006 0008 0000 0021 007b f302  .-.........!.{..
+00003c20: a3c3 0000 0028 0100 001e 0000 0000 0000  .....(..........
+00003c30: 0000 0000 0000 00ce 2800 0063 7573 746f  ........(..custo
+00003c40: 6d58 6d6c 2f5f 7265 6c73 2f69 7465 6d33  mXml/_rels/item3
+00003c50: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
+00003c60: 0006 0008 0000 0021 0010 9525 c0bc 0100  .......!...%....
+00003c70: 007d 0400 0018 0000 0000 0000 0000 0000  .}..............
+00003c80: 0000 00d5 2a00 0063 7573 746f 6d58 6d6c  ....*..customXml
+00003c90: 2f69 7465 6d50 726f 7073 312e 786d 6c50  /itemProps1.xmlP
+00003ca0: 4b01 022d 0014 0006 0008 0000 0021 007a  K..-.........!.z
+00003cb0: 0991 930e 0100 0092 0100 0013 0000 0000  ................
+00003cc0: 0000 0000 0000 0000 00ef 2c00 0064 6f63  ..........,..doc
+00003cd0: 5072 6f70 732f 6375 7374 6f6d 2e78 6d6c  Props/custom.xml
+00003ce0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00003cf0: a05a 864d 8a01 0000 0703 0000 1000 0000  .Z.M............
+00003d00: 0000 0000 0000 0000 0000 362f 0000 646f  ..........6/..do
+00003d10: 6350 726f 7073 2f61 7070 2e78 6d6c 504b  cProps/app.xmlPK
+00003d20: 0102 2d00 1400 0600 0800 0000 2100 12cf  ..-.........!...
+00003d30: 9127 4801 0000 6902 0000 1100 0000 0000  .'H...i.........
+00003d40: 0000 0000 0000 0000 f631 0000 646f 6350  .........1..docP
+00003d50: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
+00003d60: 022d 0014 0006 0008 0000 0021 0073 3226  .-.........!.s2&
+00003d70: f9a0 0100 00ba 0300 0018 0000 0000 0000  ................
+00003d80: 0000 0000 0000 0075 3400 0063 7573 746f  .......u4..custo
+00003d90: 6d58 6d6c 2f69 7465 6d50 726f 7073 332e  mXml/itemProps3.
+00003da0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00003db0: 0021 0084 4c3d 2e36 0100 003c 0200 0013  .!..L=.6...<....
+00003dc0: 0000 0000 0000 0000 0000 0000 0073 3600  .............s6.
+00003dd0: 0063 7573 746f 6d58 6d6c 2f69 7465 6d33  .customXml/item3
+00003de0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00003df0: 0000 2100 bd84 6223 9000 0000 db00 0000  ..!...b#........
+00003e00: 1300 0000 0000 0000 0000 0000 0000 0238  ...............8
+00003e10: 0000 6375 7374 6f6d 586d 6c2f 6974 656d  ..customXml/item
+00003e20: 322e 786d 6c50 4b05 0600 0000 0014 0014  2.xmlPK.........
+00003e30: 003a 0500 00eb 3800 0000 00              .:....8....
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/data_base_MM.xlsx` & `dp4plus_app-0.1.9/src/dp4plus_app/data_base_MM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/data_base_QM.xlsx` & `dp4plus_app-0.1.9/src/dp4plus_app/data_base_QM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/dp4_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/dp4_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/logo_INGEBIO.png` & `dp4plus_app-0.1.9/src/dp4plus_app/logo_INGEBIO.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/main_gui_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/main_gui_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 The function gui_input() is made to be used as widget in calc scripts. 
 Besides gui_end() is there to give neat conclusion of the programme. 
 
 """
 
 import tkinter as tk
 import pandas as pd
-import os, shutil, webbrowser, glob
+import os, shutil, webbrowser, glob, subprocess
 
 from collections import Counter
 from pathlib import Path
 from sys import exit
-from tkinter import filedialog
+from tkinter import filedialog, messagebox
 from random import sample, randint
 
 def gui_input():
     '''Main structure of the widget app (GUI). 
     The window design is placed here, while the funtions of each element are 
     defined apart. Each element is globaled to be controled during decisions. 
     The result are not return untill the app is quit in the last step (run_calc())
     
         Returns
     mode: 'QM', 'MM' or 'Custom'
     for 'Custom' the other variable indicates the TheLev or if it's a reparametrization
     for 'QM' and 'MM', it gives the inputs for the DP4 calculation
     '''
     global root
-    root = tk.Tk()      #define the widget
+    root = tk.Toplevel()      #define the widget
     root.wm_title("DP4+ App")
     root.geometry("750x260")
     
     title = tk.Label( root, text= 'DP4+ App')
     title.place(x=20, y= 5)
     title.config(font = ("Times", "35", "bold"))
     
@@ -109,15 +109,15 @@
     #-----------------------------------------------------------------
     button_dir = tk.Button(root, text='Select Directory',
                            font=("Helvetica", 10),
                            command=lambda: select_dir (),
                            state='disabled')
     button_dir.place(x=20,y=110)
     #-----------------------------------------------------------------
-    root.mainloop() #keep the window open while programme is running
+    root.wait_window() #keep the window open while programme is running
     
     if 'reparametrize' in the_lev : 
         return mode, the_lev
     else: 
         return mode, {'isom':isomer_list,
                       'the_lev': the_lev,
                       'xlsx': xlsx,
@@ -125,15 +125,18 @@
                       'warn': warn}
     
 
 def user_guide():
     '''Open user guide documentation
     '''
     file = (Path(__file__).parent / "UserGuide" /"UserGuide.pdf").as_posix()
-    webbrowser.open_new(file)
+    try: 
+        subprocess.run(['open', file])
+    except:
+        webbrowser.open_new(file)
     return
     
 def example(): 
     '''Copy an example folder into the user Desktop for trying the programm
     '''
     desktop = os.path.normpath(os.path.expanduser("~/Desktop"))
     example_fold = (Path(__file__).parent / "nmr_examples").as_posix()
@@ -141,26 +144,26 @@
     dst_folder = os.path.join(desktop,"nmr_examples")
     if  os.path.exists(dst_folder):
         dst_folder = dst_folder+f'_{str(randint(0, 100))}'
     shutil.copytree(example_fold, dst_folder)
     
     root.quit()
     
-    examp_add = tk.Tk()
+    examp_add = tk.Toplevel()
     examp_add.wm_title("DP4+ App")
     tk.Label(examp_add,text = u' Folder Copy \u2713', 
              font = ("Arial Black", "12")).grid(row=0)
     tk.Label(examp_add,text ='"nmr_examples" has been created in your desktop', 
              font = ("Arial Bold", "10")).grid(row=1, pady=10)
     tk.Label(examp_add,text ='The program will restarts. Follow the user guide instructions to process the data', 
              font = ("Arial Bold", "10")).grid(row=2, padx=10)
     tk.Button(examp_add, text='Ok', 
               command= exit).grid(row=3, pady=5 )
     
-    examp_add.mainloop()
+    examp_add.wait_window()
 
     return
 
 def select_dir():
     '''Select directory. If it doesn't find .log and/or well rotulated 
     elements doesnt enable next button.
     It changes the working directory to the path selected
@@ -182,15 +185,15 @@
     files = []
     for file in glob.glob('*'): 
         if ('nmr' in file.casefold() and 
             any(extention in file[-4:] for extention in ['.out','.log'])): 
             files.append(file)
     
     if not files:
-        singboard.config( text='"_nmr" G09 files not found. Try again')
+        singboard.config( text='" *_nmr_*.log/out " files not found. Try again')
         button_run['state'] = 'disable'
         return
     
     sing = root.direc[:9]+'  . . .  '+root.direc[-50:]
     singboard.config( text=sing)
     
     global isomer_list
@@ -341,15 +344,15 @@
             the_lev = func_list.get()
         elif 'GAS' in solv_list.get():
             the_lev = func_list.get()+"."+base_list.get()
         else: 
             the_lev = func_list.get()+"."+base_list.get()+"."+solv_list.get()
         
         tk.Label(root,text='Processing . . .').place(x=70,y=220)
-        root.after(2000, root.quit)
+        root.after(2000, root.destroy)
         #Tiempo de espera para cerrar GUI. Es para que el usuario no le de ansiedat
         #Se frena el script, pero la GUI puede modificar sus carteles, es decir, 
         #corre las lineas siguientes 
         
     elif button_run['text'] == 'Reparametrize':
         tk.Label(root,text='Redirecting . . .').place(x=150,y=220)
         the_lev = 'reparametrize'
@@ -470,22 +473,8 @@
                  font = ("Arial Bold", "10")).grid(row=3, padx=10)
         tk.Button(warn_add, text='Ok', 
                   command=warn_add.destroy).grid(row=4, pady=5, padx =10)
         warn_add.wait_window()
     return
     
 
-def gui_end():
-    '''Final window to politely finish the programe'''
-    byby = tk.Tk()
-    byby.wm_title("DP4+ App")
-    
-    tk.Label(byby,text = u' Procces completed \u2713', 
-             font = ("Arial Black", "12")).grid(row=0,padx=10, pady=(10,0))
-    tk.Label(byby,text ='Press Exit to finish', 
-             font = ("Arial Bold", "10")).grid(row=1,padx=10, pady=5)
-    tk.Button(byby, text='Exit', 
-              command= exit).grid(row=3, pady=(5,10))
-    
-    byby.mainloop()
-    
-    return
+
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/custom_molecules_set.docx` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/custom_molecules_set.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a - copia.xlsx` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a - copia.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.9/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/output_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/output_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,16 @@
 def edit_appearance(file, sheet, cant_isom):
     '''Edits the appearance of the given sheet in the .xlsx file
     It's design to embellish the 'results' sheet according the position 
     of its outputs. However, it's easy to modify for other presentations. 
     '''
     wb = load_workbook(file)
     ws = wb[sheet]
+    ws.row_dimensions[1].height = 30
+    ws.row_dimensions[2].height = 20
     ws.column_dimensions['A'].width = 20
     for i in range(4, 7):
         ws[f'A{i}'].fill = PatternFill(start_color = 'BFC9CA', end_color = 'BFC9CA', fill_type = "solid")
     for i in range(7, 10):
         ws[f'A{i}'].fill = PatternFill(start_color = 'E5E7E9', end_color = 'E5E7E9', fill_type = "solid")
     for i in range(10, 13):
         ws[f'A{i}'].fill = PatternFill(start_color = '85C1E9', end_color = '85C1E9', fill_type = "solid")
@@ -154,24 +156,24 @@
                          italic=False, vertAlign=None, underline='none',
                          strike=False, color='FF000000')
     
     #remember to: pip install Pillow (or add to dependencies)
     
     img1 =(Path(__file__).parent / 'logo_CONICET.png').as_posix()
     img1 = Image(img1)
-    img1.height = img1.height/8
-    img1.width= img1.width/8
+    img1.height = img1.height/4
+    img1.width= img1.width/4
     img1.anchor = 'D1'
     ws.add_image(img1)
     
     img2 =(Path(__file__).parent / 'logo_INGEBIO.png').as_posix()
     img2 = Image(img2)
     img2.height = img2.height/2
     img2.width= img2.width/2
-    img2.anchor = 'G1'
+    img2.anchor = 'F1'
     ws.add_image(img2)
     
     ws.sheet_view.showGridLines = False
 
     wb.save(file)
     return
 #-----------------------------------------------------------------------
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app/validation_module.py` & `dp4plus_app-0.1.9/src/dp4plus_app/validation_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app.egg-info/PKG-INFO` & `dp4plus_app-0.1.9/src/dp4plus_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp4plus-app
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to simplify your DP4+ calculations
 Home-page: https://github.com/RosarioCCLab/DP4plus-App
 Author: Bruno A. Franco
 Author-email: bruno.agustin.franco@gmail.com
 License: MIT
 Keywords: nmr
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dp4plus_app-0.1.8/src/dp4plus_app.egg-info/SOURCES.txt` & `dp4plus_app-0.1.9/src/dp4plus_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/dp4plus_app/custom_gui_module.py
 src/dp4plus_app/custom_module.py
 src/dp4plus_app/data_base_Custom.xlsx
 src/dp4plus_app/data_base_MM.xlsx
 src/dp4plus_app/data_base_QM.xlsx
 src/dp4plus_app/dp4_module.py
 src/dp4plus_app/logo_CONICET.png
+src/dp4plus_app/logo_DP4app.png
 src/dp4plus_app/logo_INGEBIO.png
 src/dp4plus_app/main.py
 src/dp4plus_app/main_gui_module.py
 src/dp4plus_app/output_module.py
 src/dp4plus_app/validation_module.py
 src/dp4plus_app.egg-info/PKG-INFO
 src/dp4plus_app.egg-info/SOURCES.txt
```

