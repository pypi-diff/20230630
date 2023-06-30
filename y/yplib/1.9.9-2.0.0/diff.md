# Comparing `tmp/yplib-1.9.9.tar.gz` & `tmp/yplib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.9.9.tar", last modified: Thu Jun 29 07:49:25 2023, max compression
+gzip compressed data, was "dist\yplib-2.0.0.tar", last modified: Fri Jun 30 02:27:40 2023, max compression
```

## Comparing `yplib-1.9.9.tar` & `yplib-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:49:25.240543 yplib-1.9.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.9.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-29 07:49:25.240151 yplib-1.9.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.9.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 07:49:25.240543 yplib-1.9.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-29 07:48:32.000000 yplib-1.9.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:49:25.235330 yplib-1.9.9/yplib/
--rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-1.9.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.9.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.9.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.9.9/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-1.9.9/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.9.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-1.9.9/yplib/index.py
--rw-rw-rw-   0        0        0     4765 2023-06-29 02:15:38.000000 yplib-1.9.9/yplib/mail.py
--rw-rw-rw-   0        0        0     3546 2023-06-28 08:18:28.000000 yplib-1.9.9/yplib/mail_html.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.9.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:49:25.239174 yplib-1.9.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 07:49:25.000000 yplib-1.9.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 02:27:40.997699 yplib-2.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-30 02:27:40.997699 yplib-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 02:27:40.998286 yplib-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-30 02:08:26.000000 yplib-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:27:40.990774 yplib-2.0.0/yplib/
+-rw-rw-rw-   0        0        0      558 2023-06-28 06:41:55.000000 yplib-2.0.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-2.0.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-2.0.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-2.0.0/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.0.0/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-2.0.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26739 2023-06-29 07:47:41.000000 yplib-2.0.0/yplib/index.py
+-rw-rw-rw-   0        0        0     5624 2023-06-30 02:26:46.000000 yplib-2.0.0/yplib/mail.py
+-rw-rw-rw-   0        0        0     3546 2023-06-28 08:18:28.000000 yplib-2.0.0/yplib/mail_html.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.0.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-30 02:27:40.996619 yplib-2.0.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-30 02:27:40.000000 yplib-2.0.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-30 02:27:40.000000 yplib-2.0.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 02:27:40.000000 yplib-2.0.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 02:27:40.000000 yplib-2.0.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.9.9/LICENSE` & `yplib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/setup.py` & `yplib-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.9.9",
+  version="2.0.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.9.9/yplib/__init__.py` & `yplib-2.0.0/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/chart.py` & `yplib-2.0.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/chart_html.py` & `yplib-2.0.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/db.py` & `yplib-2.0.0/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/file.py` & `yplib-2.0.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/http_util.py` & `yplib-2.0.0/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/index.py` & `yplib-2.0.0/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-1.9.9/yplib/mail.py` & `yplib-2.0.0/yplib/mail.py`

 * *Files 20% similar despite different names*

```diff
@@ -47,23 +47,24 @@
     #     print(e)
     #     return False
     # finally:
     smtpObj.close()
 
 
 # 获得 邮件的内容信息
-# 正常的数据
+# 正常的数据, 标准数据, 只发一个的那种
 # data_obj = {
 # 	title: "里面的一份小标题",
 # 	type: "error",
 # 	content: [
 # 		{ "调用次数": 100, "成功次数": 50 },
 # 		"总体还算可以的"
 # 	]
 # }
+# 正常的数据, 标准数据, 发几个的那种
 # data_obj = [
 # 	{
 # 		"title": "里面的一份小标题",
 # 		"type": "error",
 # 		"content": [
 # 			{ "调用次数": 100, "成功次数": 50 },
 # 			"总体还算可以的"
@@ -73,28 +74,49 @@
 # 		"title": "里面的一份正常的标题",
 # 		"content": [
 # 			{ "调用次数": 500, "成功次数": 500 },
 # 			"总体不行的"
 # 		]
 # 	}
 # ]
-#
+# 异常的数据, 也能发送, 发几个的那种
 # data_obj = [
 #     {"调用次数": 100, "成功次数": 50},
 #     {"查询次数": 200, "失败次数": 150},
 #     {"value": 735, "name": "Direct"},
 #     "总体还算可以的"
 # ]
+# 异常的数据, 也能发送, 只发一个的那种
+# data_obj = [
+# 	"调用次数100",
+# 	"调用次数200",
+# 	"调用次数300",
+# 	"调用次数400",
+# 	1,
+# 	2,
+# 	4.5,
+# 	True,
+# 	"阿斯顿发到付阿斯顿发到付阿斯顿发到"
+# ]
 def get_mail_html(data_obj):
     html_list = []
+    # 如果是 list , set . 并且, 里面都是简单的对象,没有复杂对象这种, 那就使用一个发送吧
+    is_simple = False
     if isinstance(data_obj, list) or isinstance(data_obj, set):
-        for data_one in data_obj:
-            html_list.append(get_mail_html_one(data_one))
-    else:
+        if len(list(filter(lambda x: can_use_json(x), data_obj))) == 0:
+            # 都是一些简单的对象
+            is_simple = True
+    if is_simple:
         html_list.append(get_mail_html_one(data_obj))
+    else:
+        if isinstance(data_obj, list) or isinstance(data_obj, set):
+            for data_one in data_obj:
+                html_list.append(get_mail_html_one(data_one))
+        else:
+            html_list.append(get_mail_html_one(data_obj))
     return ''.join(mail_html(html_list))
 
 
 # 获得 邮件的内容信息
 # data_obj =
 # {
 # 	"title": "里面的一份小标题",
```

### Comparing `yplib-1.9.9/yplib/mail_html.py` & `yplib-2.0.0/yplib/mail_html.py`

 * *Files identical despite different names*

