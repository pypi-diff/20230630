# Comparing `tmp/yplib-2.0.3.tar.gz` & `tmp/yplib-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.0.3.tar", last modified: Fri Jun 30 02:54:20 2023, max compression
+gzip compressed data, was "dist\yplib-2.0.4.tar", last modified: Fri Jun 30 03:09:57 2023, max compression
```

## Comparing `yplib-2.0.3.tar` & `yplib-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:54:20.927155 yplib-2.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.3/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-30 02:54:20.926990 yplib-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 02:54:20.927598 yplib-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-30 02:54:13.000000 yplib-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:54:20.923627 yplib-2.0.3/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.3/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.3/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.3/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.3/yplib/index.py
--rw-rw-rw-   0        0        0     5730 2023-06-30 02:45:57.000000 yplib-2.0.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:54:20.926338 yplib-2.0.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-30 02:54:20.000000 yplib-2.0.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-30 02:54:20.000000 yplib-2.0.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:54:20.000000 yplib-2.0.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-30 02:54:20.000000 yplib-2.0.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 03:09:57.555420 yplib-2.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-30 03:09:57.555287 yplib-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 03:09:57.555420 yplib-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-30 03:09:42.000000 yplib-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:09:57.551208 yplib-2.0.4/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.4/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.4/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.4/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6348 2023-06-30 03:08:49.000000 yplib-2.0.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.0.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 03:09:57.554364 yplib-2.0.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-30 03:09:57.000000 yplib-2.0.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-30 03:09:57.000000 yplib-2.0.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 03:09:57.000000 yplib-2.0.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 03:09:57.000000 yplib-2.0.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.0.3/LICENSE` & `yplib-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/setup.py` & `yplib-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.0.3",
+  version="2.0.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.0.3/yplib/__init__.py` & `yplib-2.0.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/chart.py` & `yplib-2.0.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/chart_html.py` & `yplib-2.0.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/db.py` & `yplib-2.0.4/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/file.py` & `yplib-2.0.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/http_util.py` & `yplib-2.0.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/index.py` & `yplib-2.0.4/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-2.0.3/yplib/mail.py` & `yplib-2.0.4/yplib/mail.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,30 +93,36 @@
 # 	"调用次数400",
 # 	1,
 # 	2,
 # 	4.5,
 # 	True,
 # 	"阿斯顿发到付阿斯顿发到付阿斯顿发到"
 # ]
-def get_mail_html(data_obj):
+def get_mail_html(data_obj, title_is_none=None, is_error=None):
     html_list = []
+    # 默认是正常的数据
+    i_e = is_error if is_error is not None else False
     # 如果是 list , set . 并且, 里面都是简单的对象,没有复杂对象这种, 那就使用一个发送吧
     is_simple = False
     if isinstance(data_obj, list) or isinstance(data_obj, set):
         if len(list(filter(lambda x: can_use_json(x), data_obj))) == 0:
             # 都是一些简单的对象
             is_simple = True
     if is_simple:
-        html_list.append(get_mail_html_one(data_obj, title_is_none=True))
+        # 默认没有 title
+        t_i_n = title_is_none if title_is_none is not None else True
+        html_list.append(get_mail_html_one(data_obj, title_is_none=t_i_n, is_error=i_e))
     else:
+        # 默认有 title
+        t_i_n = title_is_none if title_is_none is not None else False
         if isinstance(data_obj, list) or isinstance(data_obj, set):
             for data_one in data_obj:
-                html_list.append(get_mail_html_one(data_one))
+                html_list.append(get_mail_html_one(data_one, title_is_none=t_i_n, is_error=i_e))
         else:
-            html_list.append(get_mail_html_one(data_obj))
+            html_list.append(get_mail_html_one(data_obj, title_is_none=t_i_n, is_error=i_e))
     return ''.join(mail_html(html_list))
 
 
 # 获得 邮件的内容信息
 # data_obj =
 # {
 # 	"title": "里面的一份小标题",
@@ -143,29 +149,32 @@
 # 		{"成功次数2": 50},
 # 	]
 # }
 # data_obj = {
 # 	"调用次数": 100,
 # 	"成功次数": 50
 # }
-def get_mail_html_one(data_obj, title_is_none=False):
+# title_is_none : True 代表, 里面设置的 title 是无效的, 没有 title
+# is_error      : True 代表, 里面设置的 type 是无效的, 一定是 error 类型
+def get_mail_html_one(data_obj, title_is_none=False, is_error=False):
     title = data_obj['title'] if 'title' in data_obj else str(to_datetime())
     type = data_obj['type'] if 'type' in data_obj else 'normal'
+    error = type == 'error' if not is_error else is_error
     content = data_obj['content'] if 'content' in data_obj else data_obj
     stripe = False
     html_list = []
     if isinstance(content, list) or isinstance(content, set):
         for o_c in content:
             if isinstance(o_c, dict) or isinstance(o_c, tuple):
                 for o_k in o_c:
-                    html_list.extend(mail_content_html(key=o_k, value=o_c[o_k], error=type == 'error', stripe=stripe))
+                    html_list.extend(mail_content_html(key=o_k, value=o_c[o_k], error=error, stripe=stripe))
                     stripe = not stripe
             else:
-                html_list.extend(mail_content_html(key=o_c, error=type == 'error', stripe=stripe))
+                html_list.extend(mail_content_html(key=o_c, error=error, stripe=stripe))
                 stripe = not stripe
     elif isinstance(content, dict) or isinstance(content, tuple):
         for o_k in content:
-            html_list.extend(mail_content_html(key=o_k, value=content[o_k], error=type == 'error', stripe=stripe))
+            html_list.extend(mail_content_html(key=o_k, value=content[o_k], error=error, stripe=stripe))
             stripe = not stripe
     else:
-        html_list.extend(mail_content_html(key=str(content), error=type == 'error', stripe=stripe))
-    return ''.join(mail_title_html(title if not title_is_none else None, html_list, type == 'error'))
+        html_list.extend(mail_content_html(key=str(content), error=error, stripe=stripe))
+    return ''.join(mail_title_html(title=title if not title_is_none else None, body=html_list, error=error))
```

### Comparing `yplib-2.0.3/yplib/mail_html.py` & `yplib-2.0.4/yplib/mail_html.py`

 * *Files identical despite different names*

