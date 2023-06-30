# Comparing `tmp/FuncsForSPO-6.2.5.tar.gz` & `tmp/FuncsForSPO-6.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.2.5.tar", last modified: Thu Jun 29 16:54:00 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.2.6.tar", last modified: Fri Jun 30 12:27:56 2023, max compression
```

## Comparing `FuncsForSPO-6.2.5.tar` & `FuncsForSPO-6.2.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.658106 FuncsForSPO-6.2.5/
-drwxrwxrwx   0        0        0        0 2023-06-29 16:53:59.906805 FuncsForSPO-6.2.5/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-29 16:53:59.970512 FuncsForSPO-6.2.5/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.2.5/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.2.5/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:53:59.983051 FuncsForSPO-6.2.5/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.2.5/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:53:59.995135 FuncsForSPO-6.2.5/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.2.5/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.025473 FuncsForSPO-6.2.5/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.2.5/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.2.5/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.2.5/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.2.5/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.035041 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.056113 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.067688 FuncsForSPO-6.2.5/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.2.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.074222 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.120779 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0    11162 2023-06-28 17:53:11.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3579 2023-06-28 17:15:41.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-28 13:21:40.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
--rw-rw-rw-   0        0        0      586 2023-06-28 17:27:37.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.145465 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.170082 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.178099 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.216813 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     8979 2023-06-29 16:52:52.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.230873 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.246926 FuncsForSPO-6.2.5/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.259009 FuncsForSPO-6.2.5/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.2.5/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.275120 FuncsForSPO-6.2.5/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.2.5/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.290030 FuncsForSPO-6.2.5/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39081 2023-06-26 14:06:50.000000 FuncsForSPO-6.2.5/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.491614 FuncsForSPO-6.2.5/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.5/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.2.5/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.522679 FuncsForSPO-6.2.5/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.2.5/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.2.5/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:54:00.560817 FuncsForSPO-6.2.5/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.2.5/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:53:59.959967 FuncsForSPO-6.2.5/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-06-29 16:53:59.000000 FuncsForSPO-6.2.5/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2127 2023-06-29 16:53:59.000000 FuncsForSPO-6.2.5/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 16:53:59.000000 FuncsForSPO-6.2.5/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-06-29 16:53:59.000000 FuncsForSPO-6.2.5/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-06-29 16:53:59.000000 FuncsForSPO-6.2.5/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.2.5/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-06-29 16:54:00.653102 FuncsForSPO-6.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 16:54:00.659108 FuncsForSPO-6.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2663 2023-06-29 16:53:47.000000 FuncsForSPO-6.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:56.072571 FuncsForSPO-6.2.6/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.632490 FuncsForSPO-6.2.6/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.690636 FuncsForSPO-6.2.6/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.2.6/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.2.6/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.702637 FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.711637 FuncsForSPO-6.2.6/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.2.6/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.732636 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.2.6/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.739637 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.756645 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.768174 FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.774176 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.820820 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0    11162 2023-06-28 17:53:11.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3579 2023-06-28 17:15:41.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1340 2023-06-28 13:21:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+-rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.836817 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.855823 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.860355 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.893360 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0     9951 2023-06-30 12:26:15.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.904444 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.918909 FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.928908 FuncsForSPO-6.2.6/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.2.6/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.940913 FuncsForSPO-6.2.6/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.2.6/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.950923 FuncsForSPO-6.2.6/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39081 2023-06-26 14:06:50.000000 FuncsForSPO-6.2.6/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.963437 FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.973433 FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.978432 FuncsForSPO-6.2.6/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.2.6/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:27:55.678648 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2127 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-06-30 12:27:55.000000 FuncsForSPO-6.2.6/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.2.6/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-06-30 12:27:56.069297 FuncsForSPO-6.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 12:27:56.073574 FuncsForSPO-6.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2023-06-30 12:27:44.000000 FuncsForSPO-6.2.6/setup.py
```

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.2.6/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fgpt/__fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fgpt/fgpt.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fgpt/fgpt.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.2.6/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from FuncsForSPO.fpdf.fanalyser.__pdfanalyser import *
 
-def analyse_pdf_with_gpt(file_pdf:str, prompt:str, headless=True) -> str:
+def analyse_pdf_with_gpt(file_pdf:str, prompt:str, timeout=180, headless=True) -> str:
     """
     DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
     https://www.chatpdf.com/
 
 	"""
     # CREDENTIALS EXEMPLE -> (username, password)
-    app = GPTPDFV3(file_pdf=file_pdf, prompt=prompt, headless=headless)
+    app = GPTPDFV3(file_pdf=file_pdf, prompt=prompt, timeout=timeout, headless=headless)
     text = app.run()
     return text.replace('Olá, eu sou uma assistente de documentos multilíngue e estou aqui para ajudá-lo com qualquer dúvida que você possa ter sobre o documento que você enviou. ', '')
```

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import os
 import base64
 from tqdm import tqdm
 import gdown
 import pytesseract
 from PIL import Image
 import fitz
