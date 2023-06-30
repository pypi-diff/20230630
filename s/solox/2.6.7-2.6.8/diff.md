# Comparing `tmp/solox-2.6.7.tar.gz` & `tmp/solox-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-5wsd0zoo/solox-2.6.7.tar", last modified: Mon Jun 19 10:07:24 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-h_aujyiy/solox-2.6.8.tar", last modified: Fri Jun 30 01:20:09 2023, max compression
```

## Comparing `solox-2.6.7.tar` & `solox-2.6.8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-19 10:07:14.000000 solox-2.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 10:07:14.000000 solox-2.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-19 10:07:24.000000 solox-2.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-19 10:07:14.000000 solox-2.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-19 10:07:24.000000 solox-2.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 10:07:14.000000 solox-2.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 10:07:14.000000 solox-2.6.7/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-19 10:07:14.000000 solox-2.6.7/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-19 10:07:14.000000 solox-2.6.7/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29411 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-06-19 10:07:14.000000 solox-2.6.7/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-19 10:07:14.000000 solox-2.6.7/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    65914 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    43489 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/analysis_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)    38461 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    33843 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)   101320 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55683 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-19 10:07:14.000000 solox-2.6.7/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 10:07:14.000000 solox-2.6.7/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30915 2023-06-19 10:07:14.000000 solox-2.6.7/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-19 10:07:14.000000 solox-2.6.7/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-19 10:07:14.000000 solox-2.6.7/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 10:07:24.000000 solox-2.6.7/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-30 01:20:01.000000 solox-2.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-30 01:20:01.000000 solox-2.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-30 01:20:09.000000 solox-2.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-30 01:20:01.000000 solox-2.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-30 01:20:09.000000 solox-2.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-30 01:20:01.000000 solox-2.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-30 01:20:01.000000 solox-2.6.8/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-30 01:20:01.000000 solox-2.6.8/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-30 01:20:01.000000 solox-2.6.8/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33710 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29411 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-06-30 01:20:01.000000 solox-2.6.8/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-30 01:20:01.000000 solox-2.6.8/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65914 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43489 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38461 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33924 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   103005 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55646 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-06-30 01:20:01.000000 solox-2.6.8/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 01:20:01.000000 solox-2.6.8/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30509 2023-06-30 01:20:01.000000 solox-2.6.8/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-30 01:20:01.000000 solox-2.6.8/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-30 01:20:01.000000 solox-2.6.8/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:20:09.000000 solox-2.6.8/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-30 01:20:09.000000 solox-2.6.8/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-30 01:20:09.000000 solox-2.6.8/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:20:09.000000 solox-2.6.8/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 01:20:09.000000 solox-2.6.8/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 01:20:09.000000 solox-2.6.8/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.7/LICENSE` & `solox-2.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/PKG-INFO` & `solox-2.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.7
+Version: 2.6.8
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox  (pip install solox==2.6.4)
+pip install -U solox    (pip install solox==2.6.8)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
```

### Comparing `solox-2.6.7/README.md` & `solox-2.6.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox  (pip install solox==2.6.4)
+pip install -U solox    (pip install solox==2.6.8)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
```

### Comparing `solox-2.6.7/setup.py` & `solox-2.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/__main__.py` & `solox-2.6.8/solox/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/debug.py` & `solox-2.6.8/solox/debug.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/_iosPerf.py` & `solox-2.6.8/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/adb/mac/adb` & `solox-2.6.8/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/adb.py` & `solox-2.6.8/solox/public/adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 
     def shell(self, cmd, deviceId):
         run_cmd = f'{self.adb_path} -s {deviceId} shell {cmd}'
         result = subprocess.Popen(run_cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()[
             0].decode("utf-8").strip()
         return result
     
-    def tcp_shell(self, cmd, deviceId):
-        run_cmd = f'{self.adb_path} -s {deviceId} shell {cmd}'
+    def tcp_shell(self, deviceId, cmd):
+        run_cmd = f'{self.adb_path} -s {deviceId} {cmd}'
         result = os.system(run_cmd)
         return result
 
     def shell_noDevice(self, cmd):
         run_cmd = f'{self.adb_path} {cmd}'
         result = os.system(run_cmd)
         return result
```

### Comparing `solox-2.6.7/solox/public/apm.py` & `solox-2.6.8/solox/public/apm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import re
 import time
 import os
-import traceback
 from logzero import logger
 import tidevice
 import multiprocessing
 import solox.public._iosPerf as iosP
 from solox.public.iosperf._perf import DataType, Performance
 from solox.public.adb import adb
 from solox.public.common import Devices, File, Method, Platform
@@ -490,11 +489,11 @@
             pool.apply_async(self.collectFlow)
             pool.apply_async(self.collectGpu)
             pool.close()
             pool.join()
             self.setPerfs()     
         except KeyboardInterrupt:
             self.setPerfs()
-        except Exception:
-            traceback.print_exc()
+        except Exception as e:
+            logger.exception(e)
         finally:
             logger.info('End of testing')
```

### Comparing `solox-2.6.7/solox/public/apm_pk.py` & `solox-2.6.8/solox/public/apm_pk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import re
+import os
 import time
 from solox.public.adb import adb
 from solox.public.common import Devices, File
 from solox.public.fps import FPSMonitor, TimeUtils
 
 d = Devices()
 f = File()
@@ -48,39 +49,36 @@
         IdleCpu = float(int(toks[4]))
         return IdleCpu
 
     def getAndroidCpuRate(self):
         """get the Android cpu rate of a process"""
         processCpuTime1_first = self.getprocessCpuStat(pkgName=self.pkgNameList[0], deviceId=self.deviceId1)
         totalCpuTime1_first = self.getTotalCpuStat(deviceId=self.deviceId1)
-        time.sleep(1)
+        time.sleep(0.5)
         processCpuTime1_second = self.getprocessCpuStat(pkgName=self.pkgNameList[0], deviceId=self.deviceId1)
         totalCpuTime1_second = self.getTotalCpuStat(deviceId=self.deviceId1)
 
         if len(self.pkgNameList) == 1:
             processCpuTime2_first = self.getprocessCpuStat(pkgName=self.pkgNameList[0], deviceId=self.deviceId2)
             totalCpuTime2_first = self.getTotalCpuStat(deviceId=self.deviceId2)
-            time.sleep(1)
+            time.sleep(0.5)
             processCpuTime2_second = self.getprocessCpuStat(pkgName=self.pkgNameList[0], deviceId=self.deviceId2)
             totalCpuTime2_second = self.getTotalCpuStat(deviceId=self.deviceId2)
         else:
             processCpuTime2_first = self.getprocessCpuStat(pkgName=self.pkgNameList[1], deviceId=self.deviceId2)
             totalCpuTime2_first = self.getTotalCpuStat(deviceId=self.deviceId2)
-            time.sleep(1)
+            time.sleep(0.5)
             processCpuTime2_second = self.getprocessCpuStat(pkgName=self.pkgNameList[1], deviceId=self.deviceId2)
             totalCpuTime2_second = self.getTotalCpuStat(deviceId=self.deviceId2)
 
         appCpuRate1 = round(float((processCpuTime1_second - processCpuTime1_first) / (totalCpuTime1_second - totalCpuTime1_first) * 100), 2)
         appCpuRate2 = round(float((processCpuTime2_second - processCpuTime2_first) / (totalCpuTime2_second - totalCpuTime2_first) * 100), 2)
-        
         apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
-        f.add_log(f'{f.report_dir}/cpu_app1.log', apm_time, appCpuRate1)
-        f.add_log(f'{f.report_dir}/cpu_app2.log', apm_time, appCpuRate2)
-
-
+        f.add_log(os.path.join(f.report_dir, 'cpu_app1.log'), apm_time, appCpuRate1)
+        f.add_log(os.path.join(f.report_dir, 'cpu_app2.log'), apm_time, appCpuRate2)
         return appCpuRate1, appCpuRate2
 
 
 class MEM_PK:
     def __init__(self, pkgNameList: list, deviceId1, deviceId2):
         self.pkgNameList = pkgNameList
         self.deviceId1 = deviceId1
@@ -99,18 +97,17 @@
         """Get the app memory"""
         if len(self.pkgNameList) == 1:
             totalPass1 = self.getAndroidMem(self.pkgNameList[0], self.deviceId1)
             totalPass2 = self.getAndroidMem(self.pkgNameList[0], self.deviceId2)
         else:
             totalPass1 = self.getAndroidMem(self.pkgNameList[0], self.deviceId1)
             totalPass2 = self.getAndroidMem(self.pkgNameList[1], self.deviceId2)
-        
         apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
-        f.add_log(f'{f.report_dir}/mem1.log', apm_time, totalPass1)
-        f.add_log(f'{f.report_dir}/mem2.log', apm_time, totalPass2)
+        f.add_log(os.path.join(f.report_dir, 'mem1.log'), apm_time, totalPass1)
+        f.add_log(os.path.join(f.report_dir, 'mem1.log'), apm_time, totalPass2)
 
         return totalPass1, totalPass2
 
 
 class Flow_PK:
 
     def __init__(self, pkgNameList: list, deviceId1, deviceId2):
@@ -122,15 +119,15 @@
         """Get Android upflow and downflow data, unit:KB"""
         pid = d.getPid(pkgName=pkgName, deviceId=deviceId)
         cmd = f'cat /proc/{pid}/net/dev |{d.filterType()} wlan0'
         output_pre = adb.shell(cmd=cmd, deviceId=deviceId)
         m_pre = re.search(r'wlan0:\s*(\d+)\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*(\d+)', output_pre)
         sendNum_pre = round(float(float(m_pre.group(2)) / 1024), 2)
         recNum_pre = round(float(float(m_pre.group(1)) / 1024), 2)
-        time.sleep(1)
+        time.sleep(0.5)
         output_final = adb.shell(cmd=cmd, deviceId=deviceId)
         m_final = re.search(r'wlan0:\s*(\d+)\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*\d+\s*(\d+)', output_final)
         sendNum_final = round(float(float(m_final.group(2)) / 1024), 2)
         recNum_final = round(float(float(m_final.group(1)) / 1024), 2)
         sendNum = round(float(sendNum_final - sendNum_pre), 2)
         recNum = round(float(recNum_final - recNum_pre), 2)
         network = round(float(sendNum + recNum), 2)
@@ -140,18 +137,17 @@
         """Get the upflow and downflow data, unit:KB"""
         if len(self.pkgNameList) == 1:
             network1 = self.getAndroidNet(self.pkgNameList[0], self.deviceId1)
             network2 = self.getAndroidNet(self.pkgNameList[0], self.deviceId2)
         else:
             network1 = self.getAndroidNet(self.pkgNameList[0], self.deviceId1)
             network2 = self.getAndroidNet(self.pkgNameList[1], self.deviceId2)
-        
         apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')    
-        f.add_log(f'{f.report_dir}/network1.log', apm_time, network1)
-        f.add_log(f'{f.report_dir}/network2.log', apm_time, network2)
+        f.add_log(os.path.join(f.report_dir, 'network1.log'), apm_time, network1)
+        f.add_log(os.path.join(f.report_dir, 'network2.log'), apm_time, network2)
         return network1, network2
 
 
 class FPS_PK:
 
     def __init__(self, pkgNameList: list, deviceId1, deviceId2, surfaceview=True):
         self.pkgNameList = pkgNameList
@@ -169,19 +165,16 @@
 
 
     def getFPS(self):
         """get fps"""
         if len(self.pkgNameList) == 1:
             fps1 = self.getAndroidFps(pkgName=self.pkgNameList[0], deviceId=self.deviceId1)
             fps2 = self.getAndroidFps(pkgName=self.pkgNameList[0], deviceId=self.deviceId2)
-
         else:
             fps1 = self.getAndroidFps(pkgName=self.pkgNameList[0], deviceId=self.deviceId1)
             fps2 = self.getAndroidFps(pkgName=self.pkgNameList[1], deviceId=self.deviceId2)
-        
         apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
-        f.add_log(f'{f.report_dir}/fps1.log', apm_time, fps1)
-        f.add_log(f'{f.report_dir}/fps2.log', apm_time, fps2)
-
+        f.add_log(os.path.join(f.report_dir, 'fps1.log'), apm_time, fps1)
+        f.add_log(os.path.join(f.report_dir, 'fps2.log'), apm_time, fps2)
         return fps1, fps2
```

### Comparing `solox-2.6.7/solox/public/common.py` & `solox-2.6.8/solox/public/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import re
 import shutil
 import time
 import requests
 from logzero import logger
 from solox.public.adb import adb
 from tqdm import tqdm
-import traceback
 import socket
 from urllib.request import urlopen
 import ssl
 import xlwt
 from jinja2 import Environment, FileSystemLoader
  
 class Platform:
@@ -26,15 +25,15 @@
     def __init__(self, platform=Platform.Android):
         self.platform = platform
         self.adb = adb.adb_path
 
     def execCmd(self, cmd):
         """Execute the command to get the terminal print result"""
         r = os.popen(cmd)
-        text = r.read().strip()
+        text = r.buffer.read().decode(encoding='utf-8').strip()
         r.close()
         return text
 
     def filterType(self):
         """Select the pipe filtering method according to the system"""
         filtertype = ('grep', 'findstr')[platform.system() == Platform.Windows]
         return filtertype
@@ -63,29 +62,29 @@
         return Devices
 
     def getIdbyDevice(self, deviceinfo, platform):
         """Obtain the corresponding device id according to the Android device information"""
         if platform == Platform.Android:
             deviceId = re.sub(u"\\(.*?\\)|\\{.*?}|\\[.*?]", "", deviceinfo)
             if deviceId not in self.getDeviceIds():
-                raise Exception('no found device: %s'.format(deviceId))
+                raise Exception('no device found')
         else:
             deviceId = deviceinfo.split(':')[1]
         return deviceId
 
     def getPid(self, deviceId, pkgName):
         """Get the pid corresponding to the Android package name"""
         result = os.popen(f"{self.adb} -s {deviceId} shell ps -ef | {self.filterType()} {pkgName}").readlines()
         try:
             processList = ['{}:{}'.format(process.split()[1],process.split()[7]) for process in result]
             processList.reverse()
             if len(processList) == 0:
-               logger.warning('no pid found')     
-        except Exception:
-            traceback.print_exc()
+               logger.warning('{}: no pid found'.format(pkgName))     
+        except Exception as e:
+            logger.exception(e)
         return processList
 
     def checkPkgname(self, pkgname):
         flag = True
         replace_list = ['com.google']
         for i in replace_list:
             if i in pkgname:
@@ -115,33 +114,34 @@
 
     def getPkgnameByiOS(self, udid):
         """Get all package names of the corresponding iOS device"""
         pkgResult = self.execCmd(f'tidevice --udid {udid} applist').split('\n')
         pkgNames = [pkgResult[i].split(' ')[0] for i in range(len(pkgResult))]
         return pkgNames
     
-    def localIP(self):
+    def get_pc_ip(self):
         try:
             s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             s.connect(('8.8.8.8', 80))
             ip = s.getsockname()[0]
         except Exception:
             logger.error('get local ip failed')
             ip = '127.0.0.1'
         finally:
             s.close()
         return ip
     
-    def tcpConnect(self, deviceId, port):
-        logger.info('TCP mode port')
-        adb.tcp_shell(deviceId=deviceId, cmd='tcpip {}'.format(port))
-        logger.info('Connect result')
-        result = adb.tcp_shell(cmd='connect {}:{}'.format(self.localIP(), port))
-        return result
-
+    def get_device_ip(self, deviceId):
+        content = os.popen(f"{self.adb} -s {deviceId} shell ip addr show wlan0").read()
+        logger.info(content)
+        math_obj = re.search(r'inet\s(\d+\.\d+\.\d+\.\d+).*?wlan0', content)
+        if math_obj and math_obj.group(1):
+            return math_obj.group(1)
+        return None
+    
     def devicesCheck(self, platform, deviceid=None, pkgname=None):
         """Check the device environment"""
         match(platform):
             case Platform.Android:
                 if len(self.getDeviceIds()) == 0:
                     raise Exception('no devices found')
                 if len(self.getPid(deviceId=deviceid, pkgName=pkgname)) == 0:
@@ -671,24 +671,39 @@
         try:
             result = value
         except ZeroDivisionError :
             result = default    
         except Exception:
             result = default            
         return result
+    
+    @classmethod
+    def _get_setting(cls, request):
+        content = {}
+        content['cpuWarning'] = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
+        content['memWarning'] = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
+        content['fpsWarning'] = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
+        content['netdataRecvWarning'] = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
+        content['netdataSendWarning'] = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
+        content['betteryWarning'] = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
+        content['duration'] = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
+        content['solox_host'] = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
+        content['host_switch'] = request.cookies.get('host_switch')
+        return content        
+
 
 class Install:
 
     def uploadFile(self, file_path, file_obj):
         """save upload file"""
         try:
             file_obj.save(file_path)
             return True
-        except:
-            traceback.print_exc()
+        except Exception as e:
+            logger.exception(e)
             return False            
 
     def downloadLink(self,filelink=None, path=None, name=None):
         try:
             logger.info('Install link : {}'.format(filelink))
             ssl._create_default_https_context = ssl._create_unverified_context
             file_size = int(urlopen(filelink).info().get('Content-Length', -1))
@@ -719,26 +734,7 @@
     def installIPA(self, path):
         result = Devices.execCmd('tidevice install {}'.format(path))
         if result == 0:
             os.remove(path)
             return True, result
         else:
             return False, result
-
-# class Config:
-
-#     def __init__(self):
-#         self.configRoot = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'config')
-
-#     def get_devices(self):
-#         config_path = os.path.join(self.configRoot, 'devices.json')
-#         content = {}
-#         with open(config_path, "r", encoding="utf-8") as f:
-#             content = json.load(f)
-#         devices = content['content']    
-#         return devices
-
-#     def set_devices(self):
-#         pass
-
-#     def remove_device(self, deviceid):
-#         pass
```

### Comparing `solox-2.6.7/solox/public/fps.py` & `solox-2.6.8/solox/public/fps.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/__main__.py` & `solox-2.6.8/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_crash.py` & `solox-2.6.8/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_device.py` & `solox-2.6.8/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_hexdump.py` & `solox-2.6.8/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_imagemounter.py` & `solox-2.6.8/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_installation.py` & `solox-2.6.8/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_instruments.py` & `solox-2.6.8/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_ipautil.py` & `solox-2.6.8/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_perf.py` & `solox-2.6.8/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_proto.py` & `solox-2.6.8/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_relay.py` & `solox-2.6.8/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_safe_socket.py` & `solox-2.6.8/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_ssl.py` & `solox-2.6.8/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_sync.py` & `solox-2.6.8/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_types.py` & `solox-2.6.8/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_usbmux.py` & `solox-2.6.8/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_utils.py` & `solox-2.6.8/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.8/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/bplist.py` & `solox-2.6.8/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/exceptions.py` & `solox-2.6.8/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/plistlib2.py` & `solox-2.6.8/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.8/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/iosperf/struct2.py` & `solox-2.6.8/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/report_template/android.html` & `solox-2.6.8/solox/public/report_template/android.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/public/report_template/ios.html` & `solox-2.6.8/solox/public/report_template/ios.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/highlight.min.css` & `solox-2.6.8/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.8/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.8/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/select2.min.css` & `solox-2.6.8/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/sweetalert2.min.css` & `solox-2.6.8/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/tabler.demo.min.css` & `solox-2.6.8/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/css/tabler.min.css` & `solox-2.6.8/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/image/404.png` & `solox-2.6.8/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/image/500.png` & `solox-2.6.8/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/image/avatar.png` & `solox-2.6.8/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/image/coffee.png` & `solox-2.6.8/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/image/readme/home.png` & `solox-2.6.8/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/image/readme/pk.png` & `solox-2.6.8/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/apexcharts.js` & `solox-2.6.8/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/gray.js` & `solox-2.6.8/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/highlight.min.js` & `solox-2.6.8/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/highstock.js` & `solox-2.6.8/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/html2canvas.min.js` & `solox-2.6.8/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/jquery.min.js` & `solox-2.6.8/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/select2.min.js` & `solox-2.6.8/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/socket.io.js` & `solox-2.6.8/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/sweetalert2.min.js` & `solox-2.6.8/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/tabler.demo.min.js` & `solox-2.6.8/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/js/tabler.min.js` & `solox-2.6.8/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/static/logo/logo.png` & `solox-2.6.8/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/templates/404.html` & `solox-2.6.8/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/templates/500.html` & `solox-2.6.8/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/templates/analysis.html` & `solox-2.6.8/solox/templates/analysis.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/templates/analysis_compare.html` & `solox-2.6.8/solox/templates/analysis_compare.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/templates/analysis_pk.html` & `solox-2.6.8/solox/templates/analysis_pk.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.7/solox/templates/base.html` & `solox-2.6.8/solox/templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.7
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.8
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
@@ -165,48 +165,48 @@
             <div class="tab-content">
               <div id="tab-top-2" class="card tab-pane active show">
                 <div class="card-body">
                     <div class="row mb-3">
                         <div class="col-md-6 col-xl-12">
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} CPU告警值 {% else %} CPU warning value {% endif %}</label>
-                                <input id="cpu_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ cpuWarning }}">
+                                <input id="cpu_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.cpuWarning }}">
                             </div>
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} 内存告警值 {% else %} Memory warning value {% endif %}</label>
-                                <input id="mem_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ memWarning }}">
+                                <input id="mem_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.memWarning }}">
                             </div>
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} FPS告警值 {% else %} FPS warning value {% endif %}</label>
-                                <input id="fps_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ fpsWarning }}">
+                                <input id="fps_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.fpsWarning }}">
                             </div>
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} 电量告警值 {% else %} Battery warning value {% endif %}</label>
-                                <input id="battery_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ betteryWarning }}">
+                                <input id="battery_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.betteryWarning }}">
                             </div>
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} 上行流量告警值 {% else %} Send network data warning value {% endif %}</label>
-                                <input id="upflow_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ netdataSendWarning }}">
+                                <input id="upflow_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.netdataSendWarning }}">
                             </div>
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} 下行流量告警值 {% else %} Recv network data warning value {% endif %}</label>
-                                <input id="downflow_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ netdataRecvWarning }}">
+                                <input id="downflow_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.netdataRecvWarning }}">
                             </div>
                         </div>
                     </div>
                 </div>
               </div>
               <!-- Content of card #2 -->
               <div id="tab-top-3" class="card tab-pane">
                 <div class="card-body">
                     <div class="row mb-3">
                         <div class="col-md-6 col-xl-12">
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} 持续执行时间（分钟） {% else %} Duration（minutes） {% endif %}</label>
-                                <input id="duration" type="text" class="form-control"  placeholder="Input placeholder" value="{{ duration }}">
+                                <input id="duration" type="text" class="form-control"  placeholder="Input placeholder" value="{{ settings.duration }}">
                             </div>
                         </div>
                     </div>
                 </div>
               </div>
               <div id="tab-top-4" class="card tab-pane">
                 <div class="card-body">
