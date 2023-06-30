# Comparing `tmp/archive-pdf-tools-1.5.3.tar.gz` & `tmp/archive-pdf-tools-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archive-pdf-tools-1.5.3.tar", last modified: Mon Mar 20 00:13:08 2023, max compression
+gzip compressed data, was "archive-pdf-tools-1.5.4.tar", last modified: Tue Jun 27 13:16:28 2023, max compression
```

## Comparing `archive-pdf-tools-1.5.3.tar` & `archive-pdf-tools-1.5.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.269822 archive-pdf-tools-1.5.3/.github/
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.273155 archive-pdf-tools-1.5.3/.github/workflows/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      810 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/.github/workflows/wheels.yml
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       52 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/.gitignore
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      635 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/.readthedocs.yaml
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.3/LICENSE
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.3/LICENSE.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       21 2021-10-05 14:47:09.000000 archive-pdf-tools-1.5.3/MANIFEST.in
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10238 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7772 2023-03-19 23:50:14.000000 archive-pdf-tools-1.5.3/README
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7772 2023-03-19 23:50:14.000000 archive-pdf-tools-1.5.3/README.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.273155 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10238 2023-03-20 00:13:08.000000 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1515 2023-03-20 00:13:08.000000 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/SOURCES.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2023-03-20 00:13:08.000000 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/dependency_links.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2021-10-04 21:17:33.000000 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/not-zip-safe
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      122 2023-03-20 00:13:08.000000 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/requires.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       37 2023-03-20 00:13:08.000000 archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/top_level.txt
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.273155 archive-pdf-tools-1.5.3/bin/
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     4924 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/bin/compress-pdf-images
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2302 2023-02-18 17:13:13.000000 archive-pdf-tools-1.5.3/bin/epub-to-pdf
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    14003 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/bin/pdf-metadata-json
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2256 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/bin/pdf-to-imagestack
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1007 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/bin/pdfcomp
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      915 2020-11-05 13:14:57.000000 archive-pdf-tools-1.5.3/bin/pdfrenderer
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    17632 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/bin/recode_pdf
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.273155 archive-pdf-tools-1.5.3/cython/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7629 2021-11-20 10:40:05.000000 archive-pdf-tools-1.5.3/cython/optimiser-wip2.pyx
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)   491346 2023-02-19 16:44:30.000000 archive-pdf-tools-1.5.3/cython/optimiser.c
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    15952 2023-02-18 17:14:21.000000 archive-pdf-tools-1.5.3/cython/optimiser.pyx
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     8885 2021-11-20 10:40:05.000000 archive-pdf-tools-1.5.3/cython/optimisest.pyx
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)   307935 2023-02-19 16:44:30.000000 archive-pdf-tools-1.5.3/cython/sauvola.c
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7205 2023-02-18 17:14:21.000000 archive-pdf-tools-1.5.3/cython/sauvola.pyx
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.273155 archive-pdf-tools-1.5.3/docs/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      638 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/Makefile
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      764 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/make.bat
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      155 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/docs/requirements.txt
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/docs/source/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2003 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/docs/source/conf.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      139 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/docs/source/cython.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1848 2022-08-30 10:34:07.000000 archive-pdf-tools-1.5.3/docs/source/example.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7912 2022-06-28 21:47:32.000000 archive-pdf-tools-1.5.3/docs/source/index.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      127 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/source/mrc.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      121 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/source/pagenumbers.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       97 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/docs/source/pdfhacks.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      109 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/source/pdfrenderer.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       99 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/source/recode.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      111 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/docs/source/scandata.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/internetarchivepdf/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      186 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/internetarchivepdf/__init__.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1948 2023-03-19 23:50:14.000000 archive-pdf-tools-1.5.3/internetarchivepdf/const.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/internetarchivepdf/data/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      572 2020-10-19 09:53:47.000000 archive-pdf-tools-1.5.3/internetarchivepdf/data/tesseract.ttf
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3144 2020-10-22 23:09:32.000000 archive-pdf-tools-1.5.3/internetarchivepdf/data/tmp.icc
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2414 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/internetarchivepdf/grayconvert.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     6949 2023-03-19 23:46:31.000000 archive-pdf-tools-1.5.3/internetarchivepdf/jpeg2000.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    23441 2023-03-19 23:17:04.000000 archive-pdf-tools-1.5.3/internetarchivepdf/mrc.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    13653 2023-03-18 21:29:46.000000 archive-pdf-tools-1.5.3/internetarchivepdf/pagenumbers.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      665 2020-11-14 23:10:10.000000 archive-pdf-tools-1.5.3/internetarchivepdf/pdffonts.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    15804 2022-08-30 10:34:07.000000 archive-pdf-tools-1.5.3/internetarchivepdf/pdfhacks.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    18822 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.3/internetarchivepdf/pdfrenderer.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1986 2021-11-27 18:51:55.000000 archive-pdf-tools-1.5.3/internetarchivepdf/profiles.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    29331 2023-03-19 23:50:14.000000 archive-pdf-tools-1.5.3/internetarchivepdf/recode.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2731 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.3/internetarchivepdf/scandata.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       97 2021-10-04 21:22:54.000000 archive-pdf-tools-1.5.3/pyproject.toml
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      155 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/requirements.txt
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      975 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.3/run-all-tools.sh
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1041 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/setup.cfg
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      963 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.3/setup.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-03-20 00:13:08.276488 archive-pdf-tools-1.5.3/tools/
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1783 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.3/tools/compress
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      874 2021-11-14 13:33:07.000000 archive-pdf-tools-1.5.3/tools/maskview
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      957 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.3/tools/merge
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      986 2021-10-05 14:47:09.000000 archive-pdf-tools-1.5.3/tools/mrcview
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1614 2021-10-05 11:41:42.000000 archive-pdf-tools-1.5.3/tools/partial-blur
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1187 2021-11-14 13:33:07.000000 archive-pdf-tools-1.5.3/tools/pdfimagesmrc
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     3801 2021-11-10 11:04:46.000000 archive-pdf-tools-1.5.3/tools/threshold-image
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.293362 archive-pdf-tools-1.5.4/
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.280028 archive-pdf-tools-1.5.4/.github/
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.283362 archive-pdf-tools-1.5.4/.github/workflows/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      816 2023-06-27 12:21:14.000000 archive-pdf-tools-1.5.4/.github/workflows/wheels.yml
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       52 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/.gitignore
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      635 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/.readthedocs.yaml
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.4/LICENSE
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.4/LICENSE.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       21 2021-10-05 14:47:09.000000 archive-pdf-tools-1.5.4/MANIFEST.in
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10238 2023-06-27 13:16:28.293362 archive-pdf-tools-1.5.4/PKG-INFO
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7772 2023-06-27 13:16:03.000000 archive-pdf-tools-1.5.4/README
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7772 2023-06-27 13:16:03.000000 archive-pdf-tools-1.5.4/README.rst
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.283362 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10238 2023-06-27 13:16:28.000000 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/PKG-INFO
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1515 2023-06-27 13:16:28.000000 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2023-06-27 13:16:28.000000 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2021-10-04 21:17:33.000000 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/not-zip-safe
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      122 2023-06-27 13:16:28.000000 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/requires.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       37 2023-06-27 13:16:28.000000 archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/top_level.txt
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.286695 archive-pdf-tools-1.5.4/bin/
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     4924 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.4/bin/compress-pdf-images
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2302 2023-04-03 23:13:30.000000 archive-pdf-tools-1.5.4/bin/epub-to-pdf
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    14003 2023-05-16 12:49:23.000000 archive-pdf-tools-1.5.4/bin/pdf-metadata-json
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2256 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.4/bin/pdf-to-imagestack
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1007 2023-02-23 15:56:52.000000 archive-pdf-tools-1.5.4/bin/pdfcomp
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      915 2020-11-05 13:14:57.000000 archive-pdf-tools-1.5.4/bin/pdfrenderer
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    17855 2023-06-27 09:53:48.000000 archive-pdf-tools-1.5.4/bin/recode_pdf
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.286695 archive-pdf-tools-1.5.4/cython/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7629 2021-11-20 10:40:05.000000 archive-pdf-tools-1.5.4/cython/optimiser-wip2.pyx
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)   482419 2023-06-27 13:16:27.000000 archive-pdf-tools-1.5.4/cython/optimiser.c
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    15952 2023-04-03 23:13:30.000000 archive-pdf-tools-1.5.4/cython/optimiser.pyx
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     8885 2021-11-20 10:40:05.000000 archive-pdf-tools-1.5.4/cython/optimisest.pyx
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)   299198 2023-06-27 13:16:28.000000 archive-pdf-tools-1.5.4/cython/sauvola.c
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7205 2023-04-03 23:13:30.000000 archive-pdf-tools-1.5.4/cython/sauvola.pyx
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.286695 archive-pdf-tools-1.5.4/docs/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      638 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/Makefile
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      764 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/make.bat
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      155 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/docs/requirements.txt
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.290028 archive-pdf-tools-1.5.4/docs/source/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2003 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/docs/source/conf.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      139 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/docs/source/cython.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1848 2022-08-30 10:34:07.000000 archive-pdf-tools-1.5.4/docs/source/example.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7912 2022-06-28 21:47:32.000000 archive-pdf-tools-1.5.4/docs/source/index.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      127 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/source/mrc.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      121 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/source/pagenumbers.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       97 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/docs/source/pdfhacks.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      109 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/source/pdfrenderer.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       99 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/source/recode.rst
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      111 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/docs/source/scandata.rst
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.290028 archive-pdf-tools-1.5.4/internetarchivepdf/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      186 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/internetarchivepdf/__init__.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1948 2023-06-27 13:16:03.000000 archive-pdf-tools-1.5.4/internetarchivepdf/const.py
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.290028 archive-pdf-tools-1.5.4/internetarchivepdf/data/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      572 2020-10-19 09:53:47.000000 archive-pdf-tools-1.5.4/internetarchivepdf/data/tesseract.ttf
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3144 2020-10-22 23:09:32.000000 archive-pdf-tools-1.5.4/internetarchivepdf/data/tmp.icc
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2414 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/internetarchivepdf/grayconvert.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     6949 2023-03-19 23:46:31.000000 archive-pdf-tools-1.5.4/internetarchivepdf/jpeg2000.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    23432 2023-06-27 13:16:03.000000 archive-pdf-tools-1.5.4/internetarchivepdf/mrc.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    13862 2023-06-27 09:53:48.000000 archive-pdf-tools-1.5.4/internetarchivepdf/pagenumbers.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      665 2020-11-14 23:10:10.000000 archive-pdf-tools-1.5.4/internetarchivepdf/pdffonts.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    15848 2023-06-27 09:53:48.000000 archive-pdf-tools-1.5.4/internetarchivepdf/pdfhacks.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    18822 2021-11-13 22:29:53.000000 archive-pdf-tools-1.5.4/internetarchivepdf/pdfrenderer.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1986 2021-11-27 18:51:55.000000 archive-pdf-tools-1.5.4/internetarchivepdf/profiles.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    29442 2023-06-27 13:16:03.000000 archive-pdf-tools-1.5.4/internetarchivepdf/recode.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2731 2022-05-07 12:08:08.000000 archive-pdf-tools-1.5.4/internetarchivepdf/scandata.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       97 2021-10-04 21:22:54.000000 archive-pdf-tools-1.5.4/pyproject.toml
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      150 2023-06-27 12:21:19.000000 archive-pdf-tools-1.5.4/requirements.txt
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      975 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.4/run-all-tools.sh
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1041 2023-06-27 13:16:28.293362 archive-pdf-tools-1.5.4/setup.cfg
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      963 2023-04-03 23:13:30.000000 archive-pdf-tools-1.5.4/setup.py
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-06-27 13:16:28.293362 archive-pdf-tools-1.5.4/tools/
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1783 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.4/tools/compress
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      874 2021-11-14 13:33:07.000000 archive-pdf-tools-1.5.4/tools/maskview
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      957 2021-07-05 20:22:56.000000 archive-pdf-tools-1.5.4/tools/merge
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      986 2021-10-05 14:47:09.000000 archive-pdf-tools-1.5.4/tools/mrcview
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1614 2021-10-05 11:41:42.000000 archive-pdf-tools-1.5.4/tools/partial-blur
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1187 2021-11-14 13:33:07.000000 archive-pdf-tools-1.5.4/tools/pdfimagesmrc
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     3801 2021-11-10 11:04:46.000000 archive-pdf-tools-1.5.4/tools/threshold-image
```

### Comparing `archive-pdf-tools-1.5.3/.github/workflows/wheels.yml` & `archive-pdf-tools-1.5.4/.github/workflows/wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 on: [push, pull_request]
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     env:
-      CIBW_BUILD: cp37-* cp38-* cp39-* cp310-*
+      CIBW_BUILD: cp37-* cp38-* cp39-* cp310-* cp311-*
       CIBW_SKIP: cp36-* *-win32 *-manylinux_i686 pp* *musllinux*
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macOS-10.15]
+        os: [ubuntu-20.04, windows-2019, macOS-11]
 
     steps:
       - uses: actions/checkout@v3
 
       # Used to host cibuildwheel
       - uses: actions/setup-python@v3
 
       - name: Install cibuildwheel