+import uuid
 
 class ErroAPI(Exception):
     pass
 
 def faz_ocr_em_pdf(file_pdf: str, type_extract='text', dir_exit: str='output', get_text_into_code: bool=True, headless: bool=True, prints=False) -> str:
     """
     ## DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
@@ -159,25 +160,31 @@
                 raise ErroAPI('ErroAPI')
             if response_json.get('status') == 'finalizado':
                 return response_json.get('result')
             else:
                 print(response_json.get('status'))
 
 
-def ocr_tesseract(pdf, dpi=300, config_tesseract=''):
+def ocr_tesseract(pdf, dpi=300, file_output=uuid.uuid4(), return_text=True, config_tesseract=''):
     """
-    Performs OCR (Optical Character Recognition) on a PDF file using Tesseract OCR engine. If Tesseract is not installed, it will be downloaded automatically. The function takes the following parameters:
-    
-    - pdf: The path to the PDF file to be processed.
-    - dpi (optional): The resolution of the output image in dots per inch. Defaults to 300 DPI.
-    - config_tesseract (optional): Additional configuration options to be passed to the Tesseract engine. Defaults to an empty string.
-    
-    Returns a string containing the text extracted from the PDF file.
+    Perform optical character recognition (OCR) on a PDF using Tesseract.
+
+    Args:
+        pdf (str): The path to the input PDF file.
+        dpi (int, optional): The resolution in dots per inch (DPI) for the OCR process. Defaults to 300.
+        file_output (str, optional): The output file name for the OCR result. Defaults to a randomly generated UUID.
+        return_text (bool, optional): Specifies whether to return the OCR result as a string directly in the code or as the path to the output file. Defaults to True.
+        config_tesseract (str, optional): Additional configuration options for Tesseract. Defaults to an empty string.
+
+    Returns:
+        str: The OCR result as a string if `return_text` is True, otherwise the path to the output file.
     """
 
+    # se for return_text, retornará o texto no diretamente no código, se for false, retornará o caminho do arquivo com a resposta do OCR
+
     path_exit = arquivo_com_caminho_absoluto('temp_tess', 'Tesseract-OCR.zip')
     path_tesseract_extract = arquivo_com_caminho_absoluto('bin', 'Tesseract-OCR')
     path_tesseract = arquivo_com_caminho_absoluto(('bin', 'Tesseract-OCR'), 'tesseract.exe')
 
     if not os.path.exists(path_tesseract):
         faz_log('Baixando binários do Tesseract, aguarde...')
         cria_dir_no_dir_de_trabalho_atual('temp_tess')
@@ -206,18 +213,26 @@
             for i, page in enumerate(pdf_fitz):
                 page = pdf_fitz.load_page(i)
                 mat = fitz.Matrix(dpi/72, dpi/72)  # Matriz de transformação usando DPI
                 pix = page.get_pixmap(matrix=mat)
                 image = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
                 image.save(f'pages/{i}.png')
                 bar.update(1)
-        all_text = ''
+        
 
         files = arquivos_com_caminho_absoluto_do_arquivo('pages')
         with tqdm(total=len(files), desc='OCR') as bar:
             for i, image in enumerate(files):
                 text = pytesseract.image_to_string(image, config=config_tesseract)
-                all_text += text
+                with open(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'), 'a', encoding='utf-8') as f:
+                    f.write(text)
                 bar.update(1)
             else:
                 limpa_diretorio('pages')
-                return all_text
+                if return_text:
+                    text_all = ''
+                    with open(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'), 'r', encoding='utf-8') as f:
+                        text_all = f.read()
+                    os.remove(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'))
+                    return text_all
+                else:
+                    return os.path.abspath(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'))
```

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.2.6/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.2.6/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.2.6/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.2.5
+Version: 6.2.6
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.2.5/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.2.6/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/LICENSE` & `FuncsForSPO-6.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/PKG-INFO` & `FuncsForSPO-6.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.2.5
+Version: 6.2.6
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.2.5/README.md` & `FuncsForSPO-6.2.6/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.5/setup.py` & `FuncsForSPO-6.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.2.5'
+version = '6.2.6'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

