# Comparing `tmp/yplib-2.0.7.tar.gz` & `tmp/yplib-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.0.7.tar", last modified: Fri Jun 30 06:16:01 2023, max compression
+gzip compressed data, was "dist\yplib-2.0.8.tar", last modified: Fri Jun 30 06:20:14 2023, max compression
```

## Comparing `yplib-2.0.7.tar` & `yplib-2.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 06:16:01.732502 yplib-2.0.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-30 06:16:01.732000 yplib-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 06:16:01.732502 yplib-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-30 06:15:58.000000 yplib-2.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:16:01.728323 yplib-2.0.7/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.7/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.7/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.7/yplib/index.py
--rw-rw-rw-   0        0        0     6251 2023-06-30 06:15:41.000000 yplib-2.0.7/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.7/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.7/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-30 06:16:01.731103 yplib-2.0.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-30 06:16:01.000000 yplib-2.0.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-30 06:16:01.000000 yplib-2.0.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 06:16:01.000000 yplib-2.0.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 06:16:01.000000 yplib-2.0.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 06:20:14.282738 yplib-2.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-30 06:20:14.282564 yplib-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 06:20:14.283216 yplib-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-30 06:20:03.000000 yplib-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:20:14.279837 yplib-2.0.8/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.8/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.8/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.8/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.0.8/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.8/yplib/mail_html.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.8/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:20:14.281743 yplib-2.0.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 06:20:14.000000 yplib-2.0.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.0.7/LICENSE` & `yplib-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/setup.py` & `yplib-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.0.7",
+  version="2.0.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.0.7/yplib/__init__.py` & `yplib-2.0.8/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/chart.py` & `yplib-2.0.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/chart_html.py` & `yplib-2.0.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/db.py` & `yplib-2.0.8/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/file.py` & `yplib-2.0.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/http_util.py` & `yplib-2.0.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/index.py` & `yplib-2.0.8/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.7/yplib/mail.py` & `yplib-2.0.8/yplib/mail.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,32 +93,32 @@
 # 	"调用次数400",
 # 	1,
 # 	2,
 # 	4.5,
 # 	True,
 # 	"阿斯顿发到付阿斯顿发到付阿斯顿发到"
 # ]
-def get_mail_html(data_obj, title_is_none=None, is_error=None):
+def get_mail_html(data_obj, no_title=None, is_error=None):
     html_list = []
     # 如果是 list , set . 并且, 里面都是简单的对象,没有复杂对象这种, 那就使用一个发送吧
     is_simple = False
     if isinstance(data_obj, list) or isinstance(data_obj, set):
         if len(list(filter(lambda x: can_use_json(x), data_obj))) == 0:
             # 都是一些简单的对象
             is_simple = True
     if is_simple:
         # 默认有 没有 title
-        t_i_n = title_is_none if title_is_none is not None else True
-        html_list.append(get_mail_html_one(data_obj, title_is_none=t_i_n, is_error=is_error))
+        t_i_n = no_title if no_title is not None else True
+        html_list.append(get_mail_html_one(data_obj, no_title=t_i_n, is_error=is_error))
     else:
         if isinstance(data_obj, list) or isinstance(data_obj, set):
             for data_one in data_obj:
-                html_list.append(get_mail_html_one(data_one, title_is_none=title_is_none, is_error=is_error))
+                html_list.append(get_mail_html_one(data_one, no_title=no_title, is_error=is_error))
         else:
-            html_list.append(get_mail_html_one(data_obj, title_is_none=title_is_none, is_error=is_error))
+            html_list.append(get_mail_html_one(data_obj, no_title=no_title, is_error=is_error))
     return ''.join(mail_html(html_list))
 
 
 # 获得 邮件的内容信息
 # data_obj =
 # {
 # 	"title": "里面的一份小标题",
@@ -147,21 +147,21 @@
 # }
 # data_obj = {
 # 	"调用次数": 100,
 # 	"成功次数": 50
 # }
 # title_is_none : True 代表, 里面设置的 title 是无效的, 没有 title
 # is_error      : True 代表, 里面设置的 type 是无效的, 一定是 error 类型
-def get_mail_html_one(data_obj, title_is_none=None, is_error=None):
+def get_mail_html_one(data_obj, no_title=None, is_error=None):
     title = data_obj['title'] if 'title' in data_obj else str(to_datetime())
     type = data_obj['type'] if 'type' in data_obj else 'normal'
     content = data_obj['content'] if 'content' in data_obj else data_obj
     stripe = False
     html_list = []
-    title = title if title_is_none is None else None if title_is_none else title
+    title = title if no_title is None else None if no_title else title
     error = type == 'error' if is_error is None else is_error
     if isinstance(content, list) or isinstance(content, set):
         for o_c in content:
             if isinstance(o_c, dict) or isinstance(o_c, tuple):
                 for o_k in o_c:
                     html_list.extend(mail_content_html(key=o_k, value=o_c[o_k], error=error, stripe=stripe))
                     stripe = not stripe
```

### Comparing `yplib-2.0.7/yplib/mail_html.py` & `yplib-2.0.8/yplib/mail_html.py`

 * *Files identical despite different names*