-        run: python -m pip install cibuildwheel==2.8.1
+        run: python -m pip install cibuildwheel==2.13.1
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
         env:
           CIBW_BEFORE_BUILD: python -m pip install -r requirements.txt
 
       - uses: actions/upload-artifact@v3
```

### Comparing `archive-pdf-tools-1.5.3/.readthedocs.yaml` & `archive-pdf-tools-1.5.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/LICENSE` & `archive-pdf-tools-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/LICENSE.txt` & `archive-pdf-tools-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/PKG-INFO` & `archive-pdf-tools-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: archive-pdf-tools
-Version: 1.5.3
+Version: 1.5.4
 Summary: Internet Archive PDF compression tools
 Home-page: https://github.com/internetarchive/archive-pdf-tools
 Author: Merlijn Boris Wolf Wajer
 Author-email: merlijn@archive.org
 License: AGPL-3.0
-Download-URL: https://github.com/internetarchive/archive-pdf-tools/archive/1.5.3.tar.gz
+Download-URL: https://github.com/internetarchive/archive-pdf-tools/archive/1.5.4.tar.gz
 Description: Internet Archive PDF tools
         ##########################
         
         :authors: - Merlijn Wajer <merlijn@archive.org>
         :date: 2021-11-14 18:00
         
         This repository contains a library to perform MRC (Mixed Raster Content)
