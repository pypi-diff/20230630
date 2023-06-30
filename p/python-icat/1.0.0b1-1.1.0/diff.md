# Comparing `tmp/python-icat-1.0.0b1.tar.gz` & `tmp/python-icat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-icat-1.0.0b1.tar", last modified: Wed Nov 23 22:10:29 2022, max compression
+gzip compressed data, was "dist/python-icat-1.1.0.tar", last modified: Fri Jun 30 07:06:24 2023, max compression
```

## Comparing `python-icat-1.0.0b1.tar` & `python-icat-1.1.0.tar`

### file list

```diff
@@ -1,122 +1,143 @@
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    48818 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/CHANGES.rst
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    11358 2022-07-22 14:52:38.000000 python-icat-1.0.0b1/LICENSE.txt
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      471 2022-11-07 15:09:32.000000 python-icat-1.0.0b1/MANIFEST.in
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    11787 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/PKG-INFO
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     8751 2022-11-23 21:36:22.000000 python-icat-1.0.0b1/README.rst
--rw-r--r--   0 jsi      (14523) hzbited  (32415)       26 2022-11-23 22:10:18.000000 python-icat-1.0.0b1/_meta.py
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/doc/
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/doc/examples/
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     6203 2022-11-23 21:03:23.000000 python-icat-1.0.0b1/doc/examples/add-investigation-data.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     7138 2022-11-23 21:06:21.000000 python-icat-1.0.0b1/doc/examples/add-job.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     3685 2022-11-23 21:05:19.000000 python-icat-1.0.0b1/doc/examples/addfile.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     3193 2022-11-23 20:59:49.000000 python-icat-1.0.0b1/doc/examples/create-datafile.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     6803 2022-11-23 21:02:24.000000 python-icat-1.0.0b1/doc/examples/create-investigation.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     1611 2022-11-23 21:00:34.000000 python-icat-1.0.0b1/doc/examples/create-parametertypes.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     2070 2022-11-23 21:02:42.000000 python-icat-1.0.0b1/doc/examples/create-sampletype.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     4845 2022-08-13 19:23:53.000000 python-icat-1.0.0b1/doc/examples/downloaddata.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     6889 2022-08-13 19:23:54.000000 python-icat-1.0.0b1/doc/examples/dumpinvestigation.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     1609 2022-08-13 19:23:54.000000 python-icat-1.0.0b1/doc/examples/dumprules.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    18299 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/example_data.yaml
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)      490 2022-08-13 19:23:54.000000 python-icat-1.0.0b1/doc/examples/getversion.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1626 2022-07-22 14:52:39.000000 python-icat-1.0.0b1/doc/examples/icat.cfg
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    71747 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-4.10.xml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    53970 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-4.10.yaml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    69389 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-4.4.xml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    52171 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-4.4.yaml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    70332 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-4.7.xml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    52863 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-4.7.yaml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    92802 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-5.0.xml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    70016 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/examples/icatdump-5.0.yaml
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     2963 2022-08-13 19:23:59.000000 python-icat-1.0.0b1/doc/examples/icatexport.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     2745 2022-08-13 19:23:59.000000 python-icat-1.0.0b1/doc/examples/icatimport.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)      756 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/examples/icatsummary.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      828 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/examples/ingest-datafiles.xml
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      911 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/examples/ingest-ds-params.xml
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)    21489 2022-11-23 21:05:04.000000 python-icat-1.0.0b1/doc/examples/init-icat.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)      345 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/examples/login.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     7023 2022-11-23 21:00:18.000000 python-icat-1.0.0b1/doc/examples/paramtype.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     6555 2022-08-13 19:24:06.000000 python-icat-1.0.0b1/doc/examples/querytest.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    40444 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/icatdata-4.10.xsd
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    38985 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/icatdata-4.3.xsd
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    39597 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/icatdata-4.4.xsd
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    39780 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/icatdata-4.7.xsd
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    53336 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/doc/icatdata-5.0.xsd
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/doc/man/
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     5839 2022-11-23 22:10:18.000000 python-icat-1.0.0b1/doc/man/icatdump.1
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     6784 2022-11-23 22:10:18.000000 python-icat-1.0.0b1/doc/man/icatingest.1
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     4774 2022-11-23 22:10:18.000000 python-icat-1.0.0b1/doc/man/wipeicat.1
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/doc/tutorial/
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      554 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/config-custom.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      754 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/config-flag.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      335 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/config-preset.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1904 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/config-sub-commands.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      364 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/config-with-ids.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      214 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/config.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      164 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/hello-client.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      195 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/hello-nocert.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      178 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/hello.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      266 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/doc/tutorial/login.py
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/icat/
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      377 2022-11-23 22:10:18.000000 python-icat-1.0.0b1/icat/__init__.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     3631 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/icat/authinfo.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     6978 2022-07-22 14:52:40.000000 python-icat-1.0.0b1/icat/chunkedhttp.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    38740 2022-11-23 20:58:32.000000 python-icat-1.0.0b1/icat/client.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    35574 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/config.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     8573 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/icat/dump_queries.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    16559 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/icat/dumpfile.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     9164 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/dumpfile_xml.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     7928 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/icat/dumpfile_yaml.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     9322 2022-11-23 20:50:41.000000 python-icat-1.0.0b1/icat/entities.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    18144 2022-11-23 20:57:00.000000 python-icat-1.0.0b1/icat/entity.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      970 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/eval.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    12913 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/exception.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     7904 2022-11-07 15:09:32.000000 python-icat-1.0.0b1/icat/helper.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    19849 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/icat/ids.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     4376 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/listproxy.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    23917 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/query.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1439 2022-07-22 14:52:41.000000 python-icat-1.0.0b1/icat/sslcontext.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     2408 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/icatdump.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     3495 2022-07-22 14:52:42.000000 python-icat-1.0.0b1/icatingest.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     6676 2022-11-23 20:15:23.000000 python-icat-1.0.0b1/setup.py
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/tests/
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     7832 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/conftest.py
-drwxr-xr-x   0 jsi      (14523) hzbited  (32415)        0 2022-11-23 22:10:29.000000 python-icat-1.0.0b1/tests/data/
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1197 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1189 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4.acord
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1186 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4.ahau
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1187 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4.jbotu
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1186 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4.jdoe
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1189 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4.nbour
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1187 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-4.rbeck
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1608 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1600 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5.acord
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1597 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5.ahau
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1598 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5.jbotu
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1597 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5.jdoe
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1600 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5.nbour
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1598 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/data/summary-5.rbeck
--rw-r--r--   0 jsi      (14523) hzbited  (32415)       86 2022-07-22 14:52:42.000000 python-icat-1.0.0b1/tests/pytest.ini
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    46140 2022-08-13 19:24:06.000000 python-icat-1.0.0b1/tests/test_01_config.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     7315 2022-11-07 15:09:32.000000 python-icat-1.0.0b1/tests/test_01_helper.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1661 2022-07-22 14:52:42.000000 python-icat-1.0.0b1/tests/test_01_listproxy.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1344 2022-07-22 14:52:42.000000 python-icat-1.0.0b1/tests/test_03_getversion.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     3085 2022-07-22 14:52:42.000000 python-icat-1.0.0b1/tests/test_03_login.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      611 2022-07-22 14:52:42.000000 python-icat-1.0.0b1/tests/test_03_script.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     7159 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/test_05_dump.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     6813 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/test_05_dumpfile.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    17599 2022-11-23 20:46:42.000000 python-icat-1.0.0b1/tests/test_05_setup.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    17245 2022-11-23 20:53:30.000000 python-icat-1.0.0b1/tests/test_06_client.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     4989 2022-11-23 20:38:25.000000 python-icat-1.0.0b1/tests/test_06_exception.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    15912 2022-11-23 20:54:48.000000 python-icat-1.0.0b1/tests/test_06_ids.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    11626 2022-11-23 21:10:18.000000 python-icat-1.0.0b1/tests/test_06_ingest.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    39466 2022-11-23 20:15:24.000000 python-icat-1.0.0b1/tests/test_06_query.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     1823 2022-07-22 14:52:43.000000 python-icat-1.0.0b1/tests/test_07_client_clone.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     2152 2022-07-22 14:52:43.000000 python-icat-1.0.0b1/tests/test_07_client_options.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     4941 2022-07-22 14:52:43.000000 python-icat-1.0.0b1/tests/test_07_dataselection.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     2696 2022-11-23 20:37:47.000000 python-icat-1.0.0b1/tests/test_07_entity_copy.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     5128 2022-11-23 20:42:50.000000 python-icat-1.0.0b1/tests/test_07_entity_equal.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)    11394 2022-11-23 21:15:00.000000 python-icat-1.0.0b1/tests/test_07_entity_sort.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)     5542 2022-11-23 20:32:39.000000 python-icat-1.0.0b1/tests/test_07_entity_validate.py
--rw-r--r--   0 jsi      (14523) hzbited  (32415)      310 2022-07-22 14:52:43.000000 python-icat-1.0.0b1/tests/test_09_deprecations.py
--rwxr-xr-x   0 jsi      (14523) hzbited  (32415)     6331 2022-07-22 14:52:43.000000 python-icat-1.0.0b1/wipeicat.py
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/
+-rw-r--r--   0 rolf      (1000) rk        (1000)    50863 2023-06-30 07:04:54.000000 python-icat-1.1.0/CHANGES.rst
+-rw-r--r--   0 rolf      (1000) rk        (1000)    11358 2021-04-13 17:57:18.000000 python-icat-1.1.0/LICENSE.txt
+-rw-r--r--   0 rolf      (1000) rk        (1000)      759 2023-06-30 07:04:54.000000 python-icat-1.1.0/MANIFEST.in
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4199 2023-06-30 07:06:22.000000 python-icat-1.1.0/PKG-INFO
+-rw-r--r--   0 rolf      (1000) rk        (1000)     2330 2023-06-30 07:04:54.000000 python-icat-1.1.0/README.rst
+-rw-r--r--   0 rolf      (1000) rk        (1000)       24 2023-06-30 07:06:22.000000 python-icat-1.1.0/_meta.py
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/examples/
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     6203 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/add-investigation-data.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     7138 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/add-job.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     3685 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/addfile.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     3208 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/examples/create-datafile.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     6803 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/create-investigation.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     1611 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/create-parametertypes.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     2070 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/create-sampletype.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     4845 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/downloaddata.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     6889 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/dumpinvestigation.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     1609 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/dumprules.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    18299 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/example_data.yaml
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)      490 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/getversion.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1626 2021-04-13 17:57:18.000000 python-icat-1.1.0/doc/examples/icat.cfg
+-rw-r--r--   0 rolf      (1000) rk        (1000)    71739 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-4.10.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    53962 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-4.10.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    69381 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-4.4.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    52163 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-4.4.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    70324 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-4.7.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    52855 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-4.7.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    92794 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-5.0.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    70008 2023-05-25 12:09:39.000000 python-icat-1.1.0/doc/examples/icatdump-5.0.yaml
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     2963 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/icatexport.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     2745 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/icatimport.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)      756 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/icatsummary.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      828 2021-04-13 17:57:18.000000 python-icat-1.1.0/doc/examples/ingest-datafiles.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)      911 2021-04-13 17:57:18.000000 python-icat-1.1.0/doc/examples/ingest-ds-params.xml
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     5613 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/examples/ingest.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)    21489 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/init-icat.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)      345 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/login.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     2235 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/examples/metadata-4.4-inl.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)     2589 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/examples/metadata-4.4-sep.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)     2643 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/examples/metadata-5.0-inl.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)     3097 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/examples/metadata-5.0-sep.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)     7023 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/paramtype.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     6555 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/examples/querytest.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    41505 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/icatdata-4.10.xsd
+-rw-r--r--   0 rolf      (1000) rk        (1000)    39141 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/icatdata-4.3.xsd
+-rw-r--r--   0 rolf      (1000) rk        (1000)    39753 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/icatdata-4.4.xsd
+-rw-r--r--   0 rolf      (1000) rk        (1000)    40385 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/icatdata-4.7.xsd
+-rw-r--r--   0 rolf      (1000) rk        (1000)    54523 2023-06-30 07:04:54.000000 python-icat-1.1.0/doc/icatdata-5.0.xsd
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/man/
+-rw-r--r--   0 rolf      (1000) rk        (1000)     5839 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/man/icatdump.1
+-rw-r--r--   0 rolf      (1000) rk        (1000)     6784 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/man/icatingest.1
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4774 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/man/wipeicat.1
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/doc/tutorial/
+-rw-r--r--   0 rolf      (1000) rk        (1000)      554 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/config-custom.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      754 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/config-flag.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      335 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/config-preset.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1904 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/config-sub-commands.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      364 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/config-with-ids.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      214 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/config.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      164 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/hello-client.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      195 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/hello-nocert.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      178 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/hello.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      266 2022-12-21 14:53:24.000000 python-icat-1.1.0/doc/tutorial/login.py
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/etc/
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4476 2023-06-30 07:04:55.000000 python-icat-1.1.0/etc/ingest-10.xsd
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1194 2023-06-30 07:04:55.000000 python-icat-1.1.0/etc/ingest.xslt
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/icat/
+-rw-r--r--   0 rolf      (1000) rk        (1000)      375 2023-06-30 07:06:22.000000 python-icat-1.1.0/icat/__init__.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     3631 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/authinfo.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     6978 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/chunkedhttp.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    39185 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/client.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    35941 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/config.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     9524 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/dump_queries.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    16575 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/dumpfile.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     8881 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/dumpfile_xml.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     7666 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/dumpfile_yaml.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     9511 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/entities.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    18948 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/entity.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      970 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/eval.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    13379 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/exception.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     7933 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/helper.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    19849 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/ids.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     7782 2023-06-30 07:04:55.000000 python-icat-1.1.0/icat/ingest.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4376 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/listproxy.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    23917 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/query.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1439 2022-12-21 14:53:24.000000 python-icat-1.1.0/icat/sslcontext.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     2408 2022-12-21 14:53:24.000000 python-icat-1.1.0/icatdump.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     3495 2022-12-21 14:53:24.000000 python-icat-1.1.0/icatingest.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     7344 2023-06-30 07:04:55.000000 python-icat-1.1.0/setup.py
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/tests/
+-rw-r--r--   0 rolf      (1000) rk        (1000)     8193 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/conftest.py
+drwxr-xr-x   0 rolf      (1000) rk        (1000)        0 2023-06-30 07:06:22.000000 python-icat-1.1.0/tests/data/
+-rw-r--r--   0 rolf      (1000) rk        (1000)    71723 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/legacy-icatdump-4.10.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    53957 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/legacy-icatdump-4.10.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    69365 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/legacy-icatdump-4.4.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    52158 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/legacy-icatdump-4.4.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    70308 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/legacy-icatdump-4.7.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    52850 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/legacy-icatdump-4.7.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)      940 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/data/metadata-5.0-badref.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    72354 2023-05-25 12:09:39.000000 python-icat-1.1.0/tests/data/ref-icatdump-5.0.xml
+-rw-r--r--   0 rolf      (1000) rk        (1000)    54324 2023-05-25 12:09:39.000000 python-icat-1.1.0/tests/data/ref-icatdump-5.0.yaml
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1197 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1189 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4.acord
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1186 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4.ahau
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1187 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4.jbotu
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1186 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4.jdoe
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1189 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4.nbour
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1187 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-4.rbeck
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1608 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1600 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5.acord
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1597 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5.ahau
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1598 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5.jbotu
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1597 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5.jdoe
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1600 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5.nbour
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1598 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/data/summary-5.rbeck
+-rw-r--r--   0 rolf      (1000) rk        (1000)       86 2021-04-13 17:57:18.000000 python-icat-1.1.0/tests/pytest.ini
+-rw-r--r--   0 rolf      (1000) rk        (1000)    46140 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_01_config.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     7315 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_01_helper.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1661 2021-04-13 17:57:19.000000 python-icat-1.1.0/tests/test_01_listproxy.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1344 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_03_getversion.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     3085 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_03_login.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      611 2021-04-13 17:57:19.000000 python-icat-1.1.0/tests/test_03_script.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4662 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_04_client_cleanup.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     7283 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_05_dump.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     6939 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_05_dumpfile.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4054 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_05_legacy_ingest.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    17837 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_05_setup.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    17245 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_06_client.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4989 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_06_exception.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    11732 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_06_icatingest.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    15912 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_06_ids.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    12755 2023-06-30 07:04:55.000000 python-icat-1.1.0/tests/test_06_ingest.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    39466 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_06_query.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     1823 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_client_clone.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     2152 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_client_options.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     4941 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_dataselection.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     2696 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_entity_copy.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     5128 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_entity_equal.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)    11394 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_entity_sort.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)     5542 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_07_entity_validate.py
+-rw-r--r--   0 rolf      (1000) rk        (1000)      310 2022-12-21 14:53:25.000000 python-icat-1.1.0/tests/test_09_deprecations.py
+-rwxr-xr-x   0 rolf      (1000) rk        (1000)     6331 2022-12-21 14:53:25.000000 python-icat-1.1.0/wipeicat.py
```

### Comparing `python-icat-1.0.0b1/CHANGES.rst` & `python-icat-1.1.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,84 @@
 Changelog
 =========
 
 
