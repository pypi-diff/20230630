# Comparing `tmp/fastgenerateapi-0.0.6.tar.gz` & `tmp/fastgenerateapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.6.tar", last modified: Sun Jun 18 06:25:26 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.7.tar", last modified: Tue Jun 20 12:52:40 2023, max compression
```

## Comparing `fastgenerateapi-0.0.6.tar` & `fastgenerateapi-0.0.7.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.237326 fastgenerateapi-0.0.6/
--rw-rw-rw-   0        0        0    35821 2023-06-18 00:11:53.000000 fastgenerateapi-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4389 2023-06-18 06:25:26.236328 fastgenerateapi-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3747 2023-06-18 06:08:20.000000 fastgenerateapi-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.218809 fastgenerateapi-0.0.6/fastgenerateapi/
--rw-rw-rw-   0        0        0     1022 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.6/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-18 06:25:23.000000 fastgenerateapi-0.0.6/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.223796 fastgenerateapi-0.0.6/fastgenerateapi/api_view/
--rw-rw-rw-   0        0        0       14 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/api_view.py
--rw-rw-rw-   0        0        0     9189 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/base_view.py
--rw-rw-rw-   0        0        0     4177 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/create_view.py
--rw-rw-rw-   0        0        0     3628 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/delete_tree_view.py
--rw-rw-rw-   0        0        0     3035 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/delete_view.py
--rw-rw-rw-   0        0        0     7469 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_all_view.py
--rw-rw-rw-   0        0        0     3077 2023-06-18 01:49:07.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_one_view.py
--rw-rw-rw-   0        0        0     9795 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_relation_view.py
--rw-rw-rw-   0        0        0     7275 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.226792 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-06-18 04:59:15.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/base_mixin.py
--rw-rw-rw-   0        0        0     3826 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
--rw-rw-rw-   0        0        0      266 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/get_mixin.py
--rw-rw-rw-   0        0        0     2290 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/response_mixin.py
--rw-rw-rw-   0        0        0      317 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/save_mixin.py
--rw-rw-rw-   0        0        0    13029 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/tool_mixin.py
--rw-rw-rw-   0        0        0     3070 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/switch_view.py
--rw-rw-rw-   0        0        0     3553 2023-06-18 04:41:09.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/update_relation_view.py
--rw-rw-rw-   0        0        0     4006 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/api_view/update_view.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.227789 fastgenerateapi-0.0.6/fastgenerateapi/controller/
--rw-rw-rw-   0        0        0      316 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/controller/__init__.py
--rw-rw-rw-   0        0        0     3391 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/controller/filter_controller.py
--rw-rw-rw-   0        0        0     2385 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/controller/router_controller.py
--rw-rw-rw-   0        0        0     2298 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/controller/rpc_controller.py
--rw-rw-rw-   0        0        0      873 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/controller/search_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.228783 fastgenerateapi-0.0.6/fastgenerateapi/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/data_type/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/data_type/data_type.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.229780 fastgenerateapi-0.0.6/fastgenerateapi/deps/
--rw-rw-rw-   0        0        0      160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/deps/__init__.py
--rw-rw-rw-   0        0        0      813 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/deps/filter_params_deps.py
--rw-rw-rw-   0        0        0     3171 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/deps/paginator_deps.py
--rw-rw-rw-   0        0        0     1264 2023-06-18 01:09:58.000000 fastgenerateapi-0.0.6/fastgenerateapi/deps/tree_params_deps.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.230777 fastgenerateapi-0.0.6/fastgenerateapi/example/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/example/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/example/models.py
--rw-rw-rw-   0        0        0      195 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/example/routers.py
--rw-rw-rw-   0        0        0      400 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.6/fastgenerateapi/example/views.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.231775 fastgenerateapi-0.0.6/fastgenerateapi/pydantic_utils/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/pydantic_utils/__init__.py
--rw-rw-rw-   0        0        0      694 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/pydantic_utils/base_model.py
--rw-rw-rw-   0        0        0     2814 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/pydantic_utils/json_encoders.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.234338 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/
--rw-rw-rw-   0        0        0      472 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/__init__.py
--rw-rw-rw-   0        0        0     4305 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/common_function.py
--rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/create_schema_factory.py
--rw-rw-rw-   0        0        0     1284 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/filter_schema_factory.py
--rw-rw-rw-   0        0        0     3303 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_all_schema_factory.py
--rw-rw-rw-   0        0        0     2194 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_one_schema_factory.py
--rw-rw-rw-   0        0        0     2391 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
--rw-rw-rw-   0        0        0     3187 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
--rw-rw-rw-   0        0        0     1647 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/response_factory.py
--rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/update_schema_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.235335 fastgenerateapi-0.0.6/fastgenerateapi/settings/
--rw-rw-rw-   0        0        0        6 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/settings/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/settings/register_settings.py
--rw-rw-rw-   0        0        0     4064 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.6/fastgenerateapi/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.236328 fastgenerateapi-0.0.6/fastgenerateapi/utils/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/utils/__init__.py
--rw-rw-rw-   0        0        0      121 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/utils/exception.py
--rw-rw-rw-   0        0        0      670 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.6/fastgenerateapi/utils/parse_str.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:25:26.219807 fastgenerateapi-0.0.6/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0     4389 2023-06-18 06:25:26.000000 fastgenerateapi-0.0.6/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2611 2023-06-18 06:25:26.000000 fastgenerateapi-0.0.6/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 06:25:26.000000 fastgenerateapi-0.0.6/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-18 06:25:26.000000 fastgenerateapi-0.0.6/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 06:25:26.237326 fastgenerateapi-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3832 2023-06-18 06:18:28.000000 fastgenerateapi-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.868601 fastgenerateapi-0.0.7/
+-rw-rw-rw-   0        0        0    35821 2023-06-18 00:11:53.000000 fastgenerateapi-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4383 2023-06-20 12:52:40.867604 fastgenerateapi-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3741 2023-06-20 12:51:34.000000 fastgenerateapi-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.841813 fastgenerateapi-0.0.7/fastgenerateapi/
+-rw-rw-rw-   0        0        0     1022 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-20 12:49:43.000000 fastgenerateapi-0.0.7/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.848440 fastgenerateapi-0.0.7/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9399 2023-06-20 12:36:30.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4177 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3628 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_tree_view.py
+-rw-rw-rw-   0        0        0     3035 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7469 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3077 2023-06-18 01:49:07.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_one_view.py
+-rw-rw-rw-   0        0        0     9795 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_relation_view.py
+-rw-rw-rw-   0        0        0     7275 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.851431 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-06-18 04:59:15.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0     3826 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2290 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13529 2023-06-20 12:11:25.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     6899 2023-06-20 12:48:13.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/sql_get_view.py
+-rw-rw-rw-   0        0        0     3070 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     3553 2023-06-18 04:41:09.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_relation_view.py
+-rw-rw-rw-   0        0        0     4006 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.858578 fastgenerateapi-0.0.7/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     3292 2023-06-20 12:22:23.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.859582 fastgenerateapi-0.0.7/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.860572 fastgenerateapi-0.0.7/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/paginator_deps.py
+-rw-rw-rw-   0        0        0     1264 2023-06-18 01:09:58.000000 fastgenerateapi-0.0.7/fastgenerateapi/deps/tree_params_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.862617 fastgenerateapi-0.0.7/fastgenerateapi/example/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/models.py
+-rw-rw-rw-   0        0        0      195 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/routers.py
+-rw-rw-rw-   0        0        0      400 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.7/fastgenerateapi/example/views.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.862617 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      694 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.865609 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     1284 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/filter_schema_factory.py
+-rw-rw-rw-   0        0        0     3303 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     2194 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     2391 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
+-rw-rw-rw-   0        0        0     3187 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
+-rw-rw-rw-   0        0        0     1647 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.866606 fastgenerateapi-0.0.7/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     4064 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.7/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.867604 fastgenerateapi-0.0.7/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.7/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.842800 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0     4383 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2652 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 12:52:40.000000 fastgenerateapi-0.0.7/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:52:40.868601 fastgenerateapi-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-18 06:18:28.000000 fastgenerateapi-0.0.7/setup.py
```

### Comparing `fastgenerateapi-0.0.6/LICENSE` & `fastgenerateapi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/PKG-INFO` & `fastgenerateapi-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -27,23 +27,23 @@
 
 ###### FastGenerateApi 使用说明
 
 
 #### 软件架构说明
 
 ```
-封装了 快速生成API,包括(增,删,改,查,递归删除)
+封装了 快速生成API,包括(增,删,改,查,递归查询,递归删除,关联修改,关联查询)
 封装了 路由接口路径的灵活配置,返回值字段的灵活配置,分页参数的灵活配置,等其他项
 封装了 增,改 对唯一字段的校验,非空字段的校验
 封装了 删 对唯一字段追加时间戳格式修改
 封装了 查 灵活的筛选,以及swagger文档的自动生成
 封装了 通过数据库模型,自动生成schemas,并swagger附带文档
 封装了 类方法的实现,增加了相关的钩子函数
 封装了 通用性接口,例如excel的导入导出,pdf文件生成,模型数据跨表取值
-待封装 RPC的嵌套,API(关联增,关联删,关联改,关联查)
+待封装 RPC的嵌套
 ```
 
 #### 使用教程
 
 1.  简单使用
 2.  增删改查进一步优化使用
 3.  查询筛选文档注意项（本地FastAPI源码修改，上线部署不需要修改）