```

### Comparing `archive-pdf-tools-1.5.3/README` & `archive-pdf-tools-1.5.4/README`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/README.rst` & `archive-pdf-tools-1.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/PKG-INFO` & `archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: archive-pdf-tools
-Version: 1.5.3
+Version: 1.5.4
 Summary: Internet Archive PDF compression tools
 Home-page: https://github.com/internetarchive/archive-pdf-tools
 Author: Merlijn Boris Wolf Wajer
 Author-email: merlijn@archive.org
 License: AGPL-3.0
-Download-URL: https://github.com/internetarchive/archive-pdf-tools/archive/1.5.3.tar.gz
+Download-URL: https://github.com/internetarchive/archive-pdf-tools/archive/1.5.4.tar.gz
 Description: Internet Archive PDF tools
         ##########################
         
         :authors: - Merlijn Wajer <merlijn@archive.org>
         :date: 2021-11-14 18:00
         
         This repository contains a library to perform MRC (Mixed Raster Content)
```

### Comparing `archive-pdf-tools-1.5.3/archive_pdf_tools.egg-info/SOURCES.txt` & `archive-pdf-tools-1.5.4/archive_pdf_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/compress-pdf-images` & `archive-pdf-tools-1.5.4/bin/compress-pdf-images`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/epub-to-pdf` & `archive-pdf-tools-1.5.4/bin/epub-to-pdf`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/pdf-metadata-json` & `archive-pdf-tools-1.5.4/bin/pdf-metadata-json`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/pdf-to-imagestack` & `archive-pdf-tools-1.5.4/bin/pdf-to-imagestack`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/pdfcomp` & `archive-pdf-tools-1.5.4/bin/pdfcomp`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/pdfrenderer` & `archive-pdf-tools-1.5.4/bin/pdfrenderer`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/bin/recode_pdf` & `archive-pdf-tools-1.5.4/bin/recode_pdf`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,16 @@
                                'If multiple languages are specified, only the '
                                'first is added to the PDF catalog, but all of '
                                'them will end up in the XMP metadata')
     metadata_args.add_argument('--metadata-subject', type=str, default=None,
                                help='Subjects')
     metadata_args.add_argument('--metadata-creatortool', type=str, default=None,
                                help='Creator tool')
