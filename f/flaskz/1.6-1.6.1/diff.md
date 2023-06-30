# Comparing `tmp/flaskz-1.6.tar.gz` & `tmp/flaskz-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.6.tar", last modified: Fri Jun 16 02:00:30 2023, max compression
+gzip compressed data, was "flaskz-1.6.1.tar", last modified: Fri Jun 30 16:00:44 2023, max compression
```

## Comparing `flaskz-1.6.tar` & `flaskz-1.6.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.283067 flaskz-1.6/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     6853 2023-06-16 02:00:30.283321 flaskz-1.6/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     6424 2023-06-15 11:25:44.000000 flaskz-1.6/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      702 2023-06-16 02:00:30.284472 flaskz-1.6/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.246590 flaskz-1.6/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.252130 flaskz-1.6/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       21 2023-06-15 02:00:26.000000 flaskz-1.6/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.257568 flaskz-1.6/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.260418 flaskz-1.6/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    12268 2023-06-15 11:27:27.000000 flaskz-1.6/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.261459 flaskz-1.6/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2256 2023-05-15 03:14:20.000000 flaskz-1.6/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.266429 flaskz-1.6/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     5488 2023-05-17 02:06:29.000000 flaskz-1.6/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    29199 2023-06-15 11:27:27.000000 flaskz-1.6/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     8353 2023-04-26 10:19:02.000000 flaskz-1.6/src/flaskz/models/_model.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6450 2023-05-27 16:43:07.000000 flaskz-1.6/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.270163 flaskz-1.6/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    19434 2023-06-15 03:31:44.000000 flaskz-1.6/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.6/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.282134 flaskz-1.6/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-05-10 07:01:15.000000 flaskz-1.6/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6/src/flaskz/utils/_magic.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     6497 2023-05-30 05:37:32.000000 flaskz-1.6/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     9086 2023-06-15 11:19:30.000000 flaskz-1.6/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     2784 2023-04-24 11:30:26.000000 flaskz-1.6/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-16 02:00:30.255860 flaskz-1.6/src/flaskz.egg-info/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6853 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      919 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-06-16 02:00:30.000000 flaskz-1.6/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.771311 flaskz-1.6.1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2022-12-30 08:48:07.000000 flaskz-1.6.1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     7075 2023-06-30 16:00:44.771673 flaskz-1.6.1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6647 2023-06-30 02:28:23.000000 flaskz-1.6.1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.6.1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      704 2023-06-30 16:00:44.773515 flaskz-1.6.1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.715405 flaskz-1.6.1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.720337 flaskz-1.6.1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       23 2023-06-30 16:00:17.000000 flaskz-1.6.1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.730228 flaskz-1.6.1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.6.1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8831 2022-09-19 02:16:30.000000 flaskz-1.6.1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.734334 flaskz-1.6.1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.6.1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-04-26 10:31:33.000000 flaskz-1.6.1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    13138 2023-06-26 06:34:52.000000 flaskz-1.6.1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.735742 flaskz-1.6.1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2390 2023-06-26 06:36:09.000000 flaskz-1.6.1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.743379 flaskz-1.6.1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     5516 2023-06-25 03:55:22.000000 flaskz-1.6.1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    29490 2023-06-20 08:28:35.000000 flaskz-1.6.1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10649 2023-06-17 12:07:38.000000 flaskz-1.6.1/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)     9352 2023-06-26 02:18:53.000000 flaskz-1.6.1/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7426 2023-06-21 08:20:49.000000 flaskz-1.6.1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.6.1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.749027 flaskz-1.6.1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    19434 2023-06-25 06:21:35.000000 flaskz-1.6.1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.6.1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3931 2023-05-16 02:55:12.000000 flaskz-1.6.1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.769925 flaskz-1.6.1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.6.1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2359 2023-05-08 02:37:05.000000 flaskz-1.6.1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2771 2023-05-16 03:06:45.000000 flaskz-1.6.1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6947 2023-04-26 10:28:36.000000 flaskz-1.6.1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    10394 2023-05-06 11:11:55.000000 flaskz-1.6.1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      839 2023-04-26 10:28:36.000000 flaskz-1.6.1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.6.1/src/flaskz/utils/_magic.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6570 2023-06-25 10:52:01.000000 flaskz-1.6.1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      961 2023-06-25 04:29:38.000000 flaskz-1.6.1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2617 2023-05-16 03:06:45.000000 flaskz-1.6.1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4522 2023-06-29 07:20:02.000000 flaskz-1.6.1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2023-06-30 16:00:44.726687 flaskz-1.6.1/src/flaskz.egg-info/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7075 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      952 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       44 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2023-06-30 16:00:44.000000 flaskz-1.6.1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.6/LICENSE` & `flaskz-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/PKG-INFO` & `flaskz-1.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.6
+Version: 1.6.1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,36 +24,39 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.1** `2023/07/01`
+    - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
+    - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
-    - [A] `BaseModelMixin`添加`count`方法，用于数量查询(全量/条件)
-    - [A] `BaseModelMixin`添加`clear_db`方法，用于清空数据
+    - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
+    - [A] `BaseModelMixin`添加`clear_db`方法, 用于清空数据
     - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
     - [A] `flaskz.ext.ssh`添加对Paramiko>=3.0.0版本的支持
     - [A] `flaskz.ext.ssh`添加`secondary_password`和`recv_endswith`参数
 - **1.5.3** `2023/06/01`
-    - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
-    - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
+    - [F] `flaskz.utils.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
+    - [A] `flaskz.utils.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 扩展`flaskz.rest`路由生成模块*
-        - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
-        - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
-        - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
-        - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
-        - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
-        - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
-        - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
-        - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
+        - 添加`register_model_route`函数, 可用于生成指定数据模型的CRUD等路由
+        - 添加`register_model_add_route`函数, 可用于生成指定数据模型的添加路由
+        - 添加`register_model_delete_route`函数, 可用于生成指定数据模型的删除路由
+        - 添加`register_model_update_route`函数, 可用于生成指定数据模型的更新路由
+        - 添加`register_model_upsert_route`函数, 可用于生成指定数据模型的添加/更新路由
+        - 添加`register_model_query_route`函数, 可用于生成指定数据模型的全量查询路由
+        - 添加`register_model_query_pss_route`函数, 可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
+        - 添加`register_models_query_route`函数, 可用于生成多个数据模型的全量查询路由
     - [A] `ModelMixin.query_pss`方法支持多列排序*
     - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
     - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
     - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
     - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
     - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决Flask<2.2.3版本不会将结尾不带`/`的请求重定向到带`/`路由的问题