```

### Comparing `fastgenerateapi-0.0.6/README.md` & `fastgenerateapi-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 ###### FastGenerateApi 使用说明
 
 
 #### 软件架构说明
 
 ```
-封装了 快速生成API,包括(增,删,改,查,递归删除)
+封装了 快速生成API,包括(增,删,改,查,递归查询,递归删除,关联修改,关联查询)
 封装了 路由接口路径的灵活配置,返回值字段的灵活配置,分页参数的灵活配置,等其他项
 封装了 增,改 对唯一字段的校验,非空字段的校验
 封装了 删 对唯一字段追加时间戳格式修改
 封装了 查 灵活的筛选,以及swagger文档的自动生成
 封装了 通过数据库模型,自动生成schemas,并swagger附带文档
 封装了 类方法的实现,增加了相关的钩子函数
 封装了 通用性接口,例如excel的导入导出,pdf文件生成,模型数据跨表取值
-待封装 RPC的嵌套,API(关联增,关联删,关联改,关联查)
+待封装 RPC的嵌套
 ```
 
 #### 使用教程
 
 1.  简单使用
 2.  增删改查进一步优化使用
 3.  查询筛选文档注意项（本地FastAPI源码修改，上线部署不需要修改）
```

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/__init__.py` & `fastgenerateapi-0.0.7/fastgenerateapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/api_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/api_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/base_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/base_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import uuid
 from copy import copy
-from typing import Optional, Type, List, Union, Sequence
+from typing import Optional, Type, List, Union, Sequence, Dict
 from urllib.parse import parse_qs
 
 from fastapi import params
+from fastgenerateapi.controller.router_controller import BaseRouter
 from pydantic import create_model
 from starlette.requests import Request
 from tortoise import Model
 from tortoise.expressions import Q
 
 from fastgenerateapi.api_view.mixin.base_mixin import BaseMixin
 from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
@@ -23,51 +24,58 @@
 
     prefix: Optional[str] = None  # 路由追加后缀
     model_class: Optional[Type[Model]] = None  # 数据库模型
     prefetch_related_fields: Union[None, dict] = None
     schema: Optional[Type[BaseModel]] = None  # 返回序列化
     dependencies: Optional[Sequence[params.Depends]] = None
     tags: Optional[List[str]] = None  # swagger标签
+    router_args: Dict[str, Union[dict, str, tuple]] = None
 
     """
     # 增加外键字段显示
     prefetch_related_fields = {
           "avatar": None,           # 外键内容对应字典的形式
           "avatar": ["id", ("url", "avatar_url")]   # 增加 avatar_id,avatar_url2个字段
     }
 
-    # 暂不使用，可能会优化，也可能舍弃
-    # router_summary: List[Union[str, tuple, BaseRouterSummary]] = None
+    # router_args: List[Union[str, tuple, BaseRouterSummary]] = None
     # 给函数设置路由以及其他参数
-    router_summary = [
-        # 内置方法，可添加swagger备注和依赖
-        "get_one",
-        #("函数名", "默认POST方法", "路由[默认_替换为-]", "[依赖函数]", "swagger备注,默认函数名")
-        ("update_avatar", "PATCH", "update-avatar", [依赖函数], "修改头像"),
-    ]
+    # key为方法名，例如："get_one", "view_get_data"
+    router_args = {
+        "get_one": {
+            "response_model": CommonResponse;
+            "summary": "备注",
+            "dependencies": ["依赖函数"],
+        }
+        // 或者 "get_one": CommonResponse,
+        // 或者 "get_one": "备注",
+        // 或者 "get_one": ["依赖函数"],
+    }
     """
 
     def __init__(self, **kwargs):
         self.prefetch_related_fields: dict = self.prefetch_related_fields or {}
         try:
             prefix = self.prefix or self.get_model_strike_name(self.model_class)
             prefix = "/" + prefix.strip("/")
-        except:
+        except Exception:
             prefix = ""
-
-        tags = self.tags or [self.get_model_description(self.model_class) or prefix.strip("/").capitalize()]
+        try:
+            tags = self.tags or [self.get_model_description(self.model_class) or prefix.strip("/").capitalize()]
+        except Exception:
+            tags = None
         super().__init__(prefix=prefix, tags=tags, dependencies=self.dependencies, **kwargs)
 
         self.router_summary = RouterController(self, self._get_cls_func())
         for router in self.router_summary.router_data:
             self._add_api_route(
                 f"/{router.prefix}",
                 getattr(self, router.func_name),
                 methods=[router.method],
-                # response_model=self.success_response_schema,
+                response_model=router.response_model,
                 summary=router.summary,
                 dependencies=router.dependencies,
                 error_responses=[NOT_FOUND],
             )
 
         if self.model_class:
             for route_field in self._get_routes(is_controller_field=True):
```

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/create_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/create_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/delete_tree_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_tree_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/delete_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/delete_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_all_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_all_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_one_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_one_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_relation_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_relation_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/get_tree_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/get_tree_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/base_mixin.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/base_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/dbmodel_mixin.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/dbmodel_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/response_mixin.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/response_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/mixin/tool_mixin.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/mixin/tool_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,18 @@
             # rpc_param: Union[Dict[str, Dict[str, List[str]]], Type[RPCParam], None] = None,
             title: str = None,
             modules: str = "openpyxl"
     ) -> StreamingResponse:
         limit_modules = ["openpyxl", "xlsxwriter"]
         if modules not in limit_modules:
             self.error(msg=f"export xlsx modules only import {'、'.join(limit_modules)}")