+    metadata_args.add_argument('--ignore-invalid-pagenumbers', action='store_true',
+                               help='Do not error if scandata has invalid page numbers')
 
     args = parser.parse_args()
     if (args.from_pdf is None and args.from_imagestack is None) or args.out_pdf is None:
         sys.stderr.write('***** Error: --from-pdf or --out-pdf missing\n\n')
         parser.print_help()
         sys.exit(1)
 
@@ -316,13 +318,14 @@
                  args.hq_pages,
                  args.hq_bg_compression_flags.split(' '),
                  args.hq_fg_compression_flags.split(' '),
                  args.threads,
                  args.render_text_lines,
                  args.metadata_url, args.metadata_title, args.metadata_author,
                  args.metadata_creator, args.metadata_language,
-                 args.metadata_subject, args.metadata_creatortool)
+                 args.metadata_subject, args.metadata_creatortool,
+                 args.ignore_invalid_pagenumbers)
 
     errors = res['errors']
     if len(errors) > 0:
         for error in errors:
             print('Encountered runtime error:', error)
```

### Comparing `archive-pdf-tools-1.5.3/cython/optimiser-wip2.pyx` & `archive-pdf-tools-1.5.4/cython/optimiser-wip2.pyx`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/cython/optimiser.c` & `archive-pdf-tools-1.5.4/cython/optimiser.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.23 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "optimiser",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_23"
+#define CYTHON_HEX_VERSION 0x001D17F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,15 +58,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -95,22 +94,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -140,67 +135,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -220,64 +166,53 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -386,76 +321,17 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return co;
-    }
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -561,33 +437,25 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -685,18 +553,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -713,18 +581,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -856,15 +722,14 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -992,16 +857,16 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
   "cython/optimiser.pyx",
-  "__init__.pxd",
-  "type.pxd",
+  "venv/lib/python3.8/site-packages/numpy/__init__.pxd",
+  "venv/lib/python3.8/site-packages/Cython/Includes/cpython/type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
@@ -1032,195 +897,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1265,42 +1130,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1482,29 +1347,21 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -7042,15 +6899,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_mask.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7059,29 +6916,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7092,15 +6949,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7109,29 +6966,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7142,15 +6999,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7159,29 +7016,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7192,15 +7049,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7209,29 +7066,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7242,15 +7099,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7259,29 +7116,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7292,212 +7149,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7513,15 +7370,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7529,84 +7386,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7621,15 +7478,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7645,15 +7502,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7661,84 +7518,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7753,15 +7610,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7777,15 +7634,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7793,84 +7650,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7885,176 +7742,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8184,43 +8041,43 @@
   {&__pyx_n_s_ys, __pyx_k_ys, sizeof(__pyx_k_ys), 0, 0, 1, 1},
   {&__pyx_n_s_yy, __pyx_k_yy, sizeof(__pyx_k_yy), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 49, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "optimiser.pyx":22
  * @cython.cdivision(True)
  * @cython.warn.undeclared(True)
  * def optimise_gray(np.ndarray[UINT8DTYPE_t, ndim=2] mask,             # <<<<<<<<<<<<<<
@@ -8348,46 +8205,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8551,17 +8408,19 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("optimiser", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -8718,15 +8577,15 @@
  * # * Bas Weelinck <bas@weelinck.org> - fast versions
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -9727,15 +9586,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -10353,15 +10212,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -10447,48 +10306,41 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -10499,49 +10351,34 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -11470,41 +11307,19 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -11754,31 +11569,14 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `archive-pdf-tools-1.5.3/cython/optimiser.pyx` & `archive-pdf-tools-1.5.4/cython/optimiser.pyx`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/cython/optimisest.pyx` & `archive-pdf-tools-1.5.4/cython/optimisest.pyx`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/cython/sauvola.c` & `archive-pdf-tools-1.5.4/cython/sauvola.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.23 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "sauvola",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_23"
+#define CYTHON_HEX_VERSION 0x001D17F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,15 +58,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -95,22 +94,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -140,67 +135,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -220,64 +166,53 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -386,76 +321,17 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return co;
-    }
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -561,33 +437,25 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -685,18 +553,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -713,18 +581,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -856,15 +722,14 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -992,16 +857,16 @@
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
   "cython/sauvola.pyx",
