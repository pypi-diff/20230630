# Comparing `tmp/msgtools-0.37.8.tar.gz` & `tmp/msgtools-0.37.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgtools-0.37.8.tar", last modified: Fri Jan 13 18:35:16 2023, max compression
+gzip compressed data, was "msgtools-0.37.9.tar", last modified: Fri Jan 13 18:37:01 2023, max compression
```

## Comparing `msgtools-0.37.8.tar` & `msgtools-0.37.9.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.106259 msgtools-0.37.8/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      309 2020-06-17 22:29:42.000000 msgtools-0.37.8/LICENSE.txt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      843 2023-01-13 18:35:16.106259 msgtools-0.37.8/PKG-INFO
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      787 2020-06-17 22:29:42.000000 msgtools-0.37.8/README.md
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.082259 msgtools-0.37.8/msgtools/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/__init__.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.082259 msgtools-0.37.8/msgtools/console/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/console/__init__.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     9982 2023-01-09 21:28:02.000000 msgtools-0.37.8/msgtools/console/client.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     5177 2022-03-02 21:39:55.000000 msgtools-0.37.8/msgtools/console/console.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     5531 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/console/server.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.082259 msgtools-0.37.8/msgtools/csvparse/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-08-23 22:27:24.000000 msgtools-0.37.8/msgtools/csvparse/__init__.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     3810 2020-08-23 22:27:24.000000 msgtools-0.37.8/msgtools/csvparse/csvparse.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.082259 msgtools-0.37.8/msgtools/database/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/database/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      313 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/database/dalmatiner.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2924 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/database/influx.png
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2647 2022-03-24 05:46:29.000000 msgtools-0.37.8/msgtools/database/influx_msgserver_plugin.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    11542 2022-09-07 21:30:56.000000 msgtools-0.37.8/msgtools/database/influxdb.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.086259 msgtools-0.37.8/msgtools/debug/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/debug/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1343 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/debug/debug.png
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    25972 2022-12-13 18:28:20.000000 msgtools-0.37.8/msgtools/debug/debug.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     8028 2022-11-26 17:43:10.000000 msgtools-0.37.8/msgtools/debug/findprints.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      268 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/debug/launcher.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.086259 msgtools-0.37.8/msgtools/inspector/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/inspector/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3933 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/inspector/inspector.png
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     6081 2022-02-14 07:28:01.000000 msgtools-0.37.8/msgtools/inspector/inspector.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      284 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/inspector/launcher.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.086259 msgtools-0.37.8/msgtools/launcher/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/launcher/__init__.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     5570 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/launcher/codegen_gui.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6043 2022-02-14 07:39:49.000000 msgtools-0.37.8/msgtools/launcher/launcher.png
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    10122 2022-06-09 20:37:22.000000 msgtools-0.37.8/msgtools/launcher/launcher.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.090259 msgtools-0.37.8/msgtools/lib/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/lib/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    17862 2022-05-11 22:51:06.000000 msgtools-0.37.8/msgtools/lib/app.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2700 2020-08-25 23:10:15.000000 msgtools-0.37.8/msgtools/lib/conversions.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3277 2021-02-02 19:42:01.000000 msgtools-0.37.8/msgtools/lib/createmsgdialog.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4348 2022-09-29 18:51:10.000000 msgtools-0.37.8/msgtools/lib/file_reader.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    23765 2022-10-05 11:51:01.000000 msgtools-0.37.8/msgtools/lib/gui.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    10670 2022-12-28 00:45:01.000000 msgtools-0.37.8/msgtools/lib/header_translator.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6769 2022-09-29 18:25:48.000000 msgtools-0.37.8/msgtools/lib/message.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    22683 2023-01-13 05:22:16.000000 msgtools-0.37.8/msgtools/lib/messaging.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13022 2022-03-02 21:20:10.000000 msgtools-0.37.8/msgtools/lib/msgcsv.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4792 2022-10-18 16:25:09.000000 msgtools-0.37.8/msgtools/lib/msgjson.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     6981 2023-01-03 18:50:34.000000 msgtools-0.37.8/msgtools/lib/msgpandas.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    18098 2022-10-04 15:47:33.000000 msgtools-0.37.8/msgtools/lib/msgplot.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    12165 2023-01-13 05:19:02.000000 msgtools-0.37.8/msgtools/lib/txtreewidget.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     1624 2020-08-23 22:27:24.000000 msgtools-0.37.8/msgtools/lib/unknownmsg.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.090259 msgtools-0.37.8/msgtools/lumberjack/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/lumberjack/__init__.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     4853 2022-09-29 03:49:26.000000 msgtools-0.37.8/msgtools/lumberjack/lumberjack.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1241 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/lumberjack/read_json.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.090259 msgtools-0.37.8/msgtools/multilog/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/multilog/__init__.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    15604 2023-01-13 04:13:10.000000 msgtools-0.37.8/msgtools/multilog/multilog.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.090259 msgtools-0.37.8/msgtools/noisemaker/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/noisemaker/__init__.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     3606 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/noisemaker/bandwidthtestecho.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     8973 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/noisemaker/bandwidthtester.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      288 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/noisemaker/launcher.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2429 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/noisemaker/noisemaker.png
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     7089 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/noisemaker/noisemaker.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.090259 msgtools-0.37.8/msgtools/parser/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    26236 2023-01-12 23:24:49.000000 msgtools-0.37.8/msgtools/parser/MsgUtils.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/__init__.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/c/
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)      590 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/c/HeaderTemplate.h
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      445 2021-07-22 04:52:41.000000 msgtools-0.37.8/msgtools/parser/c/Template.h
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/c/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1973 2021-07-22 04:52:41.000000 msgtools-0.37.8/msgtools/parser/c/language.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     5773 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/check.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/cpp/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1211 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/cpp/HeaderTemplate.h
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1590 2022-09-29 20:07:10.000000 msgtools-0.37.8/msgtools/parser/cpp/Template.h
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/cpp/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    18295 2023-01-13 18:31:55.000000 msgtools-0.37.8/msgtools/parser/cpp/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/dart/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1071 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/dart/HeaderTemplate.dart
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1725 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/dart/Template.dart
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/dart/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    12517 2022-03-26 02:48:35.000000 msgtools-0.37.8/msgtools/parser/dart/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/html/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1676 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/html/HeaderTemplate.html
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1747 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/html/Template.html
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/html/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)   122540 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/html/bootstrap.min.css
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4063 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/html/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/java/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      980 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/java/HeaderTemplate.java
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1179 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/java/Template.java
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/java/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13686 2021-02-26 22:06:25.000000 msgtools-0.37.8/msgtools/parser/java/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/javascript/
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     1505 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/javascript/HeaderTemplate.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1964 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/javascript/Template.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/javascript/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13603 2023-01-12 23:54:46.000000 msgtools-0.37.8/msgtools/parser/javascript/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/kotlin/
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)      763 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/kotlin/HeaderTemplate.kt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      727 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/kotlin/Template.kt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/kotlin/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13617 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/kotlin/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/matlab/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1091 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/matlab/HeaderTemplate.m
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      905 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/matlab/Template.m
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/matlab/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    11123 2021-03-10 23:02:47.000000 msgtools-0.37.8/msgtools/parser/matlab/language.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    19030 2023-01-10 03:27:34.000000 msgtools-0.37.8/msgtools/parser/parser.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/python/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3083 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/python/HeaderTemplate.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1394 2020-08-25 23:10:15.000000 msgtools-0.37.8/msgtools/parser/python/Template.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/python/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    12909 2023-01-13 18:26:35.000000 msgtools-0.37.8/msgtools/parser/python/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.094259 msgtools-0.37.8/msgtools/parser/simulink/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      410 2021-07-22 04:52:41.000000 msgtools-0.37.8/msgtools/parser/simulink/HeaderTemplate.m
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2975 2021-07-22 04:52:41.000000 msgtools-0.37.8/msgtools/parser/simulink/Template.m
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2021-07-22 04:52:41.000000 msgtools-0.37.8/msgtools/parser/simulink/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4170 2021-07-22 04:52:41.000000 msgtools-0.37.8/msgtools/parser/simulink/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.098259 msgtools-0.37.8/msgtools/parser/swift/
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)      856 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/swift/HeaderTemplate.swift
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1153 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/swift/Template.swift
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/swift/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    16214 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/parser/swift/language.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.098259 msgtools-0.37.8/msgtools/scope/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/scope/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      268 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/scope/launcher.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1984 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/scope/scope.png
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    21435 2023-01-13 04:12:13.000000 msgtools-0.37.8/msgtools/scope/scope.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.098259 msgtools-0.37.8/msgtools/script/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/script/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     5678 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/script/debugger.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4198 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/script/edit_window.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      272 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/script/launcher.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1546 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/script/script.png
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    14081 2022-02-14 07:29:19.000000 msgtools-0.37.8/msgtools/script/script.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.102259 msgtools-0.37.8/msgtools/server/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4378 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/BluetoothRFCOMM.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3797 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/BluetoothRFCOMMQt.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    20014 2022-04-15 19:43:49.000000 msgtools-0.37.8/msgtools/server/CanPlugin.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3907 2022-03-26 22:10:59.000000 msgtools-0.37.8/msgtools/server/CanPortDialog.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     8189 2022-09-26 17:19:49.000000 msgtools-0.37.8/msgtools/server/SerialPlugin.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2617 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/SerialportDialog.py
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     4290 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/TcpServer.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2445 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/WebSocketServer.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      272 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/launcher.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2308 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/server/server.png
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    24348 2022-02-14 07:24:02.000000 msgtools-0.37.8/msgtools/server/server.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2541 2022-03-26 22:12:24.000000 msgtools-0.37.8/msgtools/server/socketcan_commands.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.102259 msgtools-0.37.8/msgtools/sim/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2022-10-23 01:41:53.000000 msgtools-0.37.8/msgtools/sim/__init__.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    21027 2022-12-28 00:45:01.000000 msgtools-0.37.8/msgtools/sim/sim.py
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     5644 2023-01-09 21:23:23.000000 msgtools-0.37.8/msgtools/sim/sim_exec.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.102259 msgtools-0.37.8/msgtools/webapp/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/__init__.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.102259 msgtools-0.37.8/msgtools/webapp/lib/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6751 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/Histogram-component.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2483 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/MsgDialog.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    10730 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/MsgFieldLabel.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6538 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/MsgPlot.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3397 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/MsgSelector.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3338 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/MsgTabs.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3520 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/MsgTree.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     9741 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/Plot-component.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    21680 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/WebSocketUtils.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)   151725 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/d3.v3.min.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    22916 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/lib/msgtools.js
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      693 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/template.html
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     2959 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/template.js
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     8240 2020-06-17 22:29:43.000000 msgtools-0.37.8/msgtools/webapp/webapp.py
-drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:35:16.082259 msgtools-0.37.8/msgtools.egg-info/
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      843 2023-01-13 18:35:15.000000 msgtools-0.37.8/msgtools.egg-info/PKG-INFO
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4742 2023-01-13 18:35:15.000000 msgtools-0.37.8/msgtools.egg-info/SOURCES.txt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        1 2023-01-13 18:35:15.000000 msgtools-0.37.8/msgtools.egg-info/dependency_links.txt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1989 2023-01-13 18:35:15.000000 msgtools-0.37.8/msgtools.egg-info/entry_points.txt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        1 2020-06-17 22:29:42.000000 msgtools-0.37.8/msgtools.egg-info/not-zip-safe
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)       96 2023-01-13 18:35:15.000000 msgtools-0.37.8/msgtools.egg-info/requires.txt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        9 2023-01-13 18:35:15.000000 msgtools-0.37.8/msgtools.egg-info/top_level.txt
--rw-rw-r--   0 mgazic    (1001) mgazic    (1001)       79 2023-01-13 18:35:16.106259 msgtools-0.37.8/setup.cfg
--rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     4604 2023-01-13 18:35:07.000000 msgtools-0.37.8/setup.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      309 2020-06-17 22:29:42.000000 msgtools-0.37.9/LICENSE.txt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      843 2023-01-13 18:37:01.986766 msgtools-0.37.9/PKG-INFO
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      787 2020-06-17 22:29:42.000000 msgtools-0.37.9/README.md
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/__init__.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/console/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/console/__init__.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     9982 2023-01-09 21:28:02.000000 msgtools-0.37.9/msgtools/console/client.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     5177 2022-03-02 21:39:55.000000 msgtools-0.37.9/msgtools/console/console.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     5531 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/console/server.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/csvparse/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-08-23 22:27:24.000000 msgtools-0.37.9/msgtools/csvparse/__init__.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     3810 2020-08-23 22:27:24.000000 msgtools-0.37.9/msgtools/csvparse/csvparse.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/database/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/database/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      313 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/database/dalmatiner.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2924 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/database/influx.png
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2647 2022-03-24 05:46:29.000000 msgtools-0.37.9/msgtools/database/influx_msgserver_plugin.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    11542 2022-09-07 21:30:56.000000 msgtools-0.37.9/msgtools/database/influxdb.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/debug/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/debug/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1343 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/debug/debug.png
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    25972 2022-12-13 18:28:20.000000 msgtools-0.37.9/msgtools/debug/debug.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     8028 2022-11-26 17:43:10.000000 msgtools-0.37.9/msgtools/debug/findprints.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      268 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/debug/launcher.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/inspector/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/inspector/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3933 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/inspector/inspector.png
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     6081 2022-02-14 07:28:01.000000 msgtools-0.37.9/msgtools/inspector/inspector.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      284 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/inspector/launcher.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/launcher/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/launcher/__init__.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     5570 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/launcher/codegen_gui.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6043 2022-02-14 07:39:49.000000 msgtools-0.37.9/msgtools/launcher/launcher.png
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    10122 2022-06-09 20:37:22.000000 msgtools-0.37.9/msgtools/launcher/launcher.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/lib/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/lib/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    17862 2022-05-11 22:51:06.000000 msgtools-0.37.9/msgtools/lib/app.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2700 2020-08-25 23:10:15.000000 msgtools-0.37.9/msgtools/lib/conversions.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3277 2021-02-02 19:42:01.000000 msgtools-0.37.9/msgtools/lib/createmsgdialog.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4348 2022-09-29 18:51:10.000000 msgtools-0.37.9/msgtools/lib/file_reader.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    23765 2022-10-05 11:51:01.000000 msgtools-0.37.9/msgtools/lib/gui.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    10670 2022-12-28 00:45:01.000000 msgtools-0.37.9/msgtools/lib/header_translator.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6769 2022-09-29 18:25:48.000000 msgtools-0.37.9/msgtools/lib/message.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    22683 2023-01-13 05:22:16.000000 msgtools-0.37.9/msgtools/lib/messaging.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13022 2022-03-02 21:20:10.000000 msgtools-0.37.9/msgtools/lib/msgcsv.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4792 2022-10-18 16:25:09.000000 msgtools-0.37.9/msgtools/lib/msgjson.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     6981 2023-01-03 18:50:34.000000 msgtools-0.37.9/msgtools/lib/msgpandas.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    18098 2022-10-04 15:47:33.000000 msgtools-0.37.9/msgtools/lib/msgplot.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    12165 2023-01-13 05:19:02.000000 msgtools-0.37.9/msgtools/lib/txtreewidget.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     1624 2020-08-23 22:27:24.000000 msgtools-0.37.9/msgtools/lib/unknownmsg.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/lumberjack/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/lumberjack/__init__.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     4853 2022-09-29 03:49:26.000000 msgtools-0.37.9/msgtools/lumberjack/lumberjack.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1241 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/lumberjack/read_json.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/multilog/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/multilog/__init__.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    15604 2023-01-13 04:13:10.000000 msgtools-0.37.9/msgtools/multilog/multilog.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/noisemaker/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/noisemaker/__init__.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     3606 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/noisemaker/bandwidthtestecho.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     8973 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/noisemaker/bandwidthtester.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      288 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/noisemaker/launcher.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2429 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/noisemaker/noisemaker.png
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     7089 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/noisemaker/noisemaker.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/parser/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    26236 2023-01-12 23:24:49.000000 msgtools-0.37.9/msgtools/parser/MsgUtils.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/__init__.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/parser/c/
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)      590 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/c/HeaderTemplate.h
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      445 2021-07-22 04:52:41.000000 msgtools-0.37.9/msgtools/parser/c/Template.h
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/c/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1973 2021-07-22 04:52:41.000000 msgtools-0.37.9/msgtools/parser/c/language.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     5773 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/check.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/parser/cpp/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1211 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/cpp/HeaderTemplate.h
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1590 2022-09-29 20:07:10.000000 msgtools-0.37.9/msgtools/parser/cpp/Template.h
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/cpp/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    18295 2023-01-13 18:31:55.000000 msgtools-0.37.9/msgtools/parser/cpp/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools/parser/dart/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1071 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/dart/HeaderTemplate.dart
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1725 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/dart/Template.dart
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/dart/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    12517 2022-03-26 02:48:35.000000 msgtools-0.37.9/msgtools/parser/dart/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/html/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1676 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/html/HeaderTemplate.html
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1747 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/html/Template.html
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/html/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)   122540 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/html/bootstrap.min.css
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4063 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/html/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/java/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      980 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/java/HeaderTemplate.java
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1179 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/java/Template.java
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/java/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13686 2021-02-26 22:06:25.000000 msgtools-0.37.9/msgtools/parser/java/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/javascript/
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     1505 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/javascript/HeaderTemplate.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1964 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/javascript/Template.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/javascript/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13770 2023-01-13 18:36:17.000000 msgtools-0.37.9/msgtools/parser/javascript/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/kotlin/
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)      763 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/kotlin/HeaderTemplate.kt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      727 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/kotlin/Template.kt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/kotlin/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    13617 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/kotlin/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/matlab/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1091 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/matlab/HeaderTemplate.m
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      905 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/matlab/Template.m
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/matlab/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    11123 2021-03-10 23:02:47.000000 msgtools-0.37.9/msgtools/parser/matlab/language.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    19030 2023-01-10 03:27:34.000000 msgtools-0.37.9/msgtools/parser/parser.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/python/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3083 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/python/HeaderTemplate.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1394 2020-08-25 23:10:15.000000 msgtools-0.37.9/msgtools/parser/python/Template.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/python/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    12909 2023-01-13 18:26:35.000000 msgtools-0.37.9/msgtools/parser/python/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/simulink/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      410 2021-07-22 04:52:41.000000 msgtools-0.37.9/msgtools/parser/simulink/HeaderTemplate.m
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2975 2021-07-22 04:52:41.000000 msgtools-0.37.9/msgtools/parser/simulink/Template.m
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2021-07-22 04:52:41.000000 msgtools-0.37.9/msgtools/parser/simulink/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4170 2021-07-22 04:52:41.000000 msgtools-0.37.9/msgtools/parser/simulink/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/parser/swift/
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)      856 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/swift/HeaderTemplate.swift
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1153 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/swift/Template.swift
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/swift/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    16214 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/parser/swift/language.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/scope/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/scope/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      268 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/scope/launcher.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1984 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/scope/scope.png
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    21435 2023-01-13 04:12:13.000000 msgtools-0.37.9/msgtools/scope/scope.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/script/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/script/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     5678 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/script/debugger.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4198 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/script/edit_window.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      272 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/script/launcher.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1546 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/script/script.png
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    14081 2022-02-14 07:29:19.000000 msgtools-0.37.9/msgtools/script/script.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/server/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4378 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/BluetoothRFCOMM.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3797 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/BluetoothRFCOMMQt.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    20014 2022-04-15 19:43:49.000000 msgtools-0.37.9/msgtools/server/CanPlugin.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3907 2022-03-26 22:10:59.000000 msgtools-0.37.9/msgtools/server/CanPortDialog.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     8189 2022-09-26 17:19:49.000000 msgtools-0.37.9/msgtools/server/SerialPlugin.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2617 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/SerialportDialog.py
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     4290 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/TcpServer.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2445 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/WebSocketServer.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      272 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/launcher.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2308 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/server/server.png
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)    24348 2022-02-14 07:24:02.000000 msgtools-0.37.9/msgtools/server/server.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2541 2022-03-26 22:12:24.000000 msgtools-0.37.9/msgtools/server/socketcan_commands.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/sim/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2022-10-23 01:41:53.000000 msgtools-0.37.9/msgtools/sim/__init__.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    21027 2022-12-28 00:45:01.000000 msgtools-0.37.9/msgtools/sim/sim.py
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     5644 2023-01-09 21:23:23.000000 msgtools-0.37.9/msgtools/sim/sim_exec.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/webapp/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        0 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/__init__.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.982766 msgtools-0.37.9/msgtools/webapp/lib/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6751 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/Histogram-component.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     2483 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/MsgDialog.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    10730 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/MsgFieldLabel.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     6538 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/MsgPlot.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3397 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/MsgSelector.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3338 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/MsgTabs.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     3520 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/MsgTree.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     9741 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/Plot-component.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    21680 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/WebSocketUtils.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)   151725 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/d3.v3.min.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)    22916 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/lib/msgtools.js
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      693 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/template.html
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     2959 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/template.js
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     8240 2020-06-17 22:29:43.000000 msgtools-0.37.9/msgtools/webapp/webapp.py
+drwxrwxr-x   0 mgazic    (1001) mgazic    (1001)        0 2023-01-13 18:37:01.978767 msgtools-0.37.9/msgtools.egg-info/
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)      843 2023-01-13 18:37:01.000000 msgtools-0.37.9/msgtools.egg-info/PKG-INFO
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     4742 2023-01-13 18:37:01.000000 msgtools-0.37.9/msgtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        1 2023-01-13 18:37:01.000000 msgtools-0.37.9/msgtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)     1989 2023-01-13 18:37:01.000000 msgtools-0.37.9/msgtools.egg-info/entry_points.txt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        1 2020-06-17 22:29:42.000000 msgtools-0.37.9/msgtools.egg-info/not-zip-safe
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)       96 2023-01-13 18:37:01.000000 msgtools-0.37.9/msgtools.egg-info/requires.txt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)        9 2023-01-13 18:37:01.000000 msgtools-0.37.9/msgtools.egg-info/top_level.txt
+-rw-rw-r--   0 mgazic    (1001) mgazic    (1001)       79 2023-01-13 18:37:01.986766 msgtools-0.37.9/setup.cfg
+-rwxrwxr-x   0 mgazic    (1001) mgazic    (1001)     4604 2023-01-13 18:36:57.000000 msgtools-0.37.9/setup.py
```

### Comparing `msgtools-0.37.8/PKG-INFO` & `msgtools-0.37.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgtools
-Version: 0.37.8
+Version: 0.37.9
 Summary: Tools for fixed binary protocols
 Home-page: https://github.com/MilesEngineering/MsgTools/
 Author: Miles Gazic
 Author-email: miles.gazic@gmail.com
 License: LGPLv2
 Project-URL: Documentation, https://github.com/MilesEngineering/MsgTools/wiki
 Project-URL: Source, https://github.com/MilesEngineering/MsgTools/
