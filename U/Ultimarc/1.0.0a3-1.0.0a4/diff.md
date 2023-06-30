# Comparing `tmp/Ultimarc-1.0.0a3.tar.gz` & `tmp/Ultimarc-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ultimarc-1.0.0a3.tar", last modified: Mon May 22 12:38:41 2023, max compression
+gzip compressed data, was "Ultimarc-1.0.0a4.tar", last modified: Fri Jun 30 02:30:33 2023, max compression
```

## Comparing `Ultimarc-1.0.0a3.tar` & `Ultimarc-1.0.0a4.tar`

### file list

```diff
@@ -1,20 +1,190 @@
-drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-05-22 12:38:41.673649 Ultimarc-1.0.0a3/
--rw-rw-r--   0 rabram    (1000) rabram    (1000)    35149 2021-04-11 18:43:50.000000 Ultimarc-1.0.0a3/LICENSE
--rw-r--r--   0 rabram    (1000) rabram    (1000)     4526 2023-05-22 12:38:41.673649 Ultimarc-1.0.0a3/PKG-INFO
--rw-r--r--   0 rabram    (1000) rabram    (1000)     3221 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a3/README.rst
-drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-05-22 12:38:41.672649 Ultimarc-1.0.0a3/Ultimarc.egg-info/
--rw-r--r--   0 rabram    (1000) rabram    (1000)     4526 2023-05-22 12:38:41.000000 Ultimarc-1.0.0a3/Ultimarc.egg-info/PKG-INFO
--rw-r--r--   0 rabram    (1000) rabram    (1000)      355 2023-05-22 12:38:41.000000 Ultimarc-1.0.0a3/Ultimarc.egg-info/SOURCES.txt
--rw-r--r--   0 rabram    (1000) rabram    (1000)        1 2023-05-22 12:38:41.000000 Ultimarc-1.0.0a3/Ultimarc.egg-info/dependency_links.txt
--rw-r--r--   0 rabram    (1000) rabram    (1000)      100 2023-05-22 12:38:41.000000 Ultimarc-1.0.0a3/Ultimarc.egg-info/entry_points.txt
--rw-r--r--   0 rabram    (1000) rabram    (1000)       95 2023-05-22 12:38:41.000000 Ultimarc-1.0.0a3/Ultimarc.egg-info/requires.txt
--rw-r--r--   0 rabram    (1000) rabram    (1000)        9 2023-05-22 12:38:41.000000 Ultimarc-1.0.0a3/Ultimarc.egg-info/top_level.txt
--rw-r--r--   0 rabram    (1000) rabram    (1000)     1600 2023-05-22 12:38:41.674649 Ultimarc-1.0.0a3/setup.cfg
--rw-r--r--   0 rabram    (1000) rabram    (1000)      111 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a3/setup.py
-drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-05-22 12:38:41.673649 Ultimarc-1.0.0a3/ultimarc/
--rw-r--r--   0 rabram    (1000) rabram    (1000)      311 2021-04-11 18:43:50.000000 Ultimarc-1.0.0a3/ultimarc/__init__.py
--rw-rw-r--   0 rabram    (1000) rabram    (1000)     1185 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a3/ultimarc/exceptions.py
--rw-r--r--   0 rabram    (1000) rabram    (1000)     3286 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a3/ultimarc/main.py
--rw-r--r--   0 rabram    (1000) rabram    (1000)      198 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a3/ultimarc/misc.py
--rw-r--r--   0 rabram    (1000) rabram    (1000)    13937 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a3/ultimarc/system_utils.py
--rw-r--r--   0 rabram    (1000) rabram    (1000)     3554 2021-04-11 18:43:51.000000 Ultimarc-1.0.0a3/ultimarc/test_usb.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.774464 Ultimarc-1.0.0a4/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    35149 2021-04-11 18:43:50.000000 Ultimarc-1.0.0a4/LICENSE
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      112 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     4526 2023-06-30 02:30:33.774464 Ultimarc-1.0.0a4/PKG-INFO
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     3221 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/README.rst
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.762464 Ultimarc-1.0.0a4/Ultimarc.egg-info/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     4526 2023-06-30 02:30:33.000000 Ultimarc-1.0.0a4/Ultimarc.egg-info/PKG-INFO
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     5906 2023-06-30 02:30:33.000000 Ultimarc-1.0.0a4/Ultimarc.egg-info/SOURCES.txt
+-rw-r--r--   0 rabram    (1000) rabram    (1000)        1 2023-06-30 02:30:33.000000 Ultimarc-1.0.0a4/Ultimarc.egg-info/dependency_links.txt
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      104 2023-06-30 02:30:33.000000 Ultimarc-1.0.0a4/Ultimarc.egg-info/entry_points.txt
+-rw-r--r--   0 rabram    (1000) rabram    (1000)       95 2023-06-30 02:30:33.000000 Ultimarc-1.0.0a4/Ultimarc.egg-info/requires.txt
+-rw-r--r--   0 rabram    (1000) rabram    (1000)        9 2023-06-30 02:30:33.000000 Ultimarc-1.0.0a4/Ultimarc.egg-info/top_level.txt
+-rw-r--r--   0 rabram    (1000) rabram    (1000)       81 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/pyproject.toml
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     1684 2023-06-30 02:30:33.775464 Ultimarc-1.0.0a4/setup.cfg
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      111 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/setup.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.763464 Ultimarc-1.0.0a4/ultimarc/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      377 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/ultimarc/__init__.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.764464 Ultimarc-1.0.0a4/ultimarc/devices/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1287 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/devices/__init__.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)    10902 2023-05-01 22:53:13.000000 Ultimarc-1.0.0a4/ultimarc/devices/_base.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    19555 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/devices/_device.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    10904 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/devices/_mappings.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3004 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/devices/_structures.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      431 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/devices/aimtrak.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)    17610 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/devices/ipac2.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)    18357 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/devices/ipac4.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)    18810 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/devices/jpac.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)    17678 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/devices/mini_pac.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     8071 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/devices/usb_button.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.764464 Ultimarc-1.0.0a4/ultimarc/examples/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      131 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/examples/README.md
+-rw-r--r--   0 rabram    (1000) rabram    (1000)       85 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/examples/aimtrak.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3206 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/examples/ipac2.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5144 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/examples/ipac4.json
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     3118 2023-05-01 22:53:13.000000 Ultimarc-1.0.0a4/ultimarc/examples/jpac.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3212 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/examples/mini-pac.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      166 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/examples/usb-button-color.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      750 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/examples/usb-button-config.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1185 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/exceptions.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.764464 Ultimarc-1.0.0a4/ultimarc/locale/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     7059 2021-04-11 18:43:51.000000 Ultimarc-1.0.0a4/ultimarc/locale/ultimarc.pot
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     3510 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/ultimarc/main.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      198 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/misc.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.766464 Ultimarc-1.0.0a4/ultimarc/qml/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.766464 Ultimarc-1.0.0a4/ultimarc/qml/__pycache__/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)  1209185 2023-05-02 01:28:48.000000 Ultimarc-1.0.0a4/ultimarc/qml/__pycache__/rc_assets.cpython-311.pyc
+-rw-r--r--   0 rabram    (1000) rabram    (1000)  1210079 2023-05-01 22:53:17.000000 Ultimarc-1.0.0a4/ultimarc/qml/__pycache__/rc_assets.cpython-39.pyc
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      212 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/focusrect.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.760464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/1024x1024/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/1024x1024/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    47579 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/1024x1024/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.760464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/16x16/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/16x16/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      654 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/16x16/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.760464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/22x22/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/22x22/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      904 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/22x22/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.760464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/24x24/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/24x24/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1026 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/24x24/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.761464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/256x256/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.767464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/256x256/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    10300 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/256x256/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.761464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/32x32/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.768464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/32x32/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1284 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/32x32/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.761464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/48x48/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.768464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/48x48/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1966 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/48x48/apps/org.fedoraproject.MediaWriter.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.761464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/512x512/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.768464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/512x512/apps/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    21621 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/512x512/apps/org.fedoraproject.MediaWriter.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)   206082 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/mediawriter.icns
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    45509 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/mediawriter.ico
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4537 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icon/source.svg
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.768464 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      354 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/checkmark.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      401 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/dialog-error.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1725 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/dialog-information.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1396 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/edit-find.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      959 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/go-previous.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      630 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/icons/window-close.svg
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.761464 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.770464 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    23355 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/astronomy_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    39941 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/cinnamon_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    20238 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/design-suite_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    21103 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/games_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    10780 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/icon_folder.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    23984 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/jam_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    27996 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/kde_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    22595 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/lxde_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    21922 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/lxqt_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    24971 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/mate-compiz_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     8400 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/media-optical-symbolic.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    23688 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/robotics_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    19969 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/scientific_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    17436 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/security-lab_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    14232 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/server-logo_color.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    23009 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/soas_icon_grey_pattern.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    16131 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/workstation-logo_color.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    21773 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/png/xfce_icon_grey_pattern.png
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.771464 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     9932 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/astronomy_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    14057 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/cinnamon_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5180 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/design-suite_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     7407 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/games_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)   159631 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/gray_contrast.png
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3254 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/icon_folder.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     7228 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/jam_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5960 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/kde_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3602 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/lxde_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    11956 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/lxqt_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5103 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/mate-compiz_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5008 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/media-optical-symbolic.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5917 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/robotics_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5826 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/scientific_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3841 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/security-lab_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    21275 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/server-logo_color.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3136 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/soas_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    20528 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/workstation-logo_color.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5024 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/logos/svg/xfce_icon_grey_pattern.svg
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    19740 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/metadata.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    31440 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets/releases.json
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     2248 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/qml/assets.qrc
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.771464 Ultimarc-1.0.0a4/ultimarc/qml/complex/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4797 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/complex/DelegateDetail.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5873 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/complex/DelegateDevice.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1821 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/complex/IndicatedImage.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     8320 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/complex/MacroPopup.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    11383 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/complex/PacDetail.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1634 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/complex/ZoomableImage.qml
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.771464 Ultimarc-1.0.0a4/ultimarc/qml/dialogs/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      168 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/dialogs/FileDialog.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5921 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/main.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      581 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/qml.qrc
+-rw-r--r--   0 rabram    (1000) rabram    (1000)  3567477 2023-05-01 22:53:13.000000 Ultimarc-1.0.0a4/ultimarc/qml/rc_assets.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.772464 Ultimarc-1.0.0a4/ultimarc/qml/simple/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1162 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/simple/Arrow.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1130 2021-04-11 18:43:53.000000 Ultimarc-1.0.0a4/ultimarc/qml/simple/FocusRectangle.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4212 2021-10-29 22:08:08.000000 Ultimarc-1.0.0a4/ultimarc/qml/test.qml
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.772464 Ultimarc-1.0.0a4/ultimarc/qml/views/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      576 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/views/DeviceDetails.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)    12926 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/qml/views/DeviceList.qml
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      123 2021-04-11 18:43:54.000000 Ultimarc-1.0.0a4/ultimarc/qml/windowsicon.qrc
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.772464 Ultimarc-1.0.0a4/ultimarc/schemas/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      256 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/schemas/README.md
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      564 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/schemas/aimtrak.schema
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      398 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/schemas/base.schema
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4142 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/schemas/ipac2.schema
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4692 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/schemas/ipac4.schema
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     4343 2023-05-01 22:53:13.000000 Ultimarc-1.0.0a4/ultimarc/schemas/jpac.schema
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4148 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/schemas/mini-pac.schema
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      995 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/schemas/usb-button-color.schema
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     9188 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/schemas/usb-button-config.schema
+-rw-r--r--   0 rabram    (1000) rabram    (1000)    13841 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/ultimarc/system_utils.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     3554 2021-04-11 18:43:51.000000 Ultimarc-1.0.0a4/ultimarc/test_usb.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.773464 Ultimarc-1.0.0a4/ultimarc/tools/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     4692 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/ultimarc/tools/__init__.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     3177 2023-06-30 02:29:12.000000 Ultimarc-1.0.0a4/ultimarc/tools/__main__.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     2223 2021-04-11 18:43:50.000000 Ultimarc-1.0.0a4/ultimarc/tools/_tool_template.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5971 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/tools/ipac2.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     5971 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/tools/ipac4.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     5951 2023-05-01 22:53:13.000000 Ultimarc-1.0.0a4/ultimarc/tools/jpac.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     4011 2021-11-19 17:15:37.000000 Ultimarc-1.0.0a4/ultimarc/tools/list_devices.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     6149 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/tools/mini_pac.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     6138 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/tools/usb_button.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.773464 Ultimarc-1.0.0a4/ultimarc/udev/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)       99 2021-11-19 17:15:37.000000 Ultimarc-1.0.0a4/ultimarc/udev/95-ultimarc.rules
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.774464 Ultimarc-1.0.0a4/ultimarc/ui/
+-rw-r--r--   0 rabram    (1000) rabram    (1000)      131 2021-04-11 18:43:52.000000 Ultimarc-1.0.0a4/ultimarc/ui/__init__.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1424 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/action_model.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1538 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/device_class_model.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     1355 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/device_details_model.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3680 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/device_model.py
+drwxr-xr-x   0 rabram    (1000) rabram    (1000)        0 2023-06-30 02:30:33.774464 Ultimarc-1.0.0a4/ultimarc/ui/devices/
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      131 2021-11-19 17:15:37.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices/__init__.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     2953 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices/device.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     6605 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices/ipac2.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     6597 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices/ipac4.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     6661 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices/jpac.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     6687 2023-05-21 23:23:35.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices/mini_pac.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     3643 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices_filter_proxy_model.py
+-rw-r--r--   0 rabram    (1000) rabram    (1000)     5886 2023-05-01 22:53:13.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices_model.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      938 2021-10-29 22:08:08.000000 Ultimarc-1.0.0a4/ultimarc/ui/devices_sort_proxy_model.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     2660 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/macro_model.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)      682 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/pages.py
+-rw-rw-r--   0 rabram    (1000) rabram    (1000)     2668 2022-05-05 00:12:02.000000 Ultimarc-1.0.0a4/ultimarc/ui/units.py
```

### Comparing `Ultimarc-1.0.0a3/LICENSE` & `Ultimarc-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `Ultimarc-1.0.0a3/PKG-INFO` & `Ultimarc-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ultimarc
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Tools for configuring Ultimarc USB devices
 Home-page: https://github.com/katie-snow/QtPyUltimarc
 Author: Katie Snow
 Author-email: snowywhitewater@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/katie-snow/QtPyUltimarc
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Ultimarc-1.0.0a3/README.rst` & `Ultimarc-1.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `Ultimarc-1.0.0a3/Ultimarc.egg-info/PKG-INFO` & `Ultimarc-1.0.0a4/Ultimarc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ultimarc
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Tools for configuring Ultimarc USB devices
 Home-page: https://github.com/katie-snow/QtPyUltimarc
 Author: Katie Snow
 Author-email: snowywhitewater@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/katie-snow/QtPyUltimarc
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `Ultimarc-1.0.0a3/setup.cfg` & `Ultimarc-1.0.0a4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = Ultimarc
+version = 1.0.0-alpha.4
 description = Tools for configuring Ultimarc USB devices
 url = https://github.com/katie-snow/QtPyUltimarc
 author = Katie Snow
 author_email = snowywhitewater@gmail.com
 license = GNU General Public License v3 (GPLv3)
-version = 1.0.0-alpha.3
 project_urls = 
 	Homepage = https://github.com/katie-snow/QtPyUltimarc
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: MacOS :: MacOS X
@@ -28,32 +28,36 @@
 	Topic :: System :: Hardware :: Universal Serial Bus (USB)
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license_files = LICENSE
 
 [options]
 python_requires = >= 3.7
-packages = ultimarc
+packages = find_namespace:
+include_package_data = True
 install_requires = 
 	babel >= 2.12.1
 	libusb >= 1.0.26b5
 	jsonschema >= 4.17.3
 	python-easy-json >= 1.1.2
 
 [options.extras_require]
 ui = 
 	pyside6==6.5.0
 
 [options.entry_points]
 console_scripts = 
 	ultimarc = ultimarc.tools.__main__:run
 gui_scripts = 
-	ultimarc-ui = ultimarc.main
+	ultimarc-ui = ultimarc.main:run
 
 [extract_messages]
 input_dirs = ultimarc
 output_file = ultimarc/locale/ultimarc.pot
 
+[options.packages.find]
+include = ultimarc*
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `Ultimarc-1.0.0a3/ultimarc/exceptions.py` & `Ultimarc-1.0.0a4/ultimarc/exceptions.py`

 * *Files identical despite different names*

### Comparing `Ultimarc-1.0.0a3/ultimarc/main.py` & `Ultimarc-1.0.0a4/ultimarc/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #
 # This file is subject to the terms and conditions defined in the
 # file 'LICENSE', which is part of this source code package.
 #
 import logging