-1.0.0 (not yet released)
-~~~~~~~~~~~~~~~~~~~~~~~~
+1.1.0 (2023-06-30)
+~~~~~~~~~~~~~~~~~~
+
+New features
+------------
+
++ `#113`_, `#123`_: Add module :mod:`icat.ingest`.
+
++ `#124`_: Add an optional keyword argument `keepInstRel` to
+  :meth:`icat.entity.Entity.truncateRelations`.
+
+Bug fixes and minor changes
+---------------------------
+
++ `#126`_, `#127`_: Update outdated documentation.
+
++ `#112`_, `#118`_: Extend icatdata XSD adding extra attributes to
+  reference objects.
+
++ `#111`_, `#121`_: Change the type of
+  :attr:`icat.client.Client.Register` to
+  :class:`weakref.WeakValueDictionary`, fixing a memory leak.
+
++ `#119`_, `#120`_: Remove `_config` attribute from
+  :class:`icat.config.Configuration`.
+
++ `#115`_, `#116`_: Fix the test suite to work if either PyYAML or
+  lxml is not available.
+
++ `#128`_: Return an empty list from
+  :func:`icat.dump_queries.getDataPublicationQueries` when talking to
+  an ICAT server older than 5.0.
+
++ `#117`_: Fixed deprecation warnings from upcoming Python 3.12.
+
++ `#129`_: Review the build of the documentation at Read the Docs.
+
+.. _#111: https://github.com/icatproject/python-icat/issues/111
+.. _#112: https://github.com/icatproject/python-icat/issues/112
+.. _#113: https://github.com/icatproject/python-icat/issues/113
+.. _#115: https://github.com/icatproject/python-icat/issues/115
+.. _#116: https://github.com/icatproject/python-icat/pull/116
+.. _#117: https://github.com/icatproject/python-icat/pull/117
+.. _#118: https://github.com/icatproject/python-icat/pull/118
+.. _#119: https://github.com/icatproject/python-icat/issues/119
+.. _#120: https://github.com/icatproject/python-icat/pull/120
+.. _#121: https://github.com/icatproject/python-icat/pull/121
+.. _#123: https://github.com/icatproject/python-icat/pull/123
+.. _#124: https://github.com/icatproject/python-icat/pull/124
+.. _#126: https://github.com/icatproject/python-icat/issues/126
+.. _#127: https://github.com/icatproject/python-icat/pull/127
+.. _#128: https://github.com/icatproject/python-icat/pull/128
+.. _#129: https://github.com/icatproject/python-icat/pull/129
+
+
+1.0.0 (2022-12-21)
+~~~~~~~~~~~~~~~~~~
 
 New features
 ------------
 
 + `#73`_, `#106`_: Add support for the ICAT schema 5.0 extensions.
 
-+ `#102`_, `#104`_: Make the obj argument to client.new() case
-  insensitive.
++ `#102`_, `#104`_: Make the `obj` argument to
+  :meth:`icat.client.Client.new` case insensitive.
 
 + `#77`_, `#103`_: Add a keyword argument `preset` to allow directly
   passing configuration values to the constructor of class
   :class:`icat.config.Config`.
 
 + `#66`_, `#75`_: Add pathlib support: methods that take a file name
-  argument also accept a :class:`pathlib.Path` object. Internal
-  representation of filesystem paths are changed to use
+  argument also accept a :class:`pathlib.Path` object.  Internal
+  representation of file system paths are changed to use
   :class:`pathlib.Path` where appropriate.  The predefined
   configuarion variable `configFile` now supports tilde expansion.
   Note incompatible changes below.
 
 + `#74`_: :class:`icat.ids.DataSelection` also accepts
   `DataCollection` as argument.
 
@@ -31,15 +86,15 @@
 -------------------------------------
 
 + The order and arrangement of data objects in the dump file created
   by :ref:`icatdump` has been changed.  In some cases, older versions
   of :ref:`icatingest` will fail to read dump files written by new
   versions of :ref:`icatdump`.
 
-+ As a consequence of switching to pathlib for filesystem paths some
++ As a consequence of switching to pathlib for file system paths some
   return values and variables are now :class:`pathlib.Path` objects
   rather then :class:`str`.  This affects:
 
   - the return value of :func:`icat.config.cfgpath`,
   - the predefined configuarion variable `configFile`,
   - the module variable :data:`icat.config.cfgdirs`.
```

### Comparing `python-icat-1.0.0b1/LICENSE.txt` & `python-icat-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/add-investigation-data.py` & `python-icat-1.1.0/doc/examples/add-investigation-data.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/add-job.py` & `python-icat-1.1.0/doc/examples/add-job.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/addfile.py` & `python-icat-1.1.0/doc/examples/addfile.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/create-datafile.py` & `python-icat-1.1.0/doc/examples/create-datafile.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,16 @@
               conditions={ "name": "= '%s'" % conf.dff_name })
 dff = client.assertedSearch(query)[0]
 query = Query(client, "Investigation",
               conditions={ "name": "= '%s'" % conf.investigation })
 investigation = client.assertedSearch(query)[0]
 
 fstats = df_path.stat()
-modTime = datetime.datetime.utcfromtimestamp(fstats.st_mtime).isoformat() + "Z"
+utc = datetime.timezone.utc
+modTime = datetime.datetime.fromtimestamp(fstats.st_mtime, tz=utc)
 datafile = client.new("Datafile")
 datafile.datafileFormat = dff
 datafile.name = conf.datafile.name
 datafile.location = str(conf.datafile)
 datafile.datafileModTime = modTime
 datafile.datafileCreateTime = modTime
 datafile.fileSize = fstats.st_size
```

### Comparing `python-icat-1.0.0b1/doc/examples/create-investigation.py` & `python-icat-1.1.0/doc/examples/create-investigation.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/create-parametertypes.py` & `python-icat-1.1.0/doc/examples/create-parametertypes.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/create-sampletype.py` & `python-icat-1.1.0/doc/examples/create-sampletype.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/downloaddata.py` & `python-icat-1.1.0/doc/examples/downloaddata.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/dumpinvestigation.py` & `python-icat-1.1.0/doc/examples/dumpinvestigation.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/dumprules.py` & `python-icat-1.1.0/doc/examples/dumprules.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/example_data.yaml` & `python-icat-1.1.0/doc/examples/example_data.yaml`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/icat.cfg` & `python-icat-1.1.0/doc/examples/icat.cfg`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.10.xml` & `python-icat-1.1.0/doc/examples/icatdump-4.10.xml`

 * *Files 0% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.10.xml` & `python-icat-1.1.0/doc/examples/icatdump-4.10.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <icatdata>
   <head>
-    <date>2022-11-23T16:13:28+00:00</date>
+    <date>2022-12-21T15:08:20+00:00</date>
     <service>https://icat.example.com:8181/ICATService/ICAT?wsdl</service>
     <apiversion>4.10.0</apiversion>
-    <generator>icatdump (python-icat 0.21.1.dev138)</generator>
+    <generator>icatdump (python-icat 1.0.0)</generator>
   </head>
   <data>
     <user id="User_name-db=2Facord">
       <affiliation>University of Ravenna, Institute of Modern History</affiliation>
       <email>acord@example.org</email>
       <familyName>Cordus</familyName>
       <fullName>Aelius Cordus</fullName>
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.10.yaml` & `python-icat-1.1.0/doc/examples/icatdump-4.10.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %YAML 1.1
-# Date: Wed, 23 Nov 2022 16:13:26 +0000
+# Date: Wed, 21 Dec 2022 15:08:23 +0000
 # Service: https://icat.example.com:8181/ICATService/ICAT?wsdl
 # ICAT-API: 4.10.0
-# Generator: icatdump (python-icat 0.21.1.dev138)
+# Generator: icatdump (python-icat 1.0.0)
 ---
 grouping:
   Grouping_name-ingest:
     name: ingest
     userGroups:
     - user: User_name-simple=2Fdataingest
   Grouping_name-investigation=5F08100122=2DEF=5Fowner:
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.4.xml` & `python-icat-1.1.0/doc/examples/icatdump-4.4.xml`

 * *Files 0% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.4.xml` & `python-icat-1.1.0/doc/examples/icatdump-4.4.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <icatdata>
   <head>
-    <date>2022-11-23T16:39:42+00:00</date>
+    <date>2022-12-21T14:56:55+00:00</date>
     <service>https://icat.example.com:8181/ICATService/ICAT?wsdl</service>
     <apiversion>4.4.0</apiversion>
-    <generator>icatdump (python-icat 0.21.1.dev138)</generator>
+    <generator>icatdump (python-icat 1.0.0)</generator>
   </head>
   <data>
     <user id="User_name-db=2Facord">
       <fullName>Aelius Cordus</fullName>
       <name>db/acord</name>
     </user>
     <user id="User_name-db=2Fahau">
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.4.yaml` & `python-icat-1.1.0/doc/examples/icatdump-4.4.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %YAML 1.1
-# Date: Wed, 23 Nov 2022 16:39:39 +0000
+# Date: Wed, 21 Dec 2022 14:57:08 +0000
 # Service: https://icat.example.com:8181/ICATService/ICAT?wsdl
 # ICAT-API: 4.4.0
-# Generator: icatdump (python-icat 0.21.1.dev138)
+# Generator: icatdump (python-icat 1.0.0)
 ---
 grouping:
   Grouping_name-ingest:
     name: ingest
     userGroups:
     - user: User_name-simple=2Fdataingest
   Grouping_name-investigation=5F08100122=2DEF=5Fowner:
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.7.xml` & `python-icat-1.1.0/doc/examples/icatdump-4.7.xml`

 * *Files 0% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.7.xml` & `python-icat-1.1.0/doc/examples/icatdump-4.7.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <icatdata>
   <head>
-    <date>2022-11-23T16:26:45+00:00</date>
+    <date>2022-12-21T15:02:37+00:00</date>
     <service>https://icat.example.com:8181/ICATService/ICAT?wsdl</service>
     <apiversion>4.7.0</apiversion>
-    <generator>icatdump (python-icat 0.21.1.dev138)</generator>
+    <generator>icatdump (python-icat 1.0.0)</generator>
   </head>
   <data>
     <user id="User_name-db=2Facord">
       <email>acord@example.org</email>
       <fullName>Aelius Cordus</fullName>
       <name>db/acord</name>
       <orcidId>0000-0002-3262</orcidId>
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-4.7.yaml` & `python-icat-1.1.0/doc/examples/icatdump-4.7.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %YAML 1.1
-# Date: Wed, 23 Nov 2022 16:26:41 +0000
+# Date: Wed, 21 Dec 2022 15:02:40 +0000
 # Service: https://icat.example.com:8181/ICATService/ICAT?wsdl
 # ICAT-API: 4.7.0
-# Generator: icatdump (python-icat 0.21.1.dev138)
+# Generator: icatdump (python-icat 1.0.0)
 ---
 grouping:
   Grouping_name-ingest:
     name: ingest
     userGroups:
     - user: User_name-simple=2Fdataingest
   Grouping_name-investigation=5F08100122=2DEF=5Fowner:
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-5.0.xml` & `python-icat-1.1.0/doc/examples/icatdump-5.0.xml`

 * *Files 0% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-5.0.xml` & `python-icat-1.1.0/doc/examples/icatdump-5.0.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <icatdata>
   <head>