-  "__init__.pxd",
-  "type.pxd",
+  "venv/lib/python3.8/site-packages/numpy/__init__.pxd",
+  "venv/lib/python3.8/site-packages/Cython/Includes/cpython/type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
@@ -1032,195 +897,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1265,42 +1130,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3678,15 +3543,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_integral);
   __Pyx_XDECREF((PyObject *)__pyx_v_integral_square);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3695,29 +3560,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3728,15 +3593,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3745,29 +3610,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3778,15 +3643,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3795,29 +3660,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3828,15 +3693,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3845,29 +3710,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3878,15 +3743,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3895,29 +3760,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3928,212 +3793,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4149,15 +4014,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4165,84 +4030,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4257,15 +4122,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4281,15 +4146,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4297,84 +4162,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4389,15 +4254,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4413,15 +4278,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4429,84 +4294,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4521,176 +4386,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4808,43 +4673,43 @@
   {&__pyx_n_s_window_height, __pyx_k_window_height, sizeof(__pyx_k_window_height), 0, 0, 1, 1},
   {&__pyx_n_s_window_width, __pyx_k_window_width, sizeof(__pyx_k_window_width), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 70, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "sauvola.pyx":29
  * # the window
  * @cython.warn.undeclared(True)
  * def binarise_sauvola(np.ndarray[UINT8DTYPE_t, ndim=1] in_arr, np.ndarray[UINT8DTYPE_t, ndim=1] out_arr, int width, int height, int window_width, int window_height, double k, double R):             # <<<<<<<<<<<<<<
@@ -4925,46 +4790,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5128,17 +4993,19 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("sauvola", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -5248,15 +5115,15 @@
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_binarise_sauvola_line_29, __pyx_kp_u_Perform_fast_Sauvola_binarisati) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../usr/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "venv/lib/python3.8/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6115,15 +5982,15 @@
     return __Pyx_GetBuiltinName(name);
 }
 
 /* PyObjectCall */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -6640,15 +6507,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -6734,48 +6601,41 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -6786,49 +6646,34 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -7757,41 +7602,19 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -8041,31 +7864,14 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `archive-pdf-tools-1.5.3/cython/sauvola.pyx` & `archive-pdf-tools-1.5.4/cython/sauvola.pyx`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/docs/Makefile` & `archive-pdf-tools-1.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/docs/make.bat` & `archive-pdf-tools-1.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/docs/source/conf.py` & `archive-pdf-tools-1.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/docs/source/example.rst` & `archive-pdf-tools-1.5.4/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/docs/source/index.rst` & `archive-pdf-tools-1.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/const.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Author: Merlijn Boris Wolf Wajer <merlijn@archive.org>
 
