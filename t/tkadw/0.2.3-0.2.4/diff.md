# Comparing `tmp/tkadw-0.2.3.tar.gz` & `tmp/tkadw-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.2.3.tar", max compression
+gzip compressed data, was "tkadw-0.2.4.tar", max compression
```

## Comparing `tkadw-0.2.3.tar` & `tkadw-0.2.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      356 2023-06-29 05:22:01.762234 tkadw-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7009 2023-06-29 05:14:31.903998 tkadw-0.2.3/README.md
--rw-r--r--   0        0        0      469 2023-06-24 12:01:11.022261 tkadw-0.2.3/tkadw/__init__.py
--rw-r--r--   0        0        0     2058 2023-06-24 10:25:22.777909 tkadw-0.2.3/tkadw/__main__.py
--rw-r--r--   0        0        0      142 2023-06-24 02:43:29.551423 tkadw-0.2.3/tkadw/advanced/__init__.py
--rw-r--r--   0        0        0      383 2023-06-24 02:43:30.014259 tkadw-0.2.3/tkadw/advanced/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2906 2023-06-24 02:46:00.929979 tkadw-0.2.3/tkadw/advanced/__pycache__/adw.cpython-311.pyc
--rw-r--r--   0        0        0    18187 2023-06-24 02:38:22.924598 tkadw-0.2.3/tkadw/advanced/__pycache__/icon.cpython-311.pyc
--rw-r--r--   0        0        0     1598 2023-06-24 02:45:43.966706 tkadw-0.2.3/tkadw/advanced/adw.py
--rw-r--r--   0        0        0    17230 2023-06-24 02:38:22.074901 tkadw-0.2.3/tkadw/advanced/icon.py
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.2.3/tkadw/app.config
--rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.2.3/tkadw/appconfig.py
--rw-r--r--   0        0        0     7565 2023-06-24 10:30:34.831550 tkadw-0.2.3/tkadw/bilibili.py
--rw-r--r--   0        0        0     1005 2023-06-29 03:48:16.661071 tkadw-0.2.3/tkadw/canvas/__init__.py
--rw-r--r--   0        0        0     1922 2023-06-29 03:52:47.473458 tkadw-0.2.3/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.2.3/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    23294 2023-06-29 04:11:59.700720 tkadw-0.2.3/tkadw/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.2.3/tkadw/canvas/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0    43304 2023-06-29 03:53:47.268324 tkadw-0.2.3/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    24938 2023-06-29 05:04:22.047596 tkadw-0.2.3/tkadw/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0    11883 2023-06-24 12:14:29.824607 tkadw-0.2.3/tkadw/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.2.3/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4419 2023-06-24 09:52:58.175090 tkadw-0.2.3/tkadw/canvas/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0    28157 2023-06-24 11:41:35.170220 tkadw-0.2.3/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0    18171 2023-06-29 04:11:59.617413 tkadw-0.2.3/tkadw/canvas/button.py
--rw-r--r--   0        0        0     6321 2023-06-24 03:29:46.590796 tkadw-0.2.3/tkadw/canvas/checkbox.py
--rw-r--r--   0        0        0    39175 2023-06-29 03:53:47.199775 tkadw-0.2.3/tkadw/canvas/drawengine.py
--rw-r--r--   0        0        0    18633 2023-06-29 05:04:21.949962 tkadw-0.2.3/tkadw/canvas/entry.py
--rw-r--r--   0        0        0     6506 2023-06-24 12:14:29.672566 tkadw-0.2.3/tkadw/canvas/frame.py
--rw-r--r--   0        0        0     2020 2023-06-24 06:56:34.581673 tkadw-0.2.3/tkadw/canvas/label.py
--rw-r--r--   0        0        0    20506 2023-06-24 11:39:54.083259 tkadw-0.2.3/tkadw/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.2.3/tkadw/canvas/titlebar.py
--rw-r--r--   0        0        0      184 2023-06-29 05:07:18.797984 tkadw-0.2.3/tkadw/fluent/__init__.py
--rw-r--r--   0        0        0      449 2023-06-29 05:07:18.988531 tkadw-0.2.3/tkadw/fluent/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5111 2023-06-29 05:07:18.994034 tkadw-0.2.3/tkadw/fluent/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2023-06-29 05:07:18.997629 tkadw-0.2.3/tkadw/fluent/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     1932 2023-06-29 04:45:25.653229 tkadw-0.2.3/tkadw/fluent/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     4582 2023-06-29 04:53:19.399860 tkadw-0.2.3/tkadw/fluent/button.py
--rw-r--r--   0        0        0     4524 2023-06-29 05:06:31.047114 tkadw-0.2.3/tkadw/fluent/entry.py
--rw-r--r--   0        0        0      931 2023-06-29 04:45:25.512365 tkadw-0.2.3/tkadw/fluent/frame.py
--rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.2.3/tkadw/fluent/GeneralSans-Regular.ttf
--rw-r--r--   0        0        0      631 2023-06-29 05:08:33.776299 tkadw-0.2.3/tkadw/fluent/test.py
--rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.2.3/tkadw/tkite/__init__.py
--rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.2.3/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      341 2023-06-23 11:43:18.508873 tkadw-0.2.3/tkadw/tkite/gtk/__init__.py
--rw-r--r--   0        0        0      719 2023-06-23 11:43:19.769317 tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4723 2023-06-24 01:29:02.487008 tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3193 2023-06-24 01:44:55.068151 tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     2375 2023-06-24 01:51:31.925168 tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     1471 2023-06-23 11:43:19.785605 tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0     3149 2023-06-24 02:03:32.305960 tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0     4735 2023-06-24 01:29:02.053861 tkadw-0.2.3/tkadw/tkite/gtk/button.py
--rw-r--r--   0        0        0     2551 2023-06-24 01:44:54.644195 tkadw-0.2.3/tkadw/tkite/gtk/entry.py
--rw-r--r--   0        0        0     1125 2023-06-24 01:51:31.490298 tkadw-0.2.3/tkadw/tkite/gtk/frame.py
--rw-r--r--   0        0        0      359 2023-06-23 11:43:18.648390 tkadw-0.2.3/tkadw/tkite/gtk/label.py
--rw-r--r--   0        0        0     3555 2023-06-24 00:34:13.973458 tkadw-0.2.3/tkadw/tkite/gtk/notebook.py
--rw-r--r--   0        0        0     2461 2023-06-24 02:03:31.840946 tkadw-0.2.3/tkadw/tkite/gtk/textbox.py
--rw-r--r--   0        0        0    11241 2023-06-29 03:44:18.717152 tkadw-0.2.3/tkadw/win11.py
--rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 tkadw-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      356 2023-06-30 01:30:07.776396 tkadw-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7044 2023-06-30 01:30:07.797422 tkadw-0.2.4/README.md
+-rw-r--r--   0        0        0      497 2023-06-29 10:51:34.724882 tkadw-0.2.4/tkadw/__init__.py
+-rw-r--r--   0        0        0     2058 2023-06-24 10:25:22.777909 tkadw-0.2.4/tkadw/__main__.py
+-rw-r--r--   0        0        0      142 2023-06-24 02:43:29.551423 tkadw-0.2.4/tkadw/advanced/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-24 02:43:30.014259 tkadw-0.2.4/tkadw/advanced/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2906 2023-06-24 02:46:00.929979 tkadw-0.2.4/tkadw/advanced/__pycache__/adw.cpython-311.pyc
+-rw-r--r--   0        0        0    18187 2023-06-24 02:38:22.924598 tkadw-0.2.4/tkadw/advanced/__pycache__/icon.cpython-311.pyc
+-rw-r--r--   0        0        0     1598 2023-06-24 02:45:43.966706 tkadw-0.2.4/tkadw/advanced/adw.py
+-rw-r--r--   0        0        0    17230 2023-06-24 02:38:22.074901 tkadw-0.2.4/tkadw/advanced/icon.py
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.2.4/tkadw/app.config
+-rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.2.4/tkadw/appconfig.py
+-rw-r--r--   0        0        0     7565 2023-06-24 10:30:34.831550 tkadw-0.2.4/tkadw/bilibili.py
+-rw-r--r--   0        0        0     1005 2023-06-29 03:48:16.661071 tkadw-0.2.4/tkadw/canvas/__init__.py
+-rw-r--r--   0        0        0     1922 2023-06-29 03:52:47.473458 tkadw-0.2.4/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.2.4/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    23294 2023-06-29 04:11:59.700720 tkadw-0.2.4/tkadw/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.2.4/tkadw/canvas/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0    43304 2023-06-29 03:53:47.268324 tkadw-0.2.4/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    24938 2023-06-29 05:04:22.047596 tkadw-0.2.4/tkadw/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0    11883 2023-06-24 12:14:29.824607 tkadw-0.2.4/tkadw/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.2.4/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4419 2023-06-24 09:52:58.175090 tkadw-0.2.4/tkadw/canvas/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0    28157 2023-06-24 11:41:35.170220 tkadw-0.2.4/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0    18171 2023-06-29 04:11:59.617413 tkadw-0.2.4/tkadw/canvas/button.py
+-rw-r--r--   0        0        0     6321 2023-06-24 03:29:46.590796 tkadw-0.2.4/tkadw/canvas/checkbox.py
+-rw-r--r--   0        0        0    39175 2023-06-29 03:53:47.199775 tkadw-0.2.4/tkadw/canvas/drawengine.py
+-rw-r--r--   0        0        0    18633 2023-06-29 05:04:21.949962 tkadw-0.2.4/tkadw/canvas/entry.py
+-rw-r--r--   0        0        0     6506 2023-06-24 12:14:29.672566 tkadw-0.2.4/tkadw/canvas/frame.py
+-rw-r--r--   0        0        0     2020 2023-06-24 06:56:34.581673 tkadw-0.2.4/tkadw/canvas/label.py
+-rw-r--r--   0        0        0    20506 2023-06-24 11:39:54.083259 tkadw-0.2.4/tkadw/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.2.4/tkadw/canvas/titlebar.py
+-rw-r--r--   0        0        0      184 2023-06-29 05:07:18.797984 tkadw-0.2.4/tkadw/fluent/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-29 05:07:18.988531 tkadw-0.2.4/tkadw/fluent/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5111 2023-06-29 05:07:18.994034 tkadw-0.2.4/tkadw/fluent/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2023-06-29 05:07:18.997629 tkadw-0.2.4/tkadw/fluent/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     1932 2023-06-29 04:45:25.653229 tkadw-0.2.4/tkadw/fluent/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     4582 2023-06-29 04:53:19.399860 tkadw-0.2.4/tkadw/fluent/button.py
+-rw-r--r--   0        0        0     4524 2023-06-29 05:06:31.047114 tkadw-0.2.4/tkadw/fluent/entry.py
+-rw-r--r--   0        0        0      931 2023-06-29 04:45:25.512365 tkadw-0.2.4/tkadw/fluent/frame.py
+-rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.2.4/tkadw/fluent/GeneralSans-Regular.ttf
+-rw-r--r--   0        0        0      631 2023-06-29 05:08:33.776299 tkadw-0.2.4/tkadw/fluent/test.py
+-rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.2.4/tkadw/tkite/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.2.4/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      341 2023-06-23 11:43:18.508873 tkadw-0.2.4/tkadw/tkite/gtk/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-23 11:43:19.769317 tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4723 2023-06-24 01:29:02.487008 tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3193 2023-06-24 01:44:55.068151 tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     2375 2023-06-24 01:51:31.925168 tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     1471 2023-06-23 11:43:19.785605 tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0     3149 2023-06-24 02:03:32.305960 tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0     4735 2023-06-24 01:29:02.053861 tkadw-0.2.4/tkadw/tkite/gtk/button.py
+-rw-r--r--   0        0        0     2551 2023-06-24 01:44:54.644195 tkadw-0.2.4/tkadw/tkite/gtk/entry.py
+-rw-r--r--   0        0        0     1125 2023-06-24 01:51:31.490298 tkadw-0.2.4/tkadw/tkite/gtk/frame.py
+-rw-r--r--   0        0        0      359 2023-06-23 11:43:18.648390 tkadw-0.2.4/tkadw/tkite/gtk/label.py
+-rw-r--r--   0        0        0     3555 2023-06-24 00:34:13.973458 tkadw-0.2.4/tkadw/tkite/gtk/notebook.py
+-rw-r--r--   0        0        0     2461 2023-06-24 02:03:31.840946 tkadw-0.2.4/tkadw/tkite/gtk/textbox.py
+-rw-r--r--   0        0        0    11241 2023-06-29 03:44:18.717152 tkadw-0.2.4/tkadw/win11.py
+-rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 tkadw-0.2.4/PKG-INFO
```

### Comparing `tkadw-0.2.3/README.md` & `tkadw-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -235,8 +235,11 @@
 >> `223`扩展额外界面库`Win11`，根据`Sunvalley`设计
 > 
 >> `224`修复`AdwDrawButton`类边框遮挡的问题
 
 > `0.2.3`
 >> `231` `AdwDrawEngine`添加绘画渐变图形的方法
 > 