-    <date>2022-11-23T15:30:14+00:00</date>
+    <date>2022-12-21T15:14:23+00:00</date>
     <service>https://icat.example.com:8181/ICATService/ICAT?wsdl</service>
     <apiversion>5.0.0</apiversion>
-    <generator>icatdump (python-icat 0.21.1.dev138)</generator>
+    <generator>icatdump (python-icat 1.0.0)</generator>
   </head>
   <data>
     <user id="User_name-db=2Facord">
       <affiliation>University of Ravenna, Institute of Modern History</affiliation>
       <email>acord@example.org</email>
       <familyName>Cordus</familyName>
       <fullName>Aelius Cordus</fullName>
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatdump-5.0.yaml` & `python-icat-1.1.0/doc/examples/icatdump-5.0.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %YAML 1.1
-# Date: Wed, 23 Nov 2022 15:30:08 +0000
+# Date: Wed, 21 Dec 2022 15:14:26 +0000
 # Service: https://icat.example.com:8181/ICATService/ICAT?wsdl
 # ICAT-API: 5.0.0
-# Generator: icatdump (python-icat 0.21.1.dev138)
+# Generator: icatdump (python-icat 1.0.0)
 ---
 grouping:
   Grouping_name-ingest:
     name: ingest
     userGroups:
     - user: User_name-simple=2Fdataingest
   Grouping_name-investigation=5F08100122=2DEF=5Fowner:
```

### Comparing `python-icat-1.0.0b1/doc/examples/icatexport.py` & `python-icat-1.1.0/doc/examples/icatexport.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/icatimport.py` & `python-icat-1.1.0/doc/examples/icatimport.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/icatsummary.py` & `python-icat-1.1.0/doc/examples/icatsummary.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/ingest-datafiles.xml` & `python-icat-1.1.0/doc/examples/ingest-datafiles.xml`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/ingest-ds-params.xml` & `python-icat-1.1.0/doc/examples/ingest-ds-params.xml`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/init-icat.py` & `python-icat-1.1.0/doc/examples/init-icat.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/paramtype.py` & `python-icat-1.1.0/doc/examples/paramtype.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/examples/querytest.py` & `python-icat-1.1.0/doc/examples/querytest.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/icatdata-4.10.xsd` & `python-icat-1.1.0/doc/icatdata-4.3.xsd`

 * *Files 1% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/icatdata-4.10.xsd` & `python-icat-1.1.0/doc/icatdata-4.3.xsd`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema">
   <xsd:annotation>
     <xsd:documentation>Schema definition for an ICAT data file format.
-    Valid for ICAT 4.10.*.</xsd:documentation>
+    Valid for ICAT 4.3.*.</xsd:documentation>
   </xsd:annotation>
   <xsd:element name="icatdata" type="icatdata"/>
   <xsd:complexType name="icatdata">
     <xsd:sequence>
       <xsd:element name="head" type="head" minOccurs="0"/>
       <xsd:element name="data" type="data" minOccurs="0" maxOccurs="unbounded"/>
     </xsd:sequence>
@@ -18,15 +18,17 @@
       <xsd:element name="apiversion" type="xsd:string" minOccurs="0"/>
       <xsd:element name="generator" type="xsd:string"/>
     </xsd:sequence>
   </xsd:complexType>
   <xsd:complexType name="data">
     <!-- The data element contains the entity objects.  
 
-       Order is important.  Objects referenced by others in a
+       Order is important.  Objects that setup access rules MUST come
+       first in file order, at least as far as write permission for
+       the root user is concerned.  Objects referenced by others in a
        many-to-one relation MUST come before the referencing object.
   -->
     <xsd:sequence>
       <!-- entity object references -->
       <xsd:element name="applicationRef" type="applicationRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileRef" type="datafileRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileFormatRef" type="datafileFormatRef" minOccurs="0" maxOccurs="unbounded"/>
@@ -62,15 +64,14 @@
       <xsd:element name="application" type="application" minOccurs="0" maxOccurs="unbounded"/>
       <!-- investigation -->
       <xsd:element name="investigation" type="investigation" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationParameter" type="investigationParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="keyword" type="keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="publication" type="publication" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="shift" type="shift" minOccurs="0" maxOccurs="unbounded"/>
-      <xsd:element name="investigationGroup" type="investigationGroup" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationInstrument" type="investigationInstrument" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationUser" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sample" type="sample" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sampleParameter" type="sampleParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="dataset" type="dataset" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetParameter" type="datasetParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafile" type="datafile" minOccurs="0" maxOccurs="unbounded"/>
@@ -141,14 +142,15 @@
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="dataset.investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="dataset.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafileFormatRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -160,14 +162,15 @@
   <xsd:complexType name="datasetRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datasetTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -199,14 +202,15 @@
   </xsd:complexType>
   <xsd:complexType name="investigationRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="visitId" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -284,15 +288,14 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollection">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="doi" type="xsd:string" minOccurs="0"/>
           <xsd:element name="dataCollectionDatafiles" type="dataCollectionDatafile" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="dataCollectionDatasets" type="dataCollectionDataset" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="jobsAsInput" type="job" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="jobsAsOutput" type="job" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="parameters" type="dataCollectionParameter" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
@@ -471,35 +474,32 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="grouping">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="name" type="xsd:string"/>
-          <xsd:element name="investigationGroups" type="investigationGroup" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="rules" type="rule" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="userGroups" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="instrument">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
           <xsd:element name="fullName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
-          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="type" type="xsd:string" minOccurs="0"/>
           <xsd:element name="url" type="xsd:string" minOccurs="0"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="instrumentScientists" type="instrumentScientist" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationInstruments" type="investigationInstrument" minOccurs="0" maxOccurs="unbounded"/>
-          <xsd:element name="shifts" type="shift" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="instrumentScientist">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
@@ -521,38 +521,26 @@
           <xsd:element name="startDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="summary" type="xsd:string" minOccurs="0"/>
           <xsd:element name="title" type="xsd:string"/>
           <xsd:element name="visitId" type="xsd:string"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="type" type="investigationTypeRef" minOccurs="0"/>
           <xsd:element name="datasets" type="dataset" minOccurs="0" maxOccurs="unbounded"/>
-          <xsd:element name="investigationGroups" type="investigationGroup" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationInstruments" type="investigationInstrument" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationUsers" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="keywords" type="keyword" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="parameters" type="investigationParameter" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="publications" type="publication" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="samples" type="sample" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="shifts" type="shift" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="studyInvestigations" type="studyInvestigation" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
-  <xsd:complexType name="investigationGroup">
-    <xsd:complexContent>
-      <xsd:extension base="entityBase">
-        <xsd:sequence>
-          <xsd:element name="role" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="grouping" type="groupingRef" minOccurs="0"/>
-          <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
   <xsd:complexType name="investigationInstrument">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="instrument" type="instrumentRef" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
         </xsd:sequence>
@@ -630,15 +618,14 @@
           <xsd:element name="applicableToInvestigation" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="applicableToSample" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
           <xsd:element name="enforced" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="maximumNumericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="minimumNumericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
-          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="units" type="xsd:string"/>
           <xsd:element name="unitsFullName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="valueType" type="parameterValueType"/>
           <xsd:element name="verified" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="dataCollectionParameters" type="dataCollectionParameter" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="datafileParameters" type="datafileParameter" minOccurs="0" maxOccurs="unbounded"/>
@@ -707,15 +694,14 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="sample">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="name" type="xsd:string"/>
-          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
           <xsd:element name="type" type="sampleTypeRef" minOccurs="0"/>
           <xsd:element name="datasets" type="dataset" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="parameters" type="sampleParameter" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
@@ -752,28 +738,25 @@
   <xsd:complexType name="shift">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="comment" type="xsd:string" minOccurs="0"/>
           <xsd:element name="endDate" type="xsd:dateTime"/>
           <xsd:element name="startDate" type="xsd:dateTime"/>
-          <xsd:element name="instrument" type="instrumentRef" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="study">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="endDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
-          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="startDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="status" type="studyStatus" minOccurs="0"/>
           <xsd:element name="user" type="userRef" minOccurs="0"/>
           <xsd:element name="studyInvestigations" type="studyInvestigation" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
@@ -788,21 +771,16 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="user">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="affiliation" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="email" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="familyName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="fullName" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="givenName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
-          <xsd:element name="orcidId" type="xsd:string" minOccurs="0"/>
           <xsd:element name="instrumentScientists" type="instrumentScientist" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationUsers" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="studies" type="study" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="userGroups" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
```

### Comparing `python-icat-1.0.0b1/doc/icatdata-4.3.xsd` & `python-icat-1.1.0/doc/icatdata-4.4.xsd`

 * *Files 1% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/icatdata-4.3.xsd` & `python-icat-1.1.0/doc/icatdata-4.4.xsd`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema">
   <xsd:annotation>
     <xsd:documentation>Schema definition for an ICAT data file format.
-    Valid for ICAT 4.3.*.</xsd:documentation>
+    Valid for ICAT 4.4.*.</xsd:documentation>
   </xsd:annotation>
   <xsd:element name="icatdata" type="icatdata"/>
   <xsd:complexType name="icatdata">
     <xsd:sequence>
       <xsd:element name="head" type="head" minOccurs="0"/>
       <xsd:element name="data" type="data" minOccurs="0" maxOccurs="unbounded"/>
     </xsd:sequence>
@@ -18,17 +18,15 @@
       <xsd:element name="apiversion" type="xsd:string" minOccurs="0"/>
       <xsd:element name="generator" type="xsd:string"/>
     </xsd:sequence>
   </xsd:complexType>
   <xsd:complexType name="data">
     <!-- The data element contains the entity objects.  
 
-       Order is important.  Objects that setup access rules MUST come
-       first in file order, at least as far as write permission for
-       the root user is concerned.  Objects referenced by others in a
+       Order is important.  Objects referenced by others in a
        many-to-one relation MUST come before the referencing object.
   -->
     <xsd:sequence>
       <!-- entity object references -->
       <xsd:element name="applicationRef" type="applicationRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileRef" type="datafileRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileFormatRef" type="datafileFormatRef" minOccurs="0" maxOccurs="unbounded"/>
@@ -64,14 +62,15 @@
       <xsd:element name="application" type="application" minOccurs="0" maxOccurs="unbounded"/>
       <!-- investigation -->
       <xsd:element name="investigation" type="investigation" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationParameter" type="investigationParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="keyword" type="keyword" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="publication" type="publication" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="shift" type="shift" minOccurs="0" maxOccurs="unbounded"/>
+      <xsd:element name="investigationGroup" type="investigationGroup" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationInstrument" type="investigationInstrument" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationUser" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sample" type="sample" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sampleParameter" type="sampleParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="dataset" type="dataset" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetParameter" type="datasetParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafile" type="datafile" minOccurs="0" maxOccurs="unbounded"/>
@@ -142,14 +141,15 @@
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="dataset.investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="dataset.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafileFormatRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -161,14 +161,15 @@
   <xsd:complexType name="datasetRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datasetTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -200,14 +201,15 @@
   </xsd:complexType>
   <xsd:complexType name="investigationRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="visitId" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -471,14 +473,15 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="grouping">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="name" type="xsd:string"/>
+          <xsd:element name="investigationGroups" type="investigationGroup" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="rules" type="rule" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="userGroups" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="instrument">
@@ -518,26 +521,38 @@
           <xsd:element name="startDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="summary" type="xsd:string" minOccurs="0"/>
           <xsd:element name="title" type="xsd:string"/>
           <xsd:element name="visitId" type="xsd:string"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="type" type="investigationTypeRef" minOccurs="0"/>
           <xsd:element name="datasets" type="dataset" minOccurs="0" maxOccurs="unbounded"/>
+          <xsd:element name="investigationGroups" type="investigationGroup" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationInstruments" type="investigationInstrument" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationUsers" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="keywords" type="keyword" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="parameters" type="investigationParameter" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="publications" type="publication" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="samples" type="sample" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="shifts" type="shift" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="studyInvestigations" type="studyInvestigation" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
+  <xsd:complexType name="investigationGroup">
+    <xsd:complexContent>
+      <xsd:extension base="entityBase">
+        <xsd:sequence>
+          <xsd:element name="role" type="xsd:string" minOccurs="0"/>
+          <xsd:element name="grouping" type="groupingRef" minOccurs="0"/>
+          <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
+        </xsd:sequence>
+      </xsd:extension>
+    </xsd:complexContent>
+  </xsd:complexType>
   <xsd:complexType name="investigationInstrument">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="instrument" type="instrumentRef" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
         </xsd:sequence>
```

### Comparing `python-icat-1.0.0b1/doc/icatdata-4.4.xsd` & `python-icat-1.1.0/doc/icatdata-4.7.xsd`

 * *Files 1% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/icatdata-4.4.xsd` & `python-icat-1.1.0/doc/icatdata-4.7.xsd`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema">
   <xsd:annotation>
     <xsd:documentation>Schema definition for an ICAT data file format.