```

### Comparing `flaskz-1.6/README.md` & `flaskz-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,36 +9,39 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.1** `2023/07/01`
+    - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
+    - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
-    - [A] `BaseModelMixin`添加`count`方法，用于数量查询(全量/条件)
-    - [A] `BaseModelMixin`添加`clear_db`方法，用于清空数据
+    - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
+    - [A] `BaseModelMixin`添加`clear_db`方法, 用于清空数据
     - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
     - [A] `flaskz.ext.ssh`添加对Paramiko>=3.0.0版本的支持
     - [A] `flaskz.ext.ssh`添加`secondary_password`和`recv_endswith`参数
 - **1.5.3** `2023/06/01`
-    - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
-    - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
+    - [F] `flaskz.utils.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
+    - [A] `flaskz.utils.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 扩展`flaskz.rest`路由生成模块*
-        - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
-        - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
-        - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
-        - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
-        - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
-        - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
-        - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
-        - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
+        - 添加`register_model_route`函数, 可用于生成指定数据模型的CRUD等路由
+        - 添加`register_model_add_route`函数, 可用于生成指定数据模型的添加路由
+        - 添加`register_model_delete_route`函数, 可用于生成指定数据模型的删除路由
+        - 添加`register_model_update_route`函数, 可用于生成指定数据模型的更新路由
+        - 添加`register_model_upsert_route`函数, 可用于生成指定数据模型的添加/更新路由
+        - 添加`register_model_query_route`函数, 可用于生成指定数据模型的全量查询路由
+        - 添加`register_model_query_pss_route`函数, 可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
+        - 添加`register_models_query_route`函数, 可用于生成多个数据模型的全量查询路由
     - [A] `ModelMixin.query_pss`方法支持多列排序*
     - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
     - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
     - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
     - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
     - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决Flask<2.2.3版本不会将结尾不带`/`的请求重定向到带`/`路由的问题
```

### Comparing `flaskz-1.6/setup.cfg` & `flaskz-1.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.6
+version = 1.6.1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.6/src/flaskz/auth/_jws.py` & `flaskz-1.6.1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/ext/cypher.py` & `flaskz-1.6.1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/ext/ssh.py` & `flaskz-1.6.1/src/flaskz/ext/ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,35 +88,53 @@
     def channel(self):
         if not hasattr(self, '_channel'):
             self._channel = self.ssh.invoke_shell(height=100000)
             if self._timeout > 0:
                 self._channel.settimeout(self._timeout)
         return self._channel
 
-    def run_command(self, command):
+    def run_command(self, command, recv=True):
         """
         Run the command.
+        If recv is False, just run the command and return immediately, without waiting for the result
+
+        .. versionupdated:: 1.6.1   - @2023-06-26 add recv parameter
 
         Example:
             ssh.run_command('ls -l')
             ssh.run_command('show run')
+
+         :param command: the command to run.
+         :param recv: wait for the result or not.
+
+         :return: the output of the command
         """
-        command = command.strip()
-        self.channel.send(command + '\n')
-        output = self._get_output(command)
+        if type(command) is dict:
+            _command = command.get('command')
+            _recv = command.get('recv') is not False
+        else:
+            _command = command
+            _recv = recv
+
+        _command = _command.strip()
+        self.channel.send(_command + '\n')
+        if _recv is False:
+            return None
+
+        output = self._get_output(_command)
         enable_commands = ('sudo', 'enable')
         secondary_password = self._secondary_password  # or self._password
         if secondary_password and \
-                command.lower().startswith(enable_commands) and \
+                _command.lower().startswith(enable_commands) and \
                 'assword' in output:  # input password
             pwd_output = self.run_command(secondary_password)
             # if 'assword' in pwd_output:
             if pwd_output == output:
                 return output
-            return self.run_command(command)
+            return self.run_command(_command)
 
         return output
 
     def run_command_list(self, command_list, last_result=False):
         """
         Run a command list.
         By default, returns the list of results , if last_result==True returns the result of the last command
@@ -124,14 +142,19 @@
         Example:
             ssh.run_command_list(['cd /usr/projects/git/srte',
                       'pwd',
                       'git pull origin master',
                       'wiui@hotmail.com',
                       '11111111'
                       ], True)
+
+         :param command_list: the command list to run.
+         :param last_result: if True, return the result of the last command, otherwise, return the result list
+
+         :return: command output result(list/last)
         """
         re_list = []
         for command in command_list:
             re_list.append(self.run_command(command))
         if last_result is True:
             return re_list[-1]
         return re_list
