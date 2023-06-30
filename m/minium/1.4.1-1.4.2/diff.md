# Comparing `tmp/minium-1.4.1.tar.gz` & `tmp/minium-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minium-1.4.1.tar", last modified: Tue May  9 06:44:43 2023, max compression
+gzip compressed data, was "dist/minium-1.4.2.tar", last modified: Fri Jun 30 02:36:03 2023, max compression
```

## Comparing `minium-1.4.1.tar` & `minium-1.4.2.tar`

### file list

```diff
@@ -1,279 +1,281 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.526981 minium-1.4.1/
--rw-r--r--   0 root         (0) root         (0)      697 2023-05-09 06:44:43.526981 minium-1.4.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.482981 minium-1.4.1/minium/
--rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.1/minium/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18583 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/assertbase.py
--rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.1/minium/framework/casedump.py
--rw-r--r--   0 root         (0) root         (0)     7702 2022-11-07 03:36:55.000000 minium-1.4.1/minium/framework/caseinspect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/css/
--rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/css/app.87891bf0.css
--rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/css/chunk-vendors.52eeca6f.css
--rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/dist/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/dist/fonts/element-icons.535877f5.woff
--rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/dist/fonts/element-icons.732389de.ttf
--rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.490981 minium-1.4.1/minium/framework/dist/js/
--rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/js/app.544bedf4.js
--rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/dist/js/chunk-vendors.22ed339a.js
--rw-r--r--   0 root         (0) root         (0)     3463 2023-01-16 03:26:29.000000 minium-1.4.1/minium/framework/errorReport.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-09 06:36:06.000000 minium-1.4.1/minium/framework/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/libs/tgit/
--rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/tgit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/tgit/auth.py
--rw-r--r--   0 root         (0) root         (0)    97301 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/libs/tgit/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/libs/unittest/
--rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.1/minium/framework/libs/unittest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11757 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/libs/unittest/case.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/libs/unittest/suite.py
--rw-r--r--   0 root         (0) root         (0)    19830 2022-12-19 02:27:07.000000 minium-1.4.1/minium/framework/loader.py
--rw-r--r--   0 root         (0) root         (0)    10166 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/logcolor.py
--rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/miniconfig.py
--rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/miniddt.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.1/minium/framework/minidoctor.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/minilimit.py
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/miniprogram.py
--rw-r--r--   0 root         (0) root         (0)     6669 2022-09-14 13:08:12.000000 minium-1.4.1/minium/framework/miniresult.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/minisuite.py
--rw-r--r--   0 root         (0) root         (0)    29430 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/minitest.py
--rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.1/minium/framework/report.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.4.1/minium/framework/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/framework/tools/
--rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.1/minium/framework/tools/report_issue.py
--rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.1/minium/framework/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.494981 minium-1.4.1/minium/miniprogram/
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/miniprogram/base_driver/
--rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/base_driver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47565 2023-05-09 06:36:06.000000 minium-1.4.1/minium/miniprogram/base_driver/app.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/callback.py
--rw-r--r--   0 root         (0) root         (0)    28828 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/connection.py
--rw-r--r--   0 root         (0) root         (0)    46414 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/element.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.1/minium/miniprogram/base_driver/minium.py
--rw-r--r--   0 root         (0) root         (0)     5475 2023-05-09 06:36:06.000000 minium-1.4.1/minium/miniprogram/base_driver/minium_log.py
--rw-r--r--   0 root         (0) root         (0)     8485 2023-04-27 02:49:44.000000 minium-1.4.1/minium/miniprogram/base_driver/minium_object.py
--rw-r--r--   0 root         (0) root         (0)    23560 2023-04-27 02:49:44.000000 minium-1.4.1/minium/miniprogram/base_driver/page.py
--rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/base_driver/prefixer.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-09 06:44:40.000000 minium-1.4.1/minium/miniprogram/base_driver/version.json
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.1/minium/miniprogram/base_driver/version.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/base_driver/waiter.py
--rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.1/minium/miniprogram/qq_minium.py
--rw-r--r--   0 root         (0) root         (0)    38940 2023-05-09 06:36:06.000000 minium-1.4.1/minium/miniprogram/wx_minium.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/native/
--rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.1/minium/native/__init__.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/native/lib/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.498981 minium-1.4.1/minium/native/lib/android_base/
--rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/android_base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.502981 minium-1.4.1/minium/native/lib/at/
--rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/at/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/apkapi.py
--rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/atproxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/bin/
--rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/bin/AtServer.apk
--rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/bin/AtStub.jar
--rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/command_line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/core/
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/accesshelper.py
--rw-r--r--   0 root         (0) root         (0)    46986 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/at/core/adbwrap.py
--rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/basedriver.py
--rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/case_repair_adapter.py
--rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/config.py
--rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/element.py
--rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/javadriver.py
--rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/resguard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/core/stf/
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/stf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/stf/mincap.py
--rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/stf/minitouch.py
--rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/uidevice.py
--rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/uixml.py
--rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/core/websocketcli.py
--rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/eventmonitor.py
--rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/hook.py
--rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/jlogcat.py
--rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/keycode.py
--rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/perfcollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.506981 minium-1.4.1/minium/native/lib/at/tests/
--rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/AtEvent.py
--rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/AtSocket.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/adbtest.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/airtesttest.py
--rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/atdevicetest.py
--rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/attestbase.py
--rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/drivertest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/elementtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.510981 minium-1.4.1/minium/native/lib/at/tests/images/
--rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/images/1.jpg
--rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/images/2.jpg
--rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/images/image.jpg
--rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/javadrivertest.py
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/minicap_test.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/minitest.py
--rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/minitouch_test.py
--rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/u2test.py
--rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/uixmltest.py
--rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/vs_test.py
--rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/tests/webdrivertest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.510981 minium-1.4.1/minium/native/lib/at/utils/
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/apkinfo.py
--rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/axmlparser.py
--rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/axmlparser3.py
--rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/commonhelper.py
--rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/magic.py
--rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/nbsp.py
--rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/utils/threadhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.510981 minium-1.4.1/minium/native/lib/at/vision/
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/vision/template_match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/at/webdriver/
--rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/driver.py
--rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/error.py
--rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/jsapi.py
--rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/miniapp.py
--rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/stub.js
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/tabdescription.py
--rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/tabwebsocket.py
--rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/webelement.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/webhelper.py
--rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/webdriver/wspools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/at/wechat/
--rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wechat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wechat/activtiy.py
--rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wechat/appvars.py
--rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/at/wsimp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/case_repair_sdk/
--rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/case_repair_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/case_repair_sdk/default_trace.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.1/minium/native/lib/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/wda/
--rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wda/screenhelper.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wda/xcui_element_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/lib/wx_wda/
--rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wx_wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wx_wda/wdaUI.py
--rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/lib/wx_wda/webDriverTool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/qq_native/
--rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/qandroidnative.py
--rw-r--r--   0 root         (0) root         (0)      804 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/qbasenative.py
--rwxr-xr-x   0 root         (0) root         (0)    16882 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/qq_native/qiosnative.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.514981 minium-1.4.1/minium/native/wx_native/
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.1/minium/native/wx_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39339 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/androidnative.py
--rw-r--r--   0 root         (0) root         (0)    23791 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/basenative.py
--rw-r--r--   0 root         (0) root         (0)     8053 2023-02-07 11:55:46.000000 minium-1.4.1/minium/native/wx_native/idenative.py
--rw-r--r--   0 root         (0) root         (0)    36096 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/iosnative.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.1/minium/native/wx_native/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.518981 minium-1.4.1/minium/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.1/minium/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.1/minium/utils/emitter.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.1/minium/utils/eventloop.py
--rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.1/minium/utils/injectjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.482981 minium-1.4.1/minium/utils/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.522981 minium-1.4.1/minium/utils/js/es5/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      255 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)       72 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      535 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/createContext.js
--rw-r--r--   0 root         (0) root         (0)      340 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)      617 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/getUni.js
--rw-r--r--   0 root         (0) root         (0)    38266 2023-05-09 06:44:27.000000 minium-1.4.1/minium/utils/js/es5/helpers.js
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      487 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      216 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      459 2023-05-09 06:44:25.000000 minium-1.4.1/minium/utils/js/es5/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1480 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)     5247 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)     1582 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     2837 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      726 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/mockRequestStack.js
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1171 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/requestStack.js
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)     7138 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/testAsync.js
--rw-r--r--   0 root         (0) root         (0)      307 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/uuid.js
--rw-r--r--   0 root         (0) root         (0)      181 2023-05-09 06:44:26.000000 minium-1.4.1/minium/utils/js/es5/waitUtil.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.526981 minium-1.4.1/minium/utils/js/min/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-09 06:44:39.000000 minium-1.4.1/minium/utils/js/min/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-09 06:44:37.000000 minium-1.4.1/minium/utils/js/min/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 06:44:33.000000 minium-1.4.1/minium/utils/js/min/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/createContext.js
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-09 06:44:39.000000 minium-1.4.1/minium/utils/js/min/getUni.js
--rw-r--r--   0 root         (0) root         (0)    38266 2023-05-09 06:44:38.000000 minium-1.4.1/minium/utils/js/min/helpers.js
--rw-r--r--   0 root         (0) root         (0)      270 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-09 06:44:30.000000 minium-1.4.1/minium/utils/js/min/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-09 06:44:29.000000 minium-1.4.1/minium/utils/js/min/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-09 06:44:37.000000 minium-1.4.1/minium/utils/js/min/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-09 06:44:28.000000 minium-1.4.1/minium/utils/js/min/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1118 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1202 2023-05-09 06:44:34.000000 minium-1.4.1/minium/utils/js/min/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-09 06:44:37.000000 minium-1.4.1/minium/utils/js/min/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-09 06:44:29.000000 minium-1.4.1/minium/utils/js/min/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 06:44:30.000000 minium-1.4.1/minium/utils/js/min/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-09 06:44:28.000000 minium-1.4.1/minium/utils/js/min/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-09 06:44:31.000000 minium-1.4.1/minium/utils/js/min/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)     4368 2023-05-09 06:44:29.000000 minium-1.4.1/minium/utils/js/min/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-09 06:44:35.000000 minium-1.4.1/minium/utils/js/min/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     2327 2023-05-09 06:44:30.000000 minium-1.4.1/minium/utils/js/min/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-09 06:44:36.000000 minium-1.4.1/minium/utils/js/min/mockRequestStack.js
--rw-r--r--   0 root         (0) root         (0)     1192 2023-05-09 06:44:28.000000 minium-1.4.1/minium/utils/js/min/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-09 06:44:32.000000 minium-1.4.1/minium/utils/js/min/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1018 2023-05-09 06:44:33.000000 minium-1.4.1/minium/utils/js/min/requestStack.js
--rw-r--r--   0 root         (0) root         (0)      284 2023-05-09 06:44:35.000000 minium-1.4.1/minium/utils/js/min/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      199 2023-05-09 06:44:33.000000 minium-1.4.1/minium/utils/js/min/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-09 06:44:39.000000 minium-1.4.1/minium/utils/js/min/testAsync.js
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-09 06:44:38.000000 minium-1.4.1/minium/utils/js/min/uuid.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-09 06:44:35.000000 minium-1.4.1/minium/utils/js/min/waitUtil.js
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.1/minium/utils/meta.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.1/minium/utils/platforms.py
--rw-r--r--   0 root         (0) root         (0)    15512 2023-05-09 06:36:06.000000 minium-1.4.1/minium/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:44:43.486981 minium-1.4.1/minium.egg-info/
--rw-r--r--   0 root         (0) root         (0)      697 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9118 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-09 06:44:43.000000 minium-1.4.1/minium.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 06:44:43.526981 minium-1.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2435 2023-05-09 06:36:06.000000 minium-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.707526 minium-1.4.2/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-30 02:36:03.707526 minium-1.4.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.659526 minium-1.4.2/minium/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.2/minium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-06-28 02:27:06.000000 minium-1.4.2/minium/framework/assertbase.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.2/minium/framework/casedump.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/caseinspect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/css/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/css/app.87891bf0.css
+-rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/css/chunk-vendors.52eeca6f.css
+-rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/dist/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/dist/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/dist/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/js/app.544bedf4.js
+-rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/js/chunk-vendors.22ed339a.js
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/errorReport.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.671526 minium-1.4.2/minium/framework/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.671526 minium-1.4.2/minium/framework/libs/tgit/
+-rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/libs/tgit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/libs/tgit/auth.py
+-rw-r--r--   0 root         (0) root         (0)    97167 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/libs/tgit/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.675526 minium-1.4.2/minium/framework/libs/unittest/
+-rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.2/minium/framework/libs/unittest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22297 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/libs/unittest/case.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/libs/unittest/suite.py
+-rw-r--r--   0 root         (0) root         (0)    20015 2023-06-29 15:00:02.000000 minium-1.4.2/minium/framework/loader.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/logcolor.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.2/minium/framework/miniconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/miniddt.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.2/minium/framework/minidoctor.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/minilimit.py
+-rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/miniprogram.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/miniresult.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/minisuite.py
+-rw-r--r--   0 root         (0) root         (0)    29964 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/minitest.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.2/minium/framework/report.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.4.2/minium/framework/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.675526 minium-1.4.2/minium/framework/tools/
+-rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/tools/report_issue.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.2/minium/framework/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.675526 minium-1.4.2/minium/miniprogram/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.2/minium/miniprogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.679526 minium-1.4.2/minium/miniprogram/base_driver/
+-rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/base_driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49814 2023-06-28 06:28:59.000000 minium-1.4.2/minium/miniprogram/base_driver/app.py
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/callback.py
+-rw-r--r--   0 root         (0) root         (0)    29048 2023-06-29 15:00:02.000000 minium-1.4.2/minium/miniprogram/base_driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)    46351 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/element.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.2/minium/miniprogram/base_driver/minium.py
+-rw-r--r--   0 root         (0) root         (0)     5959 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/minium_log.py
+-rw-r--r--   0 root         (0) root         (0)     8998 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/minium_object.py
+-rw-r--r--   0 root         (0) root         (0)    23516 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/page.py
+-rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/base_driver/prefixer.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-30 02:36:01.000000 minium-1.4.2/minium/miniprogram/base_driver/version.json
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.2/minium/miniprogram/base_driver/version.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/base_driver/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/qq_minium.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/wx_minium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.679526 minium-1.4.2/minium/native/
+-rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.2/minium/native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.679526 minium-1.4.2/minium/native/lib/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.683526 minium-1.4.2/minium/native/lib/android_base/
+-rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/android_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.683526 minium-1.4.2/minium/native/lib/at/
+-rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.2/minium/native/lib/at/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/apkapi.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/atproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.687526 minium-1.4.2/minium/native/lib/at/bin/
+-rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/bin/AtServer.apk
+-rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/bin/AtStub.jar
+-rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/command_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.691526 minium-1.4.2/minium/native/lib/at/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/accesshelper.py
+-rw-r--r--   0 root         (0) root         (0)    47016 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/lib/at/core/adbwrap.py
+-rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/basedriver.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/case_repair_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/element.py
+-rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/javadriver.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/resguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.695526 minium-1.4.2/minium/native/lib/at/core/stf/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/stf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/stf/mincap.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/stf/minitouch.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/uidevice.py
+-rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/uixml.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/websocketcli.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/eventmonitor.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/hook.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/jlogcat.py
+-rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/keycode.py
+-rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/perfcollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.695526 minium-1.4.2/minium/native/lib/at/tests/
+-rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/AtEvent.py
+-rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/AtSocket.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/adbtest.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/airtesttest.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/atdevicetest.py
+-rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/attestbase.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/drivertest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/elementtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/tests/images/
+-rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/images/1.jpg
+-rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/images/2.jpg
+-rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/images/image.jpg
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/javadrivertest.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/minicap_test.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/minitest.py
+-rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/minitouch_test.py
+-rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/u2test.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/uixmltest.py
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/vs_test.py
+-rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/webdrivertest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/utils/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/apkinfo.py
+-rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/axmlparser.py
+-rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/axmlparser3.py
+-rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/commonhelper.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/magic.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/nbsp.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/threadhelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/vision/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/vision/template_match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/webdriver/
+-rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/driver.py
+-rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/error.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/jsapi.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/miniapp.py
+-rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/stub.js
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/tabdescription.py
+-rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/tabwebsocket.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/webelement.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/webhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/wspools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/wechat/
+-rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wechat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wechat/activtiy.py
+-rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wechat/appvars.py
+-rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wsimp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/case_repair_sdk/
+-rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.2/minium/native/lib/case_repair_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/case_repair_sdk/default_trace.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.2/minium/native/lib/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/wda/
+-rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wda/screenhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wda/xcui_element_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/wx_wda/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wx_wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wx_wda/wdaUI.py
+-rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wx_wda/webDriverTool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/qq_native/
+-rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/qq_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/qq_native/qandroidnative.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/qq_native/qbasenative.py
+-rwxr-xr-x   0 root         (0) root         (0)    16848 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/qq_native/qiosnative.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/wx_native/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/wx_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39266 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/androidnative.py
+-rw-r--r--   0 root         (0) root         (0)    23752 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/basenative.py
+-rw-r--r--   0 root         (0) root         (0)     8051 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/idenative.py
+-rw-r--r--   0 root         (0) root         (0)    34980 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/iosnative.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.2/minium/native/wx_native/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.703525 minium-1.4.2/minium/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.2/minium/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.2/minium/utils/emitter.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.2/minium/utils/eventloop.py
+-rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.2/minium/utils/injectjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.659526 minium-1.4.2/minium/utils/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.703525 minium-1.4.2/minium/utils/js/es5/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      255 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/checkEnv.js
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      535 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      340 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      617 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-06-30 02:35:48.000000 minium-1.4.2/minium/utils/js/es5/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      487 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      459 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-06-30 02:35:47.000000 minium-1.4.2/minium/utils/js/es5/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-30 02:35:47.000000 minium-1.4.2/minium/utils/js/es5/uuid.js
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-30 02:35:47.000000 minium-1.4.2/minium/utils/js/es5/waitUtil.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.707526 minium-1.4.2/minium/utils/js/min/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-30 02:36:00.000000 minium-1.4.2/minium/utils/js/min/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-30 02:35:57.000000 minium-1.4.2/minium/utils/js/min/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-30 02:35:58.000000 minium-1.4.2/minium/utils/js/min/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-30 02:35:50.000000 minium-1.4.2/minium/utils/js/min/checkEnv.js
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-30 02:35:52.000000 minium-1.4.2/minium/utils/js/min/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      191 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-30 02:35:52.000000 minium-1.4.2/minium/utils/js/min/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-30 02:35:54.000000 minium-1.4.2/minium/utils/js/min/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-30 02:35:57.000000 minium-1.4.2/minium/utils/js/min/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-30 02:35:55.000000 minium-1.4.2/minium/utils/js/min/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      555 2023-06-30 02:36:00.000000 minium-1.4.2/minium/utils/js/min/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-06-30 02:35:59.000000 minium-1.4.2/minium/utils/js/min/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-30 02:35:55.000000 minium-1.4.2/minium/utils/js/min/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      684 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-30 02:35:50.000000 minium-1.4.2/minium/utils/js/min/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-30 02:35:49.000000 minium-1.4.2/minium/utils/js/min/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-30 02:35:58.000000 minium-1.4.2/minium/utils/js/min/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-30 02:35:49.000000 minium-1.4.2/minium/utils/js/min/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-06-30 02:35:55.000000 minium-1.4.2/minium/utils/js/min/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-30 02:35:58.000000 minium-1.4.2/minium/utils/js/min/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-30 02:35:49.000000 minium-1.4.2/minium/utils/js/min/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-30 02:35:48.000000 minium-1.4.2/minium/utils/js/min/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-30 02:35:52.000000 minium-1.4.2/minium/utils/js/min/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-06-30 02:35:50.000000 minium-1.4.2/minium/utils/js/min/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      664 2023-06-30 02:35:57.000000 minium-1.4.2/minium/utils/js/min/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-06-30 02:35:48.000000 minium-1.4.2/minium/utils/js/min/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-30 02:35:54.000000 minium-1.4.2/minium/utils/js/min/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-30 02:35:54.000000 minium-1.4.2/minium/utils/js/min/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-30 02:36:00.000000 minium-1.4.2/minium/utils/js/min/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-30 02:35:59.000000 minium-1.4.2/minium/utils/js/min/uuid.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/waitUtil.js
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.2/minium/utils/meta.py
+-rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.2/minium/utils/platforms.py
+-rw-r--r--   0 root         (0) root         (0)    15710 2023-06-21 12:00:44.000000 minium-1.4.2/minium/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.659526 minium-1.4.2/minium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 02:36:03.707526 minium-1.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-23 08:31:11.000000 minium-1.4.2/setup.py
```

### Comparing `minium-1.4.1/PKG-INFO` & `minium-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minium
-Version: 1.4.1
+Version: 1.4.2
 Summary: Minium is the best MiniProgram auto test framework.
 Home-page: https://minitest.weixin.qq.com/#/
 Author: WeChat-Test
 Author-email: minitest@tencent.com
 License: MIT
 Description: 
         install:
```

### Comparing `minium-1.4.1/minium/__init__.py` & `minium-1.4.2/minium/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/assertbase.py` & `minium-1.4.2/minium/framework/assertbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import time
 from functools import wraps
 from .logcolor import *
 import logging.handlers
 import traceback
 import datetime
 import re
-from minium.miniprogram.wx_minium import WXMinium
 from .miniconfig import MiniConfig, get_log_level
 from minium.framework.libs import unittest
 
 logger = logging.getLogger("minium")
 logger.propagate = False
 WORKSPACE_DIR = os.path.abspath(os.getcwd())
 # print("当前工作路径: %s" % WORKSPACE_DIR)
@@ -128,15 +127,15 @@
     def setUpConfig(cls, default=False):
         if cls.CONFIG is None:
             default_config_filename = os.path.join(WORKSPACE_DIR, "config.json")
             if os.path.exists(default_config_filename) and not default:
                 logger.info("read config from workspace dir: [%s]" % WORKSPACE_DIR)
                 cls.CONFIG = MiniConfig.from_file(default_config_filename)
             else:
-                logger.warning("loading default config")
+                logger.warning(f"can't find config.json in {WORKSPACE_DIR}, loading default config")
                 cls.CONFIG = MiniConfig()
         if cls.CONFIG.outputs is None:
             outputs = os.path.join(os.getcwd(), "outputs")
             if not os.path.exists(outputs):
                 os.makedirs(outputs)
             cls.CONFIG.outputs = outputs
         if cls.CONFIG.create_time is None:
```

### Comparing `minium-1.4.1/minium/framework/casedump.py` & `minium-1.4.2/minium/framework/casedump.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/caseinspect.py` & `minium-1.4.2/minium/framework/caseinspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         if min_space_count < space_count:
             min_space_count = space_count
         if len(line) < min_space_count:
             min_space_count = len(line)
     new_lines = [line[min_space_count:] for line in old_lines]
     try:
         return "\n".join(new_lines).strip()
-    except:
+    except TypeError:
         return doc_str
 
 
 def get_test_methods(test_case_class):
     s = []
     for name, value in inspect.getmembers(test_case_class):
         if name.startswith("test"):
@@ -160,15 +160,15 @@
             module_path = os.path.join(root, filename)
             module_path = os.path.relpath(
                 os.path.abspath(module_path), os.path.abspath(path)
             )
             module_name = ".".join(
                 module_path.replace(os.path.sep, ".").split(".")[:-1]
             )
-            has_hit_names = set()
+            # has_hit_names = set()
             mod = get_mod(module_name)
             if not mod or isinstance(mod, ModuleNotFoundError):
                 if mini_suite:
                     mini_suite.set_pkg_fail(module_name, mod)
                 continue
 
             human_name = getattr(mod, "NAME", None)
```

### Comparing `minium-1.4.1/minium/framework/dist/css/chunk-vendors.52eeca6f.css` & `minium-1.4.2/minium/framework/dist/css/chunk-vendors.52eeca6f.css`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/dist/favicon.ico` & `minium-1.4.2/minium/framework/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/dist/fonts/element-icons.535877f5.woff` & `minium-1.4.2/minium/framework/dist/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/dist/fonts/element-icons.732389de.ttf` & `minium-1.4.2/minium/framework/dist/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/dist/index.html` & `minium-1.4.2/minium/framework/dist/index.html`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/dist/js/app.544bedf4.js` & `minium-1.4.2/minium/framework/dist/js/app.544bedf4.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/dist/js/chunk-vendors.22ed339a.js` & `minium-1.4.2/minium/framework/dist/js/chunk-vendors.22ed339a.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/errorReport.py` & `minium-1.4.2/minium/framework/errorReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import sys
 
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), "libs"))
 sys.path.append(os.path.join(os.path.dirname(__file__)))
 import json
 import argparse
 import tools.report_issue
-import requests
 
 work_root = os.path.abspath(".")
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-k",
```

### Comparing `minium-1.4.1/minium/framework/exception.py` & `minium-1.4.2/minium/framework/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,15 +78,25 @@
     ...
 
 
 class MiniAppError(MiniError):
     ...
 
 
-class MiniLowVersionSdkError(MiniAppError):
+class MiniCommandError(MiniAppError):
+    def __init__(self, msg, msg_id=None):
+        self.msg_id = msg_id
+        super().__init__(msg)
+
+
+class PageDestroyed(MiniCommandError):
+    ...
+
+
+class MiniLowVersionSdkError(MiniCommandError):
     ...
 
 
 class MiniObserverError(MiniError):
     ...
 
 
@@ -108,9 +118,17 @@
             err = args[0]
             super().__init__(err.msg, *args[1:], name=err.name, path=err.path)
             self.with_traceback(err.__traceback__)
         else:
             super().__init__(*args, name=name, path=path)
 
 
-class RemoteDebugConnectionLost(MiniAppError):  # 远程调试服务掉线
+class RemoteDebugConnectionLost(MiniCommandError):  # 远程调试服务掉线
+    ...
+
+
+class RetrySuccess(MiniError):  # 重试成功
+    ...
+
+
+class RetryFail(MiniError):  # 重试失败
     ...
```

### Comparing `minium-1.4.1/minium/framework/libs/tgit/auth.py` & `minium-1.4.2/minium/framework/libs/tgit/auth.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/libs/tgit/client.py` & `minium-1.4.2/minium/framework/libs/tgit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,22 +269,14 @@
         """
 
         作为管理者
 
         """
         return self.get("/users", **kwargs)
 
-    def list_users(self, **kwargs):
-        """
-
-        作为普通用户
-
-        """
-        return self.get("/users", **kwargs)
-
     def get_user_watched(self, **kwargs):
         """
 
         获用户关注项目列表
 
         """
         return self.get("/user/watched", **kwargs)
```

### Comparing `minium-1.4.1/minium/framework/libs/unittest/case.py` & `minium-1.4.2/minium/framework/libs/unittest/case.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,248 +6,471 @@
     addModuleCleanup,
     FunctionTestCase,
     SkipTest,
     skip,
     skipIf as skipIfSrc,
     skipUnless,
     expectedFailure,
-)
+) # noqa: F401
 from unittest.case import TestCase as TestCaseSrc
-from unittest.case import _Outcome, _ShouldStop, warnings, safe_repr, _OrderedChainMap, _subtest_msg_sentinel
+
+
+
+# 重写testcase
 
 # unittest跟随python版本更新, 新版本unittest存在新的实现, 需要定义最新兼容python版本来防止出现兼容性问题, 并给用户报出来
-NEWEST_PYTHON_VERSION = (3, 10, 5)
-NEWEST_PYTHON_VERSION_STR = ".".join([str(s) for s in NEWEST_PYTHON_VERSION])
 
-class Outcome(_Outcome):
-    def __init__(self, result=None):
-        super().__init__(result)
-        # 兼容3.11
-        self.skipped = []
-        self.errors = []
-        self.current_stage = None
-        self.error_stages = []  # 失败发生在的步骤：_miniClassSetUp, _miniSetUp, _miniTearDown, setUpClass, tearDownClass, setUp, tearDown, testMethod
-        self.stage_errors = {}  # 发生在每个stage的具体error
-
-    @contextlib.contextmanager
-    def testPartExecutor(self, test_case, isTest=False, error_stage=None):
-        """
-        rewrite for error_stages
-        :error_stage: current error stage name
-        """
-        old_success = self.success
-        self.success = True
-        self.current_stage = error_stage or self.current_stage
-        try:
-            yield
-        except KeyboardInterrupt:
-            raise
-        except SkipTest as e:
-            self.success = False
-            self.skipped.append((test_case, str(e)))
-        except _ShouldStop:
+if sys.version_info >= (3, 11):
+    NEWEST_PYTHON_VERSION = (3, 11, 3)
+    NEWEST_PYTHON_VERSION_STR = ".".join([str(s) for s in NEWEST_PYTHON_VERSION])
+    from unittest.case import _Outcome, _ShouldStop, _addSkip, _addError, _subtest_msg_sentinel, _OrderedChainMap, _SubTest
+    from unittest.case import warnings, safe_repr
+    class Outcome(_Outcome):
+        def __init__(self, result=None):
+            super().__init__(result)
+            self.skipped = []
+            self.errors = []
+            self.current_stage = None
+            self.error_stages = []  # 失败发生在的步骤：_miniClassSetUp, _miniSetUp, _miniTearDown, setUpClass, tearDownClass, setUp, tearDown, testMethod
+            self.stage_errors = {}  # 发生在每个stage的具体error
+
+        @contextlib.contextmanager
+        def testPartExecutor(self, test_case, subTest=False, error_stage=None):
+            old_success = self.success
+            self.success = True
+            self.current_stage = error_stage or self.current_stage
+            try:
+                yield
+            except KeyboardInterrupt:
+                raise
+            except SkipTest as e:
+                self.success = False
+                self.skipped.append((test_case, str(e)))
+                _addSkip(self.result, test_case, str(e))
+            except _ShouldStop:
+                pass
+            except:
+                exc_info = sys.exc_info()
+                if self.expecting_failure:
+                    self.expectedFailure = exc_info
+                else:
+                    self.success = False
+                    self.errors.append((test_case, exc_info))
+                    if self.current_stage and self.current_stage in self.stage_errors:
+                        self.stage_errors[self.current_stage].append(exc_info)
+                    elif self.current_stage:
+                        self.stage_errors[self.current_stage] = [exc_info,]
+                        self.error_stages.append(self.current_stage)
+                    if subTest:
+                        self.result.addSubTest(test_case.test_case, test_case, exc_info)
+                    else:
+                        _addError(self.result, test_case, exc_info)
+                # explicitly break a reference cycle:
+                # exc_info -> frame -> exc_info
+                exc_info = None
+            else:
+                if subTest and self.success:
+                    self.result.addSubTest(test_case.test_case, test_case, None)
+            finally:
+                self.success = self.success and old_success
+
+    class TestCase(TestCaseSrc):
+        def __getattr__(self, name: str):
+            if name.startswith("_") and sys.version_info > NEWEST_PYTHON_VERSION:  # 重写框架使用了很多原有的_开头的函数, 如果不存在, 有可能是因为python版本引起的
+                raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}' maybe because your python version is greater than {NEWEST_PYTHON_VERSION_STR}")
+            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
+
+        def _miniSetUp(self):
+            pass
+
+        def _miniTearDown(self):
             pass
-        except:
-            exc_info = sys.exc_info()
-            if self.expecting_failure:
-                self.expectedFailure = exc_info
+
+        def run(self, result=None):
+            if result is None:
+                result = self.defaultTestResult()
+                startTestRun = getattr(result, 'startTestRun', None)
+                stopTestRun = getattr(result, 'stopTestRun', None)
+                if startTestRun is not None:
+                    startTestRun()
             else:
-                self.success = False
-                self.errors.append((test_case, exc_info))
-                if self.current_stage and self.current_stage in self.stage_errors:
-                    self.stage_errors[self.current_stage].append(exc_info)
-                elif self.current_stage:
-                    self.stage_errors[self.current_stage] = [exc_info,]
-                    self.error_stages.append(self.current_stage)
-            # explicitly break a reference cycle:
-            # exc_info -> frame -> exc_info
-            exc_info = None
-        else:
-            if self.result_supports_subtests and self.success:
-                self.errors.append((test_case, None))
-        finally:
-            self.success = self.success and old_success
+                stopTestRun = None
 
+            result.startTest(self)
+            try:
+                testMethod = getattr(self, self._testMethodName)
+                if (getattr(self.__class__, "__unittest_skip__", False) or
+                    getattr(testMethod, "__unittest_skip__", False)):
+                    # If the class or method was skipped.
+                    skip_why = (getattr(self.__class__, '__unittest_skip_why__', '')
+                                or getattr(testMethod, '__unittest_skip_why__', ''))
+                    _addSkip(result, self, skip_why)
+                    return result
+
+                expecting_failure = (
+                    getattr(self, "__unittest_expecting_failure__", False) or
+                    getattr(testMethod, "__unittest_expecting_failure__", False)
+                )
+                outcome = Outcome(result)
+                self._outcome = outcome
 
-# 重写testcase
-class TestCase(TestCaseSrc):
-    def __getattr__(self, name: str):
-        if name.startswith("_") and sys.version_info > NEWEST_PYTHON_VERSION:  # 重写框架使用了很多原有的_开头的函数, 如果不存在, 有可能是因为python版本引起的
-            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}' maybe because your python version is greater than {NEWEST_PYTHON_VERSION_STR}")
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
-
-    def _miniSetUp(self):
-        pass
-
-    def _miniTearDown(self):
-        pass
-
-    def run(self, result=None):
-        orig_result = result
-        if result is None:
-            result = self.defaultTestResult()
-            startTestRun = getattr(result, "startTestRun", None)
-            if startTestRun is not None:
-                startTestRun()
-
-        result.startTest(self)
-
-        testMethod = getattr(self, self._testMethodName)
-        if getattr(self.__class__, "__unittest_skip__", False) or getattr(
-            testMethod, "__unittest_skip__", False
-        ):
-            # If the class or method was skipped.
-            try:
-                skip_why = getattr(
-                    self.__class__, "__unittest_skip_why__", ""
-                ) or getattr(testMethod, "__unittest_skip_why__", "")
-                self._addSkip(result, self, skip_why)
-            finally:
-                result.stopTest(self)
-            return
+                with outcome.testPartExecutor(self, error_stage="_miniSetUp"):
+                    self._miniSetUp()
+                if outcome.success:
+                    with outcome.testPartExecutor(self, error_stage="setUp"):
+                        self._callSetUp()
+                    if outcome.success:
+                        outcome.expecting_failure = expecting_failure
+                        with outcome.testPartExecutor(self, error_stage="testMethod"):
+                            self._callTestMethod(testMethod)
+                        outcome.expecting_failure = False
+                        with outcome.testPartExecutor(self, error_stage="tearDown"):
+                            self._callTearDown()
+                outcome.expecting_failure = False
+                with outcome.testPartExecutor(self, error_stage="_miniTearDown"):
+                    self._miniTearDown()
+                self.doCleanups()
 
-        expecting_failure_method = getattr(
-            testMethod, "__unittest_expecting_failure__", False
-        )
-        expecting_failure_class = getattr(self, "__unittest_expecting_failure__", False)
-        expecting_failure = expecting_failure_class or expecting_failure_method
-        outcome = Outcome(result)
-        try:
-            self._outcome = outcome
-
-            with outcome.testPartExecutor(self, error_stage="_miniSetUp"):
-                self._miniSetUp()
-            if outcome.success:
-                with outcome.testPartExecutor(self, error_stage="setUp"):
-                    self._callSetUp()
                 if outcome.success:
-                    outcome.expecting_failure = expecting_failure
-                    with outcome.testPartExecutor(
-                        self, isTest=True, error_stage="testMethod"
-                    ):
-                        self._callTestMethod(testMethod)
-                    outcome.expecting_failure = False
-                    with outcome.testPartExecutor(self, error_stage="tearDown"):
-                        self._callTearDown()
-            outcome.expecting_failure = False
-            with outcome.testPartExecutor(self, error_stage="_miniTearDown"):
-                self._miniTearDown()
-
-            self.doCleanups()
-            for test, reason in outcome.skipped:
-                self._addSkip(result, test, reason)
-            self._feedErrorsToResult(result, outcome.errors)
-            if outcome.success:
-                if expecting_failure:
-                    if outcome.expectedFailure:
-                        self._addExpectedFailure(result, outcome.expectedFailure)
+                    if expecting_failure:
+                        if outcome.expectedFailure:
+                            self._addExpectedFailure(result, outcome.expectedFailure)
+                        else:
+                            self._addUnexpectedSuccess(result)
                     else:
-                        self._addUnexpectedSuccess(result)
-                else:
-                    result.addSuccess(self)
-            return result
-        finally:
-            result.stopTest(self)
-            if orig_result is None:
-                stopTestRun = getattr(result, "stopTestRun", None)
+                        result.addSuccess(self)
+                return result
+            finally:
+                result.stopTest(self)
                 if stopTestRun is not None:
                     stopTestRun()
 
-            # explicitly break reference cycles:
-            # outcome.errors -> frame -> outcome -> outcome.errors
-            # outcome.expectedFailure -> frame -> outcome -> outcome.expectedFailure
-            outcome.errors.clear()
-            outcome.expectedFailure = None
-
-            # clear the outcome, no more needed
-            self._outcome = None
-
-    @contextlib.contextmanager
-    def subTest(self, msg=_subtest_msg_sentinel, **params):
-        """Return a context manager that will return the enclosed block
-        of code in a subtest identified by the optional message and
-        keyword parameters.  A failure in the subtest marks the test
-        case as failed but resumes execution at the end of the enclosed
-        block, allowing further test code to be executed.
-        """
-        if self._outcome is None or not self._outcome.result_supports_subtests:
-            yield
-            return
-        parent = self._subtest
-        if parent is None:
-            params_map = _OrderedChainMap(params)
-        else:
-            params_map = parent.params.new_child(params)
-        self._subtest = _SubTest(self, msg, params_map)
-        try:
-            with self._outcome.testPartExecutor(self._subtest, isTest=True):
+                if self._outcome:
+                    outcome = self._outcome
+                    outcome.expectedFailure = None
+                    outcome.errors.clear()
+                    outcome.skipped.clear()
+                    outcome = None
+                    # clear the outcome, no more needed
+                    self._outcome = None
+
+        @contextlib.contextmanager
+        def subTest(self, msg=_subtest_msg_sentinel, **params):
+            """Return a context manager that will return the enclosed block
+            of code in a subtest identified by the optional message and
+            keyword parameters.  A failure in the subtest marks the test
+            case as failed but resumes execution at the end of the enclosed
+            block, allowing further test code to be executed.
+            """
+            if self._outcome is None or not self._outcome.result_supports_subtests:
                 yield