+import os
 import sys
 
 try:
     from PySide6 import QtCore, QtWidgets, QtQml
 except ImportError:
     print("\nError: PyUltimarc QT libraries not installed, unable to launch UI.")
     print("   To install, run: 'pip install PyUltimarc[ui]'\n")
@@ -24,16 +25,22 @@
 import ultimarc.qml.rc_assets
 
 _logger = logging.getLogger('ultimarc')
 
 _tool_cmd = _('ui')
 _tool_title = _('Ultimarc Editor')
 
-if __name__ == '__main__':
-    """ Main entry point """
+
+def run():
+    proj_path = os.path.abspath(__file__).split('/ultimarc/')[0]
+    app_base = os.path.join(proj_path, 'ultimarc')
+
+    os.environ['PYTHONPATH'] = proj_path
+
+    """ Main UI entry point """
     app = QtWidgets.QApplication(sys.argv)
     # QtQuickControls2.QQuickStyle('org.fedoraproject.AdwaitaTheme')
     # QtQuickControls2.QQuickStyle('Fusion')
 
     ToolContextManager.initialize_logging('ultimarc')  # Configure logging
 
     # Setup default argparser arguments.
@@ -73,18 +80,22 @@
         context.setContextProperty('_devices_filter', device_filter)
         context.setContextProperty('_devices', devices)
         context.setContextProperty('_device_class_model', device_class)
 
         context.setContextProperty('_units', units)
         context.setContextProperty('_pages', pages)
 
-        url = QtCore.QUrl.fromLocalFile('qml/main.qml')
+        url = QtCore.QUrl.fromLocalFile(os.path.join(app_base, 'qml/main.qml'))
 
         engine.load(url)
         if not engine.rootObjects():
             _logger.error(_('Bad UI settings found, aborting.'))
             sys.exit(-1)
 
         # Run UI loop.
         ret = app.exec_()
 
     sys.exit(ret)
+    
+if __name__ == '__main__':
+    run()
+
```

### Comparing `Ultimarc-1.0.0a3/ultimarc/system_utils.py` & `Ultimarc-1.0.0a4/ultimarc/system_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # -*- coding: utf-8 -*-
 #
 # Small helper functions for system services
 #
 # !!! This file is python 3.x compliant !!!
 #
 
-import gettext
-import json
 import logging
 import os
 import re
 import shlex
 import signal
 import subprocess
 import sys
-from datetime import datetime, date
-from json import JSONDecodeError
 
 try:
     import requests
     import urllib3
 
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 except ImportError:
```

### Comparing `Ultimarc-1.0.0a3/ultimarc/test_usb.py` & `Ultimarc-1.0.0a4/ultimarc/test_usb.py`

 * *Files identical despite different names*