@@ -286,22 +309,23 @@
     if path[-1] == '/':
         return path[0:-1]
     return path
 
 
 if __name__ == '__main__':
     servers = [
-        # {  # C9300
-        #     'host': '10.75.37.165',
-        #     'username': 'admin',
-        #     'password': 'Cisco123',
-        #     # 'secondary_password': 'Cisco123',
-        #     'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
-        #     'commands': ['enable', 'Cisco123', 'show run']
-        # },
+        {  # C9300
+            'host': '10.75.37.165',
+            'username': 'admin',
+            'password': 'Cisco123',
+            # 'secondary_password': 'Cisco123',
+            'recv_endswith': ['# ', '$ ', ': ', '? ', '#'],
+            'commands': ['enable', 'Cisco123', {'command': 'show run', 'wait': False}]
+            # 'commands': ['show run']
+        },
         # {  # Centos
         #     'host': '10.124.4.21',
         #     'username': 'admin1',
         #     'password': 'Cisco@123',
         #     'commands': ['show int eth3/1']
         # },
         # {  # Centos
@@ -312,21 +336,21 @@
         # },
         # {  # Ubuntu
         #     'host': '10.124.5.198',
         #     'username': 'root',
         #     'password': 'Cisco@123',
         #     'commands': ['ls -l']
         # },
-        {  # Ubuntu, test input password
-            'host': '10.124.5.216',
-            'username': 'cisco',
-            'password': 'cisco123',
-            'secondary_password': 'cisco123',
-            'commands': ['sudo ls -l']
-        },
+        # {  # Ubuntu, test input password
+        #     'host': '10.124.5.216',
+        #     'username': 'cisco',
+        #     'password': 'cisco123',
+        #     'secondary_password': 'cisco123',
+        #     'commands': ['sudo ls -l']
+        # },
         # {  # NX-OS
         #     'host': '10.124.11.134',
         #     'username': 'admin',
         #     'password': 'Cisco@123',
         #     'commands': ['show version', 'show running-config']
         # },
         # {  # NX-OS
```

### Comparing `flaskz-1.6/src/flaskz/log/__init__.py` & `flaskz-1.6.1/src/flaskz/log/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,29 @@
     """
     app_config = get_app_config_items(app) or {}
     level = logging.getLevelName(app_config.get('FLASKZ_LOGGER_LEVEL'))
     formatter = logging.Formatter(app_config.get('FLASKZ_LOGGER_FORMAT'))
     global _flaskz_logger
     _flaskz_logger = logging.getLogger('flaskz_logger')
     _flaskz_logger.setLevel(level)
-    filename = app_config.get('FLASKZ_LOGGER_FILENAME')
 
-    if filename is not None:
-        filepath = os.path.join(app_config.get('FLASKZ_LOGGER_FILEPATH') or os.path.join(os.getcwd(), './syslog'), filename)
-        log_handler = TimedRotatingFileHandler(
-            encoding='utf-8',
-            filename=filepath,
-            when=app_config.get('FLASKZ_LOGGER_WHEN'),
-            interval=1,
-            backupCount=int(app_config.get('FLASKZ_LOGGER_BACKUP_COUNT')))
-    else:
-        log_handler = logging.StreamHandler()
+    log_handler = app_config.get('FLASKZ_LOGGER_HANDLER')
+    if log_handler is None:
+        filename = app_config.get('FLASKZ_LOGGER_FILENAME')
+
+        if filename is not None:
+            filepath = os.path.join(app_config.get('FLASKZ_LOGGER_FILEPATH') or os.path.join(os.getcwd(), './syslog'), filename)
+            log_handler = TimedRotatingFileHandler(
+                encoding='utf-8',
+                filename=filepath,
+                when=app_config.get('FLASKZ_LOGGER_WHEN'),
+                interval=1,
+                backupCount=int(app_config.get('FLASKZ_LOGGER_BACKUP_COUNT')))
+        else:
+            log_handler = logging.StreamHandler()
 
     log_handler.setLevel(level)
     log_handler.setFormatter(formatter)
     _flaskz_logger.addHandler(log_handler)
     _flaskz_logger.disabled = app_config.get('FLASKZ_LOGGER_DISABLED') is True
 
     wz_logger = logging.getLogger('werkzeug')
```

### Comparing `flaskz-1.6/src/flaskz/models/__init__.py` & `flaskz-1.6.1/src/flaskz/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,9 +124,10 @@
                             flaskz_logger.warning('Slow queries:\n' + ('\n'.join(slow_queries)))
                 return response
 
 
 from ._base import *
 from ._model import *
 from ._util import *
+from ._query_util import *
 
 from ..utils import get_app_config_items
```

### Comparing `flaskz-1.6/src/flaskz/models/_base.py` & `flaskz-1.6.1/src/flaskz/models/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 
     @classmethod
     def add_db(cls, data):
         """
         Add data to the db.
 
         Example:
-            User.add_db({"name": "taozh", "email": "taozh@focus-ui.com"})
+            ins = User.add_db({"name": "taozh", "email": "taozh@focus-ui.com"})
 
         :param data:
         :return:
         """
         instance = create_instance(cls, data)
         with db_session() as session:
             session.add(instance)
@@ -365,15 +365,15 @@
     @classmethod
     def update_db(cls, data):
         """
         Update the data to the db. The primary key value must be in data.
         Only the fields in data will be updated.
 
         Example:
-            User.update_db({"id": 1, "email": "taozh@focus-ui.com"})
+            ins = User.update_db({"id": 1, "email": "taozh@focus-ui.com"})
 
         :param data:
         :return:
         """
         pk_value = cls._get_pk_value(data)
         if pk_value is None:  # pk value does not exist
             return res_status_codes.db_data_not_found
@@ -439,16 +439,16 @@
 
     @classmethod
     def delete_db(cls, pk_value):
         """
         Delete the specified data with the specified primary key value.
 
         Example:
-            User.delete_db(1)   # pk
-            User.delete_db({'id': 1})   # dict
+            ins = User.delete_db(1)   # pk
+            ins = User.delete_db({'id': 1})   # dict
 
         :param pk_value:
         :return:
         """
         if pk_value is None:  # Object does not exist
             return res_status_codes.db_data_not_found
         with db_session() as session:  # @2022-12-01 change to ensure the deleted instance and the delete action in the same session
@@ -542,15 +542,15 @@
     def query_by_unique_key(cls, data):
         """
         Query data by the unique values.
         --If exist,returns the instance.
         --Otherwise,returns None
 
         Example:
-            User.query_by_unique_key(data)
+            ins = User.query_by_unique_key(data)
 
         :param data:
         :return:
         """
         cols = cls.get_unique_columns()
         if len(cols) == 0:
             return None
@@ -572,15 +572,15 @@
 
     @classmethod
     def query_by_pk(cls, pk_value):
         """
         Query by pk value.
 
         Example:
-            User.query_by_pk(1)
+            ins = User.query_by_pk(1)
 
         :param pk_value:
         :return:
         """
         with db_session(do_commit=False) as session:
             instance = session.query(cls).get(pk_value)
         return instance
@@ -589,16 +589,16 @@
     def query_by(cls, by_dict, return_first=False):
         """
         Query by dict object.
         -If first is not True, return the list result of the query.
         -If first is True, return the first row object or None.
 
         Example:
-            User.query_by({'name': 'flaskz'})   # list
-            User.query_by({'name': 'flaskz'}, True) # first row
+            ins_list = User.query_by({'name': 'flaskz'})   # list
+            ins = User.query_by({'name': 'flaskz'}, True) # first row
 
         """
         with db_session(do_commit=False) as session:
             if return_first is True:
                 result = session.query(cls).filter_by(**by_dict).limit(1).first()
             else:
                 result = session.query(cls).filter_by(**by_dict).all()
@@ -606,15 +606,15 @@
 
     @classmethod
     def query_all(cls):
         """
         Query all the data of the model class.
 
         Example:
-            User.query_all()
+            ins_list = User.query_all()
 
         :return:
         """
         query_order = cls.get_query_default_order()
         with db_session(do_commit=False) as session:
             query = session.query(cls)
             if query_order is not None:
@@ -626,15 +626,15 @@
     def query_pss(cls, pss_option):
         """
         Query data by search, pagination and sort condition.
         Please use flaskz.utils.get_pss to parse option first.
         pss = page+search+sort
 
         Example:
-            result, result = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
+            result = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
                 TemplateModel, {   # FROM templates
                     "search": {                         # WHERE
                         "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
                         "age": {                        # AND (age>1 AND age<20)
                             ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
                             "<": 20
                         },
@@ -736,20 +736,23 @@
         if len(orders) == 0:  # @2023-05-04 fix
             orders = [cls.get_query_default_order()]  # default order
         orders = [item for item in orders if item is not None]
 
         with db_session(do_commit=False) as session:
             query = session.query(cls)
 
-            if len(filter_likes) > 0:
-                query = query.filter(text('(' + (' OR '.join(filter_likes)) + ')'))
-            if len(filter_ands) > 0:
-                query = query.filter(text('(' + (' AND '.join(filter_ands)) + ')'))
-            if len(filter_ors) > 0:
-                query = query.filter(text('(' + (' OR '.join(filter_ors)) + ')'))
+            query = append_query_filter(query, filter_likes, 'or')
+            query = append_query_filter(query, filter_ands, 'and')
+            query = append_query_filter(query, filter_ors, 'or')
+            # if len(filter_likes) > 0:
+            #     query = query.filter(text('(' + (' OR '.join(filter_likes)) + ')'))
+            # if len(filter_ands) > 0:
+            #     query = query.filter(text('(' + (' AND '.join(filter_ands)) + ')'))
+            # if len(filter_ors) > 0:
+            #     query = query.filter(text('(' + (' OR '.join(filter_ors)) + ')'))
 
             # if len(distinct) > 0:
             #     query.distinct(*distinct)
 
             if len(group) > 0:  # @2023-06-07 add
                 query = query.group_by(*group)
 
@@ -828,8 +831,8 @@
             attrs.append(field + '=' + str(getattr(self, field, None)))
         return cls.get_class_name() + '(' + (', '.join(attrs)) + ')'
 
     # -------------------------------------------new-------------------------------------------
 
 
 # must
-from ._util import create_instance, create_relationships, db_session
+from ._util import create_instance, create_relationships, db_session, append_query_filter
```

### Comparing `flaskz-1.6/src/flaskz/models/_model.py` & `flaskz-1.6.1/src/flaskz/models/_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     def add(cls, data):
         """
          Add the data to the db.
          Returns a tuple.
            --the first value represents whether the add operation was successful, True/False.
            --the second value represent the result of the add operation, reason/instance.
 
+        Example:
+            success, ins = User.add({"name": "taozh", "email": "taozh@focus-ui.com"})
+
         :param data:
         :return:
         """
         instance = None
         try:
             data = cls.get_add_data(data)
             check_result = cls.check_add_data(data)
@@ -116,14 +119,17 @@
     def update(cls, data):
         """
         Update the data to the db.
         Returns a tuple.
            --the first value represents whether the update operation was successful, True/False.
            --the second value represent the result of the update operation, reason/instance.
 
+        Example:
+            success, ins = User.update({"id": 1, "email": "taozh@focus-ui.com"})
+
         :param data:
         :return:
         """
         instance = None
         try:
             data = cls.get_update_data(data)
             check_result = cls.check_update_data(data)
@@ -182,14 +188,18 @@
     def delete(cls, pk_value):
         """
         Delete the data from the db.
         Returns a tuple.
            --the first value represents whether the delete operation was successful, True/False.
            --the second value represent the result of the delete operation, reason/instance.
 
+        Example:
+            success, ins =  User.delete(1)
+            success, ins =  User.delete({'id': 1})
+
         :param pk_value:
         :return:
         """
         if is_dict(pk_value):  # {id:10}
             pk_value = cls._get_pk_value(pk_value)
 
         instance = None
@@ -217,28 +227,65 @@
     # -------------------------------------------query-------------------------------------------
     @classmethod
     def query_all(cls):
         """
         Override the base query_all method and return success flag.
         Used in router to return query data.
 
+        Example:
+            success, ins_list = User.query_all()
+
         :return:
         """
         try:
             return True, super().query_all()
         except Exception as e:
             flaskz_logger.exception(e)
             return False, res_status_codes.db_query_err
 
     @classmethod
     def query_pss(cls, pss_option):
         """
         Override the base query_pss method and return success flag.
         Used in router to return query data.
 
+        Example:
+            result, ins_list = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
+                TemplateModel, {   # FROM templates
+                    "search": {                         # WHERE
+                        "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
+                        "age": {                        # AND (age>1 AND age<20)
+                            ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
+                            "<": 20
+                        },
+                        "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
+                        "_ors": {                       # AND (country='America' OR country='Canada')
+                            "country": "America||Canada"
+                        },
+                        "_ands": {                      # AND (grade>1 AND grade<5)
+                            "grade": {
+                                ">": 1,
+                                "<": 5
+                            }
+                        }
+                    },
+                    "sort": {                           # ORDER BY templates.name ASC
+                        "field": "name",
+                        "order": "asc"
+                    },
+                    # "sort":[                          # ORDER BY templates.name ASC, templates.age DESC
+                    #     {"field": "name", "order": "asc"},
+                    #     {field": "age", "order": "desc"}
+                    # ],
+                    "page": {                           # LIMIT ? OFFSET ? (20, 0)
+                        "offset": 0,
+                        "size": 20
+                    }
+                }))
+
         :param pss_option:
         :return:
         """
         try:
             return True, super().query_pss(pss_option)
         except Exception as e:
             flaskz_logger.exception(e)
```

### Comparing `flaskz-1.6/src/flaskz/models/_util.py` & `flaskz-1.6.1/src/flaskz/models/_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import contextmanager
 
 from flask import g
+from sqlalchemy import text, or_, and_
 
 from . import DBSession
 from ._base import BaseModelMixin
 from ..utils import get_g_cache, set_g_cache
 
 __all__ = ['create_instance', 'create_relationships',
            'query_all_models', 'query_multiple_model',
@@ -222,7 +223,44 @@
 def _has_g_context():
     # if has_request_context():  # If there is request context, g must exist
     #     return True
     if not g:  # @2022-11-28: change, (not g) != (g is None)
         return False
     return True
     # return has_request_context() or g is not None
+
+
+def append_query_filter(query, filters, joined):  # @2023-06-21 add
+    """
+    Append filters to the query
+    :param query:
+    :param filters:
+    :param joined:
+    :return:
+    """
+    if len(filters) == 0:
+        return query
+    joined = joined.lower()
+    if joined == 'or':
+        joined_text = ' OR '
+        joined_func = or_
+    elif joined == 'and':
+        joined_text = ' AND '
+        joined_func = and_
+    else:
+        return query
+
+    text_items = []
+    binary_expression_items = []
+    for item in filters:
+        if type(item) is str:
+            text_items.append(item)
+        else:
+            binary_expression_items.append(item)
+
+    if len(text_items) > 0:
+        query = query.filter(text('(' + (joined_text.join(text_items)) + ')'))
+
+    if len(binary_expression_items) > 0:
+        query = query.filter(joined_func(*binary_expression_items))
+
+    return query
```

### Comparing `flaskz-1.6/src/flaskz/res_status_codes.py` & `flaskz-1.6.1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/rest/__init__.py` & `flaskz-1.6.1/src/flaskz/rest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from flask import request
-from flaskz import res_status_codes
 
+from .. import res_status_codes
 from ..log import flaskz_logger, get_log_data
-from ..models import model_to_dict, query_all_models, ModelMixin
-from ..utils import get_list, is_dict, create_response, get_pss, get_request_json
+from ..models import model_to_dict, query_all_models, ModelMixin, parse_pss
+from ..utils import get_list, is_dict, create_response, get_request_json
 
 
 def init_model_rest_blueprint(model_cls, api_blueprint, url_prefix, module, routers=None, to_json_option=None, multiple_option=None):
     """
     ** Deprecated, please use register_model_route **
 
     Append rest api route to the api blueprint for the specified model class.
@@ -335,15 +335,15 @@
     @app.route(pss_rule, methods=methods)
     @rest_permission_required(module, action)
     @gen_route_method('query_pss', rule)
     def query_pss():
         request_json = get_request_json({})  # @2023-06-15, request.json --> get_request_json({})
         req_log_data = json.dumps(request_json)
 
-        success, data = model.query_pss(get_pss(model, request_json))
+        success, data = model.query_pss(parse_pss(model, request_json))
         if success is True:
             data['data'] = model_to_dict(data.get('data', []), to_json_option)
 
         flaskz_logger.debug(get_rest_log_msg('Query pss {} data'.format(model.get_class_name()), req_log_data, success, data))
         return create_response(success, data)
```

### Comparing `flaskz-1.6/src/flaskz/rest/_mgmt.py` & `flaskz-1.6.1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/rest/_util.py` & `flaskz-1.6.1/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_app.py` & `flaskz-1.6.1/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_cache.py` & `flaskz-1.6.1/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_cls.py` & `flaskz-1.6.1/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_common.py` & `flaskz-1.6.1/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_func.py` & `flaskz-1.6.1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_magic.py` & `flaskz-1.6.1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_request_api.py` & `flaskz-1.6.1/src/flaskz/utils/_request_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     req_kwargs = {'url': url}
     _payload = payload or ['method', 'data', 'json', 'headers', 'cookies']
     for item in _payload:
         if item == 'json':  # @2022-05-06: fix request.json -->BadRequest('Content-Type was not 'application/json')
             req_kwargs[item] = request.get_json(force=True, silent=True)
         else:
             req_kwargs[item] = getattr(request, item, None)
+    req_kwargs['params'] = request.args  # @2022-06-25 add query string
     req_kwargs.update(kwargs)  # kwargs high priority
 
     url_params = req_kwargs.get('url_params')
     if url_params is None:  # if url_params is none, append request.view_args
         req_kwargs['url_params'] = request.view_args or {}
 
     req_kwargs['raw_response'] = True
```

### Comparing `flaskz-1.6/src/flaskz/utils/_request_args.py` & `flaskz-1.6.1/src/flaskz/models/_query_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,253 +1,256 @@
-from flask import request
-from sqlalchemy import desc, asc, Column
-from sqlalchemy.sql.elements import UnaryExpression
-
-from ._common import get_dict, is_str, is_dict, is_list
-
-__all__ = ['get_remote_addr', 'is_ajax', 'get_request_json', 'get_pss']
-
-
-def get_remote_addr():
-    """
-    Get the remote ip address.
-
-    :return:
-    """
-    if request:
-        return request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
-
-
-def is_ajax():
-    """
-    Check if the request is an ajax request.
-    :return:
-    """
-    if request:
-        return request.headers.get('X-Requested-With') == 'XMLHttpRequest'
-    return False
-
-
-def get_request_json(*args):
-    """
-    Get the JSON data(parsed) in request.
-    If json does not exist or parsing json error, return {}
-
-    .. versionadded:: 1.3
-
-    :return:
-    """
-    data = None
-    try:
-        data = request.get_json(force=True, silent=True)
-    except Exception:
-        pass
-    if data is None:
-        if len(args) > 0:
-            return args[0]
-    return data
-
-
-def get_pss(cls, pss_config=None):
-    """
-    Get the search, sort and paging information.
-    pss = page+search+sort
-
-    Example:
-        result, result = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
-            TemplateModel, {   # FROM templates
-                "search": {                         # WHERE
-                    "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
-                    "age": {                        # AND (age>1 AND age<20)
-                        ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
-                        "<": 20
-                    },
-                    "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
-                    "_ors": {                       # AND (country='America' OR country='Canada')
-                        "country": "America||Canada"
-                    },
-                    "_ands": {                      # AND (grade>1 AND grade<5)
-                        "grade": {
-                            ">": 1,
-                            "<": 5
-                        }
-                    }
-                },
-                "sort": {                           # ORDER BY templates.name ASC
-                    "field": "name",
-                    "order": "asc"
-                },
-                # "sort":[                            # multiple sort
-                #     {"field": "name", "order": "asc"},
-                #     {field": "age", "order": "desc"}
-                # ],
-                "page": {                           # LIMIT ? OFFSET ? (20, 0)
-                    "offset": 0,
-                    "size": 20
-                }
-            }))
-
-    :param cls: Model class
-    :param pss_config: page+search+sort
-    :return:
-    """
-    pss_config = get_dict(pss_config)
-    # --------------------search--------------------
-    search = pss_config.get('search') or {}
-    ands = []
-    ors = []
-
-    # select
-    search_like = search.pop('like', None)
-    like_columns = getattr(cls, 'like_columns', None)
-    likes = []
-    if search_like and like_columns is not None:
-        search_like = str(search_like).strip()
-        if search_like != '':
-            for col in like_columns:
-                if is_str(col):
-                    col_field = col
-                else:
-                    col_field = cls.get_column_field(col)
-                likes.append(col_field + " like '%" + search_like + "%'")
-
-    columns_fields = cls.get_columns_fields()
-    _ands = search.pop('_ands', None)
-    if _ands:
-        for key in _ands:
-            _append_item(ands, key, _ands[key], columns_fields)
-
-    _ors = search.pop('_ors', None)
-    if _ors:
-        for key in _ors:
-            _append_item(ors, key, _ors[key], columns_fields)
-
-    for key in search:
-        _append_item(ands, key, search[key], columns_fields)
-
-    # distinct = []  # @2023-06-07 add
-    # _distinct = search.pop('_distinct', None)
-    # if _distinct:
-    #     if is_str(_distinct):
-    #         _distinct = [_distinct]
-    #
-    #     if is_list(_distinct):
-    #         for distinct_item in _distinct:
-    #             distinct_column = cls.get_column_by_field(distinct_item)
-    #             if distinct_column is not None:
-    #                 distinct.append(distinct_column)
-
-    # --------------------group--------------------
-    groups = []  # @2023-06-07 add
-    _groups = pss_config.get('group', None)
-    if _groups:
-        if is_str(_groups):
-            _groups = [_groups]
-        if is_list(_groups):
-            for group_item in _groups:
-                group_column = cls.get_column_by_field(group_item)
-                if group_column is not None:
-                    groups.append(group_column)
-
-    # --------------------page--------------------
-    page = pss_config.get('page') or {}
-    offset = page.get('offset') or page.get('skip') or 0
-    limit = page.get('limit') or page.get('size') or 100000
-
-    # --------------------sort--------------------
-    # @2022-04-10 fix exception subs2 = relationship('PerfTestSubModel2', cascade='all,delete-orphan', lazy='joined') ->
-    # Can't resolve label reference for ORDER BY / GROUP BY / DISTINCT etc. Textual SQL expression 'f2' should be explicitly declared as text('f2')
-    sort = pss_config.get('sort')
-    sorts = []
-    if is_list(sort):
-        sorts = sort
-    elif is_dict(sort):
-        sorts = [sort]
-
-    orders = []
-    for sort_item in sorts:
-        if sort_item is None or sort_item == '':
-            continue
-
-        if is_str(sort_item):  # sort: "name"/["name"...]
-            sort_column = cls.get_column_by_field(sort_item)
-            if sort_column is not None:
-                orders.append(asc(sort_column))
-        elif type(sort_item) is Column:  # User.name
-            if sort_item in cls.get_columns():
-                orders.append(asc(sort_item))
-        elif type(sort_item) is UnaryExpression:  # desc(User.name)/asc(User.name)
-            orders.append(sort_item)
-        elif is_dict(sort_item):  # {"field": "name", "order": "desc"}
-            _order = sort_item.get('order')
-            if _order and not is_str(_order):  # {"order": desc(User.name))} == "sort":desc(User.name)
-                orders.append(_order)
-            else:
-                sort_field = sort_item.get('field')  # {"field": "name", "order": "asc"}
-                if sort_field:
-                    sort_column = cls.get_column_by_field(sort_field)
-                    if sort_column is not None:
-                        if _order and str(_order).strip().lower() in ['desc', 'descend', 'descending']:  # {"field": "name", "order": "desc"}
-                            orders.append(desc(sort_column))
-                        else:
-                            orders.append(asc(sort_column))  # {"field": "name"}.
-
-    # order = None
-    # _order = sort.get('order')
-    # if _order and not is_str(_order):  # desc(Model.column)
-    #     order = _order
-    # else:
-    #     sort_field = sort.get('field')
-    #     if sort_field:
-    #         sort_column = cls.get_column_by_field(sort_field)
-    #         if sort_column is not None:
-    #             if _order and str(_order).strip().lower() in ['desc', 'descend', 'descending']:
-    #                 order = desc(sort_column)
-    #
-    #             if order is None:
-    #                 order = asc(sort_column)  # default is asc.
-
-    return {
-        'filter_ands': ands,
-        'filter_ors': ors,
-        'filter_likes': likes,
-        'offset': offset,
-        'limit': limit,
-        'order': orders,
-        'group': groups
-        # 'distinct': distinct
-    }
-
-
-def _append_item(items, key, value, columns_fields):  # @2023-02-06 add columns_fields args to fix "Unknown column 'col' in 'where clause'"
-    """
-    Create sql text
-    - if need '' in sql, add in value ex) "'abc'"
-
-    :param items:
-    :param key:
-    :param value:
-    :param columns_fields:
-    :return:
-
-    :param items:
-    :param key:
-    :param value:
-    :param columns_fields:
-    :return:
-    """
-    if columns_fields and (key not in columns_fields):
-        return items
-
-    if value is not None:
-        if is_str(value):
-            value = value.strip()
-            if value != '':
-                val_arr = value.split('||')
-                for op_v in val_arr:
-                    items.append(key + " = '" + op_v + "'")
-        elif is_dict(value):
-            for operator, op_v in value.items():
-                items.append(key + ' ' + operator + ' ' + str(op_v))  # @2023-06-15 add blank, "in":"('a','b','c')"/ "like":"'%a'"
-        else:
-            items.append(key + ' = ' + str(value))
-    return items
+from sqlalchemy import desc, asc, Column
+from sqlalchemy.sql.elements import UnaryExpression
+
+__all__ = ['parse_pss']
+
+
+def parse_pss(cls, pss_config=None):
+    """
+    Get the search, sort and paging information.
+    flaskz.utils.get_pss == flaskz.models.parse_pss
+    pss = page+search+sort
+
+    .. versionadded:: 1.6.1 - rename flaskz.utils.get_pss function to flaskz.models.parse_pss, flaskz.utils.get_pss is still available
+    .. versionupdated:: 1.6.1 - change return list item(avoid SQL injection): SQL text --> Column.operator(parameter)  ex) "name like '%admin%'" --> TemplateModel.name.like('%admin%')
+
+    Example:
+        result, result = TemplateModel.query_pss(get_pss(   # use flaskz.utils.get_pss to format condition
+            TemplateModel, {   # FROM templates
+                "search": {                         # WHERE
+                    "like": "t",                    # name like '%t%' OR description like '%t%' (TemplateModel.like_columns = ['name', description])
+                    "age": {                        # AND (age>1 AND age<20)
+                        ">": 1,                     # operator:value, operators)'='/'>'/'<'/'>='/'<='/'BETWEEN'/'LIKE'/'IN'
+                        "<": 20
+                    },
+                    "email": "taozh@focus-ui.com",  # AND (email='taozh@focus-ui.com')
+                    "_ors": {                       # AND (country='America' OR country='Canada')
+                        "country": "America||Canada"
+                    },
+                    "_ands": {                      # AND (grade>1 AND grade<5)
+                        "grade": {
+                            ">": 1,
+                            "<": 5
+                        }
+                    }
+                },
+                "sort": {                           # ORDER BY templates.name ASC
+                    "field": "name",
+                    "order": "asc"
+                },
+                # "sort":[                            # multiple sort
+                #     {"field": "name", "order": "asc"},
+                #     {field": "age", "order": "desc"}
+                # ],
+                "page": {                           # LIMIT ? OFFSET ? (20, 0)
+                    "offset": 0,
+                    "size": 20
+                }
+            }))
+
+    :param cls: Model class
+    :param pss_config: page+search+sort
+    :return:
+    """
+    pss_config = get_dict(pss_config)
+    # --------------------search--------------------
+    search = pss_config.get('search') or {}
+
+    likes = _get_search_like_filters(cls, search.pop('like', None), search.pop('ilike', None))
+
+    ands = []
+    ors = []
+    _ands = search.pop('_ands', None)
+    if _ands:
+        for key in _ands:
+            _append_search_filters(ands, cls, key, _ands[key])
+
+    _ors = search.pop('_ors', None)
+    if _ors:
+        for key in _ors:
+            _append_search_filters(ors, cls, key, _ors[key])
+
+    for key in search:
+        _append_search_filters(ands, cls, key, search[key])
+
+    # distinct = []  # @2023-06-07 add
+    # _distinct = search.pop('_distinct', None)
+    # if _distinct:
+    #     if is_str(_distinct):
+    #         _distinct = [_distinct]
+    #
+    #     if is_list(_distinct):
+    #         for distinct_item in _distinct:
+    #             distinct_column = cls.get_column_by_field(distinct_item)
+    #             if distinct_column is not None:
+    #                 distinct.append(distinct_column)
+
+    # --------------------group--------------------
+    groups = _get_groups(cls, pss_config.get('group', None))  # @2023-06-07 add
+
+    # --------------------page--------------------
+    page = pss_config.get('page') or {}
+    offset = page.get('offset') or page.get('skip') or 0
+    limit = page.get('limit') or page.get('size') or 100000
+
+    # --------------------sort--------------------
+    # @2022-04-10 fix exception subs2 = relationship('PerfTestSubModel2', cascade='all,delete-orphan', lazy='joined') ->
+    # Can't resolve label reference for ORDER BY / GROUP BY / DISTINCT etc. Textual SQL expression 'f2' should be explicitly declared as text('f2')
+    orders = _get_sorts(cls, pss_config.get('sort', None))
+
+    return {
+        'filter_ands': _filter_pss_list(ands),
+        'filter_ors': _filter_pss_list(ors),
+        'filter_likes': _filter_pss_list(likes),
+
+        'order': _filter_pss_list(orders),
+        'group': _filter_pss_list(groups),
+
+        'offset': offset,
+        'limit': limit
+        # 'distinct': distinct
+    }
+
+
+def _filter_pss_list(items):
+    return [item for item in items if item is not None]
+
+
+def _get_groups(cls, group):
+    """
+    Get group by list
+    """
+    groups = []
+    if group:
+        if is_str(group):
+            group = [group]
+        if is_list(group):
+            for group_item in group:
+                group_column = cls.get_column_by_field(group_item)
+                if group_column is not None:
+                    groups.append(group_column)
+    return groups
+
+
+def _get_sorts(cls, sort):
+    """
+    Get sort list.
+    """
+    orders = []
+    sorts = []
+    if is_list(sort):
+        sorts = sort
+    elif is_dict(sort):
+        sorts = [sort]
+
+    for sort_item in sorts:
+        if sort_item is None or sort_item == '':
+            continue
+
+        if is_str(sort_item):  # sort: "name"/["name"...]
+            sort_column = cls.get_column_by_field(sort_item)
+            if sort_column is not None:
+                orders.append(asc(sort_column))
+        elif type(sort_item) is Column:  # User.name
+            if sort_item in cls.get_columns():
+                orders.append(asc(sort_item))
+        elif type(sort_item) is UnaryExpression:  # desc(User.name)/asc(User.name)
+            orders.append(sort_item)
+        elif is_dict(sort_item):  # {"field": "name", "order": "desc"}
+            _order = sort_item.get('order')
+            if _order and not is_str(_order):  # {"order": desc(User.name))} == "sort":desc(User.name)
+                orders.append(_order)
+            else:
+                sort_field = sort_item.get('field')  # {"field": "name", "order": "asc"}
+                if sort_field:
+                    sort_column = cls.get_column_by_field(sort_field)
+                    if sort_column is not None:
+                        if _order and str(_order).strip().lower() in ['desc', 'descend', 'descending']:  # {"field": "name", "order": "desc"}
+                            orders.append(desc(sort_column))
+                        else:
+                            orders.append(asc(sort_column))  # {"field": "name"}.
+    return orders
+
+
+def _get_search_like_filters(cls, search_like, search_ilike):
+    """
+    Get like list by like_columns.
+    """
+    like_filters = []
+
+    like_columns = []
+    for col in getattr(cls, 'like_columns', []):
+        if is_str(col):
+            col = cls.get_column_by_field(col)
+        if col is not None:
+            like_columns.append(col)
+    if len(like_columns) == 0:
+        return like_filters
+
+    if search_like is not None and search_like != '':
+        if not (search_like.startswith('%') or search_like.startswith('%')):
+            search_like = "%" + search_like + "%"
+        for col in like_columns:
+            like_filters.append(_get_col_op(col, 'like', search_like))
+
+    if search_ilike is not None and search_ilike != '':
+        if not (search_ilike.startswith('%') or search_ilike.startswith('%')):
+            search_ilike = "%" + search_ilike + "%"
+        for col in like_columns:
+            like_filters.append(_get_col_op(col, 'ilike', search_ilike))
+    return like_filters
+
+
+def _append_search_filters(items, cls, key, value):
+    """
+    Append filter item
+    """
+    col = cls.get_column_by_field(key)
+    if col is None:
+        return items
+
+    if value is not None:
+        if is_str(value):
+            value = value.strip()
+            if value != '':
+                val_arr = value.split('||')
+                for op_v in val_arr:
+                    items.append(_get_col_op(col, '==', op_v))
+        elif is_dict(value):
+            for operator, op_v in value.items():
+                items.append(_get_col_op(col, operator, op_v))
+        else:
+            items.append(_get_col_op(col, '==', value))
+    return items
+
+
+def _get_col_op(column, operator, value):
+    """
+        < , <= , == , != , > , >=
+        in , notin , between ,
+        is , isnot
+        like , ilike , notlike , notilike
+
+        ~startswith , endswith , contains~
+    """
+    operator = operator.lower()
+    op_func_mapping = {
+        'in': lambda col, val: col.in_(val) if type(val) is list else None,
+        'notin': lambda col, val: col.notin_(val) if type(val) is list else None,
+        'between': lambda col, val: col.between(*val) if type(val) is list else None,
+
+        'is': lambda col, val: col.is_(val),
+        'isnot': lambda col, val: col.is_not(val),
+
+        'like': lambda col, val: col.like(val),
+        'ilike': lambda col, val: col.ilike(val),
+        'notlike': lambda col, val: col.notlike(val),
+        'notilike': lambda col, val: col.notilike(val),
+
+        '==': lambda col, val: col.__eq__(val)
+    }
+    if operator in op_func_mapping:
+        return op_func_mapping.get(operator)(column, value)
+    return column.op(operator)(value)
+
+
+from ..utils import get_dict, is_str, is_dict, is_list
```

### Comparing `flaskz-1.6/src/flaskz/utils/_response.py` & `flaskz-1.6.1/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.6/src/flaskz/utils/_timer.py` & `flaskz-1.6.1/src/flaskz/utils/_timer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from datetime import datetime
 from threading import Timer
 
-__all__ = ['set_timeout', 'set_interval']
+__all__ = ['set_interval', 'set_timeout', 'run_at']
 
 
 class _IntervalTimer(object):
     def __init__(self, interval, function, args=None, kwargs=None, immediately=False, daemon=True):
         self._timer = None
         self.interval = interval  # milliseconds
         self.function = function
@@ -67,17 +68,60 @@
      .. versionadded:: 1.0
 
     Example:
         t = set_timeout(10, print, ('Hello, World!',))
         # t.cancel()    # Stop the timer
 
     :param interval: delay time in milliseconds before the specified function is executed
-    :param function:
-    :param args:
-    :param kwargs:
-    :param daemon: if true, the timer will be daemon(Daemon threads are abruptly stopped at shutdown)
+    :param function: the function to be executed
+    :param args: the args of the function
+    :param kwargs: the kwargs of the function
+    :param daemon: whether the timer is a daemon thread, default True(Daemon thread stops abruptly when main thread is shut down)
     :return:
     """
     t = Timer(interval / 1000, function, args=args, kwargs=kwargs)
     t.daemon = daemon
     t.start()
     return t