@@ -221,19 +221,19 @@
                             </thead>
                             <tbody>
                                 <tr>
                                     <td>
                                         <svg t="1680252875419" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="19154" width="50" height="50"><path d="M471.04 727.04h81.92v184.32h-81.92z" p-id="19155"></path><path d="M307.2 911.36m30.72 0l348.16 0q30.72 0 30.72 30.72l0 0q0 30.72-30.72 30.72l-348.16 0q-30.72 0-30.72-30.72l0 0q0-30.72 30.72-30.72Z" p-id="19156"></path><path d="M20.48 51.2m51.2 0l880.64 0q51.2 0 51.2 51.2l0 573.44q0 51.2-51.2 51.2l-880.64 0q-51.2 0-51.2-51.2l0-573.44q0-51.2 51.2-51.2Z" p-id="19157"></path><path d="M122.88 645.12m20.48 0l737.28 0q20.48 0 20.48 20.48l0 0q0 20.48-20.48 20.48l-737.28 0q-20.48 0-20.48-20.48l0 0q0-20.48 20.48-20.48Z" fill="#EBBA50" p-id="19158"></path></svg>
                                     </td>
                                     <td>
-                                        <input id="host" type="text" class="form-control form-control-sm" placeholder="ex : 192.168.10.10:6006" value="{{ solox_host }}">
+                                        <input id="host" type="text" class="form-control form-control-sm" placeholder="ex : 192.168.10.10:6006" value="{{ settings.solox_host }}">
                                     </td>
                                     <td>
                                         <label class="form-check  form-switch">