-            if not self._outcome.success:
-                result = self._outcome.result
-                if result is not None and result.failfast:
+                return
+            parent = self._subtest
+            if parent is None:
+                params_map = _OrderedChainMap(params)
+            else:
+                params_map = parent.params.new_child(params)
+            self._subtest = _SubTest(self, msg, params_map)
+            try:
+                with self._outcome.testPartExecutor(self._subtest, subTest=True):
+                    yield
+                if not self._outcome.success:
+                    result = self._outcome.result
+                    if result is not None and result.failfast:
+                        raise _ShouldStop
+                elif self._outcome.expectedFailure:
+                    # If the test is expecting a failure, we really want to
+                    # stop now and register the expected failure.
                     raise _ShouldStop
-            elif self._outcome.expectedFailure:
-                # If the test is expecting a failure, we really want to
-                # stop now and register the expected failure.
-                raise _ShouldStop
-        finally:
-            self._subtest = parent
-
-    def assertSetContainsSubset(self, subset: set, superset: set, msg=None):
-        """Checks whether superset is a superset of subset."""
-        warnings.warn("assertSetContainsSubset is deprecated", DeprecationWarning)
-        missing = []
-        for item in subset:
-            if item not in superset:
-                missing.append(item)
-
-        if not missing:
-            return
-
-        standardMsg = ""
-        if missing:
-            standardMsg = "Missing: %s" % ",".join(safe_repr(m) for m in missing)
-
-        self.fail(self._formatMessage(msg, standardMsg))
-
-
-class _SubTest(TestCase):
-
-    def __init__(self, test_case, message, params):
-        super().__init__()
-        self._message = message
-        self.test_case = test_case
-        self.params = params
-        self.failureException = test_case.failureException
-
-    def runTest(self):
-        raise NotImplementedError("subtests cannot be run directly")
-
-    def _subDescription(self):
-        parts = []
-        if self._message is not _subtest_msg_sentinel:
-            parts.append("[{}]".format(self._message))
-        if self.params:
-            params_desc = ', '.join(
-                "{}={!r}".format(k, v)
-                for (k, v) in self.params.items())
-            parts.append("({})".format(params_desc))
-        return " ".join(parts) or '(<subtest>)'
-
-    def id(self):
-        return "{} {}".format(self.test_case.id(), self._subDescription())
-
-    def shortDescription(self):
-        """Returns a one-line description of the subtest, or None if no
-        description has been provided.
-        """
-        return self.test_case.shortDescription()
+            finally:
+                self._subtest = parent
+
+        def assertSetContainsSubset(self, subset: set, superset: set, msg=None):
+            """Checks whether superset is a superset of subset."""
+            warnings.warn("assertSetContainsSubset is deprecated", DeprecationWarning)
+            missing = []
+            for item in subset:
+                if item not in superset:
+                    missing.append(item)
+
+            if not missing:
+                return
+
+            standardMsg = ""
+            if missing:
+                standardMsg = "Missing: %s" % ",".join(safe_repr(m) for m in missing)
+
+            self.fail(self._formatMessage(msg, standardMsg))
+
+    # copy
+    class _SubTest(TestCase):
+
+        def __init__(self, test_case, message, params):
+            super().__init__()
+            self._message = message
+            self.test_case = test_case
+            self.params = params
+            self.failureException = test_case.failureException
+
+        def runTest(self):
+            raise NotImplementedError("subtests cannot be run directly")
+
+        def _subDescription(self):
+            parts = []
+            if self._message is not _subtest_msg_sentinel:
+                parts.append("[{}]".format(self._message))
+            if self.params:
+                params_desc = ', '.join(
+                    "{}={!r}".format(k, v)
+                    for (k, v) in self.params.items())
+                parts.append("({})".format(params_desc))
+            return " ".join(parts) or '(<subtest>)'
+
+        def id(self):
+            return "{} {}".format(self.test_case.id(), self._subDescription())
+
+        def shortDescription(self):
+            """Returns a one-line description of the subtest, or None if no
+            description has been provided.
+            """
+            return self.test_case.shortDescription()
+
+        def __str__(self):
+            return "{} {}".format(self.test_case, self._subDescription())
+
+else:
+    NEWEST_PYTHON_VERSION = (3, 10, 5)
+    NEWEST_PYTHON_VERSION_STR = ".".join([str(s) for s in NEWEST_PYTHON_VERSION])
+    from unittest.case import _Outcome, _ShouldStop, warnings, safe_repr, _OrderedChainMap, _subtest_msg_sentinel
+
+    class Outcome(_Outcome):
+        def __init__(self, result=None):
+            super().__init__(result)
+            # 兼容3.11
+            self.skipped = []
+            self.errors = []
+            self.current_stage = None
+            self.error_stages = []  # 失败发生在的步骤：_miniClassSetUp, _miniSetUp, _miniTearDown, setUpClass, tearDownClass, setUp, tearDown, testMethod
+            self.stage_errors = {}  # 发生在每个stage的具体error
+
+        @contextlib.contextmanager
+        def testPartExecutor(self, test_case, isTest=False, error_stage=None):
+            """
+            rewrite for error_stages
+            :error_stage: current error stage name
+            """
+            old_success = self.success
+            self.success = True
+            self.current_stage = error_stage or self.current_stage
+            try:
+                yield
+            except KeyboardInterrupt:
+                raise
+            except SkipTest as e:
+                self.success = False
+                self.skipped.append((test_case, str(e)))
+            except _ShouldStop:
+                pass
+            except:
+                exc_info = sys.exc_info()
+                if self.expecting_failure:
+                    self.expectedFailure = exc_info
+                else:
+                    self.success = False
+                    self.errors.append((test_case, exc_info))
+                    if self.current_stage and self.current_stage in self.stage_errors:
+                        self.stage_errors[self.current_stage].append(exc_info)
+                    elif self.current_stage:
+                        self.stage_errors[self.current_stage] = [exc_info,]
+                        self.error_stages.append(self.current_stage)
+                # explicitly break a reference cycle:
+                # exc_info -> frame -> exc_info
+                exc_info = None
+            else:
+                if self.result_supports_subtests and self.success:
+                    self.errors.append((test_case, None))
+            finally:
+                self.success = self.success and old_success
+
+
+    class TestCase(TestCaseSrc):
+        def __getattr__(self, name: str):
+            if name.startswith("_") and sys.version_info > NEWEST_PYTHON_VERSION:  # 重写框架使用了很多原有的_开头的函数, 如果不存在, 有可能是因为python版本引起的
+                raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}' maybe because your python version is greater than {NEWEST_PYTHON_VERSION_STR}")
+            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
+
+        def _miniSetUp(self):
+            pass
+
+        def _miniTearDown(self):
+            pass
+
+        def run(self, result=None):
+            orig_result = result
+            if result is None:
+                result = self.defaultTestResult()
+                startTestRun = getattr(result, "startTestRun", None)
+                if startTestRun is not None:
+                    startTestRun()
+
+            result.startTest(self)
+
+            testMethod = getattr(self, self._testMethodName)
+            if getattr(self.__class__, "__unittest_skip__", False) or getattr(
+                testMethod, "__unittest_skip__", False
+            ):
+                # If the class or method was skipped.
+                try:
+                    skip_why = getattr(
+                        self.__class__, "__unittest_skip_why__", ""
+                    ) or getattr(testMethod, "__unittest_skip_why__", "")
+                    self._addSkip(result, self, skip_why)
+                finally:
+                    result.stopTest(self)
+                return
+
+            expecting_failure_method = getattr(
+                testMethod, "__unittest_expecting_failure__", False
+            )
+            expecting_failure_class = getattr(self, "__unittest_expecting_failure__", False)
+            expecting_failure = expecting_failure_class or expecting_failure_method
+            outcome = Outcome(result)
+            try:
+                self._outcome = outcome
+
+                with outcome.testPartExecutor(self, error_stage="_miniSetUp"):
+                    self._miniSetUp()
+                if outcome.success:
+                    with outcome.testPartExecutor(self, error_stage="setUp"):
+                        self._callSetUp()
+                    if outcome.success:
+                        outcome.expecting_failure = expecting_failure
+                        with outcome.testPartExecutor(
+                            self, isTest=True, error_stage="testMethod"
+                        ):
+                            self._callTestMethod(testMethod)
+                        outcome.expecting_failure = False
+                        with outcome.testPartExecutor(self, error_stage="tearDown"):
+                            self._callTearDown()
+                outcome.expecting_failure = False
+                with outcome.testPartExecutor(self, error_stage="_miniTearDown"):
+                    self._miniTearDown()
+
+                self.doCleanups()
+                for test, reason in outcome.skipped:
+                    self._addSkip(result, test, reason)
+                self._feedErrorsToResult(result, outcome.errors)
+                if outcome.success:
+                    if expecting_failure:
+                        if outcome.expectedFailure:
+                            self._addExpectedFailure(result, outcome.expectedFailure)
+                        else:
+                            self._addUnexpectedSuccess(result)
+                    else:
+                        result.addSuccess(self)
+                return result
+            finally:
+                result.stopTest(self)
+                if orig_result is None:
+                    stopTestRun = getattr(result, "stopTestRun", None)
+                    if stopTestRun is not None:
+                        stopTestRun()
+
+                # explicitly break reference cycles:
+                # outcome.errors -> frame -> outcome -> outcome.errors
+                # outcome.expectedFailure -> frame -> outcome -> outcome.expectedFailure
+                outcome.errors.clear()
+                outcome.expectedFailure = None
+
+                # clear the outcome, no more needed
+                self._outcome = None
+
+        @contextlib.contextmanager
+        def subTest(self, msg=_subtest_msg_sentinel, **params):
+            """Return a context manager that will return the enclosed block
+            of code in a subtest identified by the optional message and
+            keyword parameters.  A failure in the subtest marks the test
+            case as failed but resumes execution at the end of the enclosed
+            block, allowing further test code to be executed.
+            """
+            if self._outcome is None or not self._outcome.result_supports_subtests:
+                yield
+                return
+            parent = self._subtest
+            if parent is None:
+                params_map = _OrderedChainMap(params)
+            else:
+                params_map = parent.params.new_child(params)
+            self._subtest = _SubTest(self, msg, params_map)
+            try:
+                with self._outcome.testPartExecutor(self._subtest, isTest=True):
+                    yield
+                if not self._outcome.success:
+                    result = self._outcome.result
+                    if result is not None and result.failfast:
+                        raise _ShouldStop
+                elif self._outcome.expectedFailure:
+                    # If the test is expecting a failure, we really want to
+                    # stop now and register the expected failure.
+                    raise _ShouldStop
+            finally:
+                self._subtest = parent
+
+        def assertSetContainsSubset(self, subset: set, superset: set, msg=None):
+            """Checks whether superset is a superset of subset."""
+            warnings.warn("assertSetContainsSubset is deprecated", DeprecationWarning)
+            missing = []
+            for item in subset:
+                if item not in superset:
+                    missing.append(item)
+
+            if not missing:
+                return
+
+            standardMsg = ""
+            if missing:
+                standardMsg = "Missing: %s" % ",".join(safe_repr(m) for m in missing)
+
+            self.fail(self._formatMessage(msg, standardMsg))
+
+
+    class _SubTest(TestCase):
+
+        def __init__(self, test_case, message, params):
+            super().__init__()
+            self._message = message
+            self.test_case = test_case
+            self.params = params
+            self.failureException = test_case.failureException
+
+        def runTest(self):
+            raise NotImplementedError("subtests cannot be run directly")
+
+        def _subDescription(self):
+            parts = []
+            if self._message is not _subtest_msg_sentinel:
+                parts.append("[{}]".format(self._message))
+            if self.params:
+                params_desc = ', '.join(
+                    "{}={!r}".format(k, v)
+                    for (k, v) in self.params.items())
+                parts.append("({})".format(params_desc))
+            return " ".join(parts) or '(<subtest>)'
+
+        def id(self):
+            return "{} {}".format(self.test_case.id(), self._subDescription())
+
+        def shortDescription(self):
+            """Returns a one-line description of the subtest, or None if no
+            description has been provided.
+            """
+            return self.test_case.shortDescription()
 
-    def __str__(self):
-        return "{} {}".format(self.test_case, self._subDescription())
+        def __str__(self):
+            return "{} {}".format(self.test_case, self._subDescription())
 
 
 def _whether_need_skip(func: types.FunctionType, *args, **kwargs):
     if func.__code__.co_argcount == 0:
         need_skip = func()
     elif func.__code__.co_argcount == 1:
         need_skip = func(args[0])  # just use TestCase
```

### Comparing `minium-1.4.1/minium/framework/libs/unittest/suite.py` & `minium-1.4.2/minium/framework/libs/unittest/suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
                 if currentClass._classSetupFailed is True:
                     currentClass.doClassCleanups()
                     if len(currentClass.tearDown_exceptions) > 0:
                         for exc in currentClass.tearDown_exceptions:
                             self._createClassOrModuleLevelException(
                                 result, exc[1], "setUpClass", className, info=exc
                             )
-                    return
 
         # run setUpClass
         setUpClass = getattr(currentClass, "setUpClass", None)
         if setUpClass is not None:
             _call_if_exists(result, "_setupStdout")
             try:
                 setUpClass()
```

### Comparing `minium-1.4.1/minium/framework/loader.py` & `minium-1.4.2/minium/framework/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-31
-from lib2to3.pgen2.token import SLASH
 import sys
 import os.path
 import argparse
 import platform
 
 # import unittest
 import logging.handlers
@@ -166,35 +165,35 @@
             "can't not find testcase %s in module %s" % (case_name, module)
         )
 
 
 def test_ws_connection(test_port):
     def on_open(ws):
         global is_connected
-        print("connection opened")
+        logger.info("connection opened")
         is_connected = True
 
     def on_error(ws, error):
-        print("error: %s" % str(error))
+        logger.error("error: %s" % str(error))
         exit(1)
 
     def on_message(ws, message):
         global test_response
-        print("receive: %s" % message)
+        logger.info("receive: %s" % message)
         message = json.loads(message)
         if message["id"] == "minitest-test-id":
             test_response = message
 
-    def on_close(ws):
+    def on_close(ws, *args):
         global is_connected
-        print("closed")
+        logger.info("closed")
         is_connected = False
 
     url = "ws://localhost:{}".format(test_port)
-    print("start connect {}".format(url))
+    logger.info("start connect {}".format(url))
     client = websocket.WebSocketApp(
         url,
         on_open=on_open,
         on_message=on_message,
         on_error=on_error,
         on_close=on_close,
     )
@@ -204,45 +203,45 @@
 
     thread = threading.Thread(target=run_forever, args=())
     thread.daemon = True
     thread.start()
     s = time.time()
     while time.time() - s < 10 and thread.is_alive():
         if is_connected:
-            print("connect to WebChatTools successfully")
-            print("连接开发者工具成功")
+            logger.info("connect to WebChatTools successfully")
+            logger.info("连接开发者工具成功")
             break
         time.sleep(1)
     else:
-        print("connect WebChatTools fail, please confirm the test port is open")
-        print("连接开发者工具失败，可能的原因有:")
-        print("1. 没有打开自动化测试端口，请检查开发者工具的通知栏是否有: 小程序的自动化端口已开启，端口号是 xxxx")
-        print("2. 调试基础库版本过低，请选择最新版本")
+        logger.warning("connect WebChatTools fail, please confirm the test port is open")
+        logger.warning("连接开发者工具失败，可能的原因有:")
+        logger.warning("1. 没有打开自动化测试端口，请检查开发者工具的通知栏是否有: 小程序的自动化端口已开启，端口号是 xxxx")
+        logger.warning("2. 调试基础库版本过低，请选择最新版本")
         exit(1)
     message = json.dumps(
         {
             "id": "minitest-test-id",
             "method": "App.callWxMethod",
             "params": {"method": "getSystemInfoSync", "args": []},
         },
         separators=(",", ":"),
     )
     client.send(message)
     s = time.time()
     while time.time() - s < 30:
         if test_response:
-            print("response successfully")
-            print("收到命令返回")
+            logger.info("response successfully")
+            logger.info("收到命令返回")
             break
         time.sleep(1)
     else:
-        print(
+        logger.warning(
             "can't receive response, please confirm miniprogram is launch successfully"
         )
-        print("未收到命令返回，请确认小程序项目是否正确运行(没有白屏/报错)")
+        logger.warning("未收到命令返回，请确认小程序项目是否正确运行(没有白屏/报错)")
         exit(1)
     client.close()
 
 
 def get_config(config):
     conf_list = []
     if config:
@@ -294,15 +293,15 @@
     :return:
     """
     # default dev_tool_path
     MAC_DEVTOOL_PATH = "/Applications/wechatwebdevtools.app/Contents/MacOS/cli"
     WINDOWS_DEVTOOL_PATH = "C:/Program Files (x86)/Tencent/微信web开发者工具/cli.bat"
 
     if sys.version_info.major < 3 and sys.version_info.minor < 8:
-        print("python version is less than 3.8, please update")
+        logger.warning("python version is less than 3.8, please update")
 
     is_mac = True
     SLASH = "/"
 
     if platform.system().lower() == "windows":
         is_mac = False
         SLASH = "\\"
@@ -375,15 +374,15 @@
                 dev_tool_path
                 if is_mac
                 else ('"%s"' % dev_tool_path)
                 + " auto --project "
                 + config.project_path
                 + "--auto-port 9420"
             )
-            print(start_cli)
+            logger.info(start_cli)
 
 
 def main():
     # bug: 在 fork 模式下Python 会出现 crash
     # crashed on child side of fork pre-exec
     # Invalid dylib load. Clients should not load the unversioned libcrypto dylib as it does not have a stable ABI.
     import multiprocessing
@@ -534,16 +533,17 @@
 
     if show_accounts:
         # 打印已登录的多账号
         if config:
             print(WXMinium(get_config(config)[0]).get_test_accounts())
         else:
             # 没有配置的先看看端口是否打开了
+            # logger.setLevel(logging.WARNING)
             test_ws_connection(9420)
-            print(WXMinium().get_test_accounts())
+            print(WXMinium(miniconfig.MiniConfig({"debug_mode": "warn"})).get_test_accounts())
         exit(0)
 
     if test_connection:
         # 测试ws链接是否正常
         test_ws_connection(test_port)
         exit(0)
```

### Comparing `minium-1.4.1/minium/framework/logcolor.py` & `minium-1.4.2/minium/framework/logcolor.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,43 +30,39 @@
 
         # Constants from the Windows API
         self.STD_OUTPUT_HANDLE = -11
         hdl = ctypes.windll.kernel32.GetStdHandle(self.STD_OUTPUT_HANDLE)
         ctypes.windll.kernel32.SetConsoleTextAttribute(hdl, code)
 
     def filter(self, record):
-        FOREGROUND_BLUE = 0x0001  # text color contains blue.
-        FOREGROUND_GREEN = 0x0002  # text color contains green.
-        FOREGROUND_RED = 0x0004  # text color contains red.
-        FOREGROUND_INTENSITY = 0x0008  # text color is intensified.
-        FOREGROUND_WHITE = FOREGROUND_BLUE | FOREGROUND_GREEN | FOREGROUND_RED
         # winbase.h
-        STD_INPUT_HANDLE = -10
-        STD_OUTPUT_HANDLE = -11
-        STD_ERROR_HANDLE = -12
+        # STD_INPUT_HANDLE = -10
+        # STD_OUTPUT_HANDLE = -11
+        # STD_ERROR_HANDLE = -12
 
         # wincon.h
-        FOREGROUND_BLACK = 0x0000
+        # FOREGROUND_BLACK = 0x0000
         FOREGROUND_BLUE = 0x0001
         FOREGROUND_GREEN = 0x0002
-        FOREGROUND_CYAN = 0x0003
+        # FOREGROUND_CYAN = 0x0003
         FOREGROUND_RED = 0x0004
         FOREGROUND_MAGENTA = 0x0005
         FOREGROUND_YELLOW = 0x0006
-        FOREGROUND_GREY = 0x0007
+        # FOREGROUND_GREY = 0x0007
         FOREGROUND_INTENSITY = 0x0008  # foreground color is intensified.
+        FOREGROUND_WHITE = FOREGROUND_BLUE | FOREGROUND_GREEN | FOREGROUND_RED
 
-        BACKGROUND_BLACK = 0x0000
-        BACKGROUND_BLUE = 0x0010
-        BACKGROUND_GREEN = 0x0020
-        BACKGROUND_CYAN = 0x0030
-        BACKGROUND_RED = 0x0040
-        BACKGROUND_MAGENTA = 0x0050
+        # BACKGROUND_BLACK = 0x0000
+        # BACKGROUND_BLUE = 0x0010
+        # BACKGROUND_GREEN = 0x0020
+        # BACKGROUND_CYAN = 0x0030
+        # BACKGROUND_RED = 0x0040
+        # BACKGROUND_MAGENTA = 0x0050
         BACKGROUND_YELLOW = 0x0060
-        BACKGROUND_GREY = 0x0070
+        # BACKGROUND_GREY = 0x0070
         BACKGROUND_INTENSITY = 0x0080  # background color is intensified.
         levelno = record.levelno
 
         if levelno >= 50:
             color = (
                 BACKGROUND_YELLOW
                 | FOREGROUND_RED
```

### Comparing `minium-1.4.1/minium/framework/miniconfig.py` & `minium-1.4.2/minium/framework/miniconfig.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/miniddt.py` & `minium-1.4.2/minium/framework/miniddt.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/minilimit.py` & `minium-1.4.2/minium/framework/minilimit.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/miniprogram.py` & `minium-1.4.2/minium/framework/miniprogram.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/miniresult.py` & `minium-1.4.2/minium/framework/miniresult.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-06-18
 # import unittest
 import json
 import os
 from minium.framework.libs import unittest
-from .miniconfig import MiniConfig, get_log_level
 from .assertbase import AssertBase
 
 FILENAME_SUMMARY = "summary.json"
 
 
 class MiniResult(unittest.TestResult):
     def __init__(self, stream=None, descriptions=None, verbosity=None):
@@ -166,27 +165,27 @@
 
     def test_2(self):
         self.assertTrue(False, "failed")
 
 
 class Test3(unittest.TestCase):
     @classmethod
-    def setUpClass(self):
+    def setUpClass(cls):
         raise RuntimeError("setup class failed")
 
     def test_1(self):
         self.assertTrue(True)
 
     def test_2(self):
         self.assertTrue(False, "failed")
 
 
 class Test4(unittest.TestCase):
     @classmethod
-    def setUpClass(self):
+    def setUpClass(cls):
         raise RuntimeError("setup class failed")
 
     def test_1(self):
         self.assertTrue(True)
 
     def test_2(self):
         self.assertTrue(False, "failed")
```

### Comparing `minium-1.4.1/minium/framework/minisuite.py` & `minium-1.4.2/minium/framework/minisuite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+'''
+Author: yopofeng yopofeng@tencent.com
+Date: 2023-04-27 10:22:31
+LastEditors: yopofeng yopofeng@tencent.com
+LastEditTime: 2023-06-21 17:57:21
+FilePath: /py-minium/minium/framework/minisuite.py
+Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
+'''
 #!/usr/local/bin/python3
 # -*- coding: utf-8 -*-
 """
 Author:         lockerzhang
 Filename:       minisuite.py
 Create time:    2020/1/3 16:22
 Update time:    2022/4/12 16:29
@@ -9,15 +17,14 @@
 
 """
 import os
 import json
 import fnmatch
 import logging.handlers
 from .exception import MiniParamsError
-import json
 from json import JSONDecodeError
 import traceback
 
 logger = logging.getLogger("minium")
 
 
 class MiniSuite(object):
```

### Comparing `minium-1.4.1/minium/framework/minitest.py` & `minium-1.4.2/minium/framework/minitest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-06
 import datetime
 import json
 import os.path
-from posixpath import realpath
 import shutil
 import time
 import inspect
 
 import minium
 import minium.miniprogram.base_driver.minium_log
 import minium.native
 from minium.native.exception import *
 from .miniconfig import MiniConfig
 from .assertbase import AssertBase, HookAssert
 from .logcolor import *
 from .exception import *
 from ..utils.utils import retry, catch
-from ..utils.injectjs import getInjectJsCode
 from .miniprogram import MiniProgram
 from ..miniprogram import Minium
 from ..miniprogram.base_driver.app import App
 from ..native import BaseNative
 from typing import Tuple
+from minium.miniprogram.base_driver.minium_log import report_exception, ExceptionData
 
 # import matplotlib.pyplot as plt
 
 logger = logging.getLogger("minium")
 
 g_minium: Minium = None
 g_native: BaseNative = None
@@ -48,19 +47,19 @@
     """
     global g_minium, g_native
     if g_minium:
         reset_minium()
     if g_native:
         try:
             g_native.stop_wechat()
-        except:
+        except Exception:
             pass
         try:
             g_native.release()
-        except:
+        except Exception:
             pass
         g_native = None
 
 
 def reset_minium():
     """
     1. miniProgram 部分 release
@@ -199,14 +198,15 @@
         g_network_resp_cache[hash_id]["timestamp"] = time.time()
     if msg_id not in g_network_message_dict:
         g_network_message_dict[msg_id] = {"timestamp": time.time() * 1000}
     g_network_message_dict[msg_id]["end_timestamp"] = ms
     g_network_message_dict[msg_id]["response"] = json.loads(res)
     g_network_message_dict[msg_id]["mocked"] = bool(mocked)
 
+
 class MetaMiniTest(HookAssert):
     def __new__(cls, name, bases, attrs):
         return super(MetaMiniTest, cls).__new__(cls, name, bases, attrs)
 
     @property
     def app(cls):
         if not inspect.isclass(cls):
@@ -229,15 +229,15 @@
 
     _app: App = None
 
     def __init__(self, methodName: str = "runTest") -> None:
         super().__init__(methodName)
         # 这个case是否需要重试, 目前重试原则为
         # 1. case运行过程中遇到断连的情况
-        self.__will_retry = None  
+        self.__will_retry = None
 
     @property
     def app(self) -> minium.App:
         return self._app or (self.mini and self.mini.app)
 
     @app.setter
     def app(self, value):
@@ -291,48 +291,47 @@
 
         :return None or Exception: None for ok
         """
         if self.native:
             if not self.native.check_connection():
                 self.logger.warning("check native connection error, relaunch app")
                 return ResetError.RELAUNCH_APP
-        if self.mini: # 小程序异常退出和链接断连都会自动重连和重新拉起
+        if self.mini:  # 小程序异常退出和链接断连都会自动重连和重新拉起
             if self.mini.is_app_relaunching:
                 self.logger.warning("app is relaunching, wait for it")
                 e = self.mini.wait_app_relaunch()
                 if e:
                     self.logger.warning(e)
                     return ResetError.RELAUNCH_APP
             if self.mini.connection and self.mini.connection.is_reconnecting:
                 self.logger.warning("connection is reconnecting, wait for it")
                 e = self.mini.connection.wait_reconnect()
                 if e:
                     self.logger.warning(e)
                     return ResetError.RELAUNCH_APP
         return ResetError.OK
-    
+
     def _update_miniprogram(self, native, mini):
         self.logger.debug(
             "start update miniprogram, class is: %s" % self.__class__.__name__
         )
         self.__class__.native = native
         self.__class__.mini = mini
         self.mini = mini
         self.native = native
         self.logger.debug(
             "finish update miniprogram, current native: %s, minium: %s"
             % (id(self.mini), id(self.native))
         )
 
     def init_miniprogram(self):
-        """case中重新实例化小程序
-        """
+        """case中重新实例化小程序"""
         try:
             native, mini, _ = init_miniprogram(self.__class__.CONFIG)
-        except:
+        except Exception:
             self._update_miniprogram(g_native, g_minium)
             raise
         else:
             self._update_miniprogram(native, mini)
 
     def _miniSetUp(self):
         super(MiniTest, self)._miniSetUp()
@@ -480,15 +479,15 @@
                     perf_re["avg_cpu"] = sum(cpu_arr) / (len(cpu_arr) or 1)
                     perf_re["avg_mem"] = sum(mem_arr) / (len(mem_arr) or 1)
                     perf_re["avg_fps"] = sum(fps_arr) / (len(fps_arr) or 1)
                     perf_re["max_cpu"] = max(cpu_arr)
                     perf_re["max_mem"] = max(mem_arr)
                     perf_re["min_fps_rt"] = min(fps_arr)
                     self.perf_data = json.dumps(perf_re)
-                except:
+                except Exception:
                     self.perf_data = json.dumps(perf_init)
 
         else:
             self.perf_data = json.dumps(perf_init)
         self.results["perf_data"] = self.perf_data
 
     # 不应在case setup做
@@ -574,15 +573,18 @@
         if not error:
             return
         if isinstance(error, (MiniConnectionClosedError, MiniReConnectSvrError)):
             # 因为断连而产生的指令超时, 可尝试重试{1}次
             if self.__will_retry is None:
                 self.__will_retry = FRAMEWORK_RETRY
             return
-        if isinstance(error, MiniElementNotFoundError) and not self.test_config.teardown_snapshot:
+        if (
+            isinstance(error, MiniElementNotFoundError)
+            and not self.test_config.teardown_snapshot
+        ):
             # 找不到元素, 把wxml拿回来帮助用户排查. 如果配置了`teardown_snapshot`, 则已经获取过不需要再获取
             self.results["page_wxml"] = self.page_wxml
             return
 
     def _miniTearDown(self):
         logger.debug("=========Current case Down: %s=========" % self._testMethodName)
         self._framework_capture("teardown")
@@ -600,19 +602,30 @@
         if self.test_config.case_output and os.path.isdir(self.test_config.case_output):
             shutil.rmtree(self.test_config.case_output)
 
     def run(self, result=None):
         ret = super().run(result)
         if self.__will_retry is None:
             return ret
-        while self.__will_retry > 0:
+        while self.__will_retry > 0 and not self.results["success"]:
             self.__will_retry -= 1
             self._cleanup_before_retry()
             self.logger.warning(f"第{FRAMEWORK_RETRY-self.__will_retry}次重试")
             ret = super().run(result)
+        else:
+            if self.results["success"]:
+                report_exception(ExceptionData(
+                    RetrySuccess(self._testMethodName),
+                    retry=FRAMEWORK_RETRY - self.__will_retry,
+                ))
+            else:
+                report_exception(ExceptionData(
+                    RetryFail(self._testMethodName),
+                    retry=FRAMEWORK_RETRY - self.__will_retry,
+                ))
         return ret
 
     @property
     def page(self) -> minium.Page:
         return self.mini.app.current_page
 
     @property
@@ -626,26 +639,26 @@
         if wxml:
             filename = datetime.datetime.now().strftime("%d%H%M%S.wxml")
             filepath = self.wrap_filename(filename)
             with open(filepath, "w", encoding="utf8") as fd:
                 fd.write(wxml)
             return filename
         return wxml
-    
+
     @catch
     @retry(2)
     def _framework_capture(self, name=""):
         """框架截图, 尝试两次, 不报错
 
         :param str name: 截图文件名, defaults to ""
         """
         if not self.test_config.framework_capture:
             return ""
         return self.capture(name)
-    
+
     @catch
     @retry(2)
     def _error_capture(self, error: Exception):
         """报错截图, 尝试两次, 不报错
 
         :param Exception error: 具体报错, 截图文件名由报错类名定义
         """
@@ -687,15 +700,15 @@
     def tap_capture(self, name, page_id):
         """
         点击截图
         :param name: 截图文件名
         :param page_id: 点击元素所属的页面id
         """
         raise NotImplementedError("仅云测支持")
-    
+
     def tap_mark(self, name: str, point: Tuple, page_id):
         """
         给截图标记点击的点
         :return: bool
         """
         raise NotImplementedError("仅云测支持")
```

### Comparing `minium-1.4.1/minium/framework/report.py` & `minium-1.4.2/minium/framework/report.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/session.py` & `minium-1.4.2/minium/framework/session.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/tools/report_issue.py` & `minium-1.4.2/minium/framework/tools/report_issue.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/framework/wording.py` & `minium-1.4.2/minium/framework/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/miniprogram/__init__.py` & `minium-1.4.2/minium/miniprogram/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/app.py` & `minium-1.4.2/minium/miniprogram/base_driver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 """
 @Author: lockerzhang
 @LastEditors: lockerzhang
 @Description: 小程序层面的操作(包含 web 和 Native)
 @Date: 2019-03-11 14:41:43
 @LastEditTime: 2019-06-05 16:30:44
 """
+from __future__ import annotations
 import typing
 import types
 from enum import Enum
+from typing import Any
+import functools
 
 from minium.utils.utils import AsyncCondition
 from .page import Page
 from .minium_object import MiniumObject, RetryableApi
 from ...framework.exception import *
-from ...utils.injectjs import getInjectJsCode, JsMode
+from ...utils.injectjs import JsMode
 from ...utils.platforms import *
 from ...utils.emitter import ee
 from ...utils.eventloop import event_loop
 from ...utils.utils import get_result, WaitTimeoutError, retry, catch, urlencode
 from .callback import AsyncCallback, Callback
 import os
 import json
@@ -187,15 +190,56 @@
         # protect(common method)
         "_mock_wx_method",  # 各类mock方法都使用到
         "_page_stack",
         # private
         "__get_pages_config",
     ]
 
-    def __init__(self, connection, relaunch=False, native=None, platform="ide"):
+    class CurrentPage(object):
+        """代理current_page
+        """
+        def __init__(self, app: App) -> None:
+            self.app = app
+
+        def __del__(self):
+            self.app = None
+
+        @property
+        def _current_page(self):
+            return self.app._current_page or self.app.get_current_page()
+
+        def _catch_page_destroyed_error(self, func):
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):
+                try:
+                    return func(*args, **kwargs)
+                except PageDestroyed:
+                    attr = getattr(self.app._current_page, func.__name__)
+                    return attr(*args, **kwargs)
+            return wrapper
+
+        def __getattr__(self, __name: str) -> Any:
+            attr = getattr(self._current_page, __name)
+            if callable(attr):  # 可能是api接口
+                return self._catch_page_destroyed_error(attr)
+            return attr
+        
+        def __eq__(self, page):
+            return self._current_page == page
+        
+        def __ne__(self, page) -> bool:
+            return not (self._current_page == page)
+        
+        def __repr__(self):
+            _current_page = self._current_page
+            return "Page(id={0}, path={1}, query={2})".format(
+                _current_page.page_id, _current_page.path, _current_page.query
+            )
+
+    def __init__(self, connection, relaunch=False, native=None, platform="ide", **kwargs):
         """
         创建一个 APP 实例
         :param connection:
         """
         super().__init__()
         self.connection = connection
         self.native = native
@@ -204,43 +248,58 @@
             JsMode.JUST_ES5 if platform in [OS_ANDROID, OS_IOS] else JsMode.ALL
         )  # 真机调试2.0环境下只支持es5语法
         self._msg_lock = threading.Condition()
         self._async_msg_lock = AsyncCondition(loop=event_loop)
         self._is_log_enable = False
         self._main_page_path = None
         self.route_return_page = None
-        self.route_return_page_update_time = None  # 监听到页面变化后由于是异步通信, 有可能出现两个相近信息重复顺序调乱
+        self._route_return_page_update_time = None  # 监听到页面变化后由于是异步通信, 有可能出现两个相近信息重复顺序调乱
         self._appid = None
         self._current_page = None  # 只有调用 get_current_page 和 监听到 _on_route_changed 回调时更新
+        self.current_page = App.CurrentPage(self)
         self._mocked_images = None
         self._mocked_images_dir = None
         self._mocked_images_data = {}
         # init methods
         self._route_change_listener()
         self._request_stack_listener()
-        self.__is_injected = self._evaluate_js(
-            "checkInject"
-        )  # 是否已经注入过了, 注入过的环境不需要重复注入, 防止出现多次回调等预期之外的情况
+        # self.__is_injected = self._evaluate_js(
+        #     "checkInject"
+        # )  # 是否已经注入过了, 注入过的环境不需要重复注入, 防止出现多次回调等预期之外的情况
+        env = self._evaluate_js("checkEnv")
+        self.__is_injected = env.get("injected")  # 是否已经注入过了, 注入过的环境不需要重复注入, 防止出现多次回调等预期之外的情况
+        self._is_third_app = env.get("isThirdApp")  # 是否是第三方开发框架构建的小程序, 影响mock & hook功能
         self.pages = []
         self.tabbar_pages = {}
         self.__get_pages_config()
         if not self.__is_injected and self.js_mode is JsMode.JUST_ES5:  # 注入一些垫片
             self._evaluate_js("helpers")
         if relaunch:
             self.relaunch(self.main_page_path.path, self.main_page_path.query)
 
+    def release(self):
+        """释放循环引用
+        _current_page -> app -> _current_page
+        """
+        current_page = self._current_page
+        if current_page:
+            self._current_page = None
+            current_page.app = None
+        self.current_page.app = None
+        self.current_page = None
+
     @property
     def app_id(self):
         if not self._appid:
             self._appid = self._get_account_info_sync().result.result.miniProgram.appId
         return self._appid
 
-    @property
-    def current_page(self):
-        return self._current_page or self.get_current_page()
+    # @property
+    # def current_page(self):
+    #     return self._current_page or self.get_current_page()
 
     @property
     def is_injected(self):
         """
         是否已经注入过, 如果没有, 则设置并进行注入操作
         """
         if self.__is_injected:
@@ -597,25 +656,25 @@
         :param is_click: 点击触发帮用户触发一下onTabItemTap
         :return:Page 对象
         """
         page = self._change_route_async(
             "switchTab", url, is_wait_url_change, wait_route_done_time
         )
         if is_click and page.path in self.tabbar_pages:  # is tabbar and is click
-            # 需要触发 onTabItemTap
             try:
                 page.call_method(
                     "onTabItemTap",
                     {
                         "index": self.tabbar_pages[page.path]["index"],
                         "pagePath": self.tabbar_pages[page.path]["pagePath"],
                         "text": self.tabbar_pages[page.path]["text"],
                     },
                 )
             except MiniAppError:
+                # 尝试触发 onTabItemTap 即可
                 pass
         if page != url.split("?")[0]:
             self.logger.warning("Switch tab(%s) but(%s)" % (url, page.path))
         return page
 
     def stop_audits(self, path: str = None):
         """
@@ -696,17 +755,18 @@
         self._wait(get, timeout)
         return ret
 
     def wait_for_page(self, page_path=None, max_timeout=10):
         if not self._current_page or self._current_page != page_path:
             # 没有记录到当前页面/当前页面不是目标页面, 等待页面跳转成功的回调
             self._route_changed(max_timeout)
-            ret = self.current_page == page_path
+            ret = (self.current_page == page_path)
             # issue#144 如果等不到预期的页面, 考虑是否因为页面栈满了(自动化流程中, 用户可以直接调用navigate to, 很有可能会满的)
             if not ret:
+                self.logger.debug(f"{self.current_page} != {page_path}")
                 if len(self._page_stack()) == 10:
                     self.logger.warning(
                         """
 wait for page fail, probably because the page stack is exceeded 10
 more infomation see: https://developers.weixin.qq.com/miniprogram/dev/api/route/wx.navigateTo.html#功能描述
 """
                     )
