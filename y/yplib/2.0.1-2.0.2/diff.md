# Comparing `tmp/yplib-2.0.1.tar.gz` & `tmp/yplib-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.0.1.tar", last modified: Fri Jun 30 02:46:28 2023, max compression
+gzip compressed data, was "dist\yplib-2.0.2.tar", last modified: Fri Jun 30 02:49:52 2023, max compression
```

## Comparing `yplib-2.0.1.tar` & `yplib-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:46:28.603896 yplib-2.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-30 02:46:28.603395 yplib-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 02:46:28.604053 yplib-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-30 02:46:04.000000 yplib-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:46:28.600370 yplib-2.0.1/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.1/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.1/yplib/index.py
--rw-rw-rw-   0        0        0     5730 2023-06-30 02:45:57.000000 yplib-2.0.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3851 2023-06-30 02:38:20.000000 yplib-2.0.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:46:28.602475 yplib-2.0.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-30 02:46:28.000000 yplib-2.0.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-30 02:46:28.000000 yplib-2.0.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:46:28.000000 yplib-2.0.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 02:46:28.000000 yplib-2.0.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 02:49:52.350211 yplib-2.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-30 02:49:52.349710 yplib-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:49:52.350211 yplib-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-30 02:49:27.000000 yplib-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:49:52.346506 yplib-2.0.2/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.2/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.2/yplib/index.py
+-rw-rw-rw-   0        0        0     5730 2023-06-30 02:45:57.000000 yplib-2.0.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:49:52.348181 yplib-2.0.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-30 02:49:52.000000 yplib-2.0.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-30 02:49:52.000000 yplib-2.0.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:49:52.000000 yplib-2.0.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 02:49:52.000000 yplib-2.0.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.0.1/LICENSE` & `yplib-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/setup.py` & `yplib-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.0.1",
+  version="2.0.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.0.1/yplib/__init__.py` & `yplib-2.0.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/chart.py` & `yplib-2.0.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/chart_html.py` & `yplib-2.0.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/db.py` & `yplib-2.0.2/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/file.py` & `yplib-2.0.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/http_util.py` & `yplib-2.0.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/index.py` & `yplib-2.0.2/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/mail.py` & `yplib-2.0.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.1/yplib/mail_html.py` & `yplib-2.0.2/yplib/mail_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
          '    </div>',
          '</div>']
     t = ['<div style="padding-bottom: 5px;background: white;text-align:center;">',
          '   <div style="font-size:13px;text-align:center;border-radius:5px;">',
          '       -body-',
          '   </div>',
          '</div>']
-    return list(map(lambda x: x.replace('-title-', title)
+    return list(map(lambda x: x.replace('-title-', 'title' if title is None else title)
                     .replace('-body-', ''.join(body))
                     .replace('-color-', color), t if title is None else c))
 
 
 # 邮件中的 content 的html 代码
 def mail_content_html(key=None, value=None, error=False, stripe=False):
     color_normal_1 = 'bee9c6'
```