-                                            {% if host_switch == '1' %}
+                                            {% if settings.host_switch == '1' %}
                                             <input  class="form-check-input host_switch" type="checkbox" checked>
                                             {% else %}
                                             <input  class="form-check-input host_switch" type="checkbox">
                                             {% endif %}
                                         </label>
                                     </td>
                                 </tr>
```

#### html2text {}

```diff
@@ -24,37 +24,39 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.7
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.8
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
     * {%_if_lan_==_'cn'_%}_åè­¦å¼_{%_else_%}_Warning_Value_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_å®æ¶å¨_{%_else_%}_Timer_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_è¿ç¨è®¿é®_{%_else_%}_Remote_{%_endif_%}_ _{%_if
       lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
-{ cpuWarning }}    ]
+{ settings.cpuWarning }}]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
-%} [{{ memWarning }}    ]
+%} [{{ settings.memWarning }}]
 {% if lan == 'cn' %} FPSåè­¦å¼ {% else %} FPS warning value {% endif %} [{
-{ fpsWarning }}    ]
+{ settings.fpsWarning }}]
 {% if lan == 'cn' %} çµéåè­¦å¼ {% else %} Battery warning value {% endif
-%} [{{ betteryWarning }}]
+%} [{{ settings.betteryWarning }}]
 {% if lan == 'cn' %} ä¸è¡æµéåè­¦å¼ {% else %} Send network data warning
-value {% endif %} [{{ netdataSendWarning }}]
+value {% endif %} [{{ settings.netdataSendWarning }}]
 {% if lan == 'cn' %} ä¸è¡æµéåè­¦å¼ {% else %} Recv network data warning
-value {% endif %} [{{ netdataRecvWarning }}]
+value {% endif %} [{{ settings.netdataRecvWarning }}]
 {% if lan == 'cn' %} æç»­æ§è¡æ¶é´ï¼åéï¼ {% else %}