+
+
+def run_at(at_time, function, args=None, kwargs=None, daemon=True, time_format='%Y-%m-%d %H:%M:%S'):
+    """
+    Call a function at the specified datetime.
+
+    .. versionadded:: 1.6.1
+
+    Example:
+        t1 = run_at('2023-06-28 14:53:00', print, ['run_at'])   # time str
+        # t1.cancel()    # Stop the timer
+
+        t2 = run_at(1629811200, print, ['run_at'])  # timestamp
+        # t2.cancel()    # Stop the timer
+
+    :param at_time: the specified datetime(str/timestamp)
+    :param function: the function to be executed
+    :param args: the args of the function
+    :param kwargs: the kwargs of the function
+    :param daemon: whether the timer is a daemon thread, default True(Daemon thread stops abruptly when main thread is shut down)
+    :param time_format: the format of the specified datetime
+    :return:
+    """
+    time_type = type(at_time)
+    if time_type is str:
+        at_time = datetime.strptime(at_time, time_format)
+    elif time_type is int:
+        at_time = datetime.fromtimestamp(at_time)
+    now = datetime.now()
+    timeout_ms = (at_time - now).total_seconds()
+    if timeout_ms < 0:
+        return False
+    elif timeout_ms == 0:
+        function(*(args if args is not None else []), **(kwargs if kwargs is not None else {}))
+        return
+
+    return set_timeout(timeout_ms * 1000, function, args=args, kwargs=kwargs, daemon=daemon)
+
+
+if __name__ == '__main__':
+    set_timeout(1000, print, ['timeout'], daemon=False)
+    run_at('2023-06-28 15:51:00', print, ['timeout_at'], daemon=False)
+    # run_at(1629811200, print, ['timeout_at'], daemon=False)
```

### Comparing `flaskz-1.6/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.6.1/src/flaskz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.6
+Version: 1.6.1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,36 +24,39 @@
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
+- **1.6.1** `2023/07/01`
+    - [C] `flaskz.utils.get_pss`(`flaskz.models.parse_pss`)函数返回项由SQL字符串拼接改为参数化模式以预防SQL注入
+    - [A] 添加`flaskz.utils.run_at`函数用于执行定时函数
 - **1.6** `2023/06/16`
