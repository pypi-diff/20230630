# Comparing `tmp/q2gui-0.1.94.tar.gz` & `tmp/q2gui-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.94.tar", max compression
+gzip compressed data, was "q2gui-0.1.95.tar", max compression
```

## Comparing `q2gui-0.1.94.tar` & `q2gui-0.1.95.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.94/LICENSE
--rw-r--r--   0        0        0      576 2023-06-30 09:57:10.711911 q2gui-0.1.94/pyproject.toml
--rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.94/q2gui/__init__.py
--rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.94/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.94/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    18395 2023-06-25 14:11:05.710673 q2gui-0.1.94/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.94/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.94/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.94/q2gui/pyqt6/q2style.py
--rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.94/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4982 2023-06-29 15:09:52.465129 q2gui-0.1.94/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.94/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.94/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.94/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0    16742 2023-06-28 20:23:31.010565 q2gui-0.1.94/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.94/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.94/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.94/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.94/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.94/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.94/q2gui/pyqt6/widgets/q2image.py
--rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.94/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.94/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.94/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.94/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.94/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.94/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.94/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.94/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.94/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0     1115 2023-06-25 14:15:33.781067 q2gui-0.1.94/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.94/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     3397 2023-06-25 14:15:24.948690 q2gui-0.1.94/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.94/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.94/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.94/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    21225 2023-06-25 14:08:40.214841 q2gui-0.1.94/q2gui/q2app.py
--rw-r--r--   0        0        0    12944 2023-06-29 20:34:11.352834 q2gui-0.1.94/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    69557 2023-06-29 20:49:50.259604 q2gui-0.1.94/q2gui/q2form.py
--rw-r--r--   0        0        0    15709 2023-06-25 14:10:22.631445 q2gui-0.1.94/q2gui/q2model.py
--rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.94/q2gui/q2style.py
--rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.94/q2gui/q2utils.py
--rw-r--r--   0        0        0     5073 2023-06-25 14:10:45.942186 q2gui-0.1.94/q2gui/q2widget.py
--rw-r--r--   0        0        0     3814 2023-06-25 14:10:50.574661 q2gui-0.1.94/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2023-06-30 09:57:13.366191 q2gui-0.1.94/q2gui/version.py
--rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.94/README.md
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.95/LICENSE
+-rw-r--r--   0        0        0      576 2023-06-30 13:41:35.102853 q2gui-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.95/q2gui/__init__.py
+-rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.95/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.95/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    18395 2023-06-25 14:11:05.710673 q2gui-0.1.95/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.95/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.95/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.95/q2gui/pyqt6/q2style.py
+-rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.95/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4982 2023-06-29 15:09:52.465129 q2gui-0.1.95/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.95/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.95/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.95/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0    16742 2023-06-28 20:23:31.010565 q2gui-0.1.95/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.95/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.95/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.95/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.95/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.95/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.95/q2gui/pyqt6/widgets/q2image.py
+-rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.95/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.95/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.95/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.95/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.95/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.95/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.95/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.95/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.95/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0     1115 2023-06-25 14:15:33.781067 q2gui-0.1.95/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.95/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     3397 2023-06-25 14:15:24.948690 q2gui-0.1.95/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.95/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    21326 2023-06-30 13:00:29.804624 q2gui-0.1.95/q2gui/q2app.py
+-rw-r--r--   0        0        0    12944 2023-06-29 20:34:11.352834 q2gui-0.1.95/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    69603 2023-06-30 13:24:00.325657 q2gui-0.1.95/q2gui/q2form.py
+-rw-r--r--   0        0        0    15709 2023-06-25 14:10:22.631445 q2gui-0.1.95/q2gui/q2model.py
+-rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.95/q2gui/q2style.py
+-rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.95/q2gui/q2utils.py
+-rw-r--r--   0        0        0     5073 2023-06-25 14:10:45.942186 q2gui-0.1.95/q2gui/q2widget.py
+-rw-r--r--   0        0        0     3814 2023-06-25 14:10:50.574661 q2gui-0.1.95/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2023-06-30 13:41:37.311287 q2gui-0.1.95/q2gui/version.py
+-rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.95/README.md
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.95/PKG-INFO
```

### Comparing `q2gui-0.1.94/LICENSE` & `q2gui-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/pyproject.toml` & `q2gui-0.1.95/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2gui"
-version = "0.1.94"
+version = "0.1.95"
 description = "Python GUI toolkit"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
```

### Comparing `q2gui-0.1.94/q2gui/__main__.py` & `q2gui-0.1.95/q2gui/__main__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/q2app.py` & `q2gui-0.1.95/q2gui/pyqt6/q2app.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/q2form.py` & `q2gui-0.1.95/q2gui/pyqt6/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/q2model.py` & `q2gui-0.1.95/q2gui/pyqt6/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/q2style.py` & `q2gui-0.1.95/q2gui/pyqt6/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.95/q2gui/pyqt6/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/q2window.py` & `q2gui-0.1.95/q2gui/pyqt6/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/__init__.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2button.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2button.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2check.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2code.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2code.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2combo.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2combo.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2date.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2date.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2doublespin.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2doublespin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2frame.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2grid.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2grid.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2image.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2image.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2label.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2line.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2list.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2list.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2progressbar.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2progressbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2radio.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2radio.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2relation.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2relation.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2scroller.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2scroller.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2sheet.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2sheet.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2space.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2space.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2spin.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2spin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2tab.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2tab.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2text.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2text.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2toolbar.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.95/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/q2app.py` & `q2gui-0.1.95/q2gui/q2app.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 import io
 import time
 import os
 import codecs
 
 
 q2_app = None