-Durationï¼minutesï¼ {% endif %} [{{ duration }}      ]
-PC HOST              SWITCH
-   [{{ solox_host }}  {% if host_switch == '1' %} * {% else %} ⁰ {% endif
-   ]                 %}
+Durationï¼minutesï¼ {% endif %} [{{ settings.duration }}]
+PC HOST                SWITCH
+   [{
+   {                    {% if settings.host_switch == '1' %} * {% else %} ⁰ {% endif
+   settings.solox_host %}
+   }}]
 {% if lan == 'cn' %} ä¿å­ {% else %} Save {% endif %}
```

### Comparing `solox-2.6.7/solox/templates/index.html` & `solox-2.6.8/solox/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends 'base.html' %}
 
 {% block title %}
 {% if lan == 'cn' %}
 SoloX - 性能测试
 {% else %}
-SoloX - APM
+SoloX - Application Performance Monitoring
 {% endif %}
 {% endblock %}
 
 {% block css %}{% endblock %}
 
 {% block page_title %}
 {% if platform == 'Android' %}
@@ -54,14 +54,21 @@
             </span>
         </a>
     </li>
 </ul>
 {% endblock %}
 
 {% block ms_auto %}
+{% if platform == 'Android' %}
+<div class="ms-auto d-print-none  col-auto">
+    <a  class="cursor-pointer"  data-bs-toggle="modal" data-bs-target="#modal-scrollable">
+        <svg t="1687917727817" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2540" width="50" height="50"><path d="M861.12 596.608L786.176 678.4c-139.936-158.4-387.04-158.4-526.976 0l-74.976-81.824c179.776-203.52 497.184-203.52 676.96 0z" fill="#080808" p-id="2541"></path><path d="M1011.808 432.896l-75.328 80.544c-219.776-248.864-607.872-248.864-827.616 0l-75.328-80.544c259.616-294.4 718.624-294.4 978.24 0z" fill="#080808" p-id="2542"></path><path d="M422.784 716.128c-50.08 50.048-50.08 128.32 0 178.4 50.08 50.08 128.32 50.08 178.432 0 50.048-50.08 50.048-128.32 0-178.4-53.248-50.24-131.52-50.24-178.432 0z" fill="#FFA115" p-id="2543"></path></svg>
+    </a>
+</div>
+{% endif %}
 <div class="ms-auto d-print-none  col-auto">
     <a class="btn btn-default" id="debug-connect">
         <svg t="1638091545450" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="231707" width="200" height="200"><path d="M207.67511 241.617978v295.694382c0 15.532584 4.602247 31.065169 13.231461 43.721348L296.268369 676.530337c13.806742 20.134831 36.242697 32.21573 60.404494 32.21573h109.303371c24.161798 0 46.597753-12.080899 60.404494-32.21573L601.742526 581.033708c8.629213-12.65618 13.231461-28.188764 13.231461-43.721348V241.617978H207.67511z" fill="#4988FD" p-id="231708"></path><path d="M253.122301 4.026966h317.555056V241.617978H253.122301z" fill="#C5DCFA" p-id="231709"></path><path d="M344.016683 184.089888c-9.204494 0-16.683146-7.478652-16.683146-16.683146V83.41573c0-9.204494 7.478652-16.683146 16.683146-16.683146 9.204494 0 16.683146 7.478652 16.683146 16.683146v83.991012c0 9.204494-7.478652 16.683146-16.683146 16.683146zM476.906571 184.089888c-9.204494 0-16.683146-7.478652-16.683146-16.683146V83.41573c0-9.204494 7.478652-16.683146 16.683146-16.683146 9.204494 0 16.683146 7.478652 16.683146 16.683146v83.991012c0 9.204494-7.478652 16.683146-16.683146 16.683146z" fill="#FFFFFF" p-id="231710"></path><path d="M606.344773 1023.424719c-118.507865 0-214.579775-96.07191-214.579775-214.579775v-28.188764c0-12.080899 9.779775-21.860674 21.860674-21.860674 12.080899 0 21.860674 9.779775 21.860674 21.860674v28.188764c0 93.770787 76.51236 170.283146 170.283146 170.283146s170.283146-76.51236 170.283146-170.283146v-231.262922c0-12.080899 9.779775-21.860674 21.860674-21.860674 12.080899 0 21.860674 9.779775 21.860675 21.860674v231.262922c0.575281 118.507865-95.496629 214.579775-213.429214 214.579775z" fill="#C5DCFA" p-id="231711"></path><path d="M439.513312 780.65618h-52.925842c-12.65618 0-23.011236-10.355056-23.011236-23.011236v-48.898877h98.373033v48.898877c0.575281 12.65618-9.779775 23.011236-22.435955 23.011236z" fill="#2767F4" p-id="231712"></path><path d="M411.899829 604.620225c-9.204494 0-16.683146-7.478652-16.683146-16.683146V335.388764c0-9.204494 7.478652-16.683146 16.683146-16.683146 9.204494 0 16.683146 7.478652 16.683146 16.683146v252.548315c-0.575281 9.779775-7.478652 16.683146-16.683146 16.683146z" fill="#FFFFFF" p-id="231713"></path><path d="M411.899829 528.683146c-3.451685 0-7.478652-1.150562-10.355056-4.026966l-65.582022-54.651686c-4.026966-2.876404-5.752809-8.053933-5.752809-12.656179v-54.076405c0-9.204494 7.478652-16.683146 16.683146-16.683146 9.204494 0 16.683146 7.478652 16.683146 16.683146v46.597753L422.830166 499.34382c6.903371 5.752809 8.053933 16.107865 2.301124 23.586517-4.026966 4.026966-8.629213 5.752809-13.231461 5.752809z" fill="#FFFFFF" p-id="231714"></path><path d="M411.899829 480.934831c-4.602247 0-9.204494-1.725843-12.65618-5.752809-5.752809-6.903371-5.177528-17.258427 1.725843-23.586516l60.979775-51.775281V362.426966c0-9.204494 7.478652-16.683146 16.683146-16.683146 9.204494 0 16.683146 7.478652 16.683147 16.683146v44.87191c0 4.602247-2.301124 9.204494-5.752809 12.65618L422.830166 476.907865c-3.451685 2.876404-7.478652 4.026966-10.930337 4.026966z" fill="#FFFFFF" p-id="231715"></path></svg>
         {% if lan == 'cn' %} 连接 {% else %} Connect {% endif %}
     </a>
 </div>
 <div class="ms-auto d-print-none  col-auto">
@@ -295,14 +302,28 @@
                 {% endif %}
             </div>
         </div>
         <pre class="mt-2" id="startup-time-content"></pre>
     </div>
   </div>
 </div>
+<div class="modal modal-blur fade" style="margin-top: 20px;margin-right: 20px;" id="modal-scrollable" tabindex="-1" role="dialog" aria-hidden="true">
+    <div class="modal-dialog  modal-full-width modal-dialog-centered modal-dialog-scrollable" role="document">
+      <div class="modal-content">
+        <div class="modal-header">
+          <h5 class="modal-title">Connect to a Android device over Wi-Fi</h5>
+          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+        </div>
+        <div class="modal-body">
+            <iframe src="https://adbshell.com/commands/adb-connect" width="100%" height="1500px"></iframe>
+        </div>
+        </div>
+      </div>
+    </div>
+  </div>
 {% endblock %}
 
 {% block js %}
 <script>
 
     var stop = false; // 任务状态
 
@@ -397,15 +418,15 @@
                 
             },
             success: function (data) {
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connection failed !', 'No pid found', 2000);
+                        SwalFire('error', 'Connect failed !', 'No pid found', 2000);
                     } 
                 }else{
                     for(var i=0;i<data['pids'].length;i++){
                         $('.select-pid').append('<option>'+data['pids'][i]+'</option>')
                     }
                     swal.close();
                 }