-    - [A] `BaseModelMixin`添加`count`方法，用于数量查询(全量/条件)
-    - [A] `BaseModelMixin`添加`clear_db`方法，用于清空数据
+    - [A] `BaseModelMixin`添加`count`方法, 用于数量查询(全量/条件)
+    - [A] `BaseModelMixin`添加`clear_db`方法, 用于清空数据
     - [A] `BaseModelMixin.query_pss`方法支持`GROUP BY`分组
     - [A] `flaskz.ext.ssh`添加对Paramiko>=3.0.0版本的支持
     - [A] `flaskz.ext.ssh`添加`secondary_password`和`recv_endswith`参数
 - **1.5.3** `2023/06/01`
-    - [F] `flaskz.util.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
-    - [A] `flaskz.util.api_request`函数添加`url_search_params`参数用于添加url查询字符串
+    - [F] `flaskz.utils.api_request`函数的`url_params`参数仅用于url中的`{变量}`替换而不添加查询字符串
+    - [A] `flaskz.utils.api_request`函数添加`url_search_params`参数用于添加url查询字符串
 - **1.5.2** `2023/05/17`
     - [C] `db_session`上下文管理器自动关闭非缓存session
     - [F] 修复`BaseModelMixin.get_query_default_order`默认排序在`query_pss`方法中不起作用的问题
 - **1.5** `2023/05/01`
     - [A] 扩展`flaskz.rest`路由生成模块*
-        - 添加`register_model_route`函数，可用于生成指定数据模型的CRUD等路由
-        - 添加`register_model_add_route`函数，可用于生成指定数据模型的添加路由
-        - 添加`register_model_delete_route`函数，可用于生成指定数据模型的删除路由
-        - 添加`register_model_update_route`函数，可用于生成指定数据模型的更新路由
-        - 添加`register_model_upsert_route`函数，可用于生成指定数据模型的添加/更新路由
-        - 添加`register_model_query_route`函数，可用于生成指定数据模型的全量查询路由
-        - 添加`register_model_query_pss_route`函数，可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
-        - 添加`register_models_query_route`函数，可用于生成多个数据模型的全量查询路由
+        - 添加`register_model_route`函数, 可用于生成指定数据模型的CRUD等路由
+        - 添加`register_model_add_route`函数, 可用于生成指定数据模型的添加路由
+        - 添加`register_model_delete_route`函数, 可用于生成指定数据模型的删除路由
+        - 添加`register_model_update_route`函数, 可用于生成指定数据模型的更新路由
+        - 添加`register_model_upsert_route`函数, 可用于生成指定数据模型的添加/更新路由
+        - 添加`register_model_query_route`函数, 可用于生成指定数据模型的全量查询路由
+        - 添加`register_model_query_pss_route`函数, 可用于生成指定数据模型的条件查询(分页+搜索+排序)路由
+        - 添加`register_models_query_route`函数, 可用于生成多个数据模型的全量查询路由
     - [A] `ModelMixin.query_pss`方法支持多列排序*
     - [A] `flaskz.models.init_model`和`flaskz.log.init_log`函数添加对`Class`类型参数的支持
     - [A] `BaseModelMixin.delete_db`方法添加对`dict`类型参数的支持
     - [A] `flaskz.utils`添加`cls_to_dict`函数, 用于生成类属性的dict对象
     - [C] `BaseModelMixin.bulk_delete`方法会删除符合条件的所有数据(此前版本只删除第一个)
 - **1.3.1** `2023/03/02`
     - [C] `init_model_rest_blueprint`函数生成的路由, 移除参数`path`类型转换, 以解决Flask<2.2.3版本不会将结尾不带`/`的请求重定向到带`/`路由的问题
```

### Comparing `flaskz-1.6/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.6.1/src/flaskz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/flaskz/ext/__init__.py
 src/flaskz/ext/cypher.py
 src/flaskz/ext/ssh.py
 src/flaskz/log/__init__.py
 src/flaskz/models/__init__.py
 src/flaskz/models/_base.py
 src/flaskz/models/_model.py
+src/flaskz/models/_query_util.py
 src/flaskz/models/_util.py
 src/flaskz/rest/__init__.py
 src/flaskz/rest/_mgmt.py
 src/flaskz/rest/_util.py
 src/flaskz/utils/__init__.py
 src/flaskz/utils/_app.py
 src/flaskz/utils/_cache.py
```