-
-        wb = importlib.import_module(modules).Workbook()
+        try:
+            wb = importlib.import_module(modules).Workbook()
+        except Exception:
+            self.error(msg=f"please pip install {modules}")
         if modules == "openpyxl":
             def write(sh, row, col, value):
                 sh.cell(row, col).value = value
 
             start_col = 1
             start_row = 1
         else:
@@ -95,16 +97,18 @@
         """
         fields_list: [["名字", ("name", "名字"), (数据库字段， 字段中文名)], [第二行]]
 
         """
         limit_modules = ["fpdf"]
         if modules not in limit_modules:
             self.error(msg=f"export xlsx modules only import {'、'.join(limit_modules)}")
-
-        pdf = importlib.import_module(modules).FPDF()
+        try:
+            pdf = importlib.import_module(modules).FPDF()
+        except Exception:
+            self.error(msg=f"please pip install {modules}")
         pdf.add_page()
         pdf.add_font(font, '', font_path if font_path else f"../font/{font}.ttf", True)
         pdf.set_font(font, '', 8)
         if data:
             for data_row in data:
                 data_row_width = 180 / len(data_row)
                 for data_col in data_row:
@@ -176,16 +180,18 @@
 
         if not file:
             self.fail(msg=f"请先选择合适的文件")
 
         res = await file.read()
         with open(file_save_path, 'wb') as destination:
             destination.write(res)
