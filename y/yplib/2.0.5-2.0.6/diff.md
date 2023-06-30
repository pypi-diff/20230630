# Comparing `tmp/yplib-2.0.5.tar.gz` & `tmp/yplib-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.0.5.tar", last modified: Fri Jun 30 03:13:52 2023, max compression
+gzip compressed data, was "dist\yplib-2.0.6.tar", last modified: Fri Jun 30 06:11:32 2023, max compression
```

## Comparing `yplib-2.0.5.tar` & `yplib-2.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 03:13:52.552239 yplib-2.0.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.5/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-30 03:13:52.551813 yplib-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 03:13:52.552239 yplib-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-30 03:13:03.000000 yplib-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:13:52.548153 yplib-2.0.5/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.5/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.5/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.5/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.5/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.5/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.5/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.5/yplib/index.py
--rw-rw-rw-   0        0        0     6240 2023-06-30 03:13:24.000000 yplib-2.0.5/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.5/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.5/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:13:52.551145 yplib-2.0.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-30 03:13:52.000000 yplib-2.0.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-30 03:13:52.000000 yplib-2.0.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 03:13:52.000000 yplib-2.0.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 03:13:52.000000 yplib-2.0.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 06:11:32.280271 yplib-2.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-30 06:11:32.280112 yplib-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 06:11:32.280271 yplib-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-30 06:06:13.000000 yplib-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:11:32.277511 yplib-2.0.6/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.6/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.6/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.6/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.6/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.6/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.6/yplib/index.py
+-rw-rw-rw-   0        0        0     6293 2023-06-30 06:10:40.000000 yplib-2.0.6/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.6/yplib/mail_html.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.6/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:11:32.279112 yplib-2.0.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-30 06:11:32.000000 yplib-2.0.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-30 06:11:32.000000 yplib-2.0.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 06:11:32.000000 yplib-2.0.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 06:11:32.000000 yplib-2.0.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.0.5/LICENSE` & `yplib-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/setup.py` & `yplib-2.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.0.5",
+  version="2.0.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.0.5/yplib/__init__.py` & `yplib-2.0.6/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/chart.py` & `yplib-2.0.6/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/chart_html.py` & `yplib-2.0.6/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/db.py` & `yplib-2.0.6/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/file.py` & `yplib-2.0.6/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/http_util.py` & `yplib-2.0.6/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/index.py` & `yplib-2.0.6/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.5/yplib/mail.py` & `yplib-2.0.6/yplib/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,21 +149,22 @@
 # }
 # data_obj = {
 # 	"调用次数": 100,
 # 	"成功次数": 50
 # }
 # title_is_none : True 代表, 里面设置的 title 是无效的, 没有 title
 # is_error      : True 代表, 里面设置的 type 是无效的, 一定是 error 类型
-def get_mail_html_one(data_obj, title_is_none=False, is_error=False):
+def get_mail_html_one(data_obj, title_is_none=None, is_error=None):
     title = data_obj['title'] if 'title' in data_obj else str(to_datetime())
     type = data_obj['type'] if 'type' in data_obj else 'normal'
-    error = type == 'error' if not is_error else is_error
     content = data_obj['content'] if 'content' in data_obj else data_obj
     stripe = False
     html_list = []
+    title = title if title_is_none is None else None if title_is_none else title
+    error = type == 'error' if is_error is None else is_error
     if isinstance(content, list) or isinstance(content, set):
         for o_c in content:
             if isinstance(o_c, dict) or isinstance(o_c, tuple):
                 for o_k in o_c:
                     html_list.extend(mail_content_html(key=o_k, value=o_c[o_k], error=error, stripe=stripe))
                     stripe = not stripe
             else:
@@ -171,8 +172,8 @@
                 stripe = not stripe
     elif isinstance(content, dict) or isinstance(content, tuple):
         for o_k in content:
             html_list.extend(mail_content_html(key=o_k, value=content[o_k], error=error, stripe=stripe))
             stripe = not stripe
     else:
         html_list.extend(mail_content_html(key=str(content), error=error, stripe=stripe))
-    return ''.join(mail_title_html(title=title if not title_is_none else None, body=html_list, error=error))
+    return ''.join(mail_title_html(title=title, body=html_list, error=error))
```

### Comparing `yplib-2.0.5/yplib/mail_html.py` & `yplib-2.0.6/yplib/mail_html.py`

 * *Files identical despite different names*

