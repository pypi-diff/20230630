# Comparing `tmp/nsj_rest_lib-1.2.0.tar.gz` & `tmp/nsj_rest_lib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.2.0.tar", last modified: Tue Jun 27 23:51:03 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.2.1.tar", last modified: Thu Jun 29 22:13:11 2023, max compression
```

## Comparing `nsj_rest_lib-1.2.0.tar` & `nsj_rest_lib-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.556127 nsj_rest_lib-1.2.0/
--rw-rw-rw-   0        0        0      760 2023-06-27 23:51:03.557130 nsj_rest_lib-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/README.md
--rw-rw-rw-   0        0        0      108 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      925 2023-06-27 23:51:03.560124 nsj_rest_lib-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.271011 nsj_rest_lib-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.363868 nsj_rest_lib-1.2.0/src/nsj_rest_lib/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.455851 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/__init__.py
--rw-rw-rw-   0        0        0       76 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-rw-   0        0        0     3211 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-rw-   0        0        0      972 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-rw-   0        0        0     3792 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/get_route.py
--rw-rw-rw-   0        0        0     4458 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/list_route.py
--rw-rw-rw-   0        0        0     4204 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-rw-   0        0        0     3774 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/post_route.py
--rw-rw-rw-   0        0        0     4194 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/put_route.py
--rw-rw-rw-   0        0        0     4798 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/route_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.463847 nsj_rest_lib-1.2.0/src/nsj_rest_lib/dao/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/dao/__init__.py
--rw-rw-rw-   0        0        0    18311 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-rw-   0        0        0     1256 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/db_pool_config.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.474123 nsj_rest_lib-1.2.0/src/nsj_rest_lib/decorator/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/decorator/dto.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.503170 nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-rw-   0        0        0    10096 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-rw-   0        0        0     7842 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-rw-   0        0        0     5536 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-rw-   0        0        0      304 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-rw-   0        0        0     2388 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.511126 nsj_rest_lib-1.2.0/src/nsj_rest_lib/dto/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/dto/__init__.py
--rw-rw-rw-   0        0        0     7491 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.526138 nsj_rest_lib-1.2.0/src/nsj_rest_lib/entity/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/entity/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-rw-   0        0        0      338 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/entity/filter.py
--rw-rw-rw-   0        0        0      509 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/exception.py
--rw-rw-rw-   0        0        0     2939 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-rw-   0        0        0      858 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.535127 nsj_rest_lib-1.2.0/src/nsj_rest_lib/service/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/service/__init__.py
--rw-rw-rw-   0        0        0    24251 2023-06-27 23:49:07.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/service/service_base.py
--rw-rw-rw-   0        0        0      598 2023-03-08 22:01:56.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.551127 nsj_rest_lib-1.2.0/src/nsj_rest_lib/validator/
--rw-rw-rw-   0        0        0        0 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/validator/__init__.py
--rw-rw-rw-   0        0        0     4376 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-rw-   0        0        0      551 2023-02-07 17:52:43.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxrwx   0        0        0        0 2023-06-27 23:51:03.393847 nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/
--rw-rw-rw-   0        0        0      760 2023-06-27 23:51:03.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1652 2023-06-27 23:51:03.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 23:51:03.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-06-27 23:51:03.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-27 23:51:03.000000 nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-29 22:13:11.488819 nsj_rest_lib-1.2.1/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.476819 nsj_rest_lib-1.2.1/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.476819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-06-29 22:11:32.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-06-29 22:11:52.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4483 2023-06-29 22:09:09.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-06-29 22:09:50.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-06-29 22:10:22.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-06-29 22:10:52.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    17770 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      293 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23612 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-06-29 21:53:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1652 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.2.0/PKG-INFO` & `nsj_rest_lib-1.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: nsj_rest_lib
-Version: 1.2.0
-Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
-Home-page: https://github.com/Nasajon/nsj_rest_lib
-Author: Nasajon Sistemas
-Author-email: contact.dev@nasajon.com.br
-Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-
-# nsj_rest_lib
-Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
+Metadata-Version: 2.1
+Name: nsj_rest_lib
+Version: 1.2.1
+Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
+Home-page: https://github.com/Nasajon/nsj_rest_lib
+Author: Nasajon Sistemas
+Author-email: contact.dev@nasajon.com.br
+Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+
+# nsj_rest_lib
+Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
```

### Comparing `nsj_rest_lib-1.2.0/setup.cfg` & `nsj_rest_lib-1.2.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206e 736a 5f72 6573 745f 6c69 620d   = nsj_rest_lib.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e32 2e30  .version = 1.2.0
-00000030: 0d0a 6175 7468 6f72 203d 204e 6173 616a  ..author = Nasaj
-00000040: 6f6e 2053 6973 7465 6d61 730d 0a61 7574  on Sistemas..aut
-00000050: 686f 725f 656d 6169 6c20 3d20 636f 6e74  hor_email = cont
-00000060: 6163 742e 6465 7640 6e61 7361 6a6f 6e2e  act.dev@nasajon.
-00000070: 636f 6d2e 6272 0d0a 6465 7363 7269 7074  com.br..descript
-00000080: 696f 6e20 3d20 4269 626c 696f 7465 6361  ion = Biblioteca
-00000090: 2070 6172 6120 636f 6e73 7472 75c3 a7c3   para constru...
-000000a0: a36f 2064 6520 4150 4973 2052 6573 7420  .o de APIs Rest 
-000000b0: 5079 7468 6f6e 2c20 6465 2061 636f 7264  Python, de acord
-000000c0: 6f20 636f 6d20 6f20 6775 6964 656c 696e  o com o guidelin
-000000d0: 6573 2069 6e74 6572 6e6f 2c20 6520 636f  es interno, e co
-000000e0: 6d20 7061 7261 6469 676d 6120 6465 636c  m paradigma decl
-000000f0: 6172 6174 6976 6f2e 0d0a 6c6f 6e67 5f64  arativo...long_d
-00000100: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000110: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-00000120: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-00000130: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000140: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000150: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000160: 622e 636f 6d2f 4e61 7361 6a6f 6e2f 6e73  b.com/Nasajon/ns
-00000170: 6a5f 7265 7374 5f6c 6962 0d0a 7072 6f6a  j_rest_lib..proj
-00000180: 6563 745f 7572 6c73 203d 200d 0a09 536f  ect_urls = ...So
-00000190: 7572 6365 203d 2068 7474 7073 3a2f 2f67  urce = https://g
-000001a0: 6974 6875 622e 636f 6d2f 4e61 7361 6a6f  ithub.com/Nasajo
-000001b0: 6e2f 6e73 6a5f 7265 7374 5f6c 6962 0d0a  n/nsj_rest_lib..
-000001c0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001d0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-000001e0: 7475 7320 3a3a 2033 202d 2041 6c70 6861  tus :: 3 - Alpha
-000001f0: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-00000200: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000210: 7273 0d0a 0954 6f70 6963 203a 3a20 536f  rs...Topic :: So
-00000220: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000230: 6e74 203a 3a20 4c69 6272 6172 6965 730d  nt :: Libraries.
-00000240: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000250: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000260: 203a 3a20 330d 0a0d 0a5b 6f70 7469 6f6e   :: 3....[option
-00000270: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000280: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000290: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-000002a0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000002b0: 3e3d 332e 340d 0a69 6e73 7461 6c6c 5f72  >=3.4..install_r
-000002c0: 6571 7569 7265 7320 3d20 0d0a 0946 6c61  equires = ...Fla
-000002d0: 736b 3e3d 322e 302e 332c 3c33 2e30 2e30  sk>=2.0.3,<3.0.0
-000002e0: 0d0a 0953 514c 416c 6368 656d 793d 3d31  ...SQLAlchemy==1
-000002f0: 2e34 2e33 320d 0a09 7067 3830 3030 3d3d  .4.32...pg8000==
-00000300: 312e 3234 2e31 0d0a 096e 736a 5f67 6366  1.24.1...nsj_gcf
-00000310: 5f75 7469 6c73 7e3d 312e 302e 310d 0a09  _utils~=1.0.1...
-00000320: 5079 4d79 5351 4c3d 3d31 2e30 2e32 0d0a  PyMySQL==1.0.2..
-00000330: 0970 792d 6865 616c 7468 6368 6563 6b3d  .py-healthcheck=
-00000340: 3d31 2e31 302e 310d 0a0d 0a5b 6f70 7469  =1.10.1....[opti
-00000350: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000360: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000370: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000380: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000390: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6e73 6a5f 7265 7374 5f6c 6962 0a76  = nsj_rest_lib.v
+00000020: 6572 7369 6f6e 203d 2031 2e32 2e31 0a61  ersion = 1.2.1.a
+00000030: 7574 686f 7220 3d20 4e61 7361 6a6f 6e20  uthor = Nasajon 
+00000040: 5369 7374 656d 6173 0a61 7574 686f 725f  Sistemas.author_
+00000050: 656d 6169 6c20 3d20 636f 6e74 6163 742e  email = contact.
+00000060: 6465 7640 6e61 7361 6a6f 6e2e 636f 6d2e  dev@nasajon.com.
+00000070: 6272 0a64 6573 6372 6970 7469 6f6e 203d  br.description =
+00000080: 2042 6962 6c69 6f74 6563 6120 7061 7261   Biblioteca para
+00000090: 2063 6f6e 7374 7275 c3a7 c3a3 6f20 6465   constru....o de
+000000a0: 2041 5049 7320 5265 7374 2050 7974 686f   APIs Rest Pytho
+000000b0: 6e2c 2064 6520 6163 6f72 646f 2063 6f6d  n, de acordo com
+000000c0: 206f 2067 7569 6465 6c69 6e65 7320 696e   o guidelines in
+000000d0: 7465 726e 6f2c 2065 2063 6f6d 2070 6172  terno, e com par
+000000e0: 6164 6967 6d61 2064 6563 6c61 7261 7469  adigma declarati
+000000f0: 766f 2e0a 6c6f 6e67 5f64 6573 6372 6970  vo..long_descrip
+00000100: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+00000110: 444d 452e 6d64 0a6c 6f6e 675f 6465 7363  DME.md.long_desc
+00000120: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000130: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000140: 646f 776e 0a75 726c 203d 2068 7474 7073  down.url = https
+00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e61  ://github.com/Na
+00000160: 7361 6a6f 6e2f 6e73 6a5f 7265 7374 5f6c  sajon/nsj_rest_l
+00000170: 6962 0a70 726f 6a65 6374 5f75 726c 7320  ib.project_urls 
+00000180: 3d20 0a09 536f 7572 6365 203d 2068 7474  = ..Source = htt
+00000190: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001a0: 4e61 7361 6a6f 6e2f 6e73 6a5f 7265 7374  Nasajon/nsj_rest
+000001b0: 5f6c 6962 0a63 6c61 7373 6966 6965 7273  _lib.classifiers
+000001c0: 203d 200a 0944 6576 656c 6f70 6d65 6e74   = ..Development
+000001d0: 2053 7461 7475 7320 3a3a 2033 202d 2041   Status :: 3 - A
+000001e0: 6c70 6861 0a09 496e 7465 6e64 6564 2041  lpha..Intended A
+000001f0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+00000200: 6f70 6572 730a 0954 6f70 6963 203a 3a20  opers..Topic :: 
+00000210: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
+00000220: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
+00000230: 730a 0950 726f 6772 616d 6d69 6e67 204c  s..Programming L
+00000240: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000250: 6e20 3a3a 2033 0a0a 5b6f 7074 696f 6e73  n :: 3..[options
+00000260: 5d0a 7061 636b 6167 655f 6469 7220 3d20  ].package_dir = 
+00000270: 0a09 3d20 7372 630a 7061 636b 6167 6573  ..= src.packages
+00000280: 203d 2066 696e 643a 0a70 7974 686f 6e5f   = find:.python_
+00000290: 7265 7175 6972 6573 203d 203e 3d33 2e34  requires = >=3.4
+000002a0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000002b0: 7320 3d20 0a09 466c 6173 6b3e 3d32 2e30  s = ..Flask>=2.0
+000002c0: 2e33 2c3c 332e 302e 300a 0953 514c 416c  .3,<3.0.0..SQLAl
+000002d0: 6368 656d 793d 3d31 2e34 2e33 320a 0970  chemy==1.4.32..p
+000002e0: 6738 3030 303d 3d31 2e32 342e 310a 096e  g8000==1.24.1..n
+000002f0: 736a 5f67 6366 5f75 7469 6c73 7e3d 312e  sj_gcf_utils~=1.
+00000300: 302e 310a 0950 794d 7953 514c 3d3d 312e  0.1..PyMySQL==1.
+00000310: 302e 320a 0970 792d 6865 616c 7468 6368  0.2..py-healthch
+00000320: 6563 6b3d 3d31 2e31 302e 310a 0a5b 6f70  eck==1.10.1..[op
+00000330: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000340: 696e 645d 0a77 6865 7265 203d 2073 7263  ind].where = src
+00000350: 0a0a 5b65 6767 5f69 6e66 6f5d 0a74 6167  ..[egg_info].tag
+00000360: 5f62 7569 6c64 203d 200a 7461 675f 6461  _build = .tag_da
+00000370: 7465 203d 2030 0a0a                      te = 0..
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any, Callable
-from flask import request
-
-
-class FunctionRouteWrapper:
-    route_ref_count = {}
-    func: Callable
-
-    def __init__(self, route_obj, func: Callable):
-        super().__init__()
-
-        self.func = func
-
-        # Assumindo o nome da rota como o nome da classe
-        route_name = route_obj.__class__.__name__
-
-        # Resolvendo o contador de referências dessa mesma rota
-        ref_count = FunctionRouteWrapper.route_ref_count.get(route_name, 0) + 1
-        FunctionRouteWrapper.route_ref_count[route_name] = ref_count
-
-        # Guardando as propriedades
-        self._route_obj = route_obj
-        self.__name__ = f"{route_name}_{ref_count}"
-
-    def __call__(self, *args: Any, **kwargs: Any):
-        # Retorna o resultado da chamada ao método handle_request do objeto de rota associado
-        response = self._route_obj.handle_request(*args, **kwargs)
-        return self.func(request, response)
+from typing import Any, Callable
+from flask import request
+
+
+class FunctionRouteWrapper:
+    route_ref_count = {}
+    func: Callable
+
+    def __init__(self, route_obj, func: Callable):
+        super().__init__()
+
+        self.func = func
+
+        # Assumindo o nome da rota como o nome da classe
+        route_name = route_obj.__class__.__name__
+
+        # Resolvendo o contador de referências dessa mesma rota
+        ref_count = FunctionRouteWrapper.route_ref_count.get(route_name, 0) + 1
+        FunctionRouteWrapper.route_ref_count[route_name] = ref_count
+
+        # Guardando as propriedades
+        self._route_obj = route_obj
+        self.__name__ = f"{route_name}_{ref_count}"
+
+    def __call__(self, *args: Any, **kwargs: Any):
+        # Retorna o resultado da chamada ao método handle_request do objeto de rota associado
+        response = self._route_obj.handle_request(*args, **kwargs)
+        return self.func(request, response)
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/post_route.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,96 @@
-from flask import request
-from typing import Callable
-
-from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
-from nsj_rest_lib.controller.route_base import RouteBase
-from nsj_rest_lib.dto.dto_base import DTOBase
-from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, NotFoundException
-from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
-
-from nsj_gcf_utils.json_util import json_dumps
-from nsj_gcf_utils.pagination_util import PaginationException
-from nsj_gcf_utils.rest_error_util import format_json_error
-
-
-class GetRoute(RouteBase):
-    def __init__(
-        self,
-        url: str,
-        http_method: str,
-        dto_class: DTOBase,
-        entity_class: EntityBase,
-        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
-        service_name: str = None,
-        handle_exception: Callable = None,
-    ):
-        super().__init__(
-            url=url,
-            http_method=http_method,
-            dto_class=dto_class,
-            entity_class=entity_class,
-            dto_response_class=None,
-            injector_factory=injector_factory,
-            service_name=service_name,
-            handle_exception=handle_exception
-        )
-
-    def handle_request(self, id):
-        """
-        Tratando requisições HTTP Get para recuperar uma instância de uma entidade.
-        """
-
-        with self._injector_factory() as factory:
-            try:
-                # Recuperando os parâmetros básicos
-                args = request.args
-
-                # Tratando dos fields
-                fields = args.get('fields')
-                fields = self._parse_fields(fields)
-
-                partition_fields = {}
-                # Tratando campos de particionamento
-                for field in self._dto_class.partition_fields:
-                    value = args.get(field)
-                    if value is None:
-                        raise MissingParameterException(field)
-                    
-                    partition_fields[field] = value
-
-                # Construindo os objetos
-                service = self._get_service(factory)
-
-                # Chamando o service (método get)
-                # TODO Rever parametro order_fields abaixo
-                data = service.get(id, partition_fields, fields)
-
-                # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
-                dict_data = data.convert_to_dict(fields)
-
-                # Retornando a resposta da requuisição
-                return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
-            except MissingParameterException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except PaginationException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except NotFoundException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
-            except Exception as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
+from flask import request
+from typing import Callable
+
+from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
+from nsj_rest_lib.controller.route_base import RouteBase
+from nsj_rest_lib.dto.dto_base import DTOBase
+from nsj_rest_lib.entity.entity_base import EntityBase
+from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, ConflictException
+from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+from nsj_rest_lib.settings import get_logger
+
+from nsj_gcf_utils.json_util import json_dumps, json_loads, JsonLoadException
+from nsj_gcf_utils.rest_error_util import format_json_error
+
+
+class PostRoute(RouteBase):
+    def __init__(
+        self,
+        url: str,
+        http_method: str,
+        dto_class: DTOBase,
+        entity_class: EntityBase,
+        dto_response_class: DTOBase = None,
+        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
+        service_name: str = None,
+        handle_exception: Callable = None,
+    ):
+        super().__init__(
+            url=url,
+            http_method=http_method,
+            dto_class=dto_class,
+            entity_class=entity_class,
+            dto_response_class=dto_response_class,
+            injector_factory=injector_factory,
+            service_name=service_name,
+            handle_exception=handle_exception,
+        )
+
+    def handle_request(self):
+        """
+        Tratando requisições HTTP Post para inserir uma instância de uma entidade.
+        """
+
+        with self._injector_factory() as factory:
+            try:
+                # Recuperando os dados do corpo da rquisição
+                data = request.json
+
+                # Convertendo os dados para o DTO
+                data = self._dto_class(**data)
+
+                # Construindo os objetos
+                service = self._get_service(factory)
+
+                # Chamando o service (método insert)
+                data = service.insert(data)
+
+                if data is not None:
+                    # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
+                    dict_data = data.convert_to_dict()
+
+                    # Retornando a resposta da requuisição
+                    return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
+                else:
+                    # Retornando a resposta da requuisição
+                    return ('', 201, {**DEFAULT_RESP_HEADERS})
+            except JsonLoadException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except MissingParameterException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except ValueError as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except ConflictException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 409, {**DEFAULT_RESP_HEADERS})
+            except Exception as e:
+                get_logger().exception(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/list_route.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,112 @@
-from flask import request
-from typing import Callable
-
-from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
-from nsj_rest_lib.controller.route_base import RouteBase
-from nsj_rest_lib.dto.dto_base import DTOBase
-from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.exception import DTOConfigException, MissingParameterException
-from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
-from nsj_rest_lib.settings import DEFAULT_PAGE_SIZE
-
-from nsj_gcf_utils.json_util import json_dumps
-from nsj_gcf_utils.pagination_util import page_body, PaginationException
-from nsj_gcf_utils.rest_error_util import format_json_error
-
-
-class ListRoute(RouteBase):
-    def __init__(
-        self,
-        url: str,
-        http_method: str,
-        dto_class: DTOBase,
-        entity_class: EntityBase,
-        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
-        service_name: str = None,
-        handle_exception: Callable = None,
-    ):
-        super().__init__(
-            url=url,
-            http_method=http_method,
-            dto_class=dto_class,
-            entity_class=entity_class,
-            dto_response_class=None,
-            injector_factory=injector_factory,
-            service_name=service_name,
-            handle_exception=handle_exception,
-        )
-
-    def handle_request(self):
-        """
-        Tratando requisições HTTP Get (para listar entidades, e não para recuperar pelo ID).
-        """
-
-        with self._injector_factory() as factory:
-            try:
-                # Recuperando os parâmetros básicos
-                base_url = request.base_url
-                args = request.args
-                limit = int(args.get('limit', DEFAULT_PAGE_SIZE))
-                current_after = args.get('after') or args.get('offset')
-
-                # Tratando dos fields
-                fields = args.get('fields')
-                fields = self._parse_fields(fields)
-
-                # Tratando dos filters
-                filters = {}
-                for arg in args:
-                    if arg in ['limit', 'after', 'offset', 'fields', 'tenant', 'grupo_empresarial']:
-                        continue
-
-                    filters[arg] = args.get(arg)
-
-                # Tratando campos de particionamento
-                for field in self._dto_class.partition_fields:
-                    value = args.get(field)
-                    if value is None:
-                        raise MissingParameterException(field)
-                    
-                    filters[field] = value
-
-                # Construindo os objetos
-                service = self._get_service(factory)
-
-                # Chamando o service (método list)
-                # TODO Rever parametro order_fields abaixo
-                data = service.list(current_after, limit,
-                                    fields, None, filters)
-
-                # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
-                dict_data = [dto.convert_to_dict(fields) for dto in data]
-
-                # Construindo o corpo da página
-                page = page_body(
-                    base_url=base_url,
-                    limit=limit,
-                    current_after=current_after,
-                    current_before=None,
-                    result=dict_data,
-                    id_field='id'  # TODO Rever esse parâmetro
-                )
-
-                # Retornando a resposta da requuisição
-                return (json_dumps(page), 200, {**DEFAULT_RESP_HEADERS})
-            except MissingParameterException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except PaginationException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except Exception as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
+from flask import request
+from typing import Callable
+
+from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
+from nsj_rest_lib.controller.route_base import RouteBase
+from nsj_rest_lib.dto.dto_base import DTOBase
+from nsj_rest_lib.entity.entity_base import EntityBase
+from nsj_rest_lib.exception import DTOConfigException, MissingParameterException
+from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+from nsj_rest_lib.settings import get_logger, DEFAULT_PAGE_SIZE
+
+from nsj_gcf_utils.json_util import json_dumps
+from nsj_gcf_utils.pagination_util import page_body, PaginationException
+from nsj_gcf_utils.rest_error_util import format_json_error
+
+
+class ListRoute(RouteBase):
+    def __init__(
+        self,
+        url: str,
+        http_method: str,
+        dto_class: DTOBase,
+        entity_class: EntityBase,
+        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
+        service_name: str = None,
+        handle_exception: Callable = None,
+    ):
+        super().__init__(
+            url=url,
+            http_method=http_method,
+            dto_class=dto_class,
+            entity_class=entity_class,
+            dto_response_class=None,
+            injector_factory=injector_factory,
+            service_name=service_name,
+            handle_exception=handle_exception,
+        )
+
+    def handle_request(self):
+        """
+        Tratando requisições HTTP Get (para listar entidades, e não para recuperar pelo ID).
+        """
+
+        with self._injector_factory() as factory:
+            try:
+                # Recuperando os parâmetros básicos
+                base_url = request.base_url
+                args = request.args
+                limit = int(args.get('limit', DEFAULT_PAGE_SIZE))
+                current_after = args.get('after') or args.get('offset')
+
+                # Tratando dos fields
+                fields = args.get('fields')
+                fields = self._parse_fields(fields)
+
+                # Tratando dos filters
+                filters = {}
+                for arg in args:
+                    if arg in ['limit', 'after', 'offset', 'fields', 'tenant', 'grupo_empresarial']:
+                        continue
+
+                    filters[arg] = args.get(arg)
+
+                # Tratando campos de particionamento
+                for field in self._dto_class.partition_fields:
+                    value = args.get(field)
+                    if value is None:
+                        raise MissingParameterException(field)
+                    
+                    filters[field] = value
+
+                # Construindo os objetos
+                service = self._get_service(factory)
+
+                # Chamando o service (método list)
+                # TODO Rever parametro order_fields abaixo
+                data = service.list(current_after, limit,
+                                    fields, None, filters)
+
+                # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
+                dict_data = [dto.convert_to_dict(fields) for dto in data]
+
+                # Construindo o corpo da página
+                page = page_body(
+                    base_url=base_url,
+                    limit=limit,
+                    current_after=current_after,
+                    current_before=None,
+                    result=dict_data,
+                    id_field='id'  # TODO Rever esse parâmetro
+                )
+
+                # Retornando a resposta da requuisição
+                return (json_dumps(page), 200, {**DEFAULT_RESP_HEADERS})
+            except MissingParameterException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except PaginationException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except Exception as e:
+                get_logger().exception(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/patch_route.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,106 @@
-from flask import request
-from typing import Callable
-
-from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
-from nsj_rest_lib.controller.route_base import RouteBase
-from nsj_rest_lib.dto.dto_base import DTOBase
-from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, NotFoundException
-from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
-
-from nsj_gcf_utils.json_util import json_dumps, json_loads, JsonLoadException
-from nsj_gcf_utils.rest_error_util import format_json_error
-
-
-class PatchRoute(RouteBase):
-    def __init__(
-        self,
-        url: str,
-        http_method: str,
-        dto_class: DTOBase,
-        entity_class: EntityBase,
-        dto_response_class: DTOBase = None,
-        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
-        service_name: str = None,
-        handle_exception: Callable = None,
-    ):
-        super().__init__(
-            url=url,
-            http_method=http_method,
-            dto_class=dto_class,
-            entity_class=entity_class,
-            dto_response_class=dto_response_class,
-            injector_factory=injector_factory,
-            service_name=service_name,
-            handle_exception=handle_exception,
-        )
-
-    def handle_request(self, id):
-        """
-        Tratando requisições HTTP Put para inserir uma instância de uma entidade.
-        """
-
-        with self._injector_factory() as factory:
-            try:
-                # Recuperando os dados do corpo da rquisição
-                data = request.json
-
-                # Convertendo os dados para o DTO
-                data = self._dto_class(**data)
-
-                # Montando os filtros de particao de dados
-                partition_filters = {}
-                
-                for field in data.partition_fields:
-                    value = getattr(data, field)
-                    if value is None:
-                        raise MissingParameterException(field)
-                    elif value is not None:
-                        partition_filters[field] = value
-
-                # Construindo os objetos
-                service = self._get_service(factory)
-
-                # Chamando o service (método insert)
-                data = service.partial_update(data, id, partition_filters)
-
-                if data is not None:
-                    # Convertendo para o formato de dicionário
-                    dict_data = data.convert_to_dict()
-
-                    # Retornando a resposta da requuisição
-                    return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
-                else:
-                    # Retornando a resposta da requuisição
-                    return ('', 204, {**DEFAULT_RESP_HEADERS})
-            except JsonLoadException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except MissingParameterException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except ValueError as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except NotFoundException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
-            except Exception as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
+from flask import request
+from typing import Callable
+
+from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
+from nsj_rest_lib.controller.route_base import RouteBase
+from nsj_rest_lib.dto.dto_base import DTOBase
+from nsj_rest_lib.entity.entity_base import EntityBase
+from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, NotFoundException
+from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+from nsj_rest_lib.settings import get_logger
+
+from nsj_gcf_utils.json_util import json_dumps, json_loads, JsonLoadException
+from nsj_gcf_utils.rest_error_util import format_json_error
+
+
+class PatchRoute(RouteBase):
+    def __init__(
+        self,
+        url: str,
+        http_method: str,
+        dto_class: DTOBase,
+        entity_class: EntityBase,
+        dto_response_class: DTOBase = None,
+        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
+        service_name: str = None,
+        handle_exception: Callable = None,
+    ):
+        super().__init__(
+            url=url,
+            http_method=http_method,
+            dto_class=dto_class,
+            entity_class=entity_class,
+            dto_response_class=dto_response_class,
+            injector_factory=injector_factory,
+            service_name=service_name,
+            handle_exception=handle_exception,
+        )
+
+    def handle_request(self, id):
+        """
+        Tratando requisições HTTP Put para inserir uma instância de uma entidade.
+        """
+
+        with self._injector_factory() as factory:
+            try:
+                # Recuperando os dados do corpo da rquisição
+                data = request.json
+
+                # Convertendo os dados para o DTO
+                data = self._dto_class(**data)
+
+                # Montando os filtros de particao de dados
+                partition_filters = {}
+                
+                for field in data.partition_fields:
+                    value = getattr(data, field)
+                    if value is None:
+                        raise MissingParameterException(field)
+                    elif value is not None:
+                        partition_filters[field] = value
+
+                # Construindo os objetos
+                service = self._get_service(factory)
+
+                # Chamando o service (método insert)
+                data = service.partial_update(data, id, partition_filters)
+
+                if data is not None:
+                    # Convertendo para o formato de dicionário
+                    dict_data = data.convert_to_dict()
+
+                    # Retornando a resposta da requuisição
+                    return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
+                else:
+                    # Retornando a resposta da requuisição
+                    return ('', 204, {**DEFAULT_RESP_HEADERS})
+            except JsonLoadException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except MissingParameterException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except ValueError as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except NotFoundException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
+            except Exception as e:
+                get_logger().exception(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/put_route.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,106 @@
-from flask import request
-from typing import Callable
-
-from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
-from nsj_rest_lib.controller.route_base import RouteBase
-from nsj_rest_lib.dto.dto_base import DTOBase
-from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, NotFoundException
-from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
-
-from nsj_gcf_utils.json_util import json_dumps, json_loads, JsonLoadException
-from nsj_gcf_utils.rest_error_util import format_json_error
-
-
-class PutRoute(RouteBase):
-    def __init__(
-        self,
-        url: str,
-        http_method: str,
-        dto_class: DTOBase,
-        entity_class: EntityBase,
-        dto_response_class: DTOBase = None,
-        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
-        service_name: str = None,
-        handle_exception: Callable = None,
-    ):
-        super().__init__(
-            url=url,
-            http_method=http_method,
-            dto_class=dto_class,
-            entity_class=entity_class,
-            dto_response_class=dto_response_class,
-            injector_factory=injector_factory,
-            service_name=service_name,
-            handle_exception=handle_exception,
-        )
-
-    def handle_request(self, id):
-        """
-        Tratando requisições HTTP Put para inserir uma instância de uma entidade.
-        """
-
-        with self._injector_factory() as factory:
-            try:
-                # Recuperando os dados do corpo da rquisição
-                data = request.json
-
-                # Convertendo os dados para o DTO
-                data = self._dto_class(**data)
-
-                # Montando os filtros de particao de dados
-                partition_filters = {}
-                
-                for field in data.partition_fields:
-                    value = getattr(data, field)
-                    if value is None:
-                        raise MissingParameterException(field)
-                    elif value is not None:
-                        partition_filters[field] = value
-
-                # Construindo os objetos
-                service = self._get_service(factory)
-
-                # Chamando o service (método insert)
-                data = service.update(data, id, partition_filters)
-
-                if data is not None:
-                    # Convertendo para o formato de dicionário
-                    dict_data = data.convert_to_dict()
-
-                    # Retornando a resposta da requuisição
-                    return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
-                else:
-                    # Retornando a resposta da requuisição
-                    return ('', 204, {**DEFAULT_RESP_HEADERS})
-            except JsonLoadException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except MissingParameterException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except ValueError as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except NotFoundException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
-            except Exception as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
+from flask import request
+from typing import Callable
+
+from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
+from nsj_rest_lib.controller.route_base import RouteBase
+from nsj_rest_lib.dto.dto_base import DTOBase
+from nsj_rest_lib.entity.entity_base import EntityBase
+from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, NotFoundException
+from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+from nsj_rest_lib.settings import get_logger
+
+from nsj_gcf_utils.json_util import json_dumps, json_loads, JsonLoadException
+from nsj_gcf_utils.rest_error_util import format_json_error
+
+
+class PutRoute(RouteBase):
+    def __init__(
+        self,
+        url: str,
+        http_method: str,
+        dto_class: DTOBase,
+        entity_class: EntityBase,
+        dto_response_class: DTOBase = None,
+        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
+        service_name: str = None,
+        handle_exception: Callable = None,
+    ):
+        super().__init__(
+            url=url,
+            http_method=http_method,
+            dto_class=dto_class,
+            entity_class=entity_class,
+            dto_response_class=dto_response_class,
+            injector_factory=injector_factory,
+            service_name=service_name,
+            handle_exception=handle_exception,
+        )
+
+    def handle_request(self, id):
+        """
+        Tratando requisições HTTP Put para inserir uma instância de uma entidade.
+        """
+
+        with self._injector_factory() as factory:
+            try:
+                # Recuperando os dados do corpo da rquisição
+                data = request.json
+
+                # Convertendo os dados para o DTO
+                data = self._dto_class(**data)
+
+                # Montando os filtros de particao de dados
+                partition_filters = {}
+                
+                for field in data.partition_fields:
+                    value = getattr(data, field)
+                    if value is None:
+                        raise MissingParameterException(field)
+                    elif value is not None:
+                        partition_filters[field] = value
+
+                # Construindo os objetos
+                service = self._get_service(factory)
+
+                # Chamando o service (método insert)
+                data = service.update(data, id, partition_filters)
+
+                if data is not None:
+                    # Convertendo para o formato de dicionário
+                    dict_data = data.convert_to_dict()
+
+                    # Retornando a resposta da requuisição
+                    return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
+                else:
+                    # Retornando a resposta da requuisição
+                    return ('', 204, {**DEFAULT_RESP_HEADERS})
+            except JsonLoadException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except MissingParameterException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except ValueError as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except NotFoundException as e:
+                get_logger().warning(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
+            except Exception as e:
+                get_logger().exception(e)
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/route_base.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-import re
-
-from typing import Callable, Dict, List, Set
-
-from nsj_rest_lib.controller.funtion_route_wrapper import FunctionRouteWrapper
-from nsj_rest_lib.dao.dao_base import DAOBase
-from nsj_rest_lib.dto.dto_base import DTOBase
-from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.service.service_base import ServiceBase
-from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
-
-
-class RouteBase:
-    url: str
-    http_method: str
-    registered_routes: List["RouteBase"] = []
-    function_wrapper: FunctionRouteWrapper
-
-    _injector_factory: NsjInjectorFactoryBase
-    _service_name: str
-    _handle_exception: Callable
-    _dto_class: DTOBase
-    _entity_class: EntityBase
-    _dto_response_class: DTOBase
-
-    def __init__(
-        self,
-        url: str,
-        http_method: str,
-        dto_class: DTOBase,
-        entity_class: EntityBase,
-        dto_response_class: DTOBase = None,
-        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
-        service_name: str = None,
-        handle_exception: Callable = None,
-    ):
-        super().__init__()
-
-        self.url = url
-        self.http_method = http_method
-        self.__class__.registered_routes.append(self)
-
-        self._injector_factory = injector_factory
-        self._service_name = service_name
-        self._handle_exception = handle_exception
-        self._dto_class = dto_class
-        self._entity_class = entity_class
-        self._dto_response_class = dto_response_class
-
-    def __call__(self, func):
-        self.function_wrapper = FunctionRouteWrapper(self, func)
-        return self.function_wrapper
-
-    def _get_service(self, factory: NsjInjectorFactoryBase) -> ServiceBase:
-        """
-        Return service instance, by service name or using NsjServiceBase.
-        """
-
-        if self._service_name is not None:
-            return factory.get_service_by_name(self._service_name)
-        else:
-            return ServiceBase(
-                factory,
-                DAOBase(factory.db_adapter(), self._entity_class),
-                self._dto_class,
-                self._entity_class,
-                self._dto_response_class
-            )
-
-    def _parse_fields(self, fields: str) -> Dict[str, Set[str]]:
-        """
-        Trata a lista de fields recebida, construindo um dict, onde as chaves
-        serão os nomes das propriedades com objetos aninhados), ou o "root"
-        indicando os campos da entidade raíz; e, os valores são listas com os
-        nomes das propriedades recebidas.
-        """
-
-        # TODO Refatorar para ser recursivo, e suportar qualquer nível de aninhamento de entidades
-
-        if fields is None:
-            fields_map = {}
-            fields_map.setdefault('root', self._dto_class.resume_fields)
-            return fields_map
-
-        fields = fields.split(',')
-
-        matcher_dot = re.compile('(.+)\.(.+)')
-        matcher_par = re.compile('(.+)\((.+)\)')
-
-        # Construindo o mapa de retorno
-        fields_map = {}
-
-        # Iterando cada field recebido
-        for field in fields:
-            field = field.strip()
-
-            match_dot = matcher_dot.match(field)
-            match_par = matcher_par.match(field)
-
-            if match_dot is not None:
-                # Tratando fields=entidade_aninhada.propriedade
-                key = match_dot.group(1)
-                value = match_dot.group(2)
-
-                # Adicionando a propriedade do objeto interno as campos root
-                root_field_list = fields_map.setdefault('root', set())
-                if not key in root_field_list:
-                    root_field_list.add(key)
-
-                field_list = fields_map.setdefault(key, set())
-                field_list.add(value)
-            elif match_par is not None:
-                # Tratando fields=entidade_aninhada(propriedade1, propriedade2)
-                key = match_dot.group(1)
-                value = match_dot.group(2)
-
-                field_list = fields_map.setdefault(key, set())
-
-                # Adicionando a propriedade do objeto interno as campos root
-                root_field_list = fields_map.setdefault('root', set())
-                if not key in root_field_list:
-                    root_field_list.add(key)
-
-                # Tratando cada campo dentro do parêntese
-                for val in value.split(','):
-                    val = val.strip()
-
-                    field_list.add(val)
-            else:
-                # Tratando propriedade simples (sem entidade aninhada)
-                root_field_list = fields_map.setdefault('root', set())
-                root_field_list.add(field)
-
-        return fields_map
+import re
+
+from typing import Callable, Dict, List, Set
+
+from nsj_rest_lib.controller.funtion_route_wrapper import FunctionRouteWrapper
+from nsj_rest_lib.dao.dao_base import DAOBase
+from nsj_rest_lib.dto.dto_base import DTOBase
+from nsj_rest_lib.entity.entity_base import EntityBase
+from nsj_rest_lib.service.service_base import ServiceBase
+from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+
+
+class RouteBase:
+    url: str
+    http_method: str
+    registered_routes: List["RouteBase"] = []
+    function_wrapper: FunctionRouteWrapper
+
+    _injector_factory: NsjInjectorFactoryBase
+    _service_name: str
+    _handle_exception: Callable
+    _dto_class: DTOBase
+    _entity_class: EntityBase
+    _dto_response_class: DTOBase
+
+    def __init__(
+        self,
+        url: str,
+        http_method: str,
+        dto_class: DTOBase,
+        entity_class: EntityBase,
+        dto_response_class: DTOBase = None,
+        injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
+        service_name: str = None,
+        handle_exception: Callable = None,
+    ):
+        super().__init__()
+
+        self.url = url
+        self.http_method = http_method
+        self.__class__.registered_routes.append(self)
+
+        self._injector_factory = injector_factory
+        self._service_name = service_name
+        self._handle_exception = handle_exception
+        self._dto_class = dto_class
+        self._entity_class = entity_class
+        self._dto_response_class = dto_response_class
+
+    def __call__(self, func):
+        self.function_wrapper = FunctionRouteWrapper(self, func)
+        return self.function_wrapper
+
+    def _get_service(self, factory: NsjInjectorFactoryBase) -> ServiceBase:
+        """
+        Return service instance, by service name or using NsjServiceBase.
+        """
+
+        if self._service_name is not None:
+            return factory.get_service_by_name(self._service_name)
+        else:
+            return ServiceBase(
+                factory,
+                DAOBase(factory.db_adapter(), self._entity_class),
+                self._dto_class,
+                self._entity_class,
+                self._dto_response_class
+            )
+
+    def _parse_fields(self, fields: str) -> Dict[str, Set[str]]:
+        """
+        Trata a lista de fields recebida, construindo um dict, onde as chaves
+        serão os nomes das propriedades com objetos aninhados), ou o "root"
+        indicando os campos da entidade raíz; e, os valores são listas com os
+        nomes das propriedades recebidas.
+        """
+
+        # TODO Refatorar para ser recursivo, e suportar qualquer nível de aninhamento de entidades
+
+        if fields is None:
+            fields_map = {}
+            fields_map.setdefault('root', self._dto_class.resume_fields)
+            return fields_map
+
+        fields = fields.split(',')
+
+        matcher_dot = re.compile('(.+)\.(.+)')
+        matcher_par = re.compile('(.+)\((.+)\)')
+
+        # Construindo o mapa de retorno
+        fields_map = {}
+
+        # Iterando cada field recebido
+        for field in fields:
+            field = field.strip()
+
+            match_dot = matcher_dot.match(field)
+            match_par = matcher_par.match(field)
+
+            if match_dot is not None:
+                # Tratando fields=entidade_aninhada.propriedade
+                key = match_dot.group(1)
+                value = match_dot.group(2)
+
+                # Adicionando a propriedade do objeto interno as campos root
+                root_field_list = fields_map.setdefault('root', set())
+                if not key in root_field_list:
+                    root_field_list.add(key)
+
+                field_list = fields_map.setdefault(key, set())
+                field_list.add(value)
+            elif match_par is not None:
+                # Tratando fields=entidade_aninhada(propriedade1, propriedade2)
+                key = match_dot.group(1)
+                value = match_dot.group(2)
+
+                field_list = fields_map.setdefault(key, set())
+
+                # Adicionando a propriedade do objeto interno as campos root
+                root_field_list = fields_map.setdefault('root', set())
+                if not key in root_field_list:
+                    root_field_list.add(key)
+
+                # Tratando cada campo dentro do parêntese
+                for val in value.split(','):
+                    val = val.strip()
+
+                    field_list.add(val)
+            else:
+                # Tratando propriedade simples (sem entidade aninhada)
+                root_field_list = fields_map.setdefault('root', set())
+                root_field_list.add(field)
+
+        return fields_map
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/dao_base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,542 +1,542 @@
-import enum
-import uuid
-
-from typing import Any, Dict, List, Tuple
-
-from nsj_rest_lib.descriptor.filter_operator import FilterOperator
-from nsj_rest_lib.entity.entity_base import EntityBase, EMPTY
-from nsj_rest_lib.entity.filter import Filter
-from nsj_rest_lib.exception import NotFoundException, AfterRecordNotFoundException
-
-from nsj_gcf_utils.db_adapter2 import DBAdapter2
-from nsj_gcf_utils.json_util import convert_to_dumps
-
-from nsj_rest_lib.settings import USE_SQL_RETURNING_CLAUSE
-
-
-class DAOBase:
-    _db: DBAdapter2
-    _entity_class: EntityBase
-
-    def __init__(
-        self,
-        db: DBAdapter2,
-        entity_class: EntityBase
-    ):
-        self._db = db
-        self._entity_class = entity_class
-
-    def begin(self):
-        """
-        Inicia uma transação no banco de dados
-        """
-        self._db.begin()
-
-    def commit(self):
-        """
-        Faz commit na transação corrente no banco de dados (se houver uma).
-
-        Não dá erro, se não houver uma transação.
-        """
-        self._db.commit()
-
-    def rollback(self):
-        """
-        Faz rollback da transação corrente no banco de dados (se houver uma).
-
-        Não dá erro, se não houver uma transação.
-        """
-        self._db.rollback()
-
-    def in_transaction(self) -> bool:
-        """
-        Verifica se há uma transação em aberto no banco de dados
-        (na verdade, verifica se há no DBAdapter, e não no BD em si).
-        """
-        return self._db.in_transaction()
-
-    def _sql_fields(self, fields: List[str] = None) -> str:
-        """
-        Returns a list of fields to build select queries (in string, with comma separator)
-        """
-
-        # Creating entity instance
-        entity = self._entity_class()
-
-        # Building SQL fields
-        if fields is None:
-            fields = [f"t0.{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_')]
-
-        return ', '.join(fields)
-
-    def get(self, id: uuid.UUID, fields: List[str] = None, filters=None) -> EntityBase:
-        """
-        Returns an entity instance by its ID.
-        """
-
-        # Creating a entity instance
-        entity = self._entity_class()
-
-        # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(filters)
-
-        # Building query
-        sql = f"""
-        select
-            {self._sql_fields(fields)}
-        from
-            {entity.get_table_name()} as t0
-        where
-            t0.{entity.get_pk_field()} = :id
-            {filters_where}
-        """
-        values = {"id": id}
-        values.update(filter_values_map)
-                
-        # Running query
-        resp = self._db.execute_query_to_model(
-            sql,
-            self._entity_class,
-            **values
-        )
-
-        # Checking if ID was found
-        if len(resp) <= 0:
-            raise NotFoundException(
-                f'{self._entity_class.__name__} com id {id} não encontrado.')
-
-        return resp[0]
-
-    def _make_filters_sql(self, filters: Dict[str, List[Filter]], with_and: bool = True, use_table_alias: bool = True) -> Tuple[str, Dict[str, Any]]:
-        """
-        Interpreta os filtros, retornando uma tupla com formato (filters_where, filter_values_map), onde
-        filters_where: Parte do SQL, a ser adicionada na cláusula where, para realização dos filtros
-        filter_values_map: Dicionário com os valores dos filtros, a serem enviados na excução da query
-
-        Se receber o parâmetro filters nulo ou vazio, retorna ('', {}).
-        """
-
-        filters_where = ''
-        filter_values_map = {}
-        if filters is not None:
-            filters_where = []
-
-            # Iterating fields with filters
-            for filter_field in filters:
-                field_filter_where_or = []
-                field_filter_where_and = []
-
-                # Iterating condictions
-                idx = -1
-                for condiction in filters[filter_field]:
-                    idx += 1
-
-                    # Resolving condiction
-                    operator = "="
-                    if condiction.operator == FilterOperator.DIFFERENT:
-                        operator = "<>"
-                    elif condiction.operator == FilterOperator.GREATER_THAN:
-                        operator = ">"
-                    elif condiction.operator == FilterOperator.LESS_THAN:
-                        operator = "<"
-                    elif condiction.operator == FilterOperator.GREATER_OR_EQUAL_THAN:
-                        operator = ">="
-                    elif condiction.operator == FilterOperator.LESS_OR_EQUAL_THAN:
-                        operator = "<="
-                    elif condiction.operator == FilterOperator.LIKE:
-                        operator = "like"
-                    elif condiction.operator == FilterOperator.ILIKE:
-                        operator = "ilike"
-
-                    # Making condiction alias
-                    condiction_alias = (
-                        f"ft_{condiction.operator.value}_{filter_field}_{idx}"
-                    )
-
-                    # Making condiction buffer
-                    if use_table_alias:
-                        condiction_buffer = (
-                            f"t0.{filter_field} {operator} :{condiction_alias}"
-                        )
-                    else:
-                        condiction_buffer = (
-                            f"{filter_field} {operator} :{condiction_alias}"
-                        )
-
-                    # Storing field filter where
-                    if operator == "=" or operator == "like" or operator == "ilike":
-                        field_filter_where_or.append(condiction_buffer)
-                    else:
-                        field_filter_where_and.append(condiction_buffer)
-
-                    # Storing condiction value
-                    if condiction.value is not None and isinstance(
-                        condiction.value.__class__, enum.EnumMeta
-                    ):
-                        filter_values_map[condiction_alias] = condiction.value.value
-                    else:
-                        filter_values_map[condiction_alias] = condiction.value
-
-                    if operator == "like" or operator == "ilike":
-                        filter_values_map[
-                            condiction_alias
-                        ] = f"%{filter_values_map[condiction_alias]}%"
-
-                # Formating condictions (with OR)
-                field_filter_where_or = " or ".join(field_filter_where_or)
-                field_filter_where_and = " and ".join(field_filter_where_and)
-                if field_filter_where_or.strip() != "":
-                    field_filter_where_or = f"({field_filter_where_or})"
-                    filters_where.append(field_filter_where_or)
-
-                if field_filter_where_and.strip() != "":
-                    field_filter_where_and = f"({field_filter_where_and})"
-                    filters_where.append(field_filter_where_and)
-
-            # Formating all filters (with AND)
-            filters_where = '\n and '.join(filters_where)
-            if filters_where.strip() != '' and with_and:
-                filters_where = f"and {filters_where}"
-
-        return (filters_where, filter_values_map)
-
-    def list(
-        self,
-        after: uuid.UUID,
-        limit: int,
-        fields: List[str],
-        order_fields: List[str],
-        filters: Dict[str, List[Filter]]
-    ) -> List[EntityBase]:
-        """
-        Returns a paginated entity list.
-        """
-
-        # Creating a entity instance
-        entity = self._entity_class()
-
-        # Cheking should use default entity order
-        if order_fields is None:
-            order_fields = entity.get_default_order_fields()
-
-        # Making order fields with alias list
-        order_fields_alias = [f"t0.{i}" for i in order_fields]
-
-        # Resolving data to pagination
-        order_map = {field: None for field in order_fields}
-
-        if after is not None:
-            try:
-                after_obj = self.get(after)
-            except NotFoundException as e:
-                raise AfterRecordNotFoundException(
-                    f'Identificador recebido no parâmetro after {id}, não encontrado para a entidade {self._entity_class.__name__}.')
-
-            if after_obj is not None:
-                for field in order_fields:
-                    order_map[field] = getattr(after_obj, field, None)
-
-        # Making default order by clause
-        order_by = f"""
-            {', '.join(order_fields_alias)}
-        """
-
-        # Organizando o where da paginação
-        pagination_where = ''
-        if after is not None:
-
-            # Making a list of pagination condictions
-            list_page_where = []
-            old_fields = []
-            for field in order_fields:
-                # Making equals condictions
-                buffer_old_fields = 'true'
-                for of in old_fields:
-                    buffer_old_fields += f" and t0.{of} = :{of}"
-
-                # Making current more than condiction
-                list_page_where.append(
-                    f"({buffer_old_fields} and t0.{field} > :{field})")
-
-                # Storing current field as old
-                old_fields.append(field)
-
-            # Making SQL page condiction
-            pagination_where = f"""
-                and (
-                    false
-                    or {' or '.join(list_page_where)}
-                )
-            """
-
-        # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(filters)
-
-        # Montando a query em si
-        sql = f"""
-        select
-
-            {self._sql_fields(fields)}
-
-        from
-            {entity.get_table_name()} as t0
-        where
-            true
-            {pagination_where}
-            {filters_where}
-        order by
-            {order_by}
-        """
-
-        # Adding limit if received
-        if limit is not None:
-            sql += f"        limit {limit}"
-
-        # Making the values dict
-        kwargs = {
-            **order_map,
-            **filter_values_map
-        }
-
-        # Running the SQL query
-        resp = self._db.execute_query_to_model(
-            sql,
-            self._entity_class,
-            **kwargs
-        )
-
-        return resp
-
-    def _sql_insert_fields(self) -> str:
-        """
-        Retorna uma tupla com duas partes: (sql_fields, sql_ref_values), onde:
-        - sql_fields: Lista de campos a inserir no insert
-        - sql_ref_values: Lista das referências aos campos, a inserir no insert (parte values)
-        """
-
-        # Creating entity instance
-        entity = self._entity_class()
-
-        # Building SQL fields
-        fields = [f"{k}" for k in entity.__dict__ if not callable(
-            getattr(entity, k, None)) and not k.startswith('_')]
-        ref_values = [f":{k}" for k in entity.__dict__ if not callable(
-            getattr(entity, k, None)) and not k.startswith('_')]
-
-        return (', '.join(fields), ', '.join(ref_values))
-
-    def insert(
-        self,
-        entity: EntityBase
-    ):
-        """
-        Insere o objeto de entidade "entity" no banco de dados
-        """
-
-        # Montando as cláusulas dos campos
-        sql_fields, sql_ref_values = self._sql_insert_fields()
-
-        # Montando a query principal
-        sql = f"""
-        insert into {entity.get_table_name()} (
-
-            {sql_fields}
-
-        ) values (
-
-            {sql_ref_values}
-
-        )
-        """
-
-        # Montando as cláusulas returning
-        returning_fields = entity.get_insert_returning_fields()
-
-        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
-            sql_returning = ', '.join(returning_fields)
-
-            sql += "\n"
-            sql += f"returning {sql_returning}"
-
-        # Montando um dicionário com valores das propriedades
-        values_map = convert_to_dumps(entity)
-
-        # Realizando o insert no BD
-        rowcount, returning = self._db.execute(
-            sql,
-            **values_map
-        )
-
-        if rowcount <= 0:
-            raise Exception(
-                f"Erro inserindo {entity.__class__.__name__} no banco de dados")
-
-        # Complementando o objeto com os dados de retorno
-        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
-            for field in returning_fields:
-                setattr(entity, field, returning[0][field])
-
-        return entity
-
-    def _sql_update_fields(self, entity: EntityBase, ignore_nones: bool = False) -> str:
-        """
-        Retorna lista com os campos para update, no padrão "field = :field"
-        """
-
-        # Building SQL fields
-        if ignore_nones:
-            fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_') and getattr(entity, k) is not None and k not in entity.get_const_fields()]
-        else:
-            fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_') and k not in entity.get_const_fields()]
-
-        return ', '.join(fields)
-
-    def update(
-        self,
-        entity: EntityBase,
-        filters: Dict[str, List[Filter]],
-        partial_update: bool = False
-    ):
-        """
-        Atualiza o objeto de entidade "entity" no banco de dados
-        """
-
-        # Montando a cláusula dos campos
-        sql_fields = self._sql_update_fields(entity, partial_update)
-
-        # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(
-            filters, False, False)
-
-        # CUIDADO PARA NÂO ATUALIZAR O QUE NÃO DEVE
-        if filters_where is None or filters_where.strip() == '':
-            raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
-
-        # Montando a query principal
-        sql = f"""
-        update {entity.get_table_name()} set
-
-            {sql_fields}
-
-        where
-
-            {filters_where}
-        """
-
-        # Montando as cláusulas returning
-        returning_fields = entity.get_update_returning_fields()
-
-        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
-            sql_returning = ', '.join(returning_fields)
-
-            sql += "\n"
-            sql += f"returning {sql_returning}"
-
-        # Montando um dicionário com valores das propriedades
-        values_map = convert_to_dumps(entity)
-
-        # Convertendo EMPTY para None, se necessário
-        if partial_update:
-            for key in values_map:
-                if values_map[key] == EMPTY:
-                    values_map[key] = None
-
-        # Montado o map de valores a passar no update
-        kwargs = {
-            **values_map,
-            **filter_values_map
-        }
-
-        # Realizando o update no BD
-        rowcount, returning = self._db.execute(
-            sql,
-            **kwargs
-        )
-
-        if rowcount <= 0:
-            raise NotFoundException(
-                f'{self._entity_class.__name__} com id {values_map[self._entity_class().get_pk_field()]} não encontrado.')
-
-        # Complementando o objeto com os dados de retorno
-        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
-            for field in returning_fields:
-                setattr(entity, field, returning[0][field])
-
-        return entity
-
-    def list_ids(self, filters: Dict[str, List[Filter]]):
-        """
-        Lista os IDs encontrados, de acordo com os filtros recebidos.
-        """
-
-        # Retorna None, se não receber filtros
-        if filters is None or len(filters) <= 0:
-            return None
-
-        # Montando uma entity fake
-        entity = self._entity_class()
-
-        # Recuperando o campo de chave primária
-        pk_field = entity.get_pk_field()
-
-        # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(filters)
-
-        # Montando a query
-        sql = f"""
-        select {pk_field} from {entity.get_table_name()} as t0 where true {filters_where}
-        """
-
-        # Executando a query
-        resp = self._db.execute_query(
-            sql,
-            **filter_values_map
-        )
-
-        # Retornando em formato de lista de IDs
-        if resp is None:
-            return None
-        else:
-            return [item[pk_field] for item in resp]
-
-    def delete(self, filters: Dict[str, List[Filter]]):
-        """
-        Exclui registros de acordo com os filtros recebidos.
-        """
-
-        # Retorna None, se não receber filtros
-        if filters is None or len(filters) <= 0:
-            raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
-
-        # Montando uma entity fake
-        entity = self._entity_class()
-
-        # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(
-            filters, False, False)
-
-        # CUIDADO PARA NÂO EXCLUIR O QUE NÃO DEVE
-        if filters_where is None or filters_where.strip() == '':
-            raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
-
-        # Montando a query
-        sql = f"""
-        delete from {entity.get_table_name()} where {filters_where}
-        """
-
-        # Executando a query
-        rowcount, _ = self._db.execute(
-            sql,
-            **filter_values_map
-        )
-
-        # Verificando se houve alguma deleção
-        if rowcount <= 0:
-            raise NotFoundException(
+import enum
+import uuid
+
+from typing import Any, Dict, List, Tuple
+
+from nsj_rest_lib.descriptor.filter_operator import FilterOperator
+from nsj_rest_lib.entity.entity_base import EntityBase, EMPTY
+from nsj_rest_lib.entity.filter import Filter
+from nsj_rest_lib.exception import NotFoundException, AfterRecordNotFoundException
+
+from nsj_gcf_utils.db_adapter2 import DBAdapter2
+from nsj_gcf_utils.json_util import convert_to_dumps
+
+from nsj_rest_lib.settings import USE_SQL_RETURNING_CLAUSE
+
+
+class DAOBase:
+    _db: DBAdapter2
+    _entity_class: EntityBase
+
+    def __init__(
+        self,
+        db: DBAdapter2,
+        entity_class: EntityBase
+    ):
+        self._db = db
+        self._entity_class = entity_class
+
+    def begin(self):
+        """
+        Inicia uma transação no banco de dados
+        """
+        self._db.begin()
+
+    def commit(self):
+        """
+        Faz commit na transação corrente no banco de dados (se houver uma).
+
+        Não dá erro, se não houver uma transação.
+        """
+        self._db.commit()
+
+    def rollback(self):
+        """
+        Faz rollback da transação corrente no banco de dados (se houver uma).
+
+        Não dá erro, se não houver uma transação.
+        """
+        self._db.rollback()
+
+    def in_transaction(self) -> bool:
+        """
+        Verifica se há uma transação em aberto no banco de dados
+        (na verdade, verifica se há no DBAdapter, e não no BD em si).
+        """
+        return self._db.in_transaction()
+
+    def _sql_fields(self, fields: List[str] = None) -> str:
+        """
+        Returns a list of fields to build select queries (in string, with comma separator)
+        """
+
+        # Creating entity instance
+        entity = self._entity_class()
+
+        # Building SQL fields
+        if fields is None:
+            fields = [f"t0.{k}" for k in entity.__dict__ if not callable(
+                getattr(entity, k, None)) and not k.startswith('_')]
+
+        return ', '.join(fields)
+
+    def get(self, id: uuid.UUID, fields: List[str] = None, filters=None) -> EntityBase:
+        """
+        Returns an entity instance by its ID.
+        """
+
+        # Creating a entity instance
+        entity = self._entity_class()
+
+        # Organizando o where dos filtros
+        filters_where, filter_values_map = self._make_filters_sql(filters)
+
+        # Building query
+        sql = f"""
+        select
+            {self._sql_fields(fields)}
+        from
+            {entity.get_table_name()} as t0
+        where
+            t0.{entity.get_pk_field()} = :id
+            {filters_where}
+        """
+        values = {"id": id}
+        values.update(filter_values_map)
+                
+        # Running query
+        resp = self._db.execute_query_to_model(
+            sql,
+            self._entity_class,
+            **values
+        )
+
+        # Checking if ID was found
+        if len(resp) <= 0:
+            raise NotFoundException(
+                f'{self._entity_class.__name__} com id {id} não encontrado.')
+
+        return resp[0]
+
+    def _make_filters_sql(self, filters: Dict[str, List[Filter]], with_and: bool = True, use_table_alias: bool = True) -> Tuple[str, Dict[str, Any]]:
+        """
+        Interpreta os filtros, retornando uma tupla com formato (filters_where, filter_values_map), onde
+        filters_where: Parte do SQL, a ser adicionada na cláusula where, para realização dos filtros
+        filter_values_map: Dicionário com os valores dos filtros, a serem enviados na excução da query
+
+        Se receber o parâmetro filters nulo ou vazio, retorna ('', {}).
+        """
+
+        filters_where = ''
+        filter_values_map = {}
+        if filters is not None:
+            filters_where = []
+
+            # Iterating fields with filters
+            for filter_field in filters:
+                field_filter_where_or = []
+                field_filter_where_and = []
+
+                # Iterating condictions
+                idx = -1
+                for condiction in filters[filter_field]:
+                    idx += 1
+
+                    # Resolving condiction
+                    operator = "="
+                    if condiction.operator == FilterOperator.DIFFERENT:
+                        operator = "<>"
+                    elif condiction.operator == FilterOperator.GREATER_THAN:
+                        operator = ">"
+                    elif condiction.operator == FilterOperator.LESS_THAN:
+                        operator = "<"
+                    elif condiction.operator == FilterOperator.GREATER_OR_EQUAL_THAN:
+                        operator = ">="
+                    elif condiction.operator == FilterOperator.LESS_OR_EQUAL_THAN:
+                        operator = "<="
+                    elif condiction.operator == FilterOperator.LIKE:
+                        operator = "like"
+                    elif condiction.operator == FilterOperator.ILIKE:
+                        operator = "ilike"
+
+                    # Making condiction alias
+                    condiction_alias = (
+                        f"ft_{condiction.operator.value}_{filter_field}_{idx}"
+                    )
+
+                    # Making condiction buffer
+                    if use_table_alias:
+                        condiction_buffer = (
+                            f"t0.{filter_field} {operator} :{condiction_alias}"
+                        )
+                    else:
+                        condiction_buffer = (
+                            f"{filter_field} {operator} :{condiction_alias}"
+                        )
+
+                    # Storing field filter where
+                    if operator == "=" or operator == "like" or operator == "ilike":
+                        field_filter_where_or.append(condiction_buffer)
+                    else:
+                        field_filter_where_and.append(condiction_buffer)
+
+                    # Storing condiction value
+                    if condiction.value is not None and isinstance(
+                        condiction.value.__class__, enum.EnumMeta
+                    ):
+                        filter_values_map[condiction_alias] = condiction.value.value
+                    else:
+                        filter_values_map[condiction_alias] = condiction.value
+
+                    if operator == "like" or operator == "ilike":
+                        filter_values_map[
+                            condiction_alias
+                        ] = f"%{filter_values_map[condiction_alias]}%"
+
+                # Formating condictions (with OR)
+                field_filter_where_or = " or ".join(field_filter_where_or)
+                field_filter_where_and = " and ".join(field_filter_where_and)
+                if field_filter_where_or.strip() != "":
+                    field_filter_where_or = f"({field_filter_where_or})"
+                    filters_where.append(field_filter_where_or)
+
+                if field_filter_where_and.strip() != "":
+                    field_filter_where_and = f"({field_filter_where_and})"
+                    filters_where.append(field_filter_where_and)
+
+            # Formating all filters (with AND)
+            filters_where = '\n and '.join(filters_where)
+            if filters_where.strip() != '' and with_and:
+                filters_where = f"and {filters_where}"
+
+        return (filters_where, filter_values_map)
+
+    def list(
+        self,
+        after: uuid.UUID,
+        limit: int,
+        fields: List[str],
+        order_fields: List[str],
+        filters: Dict[str, List[Filter]]
+    ) -> List[EntityBase]:
+        """
+        Returns a paginated entity list.
+        """
+
+        # Creating a entity instance
+        entity = self._entity_class()
+
+        # Cheking should use default entity order
+        if order_fields is None:
+            order_fields = entity.get_default_order_fields()
+
+        # Making order fields with alias list
+        order_fields_alias = [f"t0.{i}" for i in order_fields]
+
+        # Resolving data to pagination
+        order_map = {field: None for field in order_fields}
+
+        if after is not None:
+            try:
+                after_obj = self.get(after)
+            except NotFoundException as e:
+                raise AfterRecordNotFoundException(
+                    f'Identificador recebido no parâmetro after {id}, não encontrado para a entidade {self._entity_class.__name__}.')
+
+            if after_obj is not None:
+                for field in order_fields:
+                    order_map[field] = getattr(after_obj, field, None)
+
+        # Making default order by clause
+        order_by = f"""
+            {', '.join(order_fields_alias)}
+        """
+
+        # Organizando o where da paginação
+        pagination_where = ''
+        if after is not None:
+
+            # Making a list of pagination condictions
+            list_page_where = []
+            old_fields = []
+            for field in order_fields:
+                # Making equals condictions
+                buffer_old_fields = 'true'
+                for of in old_fields:
+                    buffer_old_fields += f" and t0.{of} = :{of}"
+
+                # Making current more than condiction
+                list_page_where.append(
+                    f"({buffer_old_fields} and t0.{field} > :{field})")
+
+                # Storing current field as old
+                old_fields.append(field)
+
+            # Making SQL page condiction
+            pagination_where = f"""
+                and (
+                    false
+                    or {' or '.join(list_page_where)}
+                )
+            """
+
+        # Organizando o where dos filtros
+        filters_where, filter_values_map = self._make_filters_sql(filters)
+
+        # Montando a query em si
+        sql = f"""
+        select
+
+            {self._sql_fields(fields)}
+
+        from
+            {entity.get_table_name()} as t0
+        where
+            true
+            {pagination_where}
+            {filters_where}
+        order by
+            {order_by}
+        """
+
+        # Adding limit if received
+        if limit is not None:
+            sql += f"        limit {limit}"
+
+        # Making the values dict
+        kwargs = {
+            **order_map,
+            **filter_values_map
+        }
+
+        # Running the SQL query
+        resp = self._db.execute_query_to_model(
+            sql,
+            self._entity_class,
+            **kwargs
+        )
+
+        return resp
+
+    def _sql_insert_fields(self) -> str:
+        """
+        Retorna uma tupla com duas partes: (sql_fields, sql_ref_values), onde:
+        - sql_fields: Lista de campos a inserir no insert
+        - sql_ref_values: Lista das referências aos campos, a inserir no insert (parte values)
+        """
+
+        # Creating entity instance
+        entity = self._entity_class()
+
+        # Building SQL fields
+        fields = [f"{k}" for k in entity.__dict__ if not callable(
+            getattr(entity, k, None)) and not k.startswith('_')]
+        ref_values = [f":{k}" for k in entity.__dict__ if not callable(
+            getattr(entity, k, None)) and not k.startswith('_')]
+
+        return (', '.join(fields), ', '.join(ref_values))
+
+    def insert(
+        self,
+        entity: EntityBase
+    ):
+        """
+        Insere o objeto de entidade "entity" no banco de dados
+        """
+
+        # Montando as cláusulas dos campos
+        sql_fields, sql_ref_values = self._sql_insert_fields()
+
+        # Montando a query principal
+        sql = f"""
+        insert into {entity.get_table_name()} (
+
+            {sql_fields}
+
+        ) values (
+
+            {sql_ref_values}
+
+        )
+        """
+
+        # Montando as cláusulas returning
+        returning_fields = entity.get_insert_returning_fields()
+
+        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
+            sql_returning = ', '.join(returning_fields)
+
+            sql += "\n"
+            sql += f"returning {sql_returning}"
+
+        # Montando um dicionário com valores das propriedades
+        values_map = convert_to_dumps(entity)
+
+        # Realizando o insert no BD
+        rowcount, returning = self._db.execute(
+            sql,
+            **values_map
+        )
+
+        if rowcount <= 0:
+            raise Exception(
+                f"Erro inserindo {entity.__class__.__name__} no banco de dados")
+
+        # Complementando o objeto com os dados de retorno
+        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
+            for field in returning_fields:
+                setattr(entity, field, returning[0][field])
+
+        return entity
+
+    def _sql_update_fields(self, entity: EntityBase, ignore_nones: bool = False) -> str:
+        """
+        Retorna lista com os campos para update, no padrão "field = :field"
+        """
+
+        # Building SQL fields
+        if ignore_nones:
+            fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
+                getattr(entity, k, None)) and not k.startswith('_') and getattr(entity, k) is not None and k not in entity.get_const_fields()]
+        else:
+            fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
+                getattr(entity, k, None)) and not k.startswith('_') and k not in entity.get_const_fields()]
+
+        return ', '.join(fields)
+
+    def update(
+        self,
+        entity: EntityBase,
+        filters: Dict[str, List[Filter]],
+        partial_update: bool = False
+    ):
+        """
+        Atualiza o objeto de entidade "entity" no banco de dados
+        """
+
+        # Montando a cláusula dos campos
+        sql_fields = self._sql_update_fields(entity, partial_update)
+
+        # Organizando o where dos filtros
+        filters_where, filter_values_map = self._make_filters_sql(
+            filters, False, False)
+
+        # CUIDADO PARA NÂO ATUALIZAR O QUE NÃO DEVE
+        if filters_where is None or filters_where.strip() == '':
+            raise NotFoundException(
+                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+
+        # Montando a query principal
+        sql = f"""
+        update {entity.get_table_name()} set
+
+            {sql_fields}
+
+        where
+
+            {filters_where}
+        """
+
+        # Montando as cláusulas returning
+        returning_fields = entity.get_update_returning_fields()
+
+        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
+            sql_returning = ', '.join(returning_fields)
+
+            sql += "\n"
+            sql += f"returning {sql_returning}"
+
+        # Montando um dicionário com valores das propriedades
+        values_map = convert_to_dumps(entity)
+
+        # Convertendo EMPTY para None, se necessário
+        if partial_update:
+            for key in values_map:
+                if values_map[key] == EMPTY:
+                    values_map[key] = None
+
+        # Montado o map de valores a passar no update
+        kwargs = {
+            **values_map,
+            **filter_values_map
+        }
+
+        # Realizando o update no BD
+        rowcount, returning = self._db.execute(
+            sql,
+            **kwargs
+        )
+
+        if rowcount <= 0:
+            raise NotFoundException(
+                f'{self._entity_class.__name__} com id {values_map[self._entity_class().get_pk_field()]} não encontrado.')
+
+        # Complementando o objeto com os dados de retorno
+        if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
+            for field in returning_fields:
+                setattr(entity, field, returning[0][field])
+
+        return entity
+
+    def list_ids(self, filters: Dict[str, List[Filter]]):
+        """
+        Lista os IDs encontrados, de acordo com os filtros recebidos.
+        """
+
+        # Retorna None, se não receber filtros
+        if filters is None or len(filters) <= 0:
+            return None
+
+        # Montando uma entity fake
+        entity = self._entity_class()
+
+        # Recuperando o campo de chave primária
+        pk_field = entity.get_pk_field()
+
+        # Organizando o where dos filtros
+        filters_where, filter_values_map = self._make_filters_sql(filters)
+
+        # Montando a query
+        sql = f"""
+        select {pk_field} from {entity.get_table_name()} as t0 where true {filters_where}
+        """
+
+        # Executando a query
+        resp = self._db.execute_query(
+            sql,
+            **filter_values_map
+        )
+
+        # Retornando em formato de lista de IDs
+        if resp is None:
+            return None
+        else:
+            return [item[pk_field] for item in resp]
+
+    def delete(self, filters: Dict[str, List[Filter]]):
+        """
+        Exclui registros de acordo com os filtros recebidos.
+        """
+
+        # Retorna None, se não receber filtros
+        if filters is None or len(filters) <= 0:
+            raise NotFoundException(
+                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+
+        # Montando uma entity fake
+        entity = self._entity_class()
+
+        # Organizando o where dos filtros
+        filters_where, filter_values_map = self._make_filters_sql(
+            filters, False, False)
+
+        # CUIDADO PARA NÂO EXCLUIR O QUE NÃO DEVE
+        if filters_where is None or filters_where.strip() == '':
+            raise NotFoundException(
+                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+
+        # Montando a query
+        sql = f"""
+        delete from {entity.get_table_name()} where {filters_where}
+        """
+
+        # Executando a query
+        rowcount, _ = self._db.execute(
+            sql,
+            **filter_values_map
+        )
+
+        # Verificando se houve alguma deleção
+        if rowcount <= 0:
+            raise NotFoundException(
                 f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/db_pool_config.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from nsj_rest_lib.settings import DATABASE_HOST
-from nsj_rest_lib.settings import DATABASE_PASS
-from nsj_rest_lib.settings import DATABASE_PORT
-from nsj_rest_lib.settings import DATABASE_NAME
-from nsj_rest_lib.settings import DATABASE_USER
-from nsj_rest_lib.settings import DATABASE_DRIVER
-from nsj_rest_lib.settings import CLOUD_SQL_CONN_NAME
-from nsj_rest_lib.settings import ENV
-
-import sqlalchemy
-
-
-def create_pool(database_conn_url):
-    # Creating database connection pool
-    db_pool = sqlalchemy.create_engine(
-        database_conn_url,
-        pool_size=5,
-        max_overflow=2,
-        pool_timeout=30,
-        pool_recycle=1800
-    )
-    return db_pool
-
-
-if DATABASE_DRIVER.upper() == 'SINGLE_STORE':
-    database_conn_url = f'mysql+pymysql://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}'
-else:
-    if ENV.upper() == 'GCP':
-        database_conn_url = f'postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@/{DATABASE_NAME}?unix_sock=/cloudsql/{CLOUD_SQL_CONN_NAME}/.s.PGSQL.{DATABASE_PORT}'
-    else:
-        database_conn_url = f'postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}'
-
-db_pool = create_pool(database_conn_url)
+from nsj_rest_lib.settings import DATABASE_HOST
+from nsj_rest_lib.settings import DATABASE_PASS
+from nsj_rest_lib.settings import DATABASE_PORT
+from nsj_rest_lib.settings import DATABASE_NAME
+from nsj_rest_lib.settings import DATABASE_USER
+from nsj_rest_lib.settings import DATABASE_DRIVER
+from nsj_rest_lib.settings import CLOUD_SQL_CONN_NAME
+from nsj_rest_lib.settings import ENV
+
+import sqlalchemy
+
+
+def create_pool(database_conn_url):
+    # Creating database connection pool
+    db_pool = sqlalchemy.create_engine(
+        database_conn_url,
+        pool_size=5,
+        max_overflow=2,
+        pool_timeout=30,
+        pool_recycle=1800
+    )
+    return db_pool
+
+
+if DATABASE_DRIVER.upper() == 'SINGLE_STORE':
+    database_conn_url = f'mysql+pymysql://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}'
+else:
+    if ENV.upper() == 'GCP':
+        database_conn_url = f'postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@/{DATABASE_NAME}?unix_sock=/cloudsql/{CLOUD_SQL_CONN_NAME}/.s.PGSQL.{DATABASE_PORT}'
+    else:
+        database_conn_url = f'postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}'
+
+db_pool = create_pool(database_conn_url)
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/dto.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-from typing import Any, Dict
-from nsj_rest_lib.descriptor.dto_field import DTOField
-from nsj_rest_lib.descriptor.dto_list_field import DTOListField
-
-
-class DTO:
-    def __init__(
-        self,
-        fixed_filters: Dict[str, Any] = None
-    ) -> None:
-        super().__init__()
-
-        self._fixed_filters = fixed_filters
-
-    def __call__(self, cls: object):
-        """
-        Iterating DTO class to handle DTOFields descriptors.
-        """
-
-        # Creating resume_fields in cls, if needed
-        self._check_class_attribute(cls, 'resume_fields', set())
-
-        # Creating fields_map in cls, if needed
-        self._check_class_attribute(cls, 'fields_map', {})
-
-        # Creating list_fields_map in cls, if needed
-        self._check_class_attribute(cls, 'list_fields_map', {})
-
-        # Creating field_filters_map in cls, if needed
-        self._check_class_attribute(cls, 'field_filters_map', {})
-
-        # Creating pk_field in cls, if needed
-        # TODO Refatorar para suportar PKs compostas
-        self._check_class_attribute(cls, 'pk_field', None)
-
-        # Criando a propriedade "partition_fields" na classe "cls", se necessário
-        self._check_class_attribute(cls, 'partition_fields', set())
-
-        # Iterating for the class attributes
-        for key, attr in cls.__dict__.items():
-            # Test if the attribute uses the DTOFiel descriptor
-            if isinstance(attr, DTOField):
-                # Storing field in fields_map
-                getattr(cls, 'fields_map')[key] = attr
-
-                # Setting a better name to storage_name
-                attr.storage_name = f"{key}"
-
-                # Checking filters name
-                self._check_filters(cls, key, attr)
-
-                # Copying type from annotation (if exists)
-                if key in cls.__annotations__:
-                    attr.expected_type = cls.__annotations__[key]
-
-                # Checking if it is a resume field (to store)
-                if attr.resume:
-                    resume_fields = getattr(cls, 'resume_fields')
-                    if not (key in resume_fields):
-                        resume_fields.add(key)
-
-                # TODO Refatorar para suportar PKs compostas
-                # Setting PK info
-                if attr.pk:
-                    setattr(cls, 'pk_field', f"{key}")
-
-                # Verifica se é um campo de particionamento, e o guarda em caso positivo
-                if attr.partition_data:
-                    partition_fields = getattr(cls, 'partition_fields')
-                    if not (key in partition_fields):
-                        partition_fields.add(key)
-
-            elif isinstance(attr, DTOListField):
-                # Storing field in fields_map
-                getattr(cls, 'list_fields_map')[key] = attr
-
-                # Setting a better name to storage_name
-                attr.storage_name = f"{key}"
-
-        # Setting fixed filters
-        setattr(cls, 'fixed_filters', self._fixed_filters)
-
-        return cls
-
-    def _check_filters(self, cls: object, field_name: str, dto_field: DTOField):
-        """
-        Check filters (if exists), and setting default filter name.
-        """
-
-        if dto_field.filters is None:
-            return
-
-        # Handling each filter
-        for filter in dto_field.filters:
-
-            # Resolving filter name
-            filter_name = field_name
-            if filter.name is not None:
-                filter_name = filter.name
-
-            # Storing field filter name
-            filter.field_name = field_name
-
-            # Adding into field filters map
-            field_filters_map = getattr(cls, 'field_filters_map')
-            field_filters_map[filter_name] = filter
-
-    def _check_class_attribute(self, cls: object, attr_name: str, default_value: Any):
-        """
-        Add attribute "attr_name" in class "cls", if not exists.
-        """
-
-        if attr_name not in cls.__dict__:
-            setattr(cls, attr_name, default_value)
+from typing import Any, Dict
+from nsj_rest_lib.descriptor.dto_field import DTOField
+from nsj_rest_lib.descriptor.dto_list_field import DTOListField
+
+
+class DTO:
+    def __init__(
+        self,
+        fixed_filters: Dict[str, Any] = None
+    ) -> None:
+        super().__init__()
+
+        self._fixed_filters = fixed_filters
+
+    def __call__(self, cls: object):
+        """
+        Iterating DTO class to handle DTOFields descriptors.
+        """
+
+        # Creating resume_fields in cls, if needed
+        self._check_class_attribute(cls, 'resume_fields', set())
+
+        # Creating fields_map in cls, if needed
+        self._check_class_attribute(cls, 'fields_map', {})
+
+        # Creating list_fields_map in cls, if needed
+        self._check_class_attribute(cls, 'list_fields_map', {})
+
+        # Creating field_filters_map in cls, if needed
+        self._check_class_attribute(cls, 'field_filters_map', {})
+
+        # Creating pk_field in cls, if needed
+        # TODO Refatorar para suportar PKs compostas
+        self._check_class_attribute(cls, 'pk_field', None)
+
+        # Criando a propriedade "partition_fields" na classe "cls", se necessário
+        self._check_class_attribute(cls, 'partition_fields', set())
+
+        # Iterating for the class attributes
+        for key, attr in cls.__dict__.items():
+            # Test if the attribute uses the DTOFiel descriptor
+            if isinstance(attr, DTOField):
+                # Storing field in fields_map
+                getattr(cls, 'fields_map')[key] = attr
+
+                # Setting a better name to storage_name
+                attr.storage_name = f"{key}"
+
+                # Checking filters name
+                self._check_filters(cls, key, attr)
+
+                # Copying type from annotation (if exists)
+                if key in cls.__annotations__:
+                    attr.expected_type = cls.__annotations__[key]
+
+                # Checking if it is a resume field (to store)
+                if attr.resume:
+                    resume_fields = getattr(cls, 'resume_fields')
+                    if not (key in resume_fields):
+                        resume_fields.add(key)
+
+                # TODO Refatorar para suportar PKs compostas
+                # Setting PK info
+                if attr.pk:
+                    setattr(cls, 'pk_field', f"{key}")
+
+                # Verifica se é um campo de particionamento, e o guarda em caso positivo
+                if attr.partition_data:
+                    partition_fields = getattr(cls, 'partition_fields')
+                    if not (key in partition_fields):
+                        partition_fields.add(key)
+
+            elif isinstance(attr, DTOListField):
+                # Storing field in fields_map
+                getattr(cls, 'list_fields_map')[key] = attr
+
+                # Setting a better name to storage_name
+                attr.storage_name = f"{key}"
+
+        # Setting fixed filters
+        setattr(cls, 'fixed_filters', self._fixed_filters)
+
+        return cls
+
+    def _check_filters(self, cls: object, field_name: str, dto_field: DTOField):
+        """
+        Check filters (if exists), and setting default filter name.
+        """
+
+        if dto_field.filters is None:
+            return
+
+        # Handling each filter
+        for filter in dto_field.filters:
+
+            # Resolving filter name
+            filter_name = field_name
+            if filter.name is not None:
+                filter_name = filter.name
+
+            # Storing field filter name
+            filter.field_name = field_name
+
+            # Adding into field filters map
+            field_filters_map = getattr(cls, 'field_filters_map')
+            field_filters_map[filter_name] = filter
+
+    def _check_class_attribute(self, cls: object, attr_name: str, default_value: Any):
+        """
+        Add attribute "attr_name" in class "cls", if not exists.
+        """
+
+        if attr_name not in cls.__dict__:
+            setattr(cls, attr_name, default_value)
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,269 +1,269 @@
-import datetime
-import enum
-import re
-import typing
-
-from decimal import Decimal
-import uuid
-
-from nsj_rest_lib.descriptor.filter_operator import FilterOperator
-
-
-class DTOFieldFilter:
-    def __init__(
-        self, name: str = None, operator: FilterOperator = FilterOperator.EQUALS
-    ):
-        self.name = name
-        self.operator = operator
-        self.field_name = None
-
-    def set_field_name(self, field_name: str):
-        self.field_name = field_name
-
-
-class DTOField:
-    _ref_counter = 0
-
-    def __init__(
-        self,
-        type: object = None,
-        not_null: bool = False,
-        resume: bool = False,
-        min: int = None,
-        max: int = None,
-        validator: typing.Callable = None,
-        strip: bool = False,
-        entity_field: str = None,
-        filters: typing.List[DTOFieldFilter] = None,
-        pk: bool = False,
-        use_default_validator: bool = True,
-        default_value: typing.Union[typing.Callable, typing.Any] = None,
-        partition_data: bool = False,
-    ):
-        """
-        -----------
-        Parameters:
-        -----------
-        type: Expected type for the field. If it is an enum.Enum, the receive value (to set), will be converted.
-        not_null: The field cannot be None (or empty, for strings).
-        resume: The field is used as a resume field (returned in get list request).
-        min: Min value expected (min length for strings, and min value for int, float or Decimal).
-        max: Max value expected (max length for strings, and amx value for int, float or Decimal).
-        validator: Function that receives the value (to be setted), and returns the same value (after any adjust).
-          This function overrides the default behaviour and all default constraints.
-        strip: Usefull only for strings. The value will be stript before stored.
-        entity_field: Name of equivalent field in entity class.
-        """
-        self.expected_type = type
-        self.not_null = not_null
-        self.resume = resume
-        self.min = min
-        self.max = max
-        self.validator = validator
-        self.strip = strip
-        self.entity_field = entity_field
-        self.filters = filters
-        self.pk = pk
-        self.use_default_validator = use_default_validator
-        self.default_value = default_value
-        self.partition_data = partition_data
-
-        self.storage_name = f"_{self.__class__.__name__}#{self.__class__._ref_counter}"
-        self.__class__._ref_counter += 1
-
-    def __get__(self, instance, owner):
-        if instance is None:
-            return self
-        else:
-            return instance.__dict__[self.storage_name]
-
-    def __set__(self, instance, value):
-        if self.validator is None:
-            if self.use_default_validator:
-                value = self.validate(self, value)
-        else:
-            if self.use_default_validator:
-                value = self.validate(self, value)
-            value = self.validator(self, value)
-
-        instance.__dict__[self.storage_name] = value
-
-    def validate(self, dto_field: "DTOField", value):
-        """
-        Default validator (ckecking default constraints: not null, type, min, max and enum types).
-        """
-
-        # Checking not null constraint
-        if (self.not_null) and (
-            value is None or (isinstance(value, str) and len(value.strip()) <= 0)
-        ):
-            raise ValueError(
-                f"{self.storage_name} deve estar preenchido. Valor recebido: {value}."
-            )
-
-        # Checking type constraint
-        # TODO Ver como suportar typing
-        if (
-            self.expected_type is not None
-            and not isinstance(value, self.expected_type)
-            and value is not None
-        ):
-            value = self.validate_type(value)
-
-        # Checking min constraint
-        if self.min is not None:
-            if isinstance(value, str) and (len(value) < self.min):
-                raise ValueError(
-                    f"{self.storage_name} deve conter no mínimo {self.min} caracteres. Valor recebido: {value}."
-                )
-            elif (
-                isinstance(value, int)
-                or isinstance(value, float)
-                or isinstance(value, Decimal)
-            ) and (value < self.min):
-                raise ValueError(
-                    f"{self.storage_name} deve ser maior ou igual a {self.min}. Valor recebido: {value}."
-                )
-
-        # Checking min constraint
-        if self.max is not None:
-            if isinstance(value, str) and (len(value) > self.max):
-                raise ValueError(
-                    f"{self.storage_name} deve conter no máximo {self.max} caracteres. Valor recebido: {value}."
-                )
-            elif (
-                isinstance(value, int)
-                or isinstance(value, float)
-                or isinstance(value, Decimal)
-            ) and (value > self.max):
-                raise ValueError(
-                    f"{self.storage_name} deve ser menor ou igual a {self.max}. Valor recebido: {value}."
-                )
-
-        # Striping strings (if desired)
-        if isinstance(value, str) and self.strip:
-            value = value.strip()
-
-        return value
-
-    def validate_type(self, value):
-        """
-        Valida o value recebido, de acordo com o tipo esperado, e faz as conversões necessárias (se possível).
-        """
-
-        # Montando expressões regulares para as validações
-        matcher_uuid = re.compile(
-            "^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$"
-        )
-        matcher_datetime = re.compile(
-            "^(\d\d\d\d)-(\d\d)-(\d\d)[T,t](\d\d):(\d\d):(\d\d)$"
-        )
-        matcher_date = re.compile("^(\d\d\d\d)-(\d\d)-(\d\d)$")
-
-        # Validação direta de tipos
-        erro_tipo = False
-        if self.expected_type is datetime.datetime and isinstance(value, str):
-            match_datetime = matcher_datetime.search(value)
-            match_date = matcher_date.search(value)
-
-            if match_datetime:
-                ano = int(match_datetime.group(1))
-                mes = int(match_datetime.group(2))
-                dia = int(match_datetime.group(3))
-                hora = int(match_datetime.group(4))
-                minuto = int(match_datetime.group(5))
-                segundo = int(match_datetime.group(6))
-
-                value = datetime.datetime(
-                    year=ano,
-                    month=mes,
-                    day=dia,
-                    hour=hora,
-                    minute=minuto,
-                    second=segundo,
-                )
-            elif match_date:
-                ano = int(match_date.group(1))
-                mes = int(match_date.group(2))
-                dia = int(match_date.group(3))
-
-                value = datetime.datetime(
-                    year=ano, month=mes, day=dia, hour=0, minute=0, second=0
-                )
-            else:
-                erro_tipo = True
-        elif self.expected_type is datetime.date and isinstance(value, str):
-            match_date = matcher_date.search(value)
-
-            if match_date:
-                ano = int(match_date.group(1))
-                mes = int(match_date.group(2))
-                dia = int(match_date.group(3))
-
-                value = datetime.date(year=ano, month=mes, day=dia)
-            else:
-                erro_tipo = True
-        elif isinstance(self.expected_type, enum.EnumMeta):
-            # Enumerados
-            try:
-                value = self.expected_type(value)
-            except ValueError as e:
-                raise ValueError(
-                    f"{self.storage_name} não é um {self.expected_type.__name__} válido. Valor recebido: {value}."
-                )
-        elif self.expected_type is bool and isinstance(value, int):
-            # Booleanos
-            # Converting int to bool (0 is False, otherwise is True)
-            value = bool(value)
-        elif self.expected_type is datetime.datetime and isinstance(value, datetime.date):
-            # Datetime
-            # Assumindo hora 0, minuto 0 e segundo 0 (quanto é recebida uma data para campo data + hora)
-            value = datetime.datetime(
-                value.year, value.month, value.day, 0, 0, 0)
-        elif self.expected_type is datetime.date and isinstance(value, datetime.datetime):
-            # Date
-            # Desprezando hora , minuto e segundo (quanto é recebida uma data + hora, para campo de data)
-            value = datetime.date(
-                value.year, value.month, value.day)
-        elif self.expected_type is uuid.UUID and isinstance(value, str):
-            # UUID
-            # Verificando se pode ser alterado de str para UUID
-            match_uuid = matcher_uuid.search(value)
-
-            if match_uuid:
-                value = uuid.UUID(value)
-            else:
-                erro_tipo = True
-        elif self.expected_type is int:
-            # Int
-            try:
-                value = int(value)
-            except:
-                erro_tipo = True
-        elif self.expected_type is float:
-            # Int
-            try:
-                value = float(value)
-            except:
-                erro_tipo = True
-        elif self.expected_type is Decimal:
-            # Int
-            try:
-                value = Decimal(value)
-            except:
-                erro_tipo = True
-        elif self.expected_type is str:
-            # Int
-            try:
-                value = str(value)
-            except:
-                erro_tipo = True
-        else:
-            erro_tipo = True
-
-        if erro_tipo:
-            raise ValueError(
-                f"{self.storage_name} deve ser do tipo {self.expected_type.__name__}. Valor recebido: {value}."
-            )
-
-        return value
+import datetime
+import enum
+import re
+import typing
+
+from decimal import Decimal
+import uuid
+
+from nsj_rest_lib.descriptor.filter_operator import FilterOperator
+
+
+class DTOFieldFilter:
+    def __init__(
+        self, name: str = None, operator: FilterOperator = FilterOperator.EQUALS
+    ):
+        self.name = name
+        self.operator = operator
+        self.field_name = None
+
+    def set_field_name(self, field_name: str):
+        self.field_name = field_name
+
+
+class DTOField:
+    _ref_counter = 0
+
+    def __init__(
+        self,
+        type: object = None,
+        not_null: bool = False,
+        resume: bool = False,
+        min: int = None,
+        max: int = None,
+        validator: typing.Callable = None,
+        strip: bool = False,
+        entity_field: str = None,
+        filters: typing.List[DTOFieldFilter] = None,
+        pk: bool = False,
+        use_default_validator: bool = True,
+        default_value: typing.Union[typing.Callable, typing.Any] = None,
+        partition_data: bool = False,
+    ):
+        """
+        -----------
+        Parameters:
+        -----------
+        type: Expected type for the field. If it is an enum.Enum, the receive value (to set), will be converted.
+        not_null: The field cannot be None (or empty, for strings).
+        resume: The field is used as a resume field (returned in get list request).
+        min: Min value expected (min length for strings, and min value for int, float or Decimal).
+        max: Max value expected (max length for strings, and amx value for int, float or Decimal).
+        validator: Function that receives the value (to be setted), and returns the same value (after any adjust).
+          This function overrides the default behaviour and all default constraints.
+        strip: Usefull only for strings. The value will be stript before stored.
+        entity_field: Name of equivalent field in entity class.
+        """
+        self.expected_type = type
+        self.not_null = not_null
+        self.resume = resume
+        self.min = min
+        self.max = max
+        self.validator = validator
+        self.strip = strip
+        self.entity_field = entity_field
+        self.filters = filters
+        self.pk = pk
+        self.use_default_validator = use_default_validator
+        self.default_value = default_value
+        self.partition_data = partition_data
+
+        self.storage_name = f"_{self.__class__.__name__}#{self.__class__._ref_counter}"
+        self.__class__._ref_counter += 1
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        else:
+            return instance.__dict__[self.storage_name]
+
+    def __set__(self, instance, value):
+        if self.validator is None:
+            if self.use_default_validator:
+                value = self.validate(self, value)
+        else:
+            if self.use_default_validator:
+                value = self.validate(self, value)
+            value = self.validator(self, value)
+
+        instance.__dict__[self.storage_name] = value
+
+    def validate(self, dto_field: "DTOField", value):
+        """
+        Default validator (ckecking default constraints: not null, type, min, max and enum types).
+        """
+
+        # Checking not null constraint
+        if (self.not_null) and (
+            value is None or (isinstance(value, str) and len(value.strip()) <= 0)
+        ):
+            raise ValueError(
+                f"{self.storage_name} deve estar preenchido. Valor recebido: {value}."
+            )
+
+        # Checking type constraint
+        # TODO Ver como suportar typing
+        if (
+            self.expected_type is not None
+            and not isinstance(value, self.expected_type)
+            and value is not None
+        ):
+            value = self.validate_type(value)
+
+        # Checking min constraint
+        if self.min is not None:
+            if isinstance(value, str) and (len(value) < self.min):
+                raise ValueError(
+                    f"{self.storage_name} deve conter no mínimo {self.min} caracteres. Valor recebido: {value}."
+                )
+            elif (
+                isinstance(value, int)
+                or isinstance(value, float)
+                or isinstance(value, Decimal)
+            ) and (value < self.min):
+                raise ValueError(
+                    f"{self.storage_name} deve ser maior ou igual a {self.min}. Valor recebido: {value}."
+                )
+
+        # Checking min constraint
+        if self.max is not None:
+            if isinstance(value, str) and (len(value) > self.max):
+                raise ValueError(
+                    f"{self.storage_name} deve conter no máximo {self.max} caracteres. Valor recebido: {value}."
+                )
+            elif (
+                isinstance(value, int)
+                or isinstance(value, float)
+                or isinstance(value, Decimal)
+            ) and (value > self.max):
+                raise ValueError(
+                    f"{self.storage_name} deve ser menor ou igual a {self.max}. Valor recebido: {value}."
+                )
+
+        # Striping strings (if desired)
+        if isinstance(value, str) and self.strip:
+            value = value.strip()
+
+        return value
+
+    def validate_type(self, value):
+        """
+        Valida o value recebido, de acordo com o tipo esperado, e faz as conversões necessárias (se possível).
+        """
+
+        # Montando expressões regulares para as validações
+        matcher_uuid = re.compile(
+            "^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$"
+        )
+        matcher_datetime = re.compile(
+            "^(\d\d\d\d)-(\d\d)-(\d\d)[T,t](\d\d):(\d\d):(\d\d)$"
+        )
+        matcher_date = re.compile("^(\d\d\d\d)-(\d\d)-(\d\d)$")
+
+        # Validação direta de tipos
+        erro_tipo = False
+        if self.expected_type is datetime.datetime and isinstance(value, str):
+            match_datetime = matcher_datetime.search(value)
+            match_date = matcher_date.search(value)
+
+            if match_datetime:
+                ano = int(match_datetime.group(1))
+                mes = int(match_datetime.group(2))
+                dia = int(match_datetime.group(3))
+                hora = int(match_datetime.group(4))
+                minuto = int(match_datetime.group(5))
+                segundo = int(match_datetime.group(6))
+
+                value = datetime.datetime(
+                    year=ano,
+                    month=mes,
+                    day=dia,
+                    hour=hora,
+                    minute=minuto,
+                    second=segundo,
+                )
+            elif match_date:
+                ano = int(match_date.group(1))
+                mes = int(match_date.group(2))
+                dia = int(match_date.group(3))
+
+                value = datetime.datetime(
+                    year=ano, month=mes, day=dia, hour=0, minute=0, second=0
+                )
+            else:
+                erro_tipo = True
+        elif self.expected_type is datetime.date and isinstance(value, str):
+            match_date = matcher_date.search(value)
+
+            if match_date:
+                ano = int(match_date.group(1))
+                mes = int(match_date.group(2))
+                dia = int(match_date.group(3))
+
+                value = datetime.date(year=ano, month=mes, day=dia)
+            else:
+                erro_tipo = True
+        elif isinstance(self.expected_type, enum.EnumMeta):
+            # Enumerados
+            try:
+                value = self.expected_type(value)
+            except ValueError as e:
+                raise ValueError(
+                    f"{self.storage_name} não é um {self.expected_type.__name__} válido. Valor recebido: {value}."
+                )
+        elif self.expected_type is bool and isinstance(value, int):
+            # Booleanos
+            # Converting int to bool (0 is False, otherwise is True)
+            value = bool(value)
+        elif self.expected_type is datetime.datetime and isinstance(value, datetime.date):
+            # Datetime
+            # Assumindo hora 0, minuto 0 e segundo 0 (quanto é recebida uma data para campo data + hora)
+            value = datetime.datetime(
+                value.year, value.month, value.day, 0, 0, 0)
+        elif self.expected_type is datetime.date and isinstance(value, datetime.datetime):
+            # Date
+            # Desprezando hora , minuto e segundo (quanto é recebida uma data + hora, para campo de data)
+            value = datetime.date(
+                value.year, value.month, value.day)
+        elif self.expected_type is uuid.UUID and isinstance(value, str):
+            # UUID
+            # Verificando se pode ser alterado de str para UUID
+            match_uuid = matcher_uuid.search(value)
+
+            if match_uuid:
+                value = uuid.UUID(value)
+            else:
+                erro_tipo = True
+        elif self.expected_type is int:
+            # Int
+            try:
+                value = int(value)
+            except:
+                erro_tipo = True
+        elif self.expected_type is float:
+            # Int
+            try:
+                value = float(value)
+            except:
+                erro_tipo = True
+        elif self.expected_type is Decimal:
+            # Int
+            try:
+                value = Decimal(value)
+            except:
+                erro_tipo = True
+        elif self.expected_type is str:
+            # Int
+            try:
+                value = str(value)
+            except:
+                erro_tipo = True
+        else:
+            erro_tipo = True
+
+        if erro_tipo:
+            raise ValueError(
+                f"{self.storage_name} deve ser do tipo {self.expected_type.__name__}. Valor recebido: {value}."
+            )
+
+        return value
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-import re
-import uuid
-
-from nsj_rest_lib.descriptor.dto_field import DTOField
-
-
-class DTOFieldValidators:
-
-    def validate_cpf_or_cnpj(self, dto_field: DTOField, value):
-        """
-        Valida se é um CPF ou CNPJ.
-        """
-
-        if value is None:
-            return None
-
-        if not isinstance(value, str):
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
-
-        value = self._remove_not_number_chars(value)
-
-        if self._is_cpf_or_cnpj(value):
-            return value
-        else:
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser um CPF ou CNPJ. Valor recebido: {value}.")
-
-    def validate_cpf(self, dto_field: DTOField, value):
-        """
-        Valida se é um CPF.
-        """
-
-        if value is None:
-            return None
-
-        if not isinstance(value, str):
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
-
-        value = self._remove_not_number_chars(value)
-
-        if self._is_cpf(value):
-            return value
-        else:
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser um CPF. Valor recebido: {value}.")
-
-    def validate_cnpj(self, dto_field: DTOField, value):
-        """
-        Valida se é um CNPJ.
-        """
-
-        if value is None:
-            return None
-
-        if not isinstance(value, str):
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
-
-        value = self._remove_not_number_chars(value)
-
-        if self._is_cnpj(value):
-            return value
-        else:
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser um CNPJ. Valor recebido: {value}.")
-
-    def validate_uuid(self, dto_field: DTOField, value):
-        """
-        Valida se é um UUID.
-        """
-
-        if value is None:
-            return None
-
-        if isinstance(value, uuid.UUID):
-            return value
-
-        if not isinstance(value, str):
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser um UUID ou string correspondente. Valor recebido: {value}.")
-
-        value = value.strip()
-
-        if self._is_uuid(value):
-            return uuid.UUID(value)
-        else:
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser um UUID. Valor recebido: {value}.")
-
-    def validate_email(self, dto_field: DTOField, value):
-        """
-        Valida se é um UUID.
-        """
-
-        if value is None:
-            return None
-
-        if not isinstance(value, str):
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
-
-        value = value.strip()
-
-        if self._is_email(value):
-            return value
-        else:
-            raise ValueError(
-                f"{dto_field.storage_name} deve ser um e-mail válido. Valor recebido: {value}.")
-
-    ######################
-    # Métodos Auxiliares #
-    ######################
-
-    def _remove_not_number_chars(self, value):
-        return re.sub("[^0-9]", '', value)
-
-    def _is_cpf(self, cpf: str) -> bool:
-        """ If cpf in the Brazilian format is valid, it returns True, otherwise, it returns False. """
-
-        # Check if type is str
-        if not isinstance(cpf, str):
-            return False
-
-        # Removing not number chars:
-        cpf = self._remove_not_number_chars(cpf)
-
-        # Verify if CPF number is equal
-        if cpf in ['12345678909', '00000000000', '11111111111', '22222222222', '33333333333', '44444444444', '55555555555', '66666666666', '77777777777', '88888888888', '99999999999']:
-            return False
-
-        # Checks if string has 11 characters
-        if len(cpf) != 11:
-            return False
-
-        sum = 0
-        weight = 10
-
-        """ Calculating the first cpf check digit. """
-        for n in range(9):
-            sum = sum + int(cpf[n]) * weight
-
-            # Decrement weight
-            weight = weight - 1
-
-        verifyingDigit = 11 - sum % 11
-
-        if verifyingDigit > 9:
-            firstVerifyingDigit = 0
-        else:
-            firstVerifyingDigit = verifyingDigit
-
-        """ Calculating the second check digit of cpf. """
-        sum = 0
-        weight = 11
-        for n in range(10):
-            sum = sum + int(cpf[n]) * weight
-
-            # Decrement weight
-            weight = weight - 1
-
-        verifyingDigit = 11 - sum % 11
-
-        if verifyingDigit > 9:
-            secondVerifyingDigit = 0
-        else:
-            secondVerifyingDigit = verifyingDigit
-
-        if cpf[-2:] == "%s%s" % (firstVerifyingDigit, secondVerifyingDigit):
-            return True
-        return False
-
-    def _is_cnpj(self, cnpj: str) -> bool:
-        """ 
-        Method to validate brazilian cnpjs
-        """
-
-        # defining some variables
-        lista_validacao_um = [5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
-        lista_validacao_dois = [6, 5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
-
-        # Removing not number chars:
-        cnpj = self._remove_not_number_chars(cnpj)
-
-        # finding out the digits
-        verificadores = cnpj[-2:]
-
-        # verifying the lenght of the cnpj
-        if len(cnpj) != 14:
-            return False
-
-        # calculating the first digit
-        soma = 0
-        id = 0
-        for numero in cnpj:
-
-            # to do not raise indexerrors
-            try:
-                lista_validacao_um[id]
-            except:
-                break
-
-            soma += int(numero) * int(lista_validacao_um[id])
-            id += 1
-
-        soma = soma % 11
-        if soma < 2:
-            digito_um = 0
-        else:
-            digito_um = 11 - soma
-
-        # converting to string, for later comparison
-        digito_um = str(digito_um)
-
-        # calculating the second digit
-        # suming the two lists
-        soma = 0
-        id = 0
-
-        # suming the two lists
-        for numero in cnpj:
-
-            # to do not raise indexerrors
-            try:
-                lista_validacao_dois[id]
-            except:
-                break
-
-            soma += int(numero) * int(lista_validacao_dois[id])
-            id += 1
-
-        # defining the digit
-        soma = soma % 11
-        if soma < 2:
-            digito_dois = 0
-        else:
-            digito_dois = 11 - soma
-
-        digito_dois = str(digito_dois)
-
-        # returnig
-        return bool(verificadores == digito_um + digito_dois)
-
-    def _is_cpf_or_cnpj(self, cpf_cnpj: str) -> bool:
-        """
-        Validate a brazilian CPF ou CNPJ.
-        """
-
-        # Removing not number chars:
-        cpf_cnpj = self._remove_not_number_chars(cpf_cnpj)
-
-        if len(cpf_cnpj) == 11:
-            return self._is_cpf(cpf_cnpj)
-        elif len(cpf_cnpj) == 14:
-            return self._is_cnpj(cpf_cnpj)
-        else:
-            return False
-
-    def _is_uuid(self, value: str) -> bool:
-        """
-        Validate a UUID or UUID in string
-        """
-        value = str(value)
-
-        if len(value) != 36:
-            return False
-
-        pattern = '^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$'
-        return re.search(pattern, value) is not None
-
-    def _is_email(self, value: str) -> bool:
-        """
-        Validate a email in string
-        """
-        value = str(value)
-
-        pattern = '^[^@\n]+@[^@\n]+(\.[^@\n]+)+$'
-        return re.search(pattern, value) is not None
+import re
+import uuid
+
+from nsj_rest_lib.descriptor.dto_field import DTOField
+
+
+class DTOFieldValidators:
+
+    def validate_cpf_or_cnpj(self, dto_field: DTOField, value):
+        """
+        Valida se é um CPF ou CNPJ.
+        """
+
+        if value is None:
+            return None
+
+        if not isinstance(value, str):
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
+
+        value = self._remove_not_number_chars(value)
+
+        if self._is_cpf_or_cnpj(value):
+            return value
+        else:
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser um CPF ou CNPJ. Valor recebido: {value}.")
+
+    def validate_cpf(self, dto_field: DTOField, value):
+        """
+        Valida se é um CPF.
+        """
+
+        if value is None:
+            return None
+
+        if not isinstance(value, str):
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
+
+        value = self._remove_not_number_chars(value)
+
+        if self._is_cpf(value):
+            return value
+        else:
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser um CPF. Valor recebido: {value}.")
+
+    def validate_cnpj(self, dto_field: DTOField, value):
+        """
+        Valida se é um CNPJ.
+        """
+
+        if value is None:
+            return None
+
+        if not isinstance(value, str):
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
+
+        value = self._remove_not_number_chars(value)
+
+        if self._is_cnpj(value):
+            return value
+        else:
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser um CNPJ. Valor recebido: {value}.")
+
+    def validate_uuid(self, dto_field: DTOField, value):
+        """
+        Valida se é um UUID.
+        """
+
+        if value is None:
+            return None
+
+        if isinstance(value, uuid.UUID):
+            return value
+
+        if not isinstance(value, str):
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser um UUID ou string correspondente. Valor recebido: {value}.")
+
+        value = value.strip()
+
+        if self._is_uuid(value):
+            return uuid.UUID(value)
+        else:
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser um UUID. Valor recebido: {value}.")
+
+    def validate_email(self, dto_field: DTOField, value):
+        """
+        Valida se é um UUID.
+        """
+
+        if value is None:
+            return None
+
+        if not isinstance(value, str):
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser do tipo string. Valor recebido: {value}.")
+
+        value = value.strip()
+
+        if self._is_email(value):
+            return value
+        else:
+            raise ValueError(
+                f"{dto_field.storage_name} deve ser um e-mail válido. Valor recebido: {value}.")
+
+    ######################
+    # Métodos Auxiliares #
+    ######################
+
+    def _remove_not_number_chars(self, value):
+        return re.sub("[^0-9]", '', value)
+
+    def _is_cpf(self, cpf: str) -> bool:
+        """ If cpf in the Brazilian format is valid, it returns True, otherwise, it returns False. """
+
+        # Check if type is str
+        if not isinstance(cpf, str):
+            return False
+
+        # Removing not number chars:
+        cpf = self._remove_not_number_chars(cpf)
+
+        # Verify if CPF number is equal
+        if cpf in ['12345678909', '00000000000', '11111111111', '22222222222', '33333333333', '44444444444', '55555555555', '66666666666', '77777777777', '88888888888', '99999999999']:
+            return False
+
+        # Checks if string has 11 characters
+        if len(cpf) != 11:
+            return False
+
+        sum = 0
+        weight = 10
+
+        """ Calculating the first cpf check digit. """
+        for n in range(9):
+            sum = sum + int(cpf[n]) * weight
+
+            # Decrement weight
+            weight = weight - 1
+
+        verifyingDigit = 11 - sum % 11
+
+        if verifyingDigit > 9:
+            firstVerifyingDigit = 0
+        else:
+            firstVerifyingDigit = verifyingDigit
+
+        """ Calculating the second check digit of cpf. """
+        sum = 0
+        weight = 11
+        for n in range(10):
+            sum = sum + int(cpf[n]) * weight
+
+            # Decrement weight
+            weight = weight - 1
+
+        verifyingDigit = 11 - sum % 11
+
+        if verifyingDigit > 9:
+            secondVerifyingDigit = 0
+        else:
+            secondVerifyingDigit = verifyingDigit
+
+        if cpf[-2:] == "%s%s" % (firstVerifyingDigit, secondVerifyingDigit):
+            return True
+        return False
+
+    def _is_cnpj(self, cnpj: str) -> bool:
+        """ 
+        Method to validate brazilian cnpjs
+        """
+
+        # defining some variables
+        lista_validacao_um = [5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
+        lista_validacao_dois = [6, 5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
+
+        # Removing not number chars:
+        cnpj = self._remove_not_number_chars(cnpj)
+
+        # finding out the digits
+        verificadores = cnpj[-2:]
+
+        # verifying the lenght of the cnpj
+        if len(cnpj) != 14:
+            return False
+
+        # calculating the first digit
+        soma = 0
+        id = 0
+        for numero in cnpj:
+
+            # to do not raise indexerrors
+            try:
+                lista_validacao_um[id]
+            except:
+                break
+
+            soma += int(numero) * int(lista_validacao_um[id])
+            id += 1
+
+        soma = soma % 11
+        if soma < 2:
+            digito_um = 0
+        else:
+            digito_um = 11 - soma
+
+        # converting to string, for later comparison
+        digito_um = str(digito_um)
+
+        # calculating the second digit
+        # suming the two lists
+        soma = 0
+        id = 0
+
+        # suming the two lists
+        for numero in cnpj:
+
+            # to do not raise indexerrors
+            try:
+                lista_validacao_dois[id]
+            except:
+                break
+
+            soma += int(numero) * int(lista_validacao_dois[id])
+            id += 1
+
+        # defining the digit
+        soma = soma % 11
+        if soma < 2:
+            digito_dois = 0
+        else:
+            digito_dois = 11 - soma
+
+        digito_dois = str(digito_dois)
+
+        # returnig
+        return bool(verificadores == digito_um + digito_dois)
+
+    def _is_cpf_or_cnpj(self, cpf_cnpj: str) -> bool:
+        """
+        Validate a brazilian CPF ou CNPJ.
+        """
+
+        # Removing not number chars:
+        cpf_cnpj = self._remove_not_number_chars(cpf_cnpj)
+
+        if len(cpf_cnpj) == 11:
+            return self._is_cpf(cpf_cnpj)
+        elif len(cpf_cnpj) == 14:
+            return self._is_cnpj(cpf_cnpj)
+        else:
+            return False
+
+    def _is_uuid(self, value: str) -> bool:
+        """
+        Validate a UUID or UUID in string
+        """
+        value = str(value)
+
+        if len(value) != 36:
+            return False
+
+        pattern = '^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$'
+        return re.search(pattern, value) is not None
+
+    def _is_email(self, value: str) -> bool:
+        """
+        Validate a email in string
+        """
+        value = str(value)
+
+        pattern = '^[^@\n]+@[^@\n]+(\.[^@\n]+)+$'
+        return re.search(pattern, value) is not None
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import enum
-import typing
-
-from decimal import Decimal
-
-from nsj_rest_lib.dto.dto_base import DTOBase
-from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.exception import DTOListFieldConfigException
-
-
-class DTOListField:
-    _ref_counter = 0
-
-    def __init__(
-        self,
-        dto_type: DTOBase,
-        entity_type: EntityBase,
-        related_entity_field: str,
-        not_null: bool = False,
-        min: int = None,
-        max: int = None,
-        validator: typing.Callable = None,
-        dto_post_response_type: DTOBase = None
-    ):
-        """
-        -----------
-        Parameters:
-        -----------
-        dto_type: Expected type for the related DTO (must be subclasse from DTOBase).
-        entity_type: Expected entity type for the related DTO (must be subclasse from EntityBase).
-        not_null: The field cannot be None (or an empty list).
-        min: Minimum number of itens in the list.
-        max: Maximum number of itens in the list.
-        validator: Function that receives the value (to be setted), and returns the same value (after any adjust).
-          This function overrides the default behaviour and all default constraints.
-        related_entity_field: Fields, from related entity, used for relation in database.
-        """
-        self.dto_type = dto_type
-        self.entity_type = entity_type
-        self.related_entity_field = related_entity_field
-        self.not_null = not_null
-        self.min = min
-        self.max = max
-        self.validator = validator
-        self.dto_post_response_type = dto_post_response_type
-
-        self.storage_name = f"_{self.__class__.__name__}#{self.__class__._ref_counter}"
-        self.__class__._ref_counter += 1
-
-        # Checking correct usage
-        if self.dto_type is None:
-            raise DTOListFieldConfigException(
-                'type parameter must be not None.')
-
-        if self.entity_type is None:
-            raise DTOListFieldConfigException(
-                'entity_type parameter must be not None.')
-
-    def __get__(self, instance, owner):
-        if instance is None:
-            return self
-        else:
-            return instance.__dict__[self.storage_name]
-
-    def __set__(self, instance, value):
-        if self.validator is None:
-            value = self.validate(value)
-        else:
-            value = self.validator(value)
-
-        # Preenchendo os campos de particionanmento, se necessário (normalmente: tenant e grupo_empresarial)
-        self.set_partition_fields(instance, value)
-
-        instance.__dict__[self.storage_name] = value
-
-    def set_partition_fields(self, instance, value):
-        """
-        Preenchendo os campos de particionanmento dos objetos da lista, se necessário (normalmente: tenant e grupo_empresarial).
-        """
-
-        if hasattr(instance.__class__, 'partition_fields') and value is not None:
-            for item in value:
-                for partition_field in instance.__class__.partition_fields:
-                    if (
-                        hasattr(instance, partition_field)
-                        and hasattr(item, partition_field)
-                        # TODO Analisar se devo descomentar a comparação abaixo que deixa gravar com campos de partição
-                        # diferentes entre classe mestre e detalhe (caso se especifique diferente no detalhe)
-                        # Talvez falte aqui a comparação de tipo de relacionamento como composição (quando não é composição
-                        # a diferença pode fazer sentido)
-                        # and getattr(item, partition_field) is None
-                        and getattr(instance, partition_field) != getattr(item, partition_field)
-                    ):
-                        partition_value = getattr(instance, partition_field)
-                        setattr(item, partition_field, partition_value)
-
-    def validate(self, value):
-        """
-        Default validator (ckecking default constraints: not null, type, min and max).
-        """
-
-        # Checking not null constraint
-        if (self.not_null) and (value is None or (isinstance(value, list) and len(value) <= 0)):
-            raise ValueError(
-                f"O campo {self.storage_name} deve ser preechido. Valor recebido: {value}.")
-
-        # Checking if received value is a list
-        if value is not None and not isinstance(value, list):
-            raise ValueError(
-                f"O valor recebido para o campo {self.storage_name} deveria ser uma lista. Valor recebido: {value}.")
-
-        # Checking type constraint
-        # TODO Ver como suportar typing
-        if self.dto_type is not None and value is not None and len(value) > 0 and not isinstance(value[0], self.dto_type):
-            raise ValueError(
-                f"Os items da lista {self.storage_name} deveriam se do tipo {self.dto_type.__name__}. Valor recebido: {value}.")
-
-        # Checking min constraint
-        if self.min is not None and len(value) < self.min:
-            raise ValueError(
-                f"A lista {self.storage_name} deve ter mais do que {self.min} itens. Valor recebido: {value}.")
-
-        # Checking min constraint
-        if self.max is not None and len(value) > self.max:
-            raise ValueError(
-                f"A lista {self.storage_name} deve ter menos do que {self.max} itens. Valor recebido: {value}.")
-
-        return value
+import enum
+import typing
+
+from decimal import Decimal
+
+from nsj_rest_lib.dto.dto_base import DTOBase
+from nsj_rest_lib.entity.entity_base import EntityBase
+from nsj_rest_lib.exception import DTOListFieldConfigException
+
+
+class DTOListField:
+    _ref_counter = 0
+
+    def __init__(
+        self,
+        dto_type: DTOBase,
+        entity_type: EntityBase,
+        related_entity_field: str,
+        not_null: bool = False,
+        min: int = None,
+        max: int = None,
+        validator: typing.Callable = None,
+        dto_post_response_type: DTOBase = None
+    ):
+        """
+        -----------
+        Parameters:
+        -----------
+        dto_type: Expected type for the related DTO (must be subclasse from DTOBase).
+        entity_type: Expected entity type for the related DTO (must be subclasse from EntityBase).
+        not_null: The field cannot be None (or an empty list).
+        min: Minimum number of itens in the list.
+        max: Maximum number of itens in the list.
+        validator: Function that receives the value (to be setted), and returns the same value (after any adjust).
+          This function overrides the default behaviour and all default constraints.
+        related_entity_field: Fields, from related entity, used for relation in database.
+        """
+        self.dto_type = dto_type
+        self.entity_type = entity_type
+        self.related_entity_field = related_entity_field
+        self.not_null = not_null
+        self.min = min
+        self.max = max
+        self.validator = validator
+        self.dto_post_response_type = dto_post_response_type
+
+        self.storage_name = f"_{self.__class__.__name__}#{self.__class__._ref_counter}"
+        self.__class__._ref_counter += 1
+
+        # Checking correct usage
+        if self.dto_type is None:
+            raise DTOListFieldConfigException(
+                'type parameter must be not None.')
+
+        if self.entity_type is None:
+            raise DTOListFieldConfigException(
+                'entity_type parameter must be not None.')
+
+    def __get__(self, instance, owner):
+        if instance is None:
+            return self
+        else:
+            return instance.__dict__[self.storage_name]
+
+    def __set__(self, instance, value):
+        if self.validator is None:
+            value = self.validate(value)
+        else:
+            value = self.validator(value)
+
+        # Preenchendo os campos de particionanmento, se necessário (normalmente: tenant e grupo_empresarial)
+        self.set_partition_fields(instance, value)
+
+        instance.__dict__[self.storage_name] = value
+
+    def set_partition_fields(self, instance, value):
+        """
+        Preenchendo os campos de particionanmento dos objetos da lista, se necessário (normalmente: tenant e grupo_empresarial).
+        """
+
+        if hasattr(instance.__class__, 'partition_fields') and value is not None:
+            for item in value:
+                for partition_field in instance.__class__.partition_fields:
+                    if (
+                        hasattr(instance, partition_field)
+                        and hasattr(item, partition_field)
+                        # TODO Analisar se devo descomentar a comparação abaixo que deixa gravar com campos de partição
+                        # diferentes entre classe mestre e detalhe (caso se especifique diferente no detalhe)
+                        # Talvez falte aqui a comparação de tipo de relacionamento como composição (quando não é composição
+                        # a diferença pode fazer sentido)
+                        # and getattr(item, partition_field) is None
+                        and getattr(instance, partition_field) != getattr(item, partition_field)
+                    ):
+                        partition_value = getattr(instance, partition_field)
+                        setattr(item, partition_field, partition_value)
+
+    def validate(self, value):
+        """
+        Default validator (ckecking default constraints: not null, type, min and max).
+        """
+
+        # Checking not null constraint
+        if (self.not_null) and (value is None or (isinstance(value, list) and len(value) <= 0)):
+            raise ValueError(
+                f"O campo {self.storage_name} deve ser preechido. Valor recebido: {value}.")
+
+        # Checking if received value is a list
+        if value is not None and not isinstance(value, list):
+            raise ValueError(
+                f"O valor recebido para o campo {self.storage_name} deveria ser uma lista. Valor recebido: {value}.")
+
+        # Checking type constraint
+        # TODO Ver como suportar typing
+        if self.dto_type is not None and value is not None and len(value) > 0 and not isinstance(value[0], self.dto_type):
+            raise ValueError(
+                f"Os items da lista {self.storage_name} deveriam se do tipo {self.dto_type.__name__}. Valor recebido: {value}.")
+
+        # Checking min constraint
+        if self.min is not None and len(value) < self.min:
+            raise ValueError(
+                f"A lista {self.storage_name} deve ter mais do que {self.min} itens. Valor recebido: {value}.")
+
+        # Checking min constraint
+        if self.max is not None and len(value) > self.max:
+            raise ValueError(
+                f"A lista {self.storage_name} deve ter menos do que {self.max} itens. Valor recebido: {value}.")
+
+        return value
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/dto_base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-import abc
-import copy
-# import uuid
-
-from typing import Any, Dict, List, Set, Union
-
-from nsj_rest_lib.entity.entity_base import EMPTY, EntityBase
-from nsj_rest_lib.descriptor.dto_field import DTOField, DTOFieldFilter
-
-
-class DTOBase(abc.ABC):
-    resume_fields: Set[str] = set()
-    partition_fields: Set[str] = set()
-    fields_map: Dict[str, DTOField] = {}
-    list_fields_map: dict = {}
-    field_filters_map: Dict[str, DTOFieldFilter]
-    # TODO Refatorar para suportar PK composto
-    pk_field: str
-    fixed_filters: Dict[str, Any]
-
-    def __init__(self, entity: Union[EntityBase, dict] = None, **kwargs) -> None:
-        super().__init__()
-
-        # Transformando a entity em dict (se houver uma entity)
-        if entity is not None:
-            kwargs =  copy.deepcopy(entity) if type(entity) is dict else copy.deepcopy(entity.__dict__)
-
-        # Setando os campos registrados como fields simples
-        for field in self.__class__.fields_map:
-            # Recuperando a configuração do campo
-            dto_field = self.__class__.fields_map[field]
-
-            # Tratando do valor default
-            if dto_field.default_value is not None and kwargs.get(field, None) is None:
-                default_value = dto_field.default_value
-                if callable(dto_field.default_value):
-                    default_value = dto_field.default_value()
-                kwargs[field] = default_value
-
-            # Verificando se é preciso converter o nome do field para o nome correspondente no Entity
-            entity_field = field
-            if entity is not None:
-                if dto_field.entity_field is not None:
-                    entity_field = dto_field.entity_field
-
-            if entity_field in kwargs:
-                setattr(self, field, kwargs[entity_field])
-            else:
-                setattr(self, field, None)
-
-        # Setando os campos registrados como fields de lista
-        if entity is None:
-            for field in self.__class__.list_fields_map:
-                dto_list_field = self.__class__.list_fields_map[field]
-
-                if field in kwargs:
-                    if not isinstance(kwargs[field], list):
-                        raise ValueError(
-                            f"O campo {field} deveria ser uma lista do tipo {dto_list_field.dto_type}.")
-
-                    related_itens = []
-                    for item in kwargs[field]:
-                        # Preenchendo os campos de particionanmento, se necessário (normalmente: tenant e grupo_empresarial)
-                        for partition_field in self.__class__.partition_fields:
-                            if (
-                                (
-                                    not (partition_field in item)
-                                    or item[partition_field] is None
-                                )
-                                and partition_field in dto_list_field.dto_type.partition_fields
-                            ):
-                                partition_value = getattr(
-                                    self, partition_field)
-                                item[partition_field] = partition_value
-
-                        # Criando o DTO relacionado
-                        item_dto = dto_list_field.dto_type(**item)
-
-                        # Adicionando o DTO na lista do relacionamento
-                        related_itens.append(item_dto)
-
-                    setattr(self, field, related_itens)
-                else:
-                    setattr(self, field, None)
-
-        # Tratando do ID automático
-        # if generate_pk_uuid:
-        #     if getattr(self, self.__class__.pk_field) is None:
-        #         setattr(self, self.__class__.pk_field, uuid.uuid4())
-
-    def convert_from_entity(self, obj: EntityBase):
-        """
-        Popula DTO a partir de um objeto de entidade (considerando
-        apenas as propriedades descritas como DTOFields).
-
-        Este método retorna self (a própria referencia ao objeto).
-        """
-
-        for attribute in self.__dict__:
-
-            # Ignoring non DTO fields
-            if not (attribute in self.__class__.fields_map):
-                continue
-
-            # Getting DTO field config
-            dto_field = self.__class__.fields_map[attribute]
-
-            # Checking if exists a different name to equivalent field in entity class
-            attr_name = attribute
-            if dto_field.entity_field is not None:
-                attr_name = dto_field.entity_field
-
-            # Checking if exists the equivalent attribute in entity object (skiping, if not)
-            if not hasattr(obj, attr_name):
-                continue
-
-            # Getting entity attribute
-            entity_attr = getattr(obj, attr_name, None)
-
-            # Setting value localy
-            setattr(self, attribute, entity_attr)
-
-        return self
-
-    def convert_to_entity(self, entity_class: EntityBase, none_as_empty: bool = False):
-        """
-        Cria uma instância da entidade, e a popula com os dados do DTO
-        corrente.
-
-        É importante notar que as equivalências dos nomes dos campos
-        são tratadas neste método.
-        """
-
-        entity = entity_class()
-
-        for field, dto_field in self.__class__.fields_map.items():
-            # Verificando se é preciso realizar uma tradução de nome do campo
-            entity_field = field
-            if dto_field.entity_field is not None:
-                entity_field = dto_field.entity_field
-
-            # Verificando se o campo existe na entity
-            if not hasattr(entity, entity_field):
-                continue
-
-            # Recuperando o valor
-            value = getattr(self, field)
-
-            # Convertendo None para EMPTY (se desejado)
-            if value is None and none_as_empty:
-                value = EMPTY
-
-            # Setando na entidade
-            setattr(entity, entity_field, value)
-
-        return entity
-
-    def convert_to_dict(self, fields: Dict[str, List[str]] = None, just_resume: bool = False):
-        """
-        Converte DTO para dict
-        """
-
-        # Resolving fields to use
-        if fields is None:
-            fields = {'root': self.resume_fields}
-
-        if just_resume:
-            fields = {'root': self.resume_fields}
-        else:
-            fields['root'] = fields['root'].union(self.resume_fields)
-
-        # Making result maps
-        result = {}
-
-        # Converting simple fields
-        for field in self.fields_map:
-            if not field in fields['root']:
-                continue
-
-            result[field] = getattr(self, field)
-
-        # Converting list fields
-        for field in self.list_fields_map:
-            if not field in fields['root']:
-                continue
-
-            # Criando o mapa de fileds para a entidade aninhada
-            internal_fields = None
-            if field in fields:
-                internal_fields = {'root': fields[field]}
-
-            # Recuperando o valor do atributo
-            value = getattr(self, field)
-            if value is None:
-                value = []
-
-            # Convetendo a lista de DTOs aninhados
-            result[field] = [item.convert_to_dict(
-                internal_fields, just_resume) for item in value]
-
-        return result
+import abc
+import copy
+# import uuid
+
+from typing import Any, Dict, List, Set, Union
+
+from nsj_rest_lib.entity.entity_base import EMPTY, EntityBase
+from nsj_rest_lib.descriptor.dto_field import DTOField, DTOFieldFilter
+
+
+class DTOBase(abc.ABC):
+    resume_fields: Set[str] = set()
+    partition_fields: Set[str] = set()
+    fields_map: Dict[str, DTOField] = {}
+    list_fields_map: dict = {}
+    field_filters_map: Dict[str, DTOFieldFilter]
+    # TODO Refatorar para suportar PK composto
+    pk_field: str
+    fixed_filters: Dict[str, Any]
+
+    def __init__(self, entity: Union[EntityBase, dict] = None, **kwargs) -> None:
+        super().__init__()
+
+        # Transformando a entity em dict (se houver uma entity)
+        if entity is not None:
+            kwargs =  copy.deepcopy(entity) if type(entity) is dict else copy.deepcopy(entity.__dict__)
+
+        # Setando os campos registrados como fields simples
+        for field in self.__class__.fields_map:
+            # Recuperando a configuração do campo
+            dto_field = self.__class__.fields_map[field]
+
+            # Tratando do valor default
+            if dto_field.default_value is not None and kwargs.get(field, None) is None:
+                default_value = dto_field.default_value
+                if callable(dto_field.default_value):
+                    default_value = dto_field.default_value()
+                kwargs[field] = default_value
+
+            # Verificando se é preciso converter o nome do field para o nome correspondente no Entity
+            entity_field = field
+            if entity is not None:
+                if dto_field.entity_field is not None:
+                    entity_field = dto_field.entity_field
+
+            if entity_field in kwargs:
+                setattr(self, field, kwargs[entity_field])
+            else:
+                setattr(self, field, None)
+
+        # Setando os campos registrados como fields de lista
+        if entity is None:
+            for field in self.__class__.list_fields_map:
+                dto_list_field = self.__class__.list_fields_map[field]
+
+                if field in kwargs:
+                    if not isinstance(kwargs[field], list):
+                        raise ValueError(
+                            f"O campo {field} deveria ser uma lista do tipo {dto_list_field.dto_type}.")
+
+                    related_itens = []
+                    for item in kwargs[field]:
+                        # Preenchendo os campos de particionanmento, se necessário (normalmente: tenant e grupo_empresarial)
+                        for partition_field in self.__class__.partition_fields:
+                            if (
+                                (
+                                    not (partition_field in item)
+                                    or item[partition_field] is None
+                                )
+                                and partition_field in dto_list_field.dto_type.partition_fields
+                            ):
+                                partition_value = getattr(
+                                    self, partition_field)
+                                item[partition_field] = partition_value
+
+                        # Criando o DTO relacionado
+                        item_dto = dto_list_field.dto_type(**item)
+
+                        # Adicionando o DTO na lista do relacionamento
+                        related_itens.append(item_dto)
+
+                    setattr(self, field, related_itens)
+                else:
+                    setattr(self, field, None)
+
+        # Tratando do ID automático
+        # if generate_pk_uuid:
+        #     if getattr(self, self.__class__.pk_field) is None:
+        #         setattr(self, self.__class__.pk_field, uuid.uuid4())
+
+    def convert_from_entity(self, obj: EntityBase):
+        """
+        Popula DTO a partir de um objeto de entidade (considerando
+        apenas as propriedades descritas como DTOFields).
+
+        Este método retorna self (a própria referencia ao objeto).
+        """
+
+        for attribute in self.__dict__:
+
+            # Ignoring non DTO fields
+            if not (attribute in self.__class__.fields_map):
+                continue
+
+            # Getting DTO field config
+            dto_field = self.__class__.fields_map[attribute]
+
+            # Checking if exists a different name to equivalent field in entity class
+            attr_name = attribute
+            if dto_field.entity_field is not None:
+                attr_name = dto_field.entity_field
+
+            # Checking if exists the equivalent attribute in entity object (skiping, if not)
+            if not hasattr(obj, attr_name):
+                continue
+
+            # Getting entity attribute
+            entity_attr = getattr(obj, attr_name, None)
+
+            # Setting value localy
+            setattr(self, attribute, entity_attr)
+
+        return self
+
+    def convert_to_entity(self, entity_class: EntityBase, none_as_empty: bool = False):
+        """
+        Cria uma instância da entidade, e a popula com os dados do DTO
+        corrente.
+
+        É importante notar que as equivalências dos nomes dos campos
+        são tratadas neste método.
+        """
+
+        entity = entity_class()
+
+        for field, dto_field in self.__class__.fields_map.items():
+            # Verificando se é preciso realizar uma tradução de nome do campo
+            entity_field = field
+            if dto_field.entity_field is not None:
+                entity_field = dto_field.entity_field
+
+            # Verificando se o campo existe na entity
+            if not hasattr(entity, entity_field):
+                continue
+
+            # Recuperando o valor
+            value = getattr(self, field)
+
+            # Convertendo None para EMPTY (se desejado)
+            if value is None and none_as_empty:
+                value = EMPTY
+
+            # Setando na entidade
+            setattr(entity, entity_field, value)
+
+        return entity
+
+    def convert_to_dict(self, fields: Dict[str, List[str]] = None, just_resume: bool = False):
+        """
+        Converte DTO para dict
+        """
+
+        # Resolving fields to use
+        if fields is None:
+            fields = {'root': self.resume_fields}
+
+        if just_resume:
+            fields = {'root': self.resume_fields}
+        else:
+            fields['root'] = fields['root'].union(self.resume_fields)
+
+        # Making result maps
+        result = {}
+
+        # Converting simple fields
+        for field in self.fields_map:
+            if not field in fields['root']:
+                continue
+
+            result[field] = getattr(self, field)
+
+        # Converting list fields
+        for field in self.list_fields_map:
+            if not field in fields['root']:
+                continue
+
+            # Criando o mapa de fileds para a entidade aninhada
+            internal_fields = None
+            if field in fields:
+                internal_fields = {'root': fields[field]}
+
+            # Recuperando o valor do atributo
+            value = getattr(self, field)
+            if value is None:
+                value = []
+
+            # Convetendo a lista de DTOs aninhados
+            result[field] = [item.convert_to_dict(
+                internal_fields, just_resume) for item in value]
+
+        return result
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/healthcheck_config.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import os
-import base64
-import requests
-
-from healthcheck import HealthCheck
-
-from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
-
-
-class HealthCheckConfig:
-    def __init__(
-        self,
-        flask_application,
-        injector_factory_class: NsjInjectorFactoryBase = None,
-        app_name: str = None,
-        rabbitmq_host: str = None,
-        rabbitmq_http_port: int = None,
-        rabbitmq_user: str = None,
-        rabbitmq_pass: str = None,
-    ):
-        self._flask_application = flask_application
-        self._injector_factory_class = injector_factory_class or NsjInjectorFactoryBase
-        self._app_name = app_name or os.getenv('APP_NAME')
-        self._rabbitmq_host = rabbitmq_host or os.getenv('RABBITMQ_HOST')
-        self._rabbitmq_http_port = rabbitmq_http_port or int(
-            os.getenv('RABBITMQ_HTTP_PORT', 15672))
-        self._rabbitmq_user = rabbitmq_user or os.getenv(
-            'RABBITMQ_USER', 'guest')
-        self._rabbitmq_pass = rabbitmq_pass or os.getenv(
-            'RABBITMQ_PASS', 'guest')
-
-    def check_database(self):
-        with self._injector_factory_class() as factory:
-            sql = "SELECT 1"
-
-            factory.db_adapter().execute_query(sql)
-
-            return True, "Banco de dados OK"
-
-    def check_rabbit_mq(self):
-        rabbit_url = f"{self._rabbitmq_host}:{self._rabbitmq_http_port}/api/healthchecks/node"
-        if rabbit_url[0:4] != 'http':
-            rabbit_url = 'http://' + rabbit_url
-
-        credentials = f"{self._rabbitmq_user}:{self._rabbitmq_pass}"
-        credentials = credentials.encode('utf8')
-        credentials = base64.b64encode(credentials)
-        credentials = credentials.decode('utf8')
-
-        headers = {
-            "Authorization": f"Basic {credentials}"
-        }
-
-        response = requests.get(rabbit_url, headers=headers)
-
-        if response.status_code == 200:
-            return True, "RabbitMQ OK"
-        else:
-            return False, f"Falha de comunicação com o RabbitMQ"
-
-    def config(
-        self,
-        check_database: bool = True,
-        check_rabbit_mq: bool = False
-    ):
-
-        health = HealthCheck()
-
-        # Adicionando a validação de banco de dados
-        if check_database:
-            health.add_check(self.check_database)
-
-        # Adicionando a validação do RabbitMQ
-        if check_rabbit_mq:
-            health.add_check(self.check_rabbit_mq)
-
-        # Registrando a rota do HealthCheck
-        if self._app_name is not None:
-            self._flask_application.add_url_rule(f"/{self._app_name}/healthcheck", "healthcheck",
-                                                 view_func=lambda: health.run())
-        else:
-            self._flask_application.add_url_rule(f"/healthcheck", "healthcheck",
-                                                 view_func=lambda: health.run())
+import os
+import base64
+import requests
+
+from healthcheck import HealthCheck
+
+from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+
+
+class HealthCheckConfig:
+    def __init__(
+        self,
+        flask_application,
+        injector_factory_class: NsjInjectorFactoryBase = None,
+        app_name: str = None,
+        rabbitmq_host: str = None,
+        rabbitmq_http_port: int = None,
+        rabbitmq_user: str = None,
+        rabbitmq_pass: str = None,
+    ):
+        self._flask_application = flask_application
+        self._injector_factory_class = injector_factory_class or NsjInjectorFactoryBase
+        self._app_name = app_name or os.getenv('APP_NAME')
+        self._rabbitmq_host = rabbitmq_host or os.getenv('RABBITMQ_HOST')
+        self._rabbitmq_http_port = rabbitmq_http_port or int(
+            os.getenv('RABBITMQ_HTTP_PORT', 15672))
+        self._rabbitmq_user = rabbitmq_user or os.getenv(
+            'RABBITMQ_USER', 'guest')
+        self._rabbitmq_pass = rabbitmq_pass or os.getenv(
+            'RABBITMQ_PASS', 'guest')
+
+    def check_database(self):
+        with self._injector_factory_class() as factory:
+            sql = "SELECT 1"
+
+            factory.db_adapter().execute_query(sql)
+
+            return True, "Banco de dados OK"
+
+    def check_rabbit_mq(self):
+        rabbit_url = f"{self._rabbitmq_host}:{self._rabbitmq_http_port}/api/healthchecks/node"
+        if rabbit_url[0:4] != 'http':
+            rabbit_url = 'http://' + rabbit_url
+
+        credentials = f"{self._rabbitmq_user}:{self._rabbitmq_pass}"
+        credentials = credentials.encode('utf8')
+        credentials = base64.b64encode(credentials)
+        credentials = credentials.decode('utf8')
+
+        headers = {
+            "Authorization": f"Basic {credentials}"
+        }
+
+        response = requests.get(rabbit_url, headers=headers)
+
+        if response.status_code == 200:
+            return True, "RabbitMQ OK"
+        else:
+            return False, f"Falha de comunicação com o RabbitMQ"
+
+    def config(
+        self,
+        check_database: bool = True,
+        check_rabbit_mq: bool = False
+    ):
+
+        health = HealthCheck()
+
+        # Adicionando a validação de banco de dados
+        if check_database:
+            health.add_check(self.check_database)
+
+        # Adicionando a validação do RabbitMQ
+        if check_rabbit_mq:
+            health.add_check(self.check_rabbit_mq)
+
+        # Registrando a rota do HealthCheck
+        if self._app_name is not None:
+            self._flask_application.add_url_rule(f"/{self._app_name}/healthcheck", "healthcheck",
+                                                 view_func=lambda: health.run())
+        else:
+            self._flask_application.add_url_rule(f"/healthcheck", "healthcheck",
+                                                 view_func=lambda: health.run())
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/injector_factory_base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from sqlalchemy.engine.base import Connection
-
-db_pool = None
-
-
-class NsjInjectorFactoryBase:
-    _db_connection: Connection
-
-    def __enter__(self):
-        from nsj_rest_lib.db_pool_config import db_pool as internal_db_pool
-
-        pool = internal_db_pool
-        if db_pool is not None:
-            pool = db_pool
-
-        self._db_connection = pool.connect()
-
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self._db_connection.close()
-
-    def db_adapter(self):
-        from nsj_gcf_utils.db_adapter2 import DBAdapter2
-        return DBAdapter2(self._db_connection)
-
-    def get_service_by_name(self, name: str):
-        if not hasattr(self, name):
-            raise Exception(f'Service not found: {name}')
-
-        service_method = getattr(self, name)
-
-        return service_method()
+from sqlalchemy.engine.base import Connection
+
+db_pool = None
+
+
+class NsjInjectorFactoryBase:
+    _db_connection: Connection
+
+    def __enter__(self):
+        from nsj_rest_lib.db_pool_config import db_pool as internal_db_pool
+
+        pool = internal_db_pool
+        if db_pool is not None:
+            pool = db_pool
+
+        self._db_connection = pool.connect()
+
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._db_connection.close()
+
+    def db_adapter(self):
+        from nsj_gcf_utils.db_adapter2 import DBAdapter2
+        return DBAdapter2(self._db_connection)
+
+    def get_service_by_name(self, name: str):
+        if not hasattr(self, name):
+            raise Exception(f'Service not found: {name}')
+
+        service_method = getattr(self, name)
+
+        return service_method()
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import re
-
-
-def validate_cpf(cpf: str) -> bool:
-    """ If cpf in the Brazilian format is valid, it returns True, otherwise, it returns False. """
-
-    # Check if type is str
-    if not isinstance(cpf, str):
-        return False
-
-    # Remove some unwanted characters
-    cpf = re.sub("[^0-9]", '', cpf)
-
-    # Verify if CPF number is equal
-    if cpf in ['12345678909', '00000000000', '11111111111', '22222222222', '33333333333', '44444444444', '55555555555', '66666666666', '77777777777', '88888888888', '99999999999']:
-        return False
-
-    # Checks if string has 11 characters
-    if len(cpf) != 11:
-        return False
-
-    sum = 0
-    weight = 10
-
-    """ Calculating the first cpf check digit. """
-    for n in range(9):
-        sum = sum + int(cpf[n]) * weight
-
-        # Decrement weight
-        weight = weight - 1
-
-    verifyingDigit = 11 - sum % 11
-
-    if verifyingDigit > 9:
-        firstVerifyingDigit = 0
-    else:
-        firstVerifyingDigit = verifyingDigit
-
-    """ Calculating the second check digit of cpf. """
-    sum = 0
-    weight = 11
-    for n in range(10):
-        sum = sum + int(cpf[n]) * weight
-
-        # Decrement weight
-        weight = weight - 1
-
-    verifyingDigit = 11 - sum % 11
-
-    if verifyingDigit > 9:
-        secondVerifyingDigit = 0
-    else:
-        secondVerifyingDigit = verifyingDigit
-
-    if cpf[-2:] == "%s%s" % (firstVerifyingDigit, secondVerifyingDigit):
-        return True
-    return False
-
-
-def validate_cnpj(cnpj: str) -> bool:
-    """ 
-    Method to validate brazilian cnpjs
-    """
-
-    # defining some variables
-    lista_validacao_um = [5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
-    lista_validacao_dois = [6, 5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
-
-    # cleaning the cnpj
-    cnpj = cnpj.replace("-", "")
-    cnpj = cnpj.replace(".", "")
-    cnpj = cnpj.replace("/", "")
-
-    # finding out the digits
-    verificadores = cnpj[-2:]
-
-    # verifying the lenght of the cnpj
-    if len(cnpj) != 14:
-        return False
-
-    # calculating the first digit
-    soma = 0
-    id = 0
-    for numero in cnpj:
-
-        # to do not raise indexerrors
-        try:
-            lista_validacao_um[id]
-        except:
-            break
-
-        soma += int(numero) * int(lista_validacao_um[id])
-        id += 1
-
-    soma = soma % 11
-    if soma < 2:
-        digito_um = 0
-    else:
-        digito_um = 11 - soma
-
-    # converting to string, for later comparison
-    digito_um = str(digito_um)
-
-    # calculating the second digit
-    # suming the two lists
-    soma = 0
-    id = 0
-
-    # suming the two lists
-    for numero in cnpj:
-
-        # to do not raise indexerrors
-        try:
-            lista_validacao_dois[id]
-        except:
-            break
-
-        soma += int(numero) * int(lista_validacao_dois[id])
-        id += 1
-
-    # defining the digit
-    soma = soma % 11
-    if soma < 2:
-        digito_dois = 0
-    else:
-        digito_dois = 11 - soma
-
-    digito_dois = str(digito_dois)
-
-    # returnig
-    return bool(verificadores == digito_um + digito_dois)
-
-
-def validate_cpf_cnpj(cpf_cnpj: str) -> bool:
-    """
-    Validate a brazilian CPF ou CNPJ.
-    """
-
-    if len(cpf_cnpj) == 11:
-        return validate_cpf(cpf_cnpj)
-    elif len(cpf_cnpj) == 14:
-        return validate_cnpj(cpf_cnpj)
-    else:
-        return False
-
-
-def add_mascara_cpf_cnpj(doc: str) -> str:
-    """
-    Valida o tamanho do CPF/CNPJ, e retorna já com máscara.
-    """
-
-    if doc is None:
-        return None
-
-    if len(doc) == 11:
-        return '{}.{}.{}-{}'.format(doc[0:3], doc[3:6], doc[6:9], doc[9:11])
-    elif len(doc) == 14:
-        return '{}.{}.{}/{}-{}'.format(doc[0:2], doc[2:5], doc[5:8], doc[8:12], doc[12:14])
-    else:
-        raise Exception(
-            'Invalid CPF/CNPJ length ({}): {}'.format(len(doc), doc))
-
-
-def remove_mascara_cpf_cnpj(doc: str) -> str:
-    """
-    Remove a máscara de um CPF/CNPJ e retorna.
-
-    Lança erro, se o resultado não tiver um tamanho correto de string.
-    """
-
-    if doc is None:
-        return None
-
-    doc = doc.replace('.', '').replace('/', '').replace('-', '')
-
-    if len(doc) != 11 and len(doc) != 14:
-        raise Exception(
-            'Invalid CPF/CNPJ: {}'.format(doc))
-
-    return doc
+import re
+
+
+def validate_cpf(cpf: str) -> bool:
+    """ If cpf in the Brazilian format is valid, it returns True, otherwise, it returns False. """
+
+    # Check if type is str
+    if not isinstance(cpf, str):
+        return False
+
+    # Remove some unwanted characters
+    cpf = re.sub("[^0-9]", '', cpf)
+
+    # Verify if CPF number is equal
+    if cpf in ['12345678909', '00000000000', '11111111111', '22222222222', '33333333333', '44444444444', '55555555555', '66666666666', '77777777777', '88888888888', '99999999999']:
+        return False
+
+    # Checks if string has 11 characters
+    if len(cpf) != 11:
+        return False
+
+    sum = 0
+    weight = 10
+
+    """ Calculating the first cpf check digit. """
+    for n in range(9):
+        sum = sum + int(cpf[n]) * weight
+
+        # Decrement weight
+        weight = weight - 1
+
+    verifyingDigit = 11 - sum % 11
+
+    if verifyingDigit > 9:
+        firstVerifyingDigit = 0
+    else:
+        firstVerifyingDigit = verifyingDigit
+
+    """ Calculating the second check digit of cpf. """
+    sum = 0
+    weight = 11
+    for n in range(10):
+        sum = sum + int(cpf[n]) * weight
+
+        # Decrement weight
+        weight = weight - 1
+
+    verifyingDigit = 11 - sum % 11
+
+    if verifyingDigit > 9:
+        secondVerifyingDigit = 0
+    else:
+        secondVerifyingDigit = verifyingDigit
+
+    if cpf[-2:] == "%s%s" % (firstVerifyingDigit, secondVerifyingDigit):
+        return True
+    return False
+
+
+def validate_cnpj(cnpj: str) -> bool:
+    """ 
+    Method to validate brazilian cnpjs
+    """
+
+    # defining some variables
+    lista_validacao_um = [5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
+    lista_validacao_dois = [6, 5, 4, 3, 2, 9, 8, 7, 6, 5, 4, 3, 2]
+
+    # cleaning the cnpj
+    cnpj = cnpj.replace("-", "")
+    cnpj = cnpj.replace(".", "")
+    cnpj = cnpj.replace("/", "")
+
+    # finding out the digits
+    verificadores = cnpj[-2:]
+
+    # verifying the lenght of the cnpj
+    if len(cnpj) != 14:
+        return False
+
+    # calculating the first digit
+    soma = 0
+    id = 0
+    for numero in cnpj:
+
+        # to do not raise indexerrors
+        try:
+            lista_validacao_um[id]
+        except:
+            break
+
+        soma += int(numero) * int(lista_validacao_um[id])
+        id += 1
+
+    soma = soma % 11
+    if soma < 2:
+        digito_um = 0
+    else:
+        digito_um = 11 - soma
+
+    # converting to string, for later comparison
+    digito_um = str(digito_um)
+
+    # calculating the second digit
+    # suming the two lists
+    soma = 0
+    id = 0
+
+    # suming the two lists
+    for numero in cnpj:
+
+        # to do not raise indexerrors
+        try:
+            lista_validacao_dois[id]
+        except:
+            break
+
+        soma += int(numero) * int(lista_validacao_dois[id])
+        id += 1
+
+    # defining the digit
+    soma = soma % 11
+    if soma < 2:
+        digito_dois = 0
+    else:
+        digito_dois = 11 - soma
+
+    digito_dois = str(digito_dois)
+
+    # returnig
+    return bool(verificadores == digito_um + digito_dois)
+
+
+def validate_cpf_cnpj(cpf_cnpj: str) -> bool:
+    """
+    Validate a brazilian CPF ou CNPJ.
+    """
+
+    if len(cpf_cnpj) == 11:
+        return validate_cpf(cpf_cnpj)
+    elif len(cpf_cnpj) == 14:
+        return validate_cnpj(cpf_cnpj)
+    else:
+        return False
+
+
+def add_mascara_cpf_cnpj(doc: str) -> str:
+    """
+    Valida o tamanho do CPF/CNPJ, e retorna já com máscara.
+    """
+
+    if doc is None:
+        return None
+
+    if len(doc) == 11:
+        return '{}.{}.{}-{}'.format(doc[0:3], doc[3:6], doc[6:9], doc[9:11])
+    elif len(doc) == 14:
+        return '{}.{}.{}/{}-{}'.format(doc[0:2], doc[2:5], doc[5:8], doc[8:12], doc[12:14])
+    else:
+        raise Exception(
+            'Invalid CPF/CNPJ length ({}): {}'.format(len(doc), doc))
+
+
+def remove_mascara_cpf_cnpj(doc: str) -> str:
+    """
+    Remove a máscara de um CPF/CNPJ e retorna.
+
+    Lança erro, se o resultado não tiver um tamanho correto de string.
+    """
+
+    if doc is None:
+        return None
+
+    doc = doc.replace('.', '').replace('/', '').replace('-', '')
+
+    if len(doc) != 11 and len(doc) != 14:
+        raise Exception(
+            'Invalid CPF/CNPJ: {}'.format(doc))
+
+    return doc
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: nsj-rest-lib
-Version: 1.2.0
-Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
-Home-page: https://github.com/Nasajon/nsj_rest_lib
-Author: Nasajon Sistemas
-Author-email: contact.dev@nasajon.com.br
-Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-
-# nsj_rest_lib
-Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
+Metadata-Version: 2.1
+Name: nsj-rest-lib
+Version: 1.2.1
+Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
+Home-page: https://github.com/Nasajon/nsj_rest_lib
+Author: Nasajon Sistemas
+Author-email: contact.dev@nasajon.com.br
+Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+
+# nsj_rest_lib
+Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
```

### Comparing `nsj_rest_lib-1.2.0/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