@@ -508,15 +529,15 @@
                                 y_app = data['appCpuRate'];
                                 y_sys = data['systemCpuRate'];
                             app_series.addPoint([x, y_app], true, true);
                             sys_series.addPoint([x, y_sys], true, true);
                             timerQ = setTimeout(getCpuRate(pkgname,device), 1000);
                         }catch (e) {}
                     }else{
-                        SwalFire('error','something error',data['msg'],2000);
+                        SwalFire('error','Something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
@@ -543,15 +564,15 @@
                             var series= gpu_chart.series[0];
                             var x = (new Date()).getTime(),
                             y = data['gpu'];
                             series.addPoint([x, y], true, true);
                             timerQ = setTimeout(getGpu(pkgname), 1000);
                         }catch (e) {}
                     }else{
-                        SwalFire('error','something error',data['msg'],2000);
+                        SwalFire('error','Something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
@@ -599,15 +620,15 @@
                                 seriesCurrent.addPoint([x, y_current], true, true);
                                 seriesVoltage.addPoint([x, y_voltage], true, true);
                                 seriesPower.addPoint([x, y_power], true, true);
                             } 
                             timerQ = setTimeout(getBattery(device), 1000);
                         }catch (e) {}
                     }else{
-                        SwalFire('error','something error',data['msg'],2000);
+                        SwalFire('error','Something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
@@ -656,15 +677,15 @@
                                     y = data['totalPass'];
                                 series.addPoint([x, y], true, true);
                             }
                             timerQ = setTimeout(getMemPss(pkgname,device), 1000);
 
                         }catch (e) {}
                     }else{
-                        SwalFire('error','something error',data['msg'],2000);
+                        SwalFire('error','Something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
@@ -687,15 +708,15 @@
                 device:device,
                 wifi_switch: net_switch,
                 type: type,
                 process:process
             },
             success: function (data) {
                 if(data['status'] != 1){
-                    SwalFire('error','something error',data['msg'],2000);
+                    SwalFire('error','Something error',data['msg'],2000);
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
         });
@@ -735,15 +756,15 @@
                             seriesUpFlow.addPoint([x_up, y_up], true, true);
                             seriesDownFlow.addPoint([x_down, y_down], true, true);
                             timerQ = setTimeout(getNetWork(pkgname,device,net_switch), 1000);
                         }catch (e) {
                             console.log(e)
                         }
                     }else{
-                        SwalFire('error','something error',data['msg'],2000);
+                        SwalFire('error','Something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
@@ -780,15 +801,15 @@
                                 let x_jsnk = (new Date()).getTime(),
                                     y_jank = data['jank'];
                                 seriesJank.addPoint([x_jsnk, y_jank], true, true);
                             }
                             timerQ = setTimeout(getFps(pkgname,device,fps_switch), 1000);
                         }catch (e) {}
                     }else{
-                        SwalFire('error','something error',data['msg'],2000);
+                        SwalFire('error','Something error',data['msg'],2000);
                     }
                 }
             },
             error: function(error){
                 SwalFire('error','Server Error','Please press [ctrl+shift+i] and provide the browser\'s error message',5000);
                 console.log(error);
             }
@@ -1088,15 +1109,14 @@
                 }
             }];
         }
         return plotLines;
     }
 
     function chartsInitialize(apmType,title){
-        //charts初始化
         let seriesFinal = series;
         let legend = false;
         let yAxis = {
             opposite:false,
             plotLines:setPlotLine(apmType)
         };
         let yAxis_plot = {
@@ -1165,49 +1185,44 @@
             series : seriesFinal
         });
 
         return apm_chart
     };
 
     function cpuInitialize(){
-        //初始化cpu
         let type = 'cpu';
         let cpu_chart = chartsInitialize(type,'CPU（%）');
         return cpu_chart
     }
 
     function batteryInitialize(){
-        //初始化battery
         let type = platform == 'Android' ? 'battery_android' : 'battery_ios';
         let battery_chart = chartsInitialize(type,'Battery');
         return battery_chart
     }
 
     function memInitialize(){
-        //初始化mem
         let type = platform == 'Android' ? 'mem_android' : 'mem_ios';
         let mem_chart = chartsInitialize(type,'Memory（MB）');
         return mem_chart
     }
 
     function networkInitialize(){
-        //初始化network
         let network_chart = chartsInitialize('network','Network Data（KB)');
         return network_chart
     }
 
     function gpuInitialize(){
         if(platform == 'iOS'){
             let gpu_chart = chartsInitialize('gpu','GPU（%）');
             return gpu_chart
         }
     }
 
     function fpsInitialize(){
-        //初始化fps
         if(platform === 'Android'){
             let title = 'FPS and Jank';
             let fps_chart = chartsInitialize('fps',title);
             return fps_chart
         }else{
             let title = 'FPS (HZ/s)';
             let fps_chart = chartsInitialize('fps_ios',title);
@@ -1220,15 +1235,14 @@
     var network_chart = networkInitialize();
     var fps_chart = fpsInitialize();
     var battery_chart = batteryInitialize();
     var gpu_chart = gpuInitialize()
 
 
     function collectPers(device,pkgname=null,type,title,func){
-        // 收集性能数据初始化
         let seriesFinal = series;
         let legend = false;
         let yAxis = {
             opposite:false,
             plotLines:setPlotLine(type)
         };
         let yAxis_plot = {
@@ -1407,14 +1421,15 @@
                     window.location.href = '/report?lan='+lan
                 }else{
                     SwalFire('error','Execution error',data['msg'],2000)
                 }
             }
         });
     }