```

### Comparing `msgtools-0.37.8/README.md` & `msgtools-0.37.9/README.md`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/console/client.py` & `msgtools-0.37.9/msgtools/console/client.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/console/console.py` & `msgtools-0.37.9/msgtools/console/console.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/console/server.py` & `msgtools-0.37.9/msgtools/console/server.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/csvparse/csvparse.py` & `msgtools-0.37.9/msgtools/csvparse/csvparse.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/database/influx.png` & `msgtools-0.37.9/msgtools/database/influx.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/database/influx_msgserver_plugin.py` & `msgtools-0.37.9/msgtools/database/influx_msgserver_plugin.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/database/influxdb.py` & `msgtools-0.37.9/msgtools/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/debug/debug.png` & `msgtools-0.37.9/msgtools/debug/debug.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/debug/debug.py` & `msgtools-0.37.9/msgtools/debug/debug.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/debug/findprints.py` & `msgtools-0.37.9/msgtools/debug/findprints.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/inspector/inspector.png` & `msgtools-0.37.9/msgtools/inspector/inspector.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/inspector/inspector.py` & `msgtools-0.37.9/msgtools/inspector/inspector.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/launcher/codegen_gui.py` & `msgtools-0.37.9/msgtools/launcher/codegen_gui.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/launcher/launcher.png` & `msgtools-0.37.9/msgtools/launcher/launcher.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/launcher/launcher.py` & `msgtools-0.37.9/msgtools/launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/app.py` & `msgtools-0.37.9/msgtools/lib/app.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/conversions.py` & `msgtools-0.37.9/msgtools/lib/conversions.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/createmsgdialog.py` & `msgtools-0.37.9/msgtools/lib/createmsgdialog.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/file_reader.py` & `msgtools-0.37.9/msgtools/lib/file_reader.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/gui.py` & `msgtools-0.37.9/msgtools/lib/gui.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/header_translator.py` & `msgtools-0.37.9/msgtools/lib/header_translator.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/message.py` & `msgtools-0.37.9/msgtools/lib/message.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/messaging.py` & `msgtools-0.37.9/msgtools/lib/messaging.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/msgcsv.py` & `msgtools-0.37.9/msgtools/lib/msgcsv.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/msgjson.py` & `msgtools-0.37.9/msgtools/lib/msgjson.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/msgpandas.py` & `msgtools-0.37.9/msgtools/lib/msgpandas.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/msgplot.py` & `msgtools-0.37.9/msgtools/lib/msgplot.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/txtreewidget.py` & `msgtools-0.37.9/msgtools/lib/txtreewidget.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lib/unknownmsg.py` & `msgtools-0.37.9/msgtools/lib/unknownmsg.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lumberjack/lumberjack.py` & `msgtools-0.37.9/msgtools/lumberjack/lumberjack.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/lumberjack/read_json.py` & `msgtools-0.37.9/msgtools/lumberjack/read_json.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/multilog/multilog.py` & `msgtools-0.37.9/msgtools/multilog/multilog.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/noisemaker/bandwidthtestecho.py` & `msgtools-0.37.9/msgtools/noisemaker/bandwidthtestecho.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/noisemaker/bandwidthtester.py` & `msgtools-0.37.9/msgtools/noisemaker/bandwidthtester.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/noisemaker/noisemaker.png` & `msgtools-0.37.9/msgtools/noisemaker/noisemaker.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/noisemaker/noisemaker.py` & `msgtools-0.37.9/msgtools/noisemaker/noisemaker.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/MsgUtils.py` & `msgtools-0.37.9/msgtools/parser/MsgUtils.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/c/HeaderTemplate.h` & `msgtools-0.37.9/msgtools/parser/c/HeaderTemplate.h`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/c/language.py` & `msgtools-0.37.9/msgtools/parser/c/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/check.py` & `msgtools-0.37.9/msgtools/parser/check.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/cpp/HeaderTemplate.h` & `msgtools-0.37.9/msgtools/parser/cpp/HeaderTemplate.h`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/cpp/Template.h` & `msgtools-0.37.9/msgtools/parser/cpp/Template.h`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/cpp/language.py` & `msgtools-0.37.9/msgtools/parser/cpp/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/dart/HeaderTemplate.dart` & `msgtools-0.37.9/msgtools/parser/dart/HeaderTemplate.dart`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/dart/Template.dart` & `msgtools-0.37.9/msgtools/parser/dart/Template.dart`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/dart/language.py` & `msgtools-0.37.9/msgtools/parser/dart/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/html/HeaderTemplate.html` & `msgtools-0.37.9/msgtools/parser/html/HeaderTemplate.html`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/html/Template.html` & `msgtools-0.37.9/msgtools/parser/html/Template.html`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/html/bootstrap.min.css` & `msgtools-0.37.9/msgtools/parser/html/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/html/language.py` & `msgtools-0.37.9/msgtools/parser/html/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/java/HeaderTemplate.java` & `msgtools-0.37.9/msgtools/parser/java/HeaderTemplate.java`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/java/Template.java` & `msgtools-0.37.9/msgtools/parser/java/Template.java`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/java/language.py` & `msgtools-0.37.9/msgtools/parser/java/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/javascript/HeaderTemplate.js` & `msgtools-0.37.9/msgtools/parser/javascript/HeaderTemplate.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/javascript/Template.js` & `msgtools-0.37.9/msgtools/parser/javascript/Template.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/javascript/language.py` & `msgtools-0.37.9/msgtools/parser/javascript/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,18 @@
 def initField(field):
     if "Default" in field:
         if MsgParser.fieldCount(field) > 1:
             ret = "for (i=0; i<" + str(MsgParser.fieldCount(field)) + "; i++)\n"
             ret += "    this.Set" + field["Name"] + "(" + str(field["Default"]) + ", i);" 
             return ret;
         else:
-            return  "this.Set" + field["Name"] + "(" + str(field["Default"]) + ");"
+            if MsgParser.fieldCount(field) > 1:
+                ret = "for (i=0; i<" + str(MsgParser.fieldCount(field)) + "; i++)\n"
+                ret += "    this.Set" + field["Name"] + "(" + str(field["Default"]) + ", i);"
+            return ret;
     return ""
 
 def initBitfield(field, bits):
     if "Default" in bits:
         return  "this.Set" + MsgParser.BitfieldName(field, bits) + "(" +str(bits["Default"]) + ");"
     return ""
```

### Comparing `msgtools-0.37.8/msgtools/parser/kotlin/HeaderTemplate.kt` & `msgtools-0.37.9/msgtools/parser/kotlin/HeaderTemplate.kt`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/kotlin/Template.kt` & `msgtools-0.37.9/msgtools/parser/kotlin/Template.kt`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/kotlin/language.py` & `msgtools-0.37.9/msgtools/parser/kotlin/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/matlab/HeaderTemplate.m` & `msgtools-0.37.9/msgtools/parser/matlab/HeaderTemplate.m`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/matlab/Template.m` & `msgtools-0.37.9/msgtools/parser/matlab/Template.m`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/matlab/language.py` & `msgtools-0.37.9/msgtools/parser/matlab/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/parser.py` & `msgtools-0.37.9/msgtools/parser/parser.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/python/HeaderTemplate.py` & `msgtools-0.37.9/msgtools/parser/python/HeaderTemplate.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/python/Template.py` & `msgtools-0.37.9/msgtools/parser/python/Template.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/python/language.py` & `msgtools-0.37.9/msgtools/parser/python/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/simulink/Template.m` & `msgtools-0.37.9/msgtools/parser/simulink/Template.m`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/simulink/language.py` & `msgtools-0.37.9/msgtools/parser/simulink/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/swift/HeaderTemplate.swift` & `msgtools-0.37.9/msgtools/parser/swift/HeaderTemplate.swift`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/swift/Template.swift` & `msgtools-0.37.9/msgtools/parser/swift/Template.swift`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/parser/swift/language.py` & `msgtools-0.37.9/msgtools/parser/swift/language.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/scope/scope.png` & `msgtools-0.37.9/msgtools/scope/scope.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/scope/scope.py` & `msgtools-0.37.9/msgtools/scope/scope.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/script/debugger.py` & `msgtools-0.37.9/msgtools/script/debugger.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/script/edit_window.py` & `msgtools-0.37.9/msgtools/script/edit_window.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/script/script.png` & `msgtools-0.37.9/msgtools/script/script.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/script/script.py` & `msgtools-0.37.9/msgtools/script/script.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/BluetoothRFCOMM.py` & `msgtools-0.37.9/msgtools/server/BluetoothRFCOMM.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/BluetoothRFCOMMQt.py` & `msgtools-0.37.9/msgtools/server/BluetoothRFCOMMQt.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/CanPlugin.py` & `msgtools-0.37.9/msgtools/server/CanPlugin.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/CanPortDialog.py` & `msgtools-0.37.9/msgtools/server/CanPortDialog.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/SerialPlugin.py` & `msgtools-0.37.9/msgtools/server/SerialPlugin.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/SerialportDialog.py` & `msgtools-0.37.9/msgtools/server/SerialportDialog.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/TcpServer.py` & `msgtools-0.37.9/msgtools/server/TcpServer.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/WebSocketServer.py` & `msgtools-0.37.9/msgtools/server/WebSocketServer.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/server.png` & `msgtools-0.37.9/msgtools/server/server.png`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/server.py` & `msgtools-0.37.9/msgtools/server/server.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/server/socketcan_commands.py` & `msgtools-0.37.9/msgtools/server/socketcan_commands.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/sim/sim.py` & `msgtools-0.37.9/msgtools/sim/sim.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/sim/sim_exec.py` & `msgtools-0.37.9/msgtools/sim/sim_exec.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/Histogram-component.js` & `msgtools-0.37.9/msgtools/webapp/lib/Histogram-component.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/MsgDialog.js` & `msgtools-0.37.9/msgtools/webapp/lib/MsgDialog.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/MsgFieldLabel.js` & `msgtools-0.37.9/msgtools/webapp/lib/MsgFieldLabel.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/MsgPlot.js` & `msgtools-0.37.9/msgtools/webapp/lib/MsgPlot.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/MsgSelector.js` & `msgtools-0.37.9/msgtools/webapp/lib/MsgSelector.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/MsgTabs.js` & `msgtools-0.37.9/msgtools/webapp/lib/MsgTabs.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/MsgTree.js` & `msgtools-0.37.9/msgtools/webapp/lib/MsgTree.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/Plot-component.js` & `msgtools-0.37.9/msgtools/webapp/lib/Plot-component.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/WebSocketUtils.js` & `msgtools-0.37.9/msgtools/webapp/lib/WebSocketUtils.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/d3.v3.min.js` & `msgtools-0.37.9/msgtools/webapp/lib/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/lib/msgtools.js` & `msgtools-0.37.9/msgtools/webapp/lib/msgtools.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/template.html` & `msgtools-0.37.9/msgtools/webapp/template.html`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/template.js` & `msgtools-0.37.9/msgtools/webapp/template.js`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools/webapp/webapp.py` & `msgtools-0.37.9/msgtools/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools.egg-info/PKG-INFO` & `msgtools-0.37.9/msgtools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgtools
-Version: 0.37.8
+Version: 0.37.9
 Summary: Tools for fixed binary protocols
 Home-page: https://github.com/MilesEngineering/MsgTools/
 Author: Miles Gazic
 Author-email: miles.gazic@gmail.com
 License: LGPLv2
 Project-URL: Documentation, https://github.com/MilesEngineering/MsgTools/wiki
 Project-URL: Source, https://github.com/MilesEngineering/MsgTools/
```

### Comparing `msgtools-0.37.8/msgtools.egg-info/SOURCES.txt` & `msgtools-0.37.9/msgtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/msgtools.egg-info/entry_points.txt` & `msgtools-0.37.9/msgtools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `msgtools-0.37.8/setup.py` & `msgtools-0.37.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(name='msgtools',
     python_requires='>=3.5',
-    version='0.37.8',
+    version='0.37.9',
     description='Tools for fixed binary protocols',
     url='https://github.com/MilesEngineering/MsgTools/',
     author='Miles Gazic',
     author_email='miles.gazic@gmail.com',
     license='LGPLv2',
     packages=find_packages(),
     zip_safe=False,
```