+engine = ""
+Q2Form = None
 
 ASK_REMOVE_RECORD_TEXT = "You are about to remove current record! Are You Sure?"
 ASK_REMOVE_RECORDS_TEXT = "You are about to remove records<b>(%s)</b>! Are You Sure?"
 REMOVE_RECORD_ERROR_TEXT = "Remove record error"
 
 DATE_FORMAT_STRING = "%d.%m.%Y"
 
@@ -174,14 +176,16 @@
 from q2gui.q2style import Q2Style
 
 
 def load_q2engine(glo, engine="PyQt6"):
     from q2gui.pyqt6.q2app import Q2App as Q2App
     from q2gui.pyqt6.q2form import Q2Form as Q2Form
     from q2gui.pyqt6.q2style import Q2Style as Q2Style
+    q2app.engine = engine
+    Q2App.Q2Form = Q2Form
 
     glo["Q2App"] = Q2App
     glo["Q2Form"] = Q2Form
     glo["Q2Style"] = Q2Style
 
 
 class Q2Heap:
@@ -477,14 +481,15 @@
 
     def flush(self):
         sys.__stdout__.flush()
 
 
 class Q2App:
     Q2Style = Q2Style
+    Q2Form = None
 
     def __init__(self, title=""):
         q2app.q2_app = self
         self.window_title = title
         self.heap = Q2Heap()
         self.db = None
         self.style_file = ""
```

### Comparing `q2gui-0.1.94/q2gui/q2dialogs.py` & `q2gui-0.1.95/q2gui/q2dialogs.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/q2form.py` & `q2gui-0.1.95/q2gui/q2form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1756,15 +1756,15 @@
         self.q2_form = q2_form
 
         self.load_target()
         if self.show_main_form().ok_pressed:
             self.bulk_data_enter()
 
     def bulk_data_enter(self):
-        bulk_data_form = self.q2_form.__class__(q2app.BULK_DATA_ENTRY_TITLE)
+        bulk_data_form = self.q2_form.q2_app.Q2Form(q2app.BULK_DATA_ENTRY_TITLE)
         bulk_data_form.model = self.q2_form.model
         bulk_columns = []
         current_record = self.q2_form.get_current_record()
         for x in self.target_data:
             if x["_selected"]:
                 control = dict(x)
                 control["data"] = current_record.get(control["column"], "")
@@ -1792,15 +1792,15 @@
                 self.q2_form.w.__getattr__(bulk_column).when()
                 self.q2_form.s.__setattr__(bulk_column, bulk_data_form.s.__getattr__(bulk_column))
                 self.q2_form.w.__getattr__(bulk_column).valid()
             self.q2_form.crud_save()
         waitbar.close()
 
     def show_main_form(self):
-        self.main_form = self.q2_form.__class__(q2app.BULK_DATA_MAIN_TITLE)
+        self.main_form = self.q2_form.q2_app.Q2Form(q2app.BULK_DATA_MAIN_TITLE)
         self.main_form.add_control("/v")
         self.main_form.add_control("target_form", widget=self.target_form)
         self.main_form.cancel_button = True
         self.main_form.ok_button = True
         self.main_form.add_ok_cancel_buttons()
         self.main_form.show_form()
         return self.main_form
@@ -1809,21 +1809,21 @@
         target_row = self.target_form.current_row
         target_row_data = self.target_form.get_current_record()
         target_row_data["_selected"] = "" if target_row_data["_selected"] else "*"
         self.target_form.model.update(target_row_data, target_row)
         self.target_form.set_grid_index(target_row)
 
     def load_target(self):
-        self.target_form = self.q2_form.__class__(q2app.BULK_TARGET_TITLE)
+        self.target_form = self.q2_form.q2_app.Q2Form(q2app.BULK_TARGET_TITLE)
         self.target_data = []
         for x in self.q2_form.controls:
-            if not x["pk"] and not x["noform"]:
+            if not x["pk"] and not x["noform"] and not x["column"].startswith("/"):
                 x["target_column"] = (
                     f'{x.get("label") if x.get("label") else x.get("gridlabel")} '
-                    f'\n({self.q2_form.model.get_table_name()}.{x.get("column")})'
+                    f'({self.q2_form.model.get_table_name()}.{x.get("column")})'
                 )
                 x["_target_column"] = x.get("column")
                 x["_selected"] = ""
                 self.target_data.append(dict(x))
         self.target_form.set_model(Q2Model())
         self.target_form.model.set_records(self.target_data)
         self.target_form.add_control("target_column", q2app.BULK_TARGET_COLUMNS, control="line", datalen=100)
```

### Comparing `q2gui-0.1.94/q2gui/q2model.py` & `q2gui-0.1.95/q2gui/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/q2style.py` & `q2gui-0.1.95/q2gui/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/q2utils.py` & `q2gui-0.1.95/q2gui/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/q2widget.py` & `q2gui-0.1.95/q2gui/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/q2gui/q2window.py` & `q2gui-0.1.95/q2gui/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/README.md` & `q2gui-0.1.95/README.md`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.94/PKG-INFO` & `q2gui-0.1.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.94
+Version: 0.1.95
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