-    Valid for ICAT 4.4.*.</xsd:documentation>
+    Valid for ICAT 4.7.*.</xsd:documentation>
   </xsd:annotation>
   <xsd:element name="icatdata" type="icatdata"/>
   <xsd:complexType name="icatdata">
     <xsd:sequence>
       <xsd:element name="head" type="head" minOccurs="0"/>
       <xsd:element name="data" type="data" minOccurs="0" maxOccurs="unbounded"/>
     </xsd:sequence>
@@ -24,14 +24,15 @@
 
        Order is important.  Objects referenced by others in a
        many-to-one relation MUST come before the referencing object.
   -->
     <xsd:sequence>
       <!-- entity object references -->
       <xsd:element name="applicationRef" type="applicationRef" minOccurs="0" maxOccurs="unbounded"/>
+      <xsd:element name="dataCollectionRef" type="dataCollectionRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileRef" type="datafileRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileFormatRef" type="datafileFormatRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetRef" type="datasetRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetTypeRef" type="datasetTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="facilityRef" type="facilityRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="groupingRef" type="groupingRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="instrumentRef" type="instrumentRef" minOccurs="0" maxOccurs="unbounded"/>
@@ -133,22 +134,30 @@
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="version" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
+  <xsd:complexType name="dataCollectionRef">
+    <xsd:complexContent>
+      <xsd:extension base="entityReference">
+        <xsd:attribute name="doi" type="xsd:string"/>
+      </xsd:extension>
+    </xsd:complexContent>
+  </xsd:complexType>
   <xsd:complexType name="datafileRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="dataset.investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="dataset.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafileFormatRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -160,14 +169,15 @@
   <xsd:complexType name="datasetRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datasetTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -199,14 +209,15 @@
   </xsd:complexType>
   <xsd:complexType name="investigationRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="visitId" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -242,14 +253,16 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="userRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="email" type="xsd:string"/>