+    
     $('#run-apm').click(function () {
         stop = false;
         $('#stop-apm').show();
         $('#run-apm').hide();
         initializeAPM();
         let device = $('.select-device').val();
         let pkgname = $('.select-app').val();
@@ -1579,15 +1594,15 @@
                     }
                 },
                 complete: function(){
                     swal.close();
                 }
             });
         }else{
-            SwalFire('error','Execution error','pkgname is empty',2000)
+            SwalFire('error','Execution error','No package found',2000)
         }
     }
 
     function install(){
         var fileObj = document.getElementById("app-file").files[0];
         var type = (fileObj) ? 'file' : 'link'
         if(type == 'file'){
@@ -1599,38 +1614,43 @@
     }
 
     function installLink(){
         var formData = new FormData();
         var link = $('.app-link').val().trim()
         formData.append('platform','{{ platform }}');
         formData.append('link',link);
-        
-        $.ajax({
-            url: "/apm/install/link",
-            type: "POST",
-            async: true,
-            cache: false,
-            processData: false,
-            contentType: false,
-            data:formData,
-            beforeSend: function () {
-                SwalLoading('Install App!','Installing file to device, please wait a moment.');
+        if(link){
+            $.ajax({
+                url: "/apm/install/link",
+                type: "POST",
+                async: true,
+                cache: false,
+                processData: false,
+                contentType: false,
+                data:formData,
+                beforeSend: function () {
+                    SwalLoading('Install App!','Installing file to device, please wait a moment.');
                 },
-            success: function (data) {
-                console.log(data);
-                if(data['status'] != 1 ) {
-                    SwalFire('error', 'Install failed !', data['msg'], 2000);
-                }else{
-                    SwalFire('success', 'Install success !', '', 2000);
+                success: function (data) {
+                    console.log(data);
+                    if(data['status'] != 1 ) {
+                        SwalFire('error', 'Install failed !', data['msg'], 2000);
+                    }else{
+                        SwalFire('success', 'Install success !', '', 2000);
+                    }
+                },
+                error:function (data) {
+                    SwalFire('error', 'Install failed !', '', 2000);
                 }
-            },
-            error:function (data) {
-                SwalFire('error', 'Install failed !', '', 2000);
-            }
-        });
+            });
+        }else{
+            SwalFire('error', 'Install failed !', 'No link found', 2000);
+        }
+        
+        
     }
 
     function installFile(){
         var formData = new FormData();
         var fileObj = document.getElementById("app-file").files[0];
         formData.append('platform','{{ platform }}');
         formData.append('file',fileObj);
```

### Comparing `solox-2.6.7/solox/templates/pk.html` & `solox-2.6.8/solox/templates/pk.html`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             </div>
             <div class="dropdown-divider"></div>
             <h6 class="dropdown-header">{% if lan == 'cn' %} 包名 {% else %} Package Name {% endif %}</h6>
             <div class="input-group mb-3 mt-2" style="width: 93%;margin-left: 10px;">
                 <div class="input-group-text">
                     <svg t="1645171258689" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2225" width="2000" height="2000"><path d="M352 96H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h192c35.2 0 64-28.8 64-64V224c0-70.4-57.6-128-128-128z m64 319.9l-0.1 0.1H224c-17 0-33-6.7-45.1-18.9S160 369 160 352V224c0-17 6.7-33 18.9-45.1S207 160 224 160h128c17 0 33 6.7 45.1 18.9S416 207 416 224v191.9zM800 96H672c-70.4 0-128 57.6-128 128v192c0 35.2 28.8 64 64 64h192c70.4 0 128-57.6 128-128V224c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 416 800 416H608.1l-0.1-0.1V224c0-17 6.7-33 18.9-45.1S655 160 672 160h128c17 0 33 6.7 45.1 18.9S864 207 864 224v128zM416 544H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V608c0-35.2-28.8-64-64-64z m0 256c0 17-6.7 33-18.9 45.1S369 864 352 864H224c-17 0-33-6.7-45.1-18.9S160 817 160 800V672c0-17 6.7-33 18.9-45.1S207 608 224 608h191.9l0.1 0.1V800zM800 544H608c-35.2 0-64 28.8-64 64v192c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V672c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 864 800 864H672c-17 0-33-6.7-45.1-18.9S608 817 608 800V608.1l0.1-0.1H800c17 0 33 6.7 45.1 18.9S864 655 864 672v128z" fill="#1875F0" p-id="2226"></path></svg>
                 </div>
-                <select id="select-app" class="select2-selection--single" data-placeholder="Please select app"></select>
+                <select id="select-app" class="select2-selection--single" data-placeholder="Please select a package"></select>
             </div>
             {% else %}
             <div class="input-group mb-3 mt-2" style="width: 93%;margin-left: 10px;">
                 <div class="input-group-text">
                     <svg t="1638090687049" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="186695" width="200" height="200"><path d="M213.33 128.002c-11.782 0-21.328 9.546-21.328 21.328v42.672c0 11.782 9.546 21.328 21.328 21.328s21.344-9.546 21.344-21.328V149.33c0-11.782-9.562-21.328-21.344-21.328zM213.33 234.674c-11.782 0-21.328 9.546-21.328 21.328v85.328c0 11.782 9.546 21.344 21.328 21.344s21.344-9.562 21.344-21.344v-85.328c0-11.782-9.562-21.328-21.344-21.328zM213.33 384.002c-11.782 0-21.328 9.546-21.328 21.326v85.344c0 11.782 9.546 21.328 21.328 21.328s21.344-9.546 21.344-21.328v-85.344c0-11.78-9.562-21.326-21.344-21.326z" fill="#434A54" p-id="186696"></path><path d="M810.686 256.002c-11.812 0-21.376 9.546-21.376 21.328v85.344c0 11.782 9.562 21.328 21.376 21.328 11.75 0 21.312-9.546 21.312-21.328v-85.344c0-11.782-9.562-21.328-21.312-21.328zM298.674 1002.652c-35.296 0-64-28.688-64-63.998V85.33c0-35.28 28.704-63.998 64-63.998h426.636c35.312 0 64 28.718 64 63.998v853.324c0 35.31-28.688 63.998-64 63.998H298.674z" fill="#434A54" p-id="186697"></path><path d="M234.674 149.33h554.636v682.668H234.674z" fill="#5D9CEC" p-id="186698"></path><path d="M725.31 0.004H298.674c-47.14 0-85.344 38.204-85.344 85.326v853.324c0 47.124 38.204 85.342 85.344 85.342h426.636c47.156 0 85.376-38.218 85.376-85.342V85.33c0-47.122-38.22-85.326-85.376-85.326z m64 938.65c0 35.31-28.688 63.998-64 63.998H298.674c-35.296 0-64-28.688-64-63.998V85.33c0-35.28 28.704-63.998 64-63.998h426.636c35.312 0 64 28.718 64 63.998v853.324z" fill="#656D78" p-id="186699"></path><path d="M512 853.342c-35.344 0-64 28.656-64 64s28.656 63.998 64 63.998c35.342 0 64-28.654 64-63.998s-28.656-64-64-64z m0 85.312c-11.766 0-21.328-9.562-21.328-21.312 0-11.782 9.562-21.344 21.328-21.344 11.764 0 21.328 9.562 21.328 21.344 0 11.75-9.562 21.312-21.328 21.312z" fill="#656D78" p-id="186700"></path><path d="M426.672 85.33c0 11.782-9.562 21.344-21.344 21.344S384 97.112 384 85.33s9.546-21.328 21.328-21.328 21.344 9.546 21.344 21.328z" fill="#5D9CEC" p-id="186701"></path><path d="M554.688 64.002h-85.358c-11.782 0-21.328 9.546-21.328 21.328s9.546 21.344 21.328 21.344h85.358c11.75 0 21.312-9.562 21.312-21.344s-9.562-21.328-21.312-21.328z" opacity=".2" p-id="186702"></path><path d="M509.33 832.216h-122.658l128.002-682.886h122.638z" fill="#FFFFFF" opacity=".1" p-id="186703"></path></svg>
                1
                 </div>
@@ -114,31 +114,31 @@
             <div class="dropdown-divider"></div>
             <h6 class="dropdown-header">{% if lan == 'cn' %} 包名 {% else %} Package Name {% endif %}</h6>
             <div class="input-group mb-3 mt-2" style="width: 93%;margin-left: 10px;">
                 <div class="input-group-text">
                     <svg t="1645171258689" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2225" width="2000" height="2000"><path d="M352 96H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h192c35.2 0 64-28.8 64-64V224c0-70.4-57.6-128-128-128z m64 319.9l-0.1 0.1H224c-17 0-33-6.7-45.1-18.9S160 369 160 352V224c0-17 6.7-33 18.9-45.1S207 160 224 160h128c17 0 33 6.7 45.1 18.9S416 207 416 224v191.9zM800 96H672c-70.4 0-128 57.6-128 128v192c0 35.2 28.8 64 64 64h192c70.4 0 128-57.6 128-128V224c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 416 800 416H608.1l-0.1-0.1V224c0-17 6.7-33 18.9-45.1S655 160 672 160h128c17 0 33 6.7 45.1 18.9S864 207 864 224v128zM416 544H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V608c0-35.2-28.8-64-64-64z m0 256c0 17-6.7 33-18.9 45.1S369 864 352 864H224c-17 0-33-6.7-45.1-18.9S160 817 160 800V672c0-17 6.7-33 18.9-45.1S207 608 224 608h191.9l0.1 0.1V800zM800 544H608c-35.2 0-64 28.8-64 64v192c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V672c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 864 800 864H672c-17 0-33-6.7-45.1-18.9S608 817 608 800V608.1l0.1-0.1H800c17 0 33 6.7 45.1 18.9S864 655 864 672v128z" fill="#1875F0" p-id="2226"></path></svg>
                 1
                 </div>
-                <select id="select-app1" class="select2-selection--single" data-placeholder="Please select app 1"></select>
+                <select id="select-app1" class="select2-selection--single" data-placeholder="Please select package 1"></select>
             </div>
             <div class="input-group mb-3 mt-2" style="width: 93%;margin-left: 10px;">
                 <div class="input-group-text">
                     <svg t="1645171258689" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2225" width="2000" height="2000"><path d="M352 96H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h192c35.2 0 64-28.8 64-64V224c0-70.4-57.6-128-128-128z m64 319.9l-0.1 0.1H224c-17 0-33-6.7-45.1-18.9S160 369 160 352V224c0-17 6.7-33 18.9-45.1S207 160 224 160h128c17 0 33 6.7 45.1 18.9S416 207 416 224v191.9zM800 96H672c-70.4 0-128 57.6-128 128v192c0 35.2 28.8 64 64 64h192c70.4 0 128-57.6 128-128V224c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 416 800 416H608.1l-0.1-0.1V224c0-17 6.7-33 18.9-45.1S655 160 672 160h128c17 0 33 6.7 45.1 18.9S864 207 864 224v128zM416 544H224c-70.4 0-128 57.6-128 128v128c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V608c0-35.2-28.8-64-64-64z m0 256c0 17-6.7 33-18.9 45.1S369 864 352 864H224c-17 0-33-6.7-45.1-18.9S160 817 160 800V672c0-17 6.7-33 18.9-45.1S207 608 224 608h191.9l0.1 0.1V800zM800 544H608c-35.2 0-64 28.8-64 64v192c0 70.4 57.6 128 128 128h128c70.4 0 128-57.6 128-128V672c0-70.4-57.6-128-128-128z m64 256c0 17-6.7 33-18.9 45.1S817 864 800 864H672c-17 0-33-6.7-45.1-18.9S608 817 608 800V608.1l0.1-0.1H800c17 0 33 6.7 45.1 18.9S864 655 864 672v128z" fill="#1875F0" p-id="2226"></path></svg>
                 2
                 </div>
-                <select id="select-app2" class="select2-selection--single" data-placeholder="Please select app 2"></select>
+                <select id="select-app2" class="select2-selection--single" data-placeholder="Please select package 2"></select>
             </div>
 
             {% endif %}
 
             <div class="dropdown-divider"></div>
             <h6 class="dropdown-header">{% if lan == 'cn' %} 性能指标 {% else %} APM Target {% endif %}</h6>
             <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="cpu_checkbox" type="checkbox" checked name="cpu"> CPU</label>
             <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="mem_checkbox" type="checkbox" checked name="mem"> Memory</label>
-            <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="flow_checkbox" type="checkbox" checked name="Network-Data"> Network Data</label>
+            <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="flow_checkbox" type="checkbox" checked name="Network-Data"> Network</label>
             <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="fps_checkbox" type="checkbox" name="fps" checked> FPS</label>
         </div>
     </div>
     <div class="apm-data mt-1" style="width: 75%;">
         <div id="cpu" class="mb-3 cpu" style="min-width:400px;height:310px"></div>
         <div id="mem"  class="mb-3 mem" style="min-width:400px;height:310px"></div>
         <div id="network" class="Network-Data mb-3" style="min-width:400px;height:310px"></div>
@@ -207,15 +207,15 @@
             },
             beforeSend: function () {
                 $('#'+element).empty();
                 $('#'+element).append('<option></option>');
             },
             success: function (data) {
                 if(data['status'] != 1 ) {
-                    SwalFire('error', 'Connet failed !', 'Please check if the device is connected', 2000)
+                    SwalFire('error', 'Connet failed !', 'No devices found', 2000)
                 }else{
                     for(var i=0;i<data['pkgnames'].length;i++){
                         $('#'+element).append('<option>'+data['pkgnames'][i]+'</option>')
                     }
                 }
             }
         });
@@ -235,15 +235,15 @@
                 $('.device1').empty();
                 $('.device2').empty();
                 SwalLoading('Device initialization!','Initializing device environment, please wait。');
                 },
             success: function (data) {
                 console.log(data);
                 if(data['status'] != 1 ) {
-                    SwalFire('error', 'Connect failed !', 'Please check if the device is connected', 2000);
+                    SwalFire('error', 'Connect failed !', 'No devices found', 2000);
                 }else{
                     if(data['devices'].length <2){
                         SwalFire('error', 'Android Devices < 2 !', 'Please check if the device nums are 2', 2000);
                     }else{
                         $('.device1').val(data['devices'][0]);
                         $('.device2').val(data['devices'][1]);
                         if(model == '2-devices'){
```

### Comparing `solox-2.6.7/solox/templates/report.html` & `solox-2.6.8/solox/templates/report.html`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,20 @@
 </div>
 {% else %}
 <div class="empty mt-5">
     <div class="empty-img">
         <img src="/static/image/empty.png">
     </div>
     <p class="empty-title">{% if lan == 'cn' %} 没有数据 {% else %} No results found {% endif %}</p>
+    <div class="empty-action">
+        <a href="/?platform=Android&lan={{ lan }}" class="btn btn-primary">
+            <svg t="1687835304508" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5468" width="50" height="50"><path d="M901.12 570.0608H187.7504V453.9392H901.12a29.0304 29.0304 0 0 1 29.0304 29.0304v58.0608a29.0304 29.0304 0 0 1-29.0304 29.0304z" fill="#ffffff" p-id="5469"></path><path d="M419.3792 807.8848L123.4944 512l295.8848-295.8848a29.0304 29.0304 0 0 1 40.96 0l40.96 40.96a28.928 28.928 0 0 1 0 40.96L287.6928 512l213.76 213.8112a28.928 28.928 0 0 1 0 40.96l-40.96 40.96a28.928 28.928 0 0 1-41.1136 0.1536z" fill="#ffffff" p-id="5470"></path></svg>
+            Start your first collection
+        </a>
+      </div>
 </div>
 {% endif %}
 
 <div class="modal modal-blur fade" id="modal-edit" tabindex="-1" role="dialog" aria-hidden="true">
     <div class="modal-dialog modal-sm modal-dialog-centered" role="document">
         <div class="modal-content">
             <div class="modal-header">
```

### Comparing `solox-2.6.7/solox/view/apis.py` & `solox-2.6.8/solox/view/apis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import shutil
 import time
 from flask import request, make_response
 from logzero import logger
 from flask import Blueprint
-import traceback
 from solox.public.apm import CPU, MEM, Flow, FPS, Battery, GPU, Target
 from solox.public.apm_pk import CPU_PK, MEM_PK, Flow_PK, FPS_PK
 from solox.public.common import Devices, File, Method, Install, Platform
 
 d = Devices()
 f = File()
 api = Blueprint("api", __name__)
@@ -43,17 +42,16 @@
 @api.route('/apm/initialize', methods=['post', 'get'])
 def initialize():
     """initialize apm env"""
     try:
         f.clear_file()
         result = {'status': 1, 'msg': 'initialize env success'}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
-
     return result
 
 
 @api.route('/device/ids', methods=['post', 'get'])
 def deviceids():
     """get devices info"""
     platform = method._request(request, 'platform')
@@ -82,35 +80,19 @@
                               'devices': deviceinfos,
                               'pkgnames': pkgnames, 
                               'device_detail': device_detail}
                 else:
                     result = {'status': 0, 'msg': 'no devices'}
             case _:
                 result = {'status': 0, 'msg': f'no this platform = {platform}'}        
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': 'devices connect error!'}
     return result
 
-# @api.route('/device/tcp/connect', methods=['post', 'get'])
-# def tcpConnect():
-#     """tcp connect """
-#     deviceid = method._request(request, 'deviceid')
-#     port = method._request(request, 'port')
-#     try:
-#         final = d.tcpConnect(deviceId=deviceid, port=port)
-#         if final == 0:
-#             result = {'status': 1, 'msg': 'success'}
-#         else:
-#             result = {'status': 0, 'msg': 'connect failed'}
-#     except Exception as e:
-#          traceback.print_exc()
-#          result = {'status': 0, 'msg': e}            
-#     return result
-
 @api.route('/device/packagenames', methods=['post', 'get'])
 def packageNames():
     """get devices packageNames"""
     platform = method._request(request, 'platform')
     device = method._request(request, 'device')
     match(platform):
         case Platform.Android:
@@ -131,55 +113,55 @@
     platform = method._request(request, 'platform')
     device = method._request(request, 'device')
     pkgname = method._request(request, 'pkgname')
     try:
         deviceId = d.getIdbyDevice(device, platform)
         pids = d.getPid(deviceId, pkgname)
         result = {'status': 1, 'pids': pids} 
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': 'no pid found'} 
     return result        
 
 @api.route('/package/activity', methods=['post', 'get'])
 def getPackageActivity():
     platform = method._request(request, 'platform')
     device = method._request(request, 'device')
     try:
         deviceId = d.getIdbyDevice(device, platform)
         activity = d.getCurrentActivity(deviceId)
         result = {'status': 1, 'activity': activity} 
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': 'no activity found'} 
     return result
 
 
 @api.route('/package/start/time/android', methods=['post', 'get'])
 def getStartupTimeByAndroid():
     platform = method._request(request, 'platform')
     device = method._request(request, 'device')
     activity = method._request(request, 'activity')
     try:
         deviceId = d.getIdbyDevice(device, platform)
         time = d.getStartupTimeByAndroid(activity, deviceId)
         result = {'status': 1, 'time': time} 
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': 'no result found'} 
     return result
 
 @api.route('/package/start/time/ios', methods=['post', 'get'])
 def getStartupTimeByiOS():
     pkgname = method._request(request, 'pkgname')
     try:
         time = d.getStartupTimeByiOS(pkgname)
         result = {'status': 1, 'time': time} 
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': 'no result found'} 
     return result
 
 @api.route('/apm/cpu', methods=['post', 'get'])
 def getCpuRate():
     """get process cpu rate"""
     model = method._request(request, 'model')
@@ -206,17 +188,17 @@
             case _:
                 process = method._request(request, 'process')
                 deviceId = d.getIdbyDevice(device, platform)
                 pid = process.split(':')[0] if platform == Platform.Android else None
                 cpu = CPU(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 appCpuRate, systemCpuRate = cpu.getCpuRate()
                 result = {'status': 1, 'appCpuRate': appCpuRate, 'systemCpuRate': systemCpuRate}        
-    except Exception:
+    except Exception as e:
         logger.error('get cpu failed')
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 1, 'appCpuRate': 0, 'systemCpuRate': 0, 'first': 0, 'second': 0}
     return result
 
 
 @api.route('/apm/mem', methods=['post', 'get'])
 def getMEM():
     """get memery data"""
@@ -244,17 +226,17 @@
             case _:
                 process = method._request(request, 'process')
                 deviceId = d.getIdbyDevice(device, platform)
                 pid = process.split(':')[0] if platform == Platform.Android else None
                 mem = MEM(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 totalPass, nativePass, dalvikPass = mem.getProcessMem()
                 result = {'status': 1, 'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}        
-    except Exception:
+    except Exception as e:
         logger.error('get memory data failed')
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 1, 'totalPass': 0, 'nativePass': 0, 'dalvikPass': 0, 'first': 0, 'second': 0}
     return result
 
 @api.route('/apm/set/network', methods=['post', 'get'])
 def setNetWorkData():
     """set network data"""
     platform = method._request(request, 'platform')
@@ -268,15 +250,15 @@
         deviceId = d.getIdbyDevice(device, platform)
         pid = process.split(':')[0] if platform == Platform.Android else None
         flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
         data = flow.setAndroidNet(wifi=wifi)
         f.record_net(type, data[0], data[1])
         result = {'status': 1, 'msg':'set network data success'}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg':'set network data failed'}
     return result        
 
 @api.route('/apm/network', methods=['post', 'get'])
 def getNetWorkData():
     """get network data"""
     model = method._request(request, 'model')
@@ -305,17 +287,17 @@
             case _:
                 process = method._request(request, 'process')
                 deviceId = d.getIdbyDevice(device, platform)
                 pid = process.split(':')[0] if platform == Platform.Android else None
                 flow = Flow(pkgName=pkgname, deviceId=deviceId, platform=platform, pid=pid)
                 data = flow.getNetWorkData(wifi=wifi,noLog=False)
                 result = {'status': 1, 'upflow': data[0], 'downflow': data[1]}    
-    except Exception:
+    except Exception as e:
         logger.error('get network data failed')
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 1, 'upflow': 0, 'downflow': 0, 'first': 0, 'second': 0}    
     return result
 
 
 @api.route('/apm/fps', methods=['post', 'get'])
 def getFps():
     """get fps data"""
@@ -343,17 +325,17 @@
                 first, second = fps.getFPS()
                 result = {'status': 1, 'first': first, 'second': second}
             case _:
                 deviceId = d.getIdbyDevice(device, platform)
                 fps_monitor = FPS(pkgName=pkgname, deviceId=deviceId, surfaceview=surfaceview, platform=platform)
                 fps, jank = fps_monitor.getFPS()
                 result = {'status': 1, 'fps': fps, 'jank': jank}       
-    except Exception:
+    except Exception as e:
         logger.error('get fps failed')
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 1, 'fps': 0, 'jank': 0, 'first': 0, 'second': 0}
     return result
 
 
 @api.route('/apm/battery', methods=['post', 'get'])
 def getBattery():
     """get Battery data"""
@@ -368,29 +350,29 @@
         else:
             result = {
                 'status': 1, 
                 'temperature': final[0], 
                 'current': final[1], 
                 'voltage': final[2], 
                 'power': final[3]}    
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 1, 'level': 0, 'temperature': 0, 'current':0, 'voltage':0 , 'power':0}
     return result
 
 @api.route('/apm/gpu', methods=['post', 'get'])
 def getGpu():
     """get gpu data"""
     pkgname = method._request(request, 'pkgname')
     try:
         gpu = GPU(pkgName=pkgname)
         final = gpu.getGPU()
         result = {'status': 1, 'gpu': final}
-    except Exception:
-        traceback.print_exc()
+    except Exception as e:
+        logger.exception(e)
         result = {'status': 1, 'gpu': 0}
     return result
 
 
 @api.route('/apm/create/report', methods=['post', 'get'])
 def makeReport():
     """Create test report records"""
@@ -412,47 +394,48 @@
             flow = Flow(pkgName=app, deviceId=deviceId, platform=platform, pid=pid)
             data = flow.setAndroidNet(wifi=wifi)
             f.record_net('end', data[0], data[1])
             app = process
         f.make_report(app=app, devices=devices, platform=platform, model=model)
         result = {'status': 1}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
 @api.route('/apm/edit/report', methods=['post', 'get'])
 def editReport():
     """Edit test report records"""
     old_scene = method._request(request, 'old_scene')
     new_scene = method._request(request, 'new_scene')
     report_dir = os.path.join(os.getcwd(), 'report')
     if old_scene == new_scene:
         result = {'status': 0, 'msg': 'scene not changed'}
-    elif os.path.exists(f'{report_dir}/{new_scene}'):
+    elif os.path.exists(os.path.join(report_dir, new_scene)):
         result = {'status': 0, 'msg': 'scene existed'}
     else:
         try:
             new_scene = new_scene.replace('/', '_').replace(' ', '').replace('&', '_')
-            os.rename(f'{report_dir}/{old_scene}', f'{report_dir}/{new_scene}')
+            os.rename(os.path.join(report_dir, old_scene), os.path.join(report_dir, new_scene))
             result = {'status': 1}
         except Exception as e:
+            logger.exception(e)
             result = {'status': 0, 'msg': str(e)}
     return result
 
 @api.route('/apm/export/report', methods=['post', 'get'])
 def exportReport():
     platform = method._request(request, 'platform')
     scene = method._request(request, 'scene')
     try:
         path = f.export_excel(platform=platform, scene=scene)
         result = {'status': 1, 'msg':'success', 'path': path}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg':str(e)}    
     return result
 
 @api.route('/apm/export/html/android', methods=['post', 'get'])
 def exportAndroidHtml():
     scene = method._request(request, 'scene')
     cpu_app = method._request(request, 'cpu_app')
@@ -484,15 +467,15 @@
         summary_dict['net_charts'] = f.getFlowLog(Platform.Android, scene)
         summary_dict['battery_charts'] = f.getBatteryLog(Platform.Android, scene)
         summary_dict['fps_charts'] = f.getFpsLog(Platform.Android, scene)['fps']
         summary_dict['jank_charts'] = f.getFpsLog(Platform.Android, scene)['jank']
         path = f.make_android_html(scene, summary_dict)
         result = {'status': 1, 'msg':'success', 'path':path}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg':str(e)}    
     return result
 
 @api.route('/apm/export/html/ios', methods=['post', 'get'])
 def exportiOSHtml():
     scene = method._request(request, 'scene')
     cpu_app = method._request(request, 'cpu_app')
@@ -524,15 +507,15 @@
         summary_dict['net_charts'] = f.getFlowLog(Platform.iOS, scene)
         summary_dict['battery_charts'] = f.getBatteryLog(Platform.iOS, scene)
         summary_dict['fps_charts'] = f.getFpsLog(Platform.iOS, scene)
         summary_dict['gpu_charts'] = f.getGpuLog(Platform.iOS, scene)
         path = f.make_ios_html(scene, summary_dict)
         result = {'status': 1, 'msg':'success', 'path':path}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg':str(e)}    
     return result    
 
 @api.route('/apm/log', methods=['post', 'get'])
 def getLogData():
     """Get apm detailed data"""
     scene = method._request(request, 'scene')
@@ -545,14 +528,15 @@
             'battery': f.getBatteryLog(platform, scene),
             'flow': f.getFlowLog(platform, scene),
             'fps': f.getFpsLog(platform, scene),
             'gpu': f.getGpuLog(platform, scene)
         }
         result = fucDic[target]
     except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
     return result
 
 @api.route('/apm/log/compare', methods=['post', 'get'])
 def getLogCompareData():
     """Get apm detailed data"""
     scene1 = method._request(request, 'scene1')