->> `232`扩展额外界面库`Fluent`，作者制作设计
+>> `232`扩展额外界面库`Fluent`，作者制作设计
+
+> `0.2.4`
+>> `241`补充导入
```

### Comparing `tkadw-0.2.3/tkadw/__main__.py` & `tkadw-0.2.4/tkadw/__main__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/advanced/__pycache__/adw.cpython-311.pyc` & `tkadw-0.2.4/tkadw/advanced/__pycache__/adw.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/advanced/__pycache__/icon.cpython-311.pyc` & `tkadw-0.2.4/tkadw/advanced/__pycache__/icon.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/advanced/adw.py` & `tkadw-0.2.4/tkadw/advanced/adw.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/advanced/icon.py` & `tkadw-0.2.4/tkadw/advanced/icon.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/appconfig.py` & `tkadw-0.2.4/tkadw/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/bilibili.py` & `tkadw-0.2.4/tkadw/bilibili.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__init__.py` & `tkadw-0.2.4/tkadw/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/button.cpython-38.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/label.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/label.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.2.4/tkadw/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/button.py` & `tkadw-0.2.4/tkadw/canvas/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/checkbox.py` & `tkadw-0.2.4/tkadw/canvas/checkbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/drawengine.py` & `tkadw-0.2.4/tkadw/canvas/drawengine.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/entry.py` & `tkadw-0.2.4/tkadw/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/frame.py` & `tkadw-0.2.4/tkadw/canvas/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/label.py` & `tkadw-0.2.4/tkadw/canvas/label.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/textbox.py` & `tkadw-0.2.4/tkadw/canvas/textbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/canvas/titlebar.py` & `tkadw-0.2.4/tkadw/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.4/tkadw/fluent/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.4/tkadw/fluent/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.4/tkadw/fluent/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/button.py` & `tkadw-0.2.4/tkadw/fluent/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/entry.py` & `tkadw-0.2.4/tkadw/fluent/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/frame.py` & `tkadw-0.2.4/tkadw/fluent/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/GeneralSans-Regular.ttf` & `tkadw-0.2.4/tkadw/fluent/GeneralSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/fluent/test.py` & `tkadw-0.2.4/tkadw/fluent/test.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc` & `tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc` & `tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc` & `tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc` & `tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/label.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.2.4/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/button.py` & `tkadw-0.2.4/tkadw/tkite/gtk/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/entry.py` & `tkadw-0.2.4/tkadw/tkite/gtk/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/frame.py` & `tkadw-0.2.4/tkadw/tkite/gtk/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/notebook.py` & `tkadw-0.2.4/tkadw/tkite/gtk/notebook.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/tkite/gtk/textbox.py` & `tkadw-0.2.4/tkadw/tkite/gtk/textbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/tkadw/win11.py` & `tkadw-0.2.4/tkadw/win11.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.2.3/PKG-INFO` & `tkadw-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.2.3
+Version: 0.2.4
 Summary: extra for tkinter
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -252,7 +252,10 @@
 > 
 >> `224`修复`AdwDrawButton`类边框遮挡的问题
 
 > `0.2.3`
 >> `231` `AdwDrawEngine`添加绘画渐变图形的方法
 > 
 >> `232`扩展额外界面库`Fluent`，作者制作设计
+
+> `0.2.4`
+>> `241`补充导入
```