-VERSION = '1.5.3'
+VERSION = '1.5.4'
 
 PRODUCER = 'Internet Archive PDF %s; including '\
            'mupdf and pymupdf/skimage' % (VERSION,)
 
 
 IMAGE_MODE_PASSTHROUGH = 0
 IMAGE_MODE_PIXMAP = 1
```

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/data/tesseract.ttf` & `archive-pdf-tools-1.5.4/internetarchivepdf/data/tesseract.ttf`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/data/tmp.icc` & `archive-pdf-tools-1.5.4/internetarchivepdf/data/tmp.icc`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/grayconvert.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/grayconvert.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/jpeg2000.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/jpeg2000.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/mrc.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/mrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     if dpi is not None:
         window_size = int(dpi / 4)
         if window_size % 2 == 0:
             window_size += 1
 
     h, w = img.shape
-    out_img = np.ndarray(img.shape, dtype=np.bool)
+    out_img = np.ndarray(img.shape, dtype=bool)
     out_img = np.reshape(out_img, w*h)
     in_img = np.reshape(img, w*h)
 
     binarise_sauvola(in_img, out_img, w, h, window_size, window_size, k, 128)
     out_img = np.reshape(out_img, (h, w))
     # TODO: optimise this, we can do it in binarise_sauvola
     out_img = np.invert(out_img)
@@ -99,15 +99,15 @@
     """
     thresf = np.array(binary_img, dtype=np.float32)
     #denoise = denoise_tv_bregman(thresf, weight=0.25)
     denoise = denoise_tv_bregman(thresf, weight=1.)
 
     #denoise = denoise > 0.6
     denoise = denoise > 0.4  # XXX: 0.4?
-    denoise = np.array(denoise, dtype=np.bool)
+    denoise = np.array(denoise, dtype=bool)
 
     return denoise
 
 # TODO: Rename, can be either foreground or background
 def partial_blur(mask, img, sigma=5, mode=None):
     """
     Blur a part of the image 'img', where mask = 0.
@@ -370,15 +370,15 @@
     create_hocr_mask(grayimg, mask_arr, hocr_word_data, downsample=downsample,
                      dpi=dpi, timing_data=timing_data)
     grayimgf = np.array(grayimg, dtype=np.float32)
 
     MIX_THRESHOLD = True
     if MIX_THRESHOLD:
         # XXX: this nukes the hocr threshold, testing only
-        # mask_arr = np.zeros(mask_arr.shape, dtype=np.bool)
+        # mask_arr = np.zeros(mask_arr.shape, dtype=bool)
 
         # Modifies mask_arr in place
         create_threshold_mask(mask_arr, grayimgf, dpi=dpi,
                               denoise_mask=denoise_mask,
                               timing_data=timing_data)
 
     if denoise_mask != DENOISE_NONE:
```

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/pagenumbers.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/pagenumbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             first = False
         else:
             res += 26 - tmp
 
     return res
 
 