@@ -574,41 +558,44 @@
             case 'net_send':
                 result = f.getFlowSendLogCompare(platform, scene1, scene2)
             case 'net_recv':
                 result = f.getFlowRecvLogCompare(platform, scene1, scene2)                     
             case _:
                 result = {'status': 0, 'msg': 'no target found'}        
     except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
     return result
 
 @api.route('/apm/log/pk', methods=['post', 'get'])
 def getpkLogData():
     """Get apm detailed data"""
     scene = method._request(request, 'scene')
     target1 = method._request(request, 'target1')
     target2 = method._request(request, 'target2')
     try:
         first = f.readLog(scene=scene, filename=f'{target1}.log')[0]
         second = f.readLog(scene=scene, filename=f'{target2}.log')[0]
         result = {'status': 1, 'first': first, 'second': second}
     except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
 @api.route('/apm/remove/report', methods=['post', 'get'])
 def removeReport():
     """Remove test report record"""
     scene = method._request(request, 'scene')
     report_dir = os.path.join(os.getcwd(), 'report')
     try:
         shutil.rmtree(f'{report_dir}/{scene}', True)
         result = {'status': 1}
     except Exception as e:
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
     return result
 
 
 @api.route('/apm/collect', methods=['post', 'get'])
 def apmCollect():
     """apm common api"""