@@ -767,16 +827,16 @@
     def _on_route_changed(self, message):
         if not message.name == "onAppRouteDone":
             return
         args = message.args
         options = args[0]
         update_time = args[1] if len(args) > 1 else int(time.time() * 1000)
         if (
-            self.route_return_page_update_time
-            and self.route_return_page_update_time > update_time
+            self._route_return_page_update_time
+            and self._route_return_page_update_time > update_time
         ):
             # 旧信息, 丢弃
             return
         self.route_return_page = Page(
             options.webviewId, options.path, options.query, self
         )
         # 记录当前页面
@@ -926,15 +986,14 @@
                     after=method + "_" + super_after.__name__,
                     callback=method + "_" + super_callback.__name__,
                 ),
             )
         except MiniError:
             for stage in stages:
                 self.remove_observer(method + "_" + stage.__name__, stage)
-            stages = []
             raise
 
     def release_hook_wx_method(self, method):
         """
         释放 hook wx 方法
         :param method: 需要释放 hook 的方法
         :return:
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/callback.py` & `minium-1.4.2/minium/miniprogram/base_driver/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,22 +103,22 @@
             return True
         try:
             return self._loop.run_coroutine(
                 async_wait(self._waiter, timeout, self._loop)
             ).result()
         except WaitTimeoutError:
             return False
-        except:
+        except Exception:
             return self._waiter.done()
 
     def get_callback_result(self, timeout=0) -> any:
         if self.wait_called(timeout):
             try:
                 return self._waiter.result()
-            except:
+            except Exception:
                 return sys.exc_info()[1]
         assert self._is_called, f"No callback received within {timeout} seconds"
 
     def get_result(self, timeout=0):
         """
         获取回调结果, 结果如果为exception直接抛出, 超时未获取到则抛MiniTimeoutError
         """
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/connection.py` & `minium-1.4.2/minium/miniprogram/base_driver/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -658,22 +658,27 @@
                     err_msg = ret_json["error"]["message"]
                     if err_msg:  # 生成错误实例
                         self.logger.error(f"[{req_id}]: {err_msg}")
                         if err_msg.find("unimplemented") > 0:
                             self.logger.warn(
                                 f"{err_msg}, It may be caused by the low sdk version"
                             )
-                            ret_json = MiniLowVersionSdkError(err_msg)
+                            ret_json = MiniLowVersionSdkError(err_msg, msg_id=req_id)
                         elif err_msg == "Remote debug connection lost":
                             if self._is_close_app_by_cmd:
                                 # 主动关闭小程序可能会导致丢失链接
                                 ret_json = json2obj('{"id":"%s","result":{}}' % req_id)
-                            raise RemoteDebugConnectionLost(err_msg)
+                            else:
+                                ret_json =  RemoteDebugConnectionLost(err_msg, msg_id=req_id)
+                        elif err_msg == "page destroyed":
+                            ret_json = PageDestroyed(err_msg, msg_id=req_id)
                         else:
-                            ret_json = MiniAppError(err_msg)
+                            ret_json = MiniCommandError(err_msg, msg_id=req_id)
+                    else:
+                        ret_json = MiniCommandError(err_msg, msg_id=req_id)
                 if req_id in self._sync_wait_map:
                     self._sync_wait_map[req_id] = ret_json
                     self._notify()
                 else:
                     self._handle_async_msg(req_id, ret_json)
             else:
                 if "method" in ret_json and ret_json["method"] in self._method_wait_map:
@@ -725,32 +730,29 @@
         else:
             cmd = Command(method, max_timeout=max_timeout)
         if cmd.method in self._method_wait_map and self._method_wait_map.get(
             cmd.method, None
         ):  # 已经有间听到并没被删除（一般只有别的线程同样在等这个方法，但又还没响应才会命中，兜底逻辑）
             return True
         self._method_wait_map[cmd.method] = None
-        try:
-            while cmd.max_timeout > 0:
-                self._wait(cmd)
-                if cmd.method in self._method_wait_map and self._method_wait_map.get(
-                    cmd.method, None
-                ):
-                    del self._method_wait_map[cmd.method]
-                    return True
-                if cmd.is_cancel:
-                    return False
-                if cmd.method.startswith("Tool.") and not self.is_close_conn_by_myself:
-                    continue
-                if self.is_close_by_myself:
-                    return False
-            self.logger.error("Can't wait until %s" % cmd.method)
-            return False
-        finally:
-            del cmd
+        while cmd.max_timeout > 0:
+            self._wait(cmd)
+            if cmd.method in self._method_wait_map and self._method_wait_map.get(
+                cmd.method, None
+            ):
+                del self._method_wait_map[cmd.method]
+                return True
+            if cmd.is_cancel:
+                return False
+            if cmd.method.startswith("Tool.") and not self.is_close_conn_by_myself:
+                continue
+            if self.is_close_by_myself:
+                return False
+        self.logger.error("Can't wait until %s" % cmd.method)
+        return False
 
     def get_aysnc_msg_return(self, msg_id=None):
         if not msg_id:
             self.logger.warning(
                 "Can't get msg without msg_id, you can get msg_id when calling send_async()"
             )
             return None
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/element.py` & `minium-1.4.2/minium/miniprogram/base_driver/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 @Author: lockerzhang
 @LastEditors: lockerzhang
 @Description: 元素相关的操作和信息获取
 @Date: 2019-03-11 14:42:10
 @LastEditTime: 2019-06-06 15:13:32
 """
 from __future__ import annotations
-import code
-from logging import Logger
 import typing
 from minium.framework.exception import MiniElementNotFoundError, MiniTimeoutCauseByConnectionBreakError
 from .minium_object import MiniumObject, RetryableApi
 from ...utils.utils import timeout
 from ...utils.emitter import ee
 import time
 from .prefixer import *
@@ -599,15 +597,15 @@
 
         return self.connection.send(method, params, max_timeout=Command.max_timeout+extra_time)
 
     def _move(self, x_offset, y_offset, move_delay=350, smooth=False):
         offset = self.offset
         size = self.size
         page_offset = self.page_offset