-def get_val_type(v):
+def get_val_type(v, ignore_invalid=False):
     if v is None:
         # XXX: Does this special case make sense?
         return INVALID
     elif is_arabic(v):
         return ARABIC
     # Prefer roman over alpha since we do not yet support alpha
     elif is_roman_lower(v):
@@ -111,15 +111,18 @@
     elif is_roman_upper(v):
         return ROMAN_UPPER
     elif is_alpha_upper(v):
         return ALPHA_UPPER
     elif is_alpha_lower(v):
         return ALPHA_LOWER
     else:
-        raise ValueError('Page number not in spec: %s' % repr(v))
+        if ignore_invalid:
+            return INVALID
+        else:
+            raise ValueError('Page number not in spec: %s' % repr(v))
 
 
 def get_val_value(v, vtype):
     if v and ' ' in v:
         v = v.strip().split(' ')[0]
     if vtype == INVALID:
         return None
@@ -138,15 +141,15 @@
 def find_next_nonzero(series):
     for v in series:
         if v is not None:
             return v
     return None
 
 
-def parse_series(series):
+def parse_series(series, ignore_invalid=False):
     # Let's first split up the series:
     # - detect when the numbers are not in sequence
     # - detect when the type changes
     last_value = None
     last_val_type = INVALID
 
     series_start = 0
@@ -157,34 +160,34 @@
     running_series = []
     running_series_n = []
 
     for idx, val in enumerate(series):
         new = False
 
         try:
-            val_type = get_val_type(val)
+            val_type = get_val_type(val, ignore_invalid=ignore_invalid)
             val_value = get_val_value(val, val_type)
         except ValueError as e:
             all_ok = False
             val_type = INVALID
             val_value = None
 
         if val_type in (ROMAN_UPPER, ROMAN_LOWER):
             next_val = find_next_nonzero(series[idx+1:])
-            next_val_type = get_val_type(next_val)
+            next_val_type = get_val_type(next_val, ignore_invalid=ignore_invalid)
 
             if val_type != next_val_type:
                 if val_type == ROMAN_UPPER and next_val_type == ALPHA_UPPER or \
                         val_type == ROMAN_LOWER and next_val_type == ALPHA_LOWER:
                     val_type = next_val_type
                     val_value = get_val_value(val, val_type)
 
         if val_type in (ALPHA_UPPER, ALPHA_LOWER):
             next_val = find_next_nonzero(series[idx+1:])
-            next_val_type = get_val_type(next_val)
+            next_val_type = get_val_type(next_val, ignore_invalid=ignore_invalid)
 
             ord_val = None
             ord_next_val = None
             try:
                 ord_val = ord(val)
                 ord_next_val = ord(next_val)
             except TypeError:
```

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/pdffonts.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/pdffonts.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/pdfhacks.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/pdfhacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,17 +203,17 @@
     s = to_pdf.xref_object(to_pdf.pdf_catalog())
     s = s[:-2]
     s += '  /OutputIntents [ %d 0 R ]' % intentxref
     s += '>>'
     to_pdf.update_object(catalogxref, s)
 
 
-def write_page_labels(to_pdf, scandata, errors=None):
+def write_page_labels(to_pdf, scandata, errors=None, ignore_invalid=False):
     page_numbers = scandata_xml_get_page_numbers(scandata)
-    res, all_ok = parse_series(page_numbers)
+    res, all_ok = parse_series(page_numbers, ignore_invalid=False)
 
     # Add warning/error
     if errors is not None and not all_ok:
         errors.add(RECODE_RUNTIME_WARNING_INVALID_PAGE_NUMBERS)
 
     catalogxref = to_pdf.pdf_catalog()
     s = to_pdf.xref_object(to_pdf.pdf_catalog())
```

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/pdfrenderer.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/pdfrenderer.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/profiles.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/profiles.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/recode.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/recode.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,15 +578,16 @@
         denoise_mask=None,
         hq_pages=None,
         hq_bg_compression_flags=None, hq_fg_compression_flags=None,
         threads=None,
         render_text_lines=False,
         metadata_url=None, metadata_title=None, metadata_author=None,
         metadata_creator=None, metadata_language=None,
-        metadata_subject=None, metadata_creatortool=None):
+        metadata_subject=None, metadata_creatortool=None,
+        ignore_invalid_pagenumbers=False):
     # TODO: document that the scandata document dpi will override the dpi arg
     # TODO: Take hq-pages and reporter arg and change format (as lib call we
     # don't want to pass that as one string, I guess?)
 
     errors = set()
 
     in_pdf = None
@@ -718,15 +719,16 @@
 
     # 3. Add PDF/A compliant data
     write_pdfa(outdoc)
 
     if scandata_file is not None:
         # XXX: we parse scandata twice now, let's not do that
         # 3b. Write page labels from scandata file, if present
-        write_page_labels(outdoc, scandata_file, errors=errors)
+        write_page_labels(outdoc, scandata_file, errors=errors,
+                          ignore_invalid=ignore_invalid_pagenumbers)
 
 
     lang_if_any = metadata_language[0] if metadata_language else None
     write_basic_ua(outdoc, language=lang_if_any)
 
     # 4. Write metadata
     extra_metadata = {}
```

### Comparing `archive-pdf-tools-1.5.3/internetarchivepdf/scandata.py` & `archive-pdf-tools-1.5.4/internetarchivepdf/scandata.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/run-all-tools.sh` & `archive-pdf-tools-1.5.4/run-all-tools.sh`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/setup.cfg` & `archive-pdf-tools-1.5.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	tools/pdfimagesmrc
 include_package_data = true
 zip_safe = false
 python_requires = >=3.6
 install_requires = 
 	PyMuPDF >=1.19
 	Pillow >=8.3
-	archive_hocr_tools >=1.1.13
+	archive_hocr_tools >=1.1.41
 	xmltodict >=0.12
 	roman >=3.3
 	numpy
 	lxml
 	scikit-image
 
 [options.package_data]
```

### Comparing `archive-pdf-tools-1.5.3/setup.py` & `archive-pdf-tools-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/compress` & `archive-pdf-tools-1.5.4/tools/compress`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/maskview` & `archive-pdf-tools-1.5.4/tools/maskview`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/merge` & `archive-pdf-tools-1.5.4/tools/merge`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/mrcview` & `archive-pdf-tools-1.5.4/tools/mrcview`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/partial-blur` & `archive-pdf-tools-1.5.4/tools/partial-blur`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/pdfimagesmrc` & `archive-pdf-tools-1.5.4/tools/pdfimagesmrc`

 * *Files identical despite different names*

### Comparing `archive-pdf-tools-1.5.3/tools/threshold-image` & `archive-pdf-tools-1.5.4/tools/threshold-image`

 * *Files identical despite different names*