@@ -647,15 +634,15 @@
                     final = gpu.getGPU()
                     result = {'status': 1, 'gpu': final}
                 else:
                     result = {'status': 0, 'msg': 'not support android'}    
             case _:
                 result = {'status': 0, 'msg': 'no this target'}
     except Exception as e:
-        traceback.print_exc()
+        logger.exception(e)
         result = {'status': 0, 'msg': str(e)}
     return result
 
 @api.route('/apm/install/file', methods=['post', 'get'])
 def installFile():
     """install apk/ipa from file"""
     platform = method._request(request, 'platform')
```

### Comparing `solox-2.6.7/solox/web.py` & `solox-2.6.8/solox/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import os
 import platform
 import re
 import webbrowser
 import requests
 import socket
 import sys
-import traceback
 from solox.view.apis import api
 from solox.view.pages import page
 from logzero import logger
 from threading import Lock
 from flask_socketio import SocketIO, disconnect
 from flask import Flask
 from pyfiglet import Figlet
+from solox import __version__
 
 app = Flask(__name__, template_folder='templates', static_folder='static')
 app.register_blueprint(api)
 app.register_blueprint(page)
 
 socketio = SocketIO(app, cors_allowed_origins="*")
 thread = True
@@ -104,17 +104,17 @@
     flag = (True, False)[r.status_code == 200]
     return flag
 
 
 def openUrl(host: str, port: int):
     flag = True
     while flag:
-        logger.info('Start solox server ...')
+        logger.info('start solox server ...')
         f = Figlet(font="slant", width=300)
-        print(f.renderText("SOLOX 2. 6. 7"))
+        print(f.renderText("SOLOX {}".format(__version__)))
         flag = getServerStatus(host, port)
     webbrowser.open('http://{}:{}/?platform=Android&lan=en'.format(host, port), new=2)
     logger.info('Running on http://{}:{}/?platform=Android&lan=en (Press CTRL+C to quit)'.format(host, port))
 
 
 def startServer(host: str, port: int):
     socketio.run(app, host=host, debug=False, port=port)
```

### Comparing `solox-2.6.7/solox.egg-info/PKG-INFO` & `solox-2.6.8/solox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.7
+Version: 2.6.8
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox  (pip install solox==2.6.4)
+pip install -U solox    (pip install solox==2.6.8)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
```

### Comparing `solox-2.6.7/solox.egg-info/SOURCES.txt` & `solox-2.6.8/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