-
-        wb = importlib.import_module(modules).load_workbook(file_save_path, read_only=True, data_only=True)
+        try:
+            wb = importlib.import_module(modules).load_workbook(file_save_path, read_only=True, data_only=True)
+        except Exception:
+            self.error(msg=f"please pip install {modules}")
         try:
             ws = wb.active
 
             header_row = ws[1]
             header_list = []
             for msg in header_row:
                 header_list.append(str(msg.value).replace(" ", ''))
@@ -258,14 +264,15 @@
                                 model_val = function(*args_list)
                         data[field] = model_val
                 try:
                     create_obj = model_class(**data)
                 except ValueError as e:
                     error_field = str(e).split(" ")[0]
                     return self.fail(msg=f"第{row}行{self._get_field_description(error_field)}填写错误")
+                await self.check_unique_field(create_obj, model_class=model_class)
                 create_list.append(create_obj)
 
             await model_class.bulk_create(create_list)
         finally:
             wb.close()
 
         if is_delete:
@@ -289,16 +296,18 @@
                 filename="导入模板.xlsx",
                 media_type="xlsx",
             )
 
         limit_modules = ["openpyxl", "xlsxwriter"]
         if modules not in limit_modules:
             return self.error(msg=f"export xlsx modules only import {'、'.join(limit_modules)}")