+        <xsd:attribute name="orcidId" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <!-- Entity object definition types
 
      Note that this schema is somewhat too liberal.  Additional
      constraints that depend on context (and thus are not easy to
@@ -284,38 +297,39 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollection">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
+          <xsd:element name="doi" type="xsd:string" minOccurs="0"/>
           <xsd:element name="dataCollectionDatafiles" type="dataCollectionDatafile" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="dataCollectionDatasets" type="dataCollectionDataset" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="jobsAsInput" type="job" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="jobsAsOutput" type="job" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="parameters" type="dataCollectionParameter" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionDatafile">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="datafile" type="datafileRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionDataset">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="dataset" type="datasetRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionParameter">
     <xsd:complexContent>
@@ -323,15 +337,15 @@
         <xsd:sequence>
           <xsd:element name="dateTimeValue" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="error" type="xsd:double" minOccurs="0"/>
           <xsd:element name="numericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="rangeBottom" type="xsd:double" minOccurs="0"/>
           <xsd:element name="rangeTop" type="xsd:double" minOccurs="0"/>
           <xsd:element name="stringValue" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="type" type="parameterTypeRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafile">
     <xsd:complexContent>
@@ -597,16 +611,16 @@
   </xsd:complexType>
   <xsd:complexType name="job">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="arguments" type="xsd:string" minOccurs="0"/>
           <xsd:element name="application" type="applicationRef" minOccurs="0"/>
-          <xsd:element name="inputDataCollection" type="entityReference" minOccurs="0"/>
-          <xsd:element name="outputDataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="inputDataCollection" type="dataCollectionRef" minOccurs="0"/>
+          <xsd:element name="outputDataCollection" type="dataCollectionRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="keyword">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
@@ -780,16 +794,18 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="user">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
+          <xsd:element name="email" type="xsd:string" minOccurs="0"/>
           <xsd:element name="fullName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
+          <xsd:element name="orcidId" type="xsd:string" minOccurs="0"/>
           <xsd:element name="instrumentScientists" type="instrumentScientist" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationUsers" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="studies" type="study" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="userGroups" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
```

### Comparing `python-icat-1.0.0b1/doc/icatdata-4.7.xsd` & `python-icat-1.1.0/doc/icatdata-4.10.xsd`

 * *Files 2% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/icatdata-4.7.xsd` & `python-icat-1.1.0/doc/icatdata-4.10.xsd`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema">
   <xsd:annotation>
     <xsd:documentation>Schema definition for an ICAT data file format.
-    Valid for ICAT 4.7.*.</xsd:documentation>
+    Valid for ICAT 4.10.*.</xsd:documentation>
   </xsd:annotation>
   <xsd:element name="icatdata" type="icatdata"/>
   <xsd:complexType name="icatdata">
     <xsd:sequence>
       <xsd:element name="head" type="head" minOccurs="0"/>
       <xsd:element name="data" type="data" minOccurs="0" maxOccurs="unbounded"/>
     </xsd:sequence>
@@ -24,26 +24,28 @@
 
        Order is important.  Objects referenced by others in a
        many-to-one relation MUST come before the referencing object.
   -->
     <xsd:sequence>
       <!-- entity object references -->
       <xsd:element name="applicationRef" type="applicationRef" minOccurs="0" maxOccurs="unbounded"/>
+      <xsd:element name="dataCollectionRef" type="dataCollectionRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileRef" type="datafileRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileFormatRef" type="datafileFormatRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetRef" type="datasetRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetTypeRef" type="datasetTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="facilityRef" type="facilityRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="groupingRef" type="groupingRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="instrumentRef" type="instrumentRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationRef" type="investigationRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationTypeRef" type="investigationTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="parameterTypeRef" type="parameterTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sampleRef" type="sampleRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sampleTypeRef" type="sampleTypeRef" minOccurs="0" maxOccurs="unbounded"/>
+      <xsd:element name="studyRef" type="studyRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="userRef" type="userRef" minOccurs="0" maxOccurs="unbounded"/>
       <!-- entity object definitions -->
       <!-- authz -->
       <xsd:element name="user" type="user" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="grouping" type="grouping" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="userGroup" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="rule" type="rule" minOccurs="0" maxOccurs="unbounded"/>
@@ -133,22 +135,30 @@
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="version" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
+  <xsd:complexType name="dataCollectionRef">
+    <xsd:complexContent>
+      <xsd:extension base="entityReference">
+        <xsd:attribute name="doi" type="xsd:string"/>
+      </xsd:extension>
+    </xsd:complexContent>
+  </xsd:complexType>
   <xsd:complexType name="datafileRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="dataset.investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="dataset.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafileFormatRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -160,14 +170,15 @@
   <xsd:complexType name="datasetRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datasetTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -190,23 +201,25 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="instrumentRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="visitId" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -216,40 +229,51 @@
   </xsd:complexType>
   <xsd:complexType name="parameterTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="units" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="sampleRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="sampleTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="molecularFormula" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
+  <xsd:complexType name="studyRef">
+    <xsd:complexContent>
+      <xsd:extension base="entityReference">
+        <xsd:attribute name="pid" type="xsd:string"/>
+      </xsd:extension>
+    </xsd:complexContent>
+  </xsd:complexType>
   <xsd:complexType name="userRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="email" type="xsd:string"/>
+        <xsd:attribute name="orcidId" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <!-- Entity object definition types
 
      Note that this schema is somewhat too liberal.  Additional
      constraints that depend on context (and thus are not easy to
@@ -298,25 +322,25 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionDatafile">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="datafile" type="datafileRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionDataset">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="dataset" type="datasetRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionParameter">
     <xsd:complexContent>
@@ -324,15 +348,15 @@
         <xsd:sequence>
           <xsd:element name="dateTimeValue" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="error" type="xsd:double" minOccurs="0"/>
           <xsd:element name="numericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="rangeBottom" type="xsd:double" minOccurs="0"/>
           <xsd:element name="rangeTop" type="xsd:double" minOccurs="0"/>
           <xsd:element name="stringValue" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="type" type="parameterTypeRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafile">
     <xsd:complexContent>
@@ -485,19 +509,21 @@
   <xsd:complexType name="instrument">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
           <xsd:element name="fullName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
+          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="type" type="xsd:string" minOccurs="0"/>
           <xsd:element name="url" type="xsd:string" minOccurs="0"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="instrumentScientists" type="instrumentScientist" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationInstruments" type="investigationInstrument" minOccurs="0" maxOccurs="unbounded"/>
+          <xsd:element name="shifts" type="shift" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="instrumentScientist">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
@@ -598,16 +624,16 @@
   </xsd:complexType>
   <xsd:complexType name="job">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="arguments" type="xsd:string" minOccurs="0"/>
           <xsd:element name="application" type="applicationRef" minOccurs="0"/>
-          <xsd:element name="inputDataCollection" type="entityReference" minOccurs="0"/>
-          <xsd:element name="outputDataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="inputDataCollection" type="dataCollectionRef" minOccurs="0"/>
+          <xsd:element name="outputDataCollection" type="dataCollectionRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="keyword">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
@@ -628,14 +654,15 @@
           <xsd:element name="applicableToInvestigation" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="applicableToSample" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
           <xsd:element name="enforced" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="maximumNumericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="minimumNumericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
+          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="units" type="xsd:string"/>
           <xsd:element name="unitsFullName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="valueType" type="parameterValueType"/>
           <xsd:element name="verified" type="xsd:boolean" minOccurs="0"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="dataCollectionParameters" type="dataCollectionParameter" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="datafileParameters" type="datafileParameter" minOccurs="0" maxOccurs="unbounded"/>
@@ -704,14 +731,15 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="sample">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="name" type="xsd:string"/>
+          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
           <xsd:element name="type" type="sampleTypeRef" minOccurs="0"/>
           <xsd:element name="datasets" type="dataset" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="parameters" type="sampleParameter" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
@@ -748,49 +776,55 @@
   <xsd:complexType name="shift">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="comment" type="xsd:string" minOccurs="0"/>
           <xsd:element name="endDate" type="xsd:dateTime"/>
           <xsd:element name="startDate" type="xsd:dateTime"/>
+          <xsd:element name="instrument" type="instrumentRef" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="study">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
+          <xsd:element name="endDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
+          <xsd:element name="pid" type="xsd:string" minOccurs="0"/>
           <xsd:element name="startDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="status" type="studyStatus" minOccurs="0"/>
           <xsd:element name="user" type="userRef" minOccurs="0"/>
           <xsd:element name="studyInvestigations" type="studyInvestigation" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="studyInvestigation">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
-          <xsd:element name="study" type="entityReference" minOccurs="0"/>
+          <xsd:element name="study" type="studyRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="user">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
+          <xsd:element name="affiliation" type="xsd:string" minOccurs="0"/>
           <xsd:element name="email" type="xsd:string" minOccurs="0"/>
+          <xsd:element name="familyName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="fullName" type="xsd:string" minOccurs="0"/>
+          <xsd:element name="givenName" type="xsd:string" minOccurs="0"/>
           <xsd:element name="name" type="xsd:string"/>
           <xsd:element name="orcidId" type="xsd:string" minOccurs="0"/>
           <xsd:element name="instrumentScientists" type="instrumentScientist" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="investigationUsers" type="investigationUser" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="studies" type="study" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="userGroups" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
```

### Comparing `python-icat-1.0.0b1/doc/icatdata-5.0.xsd` & `python-icat-1.1.0/doc/icatdata-5.0.xsd`

 * *Files 1% similar despite different names*

#### Comparing `python-icat-1.0.0b1/doc/icatdata-5.0.xsd` & `python-icat-1.1.0/doc/icatdata-5.0.xsd`

```diff
@@ -24,14 +24,15 @@
 
        Order is important.  Objects referenced by others in a
        many-to-one relation MUST come before the referencing object.
   -->
     <xsd:sequence>
       <!-- entity object references -->
       <xsd:element name="applicationRef" type="applicationRef" minOccurs="0" maxOccurs="unbounded"/>
+      <xsd:element name="dataCollectionRef" type="dataCollectionRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="dataPublicationRef" type="dataPublicationRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="dataPublicationTypeRef" type="dataPublicationTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="dataPublicationUserRef" type="dataPublicationUserRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileRef" type="datafileRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datafileFormatRef" type="datafileFormatRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetRef" type="datasetRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="datasetTypeRef" type="datasetTypeRef" minOccurs="0" maxOccurs="unbounded"/>
@@ -41,14 +42,15 @@
       <xsd:element name="groupingRef" type="groupingRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="instrumentRef" type="instrumentRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationRef" type="investigationRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="investigationTypeRef" type="investigationTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="parameterTypeRef" type="parameterTypeRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sampleRef" type="sampleRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="sampleTypeRef" type="sampleTypeRef" minOccurs="0" maxOccurs="unbounded"/>
+      <xsd:element name="studyRef" type="studyRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="techniqueRef" type="techniqueRef" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="userRef" type="userRef" minOccurs="0" maxOccurs="unbounded"/>
       <!-- entity object definitions -->
       <!-- authz -->
       <xsd:element name="user" type="user" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="grouping" type="grouping" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="userGroup" type="userGroup" minOccurs="0" maxOccurs="unbounded"/>
@@ -155,14 +157,21 @@
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="version" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
+  <xsd:complexType name="dataCollectionRef">
+    <xsd:complexContent>
+      <xsd:extension base="entityReference">
+        <xsd:attribute name="doi" type="xsd:string"/>
+      </xsd:extension>
+    </xsd:complexContent>
+  </xsd:complexType>
   <xsd:complexType name="dataPublicationRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
@@ -189,14 +198,15 @@
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="dataset.investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.name" type="xsd:string"/>
         <xsd:attribute name="dataset.investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="dataset.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datafileFormatRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -208,14 +218,15 @@
   <xsd:complexType name="datasetRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="datasetTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -239,14 +250,15 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="fundingReferenceRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="funderName" type="xsd:string"/>
         <xsd:attribute name="awardNumber" type="xsd:string"/>
+        <xsd:attribute name="funderIdentifier" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="groupingRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="name" type="xsd:string"/>
@@ -254,23 +266,25 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="instrumentRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="visitId" type="xsd:string"/>
+        <xsd:attribute name="doi" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="investigationTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
@@ -280,47 +294,59 @@
   </xsd:complexType>
   <xsd:complexType name="parameterTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="units" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="sampleRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="investigation.facility.name" type="xsd:string"/>
         <xsd:attribute name="investigation.name" type="xsd:string"/>
         <xsd:attribute name="investigation.visitId" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="sampleTypeRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="facility.name" type="xsd:string"/>
         <xsd:attribute name="name" type="xsd:string"/>
         <xsd:attribute name="molecularFormula" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
+  <xsd:complexType name="studyRef">
+    <xsd:complexContent>
+      <xsd:extension base="entityReference">
+        <xsd:attribute name="pid" type="xsd:string"/>
+      </xsd:extension>
+    </xsd:complexContent>
+  </xsd:complexType>
   <xsd:complexType name="techniqueRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="pid" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="userRef">
     <xsd:complexContent>
       <xsd:extension base="entityReference">
         <xsd:attribute name="name" type="xsd:string"/>
+        <xsd:attribute name="email" type="xsd:string"/>
+        <xsd:attribute name="orcidId" type="xsd:string"/>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <!-- Entity object definition types
 
      Note that this schema is somewhat too liberal.  Additional
      constraints that depend on context (and thus are not easy to
@@ -382,35 +408,35 @@
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionDatafile">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="datafile" type="datafileRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionDataset">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="dataset" type="datasetRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionInvestigation">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataCollectionParameter">
     <xsd:complexContent>
@@ -418,30 +444,30 @@
         <xsd:sequence>
           <xsd:element name="dateTimeValue" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="error" type="xsd:double" minOccurs="0"/>
           <xsd:element name="numericValue" type="xsd:double" minOccurs="0"/>
           <xsd:element name="rangeBottom" type="xsd:double" minOccurs="0"/>
           <xsd:element name="rangeTop" type="xsd:double" minOccurs="0"/>
           <xsd:element name="stringValue" type="xsd:string" minOccurs="0"/>
-          <xsd:element name="dataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="dataCollection" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="type" type="parameterTypeRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="dataPublication">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="description" type="xsd:string" minOccurs="0"/>
           <xsd:element name="pid" type="xsd:string"/>
           <xsd:element name="publicationDate" type="xsd:dateTime" minOccurs="0"/>
           <xsd:element name="subject" type="xsd:string" minOccurs="0"/>
           <xsd:element name="title" type="xsd:string"/>
-          <xsd:element name="content" type="entityReference" minOccurs="0"/>
+          <xsd:element name="content" type="dataCollectionRef" minOccurs="0"/>
           <xsd:element name="facility" type="facilityRef" minOccurs="0"/>
           <xsd:element name="type" type="dataPublicationTypeRef" minOccurs="0"/>
           <xsd:element name="dates" type="dataPublicationDate" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="fundingReferences" type="dataPublicationFunding" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="relatedItems" type="relatedItem" minOccurs="0" maxOccurs="unbounded"/>
           <xsd:element name="users" type="dataPublicationUser" minOccurs="0" maxOccurs="unbounded"/>
         </xsd:sequence>
@@ -831,16 +857,16 @@
   </xsd:complexType>
   <xsd:complexType name="job">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="arguments" type="xsd:string" minOccurs="0"/>
           <xsd:element name="application" type="applicationRef" minOccurs="0"/>
-          <xsd:element name="inputDataCollection" type="entityReference" minOccurs="0"/>
-          <xsd:element name="outputDataCollection" type="entityReference" minOccurs="0"/>
+          <xsd:element name="inputDataCollection" type="dataCollectionRef" minOccurs="0"/>
+          <xsd:element name="outputDataCollection" type="dataCollectionRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="keyword">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
@@ -1024,15 +1050,15 @@
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="studyInvestigation">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
         <xsd:sequence>
           <xsd:element name="investigation" type="investigationRef" minOccurs="0"/>
-          <xsd:element name="study" type="entityReference" minOccurs="0"/>
+          <xsd:element name="study" type="studyRef" minOccurs="0"/>
         </xsd:sequence>
       </xsd:extension>
     </xsd:complexContent>
   </xsd:complexType>
   <xsd:complexType name="technique">
     <xsd:complexContent>
       <xsd:extension base="entityBase">
```

### Comparing `python-icat-1.0.0b1/doc/man/icatdump.1` & `python-icat-1.1.0/doc/man/icatdump.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "ICATDUMP" "1" "Nov 23, 2022" "1.0" "python-icat"
+.TH "ICATDUMP" "1" "Jun 30, 2023" "1.1" "python-icat"
 .SH NAME
 icatdump \- Dump the content of the ICAT to a file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -213,10 +213,10 @@
 .UNINDENT
 .SH SEE ALSO
 .sp
 \fBicatingest(1)\fP
 .SH AUTHOR
 Rolf Krahl
 .SH COPYRIGHT
-2013–2022, Helmholtz-Zentrum Berlin für Materialien und Energie GmbH
+2013–2023, Helmholtz-Zentrum Berlin für Materialien und Energie GmbH
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `python-icat-1.0.0b1/doc/man/icatingest.1` & `python-icat-1.1.0/doc/man/icatingest.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "ICATINGEST" "1" "Nov 23, 2022" "1.0" "python-icat"
+.TH "ICATINGEST" "1" "Jun 30, 2023" "1.1" "python-icat"
 .SH NAME
 icatingest \- Restore the content of the ICAT from a dump file
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -249,10 +249,10 @@
 .UNINDENT
 .SH SEE ALSO
 .sp
 \fBicatdump(1)\fP
 .SH AUTHOR
 Rolf Krahl
 .SH COPYRIGHT
-2013–2022, Helmholtz-Zentrum Berlin für Materialien und Energie GmbH
+2013–2023, Helmholtz-Zentrum Berlin für Materialien und Energie GmbH
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `python-icat-1.0.0b1/doc/man/wipeicat.1` & `python-icat-1.1.0/doc/man/wipeicat.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "WIPEICAT" "1" "Nov 23, 2022" "1.0" "python-icat"
+.TH "WIPEICAT" "1" "Jun 30, 2023" "1.1" "python-icat"
 .SH NAME
 wipeicat \- Delete all content from an ICAT
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -177,10 +177,10 @@
 .TP
 .B ICAT_USER
 ICAT user name, see \fI\%\-\-user\fP\&.
 .UNINDENT
 .SH AUTHOR
 Rolf Krahl
 .SH COPYRIGHT
-2013–2022, Helmholtz-Zentrum Berlin für Materialien und Energie GmbH
+2013–2023, Helmholtz-Zentrum Berlin für Materialien und Energie GmbH
 .\" Generated by docutils manpage writer.
 .
```

### Comparing `python-icat-1.0.0b1/doc/tutorial/config-custom.py` & `python-icat-1.1.0/doc/tutorial/config-custom.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/tutorial/config-flag.py` & `python-icat-1.1.0/doc/tutorial/config-flag.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/doc/tutorial/config-sub-commands.py` & `python-icat-1.1.0/doc/tutorial/config-sub-commands.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/authinfo.py` & `python-icat-1.1.0/icat/authinfo.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/chunkedhttp.py` & `python-icat-1.1.0/icat/chunkedhttp.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/client.py` & `python-icat-1.1.0/icat/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 import os
 from pathlib import Path
 import re
 import time
 import urllib.parse
 from warnings import warn
+import weakref
 
 import suds
 import suds.client
 import suds.sudsobject
 
 from icat.entities import getTypeMap
 from icat.entity import Entity
@@ -72,33 +73,38 @@
         proxy to use as values.
     :type proxy: :class:`dict`
     :param kwargs: additional keyword arguments that will be passed to
         :class:`suds.client.Client`, see :class:`suds.options.Options`
         for details.
     """
 
-    Register = {}
-    """The register of all active clients."""
+    Register = weakref.WeakValueDictionary()
+    """The register of all active clients.
+
+    .. versionchanged:: 1.1.0
+        changed type to :class:`weakref.WeakValueDictionary`.
+    """
 
     AutoRefreshRemain = 30
     """Number of minutes to leave in the session before automatic refresh
     should be called.
     """
 
     @classmethod
     def cleanupall(cls):
         """Cleanup all class instances.
 
         Call :meth:`~icat.client.Client.cleanup` on all registered
         class instances, e.g. on all clients that have not yet been
         cleaned up.
         """
-        cl = list(cls.Register.values())
-        for c in cl:
-            c.cleanup()
+        for r in list(cls.Register.valuerefs()):
+            c = r()
+            if c:
+                c.cleanup()
 
     def _schedule_auto_refresh(self, t=None):
         now = time.time()
         if t == "never":
             # Schedule it very far in the future.  This is just to
             # make sure that self._next_refresh has a formally valid
             # value.
@@ -163,17 +169,17 @@
     def cleanup(self):
         """Release resources allocated by the client.
 
         Logout from the active ICAT session (if :attr:`autoLogout` is
         :const:`True`).  The client should not be used any more after
         calling this method.
         """
+        if self.autoLogout:
+            self.logout()
         if id(self) in self.Register:
-            if self.autoLogout:
-                self.logout()
             del self.Register[id(self)]
 
     def add_ids(self, url, proxy=None):
         """Add the URL to an ICAT Data Service."""
         if proxy is None:
             proxy = self.options.proxy
         idsargs = {}
@@ -228,14 +234,18 @@
         :type obj: :class:`suds.sudsobject.Object` or :class:`str`
         :param kwargs: attributes passed to the constructor of
             :class:`icat.entity.Entity`.
         :return: the new entity object or :const:`None`.
         :rtype: :class:`icat.entity.Entity`
         :raise EntityTypeError: if obj is neither a valid instance
             object, nor a valid name of an entity type, nor None.
+
+        .. versionchanged:: 1.0.0
+            if the `obj` argument is a string, it is taken case
+            insensitive.
         """
 
         if isinstance(obj, suds.sudsobject.Object):
             # obj is already an instance, use it right away
             instance = obj
             instancetype = instance.__class__.__name__
             try:
@@ -785,15 +795,15 @@
         :type infile: :class:`file` or :class:`~pathlib.Path` or :class:`str`
         :param datafile: A Datafile object.
         :type datafile: :class:`icat.entity.Entity`
         :return: The Datafile object created by IDS.
         :rtype: :class:`icat.entity.Entity`
 
         .. versionchanged:: 1.0.0
-            The `infile` parameter also accepts a
+            the `infile` parameter also accepts a
             :class:`~pathlib.Path` object.
         """
 
         if not self.ids:
             raise RuntimeError("no IDS.")
         if not datafile.name:
             raise ValueError("datafile.name is not set.")
@@ -866,14 +876,17 @@
             specify in the Content-Disposition header.
         :type outname: :class:`str`
         :param offset: if larger then zero, add Range header to the
             HTTP request with the indicated bytes offset.
         :type offset: :class:`int`
         :return: a file-like object as returned by
             :meth:`urllib.request.OpenerDirector.open`.
+
+        .. versionchanged:: 0.17.0
+            accept a prepared id in `objs`.
         """
         if not self.ids:
             raise RuntimeError("no IDS.")
         if not isinstance(objs, (DataSelection, str)):
             objs = DataSelection(objs)
         return self.ids.getData(objs, compressFlag, zipFlag, outname, offset)
 
@@ -903,14 +916,17 @@
             format.  For multiple files zip format is always used.
         :type zipFlag: :class:`bool`
         :param outname: the preferred name for the downloaded file to
             specify in the Content-Disposition header.
         :type outname: :class:`str`
         :return: the URL for the data at the IDS.
         :rtype: :class:`str`
+
+        .. versionchanged:: 0.17.0
+            accept a prepared id in `objs`.
         """
         if not self.ids:
             raise RuntimeError("no IDS.")
         if not isinstance(objs, (DataSelection, str)):
             objs = DataSelection(objs)
         return self.ids.getDataUrl(objs, compressFlag, zipFlag, outname)
```

### Comparing `python-icat-1.0.0b1/icat/config.py` & `python-icat-1.1.0/icat/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,34 +373,45 @@
 
     :meth:`icat.config.Config.getconfig` returns a Configuration
     object having the configuration values stored in the respective
     attributes.
     """
     def __init__(self, config):
         self._config = config
+        self._var_nl = None
+
+    @property
+    def _varnames(self):
+        if self._var_nl:
+            return self._var_nl
+        else:
+            return ([var.name for var in self._config.confvariables] +
+                    self._config.ReservedVariables)
+
+    def _freeze_varnames(self):
+        self._var_nl = ([var.name for var in self._config.confvariables] +
+                        self._config.ReservedVariables)
+        del self._config
 
     def __str__(self):
         typename = type(self).__name__
         arg_strings = []
-        vars = [var.name for var in self._config.confvariables] \
-            + self._config.ReservedVariables
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            for f in vars:
+            for f in self._varnames:
                 if hasattr(self, f):
                     arg_strings.append('%s=%r' % (f, getattr(self, f)))
         return '%s(%s)' % (typename, ', '.join(arg_strings))
 
     def as_dict(self):
         """Return the configuration as a :class:`dict`."""
-        vars = [var.name for var in self._config.confvariables] \
-            + self._config.ReservedVariables
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            d = { f:getattr(self, f) for f in vars if hasattr(self, f) }
+            d = { f:getattr(self, f)
+                  for f in self._varnames if hasattr(self, f) }
         return d
 
 
 class BaseConfig():
     """Abstract base class for :class:`icat.config.Config` and
     :class:`icat.config.SubConfig`.  This class defines the common
     API.  It is not intended to be instantiated directly.
@@ -650,14 +661,17 @@
         environment variables, and settings in the configuration files
         still take precedence over the preset values.
     :type preset: :class:`dict`
     :param args: list of command line arguments or :const:`None`.  If
         not set, the command line arguments will be taken from
         :data:`sys.argv`.
     :type args: :class:`list` of :class:`str`
+
+    .. versionchanged:: 1.0.0
+        add the `preset` argument.
     """
 
     def __init__(self, defaultvars=True, needlogin=True, ids="optional", 
                  preset=None, args=None):
         """Initialize the object.
         """
         super().__init__(argparse.ArgumentParser())
@@ -721,14 +735,15 @@
 
         if self.needlogin:
             config.credentials = { 
                 k: getattr(config, self.credentialKey[k].name)
                 for k in self.authenticatorInfo.getCredentialKeys(config.auth)
             }
 
+        config._freeze_varnames()
         return (self.client, config)
 
     def _add_fundamental_variables(self):
         """The fundamental variables that are always needed.
         """
         var = self.add_variable('configFile', ("-c", "--configfile"), 
                                 dict(help="config file"),
```

### Comparing `python-icat-1.0.0b1/icat/dump_queries.py` & `python-icat-1.1.0/icat/dump_queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Define queries needed to dump the full ICAT content.
 
 .. note::
    This module is mostly intended as a helper for the icatdump script.
    Most users will not need to use it directly or even care about it.
 
-The data icatdump is written in chunks, see the documentation of
-icat.dumpfile for details why this is needed.  The partition used
-here is the following:
+ICAT data files are written in chunks.  The partition used here is the
+following:
 
 1. One chunk with all objects that define authorization (User, Group,
    Rule, PublicStep).
 2. All static content in one chunk, e.g. all objects not related to
    individual investigations and that need to be present, before we
    can add investigations.
 3. FundingReferences.
@@ -20,15 +19,21 @@
 5. DataCollections.
 6. DataPublications.  All content related to individual data
    publications, each one in one chunk on its own respectively.
 7. One last chunk with all remaining stuff (Study, RelatedDatafile,
    Job).
 
 The functions defined in this module each return a list of queries
-needed to fetch all objects to be included in one of these chunks.
+needed to fetch the objects to be included in one of these chunks.
+The queries are adapted to the ICAT server version the client is
+connected to.
+
+.. versionchanged:: 1.0.0
+    review the partition to take the schema extensions in ICAT 5.0
+    into account and include the new entity types.
 """
 
 import icat
 from icat.query import Query
 
 __all__ = [ 'getAuthQueries', 'getStaticQueries', 'getFundingQueries',
             'getInvestigationQueries', 'getDataCollectionQueries',
@@ -45,17 +50,20 @@
         Query(client, "Rule", order=["grouping.name", "what", "id"],
               includes={"grouping"}, join_specs={"grouping": "LEFT JOIN"}),
         Query(client, "PublicStep", order=True)
     ]
 
 def getStaticQueries(client):
     """Return the queries to fetch all static objects.
+
+    .. versionchanged:: 1.0.0
+        include queries for ``Technique`` and ``DataPublicationType``.
     """
     # Compatibility between ICAT versions:
-    # - ICAT 5.0.0 added Technique.
+    # - ICAT 5.0.0 added DataPublicationType and Technique.
     queries = [
         Query(client, "Facility", order=True),
         Query(client, "Instrument", order=True,
               includes={"facility", "instrumentScientists.user"}),
         Query(client, "ParameterType", order=True,
               includes={"facility", "permissibleStringValues"}),
         Query(client, "InvestigationType", order=True,
@@ -78,24 +86,32 @@
     if 'technique' in client.typemap:
         # ICAT >= 5.0.0
         queries.insert(0, Query(client, "Technique", order=True) )
     return queries
 
 def getFundingQueries(client):
     """Return the queries to fetch all FundingReferences.
+
+    .. versionadded:: 1.0.0
     """
     # Compatibility between ICAT versions:
     # - ICAT 5.0.0 added FundingReference.
     if 'fundingReference' in client.typemap:
         return [ Query(client, "FundingReference", order=True), ]
     else:
         return []
 
 def getInvestigationQueries(client, invid):
     """Return the queries to fetch all objects related to an investigation.
+
+    .. versionchanged:: 1.0.0
+        add include clauses for ``investigationFacilityCycles`` and
+        ``fundingReferences`` into query for ``Investigation``, add
+        include clauses for ``datasetInstruments`` and
+        ``datasetTechniques`` into query for ``Dataset``.
     """
     # Compatibility between ICAT versions:
     # - ICAT 4.4.0 added InvestigationGroups.
     # - ICAT 4.10.0 added relation between Shift and Instrument.
     # - ICAT 5.0.0 added InvestigationFunding and InvestigationFacilityCycle.
     # - ICAT 5.0.0 added DatasetInstrument and DatasetTechnique.
     inv_includes = {
@@ -140,19 +156,21 @@
               conditions={"dataset.investigation.id": "= %d" % invid},
               includes={"dataset", "datafileFormat.facility",
                         "parameters.type.facility"})
     ]
 
 def getDataCollectionQueries(client):
     """Return the queries to fetch all DataCollections.
+
+    .. versionadded:: 1.0.0
     """
     # Compatibility between ICAT versions:
     # - ICAT 4.3.0 vs. ICAT 4.3.1 and later: name of the parameters
     #   relation in DataCollection.
-    # - ICAT 5.0.0 added DatasetInstrument and DatasetTechnique.
+    # - ICAT 5.0.0 added DataCollectionInvestigation.
     dc_includes = {
         "dataCollectionDatasets.dataset.investigation.facility",
         "dataCollectionDatafiles.datafile.dataset.investigation.facility",
     }
     if 'parameters' in client.typemap['dataCollection'].InstMRel:
         # ICAT >= 4.3.1
         dc_includes |= { "parameters.type.facility" }
@@ -165,32 +183,44 @@
     return [
         Query(client, "DataCollection", order=True,
               includes=dc_includes),
     ]
 
 def getDataPublicationQueries(client, pubid):
     """Return the queries to fetch all objects related to a data publication.
+
+    .. versionadded:: 1.0.0
+
+    .. versionchanged:: 1.1.0
+        return an empty list if the ICAT server is older than 5.0
+        rather than raising :exc:`~icat.exception.EntityTypeError`.
     """
     # Compatibility between ICAT versions:
     # - ICAT 5.0.0 added DataPublication and related classes.
-    # This is not tested here, we assume the caller to check this.
-    # Otherwise the pubid argument would make no sense.
-    return [
-        Query(client, "DataPublication", order=True,
-              conditions={"id": "= %d" % pubid},
-              includes={"facility", "content", "type.facility", "dates",
-                        "fundingReferences.funding", "relatedItems"}),
-        Query(client, "DataPublicationUser", order=True,
-              conditions={"publication.id": "= %d" % pubid},
-              includes={"publication", "user", "affiliations"}),
-    ]
+    if 'dataPublication' in client.typemap:
+        # ICAT >= 5.0.0
+        return [
+            Query(client, "DataPublication", order=True,
+                  conditions={"id": "= %d" % pubid},
+                  includes={"facility", "content", "type.facility", "dates",
+                            "fundingReferences.funding", "relatedItems"}),
+            Query(client, "DataPublicationUser", order=True,
+                  conditions={"publication.id": "= %d" % pubid},
+                  includes={"publication", "user", "affiliations"}),
+        ]
+    else:
+        return []
 
 def getOtherQueries(client):
     """Return the queries to fetch all other objects,
     e.g. not static and not directly related to an investigation.
+
+    .. versionchanged:: 1.0.0
+        drop query for ``DataCollection``, now in a separate function
+        :func:`getDataCollectionQueries`.
     """
     return [
         Query(client, "Study", order=True,
               includes={"user", "studyInvestigations",
                         "studyInvestigations.investigation.facility"}),
         Query(client, "RelatedDatafile", order=True,
               includes={"sourceDatafile.dataset.investigation.facility",
```

### Comparing `python-icat-1.0.0b1/icat/dumpfile.py` & `python-icat-1.1.0/icat/dumpfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     :param infile: the data source to read the objects from.  It
         depends on the backend which kind of data source they accept.
         Most backends will at least accept a file object opened for
         reading or a :class:`~pathlib.Path` or a :class:`str` with a
         file name.
 
     .. versionchanged:: 1.0.0
-        The `infile` parameter also accepts a :class:`~pathlib.Path`
+        the `infile` parameter also accepts a :class:`~pathlib.Path`
         object.
     """
 
     mode = "r"
     """File mode suitable for the backend.
 
     Subclasses should override this with either "rt" or "rb",
@@ -166,15 +166,15 @@
         resetindex = (objindex is None)
         for data in self.getdata():
             self.client.autoRefresh()
             if resetindex:
                 objindex = ChainMap(dict(), self.objindex)
             for key, obj in self.getobjs_from_data(data, objindex):
                 yield obj
-                obj.truncateRelations()
+                obj.truncateRelations(keepInstRel=True)
                 if key:
                     if obj.BeanName in self._retain_entities:
                         self.objindex[key] = obj
                     else:
                         objindex[key] = obj
 
 
@@ -190,15 +190,15 @@
     :type client: :class:`icat.client.Client`
     :param outfile: the data file to write the objects to.  It depends
         on the backend what they accept here.  Most backends will at
         least accept a file object opened for writing or a
         :class:`~pathlib.Path` or a :class:`str` with a file name.
 
     .. versionchanged:: 1.0.0
-        The `outfile` parameter also accepts a :class:`~pathlib.Path`
+        the `outfile` parameter also accepts a :class:`~pathlib.Path`
         object.
     """
 
     mode = "w"
     """File mode suitable for the backend.
 
     Subclasses should override this with either "wt" or "wb",
```

### Comparing `python-icat-1.0.0b1/icat/dumpfile_xml.py` & `python-icat-1.1.0/icat/dumpfile_xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,16 @@
 import datetime
 import os
 import sys
 from lxml import etree
 import icat
 import icat.dumpfile
 from icat.query import Query
-try:
-    utc = datetime.timezone.utc
-except AttributeError:
-    try:
-        from suds.sax.date import UtcTimezone
-        utc = UtcTimezone()
-    except ImportError:
-        utc = None
+
+utc = datetime.timezone.utc
 
 
 # ------------------------------------------------------------
 # XMLDumpFileReader
 # ------------------------------------------------------------
 
 class XMLDumpFileReader(icat.dumpfile.DumpFileReader):
@@ -181,21 +175,18 @@
             elif isinstance(v, datetime.datetime):
                 if v.tzinfo is not None and v.tzinfo.utcoffset(v) is not None:
                     # v has timezone info.  This will be the timezone set
                     # in the ICAT server.  Convert it to UTC to avoid
                     # dependency of server settings in the dumpfile.
                     # Assume v.isoformat() to have a valid timezone
                     # suffix.
-                    if utc:
-                        v = v.astimezone(utc)
-                    v = v.isoformat()
+                    v = v.astimezone(tz=utc).isoformat()
                 else:
-                    # v has no timezone info, assume it to be UTC, append
-                    # the corresponding timezone suffix.
-                    v = v.isoformat() + 'Z'
+                    # v has no timezone info, assume it to be UTC.
+                    v = v.replace(tzinfo=utc).isoformat()
             else:
                 v = str(v)
             etree.SubElement(d, attr).text = v
         for attr in sorted(obj.InstRel):
             o = getattr(obj, attr, None)
             if o is not None:
                 k = o.getUniqueKey(keyindex=keyindex)
@@ -204,15 +195,15 @@
             for o in sorted(getattr(obj, attr), 
                             key=icat.entity.Entity.__sortkey__):
                 d.append(self._entity2elem(o, tag=attr, keyindex=keyindex))
         return d
 
     def head(self):
         """Write a header with some meta information to the data file."""
-        date = datetime.datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S+00:00")
+        date = datetime.datetime.now(tz=utc).isoformat()
         head = etree.Element("head")
         etree.SubElement(head, "date").text = date
         etree.SubElement(head, "service").text = self.client.url
         etree.SubElement(head, "apiversion").text = str(self.client.apiversion)
         etree.SubElement(head, "generator").text = ("icatdump (python-icat %s)" 
                                                     % icat.__version__)
         self.outfile.write(b"""<?xml version="1.0" encoding="utf-8"?>
```

### Comparing `python-icat-1.0.0b1/icat/dumpfile_yaml.py` & `python-icat-1.1.0/icat/dumpfile_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """YAML data file backend for icatdump.py and icatingest.py.
 """
 
 import datetime
 import yaml
 import icat
 import icat.dumpfile
-try:
-    utc = datetime.timezone.utc
-except AttributeError:
-    try:
-        from suds.sax.date import UtcTimezone
-        utc = UtcTimezone()
-    except ImportError:
-        utc = None
+
+utc = datetime.timezone.utc
 
 
 # List of entity types.  This defines in particular the order in which
 # the types must be restored.
 entitytypes = [
     'user',
     'grouping',
@@ -178,21 +172,18 @@
             elif isinstance(v, datetime.datetime):
                 if v.tzinfo is not None and v.tzinfo.utcoffset(v) is not None:
                     # v has timezone info.  This will be the timezone set
                     # in the ICAT server.  Convert it to UTC to avoid
                     # dependency of server settings in the dumpfile.
                     # Assume v.isoformat() to have a valid timezone
                     # suffix.
-                    if utc:
-                        v = v.astimezone(utc)
-                    v = v.isoformat()
+                    v = v.astimezone(tz=utc).isoformat()
                 else:
-                    # v has no timezone info, assume it to be UTC, append
-                    # the corresponding timezone suffix.
-                    v = v.isoformat() + 'Z'
+                    # v has no timezone info, assume it to be UTC.
+                    v = v.replace(tzinfo=utc).isoformat()
             else:
                 v = str(v)
             d[attr] = v
         for attr in obj.InstRel:
             o = getattr(obj, attr, None)
             if o is not None:
                 d[attr] = o.getUniqueKey(keyindex=keyindex)
@@ -202,16 +193,16 @@
                 for o in sorted(getattr(obj, attr), 
                                 key=icat.entity.Entity.__sortkey__):
                     d[attr].append(self._entity2dict(o, keyindex=keyindex))
         return d
 
     def head(self):
         """Write a header with some meta information to the data file."""
-        dateformat = "%a, %d %b %Y %H:%M:%S +0000"
-        date = datetime.datetime.utcnow().strftime(dateformat)
+        dateformat = "%a, %d %b %Y %H:%M:%S %z"
+        date = datetime.datetime.now(tz=utc).strftime(dateformat)
         head = """%%YAML 1.1
 # Date: %s
 # Service: %s
 # ICAT-API: %s
 # Generator: icatdump (python-icat %s)
 """ % (date, self.client.url, self.client.apiversion, icat.__version__)
         self.outfile.write(head)
```

### Comparing `python-icat-1.0.0b1/icat/entities.py` & `python-icat-1.1.0/icat/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Provide the classes corresponding to the entities in the ICAT schema.
 
-Entity classes defined in this module are derived from the abstract
-base class :class:`icat.entity.Entity`.  They override the class
-attributes :attr:`icat.entity.Entity.BeanName`,
+The classes representing the entities in the ICAT schema are
+dynamically created based on the entity information queried from the
+ICAT server.  The classes are derived from the abstract base class
+:class:`icat.entity.Entity`.  They override the class attributes
+:attr:`icat.entity.Entity.BeanName`,
 :attr:`icat.entity.Entity.Constraint`,
 :attr:`icat.entity.Entity.InstAttr`,
 :attr:`icat.entity.Entity.InstRel`,
 :attr:`icat.entity.Entity.InstMRel`,
 :attr:`icat.entity.Entity.AttrAlias`, and
 :attr:`icat.entity.Entity.SortAttrs` as appropriate.
+
+.. versionchanged:: 0.17.0
+    create the entity classes dynamically.
 """
 
 import itertools
 from icat.entity import Entity
 from icat.exception import InternalError
```

### Comparing `python-icat-1.0.0b1/icat/entity.py` & `python-icat-1.1.0/icat/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,18 @@
     entity object.  It will then be called before creating the object
     at the ICAT server.  The function is expected to raise an
     exception (preferably ValueError) in case of validation errors.
     """
 
     @classmethod
     def getInstanceName(cls):
-        """Get the name of this class in the ICAT WSDL"""
+        """Get the name of this class in the ICAT WSDL.
+
+        .. versionadded:: 1.0.0
+        """
         if cls is Entity:
             return 'entityBaseBean'
         else:
             return cls.__name__[0].lower() + cls.__name__[1:]
 
     @classmethod
     def getInstance(cls, obj):
@@ -347,25 +350,40 @@
         :raise ValueError: if no attribute by that name is found.
         """
         if attr in self.AttrAlias:
             attr = self.AttrAlias[attr]
         return self.getAttrInfo(self.client, attr).type
 
 
-    def truncateRelations(self):
+    def truncateRelations(self, keepInstRel=False):
         """Delete all relationships.
 
         Delete all attributes having relationships to other objects
         from this object.  Note that this is a local operation on the
         object in the client only.  It does not affect the
         corresponding object at the ICAT server.  This is useful if
         you only need to keep the object's attributes but not the
         (possibly large) tree of related objects in local memory.
+
+        :param keepInstRel: if :const:`True`, delete only the one to
+            many, but keep the many to one relationships.  This is
+            particularly useful if you want to call
+            :meth:`~icat.entity.Entity.update` for this object later
+            on, because in this case, you'd definitely need to keep
+            the many to one relationships, but you may want to avoid
+            transmitting a large tree of objects in one to many
+            relationships to the ICAT server in the call, as they'd be
+            essentially useless then.
+        :type keepInstRel: :class:`bool`
+
+        .. versionchanged:: 1.1.0
+            add the `keepInstRel` argument.
         """
-        for r in (self.InstRel | self.InstMRel):
+        rels = self.InstMRel if keepInstRel else (self.InstRel | self.InstMRel)
+        for r in rels:
             delattr(self, r)
         
 
     def getUniqueKey(self, keyindex=None):
         """Return a unique key.
 
         The key is a string that is guaranteed to be unique for all
```

### Comparing `python-icat-1.0.0b1/icat/eval.py` & `python-icat-1.1.0/icat/eval.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/exception.py` & `python-icat-1.1.0/icat/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     # icat.query
     'QueryWarning', 'QueryNullableOrderWarning', 'QueryOneToManyOrderWarning',
     # icat.client, icat.entity
     'ClientVersionWarning', 'ICATDeprecationWarning', 
     'EntityTypeError', 'VersionMethodError', 'SearchResultError', 
     'SearchAssertionError', 'DataConsistencyError', 
     # icat.ids
-    'IDSResponseError', 
+    'IDSResponseError',
+    # icat.ingest
+    'InvalidIngestFileError',
     ]
 
 
 # =========================== base class ===========================
 
 class _BaseException(Exception):
     """An exception that tries to suppress misleading context.
@@ -279,15 +281,15 @@
     """
     pass
 
 class QueryNullableOrderWarning(QueryWarning):
     """Warn about using a nullable many to one relation for ordering.
 
     .. versionchanged:: 0.19.0
-        Inherit from :exc:`QueryWarning`.
+        inherit from :exc:`QueryWarning`.
     """
     def __init__(self, attr):
         msg = ("ordering on a nullable many to one relation implicitly "
                "adds a '%s IS NOT NULL' condition." % attr)
         super().__init__(msg)
 
 class QueryOneToManyOrderWarning(QueryWarning):
@@ -333,15 +335,15 @@
                % (feature, icatstr))
         super().__init__(msg)
 
 class EntityTypeError(_BaseException, TypeError):
     """An invalid entity type has been used.
 
     .. versionchanged:: 0.18.0
-        Inherit from :exc:`TypeError`.
+        inherit from :exc:`TypeError`.
     """
     pass
 
 class VersionMethodError(_BaseException):
     """Call of an API method that is not supported in the version
     of the server.
     """
@@ -395,7 +397,22 @@
 
 # ================= Exceptions raised in icat.ids ==================
 
 class IDSResponseError(_BaseException):
     """The response from the IDS was not what should have been expected.
     """
     pass
+
+
+# ================ Exceptions raised in icat.ingest ================
+
+class InvalidIngestFileError(_BaseException, ValueError):
+    """The content of the file is not valid ingest format.
+
+    .. versionadded:: 1.1.0
+    """
+    def __init__(self, detail=None):
+        if detail:
+            msg = "Invalid ingest file: %s" % detail
+        else:
+            msg = "Invalid ingest file"
+        super().__init__(msg)
```

### Comparing `python-icat-1.0.0b1/icat/helper.py` & `python-icat-1.1.0/icat/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     <Version('5.0.0a1')>
     >>> version > '4.11.1'
     True
     >>> version < '5.0.0'
     True
     >>> version == '5.0.0a1'
     True
+
+    .. versionadded:: 1.0.0
     """
     def __init__(self, version):
         super().__init__(re.sub(r'-SNAPSHOT$', 'a1', version))
     def __lt__(self, other):
         if isinstance(other, str):
             other = type(self)(other)
         return super().__lt__(other)
```

### Comparing `python-icat-1.0.0b1/icat/ids.py` & `python-icat-1.1.0/icat/ids.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/listproxy.py` & `python-icat-1.1.0/icat/listproxy.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/query.py` & `python-icat-1.1.0/icat/query.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icat/sslcontext.py` & `python-icat-1.1.0/icat/sslcontext.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icatdump.py` & `python-icat-1.1.0/icatdump.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/icatingest.py` & `python-icat-1.1.0/icatingest.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/setup.py` & `python-icat-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,19 @@
     def finalize_options(self):
         self.package_dir = {}
         if self.distribution.package_dir:
             for name, path in self.distribution.package_dir.items():
                 self.package_dir[name] = convert_path(path)
 
     def run(self):
+        version = self.distribution.get_version()
+        log.info("version: %s", version)
         values = {
-            'version': self.distribution.get_version(),
-            'doc': docstring
+            'version': version,
+            'doc': docstring,
         }
         try:
             pkgname = self.distribution.packages[0]
         except IndexError:
             log.warn("warning: no package defined")
         else:
             pkgdir = Path(self.package_dir.get(pkgname, pkgname))
@@ -115,23 +117,28 @@
         for script in scripts:
             dest = os.path.join(destdir, os.path.basename(script))
             self.copy_file(script, dest, preserve_mode=False)
 
     def copy_test_data(self):
         destdir = os.path.join("tests", "data")
         self.mkpath(destdir)
-        refdumpfiles = ["icatdump-%s.%s" % (ver, ext)
-                        for ver in ("4.4", "4.7", "4.10", "5.0")
-                        for ext in ("xml", "yaml")]
-        files = ["example_data.yaml",
-                 "ingest-datafiles.xml", "ingest-ds-params.xml"] + refdumpfiles
+        files = []
+        files += [ os.path.join("doc", "examples", f)
+                   for f in ["example_data.yaml",
+                             "ingest-datafiles.xml", "ingest-ds-params.xml"] ]
+        files += [ os.path.join("doc", "examples",
+                                "icatdump-%s.%s" % (ver, ext))
+                   for ver in ("4.4", "4.7", "4.10", "5.0")
+                   for ext in ("xml", "yaml") ]
+        files += glob(os.path.join("doc", "examples", "metadata-*.xml"))
+        files += [ os.path.join("etc", f)
+                   for f in ["ingest-10.xsd", "ingest.xslt"] ]
         for f in files:
-            src = os.path.join("doc", "examples", f)
             dest = os.path.join(destdir, os.path.basename(f))
-            self.copy_file(src, dest, preserve_mode=False)
+            self.copy_file(f, dest, preserve_mode=False)
 
 
 # Note: Do not use setuptools for making the source distribution,
 # rather use the good old distutils instead.
 # Rationale: https://rhodesmill.org/brandon/2009/eby-magic/
 class sdist(distutils.command.sdist.sdist):
     def run(self):
@@ -158,28 +165,29 @@
 # There are several forks of the original suds package around, most of
 # them short-lived.  Two of them have been evaluated with python-icat
 # and found to work: suds-jurko and the more recent suds-community.
 # The latter has been renamed to suds.  We don't want to force to use
 # one particular suds clone.  Therefore, we first try if (any clone
 # of) suds is already installed and only add suds to install_requires
 # if not.
-requires = ["packaging"]
+requires = ["lxml", "packaging"]
 try:
     import suds
 except ImportError:
     requires.append("suds")
 
 with Path("README.rst").open("rt", encoding="utf8") as f:
     readme = f.read()
 
 setup(
     name = "python-icat",
     version = version,
     description = docstring.split("\n")[0],
     long_description = readme,
+    long_description_content_type = "text/x-rst",
     url = "https://github.com/icatproject/python-icat",
     author = "Rolf Krahl",
     author_email = "rolf.krahl@helmholtz-berlin.de",
     license = "Apache-2.0",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
@@ -190,16 +198,22 @@
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
+    project_urls = dict(
+        Documentation="https://python-icat.readthedocs.io/",
+        Source="https://github.com/icatproject/python-icat/",
+        Changes="https://python-icat.readthedocs.io/en/latest/changelog.html",
+    ),
     packages = ["icat"],
     python_requires = ">=3.4",
     install_requires = requires,
     scripts = ["icatdump.py", "icatingest.py", "wipeicat.py"],
     cmdclass = dict(cmdclass,
                     meta=meta,
                     build_py=build_py,
```

### Comparing `python-icat-1.0.0b1/tests/conftest.py` & `python-icat-1.1.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 import subprocess
 import sys
 import tempfile
 import zlib
 import pytest
 import icat
 import icat.config
+import icat.dumpfile
+try:
+    import icat.dumpfile_xml
+except ImportError:
+    pass
+try:
+    import icat.dumpfile_yaml
+except ImportError:
+    pass
 from icat.helper import Version
 try:
     from suds.sax.date import UtcTimezone
 except ImportError:
     UtcTimezone = None
 
 # There are tests that depend on being able to read utf8-encoded text
@@ -35,15 +44,15 @@
 # error.  The problem is that suds is rather chatty, so it will
 # clutter the output to an extent that we wont be able to see
 # anything.  Silence it.
 logging.getLogger('suds.client').setLevel(logging.CRITICAL)
 logging.getLogger('suds').setLevel(logging.ERROR)
 
 testdir = Path(__file__).resolve().parent
-
+testdatadir = testdir / "data"
 
 def _skip(reason):
     if Version(pytest.__version__) >= '3.3.0':
         pytest.skip(reason, allow_module_level=True)
     else:
         raise pytest.skip.Exception(reason, allow_module_level=True)
 
@@ -79,15 +88,15 @@
         else:
             self.mtime = None
 
 
 def getConfig(confSection="root", **confArgs):
     """Get the configuration, skip on ConfigError.
     """
-    confFile = testdir / "data" / "icat.cfg"
+    confFile = testdatadir / "icat.cfg"
     if not confFile.is_file():
         _skip("no test ICAT server configured")
     try:
         confArgs['args'] = ["-c", str(confFile), "-s", confSection]
         client, conf = icat.config.Config(**confArgs).getconfig()
         conf.cmdargs = ["-c", str(conf.configFile[0]), "-s", conf.configSection]
         return (client, conf)
@@ -118,15 +127,15 @@
         self.client.login(self.conf.auth, self.conf.credentials)
         return self.client
     def __exit__(self, type, value, tb):
         self.client.logout()
 
 
 def gettestdata(fname):
-    fname = testdir / "data" / fname
+    fname = testdatadir / fname
     assert fname.is_file()
     return fname
 
 
 def get_icat_version():
     client, _ = getConfig(needlogin=False)
     ids_version = client.ids.apiversion if client.ids else Version("0.0")
@@ -140,14 +149,18 @@
 except:
     icat_version, ids_version = Version("0.0"), Version("0.0")
 
 def require_icat_version(minversion, reason):
     if icat_version < minversion:
         _skip("need ICAT server version %s or newer: %s" % (minversion, reason))
 
+def require_dumpfile_backend(backend):
+    if backend not in icat.dumpfile.Backends.keys():
+        _skip("need %s backend for icat.dumpfile" % (backend))
+
 
 def get_reference_dumpfile(ext = "yaml"):
     require_icat_version("4.4.0", "oldest available set of test data")
     if icat_version < "4.7":
         fname = "icatdump-4.4.%s" % ext
     elif icat_version < "4.10":
         fname = "icatdump-4.7.%s" % ext
@@ -217,14 +230,15 @@
 def standardCmdArgs():
     _, conf = getConfig()
     return conf.cmdargs
 
 
 @pytest.fixture(scope="session")
 def setupicat(standardCmdArgs):
+    require_dumpfile_backend("YAML")
     testcontent = get_reference_dumpfile()
     callscript("wipeicat.py", standardCmdArgs)
     args = standardCmdArgs + ["-f", "YAML", "-i", str(testcontent)]
     callscript("icatingest.py", args)
 
 # ============================= hooks ================================
```

### Comparing `python-icat-1.0.0b1/tests/data/summary-4` & `python-icat-1.1.0/tests/data/summary-4`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-4.acord` & `python-icat-1.1.0/tests/data/summary-4.acord`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-4.ahau` & `python-icat-1.1.0/tests/data/summary-4.ahau`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-4.jbotu` & `python-icat-1.1.0/tests/data/summary-4.jbotu`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-4.jdoe` & `python-icat-1.1.0/tests/data/summary-4.jdoe`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-4.nbour` & `python-icat-1.1.0/tests/data/summary-4.nbour`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-4.rbeck` & `python-icat-1.1.0/tests/data/summary-4.rbeck`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5` & `python-icat-1.1.0/tests/data/summary-5`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5.acord` & `python-icat-1.1.0/tests/data/summary-5.acord`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5.ahau` & `python-icat-1.1.0/tests/data/summary-5.ahau`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5.jbotu` & `python-icat-1.1.0/tests/data/summary-5.jbotu`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5.jdoe` & `python-icat-1.1.0/tests/data/summary-5.jdoe`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5.nbour` & `python-icat-1.1.0/tests/data/summary-5.nbour`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/data/summary-5.rbeck` & `python-icat-1.1.0/tests/data/summary-5.rbeck`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_01_config.py` & `python-icat-1.1.0/tests/test_01_config.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_01_helper.py` & `python-icat-1.1.0/tests/test_01_helper.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_01_listproxy.py` & `python-icat-1.1.0/tests/test_01_listproxy.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_03_getversion.py` & `python-icat-1.1.0/tests/test_03_getversion.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_03_login.py` & `python-icat-1.1.0/tests/test_03_login.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_03_script.py` & `python-icat-1.1.0/tests/test_03_script.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_05_dump.py` & `python-icat-1.1.0/tests/test_05_dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from pytest_dependency import depends
 except ImportError:
     def depends(request, other_tests):
         pass
 import icat
 import icat.config
 from conftest import (getConfig, icat_version, gettestdata,
+                      require_dumpfile_backend,
                       get_reference_dumpfile, get_reference_summary,
                       callscript, filter_file, yaml_filter, xml_filter)
 
 
 backends = {
     'XML': {
         'refdump': get_reference_dumpfile("xml"),
@@ -108,14 +109,15 @@
 
 
 @pytest.mark.dependency()
 def test_ingest(ingestcase, standardCmdArgs):
     """Restore the ICAT content from a dumpfile.
     """
     backend, filetype = ingestcase
+    require_dumpfile_backend(backend)
     refdump = backends[backend]['refdump']
     if filetype == 'FILE':
         args = standardCmdArgs + ["-f", backend, "-i", str(refdump)]
         callscript("icatingest.py", args)
     elif filetype == 'STDINOUT':
         args = standardCmdArgs + ["-f", backend]
         with refdump.open("rt") as infile:
@@ -124,14 +126,15 @@
         raise RuntimeError("Invalid file type %s" % filetype)
 
 @pytest.mark.parametrize(("case"), cases)
 def test_check_content(ingestcheck, standardCmdArgs, tmpdirsec, case):
     """Dump the content and check that we get the reference dump file back.
     """
     backend, filetype = case
+    require_dumpfile_backend(backend)
     refdump = backends[backend]['refdump']
     fileext = backends[backend]['fileext']
     dump = tmpdirsec / ("dump" + fileext)
     fdump = tmpdirsec / ("dump-filter" + fileext)
     reffdump = tmpdirsec / ("dump-filter-ref" + fileext)
     filter_file(refdump, reffdump, *backends[backend]['filter'])
     if filetype == 'FILE':
```

### Comparing `python-icat-1.0.0b1/tests/test_05_dumpfile.py` & `python-icat-1.1.0/tests/test_05_dumpfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 This test module has a similar structure as test_05_dump.py, but
 rather than calling icatdump and icatingest as external scripts, it
 uses the internal API icat.dumpfile.
 """
 
 import filecmp
 import io
-from lxml import etree
+try:
+    from lxml import etree
+except ImportError:
+    etree = None
 import pytest
 try:
     from pytest_dependency import depends
 except ImportError:
     def depends(request, other_tests):
         pass
 import icat
 import icat.config
 from icat.dump_queries import *
 from icat.dumpfile import open_dumpfile
-import icat.dumpfile_xml
-import icat.dumpfile_yaml
 from icat.query import Query
-from conftest import (getConfig, get_reference_dumpfile, callscript,
+from conftest import (getConfig, require_dumpfile_backend,
+                      get_reference_dumpfile, callscript,
                       filter_file, yaml_filter, xml_filter)
 
 
 backends = {
     'XML': {
         'refdump': get_reference_dumpfile("xml"),
         'fileext': '.xml',
@@ -33,15 +35,14 @@
     },
     'YAML': {
         'refdump': get_reference_dumpfile("yaml"),
         'fileext': '.yaml',
         'filter': yaml_filter,
     },
 }
-assert backends.keys() == icat.dumpfile.Backends.keys()
 
 # The following cases are tuples of a backend and a file type (regular
 # file, stdin/stdout, in-memory stream).  They are used for both,
 # input and output.  We test all combinations, e.g. reading from a XML
 # file and writing it back as YAML to stdout.
 cases = [ (b, t) 
           for b in backends.keys() 
@@ -124,38 +125,42 @@
 # ============================= tests ================================
 
 @pytest.mark.dependency()
 def test_ingest(ingestcase, client):
     """Restore the ICAT content from a dumpfile.
     """
     backend, filetype = ingestcase
+    require_dumpfile_backend(backend)
     refdump = backends[backend]['refdump']
     if filetype == 'FILE':
         icatingest(client, refdump, backend)
     elif filetype == 'MEMORY':
         with refdump.open("rb") as f:
             icatdata = f.read()
         if 'b' in icat.dumpfile.Backends[backend][0].mode:
             stream = io.BytesIO(icatdata)
         else:
             stream = io.StringIO(icatdata.decode('ascii'))
         icatingest(client, stream, backend)
         stream.close()
     elif filetype == 'ETREE':
+        if etree is None:
+            pytest.skip("Need lxml")
         with refdump.open("rb") as f:
             icatdata = etree.parse(f)
         icatingest(client, icatdata, backend)
     else:
         raise RuntimeError("Invalid file type %s" % filetype)
 
 @pytest.mark.parametrize(("case"), ocases)
 def test_check_content(ingestcheck, client, tmpdirsec, case):
     """Dump the content and check that we get the reference dump file back.
     """
     backend, filetype = case
+    require_dumpfile_backend(backend)
     refdump = backends[backend]['refdump']
     fileext = backends[backend]['fileext']
     dump = tmpdirsec / ("dump" + fileext)
     fdump = tmpdirsec / ("dump-filter" + fileext)
     reffdump = tmpdirsec / ("dump-filter-ref" + fileext)
     filter_file(refdump, reffdump, *backends[backend]['filter'])
     if filetype == 'FILE':
```

### Comparing `python-icat-1.0.0b1/tests/test_05_setup.py` & `python-icat-1.1.0/tests/test_05_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 server, creating a few example investigations, and adding some data to
 these investigations.  It then compares the result with a reference
 dump file.
 """
 
 import filecmp
 import re
-import yaml
+try:
+    import yaml
+except ImportError:
+    yaml = None
 import pytest
 import icat
 import icat.config
 from icat.query import Query
 from conftest import (getConfig, icat_version, gettestdata,
+                      require_dumpfile_backend,
                       get_reference_dumpfile, get_reference_summary,
                       callscript, filter_file, yaml_filter)
 
 
 # Study is broken in icat.server older then 4.6.0, see
 # icatproject/icat.server#155.  We do not maintain specific set of
 # test data for 4.6.  Therefore we skip testing Study for ICAT older
@@ -46,14 +50,16 @@
     alldata.extend(["data_pub1", "data_collect2"])
 summary_study_filter = (re.compile(r"^((?:Study(?:Investigation)?)\s*) : \d+$"),
                         r"\1 : 0")
 
 
 @pytest.fixture(scope="module")
 def data():
+    if yaml is None:
+        pytest.skip("Need yaml")
     with testinput.open('r') as f:
         return yaml.safe_load(f)
 
 
 def initobj(obj, attrs):
     """Initialize an entity object from a dict of attributes."""
     for a in obj.InstAttr:
@@ -128,14 +134,16 @@
         inv.fileCount += ds.fileCount
         inv.fileSize += ds.fileSize
     inv.update()
 
 
 @pytest.mark.dependency(name="init")
 def test_init(standardCmdArgs):
+    if yaml is None:
+        pytest.skip("Need yaml")
     callscript("wipeicat.py", standardCmdArgs)
     callscript("init-icat.py", standardCmdArgs + [str(testinput)])
 
 
 @pytest.mark.parametrize("invname", [
     pytest.param("08100122-EF",
                  marks=pytest.mark.dependency(name="inv_081",
@@ -382,14 +390,15 @@
             raise AssertionError("invalid object type %s" % obj.BeanName)
     collection.create()
 
 @pytest.mark.dependency(depends=alldata)
 def test_check_content(standardCmdArgs, tmpdirsec):
     """Dump the resulting content and compare with a reference dump.
     """
+    require_dumpfile_backend("YAML")
     dump = tmpdirsec / "dump.yaml"
     fdump = tmpdirsec / "dump-filter.yaml"
     reffdump = tmpdirsec / "dump-filter-ref.yaml"
     filter_file(refdump, reffdump, *yaml_filter)
     args = standardCmdArgs + ["-f", "YAML", "-o", str(dump)]
     callscript("icatdump.py", args)
     filter_file(dump, fdump, *yaml_filter)
```

### Comparing `python-icat-1.0.0b1/tests/test_06_client.py` & `python-icat-1.1.0/tests/test_06_client.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_06_exception.py` & `python-icat-1.1.0/tests/test_06_exception.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_06_ids.py` & `python-icat-1.1.0/tests/test_06_ids.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_06_ingest.py` & `python-icat-1.1.0/tests/test_06_icatingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-"""Test icatdump and icatingest.
+"""Test ingest metadata using the icatingest script.
 """
 
 from subprocess import CalledProcessError
 import pytest
 import icat
 import icat.config
 from icat.query import Query
-from conftest import DummyDatafile, gettestdata, getConfig, callscript
+from conftest import (DummyDatafile, require_dumpfile_backend,
+                      gettestdata, getConfig, callscript)
 
 
 # Test input
 ds_params = str(gettestdata("ingest-ds-params.xml"))
 datafiles = str(gettestdata("ingest-datafiles.xml"))
 
 @pytest.fixture(scope="module")
 def client(setupicat):
     client, conf = getConfig(confSection="acord", ids="mandatory")
     client.login(conf.auth, conf.credentials)
     return client
 
 @pytest.fixture(scope="module")
 def cmdargs(setupicat):
+    require_dumpfile_backend("XML")
     _, conf = getConfig(confSection="acord", ids="mandatory")
     return conf.cmdargs + ["-f", "XML"]
 
 @pytest.fixture(scope="function")
 def dataset(client):
     """A dataset to be used in the test.
```

### Comparing `python-icat-1.0.0b1/tests/test_06_query.py` & `python-icat-1.1.0/tests/test_06_query.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_client_clone.py` & `python-icat-1.1.0/tests/test_07_client_clone.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_client_options.py` & `python-icat-1.1.0/tests/test_07_client_options.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_dataselection.py` & `python-icat-1.1.0/tests/test_07_dataselection.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_entity_copy.py` & `python-icat-1.1.0/tests/test_07_entity_copy.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_entity_equal.py` & `python-icat-1.1.0/tests/test_07_entity_equal.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_entity_sort.py` & `python-icat-1.1.0/tests/test_07_entity_sort.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/tests/test_07_entity_validate.py` & `python-icat-1.1.0/tests/test_07_entity_validate.py`

 * *Files identical despite different names*

### Comparing `python-icat-1.0.0b1/wipeicat.py` & `python-icat-1.1.0/wipeicat.py`

 * *Files identical despite different names*