-        changed_touch = touch = ori_changed_touch = ori_touch = {
+        ori_changed_touch = ori_touch = {
             "identifier": 0,
             "pageX": offset["left"] + size["width"] // 2,
             "pageY": offset["top"] + size["height"] // 2,
             "clientX": offset["left"] + size["width"] // 2 - page_offset.x,
             "clientY": offset["top"] + size["height"] // 2 - page_offset.y,
         }
         self._touch_start(touches=[ori_touch], changed_touches=[ori_changed_touch])
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/minium.py` & `minium-1.4.2/minium/miniprogram/base_driver/minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/minium_log.py` & `minium-1.4.2/minium/miniprogram/base_driver/minium_log.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,44 +19,51 @@
 import os
 import time
 import traceback
 from .version import build_version
 from ...framework.exception import MiniError
 
 logging.getLogger("urllib3").setLevel(logging.WARNING)
-# logger = logging.getLogger("DataReport")
+logger = logging.getLogger("minium").getChild("datareport")
 
 REPORT_DOMAIN = "minitest.weixin.qq.com"
 REPORT_PATH = "xbeacon/user_report"
 app_id = None
 version = build_version().get("version")
 revision = build_version().get("revision")
-
+__DEV = os.environ.get("MINIUM_DEV", None)
 class ReportData(dict):
     cmd = ""
 
+    def __eq__(self, __value: object) -> bool:
+        if isinstance(__value, ReportData):
+            return self.dumps() == __value.dumps()
+        return super().__eq__(__value)
+
     def dumps(self):
         return json.dumps(self)
 
-class ExceptionData(dict):
+class ExceptionData(ReportData):
     def __init__(self, err: Exception, **kwargs):
         kwargs["from"] = "minium"
         self.TimeStamp = getattr(err, "timestamp", None) or time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
         self.error = err.__class__.__name__
         self.err_msg = getattr(err, "msg", None) or str(err)
         self.Uin = 0
         self.version = version
         self.revision = revision
         self.ext = ""
         self.app_id = app_id
+        self.msg_id = getattr(err, "msg_id", "")
         self.__dict__.update(kwargs)
         super().__init__(self.__dict__)
         self.cmd = "cloud_exception_log"
 
-class ConsumeData(dict):
+
+class ConsumeData(ReportData):
     def __init__(self, __map: dict, **kwargs):
         self.version = version
         self.revision = revision
         self.app_id = app_id
         self.time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         __map.update(kwargs)
         self.__dict__.update(__map)
@@ -65,15 +72,15 @@
 
 def process_report():
     global existFlag
     while not existFlag:
         lock.acquire()
         lock.wait(10)
         lock.release()
-        if not report_queue.empty():
+        while not report_queue.empty():
             data = report_queue.get()
             # logger.debug("Thread processing report data %s" % data)
             report(data=data)
 
 
 def report_fail(failed=True):
     global fail, existFlag
@@ -96,38 +103,43 @@
 
 def report(data: ReportData):
     """
     report minium_new
     """
     if existFlag:
         return
-    print(f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}")
-    print(data)
+    # print(f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}")
+    # print(data)
+    if __DEV:
+        logger.debug(f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}")
+        logger.debug(data.dumps())
     try:
         ret = requests.post(
             url=f"https://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}",
             data=data.dumps(),
             timeout=10,
         )
-        # logger.debug(ret.text)
+        if __DEV:
+            logger.debug(ret.text)
         report_fail(ret.status_code != 200)
     except Exception as e:
         # logger.debug("data report fail with https")
         try:
             ret = requests.post(
                 url=f"http://{REPORT_DOMAIN}/{REPORT_PATH}/{data.cmd}",
                 data=data.dumps(),
                 timeout=10,
             )
-            # logger.debug(ret.text)
+            if __DEV:
+                logger.debug(ret.text)
             report_fail(ret.status_code != 200)
         except Exception as e:
             # logger.error("data report fail with http, give up")
-            # logger.exception(e)
-            pass
+            if __DEV:
+                logger.exception(e)
 
 
 # logger.debug(ret.text)
 
 
 existFlag = 0
 fail = 0
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/minium_object.py` & `minium-1.4.2/minium/miniprogram/base_driver/minium_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Author:         lockerzhang
 Filename:       minium_object.py
 Create time:    2019/4/30 21:21
 Description:
 
 """
 
-from .minium_log import MonitorMetaClass
+from .minium_log import MonitorMetaClass, report_exception, ExceptionData
 from .callback import Callback
 from .connection import Command, Connection
 from ...utils.injectjs import getInjectJsCode
 from ...utils.utils import retry
 from ...framework.exception import *
 import subprocess
 import time
@@ -24,33 +24,48 @@
 
 class RetryableApi(MonitorMetaClass):
     """
     给attr_dict["__RETRY_API__"]中的接口(包括property.fget)添加retry修饰器
     __RETRY_CNT__: 接口重试次数, 默认2
     __RETRY_EXCEPTION__: 命中给定错误才重试, 默认(MiniTimeoutCauseByConnectionBreakError, MiniTimeoutCauseByClientOffline)
     """
+
     def __new__(mcs, cls_name, bases, attr_dict):
         if "__RETRY_API__" in attr_dict:
             if "__RETRY_CNT__" not in attr_dict:
                 attr_dict["__RETRY_CNT__"] = 2
             RETRY_CNT = attr_dict["__RETRY_CNT__"]
             if "__RETRY_EXCEPTION__" not in attr_dict:
-                attr_dict["__RETRY_EXCEPTION__"] = (MiniTimeoutCauseByConnectionBreakError, MiniTimeoutCauseByClientOffline)
+                attr_dict["__RETRY_EXCEPTION__"] = (
+                    MiniTimeoutCauseByConnectionBreakError,
+                    MiniTimeoutCauseByClientOffline,
+                )
             RETRY_EXCEPTION = attr_dict["__RETRY_EXCEPTION__"]
             for api in attr_dict["__RETRY_API__"]:
                 if api.startswith("__"):  # private method
                     api = f"_{cls_name}{api}"
                 if api not in attr_dict:
                     continue
                 if isinstance(attr_dict[api], property):
                     if attr_dict[api].fget:
-                        attr_dict[api] = property(retry(2, ValueError)(attr_dict[api].fget), attr_dict[api].fset, attr_dict[api].fdel, attr_dict[api].__doc__)
+                        attr_dict[api] = property(
+                            retry(2, ValueError)(attr_dict[api].fget),
+                            attr_dict[api].fset,
+                            attr_dict[api].fdel,
+                            attr_dict[api].__doc__,
+                        )
                 if not isinstance(attr_dict[api], types.FunctionType):
                     continue
-                attr_dict[api] = retry(RETRY_CNT, RETRY_EXCEPTION)(attr_dict[api])
+                attr_dict[api] = retry(
+                    RETRY_CNT,
+                    RETRY_EXCEPTION,
+                    lambda cnt, name: report_exception(
+                        ExceptionData(RetrySuccess(f"{cls_name}.{api}"), func=name, retry=cnt - 1)
+                    ),
+                )(attr_dict[api])
         return super().__new__(mcs, cls_name, bases, attr_dict)
 
 
 class MiniumObject(object, metaclass=MonitorMetaClass):
     _cant_use_interface = {}
 
     def __init__(self):
@@ -112,15 +127,17 @@
         timeout = timeout or interval
         while time.time() - s < timeout:
             if func():
                 return True
             time.sleep(interval)
         return False
 
-    def _call_wx_method(self, method, args=None, plugin_appid=None, sync=True, ignore_response=False):
+    def _call_wx_method(
+        self, method, args=None, plugin_appid=None, sync=True, ignore_response=False
+    ):
         if args is None:
             args = []
         if not isinstance(args, list):
             if isinstance(args, str):
                 # 如果是字符型参数，就可以不用管是否是 sync 方法，直接转数组传参即可
                 args = [args]
             elif "Sync" in method:
@@ -134,15 +151,17 @@
                 # 异步方法的话无需管 args 是str 还是 dict，直接转成 list 即可
                 args = [args]
 
         params = {"method": method, "args": args}
         if plugin_appid:
             params["pluginId"] = plugin_appid
         if not sync:
-            return self.connection.send_async("App.callWxMethod", params, ignore_response=ignore_response)
+            return self.connection.send_async(
+                "App.callWxMethod", params, ignore_response=ignore_response
+            )
         return self.connection.send("App.callWxMethod", params)
 
     def _evaluate(self, app_function: str, args=None, sync=False, desc=None):
         if not args:
             args = []
         if sync:
             return self.connection.send(
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/page.py` & `minium-1.4.2/minium/miniprogram/base_driver/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,25 +322,23 @@
             return True
         elif isinstance(condition, str):
             while (time.time() - s_time) < max_timeout:
                 if self._element_is_exists(condition):
                     return True
                 else:
                     time.sleep(0.25)
-            else:
-                return False
+            return False
         elif hasattr(condition, "__call__"):
             while (time.time() - s_time) < max_timeout:
                 res = condition()
                 if res:
                     return True
                 else:
                     time.sleep(0.25)
-            else:
-                return False
+            return False
 
     def get_elements(
         self,
         selector,
         max_timeout=0,
         inner_text=None,
         text_contains=None,
```

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/prefixer.py` & `minium-1.4.2/minium/miniprogram/base_driver/prefixer.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/miniprogram/base_driver/version.py` & `minium-1.4.2/minium/miniprogram/base_driver/version.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/miniprogram/qq_minium.py` & `minium-1.4.2/minium/miniprogram/qq_minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/miniprogram/wx_minium.py` & `minium-1.4.2/minium/miniprogram/wx_minium.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,14 +660,16 @@
             try:
                 self.logger.info("Trying to connect Dev tool ...")
                 self.connection = Connection.create(
                     self.uri, timeout=self.conf.get("request_timeout")
                 )
                 self.__get_dev_tool_info()
                 self._get_system_info()
+                if self.app:
+                    self.app.release()  # 释放上一个
                 self.app = App(
                     self.connection,
                     self.conf.get("auto_relaunch"),
                     native=self.native,
                     platform=self.platform,
                 )
                 ee.on("ide_closed", self._relaunch_ide)
@@ -805,14 +807,16 @@
                             self.connection.send(
                                 "Tool.enableRemoteDebug",
                                 params={"auto": False},
                                 max_timeout=connect_timeout,
                             )
             # 远程调试开启成功后，小程序运行态已经转到手机，需要重新实例化app
             self._get_system_info()
+            if self.app:
+                self.app.release()  # 释放上一个
             self.app = App(
                 self.connection,
                 self.conf.get("auto_relaunch"),
                 native=self.native,
                 platform=self.platform,
             )
             setattr(self.connection, "_is_close_app_by_cmd", False)  # 重新拉起重置一下
```

### Comparing `minium-1.4.1/minium/native/__init__.py` & `minium-1.4.2/minium/native/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/android_base/__init__.py` & `minium-1.4.2/minium/native/lib/android_base/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/__init__.py` & `minium-1.4.2/minium/native/lib/at/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/apkapi.py` & `minium-1.4.2/minium/native/lib/at/apkapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/atproxy.py` & `minium-1.4.2/minium/native/lib/at/atproxy.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/bin/AtServer.apk` & `minium-1.4.2/minium/native/lib/at/bin/AtServer.apk`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/bin/AtStub.jar` & `minium-1.4.2/minium/native/lib/at/bin/AtStub.jar`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/command_line.py` & `minium-1.4.2/minium/native/lib/at/command_line.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/accesshelper.py` & `minium-1.4.2/minium/native/lib/at/core/accesshelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/adbwrap.py` & `minium-1.4.2/minium/native/lib/at/core/adbwrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         self._has_call_back = False
         serial_ids = get_device_ids()
         logger.info(str(serial_ids))
         if serial is None:
             self._serial = self.get_default_serial()
         if serial is not None and serial not in serial_ids:
             logger.error("可用手机:%s, '%s'不可用", serial_ids, serial)
-            raise AdbDisconnectedError(u"手机可用:"+serial)
+            raise AdbDisconnectedError(u"手机不可用:"+serial)
         if self._serial is None and self.kv is None:
             self._serial_kv['none'] = {}
         elif self._serial is not None and self.kv is None:
             self._serial_kv[self._serial] = {}
 
     def check_connected(self):
         self.run_adb("shell echo 1")
@@ -653,15 +653,15 @@
 
     def get_current_active_process(self, reg_exp):
         """
         grep top 5 process, and return process match {reg_exp}
         :return: process_name, pid
         """
         output = self.run_shell("COLUMNS=512 top -m 5 -n 2 -d 2")
-        lines = [line.strip() for line in output.split("\n")]
+        lines = [re.sub(r"\x1B[^m]*m", "", line.strip()) for line in output.split("\n")]
         for output2 in lines:
             r = re.compile("(%s)" % reg_exp)
             m = r.search(output2)
             if m:
                 pid = output2.split()[0]
                 m_name = m.group(1)
                 return (m_name, pid)
```

### Comparing `minium-1.4.1/minium/native/lib/at/core/basedriver.py` & `minium-1.4.2/minium/native/lib/at/core/basedriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/case_repair_adapter.py` & `minium-1.4.2/minium/native/lib/at/core/case_repair_adapter.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/config.py` & `minium-1.4.2/minium/native/lib/at/core/config.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/element.py` & `minium-1.4.2/minium/native/lib/at/core/element.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/exceptions.py` & `minium-1.4.2/minium/native/lib/at/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/javadriver.py` & `minium-1.4.2/minium/native/lib/at/core/javadriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/resguard.py` & `minium-1.4.2/minium/native/lib/at/core/resguard.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/stf/mincap.py` & `minium-1.4.2/minium/native/lib/at/core/stf/mincap.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/stf/minitouch.py` & `minium-1.4.2/minium/native/lib/at/core/stf/minitouch.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/uidevice.py` & `minium-1.4.2/minium/native/lib/at/core/uidevice.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/uixml.py` & `minium-1.4.2/minium/native/lib/at/core/uixml.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/core/websocketcli.py` & `minium-1.4.2/minium/native/lib/at/core/websocketcli.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/eventmonitor.py` & `minium-1.4.2/minium/native/lib/at/eventmonitor.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/hook.py` & `minium-1.4.2/minium/native/lib/at/hook.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/jlogcat.py` & `minium-1.4.2/minium/native/lib/at/jlogcat.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/keycode.py` & `minium-1.4.2/minium/native/lib/at/keycode.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/perfcollector.py` & `minium-1.4.2/minium/native/lib/at/perfcollector.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/AtEvent.py` & `minium-1.4.2/minium/native/lib/at/tests/AtEvent.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/atdevicetest.py` & `minium-1.4.2/minium/native/lib/at/tests/atdevicetest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/drivertest.py` & `minium-1.4.2/minium/native/lib/at/tests/drivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/elementtest.py` & `minium-1.4.2/minium/native/lib/at/tests/elementtest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/images/1.jpg` & `minium-1.4.2/minium/native/lib/at/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/images/2.jpg` & `minium-1.4.2/minium/native/lib/at/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/images/image.jpg` & `minium-1.4.2/minium/native/lib/at/tests/images/image.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/minitouch_test.py` & `minium-1.4.2/minium/native/lib/at/tests/minitouch_test.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/u2test.py` & `minium-1.4.2/minium/native/lib/at/tests/u2test.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/uixmltest.py` & `minium-1.4.2/minium/native/lib/at/tests/uixmltest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/tests/webdrivertest.py` & `minium-1.4.2/minium/native/lib/at/tests/webdrivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/apkinfo.py` & `minium-1.4.2/minium/native/lib/at/utils/apkinfo.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/axmlparser.py` & `minium-1.4.2/minium/native/lib/at/utils/axmlparser.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/axmlparser3.py` & `minium-1.4.2/minium/native/lib/at/utils/axmlparser3.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/commonhelper.py` & `minium-1.4.2/minium/native/lib/at/utils/commonhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/decorator.py` & `minium-1.4.2/minium/native/lib/at/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/nbsp.py` & `minium-1.4.2/minium/native/lib/at/utils/nbsp.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/utils/threadhelper.py` & `minium-1.4.2/minium/native/lib/at/utils/threadhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/driver.py` & `minium-1.4.2/minium/native/lib/at/webdriver/driver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/jsapi.py` & `minium-1.4.2/minium/native/lib/at/webdriver/jsapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/miniapp.py` & `minium-1.4.2/minium/native/lib/at/webdriver/miniapp.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/stub.js` & `minium-1.4.2/minium/native/lib/at/webdriver/stub.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/tabdescription.py` & `minium-1.4.2/minium/native/lib/at/webdriver/tabdescription.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/tabwebsocket.py` & `minium-1.4.2/minium/native/lib/at/webdriver/tabwebsocket.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/webelement.py` & `minium-1.4.2/minium/native/lib/at/webdriver/webelement.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/webhelper.py` & `minium-1.4.2/minium/native/lib/at/webdriver/webhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/webdriver/wspools.py` & `minium-1.4.2/minium/native/lib/at/webdriver/wspools.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/at/wechat/activtiy.py` & `minium-1.4.2/minium/native/lib/at/wechat/activtiy.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/case_repair_sdk/__init__.py` & `minium-1.4.2/minium/native/lib/case_repair_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/case_repair_sdk/default_trace.py` & `minium-1.4.2/minium/native/lib/case_repair_sdk/default_trace.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/wda/__init__.py` & `minium-1.4.2/minium/native/lib/wda/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/wda/screenhelper.py` & `minium-1.4.2/minium/native/lib/wda/screenhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/wda/xcui_element_types.py` & `minium-1.4.2/minium/native/lib/wda/xcui_element_types.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/wx_wda/wdaUI.py` & `minium-1.4.2/minium/native/lib/wx_wda/wdaUI.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/lib/wx_wda/webDriverTool.py` & `minium-1.4.2/minium/native/lib/wx_wda/webDriverTool.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/qq_native/qandroidnative.py` & `minium-1.4.2/minium/native/qq_native/qandroidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/native/qq_native/qiosnative.py` & `minium-1.4.2/minium/native/qq_native/qiosnative.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import sys
 import os
 
 lib_path = os.path.abspath(os.path.join(".."))
 # print(lib_path)
 sys.path.append(lib_path)
 
-import requests
-import wda
-from minium.native.qq_native.qbasenative import QBaseNative, NativeError
+from minium.native.qq_native.qbasenative import QBaseNative
 from minium.native.lib.wx_wda import *
 from urllib.parse import quote
 
 
 class QiOSNative(QBaseNative):
     def __init__(self, json_conf):
         super(QiOSNative, self).__init__(json_conf)
@@ -105,15 +103,15 @@
         :param names: 传入一个 list 选择多张照片或者视频(照片和视频不能同时选择, 且图片最多 9 张, 视频一次只能选择一个)
         :param media_type: photo 或者 video
         :param duration: 拍摄时长
         :param original: 是否选择原图(仅图片)
         :return:
         """
         if cap_type == "album" and names is None:
-            Exception("从相册选择照片必须提供照片名称, 可以通过 wda inspector 查看照片名称")
+            raise Exception("从相册选择照片必须提供照片名称, 可以通过 wda inspector 查看照片名称")
         if cap_type == "camera":
             self._capture_photo(media_type=media_type, duration=duration)
         elif cap_type == "album":
             if media_type == "photo":
                 if isinstance(names, str):
                     names = [names]
                 self._select_photos_from_album(names=names, original=original)
```

### Comparing `minium-1.4.1/minium/native/wx_native/androidnative.py` & `minium-1.4.2/minium/native/wx_native/androidnative.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-22
 import os.path
 import time
 
 from minium.utils.utils import timeout, wait
-from .basenative import BaseNative, NativeError, ResetError, ModalStatus
+from .basenative import BaseNative, NativeError, ModalStatus
 import at
 from at.core.adbwrap import AdbWrap
 from at.core.element import Element as ATElement, AtSelector
 import at.keycode
 import json
 import logging
 import threading
 import shutil
 import ssl
 import requests
 import re
-from enum import Enum
 from ..lib.android_base import UiDefine, ScreenType
 from .wording import Language, WORDING
 
 ssl._create_default_https_context = ssl._create_unverified_context
 
 WECHAT_PACKAGE = "com.tencent.mm"
 WECHAT_ACTIVITY = "ui.LauncherUI"
@@ -43,15 +42,14 @@
         self.at = at.At(self.serial)
         self.at.java_driver.set_capture_op(False)
         self.ui = UiDefine(self.at)
         self.lang = json_conf.get("lang")
         self.perf_thread = None
         self.perf_flag = False
         self.ef_able_flag = False
-        self.perf_data = []
         self.fps_data_dict = {}  # fps dict
         self.jank_count_dict = {}  # 卡顿次数
         self.fps_thread = None
         self.startup_time = 0
         self.outputs = json_conf.get("outputs") or os.path.dirname(
             os.path.realpath(__file__)
         )
@@ -409,15 +407,15 @@
     def call_phone(self):
         pass
 
     def handle_picker(self, *items):
         instance = 0
         for item in items:
             input_elem = self.ui.comp_picker_input.instance(instance)
-            next_elem = input_elem.parent().child("android.widget.Button")
+            # next_elem = input_elem.parent().child("android.widget.Button")
             first_text = input_elem.get_text()
             while True:
                 # todo: 要判断上滑还是下滑
                 current_text = input_elem.get_text()
                 if current_text == str(item):
                     break
                 if first_text == str(item):
@@ -505,17 +503,16 @@
             try:
                 if el1.exists(timeout):
                     el1.click()
                 elif el2.exists(timeout):
                     el2.click()
                 else:
                     break
-            except:
+            except Exception:
                 logger.exception("返回 failed")
-                pass
 
     def stop_wechat(self):
         self.at.adb.stop_app(WECHAT_PACKAGE)
 
     def click_coordinate(self, x, y):
         self.at.adb.click_point(x, y)
 
@@ -523,17 +520,15 @@
         """
         Alias for click_coordinate
         """
         return self.click_coordinate(x, y)
 
     def _get_mem_used_new(self, pkg_name, pid):
         used = 0
-        i = 0
         m = None
-        m1 = None
         m2 = None
         cmd = "dumpsys meminfo %s" % pkg_name
         # logger.info(cmd)
         output_mem = self.at.adb.run_shell(cmd)
         # logger.info(output_mem)
         r = re.compile(r"TOTAL\s+(\d+)")
 
@@ -733,15 +728,15 @@
             else:
                 break
         if processname and curview:
             try:
                 self.perf_data = []
                 self.write_perf_data(processname, pid, curview, timeinterval)
                 return self.perf_flag
-            except:
+            except Exception:
                 self.perf_flag = False
                 return self.perf_flag
         else:
             self.perf_flag = False
             return self.perf_flag
 
     def start_get_perf(self, timeinterval=15):
@@ -769,15 +764,15 @@
 
     def get_pay_value(self):
         try:
             if self.e.text_contains("￥").exists():
                 return self.e.text_contains("￥").get_text()
             else:
                 return ""
-        except:
+        except Exception:
             return ""
 
     def _check_pay_modal_version(self):
         if not self.pay_modal_version:  # 先检测版本
             self._get_current_views()
             if self._el_exist_in_current_view(
                 self.e.rid("com.tencent.mm:id/tenpay_keyboard_0")
@@ -841,15 +836,15 @@
 
     def get_system_info(self):
         return self.at.adb.desc
 
     def _press_back(self):
         try:
             self.at.adb.press_key_code(at.keycode.KEYCODE_BACK)
-        except:
+        except Exception:
             return False
         return True
 
     def is_app_in_foreground(self, appid):
         # exists text like appid:page_path:VISIBLE
         return self.e.text_contains(text=appid).exists(0.5)
```

### Comparing `minium-1.4.1/minium/native/wx_native/basenative.py` & `minium-1.4.2/minium/native/wx_native/basenative.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import shutil
 import json
 import threading
 import types
 import typing
 from functools import wraps
 
-from minium.utils.utils import timeout
 from ..exception import *
 from ...utils.emitter import ee
 from .wording import Language, WORDING
 
 logger = logging.getLogger("minium")
```

### Comparing `minium-1.4.1/minium/native/wx_native/idenative.py` & `minium-1.4.2/minium/native/wx_native/idenative.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-06-11
-from .basenative import BaseNative, NativeError, logger
+from .basenative import BaseNative, logger
 from ...utils.utils import Version
 from ...framework.exception import MiniLaunchError
 
 class IdeNative(BaseNative):
     _mini = None  # ide的native操作也以来minium的实例，可能引起循环引用，需要谨慎处理
 
     def __init__(self, json_conf, mini=None):
@@ -28,26 +28,26 @@
         if self._mini == value:
             return
         self._mini = value
         if value is not None and getattr(self._mini, "connection"):
             self.__get_dev_tool_info()
 
     def start_wechat(self):
-        ...
+        pass
 
     def stop_wechat(self):
         ...
 
     def connect_weapp(self, path):
         ...
 
     def __get_dev_tool_info(self):
         try:
             result = self._mini.connection.send("Tool.getInfo", max_timeout=3).result
-        except:
+        except Exception:
             # not support Tool.getInfo
             return
         if Version(result.SDKVersion) < Version("2.7.3"):
             raise MiniLaunchError("基础库版本[%s]过低，请确认基础库版本>=2.7.3" % self.sdk_version)
         if str(result.version).endswith("2") and Version(result.version) >= "1.06.2211072":  # nightly
             self.use_native = True
         elif str(result.version).endswith("1") and Version(result.version) >= "1.06.2212011":  # RC
```

### Comparing `minium-1.4.1/minium/native/wx_native/iosnative.py` & `minium-1.4.2/minium/native/wx_native/iosnative.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         # 使用tidevice
         self.wda_bundle = json_conf.get("wda_bundle", None)
         # 目标app实例
         self.app = None
         # 获取性能的实例
         self.perf_flag = False
         self.perf = None
-        self.perf_data = []
         self.last_cpu = 0
         self.last_fps = 0
         self.last_mem = 0
         # 健康弹窗处理
         self.health_modal_handle_thread = None
         self.stop_check = True
         self.check_done = True
@@ -134,35 +133,14 @@
                 self.wda_runner.start_driver()
 
     def connect_weapp(self, path):
         """
         有push的方式, 理应可以废掉
         """
         raise NotImplementedError("ios不再支持长按识别二维码的方式，请使用推送方式调用")
-        filename = "remote_debug.jpg"
-        r = requests.post(
-            "https://stream.weixin.qq.com/weapp/UploadFile",
-            files={filename: (filename, open(path, "rb"))},
-        )
-        if r.status_code != 200:
-            logger.error(r.text)
-            r.raise_for_status()
-
-        url = "https://stream.weixin.qq.com/weapp/GetQRCodePage?file_name={0}".format(
-            filename
-        )
-        self.app.session(class_name="Button", text="通讯录").click(timeout=10.0)
-        self.app.session(class_name="SearchField", text="搜索").set_text("文件传输助手")
-        self.app.session(xpath="//Table[1]/Cell[2]/Button[1]").click(timeout=10)
-        self.app.session(class_name="TextView").set_text(url + "\n")
-        self.app.session(class_name="Other", partial_text=url)[-1].click(timeout=10.0)
-        self.app.session(class_name="WebView").subelems(
-            class_name="Other", text="小程序web view测试"
-        ).subelems(class_name="Image").tap_hold(3.0)
-        self.app.session(partial_text="识别图中二维码").click(timeout=10.0)
 
     def screen_shot(self, filename: str, return_format: str = "raw") -> object:
         """
         截图
         :param filename: 文件存放的路径
         :param return_format: 除了将截图保存在本地之外, 需要返回的图片内容格式: raw(default) or pillow
         :return: raw data or PIL.Image
```

### Comparing `minium-1.4.1/minium/native/wx_native/wording.py` & `minium-1.4.2/minium/native/wx_native/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/emitter.py` & `minium-1.4.2/minium/utils/emitter.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/injectjs.py` & `minium-1.4.2/minium/utils/injectjs.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/createContext.js` & `minium-1.4.2/minium/utils/js/es5/createContext.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/getUni.js` & `minium-1.4.2/minium/utils/js/es5/getUni.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/helpers.js` & `minium-1.4.2/minium/utils/js/es5/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/hookWxMethod.js` & `minium-1.4.2/minium/utils/js/es5/hookWxMethod.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 function hookWxMethod() {
-    var a;
-    wx.$_origin_$ ? a = wx.$_origin_$ : (a = wx.$_method_$, Object.defineProperty(wx, "$_origin_$", {
+    var a, b = wx._MINI_WX_PROXY_ || wx;
+    b.$_origin_$ ? a = b.$_origin_$ : (a = b.$_method_$, Object.defineProperty(b, "$_origin_$", {
         configurable: !0,
         get: function get() {
             return a
         }
-    })), Object.defineProperty(wx, "$_method_$", {
+    })), Object.defineProperty(b, "$_method_$", {
         configurable: !0,
         get: function get() {
             return function() {
                 var b = 0 >= arguments.length ? void 0 : arguments[0],
                     c = !1;
                 "$_method_$".endsWith("Sync") || b && (b.success || b.fail || b.complete) || (c = !0), "undefined" != typeof $_before_$ && $_before_$.apply(void 0, arguments);
                 var d;
```

### Comparing `minium-1.4.1/minium/utils/js/es5/ideMockChooseLocation.js` & `minium-1.4.2/minium/utils/js/es5/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/ideMockGetLocation.js` & `minium-1.4.2/minium/utils/js/es5/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/ideMockGetWeRunData.js` & `minium-1.4.2/minium/utils/js/es5/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/ideMockModal.js` & `minium-1.4.2/minium/utils/js/es5/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/mockChooseImage.js` & `minium-1.4.2/minium/utils/js/es5/mockChooseImage.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,97 +1,102 @@
 function mockChooseImage() {
     var a = wx.getFileSystemManager();
     if (!global.__minium_mock_choose_image) {
-        var b = function rewriteChooseImage(a, b) {
-                function d() {
-                    c && (c = !1, h.forEach(function(b) {
-                        f[b] ? f[b].get ? Object.defineProperty(a, b, {
-                            configurable: !0,
-                            get: function get() {
-                                return e[b]
-                            }
-                        }) : Object.defineProperty(a, b, {
-                            writable: !0,
-                            value: e[b]
-                        }) : a[b] = e[b]
-                    }))
-                }
-                if (c) return !1;
-                c = !0;
-                var e = {},
-                    f = {},
-                    g = {
+        var b = function() {
+                e.forEach(function(a) {
+                    a()
+                })
+            },
+            c = function(a, c) {
+                if (d.get(a)) return !1;
+                d.set(a, !0);
+                var f = {},
+                    g = {},
+                    h = {
                         chooseImage: function chooseImage(a) {
-                            d();
-                            var c = {
+                            b();
+                            var d = {
                                 errMsg: "chooseImage:ok",
-                                tempFilePaths: b.map(function(a) {
+                                tempFilePaths: c.map(function(a) {
                                     return a.filePath
                                 }),
-                                tempFiles: b.map(function(a) {
+                                tempFiles: c.map(function(a) {
                                     return {
                                         path: a.filePath,
                                         size: a.size
                                     }
                                 })
                             };
-                            return a.success || a.fail || a.complete ? void(a.success && a.success(c), a.complete && a.complete(c)) : Promise.resolve(c)
+                            return a.success || a.fail || a.complete ? void(a.success && a.success(d), a.complete && a.complete(d)) : Promise.resolve(d)
                         },
                         chooseMedia: function chooseMedia(a) {
-                            d();
-                            var c = {
+                            b();
+                            var d = {
                                 errMsg: "chooseMedia:ok",
-                                tempFiles: b.map(function(a) {
+                                tempFiles: c.map(function(a) {
                                     return {
                                         tempFilePath: a.filePath,
                                         size: a.size,
                                         fileType: "image"
                                     }
                                 }),
                                 type: "image"
                             };
-                            return a.success || a.fail || a.complete ? void(a.success && a.success(c), a.complete && a.complete(c)) : Promise.resolve(c)
+                            return a.success || a.fail || a.complete ? void(a.success && a.success(d), a.complete && a.complete(d)) : Promise.resolve(d)
                         },
                         createCameraContext: function createCameraContext() {
-                            var a = e.createCameraContext(),
-                                f = a.takePhoto;
-                            return Object.defineProperty(a, "takePhoto", {
+                            var e = f.createCameraContext(),
+                                g = e.takePhoto;
+                            return Object.defineProperty(e, "takePhoto", {
                                 configurable: !0,
                                 get: function get() {
-                                    return function(a) {
-                                        if (!c) return f.call(this, a);
-                                        d();
-                                        var e = {
-                                            tempImagePath: b[0].filePath,
+                                    return function(e) {
+                                        if (!d.get(a)) return g.call(this, e);
+                                        b();
+                                        var f = {
+                                            tempImagePath: c[0].filePath,
                                             errMsg: "takePhoto:ok"
                                         };
-                                        a.success && a.success(e), a.complete && a.complete(e)
+                                        e.success && e.success(f), e.complete && e.complete(f)
                                     }
                                 }
-                            }), a
+                            }), e
                         }
                     },
-                    h = Object.keys(g);
-                return h.forEach(function(b) {
-                    e[b] = a[b], f[b] = Object.getOwnPropertyDescriptor(a, b)
-                }), h.forEach(function(b) {
-                    f[b] ? f[b].get ? Object.defineProperty(a, b, {
+                    i = Object.keys(h);
+                return i.forEach(function(b) {
+                    f[b] = a[b], g[b] = Object.getOwnPropertyDescriptor(a, b)
+                }), e.set(a, function() {
+                    d.get(a) && (console.debug("release target"), d.set(a, !1), i.forEach(function(b) {
+                        g[b] ? g[b].get ? Object.defineProperty(a, b, {
+                            configurable: !0,
+                            get: function get() {
+                                return f[b]
+                            }
+                        }) : Object.defineProperty(a, b, {
+                            writable: !0,
+                            value: f[b]
+                        }) : a[b] = f[b]
+                    }))
+                }), i.forEach(function(b) {
+                    g[b] ? g[b].get ? Object.defineProperty(a, b, {
                         configurable: !0,
                         get: function get() {
-                            return g[b]
+                            return h[b]
                         }
                     }) : Object.defineProperty(a, b, {
                         writable: !0,
-                        value: g[b]
-                    }) : a[b] = g[b]
+                        value: h[b]
+                    }) : a[b] = h[b]
                 }), !0
             },
-            c = !1;
+            d = new Map,
+            e = new Map;
         global.__minium_mock_choose_image = function() {
-            for (var c = arguments.length, d = Array(c), e = 0; e < c; e++) d[e] = arguments[e];
+            for (var b = arguments.length, d = Array(b), e = 0; e < b; e++) d[e] = arguments[e];
             var f = d.map(function(b) {
                 var c = b.imageData,
                     d = b.imageName,
                     e = b.size,
                     f = "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP/").concat(d);
                 return c && 0 !== c.length ? new Promise(function(b, e) {
                     a.writeFile({
@@ -119,109 +124,108 @@
                 }) : Promise.resolve({
                     imageName: d,
                     filePath: f,
                     size: e
                 })
             });
             return Promise.all(f).then(function(a) {
-                return b(wx, a), a.map(function(a) {
+                return c(wx, a), wx._MINI_WX_PROXY_ && c(wx._MINI_WX_PROXY_, a), a.map(function(a) {
                     return {
                         name: a.imageName,
                         size: a.size
                     }
                 })
             })
         };
-        var d = !1;
+        var f = !1;
         a.mkdir({
             dirPath: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE"),
             recursive: !1,
             success: function success() {
-                d = !0
+                f = !0
             },
             fail: function fail(a) {
                 var b = a.errMsg;
-                0 <= b.indexOf("file already exists") && (d = !0)
+                0 <= b.indexOf("file already exists") && (f = !0)
             }
         });
-        var e = a.saveFile,
-            f = a.saveFileSync,
-            g = a.getSavedFileList;
+        var g = a.saveFile,
+            h = a.saveFileSync,
+            i = a.getSavedFileList;
         Object.defineProperty(a, "saveFile", {
             configurable: !0,
             get: function get() {
                 return function(b) {
                     var c = b.tempFilePath,
                         d = b.filePath,
-                        f = b.success,
-                        g = b.fail,
+                        e = b.success,
+                        f = b.fail,
                         h = b.complete;
                     if (c.startsWith("".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP"))) {
                         var i = {
                             srcPath: c,
                             destPath: d || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(c.split("/").pop())
                         };
-                        return f && (i.success = function(a) {
-                            a.errMsg = a.errMsg.replace("copyFile", "saveFile"), a.savedFilePath = i.destPath, f(a)
-                        }), g && (i.fail = function(a) {
-                            a.errMsg = a.errMsg.replace("copyFile", "saveFile"), g(a)
+                        return e && (i.success = function(a) {
+                            a.errMsg = a.errMsg.replace("copyFile", "saveFile"), a.savedFilePath = i.destPath, e(a)
+                        }), f && (i.fail = function(a) {
+                            a.errMsg = a.errMsg.replace("copyFile", "saveFile"), f(a)
                         }), h && (i.complete = function(a) {
                             a.errMsg = a.errMsg.replace("copyFile", "saveFile"), 0 === a.errMsg.indexOf("saveFile:ok") && (a.savedFilePath = i.destPath), h(a)
                         }), a.copyFile(i)
                     }
-                    return e({
+                    return g({
                         tempFilePath: c,
                         filePath: d,
-                        success: f,
-                        fail: g,
+                        success: e,
+                        fail: f,
                         complete: h
                     })
                 }
             }
         }), Object.defineProperty(a, "saveFileSync", {
             configurable: !0,
             get: function get() {
                 return function(b, c) {
                     if (b.startsWith("".concat(wx.env.USER_DATA_PATH, "/.MINIUM_TMP"))) {
-                        var d = b,
-                            e = c || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(b.split("/").pop());
+                        var d = c || "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(b.split("/").pop());
                         try {
-                            return a.copyFileSync(d, e), e
+                            return a.copyFileSync(b, d), d
                         } catch (a) {
                             throw a.message.replace("copyFileSync", "saveFileSync")
                         }
                     }
-                    return f(b, c)
+                    return h(b, c)
                 }
             }
         }), Object.defineProperty(a, "getSavedFileList", {
             configurable: !0,
             get: function get() {
                 return function(b) {
                     var c = b.success,
                         d = b.complete;
                     Promise.all([new Promise(function(b) {
                         a.stat({
                             path: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/"),
                             recursive: !0,
-                            complete: function complete(a) {
+                            complete: function(a) {
                                 b((a.stats || []).filter(function(a) {
                                     return "/" !== a.path
                                 }).map(function(a) {
                                     return {
                                         filePath: "".concat(wx.env.USER_DATA_PATH, "/.MINIUM_STORE/").concat(a.path.startsWith("/") ? a.path.slice(1) : a.path),
                                         size: a.stats.size,
                                         createTime: a.stats.lastModifiedTime
                                     }
                                 }))
                             }
                         })
                     }), new Promise(function(a) {
-                        g({
-                            complete: function complete(b) {
+                        i({
+                            complete: function(b) {
                                 a(b.fileList || [])
                             }
                         })
                     })]).then(function(a) {
                         var b = global.babelHelpers.slicedToArray(a, 2),
                             e = b[0],
                             f = b[1],
```

### Comparing `minium-1.4.1/minium/utils/js/es5/mockCloudCall.js` & `minium-1.4.2/minium/utils/js/es5/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/mockNetwork.js` & `minium-1.4.2/minium/utils/js/es5/mockNetwork.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -75,32 +75,33 @@
             }, {
                 key: "onProgressUpdate",
                 value: function onProgressUpdate(a) {
                     this.progressUpdateCallback.push(a)
                 }
             }]), a
         }();
-        var b = wx["%(interface)s"];
-        Object.defineProperty(wx, "%(interface)s", {
+        var b = wx._MINI_WX_PROXY_ || wx,
+            c = b["%(interface)s"];
+        Object.defineProperty(b, "%(interface)s", {
             configurable: !0,
             get: function get() {
-                return function(c) {
+                return function(b) {
                     for (var d, e = 0; e < global["__minium_%(interface)s_network_mock_rule"].length; e++)
-                        if (d = global["__minium_%(interface)s_network_mock_rule"][e], a(d, c)) {
+                        if (d = global["__minium_%(interface)s_network_mock_rule"][e], a(d, b)) {
                             if (1 === d._miniMockType) {
                                 var f = global["__minium_%(interface)s_network_mock_rule"].splice(e, 1),
                                     g = global.babelHelpers.slicedToArray(f, 1);
                                 d = g[0]
                             }
-                            if (console.log("@@@@rule match", d), c.__miniumMocked = !0, d.success) return new global["__minium_%(interface)sTask"](d.success, void 0, function(a) {
-                                c.success && c.success(a), c.complete && c.complete(a)
+                            if (console.log("@@@@rule match", d), b.__miniumMocked = !0, d.success) return new global["__minium_%(interface)sTask"](d.success, void 0, function(a) {
+                                b.success && b.success(a), b.complete && b.complete(a)
                             });
                             if (d.fail) return new global["__minium_%(interface)sTask"](void 0, d.fail, function(a) {
-                                c.fail && c.fail(a), c.complete && c.complete(a)
+                                b.fail && b.fail(a), b.complete && b.complete(a)
                             });
                             if (1 === d._miniMockType) return
-                        } return b(c)
+                        } return c(b)
                 }
             }
         })
     }
 }
```

### Comparing `minium-1.4.1/minium/utils/js/es5/mockRequestStack.js` & `minium-1.4.2/minium/utils/js/es5/mockRequestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/es5/networkPannel.js` & `minium-1.4.2/minium/utils/js/es5/networkPannel.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,49 @@
 function enableNetworkPanel() {
-    var a = wx.request;
+    var a = wx._MINI_WX_PROXY_ || wx,
+        b = a.request;
     if (!global.__minium_request_hooked) {
         Object.defineProperty(global, "__minium_request_hooked", {
             value: !0,
             writable: !1
         });
-        var b = Object.getOwnPropertyDescriptor(wx, "request");
-        if (b && !1 === b.configurable) return void console.warn("[minitest] Cannot redefine property: request");
-        var c = function(a) {
+        var c = Object.getOwnPropertyDescriptor(a, "request");
+        if (c && !1 === c.configurable) return void console.warn("[minitest] Cannot redefine property: request");
+        var d = function(a) {
                 for (var b = 5381, c = a.length; c;) b = 33 * b ^ a.charCodeAt(--c);
                 return b >>> 0
             },
-            d = new Map,
-            e = new Map;
-        Object.defineProperty(wx, "request", {
+            e = new Map,
+            f = new Map;
+        Object.defineProperty(a, "request", {
             configurable: !0,
             get: function get() {
-                return function(b) {
-                    if (!global || !global.__minium_get_mini_network_id) return a(b);
-                    if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == b.url) return a(b);
-                    var f = global.__minium_get_mini_network_id(),
-                        g = Object.assign({}, b);
+                return function(a) {
+                    if (!global || !global.__minium_get_mini_network_id) return b(a);
+                    if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == a.url) return b(a);
+                    var c = global.__minium_get_mini_network_id(),
+                        g = Object.assign({}, a);
                     delete g.success, delete g.fail, delete g.complete;
                     var h, i = Date.now();
                     try {
                         var j = JSON.stringify(g);
-                        h = c(j), d.has(h) && d.get(h) > i && (j = ""), d.set(h, i + 21e3), mini_send_request(f, j, i, h)
+                        h = d(j), e.has(h) && e.get(h) > i && (j = ""), e.set(h, i + 21e3), mini_send_request(c, j, i, h)
                     } catch (a) {
-                        mini_send_request(f, JSON.stringify({
+                        mini_send_request(c, JSON.stringify({
                             url: g.url,
                             err: a.toString()
                         }), i, 0)
                     }
-                    var k = b.complete;
-                    return b.complete = function(a) {
-                        var d = Object.assign({}, a);
-                        delete d.profile;
-                        var g = JSON.stringify(d),
-                            h = c(g),
+                    var k = a.complete;
+                    return a.complete = function(b) {
+                        var e = Object.assign({}, b);
+                        delete e.profile;
+                        var g = JSON.stringify(e),
+                            h = d(g),
                             i = Date.now();
-                        e.has(h) && e.get(h) > i && (g = ""), e.set(h, i + 21e3), mini_request_callback(f, g, i, h, b.__miniumMocked), k && k(a)
-                    }, a(b)
+                        f.has(h) && f.get(h) > i && (g = ""), f.set(h, i + 21e3), mini_request_callback(c, g, i, h, a.__miniumMocked), k && k(b)
+                    }, b(a)
                 }
             }
         })
     }
 }
```

### Comparing `minium-1.4.1/minium/utils/js/es5/requestStack.js` & `minium-1.4.2/minium/utils/js/es5/requestStack.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -9,27 +9,28 @@
                     f = setInterval(function() {
                         e--;
                         var b = global.__minium_request_stack.has(c) ? global.__minium_request_stack.get(c).size : 0;
                         console.debug("[minitest] current stack size: ", b), b <= a ? (clearInterval(f), d(!0)) : 0 > e && (clearInterval(f), d(!1))
                     }, 100)
             })
         };
-        var a = wx.request;
-        return Object.defineProperty(wx, "request", {
+        var a = wx._MINI_WX_PROXY_ || wx,
+            b = a.request;
+        return Object.defineProperty(a, "request", {
             configurable: !0,
             get: function get() {
-                return function(b) {
-                    if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == b.url) return a(b);
+                return function(a) {
+                    if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == a.url) return b(a);
                     var c, d = (getCurrentPages().pop() || {}).__wxWebviewId__;
                     global.__minium_request_stack.has(d) ? c = global.__minium_request_stack.get(d) : (c = new Map, global.__minium_request_stack.set(d, c));
-                    var e, f = b.complete;
-                    b.complete = function(a) {
+                    var e, f = a.complete;
+                    a.complete = function(a) {
                         c["delete"](e), 0 === c.size && global.__minium_request_stack["delete"](d), f && f(a)
                     };
-                    var g = a(b);
+                    var g = b(a);
                     return e = g && g.uniqueId || Math.random(), c.set(e, Date.now()), g
                 }
             }
         }), !0
     }
     return !1
 }
```

### Comparing `minium-1.4.1/minium/utils/js/es5/testAsync.js` & `minium-1.4.2/minium/utils/js/es5/testAsync.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/getUni.js` & `minium-1.4.2/minium/utils/js/min/getUni.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/helpers.js` & `minium-1.4.2/minium/utils/js/min/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/hookWxMethod.js` & `minium-1.4.2/minium/utils/js/min/hookWxMethod.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 function hookWxMethod() {
-    var e;
-    wx.$_origin_$ ? e = wx.$_origin_$ : (e = wx.$_method_$, Object.defineProperty(wx, "$_origin_$", {
+    var e, _ = wx._MINI_WX_PROXY_ || wx;
+    _.$_origin_$ ? e = _.$_origin_$ : (e = _.$_method_$, Object.defineProperty(_, "$_origin_$", {
         configurable: !0,
         get: () => e
-    })), Object.defineProperty(wx, "$_method_$", {
+    })), Object.defineProperty(_, "$_method_$", {
         configurable: !0,
-        get: () => function(...t) {
-            var n, $ = t[0],
-                _ = !1;
-            if ("$_method_$".endsWith("Sync") || $ && ($.success || $.fail || $.complete) || (_ = !0), "undefined" != typeof $_before_$ && $_before_$(...t), "undefined" != typeof $_callback_$)
-                if (_) n = e(...t).then((function(e) {
+        get: () => function(..._) {
+            var t, n = _[0],
+                $ = !1;
+            if ("$_method_$".endsWith("Sync") || n && (n.success || n.fail || n.complete) || ($ = !0), "undefined" != typeof $_before_$ && $_before_$(..._), "undefined" != typeof $_callback_$)
+                if ($) t = e(..._).then((function(e) {
                     return $_callback_$(e), e
                 })).catch((function(e) {
                     throw $_callback_$(e), e
                 }));
                 else {
-                    if ($) {
-                        var o = $.complete;
-                        $.complete = function(e) {
+                    if (n) {
+                        var o = n.complete;
+                        n.complete = function(e) {
                             $_callback_$(e), o && o(e)
                         }
                     }
-                    n = e(...t)
+                    t = e(..._)
                 }
-            else n = e(...t);
-            return "undefined" != typeof $_after_$ && $_after_$(n), n
+            else t = e(..._);
+            return "undefined" != typeof $_after_$ && $_after_$(t), t
         }
     })
 }
```

### Comparing `minium-1.4.1/minium/utils/js/min/ideMockChooseLocation.js` & `minium-1.4.2/minium/utils/js/min/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/ideMockGetLocation.js` & `minium-1.4.2/minium/utils/js/min/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/ideMockGetWeRunData.js` & `minium-1.4.2/minium/utils/js/min/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/ideMockModal.js` & `minium-1.4.2/minium/utils/js/min/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/mockChooseImage.js` & `minium-1.4.2/minium/utils/js/min/mockChooseImage.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,94 @@
 function mockChooseImage() {
     let e = wx.getFileSystemManager();
     if (!global.__minium_mock_choose_image) {
-        let t = !1;
-        global.__minium_mock_choose_image = function(...s) {
-            const i = s.map((t => {
+        let i = new Map,
+            a = new Map;
+
+        function t() {
+            a.forEach((e => {
+                e()
+            }))
+        }
+
+        function s(e, s) {
+            if (i.get(e)) return !1;
+            i.set(e, !0);
+            const r = {},
+                c = {},
+                o = {
+                    chooseImage(e) {
+                        t();
+                        const i = {
+                            errMsg: "chooseImage:ok",
+                            tempFilePaths: s.map((e => e.filePath)),
+                            tempFiles: s.map((e => ({
+                                path: e.filePath,
+                                size: e.size
+                            })))
+                        };
+                        if (!e.success && !e.fail && !e.complete) return Promise.resolve(i);
+                        e.success && e.success(i), e.complete && e.complete(i)
+                    },
+                    chooseMedia(e) {
+                        t();
+                        const i = {
+                            errMsg: "chooseMedia:ok",
+                            tempFiles: s.map((e => ({
+                                tempFilePath: e.filePath,
+                                size: e.size,
+                                fileType: "image"
+                            }))),
+                            type: "image"
+                        };
+                        if (!e.success && !e.fail && !e.complete) return Promise.resolve(i);
+                        e.success && e.success(i), e.complete && e.complete(i)
+                    },
+                    createCameraContext() {
+                        const a = r.createCameraContext(),
+                            c = a.takePhoto;
+                        return Object.defineProperty(a, "takePhoto", {
+                            configurable: !0,
+                            get: () => function(a) {
+                                if (!i.get(e)) return c.call(this, a);
+                                t();
+                                const r = {
+                                    tempImagePath: s[0].filePath,
+                                    errMsg: "takePhoto:ok"
+                                };
+                                a.success && a.success(r), a.complete && a.complete(r)
+                            }
+                        }), a
+                    }
+                },
+                l = Object.keys(o);
+            return l.forEach((t => {
+                r[t] = e[t], c[t] = Object.getOwnPropertyDescriptor(e, t)
+            })), a.set(e, (function() {
+                i.get(e) && (console.debug("release target"), i.set(e, !1), l.forEach((t => {
+                    c[t] ? c[t].get ? Object.defineProperty(e, t, {
+                        configurable: !0,
+                        get: () => r[t]
+                    }) : Object.defineProperty(e, t, {
+                        writable: !0,
+                        value: r[t]
+                    }) : e[t] = r[t]
+                })))
+            })), l.forEach((t => {
+                c[t] ? c[t].get ? Object.defineProperty(e, t, {
+                    configurable: !0,
+                    get: () => o[t]
+                }) : Object.defineProperty(e, t, {
+                    writable: !0,
+                    value: o[t]
+                }) : e[t] = o[t]
+            })), !0
+        }
+        global.__minium_mock_choose_image = function(...t) {
+            const i = t.map((t => {
                 const {
                     imageData: s,
                     imageName: i,
                     size: a
                 } = t, r = `${wx.env.USER_DATA_PATH}/.MINIUM_TMP/${i}`;
                 return s && 0 !== s.length ? new Promise(((t, a) => {
                     e.writeFile({
@@ -36,152 +117,78 @@
                     })
                 })) : Promise.resolve({
                     imageName: i,
                     filePath: r,
                     size: a
                 })
             }));
-            return Promise.all(i).then((e => (function(e, s) {
-                if (t) return !1;
-                t = !0;
-                const i = {},
-                    a = {},
-                    r = {
-                        chooseImage(e) {
-                            o();
-                            const t = {
-                                errMsg: "chooseImage:ok",
-                                tempFilePaths: s.map((e => e.filePath)),
-                                tempFiles: s.map((e => ({
-                                    path: e.filePath,
-                                    size: e.size
-                                })))
-                            };
-                            if (!e.success && !e.fail && !e.complete) return Promise.resolve(t);
-                            e.success && e.success(t), e.complete && e.complete(t)
-                        },
-                        chooseMedia(e) {
-                            o();
-                            const t = {
-                                errMsg: "chooseMedia:ok",
-                                tempFiles: s.map((e => ({
-                                    tempFilePath: e.filePath,
-                                    size: e.size,
-                                    fileType: "image"
-                                }))),
-                                type: "image"
-                            };
-                            if (!e.success && !e.fail && !e.complete) return Promise.resolve(t);
-                            e.success && e.success(t), e.complete && e.complete(t)
-                        },
-                        createCameraContext() {
-                            const e = i.createCameraContext(),
-                                a = e.takePhoto;
-                            return Object.defineProperty(e, "takePhoto", {
-                                configurable: !0,
-                                get: () => function(e) {
-                                    if (!t) return a.call(this, e);
-                                    o();
-                                    const i = {
-                                        tempImagePath: s[0].filePath,
-                                        errMsg: "takePhoto:ok"
-                                    };
-                                    e.success && e.success(i), e.complete && e.complete(i)
-                                }
-                            }), e
-                        }
-                    },
-                    c = Object.keys(r);
-
-                function o() {
-                    t && (t = !1, c.forEach((t => {
-                        a[t] ? a[t].get ? Object.defineProperty(e, t, {
-                            configurable: !0,
-                            get: () => i[t]
-                        }) : Object.defineProperty(e, t, {
-                            writable: !0,
-                            value: i[t]
-                        }) : e[t] = i[t]
-                    })))
-                }
-                c.forEach((t => {
-                    i[t] = e[t], a[t] = Object.getOwnPropertyDescriptor(e, t)
-                })), c.forEach((t => {
-                    a[t] ? a[t].get ? Object.defineProperty(e, t, {
-                        configurable: !0,
-                        get: () => r[t]
-                    }) : Object.defineProperty(e, t, {
-                        writable: !0,
-                        value: r[t]
-                    }) : e[t] = r[t]
-                }))
-            }(wx, e), e.map((e => ({
+            return Promise.all(i).then((e => (s(wx, e), wx._MINI_WX_PROXY_ && s(wx._MINI_WX_PROXY_, e), e.map((e => ({
                 name: e.imageName,
                 size: e.size
             }))))))
         };
-        let s = !1;
+        let r = !1;
         e.mkdir({
             dirPath: `${wx.env.USER_DATA_PATH}/.MINIUM_STORE`,
             recursive: !1,
             success() {
-                s = !0
+                r = !0
             },
             fail: ({
                 errMsg: e
             }) => {
-                e.indexOf("file already exists") >= 0 && (s = !0)
+                e.indexOf("file already exists") >= 0 && (r = !0)
             }
         });
-        const i = e.saveFile,
-            a = e.saveFileSync,
-            r = e.getSavedFileList;
+        const c = e.saveFile,
+            o = e.saveFileSync,
+            l = e.getSavedFileList;
         Object.defineProperty(e, "saveFile", {
             configurable: !0,
             get: () => function({
                 tempFilePath: t,
                 filePath: s,
-                success: a,
-                fail: r,
-                complete: c
+                success: i,
+                fail: a,
+                complete: r
             }) {
                 if (t.startsWith(`${wx.env.USER_DATA_PATH}/.MINIUM_TMP`)) {
-                    const i = {
+                    const c = {
                         srcPath: t,
                         destPath: s || `${wx.env.USER_DATA_PATH}/.MINIUM_STORE/${t.split("/").pop()}`
                     };
-                    return a && (i.success = e => {
-                        e.errMsg = e.errMsg.replace("copyFile", "saveFile"), e.savedFilePath = i.destPath, a(e)
-                    }), r && (i.fail = e => {
-                        e.errMsg = e.errMsg.replace("copyFile", "saveFile"), r(e)
-                    }), c && (i.complete = e => {
-                        e.errMsg = e.errMsg.replace("copyFile", "saveFile"), 0 === e.errMsg.indexOf("saveFile:ok") && (e.savedFilePath = i.destPath), c(e)
-                    }), e.copyFile(i)
+                    return i && (c.success = e => {
+                        e.errMsg = e.errMsg.replace("copyFile", "saveFile"), e.savedFilePath = c.destPath, i(e)
+                    }), a && (c.fail = e => {
+                        e.errMsg = e.errMsg.replace("copyFile", "saveFile"), a(e)
+                    }), r && (c.complete = e => {
+                        e.errMsg = e.errMsg.replace("copyFile", "saveFile"), 0 === e.errMsg.indexOf("saveFile:ok") && (e.savedFilePath = c.destPath), r(e)
+                    }), e.copyFile(c)
                 }
-                return i({
+                return c({
                     tempFilePath: t,
                     filePath: s,
-                    success: a,
-                    fail: r,
-                    complete: c
+                    success: i,
+                    fail: a,
+                    complete: r
                 })
             }
         }), Object.defineProperty(e, "saveFileSync", {
             configurable: !0,
             get: () => function(t, s) {
                 if (t.startsWith(`${wx.env.USER_DATA_PATH}/.MINIUM_TMP`)) {
                     const i = t,
                         a = s || `${wx.env.USER_DATA_PATH}/.MINIUM_STORE/${t.split("/").pop()}`;
                     try {
                         return e.copyFileSync(i, a), a
                     } catch (e) {
                         throw e.message.replace("copyFileSync", "saveFileSync")
                     }
                 }
-                return a(t, s)
+                return o(t, s)
             }
         }), Object.defineProperty(e, "getSavedFileList", {
             configurable: !0,
             get: () => function({
                 success: t,
                 complete: s
             }) {
@@ -194,15 +201,15 @@
                                 filePath: `${wx.env.USER_DATA_PATH}/.MINIUM_STORE/${e.path.startsWith("/")?e.path.slice(1):e.path}`,
                                 size: e.stats.size,
                                 createTime: e.stats.lastModifiedTime
                             }))))
                         }
                     })
                 })), new Promise((e => {
-                    r({
+                    l({
                         complete: t => {
                             e(t.fileList || [])
                         }
                     })
                 }))]).then((([e, i]) => {
                     const a = {
                         fileList: e.concat(i),
```

### Comparing `minium-1.4.1/minium/utils/js/min/mockCloudCall.js` & `minium-1.4.2/minium/utils/js/min/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/mockNetwork.js` & `minium-1.4.2/minium/utils/js/min/mockNetwork.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -58,28 +58,29 @@
             onHeadersReceived(e) {
                 this.headersReceivedCallback.push(e)
             }
             onProgressUpdate(e) {
                 this.progressUpdateCallback.push(e)
             }
         };
-        var i = wx["%(interface)s"];
-        Object.defineProperty(wx, "%(interface)s", {
+        var i = wx._MINI_WX_PROXY_ || wx,
+            s = i["%(interface)s"];
+        Object.defineProperty(i, "%(interface)s", {
             configurable: !0,
-            get: () => function(s) {
+            get: () => function(i) {
                 for (var c = 0; c < global["__minium_%(interface)s_network_mock_rule"].length; c++) {
                     var t = global["__minium_%(interface)s_network_mock_rule"][c];
-                    if (e(t, s)) {
-                        if (1 === t._miniMockType && ([t] = global["__minium_%(interface)s_network_mock_rule"].splice(c, 1)), console.log("@@@@rule match", t), s.__miniumMocked = !0, t.success) return new global["__minium_%(interface)sTask"](t.success, void 0, (e => {
-                            s.success && s.success(e), s.complete && s.complete(e)
+                    if (e(t, i)) {
+                        if (1 === t._miniMockType && ([t] = global["__minium_%(interface)s_network_mock_rule"].splice(c, 1)), console.log("@@@@rule match", t), i.__miniumMocked = !0, t.success) return new global["__minium_%(interface)sTask"](t.success, void 0, (e => {
+                            i.success && i.success(e), i.complete && i.complete(e)
                         }));
                         if (t.fail) return new global["__minium_%(interface)sTask"](void 0, t.fail, (e => {
-                            s.fail && s.fail(e), s.complete && s.complete(e)
+                            i.fail && i.fail(e), i.complete && i.complete(e)
                         }));
                         if (1 === t._miniMockType) return
                     }
                 }
-                return i(s)
+                return s(i)
             }
         })
     }
 }
```

### Comparing `minium-1.4.1/minium/utils/js/min/mockRequestStack.js` & `minium-1.4.2/minium/utils/js/min/mockRequestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/js/min/networkPannel.js` & `minium-1.4.2/minium/utils/js/min/networkPannel.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,49 @@
 function enableNetworkPanel() {
-    let e = wx.request;
+    let e = wx._MINI_WX_PROXY_ || wx,
+        t = e.request;
     if (!global.__minium_request_hooked) {
         Object.defineProperty(global, "__minium_request_hooked", {
             value: !0,
             writable: !1
         });
-        const t = Object.getOwnPropertyDescriptor(wx, "request");
-        if (t && !1 === t.configurable) return void console.warn("[minitest] Cannot redefine property: request");
-        let r = function(e) {
+        const r = Object.getOwnPropertyDescriptor(e, "request");
+        if (r && !1 === r.configurable) return void console.warn("[minitest] Cannot redefine property: request");
+        let i = function(e) {
                 let t = 5381,
                     r = e.length;
                 for (; r;) t = 33 * t ^ e.charCodeAt(--r);
                 return t >>> 0
             },
-            i = new Map,
-            n = new Map;
-        Object.defineProperty(wx, "request", {
+            n = new Map,
+            l = new Map;
+        Object.defineProperty(e, "request", {
             configurable: !0,
-            get: () => function(t) {
-                if (!global || !global.__minium_get_mini_network_id) return e(t);
-                if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == t.url) return e(t);
-                let l, o = global.__minium_get_mini_network_id(),
-                    s = Object.assign({}, t);
-                delete s.success, delete s.fail, delete s.complete;
-                let u = Date.now();
+            get: () => function(e) {
+                if (!global || !global.__minium_get_mini_network_id) return t(e);
+                if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == e.url) return t(e);
+                let r, o = global.__minium_get_mini_network_id(),
+                    _ = Object.assign({}, e);
+                delete _.success, delete _.fail, delete _.complete;
+                let s = Date.now();
                 try {
-                    let e = JSON.stringify(s);
-                    l = r(e), i.has(l) && i.get(l) > u && (e = ""), i.set(l, u + 21e3), mini_send_request(o, e, u, l)
+                    let e = JSON.stringify(_);
+                    r = i(e), n.has(r) && n.get(r) > s && (e = ""), n.set(r, s + 21e3), mini_send_request(o, e, s, r)
                 } catch (e) {
                     mini_send_request(o, JSON.stringify({
-                        url: s.url,
+                        url: _.url,
                         err: e.toString()
-                    }), u, 0)
+                    }), s, 0)
                 }
-                let _ = t.complete;
-                return t.complete = e => {
-                    let i = Object.assign({}, e);
-                    delete i.profile;
-                    let l = JSON.stringify(i),
-                        s = r(l),
-                        u = Date.now();
-                    n.has(s) && n.get(s) > u && (l = ""), n.set(s, u + 21e3), mini_request_callback(o, l, u, s, t.__miniumMocked), _ && _(e)
-                }, e(t)
+                let u = e.complete;
+                return e.complete = t => {
+                    let r = Object.assign({}, t);
+                    delete r.profile;
+                    let n = JSON.stringify(r),
+                        _ = i(n),
+                        s = Date.now();
+                    l.has(_) && l.get(_) > s && (n = ""), l.set(_, s + 21e3), mini_request_callback(o, n, s, _, e.__miniumMocked), u && u(t)
+                }, t(e)
             }
         })
     }
 }
```

### Comparing `minium-1.4.1/minium/utils/js/min/requestStack.js` & `minium-1.4.2/minium/utils/js/min/requestStack.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,32 @@
 function miniumRequestStack() {
     if (!global.__minium_request_stack) {
         global.__minium_request_stack = new Map, global.__minium_wait_util = function(e = 0, t = 20) {
-            var r = (getCurrentPages().pop() || {}).__wxWebviewId__;
-            return new Promise((_ => {
+            var _ = (getCurrentPages().pop() || {}).__wxWebviewId__;
+            return new Promise((r => {
                 var a = 10 * t,
                     i = setInterval((() => {
                         a--;
-                        var t = global.__minium_request_stack.has(r) ? global.__minium_request_stack.get(r).size : 0;
-                        console.debug("[minitest] current stack size: ", t), t <= e ? (clearInterval(i), _(!0)) : a < 0 && (clearInterval(i), _(!1))
+                        var t = global.__minium_request_stack.has(_) ? global.__minium_request_stack.get(_).size : 0;
+                        console.debug("[minitest] current stack size: ", t), t <= e ? (clearInterval(i), r(!0)) : a < 0 && (clearInterval(i), r(!1))
                     }), 100)
             }))
         };
-        var e = wx.request;
-        return Object.defineProperty(wx, "request", {
+        var e = wx._MINI_WX_PROXY_ || wx,
+            t = e.request;
+        return Object.defineProperty(e, "request", {
             configurable: !0,
-            get: () => function(t) {
-                if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == t.url) return e(t);
-                var r, _ = (getCurrentPages().pop() || {}).__wxWebviewId__;
-                global.__minium_request_stack.has(_) ? r = global.__minium_request_stack.get(_) : (r = new Map, global.__minium_request_stack.set(_, r));
-                var a, i = t.complete;
-                t.complete = e => {
-                    r.delete(a), 0 === r.size && global.__minium_request_stack.delete(_), i && i(e)
+            get: () => function(e) {
+                if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == e.url) return t(e);
+                var _, r = (getCurrentPages().pop() || {}).__wxWebviewId__;
+                global.__minium_request_stack.has(r) ? _ = global.__minium_request_stack.get(r) : (_ = new Map, global.__minium_request_stack.set(r, _));
+                var a, i = e.complete;
+                e.complete = e => {
+                    _.delete(a), 0 === _.size && global.__minium_request_stack.delete(r), i && i(e)
                 };
-                var n = e(t);
-                return a = n && n.uniqueId || Math.random(), r.set(a, Date.now()), n
+                var n = t(e);
+                return a = n && n.uniqueId || Math.random(), _.set(a, Date.now()), n
             }
         }), !0
     }
     return !1
 }
```

### Comparing `minium-1.4.1/minium/utils/meta.py` & `minium-1.4.2/minium/utils/meta.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.1/minium/utils/utils.py` & `minium-1.4.2/minium/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,43 +61,45 @@
             return r
 
         return wrapper
 
     return spin_until_true
 
 
-def retry(cnt, expected_exception=None):
+def retry(cnt, expected_exception=None, report: types.FunctionType=None):
     """
     重试固定次数装饰器, 被修饰函数没有raise error则直接返回, 有则最多执行${cnt}次
     :cnt: 重试次数，函数最多被执行 ${cnt} 次
     :expected_exception: 命中预期的错误(isinstance(e, expected_exception))才重试, None为所有错误
+    :report: 重试成功后上报
     """
-
     def try_until_no_error(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             _cnt = 0
             while _cnt < cnt:
                 try:
                     _cnt += 1
-                    return func(*args, **kwargs)
+                    ret = func(*args, **kwargs)
                 except:
                     if _cnt >= cnt:
                         raise
                     e = sys.exc_info()[1]
                     if expected_exception is None or isinstance(e, expected_exception):
                         logger.warning(
                             f'{f"第 {_cnt} 次" if _cnt < cnt else "最后一次"}重新运行{func.__name__}'
                         )
                         logger.info(f'原因: {e.__class__.__name__}{str(e.args)}')
                         continue
                     raise
-
+                else:
+                    if report and _cnt > 1:
+                        report(_cnt, func.__name__)
+                    return ret
         return wrapper
-
     return try_until_no_error
 
 
 CatchableType = typing.Union[types.FunctionType, types.MethodType]
 
 
 @overload
@@ -181,15 +183,15 @@
         args=(),
         kwargs=None,
         daemon=None,
         semaphore=None,
     ):
         super().__init__(group, target, name, args, kwargs, daemon=daemon)
         self._result = None
-        self._exception = None
+        self._exception: BaseException = None
         self._semaphore: threading.Semaphore = semaphore
 
     def run(self):
         try:
             if self._target:
                 self._result = self._target(*self._args, **self._kwargs)
         except:
@@ -378,16 +380,14 @@
     reference asyncio.wait_for
     wait fut done, when timeout, raise
     """
     if loop is None:
         loop = asyncio.get_running_loop()
     elif isinstance(loop, ProcessSafeEventLoop):
         loop = loop.loop
-    else:
-        loop = loop
     waiter = loop.create_future()
     cb = functools.partial(_release_waiter, waiter)
     fut = asyncio.ensure_future(fut, loop=loop)
     fut.add_done_callback(cb)
     timeout_handle = loop.call_later(timeout, _release_waiter, waiter)
 
     try:
```

### Comparing `minium-1.4.1/minium.egg-info/PKG-INFO` & `minium-1.4.2/minium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minium
-Version: 1.4.1
+Version: 1.4.2
 Summary: Minium is the best MiniProgram auto test framework.
 Home-page: https://minitest.weixin.qq.com/#/
 Author: WeChat-Test
 Author-email: minitest@tencent.com
 License: MIT
 Description: 
         install:
```

### Comparing `minium-1.4.1/minium.egg-info/SOURCES.txt` & `minium-1.4.2/minium.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 minium/utils/injectjs.py
 minium/utils/meta.py
 minium/utils/platforms.py
 minium/utils/utils.py
 minium/utils/js/es5/addCloudCallMockRule.js
 minium/utils/js/es5/addNetworkMockRule.js
 minium/utils/js/es5/callContextMethod.js
+minium/utils/js/es5/checkEnv.js
 minium/utils/js/es5/checkInject.js
 minium/utils/js/es5/cleanCloudCallMockRule.js
 minium/utils/js/es5/cleanNetworkMockRule.js
 minium/utils/js/es5/createContext.js
 minium/utils/js/es5/editEditorText.js
 minium/utils/js/es5/evalMockChooseImage.js
 minium/utils/js/es5/getAppConfig.js
@@ -199,14 +200,15 @@
 minium/utils/js/es5/stopGetPerformance.js
 minium/utils/js/es5/testAsync.js
 minium/utils/js/es5/uuid.js
 minium/utils/js/es5/waitUtil.js
 minium/utils/js/min/addCloudCallMockRule.js
 minium/utils/js/min/addNetworkMockRule.js
 minium/utils/js/min/callContextMethod.js
+minium/utils/js/min/checkEnv.js
 minium/utils/js/min/checkInject.js
 minium/utils/js/min/cleanCloudCallMockRule.js
 minium/utils/js/min/cleanNetworkMockRule.js
 minium/utils/js/min/createContext.js
 minium/utils/js/min/editEditorText.js
 minium/utils/js/min/evalMockChooseImage.js
 minium/utils/js/min/getAppConfig.js
```

### Comparing `minium-1.4.1/setup.py` & `minium-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import sys
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 from setuptools import setup, find_packages
 
 # We do not support Python <3.8
 if sys.version_info < (3, 8):
     print(
         "Unfortunately, your python version is not supported!\n"
```