-
-        wb = importlib.import_module(modules).Workbook()
+        try:
+            wb = importlib.import_module(modules).Workbook()
+        except Exception:
+            self.error(msg=f"please pip install {modules}")
         if modules == "openpyxl":
             def write(sh, row, col, value):
                 sh.cell(row, col).value = value
 
             start_col = 1
             start_row = 1
         else:
```

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/switch_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/switch_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/update_relation_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_relation_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/api_view/update_view.py` & `fastgenerateapi-0.0.7/fastgenerateapi/api_view/update_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/controller/filter_controller.py` & `fastgenerateapi-0.0.7/fastgenerateapi/controller/filter_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/controller/rpc_controller.py` & `fastgenerateapi-0.0.7/fastgenerateapi/controller/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/controller/search_controller.py` & `fastgenerateapi-0.0.7/fastgenerateapi/controller/search_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/data_type/data_type.py` & `fastgenerateapi-0.0.7/fastgenerateapi/data_type/data_type.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/deps/filter_params_deps.py` & `fastgenerateapi-0.0.7/fastgenerateapi/deps/filter_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/deps/paginator_deps.py` & `fastgenerateapi-0.0.7/fastgenerateapi/deps/paginator_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/deps/tree_params_deps.py` & `fastgenerateapi-0.0.7/fastgenerateapi/deps/tree_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/example/models.py` & `fastgenerateapi-0.0.7/fastgenerateapi/example/models.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/pydantic_utils/base_model.py` & `fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/base_model.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/pydantic_utils/json_encoders.py` & `fastgenerateapi-0.0.7/fastgenerateapi/pydantic_utils/json_encoders.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/common_function.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/common_function.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/create_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/create_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/filter_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/filter_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_all_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_all_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_one_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_one_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_relation_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_relation_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/get_tree_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/get_tree_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/response_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/response_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/schemas_factory/update_schema_factory.py` & `fastgenerateapi-0.0.7/fastgenerateapi/schemas_factory/update_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/settings/settings.py` & `fastgenerateapi-0.0.7/fastgenerateapi/settings/settings.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi/utils/parse_str.py` & `fastgenerateapi-0.0.7/fastgenerateapi/utils/parse_str.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.7/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -27,23 +27,23 @@
 
 ###### FastGenerateApi 使用说明
 
 
 #### 软件架构说明
 
 ```
-封装了 快速生成API,包括(增,删,改,查,递归删除)
+封装了 快速生成API,包括(增,删,改,查,递归查询,递归删除,关联修改,关联查询)
 封装了 路由接口路径的灵活配置,返回值字段的灵活配置,分页参数的灵活配置,等其他项
 封装了 增,改 对唯一字段的校验,非空字段的校验
 封装了 删 对唯一字段追加时间戳格式修改
 封装了 查 灵活的筛选,以及swagger文档的自动生成
 封装了 通过数据库模型,自动生成schemas,并swagger附带文档
 封装了 类方法的实现,增加了相关的钩子函数
 封装了 通用性接口,例如excel的导入导出,pdf文件生成,模型数据跨表取值
-待封装 RPC的嵌套,API(关联增,关联删,关联改,关联查)
+待封装 RPC的嵌套
 ```
 
 #### 使用教程
 
 1.  简单使用
 2.  增删改查进一步优化使用
 3.  查询筛选文档注意项（本地FastAPI源码修改，上线部署不需要修改）
```

### Comparing `fastgenerateapi-0.0.6/fastgenerateapi.egg-info/SOURCES.txt` & `fastgenerateapi-0.0.7/fastgenerateapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 fastgenerateapi/api_view/create_view.py
 fastgenerateapi/api_view/delete_tree_view.py
 fastgenerateapi/api_view/delete_view.py
 fastgenerateapi/api_view/get_all_view.py
 fastgenerateapi/api_view/get_one_view.py
 fastgenerateapi/api_view/get_relation_view.py
 fastgenerateapi/api_view/get_tree_view.py
+fastgenerateapi/api_view/sql_get_view.py
 fastgenerateapi/api_view/switch_view.py
 fastgenerateapi/api_view/update_relation_view.py
 fastgenerateapi/api_view/update_view.py
 fastgenerateapi/api_view/mixin/__init__.py
 fastgenerateapi/api_view/mixin/base_mixin.py
 fastgenerateapi/api_view/mixin/dbmodel_mixin.py
 fastgenerateapi/api_view/mixin/get_mixin.py
```

### Comparing `fastgenerateapi-0.0.6/setup.py` & `fastgenerateapi-0.0.7/setup.py`

 * *Files identical despite different names*

