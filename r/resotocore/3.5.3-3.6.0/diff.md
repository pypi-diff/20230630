# Comparing `tmp/resotocore-3.5.3.tar.gz` & `tmp/resotocore-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.5.3.tar", last modified: Wed Jun 21 14:20:18 2023, max compression
+gzip compressed data, was "resotocore-3.6.0.tar", last modified: Fri Jun 30 19:29:18 2023, max compression
```

## Comparing `resotocore-3.5.3.tar` & `resotocore-3.6.0.tar`

### file list

```diff
@@ -1,804 +1,804 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 14:16:24.000000 resotocore-3.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-21 14:16:24.000000 resotocore-3.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-21 14:20:18.328908 resotocore-3.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-21 14:16:24.000000 resotocore-3.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-21 14:16:24.000000 resotocore-3.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.224905 resotocore-3.5.3/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.224905 resotocore-3.5.3/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.224905 resotocore-3.5.3/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.224905 resotocore-3.5.3/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   229427 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/cli/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.224905 resotocore-3.5.3/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    37884 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.228905 resotocore-3.5.3/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32054 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/deferred_edge_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    64016 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.228905 resotocore-3.5.3/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.228905 resotocore-3.5.3/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.232905 resotocore-3.5.3/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.212905 resotocore-3.5.3/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.232905 resotocore-3.5.3/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 14:20:14.000000 resotocore-3.5.3/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.232905 resotocore-3.5.3/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 14:20:14.000000 resotocore-3.5.3/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 14:20:14.000000 resotocore-3.5.3/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.288907 resotocore-3.5.3/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1037.51967a2.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1079.cdbaf67.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1084.4cd1c89.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1113.23c9417.js
--rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1125.129d070.js
--rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1163.ac28297.js
--rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1221.c51249a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1245.be46619.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1261.199fc1d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1272.f334098.js
--rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1278.0524a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1290.3981211.js
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1295.46e72b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1310.23bbe67.js
--rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1320.21effe3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1325.f76267c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1408.7461890.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1440.a9e7ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1483.616d9ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1489.e50b6d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1507.5705605.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/152.525d460.js
--rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1520.4e2eb21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1555.e188f3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1559.7c89925.js
--rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/160.5f28731.js
--rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1603.370a2a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1644.0e49167.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1667.f0afb2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1687.27f1ad6.js
--rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1725.f151c33.js
--rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1767.c8c2f26.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1806.1aaf66b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1838.1202b16.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1909.28a2def.js
--rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/1989.88d258f.js
--rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2030.1562cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2047.baed97b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2099.f4b6fcd.js
--rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2118.5b65f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/213.5769e57.js
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2161.dcb27b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2169.635c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/217.90d10e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2212.72be094.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2287.997c38e.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2303.9ff8710.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2319.6b4cbb7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2329.4c5ca6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2351.fbd96d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2358.d5cf7c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2359.6451c3e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/237.f765e77.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2384.71782be.js
--rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/240.cddc46b.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2431.648d237.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2546.1f48267.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2557.75e9da2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/261.5f53c0e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2629.c0e1cd6.js
--rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2788.46acc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2834.942acc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2887.47ba752.js
--rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2956.8880209.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/2973.2a51dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3004.255e79c.js
--rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/302.8bcc38f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3037.70ee38d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3042.7cfad84.js
--rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3051.34fac68.js
--rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3122.2289fca.js
--rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3151.10ef4de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/316.c850a76.js
--rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3196.4e35a17.js
--rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3265.a80440a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3277.9c04e75.js
--rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/330.126fa98.js
--rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3392.29fe6b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3413.480a49d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3444.47d5ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3469.7d14d0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3546.fee1bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/362.6716970.js
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3708.410d087.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3850.903abc2.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3880.bd39dce.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3970.236586f.js
--rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3976.58893b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/3979.385527e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/400.d72234b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4018.1a35967.js
--rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/406.9b7af92.js
--rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4117.a8107fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4182.e2430f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4191.02bbea8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4197.53ab10b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4206.a5f8bb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4207.0d0580b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4262.bb73457.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4298.5ee510c.js
--rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/44.0cfa785.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4410.e4a25d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4466.64d23d1.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/451.d9683ad.js
--rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4535.34b060a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4565.43bdb91.js
--rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4569.f374f9d.js
--rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4615.eb5d40a.js
--rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4658.090d4a9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4665.aa19a41.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4668.f65690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4690.3dd4096.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4715.e7690b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4749.46ebbb2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4750.56c06ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4856.2d7415f.js
--rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4875.375150e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/489.b981dea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/490.c2624d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4905.667bf33.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4931.430433b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/4942.b96c164.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5016.dd2fe83.js
--rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5072.733a1b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/509.6448878.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5096.8ed0d8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5126.eecad7a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5129.1ba4763.js
--rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5153.763d8fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5155.06b4ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5193.e9f6866.js
--rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5213.3e1a360.js
--rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5227.8c8acd8.js
--rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5238.1751cc3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/528.2262cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5292.79d4aba.js
--rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5437.31236f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5489.848a8cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5508.317fca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/554.ac98303.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/555.2cd31dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5573.ebcdb93.js
--rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5666.c5e5324.js
--rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5710.70d0b1d.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5747.94ad626.js
--rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/582.21b8e7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5823.5045bdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5851.30b7b2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5878.32d92fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5880.68f975b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5955.88508f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/5971.88c5642.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6080.aa0ff24.js
--rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/61.2808a0d.js
--rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6136.b8ba2b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6141.9831d58.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6475.6037fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6493.d796aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6556.b3d9293.js
--rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6571.2c8884e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6576.3ea568e.js
--rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6591.94ed352.js
--rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6612.1632879.js
--rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6623.ae3b3cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6664.2160109.js
--rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6747.47be7f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6748.be68f5f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6870.7940288.js
--rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6879.c8367a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6898.9bbc12a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6952.f68b818.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6985.321ad92.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6993.32cf9a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/6997.b06fe71.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7041.d4f561e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7058.805c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7174.6c45206.js
--rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7334.8859b1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7359.6ee65ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7364.195178b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7380.58a4413.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7427.f9c2017.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7463.18fd278.js
--rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7509.1e0189e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7526.1a303e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7537.1323a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7692.33d5169.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7746.5908d29.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7808.1d582a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/783.c156751.js
--rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7858.2386e4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/7941.01ea680.js
--rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8005.c5ad7b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8028.39e2fa1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8061.cc62561.js
--rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8101.cf46d02.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/812.9b0e86e.js
--rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/816.c8050f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8165.b2c3285.js
--rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8232.a578bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/824.8678196.js
--rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8270.89fe7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/833.9cc6653.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8370.8f855e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8373.96b0b3a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8389.ffe031f.js
--rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8412.1528057.js
--rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8427.4923f43.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8542.027afdc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8594.0112f03.js
--rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8656.d5b8e92.js
--rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8685.d78bdab.js
--rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8698.9817d75.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8732.9320f73.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8785.cf4fe95.js
--rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8828.77c71d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8883.80c7b63.js
--rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8976.3816942.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8981.99a4275.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/8990.2a453cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9035.1e45c1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9053.45b77fc.js
--rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9077.fefb6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9128.b8fa6f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9156.0cefbd3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9170.0023587.js
--rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9196.315f9f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9198.9971d70.js
--rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/920.d15c177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9253.0b31caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9266.bacd0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9307.c3a00ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9321.869e413.js
--rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9344.ba0abcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9382.9014799.js
--rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9440.1b10b8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9464.79e6ac5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9502.9a24831.js
--rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9507.1e6cc5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9602.62bf0f1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9621.e2e8b5d.js
--rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9622.ccab065.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9626.a178bd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9647.ed91993.js
--rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9657.bc5c60e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/97.ad126b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9712.796a0a1.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9733.a3b2a7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9737.7dc8f98.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9777.0b8a504.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9793.6d63a85.js
--rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9806.652c162.js
--rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9865.2e3db6f.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/989.bcca86a.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9943.f3f35c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9958.25c8c06.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/9960.64cd61e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.288907 resotocore-3.5.3/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.288907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.288907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.288907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.288907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.292907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/service-worker-b2fb40a.js
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.216905 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.296907 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.300907 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
--rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.300907 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.300907 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
--rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-06-21 14:20:11.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.300907 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-06-21 14:20:02.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-06-21 14:20:08.000000 resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-21 14:20:14.000000 resotocore-3.5.3/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/kernelspecs/javascript.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/service-worker-b2fb40a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.308907 resotocore-3.5.3/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.5.3/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.312908 resotocore-3.5.3/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    55069 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.312908 resotocore-3.5.3/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.312908 resotocore-3.5.3/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/report/report_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.312908 resotocore-3.5.3/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   129588 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.312908 resotocore-3.5.3/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.220905 resotocore-3.5.3/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.312908 resotocore-3.5.3/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.220905 resotocore-3.5.3/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.316908 resotocore-3.5.3/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/report/checks/aws/aws_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/resoto.css
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/static/resoto_logo_and_text.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.316908 resotocore-3.5.3/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.316908 resotocore-3.5.3/resotocore/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.316908 resotocore-3.5.3/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.320908 resotocore-3.5.3/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65833 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-21 14:16:24.000000 resotocore-3.5.3/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.224905 resotocore-3.5.3/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-21 14:20:18.000000 resotocore-3.5.3/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-06-21 14:20:18.000000 resotocore-3.5.3/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:18.000000 resotocore-3.5.3/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 14:20:18.000000 resotocore-3.5.3/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:20:17.000000 resotocore-3.5.3/resotocore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-21 14:20:18.000000 resotocore-3.5.3/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 14:20:18.000000 resotocore-3.5.3/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-21 14:20:18.328908 resotocore-3.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.320908 resotocore-3.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.320908 resotocore-3.5.3/tests/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.320908 resotocore-3.5.3/tests/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.320908 resotocore-3.5.3/tests/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    57404 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.324908 resotocore-3.5.3/tests/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27555 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.324908 resotocore-3.5.3/tests/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    28962 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/subscriberdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.324908 resotocore-3.5.3/tests/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.324908 resotocore-3.5.3/tests/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/tests/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/tests/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/tests/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/report/benchnmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/tests/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/tests/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:20:18.328908 resotocore-3.5.3/tests/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-21 14:16:24.000000 resotocore-3.5.3/tests/resotocore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 19:24:13.000000 resotocore-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 19:24:13.000000 resotocore-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-30 19:29:18.584757 resotocore-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-30 19:24:13.000000 resotocore-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 19:24:13.000000 resotocore-3.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.392756 resotocore-3.6.0/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.392756 resotocore-3.6.0/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.396756 resotocore-3.6.0/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.396756 resotocore-3.6.0/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31065 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   242365 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26704 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.396756 resotocore-3.6.0/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.400756 resotocore-3.6.0/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32054 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/deferred_edge_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64492 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.400756 resotocore-3.6.0/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.376756 resotocore-3.6.0/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.504756 resotocore-3.6.0/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1037.51967a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1079.cdbaf67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1084.4cd1c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1113.23c9417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1125.129d070.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1163.ac28297.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1221.c51249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1245.be46619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1261.199fc1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1272.f334098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1290.3981211.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1295.46e72b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1310.23bbe67.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1320.21effe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1325.f76267c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1408.7461890.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1440.a9e7ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1483.616d9ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1489.e50b6d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1507.5705605.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/152.525d460.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1520.4e2eb21.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1555.e188f3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1559.7c89925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/160.5f28731.js
+-rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1603.370a2a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1644.0e49167.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1667.f0afb2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1687.27f1ad6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1725.f151c33.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1767.c8c2f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1806.1aaf66b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1838.1202b16.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1909.28a2def.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1989.88d258f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2030.1562cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2047.baed97b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2099.f4b6fcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2118.5b65f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/213.5769e57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2161.dcb27b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2169.635c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/217.90d10e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2212.72be094.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2303.9ff8710.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2319.6b4cbb7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2329.4c5ca6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2351.fbd96d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2358.d5cf7c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2359.6451c3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/237.f765e77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2384.71782be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/240.cddc46b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2431.648d237.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2546.1f48267.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2557.75e9da2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/261.5f53c0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2629.c0e1cd6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2788.46acc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2834.942acc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2887.47ba752.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2956.8880209.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2973.2a51dc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3004.255e79c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/302.8bcc38f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3037.70ee38d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3042.7cfad84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3051.34fac68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3122.2289fca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3151.10ef4de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/316.c850a76.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3196.4e35a17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3265.a80440a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3277.9c04e75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/330.126fa98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3392.29fe6b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3413.480a49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3444.47d5ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3469.7d14d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3546.fee1bd7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/362.6716970.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3708.410d087.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3880.bd39dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3970.236586f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3979.385527e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/400.d72234b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4018.1a35967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/406.9b7af92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4117.a8107fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4182.e2430f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4191.02bbea8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4197.53ab10b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4206.a5f8bb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4207.0d0580b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4262.bb73457.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4298.5ee510c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4410.e4a25d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4466.64d23d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/451.d9683ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4535.34b060a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4565.43bdb91.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4569.f374f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4615.eb5d40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4658.090d4a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4665.aa19a41.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4668.f65690b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4690.3dd4096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4715.e7690b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4749.46ebbb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4750.56c06ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4856.2d7415f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4875.375150e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/489.b981dea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/490.c2624d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4905.667bf33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4931.430433b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4942.b96c164.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5016.dd2fe83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5072.733a1b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/509.6448878.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5096.8ed0d8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5126.eecad7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5129.1ba4763.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5153.763d8fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5155.06b4ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5193.e9f6866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5213.3e1a360.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5227.8c8acd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5238.1751cc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/528.2262cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5292.79d4aba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5437.31236f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5489.848a8cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5508.317fca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/554.ac98303.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/555.2cd31dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5573.ebcdb93.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5666.c5e5324.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5710.70d0b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5747.94ad626.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/582.21b8e7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5823.5045bdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5851.30b7b2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5878.32d92fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5880.68f975b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5955.88508f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5971.88c5642.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6080.aa0ff24.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/61.2808a0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6136.b8ba2b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6141.9831d58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6475.6037fbb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6493.d796aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6556.b3d9293.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6571.2c8884e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6576.3ea568e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6591.94ed352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6612.1632879.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6623.ae3b3cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6664.2160109.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6747.47be7f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6748.be68f5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6870.7940288.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6879.c8367a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6898.9bbc12a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6952.f68b818.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6985.321ad92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6993.32cf9a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6997.b06fe71.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7041.d4f561e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7058.805c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7174.6c45206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7334.8859b1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7359.6ee65ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7364.195178b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7380.58a4413.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7427.f9c2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7463.18fd278.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7509.1e0189e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7526.1a303e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7537.1323a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7692.33d5169.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7746.5908d29.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7808.1d582a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/783.c156751.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7858.2386e4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7941.01ea680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8005.c5ad7b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8028.39e2fa1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8061.cc62561.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8101.cf46d02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/812.9b0e86e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/816.c8050f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8165.b2c3285.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8232.a578bf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/824.8678196.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8270.89fe7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/833.9cc6653.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8370.8f855e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8373.96b0b3a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8389.ffe031f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8412.1528057.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8427.4923f43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8542.027afdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8594.0112f03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8656.d5b8e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8685.d78bdab.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8698.9817d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8732.9320f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8785.cf4fe95.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8828.77c71d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8883.80c7b63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8976.3816942.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8981.99a4275.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8990.2a453cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9035.1e45c1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9053.45b77fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9077.fefb6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9128.b8fa6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9156.0cefbd3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9170.0023587.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9196.315f9f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9198.9971d70.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/920.d15c177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9253.0b31caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9266.bacd0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9307.c3a00ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9321.869e413.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9344.ba0abcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9382.9014799.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9440.1b10b8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9464.79e6ac5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9502.9a24831.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9507.1e6cc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9602.62bf0f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9621.e2e8b5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9622.ccab065.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9626.a178bd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9647.ed91993.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9657.bc5c60e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/97.ad126b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9712.796a0a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9733.a3b2a7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9737.7dc8f98.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9777.0b8a504.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9793.6d63a85.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9806.652c162.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9865.2e3db6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/989.bcca86a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9943.f3f35c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9958.25c8c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9960.64cd61e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/service-worker-b2fb40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.384756 resotocore-3.6.0/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.528756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.528756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.532756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.532756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.536756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.536756 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/kernelspecs/javascript.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/service-worker-b2fb40a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.552757 resotocore-3.6.0/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58079 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.552757 resotocore-3.6.0/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.552757 resotocore-3.6.0/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/report_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.556757 resotocore-3.6.0/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   129588 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.556757 resotocore-3.6.0/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.384756 resotocore-3.6.0/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.556757 resotocore-3.6.0/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.384756 resotocore-3.6.0/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.560757 resotocore-3.6.0/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/resoto.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/resoto_logo_and_text.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.560757 resotocore-3.6.0/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/resotocore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66253 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.392756 resotocore-3.6.0/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:17.000000 resotocore-3.6.0/resotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:29:18.584757 resotocore-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.568757 resotocore-3.6.0/tests/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.568757 resotocore-3.6.0/tests/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.568757 resotocore-3.6.0/tests/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59377 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.572757 resotocore-3.6.0/tests/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27737 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.576757 resotocore-3.6.0/tests/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/subscriberdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.576757 resotocore-3.6.0/tests/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.576757 resotocore-3.6.0/tests/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.580757 resotocore-3.6.0/tests/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.580757 resotocore-3.6.0/tests/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.580757 resotocore-3.6.0/tests/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/report/benchnmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/tests/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/tests/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/tests/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/worker_task_queue_test.py
```

### Comparing `resotocore-3.5.3/LICENSE` & `resotocore-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/PKG-INFO` & `resotocore-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.5.3
+Version: 3.6.0
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://resoto.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: extra
 Provides-Extra: test
 License-File: LICENSE
 
 # `resotocore`
 Resoto core graph platform
```

### Comparing `resotocore-3.5.3/README.md` & `resotocore-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/pyproject.toml` & `resotocore-3.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotocore"
-version = "3.5.3"
+version = "3.6.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = {file="LICENSE"}
 urls = {"Homepage" = "https://resoto.com"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
@@ -24,42 +24,47 @@
     "jq",
     "jsons",
     "parsy",
     "plantuml",
     "posthog",
     "python-arango",
     "python-dateutil",
+    "resotodatalink>=1.2.0",
     "resotoui",
     "rich",
     "toolz",
     "transitions",
     "tzlocal",
     "ustache",
 ]
 
 [project.optional-dependencies]
-dev = [
-    "mypy",
+
+extra = [
+    "resotodatalink[extra]"
+]
+
+test = [
+    "black",
+    "coverage",
     "flake8",
+    "hypothesis",
+    "mypy",
     "pep8-naming",
-    "tox",
-    "coverage",
-    "pylint",
-    "black",
-    "toml",
     "pip-tools",
-]
-test = [
+    "pylint",
     "pytest",
-    "pytest-cov",
     "pytest-asyncio",
-    "hypothesis",
-    "resotoclient",
+    "pytest-cov",
+    "resotoclient>=1.5.0",
+    "toml",
+    "tox",
 ]
 
+
 [project.scripts]
 resotocore = "resotocore.__main__:main"
 
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `resotocore-3.5.3/resotocore/__main__.py` & `resotocore-3.6.0/resotocore/__main__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.6.0/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/analytics/__init__.py` & `resotocore-3.6.0/resotocore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/analytics/posthog.py` & `resotocore-3.6.0/resotocore/analytics/posthog.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         # acquire the lock, send all events to the client and clear the queue
         async with self.lock:
             for event in self.queue:
                 self.client.capture(
                     distinct_id=self.system_data.system_id,
                     event=event.kind,
                     properties={
-                        **event.context,  # type: ignore
-                        **event.counters,  # type: ignore
+                        **event.context,
+                        **event.counters,
                         "source": event.system,
                         "run_id": self.run_id,
                     },
                     timestamp=event.at,
                 )
             self.queue.clear()
```

### Comparing `resotocore-3.5.3/resotocore/analytics/recurrent_events.py` & `resotocore-3.6.0/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/async_extensions.py` & `resotocore-3.6.0/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/cli/__init__.py` & `resotocore-3.6.0/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/cli/cli.py` & `resotocore-3.6.0/resotocore/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import logging
 from asyncio import Task
 from contextlib import suppress
 from itertools import takewhile
 from operator import attrgetter
 from textwrap import dedent
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Union, Sequence
 from typing import Optional, Any
 
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import evolve
 from parsy import Parser
 from rich.padding import Padding
@@ -35,14 +35,15 @@
     WelcomeCommand,
     SortPart,
     LimitPart,
     HistoryPart,
     ReportCommand,
     WriteCommand,
 )
+from resotocore.cli.dependencies import CLIDependencies
 from resotocore.cli.model import (
     ParsedCommand,
     ParsedCommands,
     ExecutableCommand,
     ParsedCommandLine,
     CLICommand,
     InternalPart,
@@ -55,15 +56,14 @@
     PreserveOutputFormat,
     AliasTemplate,
     InfraAppAlias,
     ArgsInfo,
     ArgInfo,
     AliasTemplateParameter,
 )
-from resotocore.cli.dependencies import CLIDependencies
 from resotocore.console_renderer import ConsoleRenderer
 from resotocore.error import CLIParseError
 from resotocore.model.typed_model import class_fqn
 from resotocore.query.model import (
     Query,
     Navigation,
     AllTerm,
@@ -496,23 +496,21 @@
         async def combine_query_parts(
             commands: List[ExecutableCommand], ctx: CLIContext
         ) -> Tuple[CLIContext, List[ExecutableCommand]]:
             parts = list(takewhile(lambda x: isinstance(x.command, SearchCLIPart), commands))
             if parts:
                 query, options, query_parts = await self.create_query(parts, ctx)
                 ctx_wq = evolve(ctx, query=query, query_options=options, commands=commands)
-                part_offset = len(parts)
-                remaining = [
-                    self.command(c.name, c.arg, ctx_wq, position=pos + part_offset)
-                    for pos, c in enumerate(commands[len(parts) :])
-                ]  # noqa: E203
+                remaining = executable_commands(
+                    commands[len(parts) :], ctx_wq, offset=len(parts), previous_command=query_parts[-1]
+                )
                 rewritten_parts = [*query_parts, *remaining]
             else:
                 ctx_wq = evolve(ctx, commands=commands)
-                rewritten_parts = [self.command(c.name, c.arg, ctx_wq, position=pos) for pos, c in enumerate(commands)]
+                rewritten_parts = executable_commands(commands, ctx_wq)
             # re-evaluate remaining commands - to take the adapted context into account
             return ctx_wq, rewritten_parts
 
         def rewrite_command_line(cmds: List[ExecutableCommand], ctx: CLIContext) -> List[ExecutableCommand]:
             """
             Rewrite the command line to make it more user-friendly.
             Rules:
@@ -555,17 +553,33 @@
             ctx = evolve(context, env=cmd_env)
             last_command = self.commands.get(parsed.commands[-1].cmd) if parsed.commands else None
             if isinstance(last_command, NoTerminalOutput) and ctx.console_renderer:
                 return evolve(ctx, env=cmd_env, console_renderer=ConsoleRenderer.default_renderer())
             else:
                 return evolve(context, env=cmd_env)
 
+        # iterate the list of commands and pass information about position, previous command, etc.
+        def executable_commands(
+            commands: Sequence[Union[ParsedCommand, ExecutableCommand]],
+            ctx: CLIContext,
+            *,
+            previous_command: Optional[ExecutableCommand] = None,
+            offset: int = 0,
+        ) -> List[ExecutableCommand]:
+            result: List[ExecutableCommand] = []
+            for pos, c in enumerate(commands):
+                name, arg = (c.cmd, c.args) if isinstance(c, ParsedCommand) else (c.name, c.arg)
+                command = self.command(name, arg, ctx, position=pos + offset, previous_command=previous_command)
+                previous_command = command
+                result.append(command)
+            return result
+
         async def parse_line(parsed: ParsedCommands) -> ParsedCommandLine:
             ctx = adjust_context(parsed)
-            executable = [self.command(c.cmd, c.args, ctx, position=i) for i, c in enumerate(parsed.commands)]
+            executable = executable_commands(parsed.commands, ctx)
             rewritten = rewrite_command_line(executable, ctx)
             ctx, commands = await combine_query_parts(rewritten, ctx)
             not_met = [r for cmd in commands for r in cmd.action.required if r.name not in context.uploaded_files]
             envelope = {k: v for cmd in commands for k, v in cmd.action.envelope.items()}
             return ParsedCommandLine(ctx, parsed, commands, not_met, envelope)
 
         def expand_aliases(line: ParsedCommands) -> ParsedCommands:
```

### Comparing `resotocore-3.5.3/resotocore/cli/command.py` & `resotocore-3.6.0/resotocore/cli/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,52 +5,60 @@
 import io
 import json
 import logging
 import os.path
 import re
 import shutil
 import tarfile
-import tempfile
 from abc import abstractmethod, ABC
 from argparse import Namespace
 from asyncio import Future, Task
+
+# noinspection PyProtectedMember
 from asyncio.subprocess import Process
 from collections import defaultdict
 from contextlib import suppress
 from datetime import timedelta, datetime
 from functools import partial, lru_cache
 from itertools import dropwhile, chain
-from tempfile import TemporaryDirectory
+from pathlib import Path
 from typing import (
     Dict,
     List,
     Tuple,
     Optional,
     Any,
     AsyncIterator,
     Hashable,
     Iterable,
     Callable,
     Awaitable,
     cast,
     Set,
     FrozenSet,
+    Union,
 )
 from urllib.parse import urlparse, urlunparse
 
 import aiofiles
 import jq
 import yaml
+from aiofiles.tempfile import TemporaryDirectory
 from aiohttp import ClientTimeout, JsonPayload, BasicAuth
 from aiostream import stream, pipe
 from aiostream.aiter_utils import is_async_iterable
 from aiostream.core import Stream
+from attr import evolve
 from attrs import define, field
 from dateutil import parser as date_parser
 from parsy import Parser, string
+from resotoclient.models import Model as RCModel, Kind as RCKind
+from resotodatalink import EngineConfig
+from resotodatalink.batch_stream import BatchStream
+from resotodatalink.collect_plugins import update_sql
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 
 from resotocore import version
 from resotocore.async_extensions import run_async
@@ -62,14 +70,15 @@
     is_edge,
     is_node,
     js_value_at,
     js_value_get,
     key_values_parser,
     parse_time_or_delta,
     strip_quotes,
+    key_value_parser,
 )
 from resotocore.cli.dependencies import CLIDependencies
 from resotocore.cli.model import (
     CLICommand,
     CLIContext,
     EmptyContext,
     CLIAction,
@@ -81,14 +90,15 @@
     MediaType,
     CLIFileRequirement,
     ParsedCommand,
     NoTerminalOutput,
     ArgsInfo,
     ArgInfo,
     EntityProvider,
+    FilePath,
 )
 from resotocore.cli.tip_of_the_day import SuggestionPolicy, SuggestionStrategy, get_suggestion_strategy
 from resotocore.config import ConfigEntity
 from resotocore.db.async_arangodb import AsyncCursor
 from resotocore.db.graphdb import HistoryChange, GraphDB
 from resotocore.db.model import QueryModel
 from resotocore.db.runningtaskdb import RunningTaskData
@@ -116,14 +126,18 @@
     Template,
     NavigateUntilRoot,
     Term,
     AggregateFunction,
     AggregateVariableName,
     AggregateVariableCombined,
     Aggregate,
+    AggregateVariable,
+    Part,
+    NavigateUntilLeaf,
+    IsTerm,
 )
 from resotocore.query.query_parser import parse_query, aggregate_parameter_parser
 from resotocore.query.template_expander import tpl_props_p
 from resotocore.report import BenchmarkConfigPrefix, ReportSeverity
 from resotocore.report.benchmark_renderer import respond_benchmark_result
 from resotocore.task.task_description import Job, TimeTrigger, EventTrigger, ExecuteCommand, Workflow, RunningTask
 from resotocore.types import Json, JsonElement, EdgeType
@@ -134,14 +148,15 @@
     if_set,
     duration,
     identity,
     rnd_str,
     set_value_in_path,
     restart_service,
     combine_optional,
+    value_in_path,
 )
 from resotocore.web.content_renderer import (
     respond_ndjson,
     respond_json,
     respond_text,
     respond_graphml,
     respond_dot,
@@ -163,14 +178,18 @@
 )
 from resotolib.utils import safe_members_in_tarfile, get_local_tzinfo
 from resotolib.x509 import write_cert_to_file, write_key_to_file
 
 log = logging.getLogger(__name__)
 
 
+def deps(command: CLICommand) -> CLIDependencies:
+    return cast(CLIDependencies, command.dependencies)
+
+
 # A SearchCLIPart is a command that can be used on the command line.
 # Such a part is not executed, but builds a search, which is executed.
 # Therefore, the parse method is implemented in a dummy fashion here.
 # The real interpretation happens in CLI.create_query.
 class SearchCLIPart(CLICommand, EntityProvider, ABC):
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         return CLISource.empty()
@@ -3457,119 +3476,117 @@
                 "restore": [
                     ArgInfo(None, expects_value=True, help_text="local backup file to upload.", value_hint="file")
                 ],
             },
             "info": [],
         }
 
-    async def create_backup(self, arg: Optional[str]) -> AsyncIterator[str]:
-        temp_dir: str = tempfile.mkdtemp()
+    async def create_backup(self, arg: Optional[str]) -> AsyncIterator[JsonElement]:
         maybe_proc: Optional[Process] = None
-        try:
-            db_config = cast(CLIDependencies, self.dependencies).config.db
-            if not shutil.which("arangodump"):
-                raise CLIParseError("db_backup expects the executable `arangodump` to be in path!")
-            # fmt: off
-            process = await asyncio.create_subprocess_exec(
-                "arangodump",
-                "--progress", "false",  # do not show progress
-                "--include-system-collections", "true",  # graphs are considered a system collection
-                "--threads", "8",  # default is 2
-                "--log.level", "error",  # only print error messages
-                "--output-directory", temp_dir,  # directory to write to
-                "--overwrite", "true",  # required for existing directories
-                "--server.endpoint", db_config.server.replace("http", "http+tcp"),
-                "--server.authentication", "false" if db_config.no_ssl_verify else "true",
-                "--server.database", db_config.database,
-                "--server.username", db_config.username,
-                "--server.password", db_config.password,
-                "--configuration", "none",
-                stdout=asyncio.subprocess.PIPE,
-                stderr=asyncio.subprocess.PIPE,
-            )
-            # fmt: on
-            stdout_b, stderr_b = await process.communicate()
-            maybe_proc = process
-            code = await process.wait()
-            stdout = stdout_b.decode() if stdout_b else ""
-            stderr = stderr_b.decode() if stderr_b else ""
-
-            if code == 0:
-                log.debug(f"arangodump: out={stdout}, err={stderr}.")
-                files = os.listdir(temp_dir)
-                name = re.sub("[^a-zA-Z0-9_\\-.]", "_", arg) if arg else f'backup_{utc().strftime("%Y%m%d_%H%M")}'
-                backup = os.path.join(temp_dir, name)
-                # create an unzipped tarfile (all of the entries are already gzipped)
-                with tarfile.open(backup, "w") as tar:
-                    for file in files:
-                        await run_async(tar.add, os.path.join(temp_dir, file), file)
-                yield backup
-            else:
-                log.error(f"Could not create backup: {code}. out={stdout}, err={stderr}")
-                raise CLIExecutionError(f"Creation of backup failed! Response from process:\n{stderr}")
-        finally:
-            if maybe_proc and maybe_proc.returncode is None:
-                with suppress(Exception):
-                    maybe_proc.kill()
-                    await asyncio.sleep(5)
-            shutil.rmtree(temp_dir)
+        async with TemporaryDirectory() as temp_dir:
+            try:
+                db_config = cast(CLIDependencies, self.dependencies).config.db
+                if not shutil.which("arangodump"):
+                    raise CLIParseError("db_backup expects the executable `arangodump` to be in path!")
+                # fmt: off
+                process = await asyncio.create_subprocess_exec(
+                    "arangodump",
+                    "--progress", "false",  # do not show progress
+                    "--include-system-collections", "true",  # graphs are considered a system collection
+                    "--threads", "8",  # default is 2
+                    "--log.level", "error",  # only print error messages
+                    "--output-directory", temp_dir,  # directory to write to
+                    "--overwrite", "true",  # required for existing directories
+                    "--server.endpoint", db_config.server.replace("http", "http+tcp"),
+                    "--server.authentication", "false" if db_config.no_ssl_verify else "true",
+                    "--server.database", db_config.database,
+                    "--server.username", db_config.username,
+                    "--server.password", db_config.password,
+                    "--configuration", "none",
+                    stdout=asyncio.subprocess.PIPE,
+                    stderr=asyncio.subprocess.PIPE,
+                )
+                # fmt: on
+                stdout_b, stderr_b = await process.communicate()
+                maybe_proc = process
+                code = await process.wait()
+                stdout = stdout_b.decode() if stdout_b else ""
+                stderr = stderr_b.decode() if stderr_b else ""
+
+                if code == 0:
+                    log.debug(f"arangodump: out={stdout}, err={stderr}.")
+                    files = os.listdir(temp_dir)
+                    name = re.sub("[^a-zA-Z0-9_\\-.]", "_", arg) if arg else f'backup_{utc().strftime("%Y%m%d_%H%M")}'
+                    backup = os.path.join(temp_dir, name)
+                    # create an unzipped tarfile (all of the entries are already gzipped)
+                    with tarfile.open(backup, "w") as tar:
+                        for file in files:
+                            await run_async(tar.add, os.path.join(temp_dir, file), file)
+                    yield FilePath.user_local(arg or name, backup).json()
+                else:
+                    log.error(f"Could not create backup: {code}. out={stdout}, err={stderr}")
+                    raise CLIExecutionError(f"Creation of backup failed! Response from process:\n{stderr}")
+            finally:
+                if maybe_proc and maybe_proc.returncode is None:
+                    with suppress(Exception):
+                        maybe_proc.kill()
+                        await asyncio.sleep(5)
 
     async def restore_backup(self, backup_file: Optional[str], ctx: CLIContext) -> AsyncIterator[str]:
         if not backup_file:
             raise CLIExecutionError(f"No backup file defined: {backup_file}")
         if not os.path.exists(backup_file):
             raise CLIExecutionError(f"Provided backup file does not exist: {backup_file}")
         if not shutil.which("arangorestore"):
             raise CLIParseError("db_restore expects the executable `arangorestore` to be in path!")
 
-        temp_dir: str = tempfile.mkdtemp()
-        maybe_proc: Optional[Process] = None
-        try:
-            # extract tar file
-            with tarfile.open(backup_file, "r") as tar:
-                tar.extractall(temp_dir, members=safe_members_in_tarfile(tar))
-
-            # fmt: off
-            db_conf = cast(CLIDependencies, self.dependencies).config.db
-            process = await asyncio.create_subprocess_exec(
-                "arangorestore",
-                "--progress", "false",  # do not show progress
-                "--include-system-collections", "true",  # graphs are considered a system collection
-                "--threads", "8",  # default is 2
-                "--log.level", "error",  # only print error messages
-                "--input-directory", temp_dir,  # directory to write to
-                "--overwrite", "true",  # required for existing db collections
-                "--server.endpoint", db_conf.server.replace("http", "http+tcp"),
-                "--server.authentication", "false" if db_conf.no_ssl_verify else "true",
-                "--server.database", db_conf.database,
-                "--server.username", db_conf.username,
-                "--server.password", db_conf.password,
-                "--configuration", "none",
-                stdout=asyncio.subprocess.PIPE,
-                stderr=asyncio.subprocess.PIPE,
-            )
-            # fmt: on
-            stdout_b, stderr_b = await process.communicate()
-            maybe_proc = process
-            code = await process.wait()
-            stdout = stdout_b.decode() if stdout_b else ""
-            stderr = stderr_b.decode() if stderr_b else ""
-
-            if code == 0:
-                log.debug(f"arangorestore: out={stdout}, err={stderr}.")
-                yield "Database has been restored successfully!"
-            else:
-                log.error(f"Could not restore backup: {code}. out={stdout}, err={stderr}")
-                raise CLIExecutionError(f"Restore of backup failed! Response from process:\n{stderr}")
-        finally:
-            if maybe_proc and maybe_proc.returncode is None:
-                with suppress(Exception):
-                    maybe_proc.kill()
-                    await asyncio.sleep(5)
-            shutil.rmtree(temp_dir)
+        async with TemporaryDirectory() as temp_dir:
+            maybe_proc: Optional[Process] = None
+            try:
+                # extract tar file
+                with tarfile.open(backup_file, "r") as tar:
+                    tar.extractall(temp_dir, members=safe_members_in_tarfile(tar))
+
+                # fmt: off
+                db_conf = cast(CLIDependencies, self.dependencies).config.db
+                process = await asyncio.create_subprocess_exec(
+                    "arangorestore",
+                    "--progress", "false",  # do not show progress
+                    "--include-system-collections", "true",  # graphs are considered a system collection
+                    "--threads", "8",  # default is 2
+                    "--log.level", "error",  # only print error messages
+                    "--input-directory", temp_dir,  # directory to write to
+                    "--overwrite", "true",  # required for existing db collections
+                    "--server.endpoint", db_conf.server.replace("http", "http+tcp"),
+                    "--server.authentication", "false" if db_conf.no_ssl_verify else "true",
+                    "--server.database", db_conf.database,
+                    "--server.username", db_conf.username,
+                    "--server.password", db_conf.password,
+                    "--configuration", "none",
+                    stdout=asyncio.subprocess.PIPE,
+                    stderr=asyncio.subprocess.PIPE,
+                )
+                # fmt: on
+                stdout_b, stderr_b = await process.communicate()
+                maybe_proc = process
+                code = await process.wait()
+                stdout = stdout_b.decode() if stdout_b else ""
+                stderr = stderr_b.decode() if stderr_b else ""
+
+                if code == 0:
+                    log.debug(f"arangorestore: out={stdout}, err={stderr}.")
+                    yield "Database has been restored successfully!"
+                else:
+                    log.error(f"Could not restore backup: {code}. out={stdout}, err={stderr}")
+                    raise CLIExecutionError(f"Restore of backup failed! Response from process:\n{stderr}")
+            finally:
+                if maybe_proc and maybe_proc.returncode is None:
+                    with suppress(Exception):
+                        maybe_proc.kill()
+                        await asyncio.sleep(5)
 
         log.info("Restore process complete. Restart the service.")
         yield "Since all data has changed in the database eventually, this service needs to be restarted!"
         # for testing purposes, we can avoid sys exit
         if str(ctx.env.get("BACKUP_NO_SYS_EXIT", "false")).lower() != "true":
 
             async def wait_and_exit() -> None:
@@ -3586,23 +3603,23 @@
         yield {"name": "resotocore", **info}
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         parts = re.split(r"\s+", arg if arg else "")
         if len(parts) >= 2 and parts[0] == "backup" and parts[1] == "create":
             rest = parts[2:]
 
-            def backup() -> AsyncIterator[str]:
+            def backup() -> AsyncIterator[JsonElement]:
                 return self.create_backup(" ".join(rest) if rest else None)
 
             return CLISource.single(backup, MediaType.FilePath)
 
         elif len(parts) == 3 and parts[0] == "backup" and parts[1] == "restore":
             backup_file = parts[2]
 
-            def restore() -> AsyncIterator[str]:
+            def restore() -> AsyncIterator[JsonElement]:
                 return self.restore_backup(ctx.uploaded_files.get("backup"), ctx)
 
             return CLISource.single(restore, MediaType.Json, [CLIFileRequirement("backup", backup_file)])
         elif len(parts) == 1 and parts[0] == "info":
             return CLISource.single(self.show_system_info)
         else:
             raise CLIParseError(f"system: Can not parse {arg}")
@@ -3638,34 +3655,40 @@
     def info(self) -> str:
         return "Writes the incoming stream of data to a file in the defined format."
 
     def args_info(self) -> ArgsInfo:
         return [ArgInfo(expects_value=True, value_hint="file", help_text="file to write to")]
 
     @staticmethod
-    async def write_result_to_file(in_stream: Stream, file_name: str) -> AsyncIterator[str]:
-        temp_dir: str = tempfile.mkdtemp()
-        path = os.path.join(temp_dir, file_name)
-        try:
+    async def write_result_to_file(in_stream: Stream, file_name: str) -> AsyncIterator[JsonElement]:
+        async with TemporaryDirectory() as temp_dir:
+            path = os.path.join(temp_dir, uuid_str())
             async with aiofiles.open(path, "w") as f:
                 async with in_stream.stream() as streamer:
                     async for out in streamer:
                         if isinstance(out, str):
                             await f.write(out + "\n")
                         else:
                             raise AttributeError("No output format is defined! Consider to use the format command.")
-            yield path
-        finally:
-            shutil.rmtree(temp_dir)
+            yield FilePath.user_local(user=file_name, local=path).json()
+
+    @staticmethod
+    async def already_file_stream(in_stream: Stream, file_name: str) -> AsyncIterator[JsonElement]:
+        async with in_stream.stream() as streamer:
+            async for out in streamer:
+                yield evolve(FilePath.from_path(out), user=Path(file_name)).json()
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         if arg is None:
             raise AttributeError("write requires a filename to write to")
-        defined_arg: str = arg
-        return CLIFlow(lambda in_stream: self.write_result_to_file(in_stream, defined_arg), MediaType.FilePath)
+        if (ex := self.get_previous_command(kwargs)) and ex.action.produces == MediaType.FilePath:
+            fn = self.already_file_stream
+        else:
+            fn = self.write_result_to_file
+        return CLIFlow(lambda in_stream: fn(in_stream, cast(str, arg)), MediaType.FilePath)
 
 
 class TemplatesCommand(CLICommand, PreserveOutputFormat):
     """
     ```shell
     templates
     templates <name_of_template>
@@ -4398,22 +4421,19 @@
             yield cfg if cfg else f"No config with this id: {cfg_id}"
 
         async def delete_config(cfg_id: ConfigId) -> AsyncIterator[str]:
             await self.dependencies.config_handler.delete_config(cfg_id)
             yield f"Config {cfg_id} has been deleted."
 
         async def send_file(content: str) -> AsyncIterator[str]:
-            temp_dir: str = tempfile.mkdtemp()
-            path = os.path.join(temp_dir, "config.yaml")
-            try:
+            async with TemporaryDirectory() as temp_dir:
+                path = os.path.join(temp_dir, "config.yaml")
                 async with aiofiles.open(path, "w") as f:
                     await f.write(content)
                 yield path
-            finally:
-                shutil.rmtree(temp_dir)
 
         async def set_config(cfg_id: ConfigId, updates: List[Tuple[str, JsonElement]]) -> AsyncIterator[JsonElement]:
             cfg = await self.dependencies.config_handler.get_config(cfg_id)
             updated = cfg.config if cfg else {}
             for prop, js in updates:
                 updated = set_value_in_path(js, prop, updated)
             await self.dependencies.config_handler.put_config(ConfigEntity(cfg_id, updated))
@@ -4660,15 +4680,15 @@
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         async def create_certificate(
             common_name: str, dns_names: List[str], ip_addresses: List[str], days_valid: int
         ) -> AsyncIterator[str]:
             key, cert = cast(CLIDependencies, self.dependencies).cert_handler.create_key_and_cert(
                 common_name, dns_names, ip_addresses, days_valid
             )
-            with TemporaryDirectory() as tmpdir:
+            async with TemporaryDirectory() as tmpdir:
                 key_file = os.path.join(tmpdir, f"{common_name}.key")
                 cert_file = os.path.join(tmpdir, f"{common_name}.crt")
                 write_cert_to_file(cert, cert_file, rename=False)
                 write_key_to_file(key, key_file, rename=False)
                 yield key_file
                 yield cert_file
 
@@ -4974,22 +4994,19 @@
             yield await self.dependencies.infra_apps_package_manager.info(app_name, url)
 
         async def app_install(app_name: InfraAppName, url: Optional[str]) -> AsyncIterator[JsonElement]:
             manifest = await self.dependencies.infra_apps_package_manager.install(app_name, url)
             yield f"App {app_name} version {manifest.version} installed successfully"
 
         async def send_file(content: str) -> AsyncIterator[str]:
-            temp_dir: str = tempfile.mkdtemp()
-            path = os.path.join(temp_dir, "manifest.yaml")
-            try:
+            async with TemporaryDirectory() as temp_dir:
+                path = os.path.join(temp_dir, "manifest.yaml")
                 async with aiofiles.open(path, "w") as f:
                     await f.write(content)
                 yield path
-            finally:
-                shutil.rmtree(temp_dir)
 
         async def edit_app(app_name: InfraAppName) -> AsyncIterator[str]:
             # Editing a config is a two-step process:
             # 1) download the config and make it available to edit
             # 2) upload the config file and update the config from content --> update_config
             manifest = await self.dependencies.infra_apps_package_manager.get_manifest(app_name)
             if not manifest:
@@ -5448,24 +5465,21 @@
             snapshot_name = await self.dependencies.graph_manager.snapshot(source, label)
             yield f"Graph {source} snapshoted to {snapshot_name}."
 
         async def graph_delete(graph_name: GraphName) -> AsyncIterator[JsonElement]:
             await self.dependencies.graph_manager.delete(graph_name)
             yield f"Graph {graph_name} deleted."
 
-        async def write_result_to_file(export_lines: AsyncIterator[str], file_name: str) -> AsyncIterator[str]:
-            temp_dir: str = tempfile.mkdtemp()
-            path = os.path.join(temp_dir, file_name)
-            try:
+        async def write_result_to_file(export_lines: AsyncIterator[str], file_name: str) -> AsyncIterator[JsonElement]:
+            async with TemporaryDirectory() as temp_dir:
+                path = os.path.join(temp_dir, uuid_str())
                 async with aiofiles.open(path, "w") as f:
                     async for line in export_lines:
                         await f.write(line + "\n")
-                yield path
-            finally:
-                shutil.rmtree(temp_dir)
+                yield FilePath.user_local(file_name, path).json()
 
         async def graph_export(graph_name: Optional[GraphName], file_name: str) -> AsyncIterator[JsonElement]:
             if not graph_name:
                 graph_name = ctx.graph_name
             lines = cast(CLIDependencies, self.dependencies).graph_manager.export_graph(graph_name)
             return write_result_to_file(lines, file_name)
 
@@ -5540,24 +5554,266 @@
                 [CLIFileRequirement("dump", parsed.file_name)],
             )
 
         else:
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
 
+class DbCommand(CLICommand, PreserveOutputFormat):
+    """
+    ```
+    db sync <db-engine> --host <host> --port <port> --user <user> --password <password> --database <database>
+                   --arg key=value --arg key2=value2
+                   --complete-schema --drop-existing-tables --batch-size <batch-size>
+    ```
+
+    Takes the result of a search expression and synchronizes the data to an SQL database.
+    All matching tables will be updated with the result of the search expression.
+
+    If invoked without a search command, the entire graph will be exported.
+
+    By default, the database tables will be updated only for the data that is returned by the search expression.
+    This behaviour can be overridden by using the `--complete-schema` flag, which will export the entire schema
+    always. This is useful when you want to have a consistent database scheme, no matter which data gets exported.
+
+    The `--drop-existing-tables` can come in handy, if you only want to export a subset of data from a graph and
+    make sure everything from the last export is cleaned up. This flag does not have any effect in combination with
+    `--complete-schema`.
+
+    ## Parameters
+
+    - `db-engine` - The database engine to use. The following engines are supported:
+        - postgresql
+        - mariadb
+        - mysql
+        - sqlite
+        - snowflake
+    - `--host` - The host of the database server.
+    - `--port` - The port of the database server.
+    - `--user` - The user to use for authentication.
+    - `--password` - The password to use for authentication.
+    - `--database` - The database to use.
+    - `--arg` - A key-value pair that will be passed to the connection driver.
+                This property can be used multiple times.
+    - `--batch-size` - The number of rows that will be inserted in a single batch.
+
+    ## Options
+
+    - `--complete-schema` - Export the entire schema, no matter which data gets exported.
+    - `--drop-existing-tables` - Drop all tables that are not part of the current export.
+
+    ## Examples
+
+    ```
+    # Sync the complete graph to a sqlite database
+    > db sync sqlite --database resoto.db --drop-existing
+
+    # Sync the complete graph to a postgresql database
+    > db sync postgresql --host localhost --port 5432 --database resoto --user ci --password bombproof
+
+    # Sync the complete graph to a mariadb database
+    > db sync mariadb --host localhost --port 3306 --user root --password pw --database test
+
+    # Sync the complete graph to a mysql database
+    > db sync mysql --host localhost --port 3306 --user root --password pw --database test
+
+    # Sync the complete graph to a snowflake database
+    > db sync snowflake --host localhost --port 3306 --user root --password pw --database test
+      --arg warehouse=compute_wh --arg role=accountadmin
+
+    # Select a subset of data and sync it to a sqlite database
+    > search --with-edges is(graph_root) -[0:2]-> | db sync sqlite --database resoto.db
+    ```
+    """
+
+    @property
+    def name(self) -> str:
+        return "db"
+
+    def args_info(self) -> ArgsInfo:
+        return {
+            "sync": [
+                ArgInfo(
+                    expects_value=False,
+                    possible_values=["mariadb", "mysql", "postgresql", "sqlite", "snowflake"],
+                    help_text="<db-engine>",
+                ),
+                ArgInfo(name="--host", expects_value=True, help_text="host-name"),
+                ArgInfo(name="--port", expects_value=True, help_text="port"),
+                ArgInfo(name="--user", expects_value=True, help_text="username"),
+                ArgInfo(name="--password", expects_value=True, help_text="password"),
+                ArgInfo(name="--database", expects_value=True, help_text="database"),
+                ArgInfo(name="--arg", can_occur_multiple_times=True, expects_value=True, help_text="key=value"),
+                ArgInfo(name="--batch-size", expects_value=True, help_text="count"),
+            ]
+        }
+
+    def info(self) -> str:
+        return "Synchronizes data to an SQL database."
+
+    async def list_kinds_of_query(
+        self, query: Optional[Query], graph_name: GraphName, model: Model
+    ) -> List[ComplexKind]:
+        assert query is not None, "No query provided, not sure what to synchronize?"
+        assert query.aggregate is None, "Aggregates are not supported for synchronization"
+        db = deps(self).db_access.get_graph_db(graph_name)
+        aggregate_by_kind = Aggregate(
+            [AggregateVariable(AggregateVariableName("reported.kind"), "kind")],
+            [AggregateFunction("sum", 1)],
+        )
+        query = evolve(query, aggregate=aggregate_by_kind)
+        async with await db.search_aggregation(QueryModel(query, model)) as cursor:
+            return [
+                kind
+                async for elem in cursor
+                if (
+                    (kind_name := value_in_path(elem, ["group", "kind"]))
+                    and (kind := model.get(kind_name))
+                    and isinstance(kind, ComplexKind)
+                )
+            ]
+
+    def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
+        in_source_position = kwargs.get("position") == 0
+        db_lookup = dict(mysql="mysql+pymysql", mariadb="mariadb+pymysql")
+
+        async def sync_database_result(p: Namespace, maybe_stream: Optional[Stream]) -> AsyncIterator[JsonElement]:
+            async with TemporaryDirectory() as temp_dir:
+                # optional: path of the output file
+                file_output: Optional[Path] = Path(temp_dir) / "db" if p.db == "sqlite" else None
+                db_string = f"{db_lookup.get(p.db, p.db)}://"
+                if p.user:
+                    db_string += p.user
+                    if p.password:
+                        db_string += f":{p.password}"
+                    db_string += "@"
+                if p.host:
+                    db_string += p.host
+                    if p.port:
+                        db_string += f":{p.port}"
+                if p.database:
+                    database = str(file_output) if file_output is not None else p.database
+                    db_string += f"/{database}"
+                db_string += "?" + "&".join([f"{k}={v}" for pl in p.arg for k, v in pl])
+                db_config = EngineConfig(db_string, p.batch_size)
+
+                sync_fn = partial(database_synchronize, db_config, p.complete_schema, p.drop_existing_tables)
+                if maybe_stream is not None:  # search | db sync
+                    await sync_fn(query=ctx.query, in_stream=maybe_stream)
+                else:
+                    resoto_model = await deps(self).model_handler.load_model(ctx.graph_name)
+                    query = Query(parts=[Part(term=IsTerm(["graph_root"]), navigation=NavigateUntilLeaf)])
+                    graph_db = deps(self).db_access.get_graph_db(ctx.graph_name)
+                    async with await graph_db.search_graph_gen(
+                        QueryModel(query, resoto_model), timeout=timedelta(weeks=200000)
+                    ) as cursor:
+                        await sync_fn(query=query, in_stream=stream.iterate(cursor))
+
+                yield FilePath.user_local(p.database, file_output).json() if file_output else "Database synchronized."
+
+        async def database_synchronize(
+            engine_config: EngineConfig,
+            complete_model: bool,
+            drop_existing_tables: bool,
+            query: Optional[Query],
+            in_stream: Stream,
+        ) -> None:
+            resoto_model = await deps(self).model_handler.load_model(ctx.graph_name)
+
+            if complete_model:
+                complex_kinds = resoto_model.complex_kinds()
+                kinds = list(resoto_model.kinds.values())
+            else:
+                # only export the kinds that are exported by this query
+                complex_kinds = await self.list_kinds_of_query(query, ctx.graph_name, resoto_model)
+                tct = [
+                    ck
+                    for kind in complex_kinds
+                    for ck in kind.transitive_complex_types(with_bases=True, with_properties=True)
+                ]
+                sk = [kind for kind in resoto_model.kinds.values() if isinstance(kind, SimpleKind)]
+                kinds = [*tct, *sk]
+
+            kind_by_name = {k.fqn: from_js(to_js(k), RCKind) for k in kinds}
+            rcm = RCModel(kind_by_name)
+
+            edges = {
+                (kind.fqn, succ)
+                for kind in complex_kinds
+                for succ_lists in kind.successor_kinds.values()
+                for succ in succ_lists
+                if succ in kind_by_name
+            }
+
+            # lookup map for edges: id -> kind. Assumption: when an edge is created, the nodes already passed
+            kind_by_id: Dict[str, str] = {}
+
+            def key_fn(node: Json) -> Union[str, Tuple[str, str]]:
+                assert isinstance(node, dict) and node.get("type") in ("edge", "node"), (
+                    f"Expected a JSON object. Don't know how to handle >{node}<.\n"
+                    "Execute `help db` to get more information on how to use this command."
+                )
+                if node["type"] == "edge":
+                    fr = node["from"]
+                    to = node["to"]
+                    return kind_by_id[fr], kind_by_id[to]
+                else:  # node
+                    kind_by_id[node["id"]] = node["reported"]["kind"]
+                    return cast(str, node["reported"]["kind"])
+
+            async with in_stream.stream() as streamer:
+                batched = BatchStream(streamer, key_fn, engine_config.batch_size, engine_config.batch_size * 10)
+                await update_sql(
+                    engine_config, rcm, batched, edges, swap_temp_tables=True, drop_existing_tables=drop_existing_tables
+                )
+
+        args = arg.split(maxsplit=1) if arg else []
+        if len(args) == 2 and args[0] == "sync":
+            parser = NoExitArgumentParser()
+            parser.add_argument("db", type=str)
+            parser.add_argument("--host", type=str)
+            parser.add_argument("--port", type=int)
+            parser.add_argument("--user", type=str)
+            parser.add_argument("--password", type=str)
+            parser.add_argument("--database", type=str)
+            parser.add_argument("--arg", type=key_value_parser.parse, nargs="+", action="append", default=[])
+            parser.add_argument("--complete-schema", action="store_true")
+            parser.add_argument("--drop-existing-tables", action="store_true")
+            parser.add_argument("--batch-size", type=int, default=1000)
+            parsed_args = parser.parse_args(args_parts_unquoted_parser.parse(args[1]))
+            produces = MediaType.FilePath if parsed_args.db == "sqlite" else MediaType.Json
+            if in_source_position:
+                # in this position we fall back to exporting the whole graph
+                return CLISource.single(
+                    fn=partial(sync_database_result, parsed_args, None),
+                    envelope={CLIEnvelope.no_history: "yes"},
+                    produces=produces,
+                )
+            else:
+                # sync = partial(database_synchronize, db_config, p.complete_schema, p.drop_existing_tables, ctx.query)
+                return CLIFlow(
+                    fn=partial(sync_database_result, parsed_args),
+                    envelope={CLIEnvelope.no_history: "yes"},
+                    produces=produces,
+                )
+        else:
+            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+
+
 def all_commands(d: CLIDependencies) -> List[CLICommand]:
     commands = [
         AggregateCommand(d, "search"),
         AggregateToCountCommand(d, "search"),
         AncestorsPart(d, "search"),
         CertificateCommand(d, "setup", allowed_in_source_position=True),
         ChunkCommand(d, "misc"),
         CleanCommand(d, "action"),
         ConfigsCommand(d, "setup", allowed_in_source_position=True),
         CountCommand(d, "search"),
+        DbCommand(d, "action", allowed_in_source_position=True),
         DescendantsPart(d, "search"),
         DumpCommand(d, "format"),
         EchoCommand(d, "misc", allowed_in_source_position=True),
         EnvCommand(d, "misc", allowed_in_source_position=True),
         ExecuteTaskCommand(d, "action", allowed_in_source_position=True),
         ExecuteSearchCommand(d, "search", allowed_in_source_position=True),
         FlattenCommand(d, "misc"),
```

### Comparing `resotocore-3.5.3/resotocore/cli/dependencies.py` & `resotocore-3.6.0/resotocore/cli/dependencies.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/cli/model.py` & `resotocore-3.6.0/resotocore/cli/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 import inspect
 import json
 from abc import ABC, abstractmethod
 from asyncio import iscoroutine
 from datetime import timedelta
 from enum import Enum
 from functools import reduce
+from pathlib import Path
 from textwrap import dedent
 from typing import Optional, List, Any, Dict, Tuple, Callable, Union, Awaitable, Type, cast, Set, AsyncIterator
 
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import define, field
 from parsy import test_char, string
 from rich.jupyter import JupyterMixin
 
 from resotocore.cli import JsGen, T, Sink
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.core_config import AliasTemplateConfig, AliasTemplateParameterConfig
 from resotocore.error import CLIParseError
-from resotocore.query.template_expander import render_template
+from resotocore.ids import GraphName
 from resotocore.query.model import Query, variable_to_absolute, PathRoot
+from resotocore.query.template_expander import render_template
 from resotocore.types import Json, JsonElement
-from resotocore.ids import GraphName
 from resotocore.util import AccessJson, uuid_str, from_utc, utc, utc_str
 from resotolib.parse_util import l_curly_dp, r_curly_dp
 from resotolib.utils import get_local_tzinfo
 
 
 class MediaType(Enum):
     Json = 1
@@ -55,14 +56,37 @@
 l_or_r_curly_dp = string("{") | string("}")
 
 # use this property name as reference to self when defined via .
 self_name = "self_" + uuid_str()
 
 
 @define(frozen=True)
+class FilePath:
+    user: Path
+    local: Path
+
+    def json(self) -> Json:
+        return {"user_path": str(self.user), "local_path": str(self.local)}
+
+    @staticmethod
+    def from_path(in_path: JsonElement) -> FilePath:
+        if isinstance(in_path, str):
+            p = Path(in_path)
+            return FilePath(Path(p.name), p.expanduser().absolute())
+        elif isinstance(in_path, dict) and "user_path" in in_path and "local_path" in in_path:
+            return FilePath(Path(in_path["user_path"]), Path(in_path["local_path"]).expanduser().absolute())
+        else:
+            raise ValueError(f"Invalid file path: {in_path}")
+
+    @staticmethod
+    def user_local(user: Union[str, Path], local: Union[str, Path]) -> FilePath:
+        return FilePath(Path(user), Path(local).expanduser().absolute())
+
+
+@define(frozen=True)
 class CLIContext:
     env: Dict[str, str] = field(factory=dict)
     uploaded_files: Dict[str, str] = field(factory=dict)  # id -> path
     query: Optional[Query] = None
     query_options: Dict[str, Any] = field(factory=dict)
     commands: List[ExecutableCommand] = field(factory=list)
     console_renderer: Optional[ConsoleRenderer] = None
@@ -322,14 +346,24 @@
     def info(self) -> str:
         pass
 
     @abstractmethod
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         pass
 
+    @staticmethod
+    def get_from(name: str, kind: Type[T], kwargs: Dict[str, Any]) -> Optional[T]:
+        if (kd := kwargs.get(name)) and isinstance(kd, kind):
+            return kd
+        return None
+
+    @staticmethod
+    def get_previous_command(kwargs: Dict[str, Any]) -> Optional[ExecutableCommand]:
+        return CLICommand.get_from("previous_command", ExecutableCommand, kwargs)
+
 
 @define(order=True, hash=True, frozen=True)
 class AliasTemplateParameter:
     name: str
     description: str
     default: Optional[JsonElement] = None
```

### Comparing `resotocore-3.5.3/resotocore/cli/tip_of_the_day.py` & `resotocore-3.6.0/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/config/__init__.py` & `resotocore-3.6.0/resotocore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/config/config_handler_service.py` & `resotocore-3.6.0/resotocore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/config/config_override_service.py` & `resotocore-3.6.0/resotocore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/config/core_config_handler.py` & `resotocore-3.6.0/resotocore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/console_renderer.py` & `resotocore-3.6.0/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/constants.py` & `resotocore-3.6.0/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/core_config.py` & `resotocore-3.6.0/resotocore/core_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -225,86 +225,14 @@
         default=False,
     )
 
 
 def alias_templates() -> List[AliasTemplateConfig]:
     return [
         AliasTemplateConfig(
-            name="discord",
-            info="Send the result of a search to Discord",
-            description=(
-                "Perform a search and send the result to Discord.\n\n"
-                "Discord allows a maximum of 25 items per message. "
-                "If your search result is larger than 25 items, it will be split into multiple messages. "
-                "There are parameters to adjust the information displayed for each resource. "
-                "You can define the title and the message to be displayed.\n\n"
-                "We recommend to define the webhook URL as part of the command configuration. "
-                "This way you do not need to provide it every time you execute the command. "
-                "If you want to use a different webhook URL, you can provide it as a parameter, "
-                "or define different discord commands (e.g. discord-sre, discord-dev)."
-            ),
-            template=(
-                # define the fields to show in the message
-                "jq {name:{{key}}, value:{{value}}} | "
-                # Discord limit: https://discord.com/developers/docs/resources/channel#embed-object-embed-limits
-                "chunk 25 | "
-                # define the Discord webhook JSON
-                'jq {embeds: [{type: "rich", title: "{{title}}", {{#message}}description: "{{message}}",{{/message}} '
-                'fields:., footer:{text: "Message created by Resoto"}}]} | '
-                # call the API
-                "http POST {{webhook}}"
-            ),
-            parameters=[
-                AliasTemplateParameterConfig("key", "Resource field to show as key", ".kind"),
-                AliasTemplateParameterConfig("value", "Resource field to show as value", ".name"),
-                AliasTemplateParameterConfig("message", "Alert message", ""),
-                AliasTemplateParameterConfig("title", "Alert title"),
-                AliasTemplateParameterConfig("webhook", "Discord webhook URL"),
-            ],
-            allowed_in_source_position=False,
-        ),
-        AliasTemplateConfig(
-            name="slack",
-            info="Send the result of a search to Slack",
-            description=(
-                "Perform a search and send the result to Slack.\n\n"
-                "Slack allows a maximum of 25 items per message. "
-                "If your search result is larger than 25 items, it will be split into multiple messages. "
-                "There are parameters to adjust the information displayed for each resource. "
-                "You can define the title and the message to be displayed.\n\n"
-                "We recommend to define the webhook URL as part of the command configuration. "
-                "This way you do not need to provide it every time you execute the command. "
-                "If you want to use a different webhook URL, you can provide it as a parameter, "
-                "or define different slack commands (e.g. slack-sre, slack-dev)."
-            ),
-            template=(
-                # define the fields to show in the message
-                'jq {type: "mrkdwn", text: ("*" + {{key}} + "*: " + {{value}})} | '
-                # Slack limit: https://api.slack.com/reference/block-kit/blocks#actions
-                "chunk 25 | "
-                # define the Slack webhook JSON
-                "jq { blocks: ["
-                '{ type: "header", text: { type: "plain_text", text: "{{title}}" } }, '
-                '{{#message}}{ type: "section", text: { type: "mrkdwn", text: "{{message}}" } }, {{/message}}'
-                '{ type: "section", fields: . }, '
-                '{ type: "context", elements: [ { type: "mrkdwn", text: "Message created by Resoto" } ] } '
-                "] } | "
-                # call the API
-                "http POST {{webhook}}"
-            ),
-            parameters=[
-                AliasTemplateParameterConfig("key", "Resource field to show as key", ".kind"),
-                AliasTemplateParameterConfig("value", "Resource field to show as value", ".name"),
-                AliasTemplateParameterConfig("message", "Alert message", ""),
-                AliasTemplateParameterConfig("title", "Alert title"),
-                AliasTemplateParameterConfig("webhook", "Slack webhook URL"),
-            ],
-            allowed_in_source_position=False,
-        ),
-        AliasTemplateConfig(
             name="jira",
             info="Send the result of a search to Jira",
             description=(
                 "Perform a search and send the result to Jira.\n\n"
                 "If your search result is larger than 25 items, only the first 25 items will be added to the ticket, "
                 "and the remaining items will be dropped.\n\n"
                 "Note that invoking this command will always create a new ticket since JIRA does not have any "
@@ -589,15 +517,15 @@
 
 @define()
 class RuntimeConfig(ConfigObject):
     kind: ClassVar[str] = f"{ResotoCoreRoot}_runtime_config"
     debug: bool = field(default=False, metadata={"description": "Enable debug logging and exception tracing."})
     log_level: str = field(default="info", metadata={"description": "Log level (default: info)"})
     plantuml_server: str = field(
-        default="http://plantuml.resoto.org:8080",
+        default="https://plantuml.resoto.org",
         metadata={"description": "PlantUML server URI for UML image rendering."},
     )
     start_collect_on_subscriber_connect: bool = field(
         default=False,
         metadata={"description": "Start the collect workflow, when the first handling actor connects to the system."},
     )
     usage_metrics: bool = field(
@@ -819,14 +747,17 @@
     del_value_in_path(adapted, "api.ui_path")
 
     # 3.5 -> 3.6: web_port -> https_port
     if web_port := value_in_path(cfg, "api.web_port"):
         set_value_in_path(web_port, "api.https_port", adapted)
         del_value_in_path(adapted, "api.web_port")
 
+    if value_in_path(cfg, "runtime.plantuml_server") == "http://plantuml.resoto.org:8080":
+        set_value_in_path("https://plantuml.resoto.org", "runtime.plantuml_server", adapted)
+
     return {ResotoCoreRoot: adapted}
 
 
 def migrate_command_config(cmd_config: Json) -> Optional[Json]:
     config = from_js(cmd_config.get(ResotoCoreCommandsRoot), CustomCommandsConfig)
     existing_commands = {tpl.name: tpl for tpl in config.commands}
     adjusted = False
```

### Comparing `resotocore-3.5.3/resotocore/db/__init__.py` & `resotocore-3.6.0/resotocore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/arango_query.py` & `resotocore-3.6.0/resotocore/db/arango_query.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/arangodb_extensions.py` & `resotocore-3.6.0/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/arangodb_functions.py` & `resotocore-3.6.0/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/async_arangodb.py` & `resotocore-3.6.0/resotocore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/configdb.py` & `resotocore-3.6.0/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/db_access.py` & `resotocore-3.6.0/resotocore/db/db_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/deferred_edge_db.py` & `resotocore-3.6.0/resotocore/db/deferred_edge_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/entitydb.py` & `resotocore-3.6.0/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/graphdb.py` & `resotocore-3.6.0/resotocore/db/graphdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         pass
 
     @abstractmethod
     async def create_update_schema(self) -> None:
         pass
 
     @abstractmethod
-    async def copy_graph(self, to_graph: GraphName) -> "GraphDB":
+    async def copy_graph(self, to_graph: GraphName, to_snapshot: bool = False) -> "GraphDB":
         pass
 
 
 class ArangoGraphDB(GraphDB):
     def __init__(self, db: AsyncArangoDB, name: GraphName, adjust_node: AdjustNode, config: GraphUpdateConfig) -> None:
         super().__init__()
         self._name = name
@@ -907,15 +907,15 @@
         root_node = {"_key": "root", "id": "root", Section.reported: root_data, "kinds": ["graph_root"], "hash": sha}
         try:
             await self.db.insert(self.vertex_name, root_node)
         except Exception:
             # ignore if the root not is already created
             return None
 
-    async def create_update_schema(self, init_with_data: bool = True) -> None:
+    async def create_update_schema(self, init_with_data: bool = True, to_snapshot: bool = False) -> None:
         db = self.db
 
         async def create_update_graph(
             graph_name: GraphName, vertex_name: str, edge_name: str
         ) -> Tuple[Graph, VertexCollection, EdgeCollection]:
             graph = db.graph(graph_name) if await db.has_graph(graph_name) else await db.create_graph(graph_name)
             vertex_collection = (
@@ -926,18 +926,15 @@
             edge_collection = (
                 graph.edge_collection(edge_name)
                 if await db.has_edge_definition(graph_name, edge_name)
                 else await db.create_edge_definition(graph_name, edge_name, [vertex_name], [vertex_name])
             )
             return graph, vertex_collection, edge_collection
 
-        def create_update_collection_indexes(
-            nodes: VertexCollection, progress: StandardCollection, node_history: StandardCollection
-        ) -> None:
-            # node indexes ------
+        def create_node_indexes(nodes: VertexCollection) -> None:
             node_idxes = {idx["name"]: idx for idx in cast(List[Json], nodes.indexes())}
             # this index will hold all the necessary data to query for an update (index only query)
             if "update_nodes_ref_id" not in node_idxes:
                 log.info(f"Add index update_nodes_ref_id on {nodes.name}")
                 nodes.add_persistent_index(
                     # if _key would be defined as first property, the optimizer would use it in case
                     # a simple id() query would be executed.
@@ -948,14 +945,16 @@
 
             if "kinds_id_name_ctime" not in node_idxes:
                 nodes.add_persistent_index(
                     ["kinds[*]", "reported.id", "reported.name", "reported.ctime"],
                     sparse=False,
                     name="kinds_id_name_ctime",
                 )
+
+        def create_update_collection_indexes(progress: StandardCollection, node_history: StandardCollection) -> None:
             # progress indexes ------
             progress_idxes = {idx["name"]: idx for idx in cast(List[Json], progress.indexes())}
             if "parent_nodes" not in progress_idxes:
                 log.info(f"Add index parent_nodes on {progress.name}")
                 progress.add_persistent_index(["parent_nodes[*]"], name="parent_nodes")
             if "root_nodes" not in progress_idxes:
                 log.info(f"Add index root_nodes on {progress.name}")
@@ -1027,35 +1026,43 @@
                 )
 
         for edge_type in EdgeTypes.all:
             edge_type_name = self.edge_collection(edge_type)
             await create_update_graph(self.name, self.vertex_name, edge_type_name)
 
         vertex = db.graph(self.name).vertex_collection(self.vertex_name)
-        in_progress = await create_collection(self.in_progress)
-        node_history_collection = await create_collection(self.node_history)
-        create_update_collection_indexes(vertex, in_progress, node_history_collection)
+
+        if to_snapshot:
+            # since the snapshots are immutable, we don't in_progress or node_history collections
+            # we only create the indexes on the vertex collection
+            create_node_indexes(vertex)
+        else:
+            in_progress = await create_collection(self.in_progress)
+            node_history_collection = await create_collection(self.node_history)
+            create_node_indexes(vertex)
+            create_update_collection_indexes(in_progress, node_history_collection)
+
         for edge_type in EdgeTypes.all:
             edge_collection = db.graph(self.name).edge_collection(self.edge_collection(edge_type))
             create_update_edge_indexes(edge_collection)
 
         await create_update_views(vertex)
         if init_with_data:
             await self.insert_genesis_data()
 
-    async def copy_graph(self, to_graph: GraphName) -> GraphDB:
+    async def copy_graph(self, to_graph: GraphName, to_snapshot: bool = False) -> GraphDB:
         if await self.db.has_graph(to_graph):
             raise ValueError(f"Graph {to_graph} already exists")
 
         new_graph_db = ArangoGraphDB(db=self.db, name=to_graph, adjust_node=self.node_adjuster, config=self.config)
 
         # collection creation can't be a part of a transaction so we do that first
         # we simply reuse the existing create_update_schema method but do not insert any genesis data
-        async def create_new_collections(new_db: ArangoGraphDB) -> None:
-            await new_db.create_update_schema(init_with_data=False)
+        async def create_new_collections(new_db: ArangoGraphDB, to_snapshot: bool) -> None:
+            await new_db.create_update_schema(init_with_data=False, to_snapshot=to_snapshot)
 
         # we want to have a consistent snapshot view of the graph
         async def copy_data() -> None:
             old_vertex = self.vertex_name
             old_default_edge = self.edge_collection(EdgeTypes.default)
             old_delete_edge = self.edge_collection(EdgeTypes.delete)
 
@@ -1106,15 +1113,15 @@
             """
             await self.db.execute_transaction(
                 tx,
                 read=[old_vertex, old_default_edge, old_delete_edge],
                 write=[new_vertex, new_default_edge, new_delete_edge],
             )
 
-        await create_new_collections(new_graph_db)
+        await create_new_collections(new_graph_db, to_snapshot=to_snapshot)
         await copy_data()
 
         return cast(GraphDB, new_graph_db)
 
     @staticmethod
     def db_edge_key(from_node: str, to_node: str) -> str:
         return str(uuid.uuid5(uuid.NAMESPACE_DNS, f"{from_node}:{to_node}"))
@@ -1360,13 +1367,13 @@
 
     async def to_query(self, query_model: QueryModel, with_edges: bool = False) -> Tuple[str, Json]:
         return await self.real.to_query(query_model, with_edges)
 
     async def create_update_schema(self) -> None:
         await self.real.create_update_schema()
 
-    async def copy_graph(self, to_graph: GraphName) -> GraphDB:
+    async def copy_graph(self, to_graph: GraphName, to_snapshot: bool = False) -> GraphDB:
         await self.event_sender.core_event(
             CoreEvent.GraphCopied,
             {"graph": self.graph_name, "to_graph": to_graph},
         )
-        return await self.real.copy_graph(to_graph)
+        return await self.real.copy_graph(to_graph, to_snapshot=to_snapshot)
```

### Comparing `resotocore-3.5.3/resotocore/db/model.py` & `resotocore-3.6.0/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/packagedb.py` & `resotocore-3.6.0/resotocore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/runningtaskdb.py` & `resotocore-3.6.0/resotocore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/db/system_data_db.py` & `resotocore-3.6.0/resotocore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/dependencies.py` & `resotocore-3.6.0/resotocore/dependencies.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/error.py` & `resotocore-3.6.0/resotocore/error.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/graph_manager/graph_manager.py` & `resotocore-3.6.0/resotocore/graph_manager/graph_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,42 +130,49 @@
             if graph_time <= time:
                 return graph
 
         # nothing found
         return None
 
     async def copy(
-        self, source: GraphName, destination: GraphName, replace_existing: bool, validate_name: bool = True
+        self,
+        source: GraphName,
+        destination: GraphName,
+        replace_existing: bool,
+        validate_name: bool = True,
+        to_snapshot: bool = False,
     ) -> GraphName:
         if not self.lock:
             raise RuntimeError("GraphManager has not been started")
 
         async with self.lock:
             if not await self.db_access.db.has_graph(source):
                 raise ValueError(f"Source graph {source} does not exist")
 
             if await self.db_access.db.has_graph(destination):
                 if replace_existing:
                     await self.delete(destination)
                 else:
                     raise ValueError(f"Destination graph {destination} already exists")
-            return await self._copy_graph(source, destination, validate_name)
+            return await self._copy_graph(source, destination, validate_name, to_snapshot)
 
-    async def _copy_graph(self, source: GraphName, destination: GraphName, validate_name: bool = True) -> GraphName:
+    async def _copy_graph(
+        self, source: GraphName, destination: GraphName, validate_name: bool = True, to_snapshot: bool = False
+    ) -> GraphName:
         destination = GraphName(_compress_timestamps(destination))
 
         if validate_name:
             check_graph_name(destination)
 
         if not await self.db_access.db.has_graph(source):
             raise ValueError(f"Source graph {source} does not exist")
 
         source_db = self.db_access.get_graph_db(source, no_check=True)
 
-        await source_db.copy_graph(destination)
+        await source_db.copy_graph(destination, to_snapshot)
 
         source_model_db = await self.db_access.get_graph_model_db(source)
         destination_model_db = await self.db_access.get_graph_model_db(destination)
 
         model_kinds = [kind async for kind in source_model_db.all()]
         await destination_model_db.update_many(model_kinds)
 
@@ -177,15 +184,15 @@
 
         if source.startswith("snapshot-"):
             raise ValueError("Can not snapshot a snapshot")
 
         time = utc_str(timestamp, date_format=UTC_Date_Format_short)
         check_graph_name(label)
         snapshot_name = GraphName(f"snapshot-{source}-{label}-{time}")
-        return await self.copy(source, snapshot_name, replace_existing=False, validate_name=False)
+        return await self.copy(source, snapshot_name, replace_existing=False, validate_name=False, to_snapshot=True)
 
     async def delete(self, graph_name: GraphName) -> None:
         await self.db_access.delete_graph(graph_name)
         await self.db_access.delete_graph_model(graph_name)
 
     async def export_graph(self, graph_name: GraphName) -> AsyncIterator[str]:
         if not await self.db_access.db.has_graph(graph_name):
```

### Comparing `resotocore-3.5.3/resotocore/infra_apps/local_runtime.py` & `resotocore-3.6.0/resotocore/infra_apps/local_runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/infra_apps/manifest.py` & `resotocore-3.6.0/resotocore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/infra_apps/package_manager.py` & `resotocore-3.6.0/resotocore/infra_apps/package_manager.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/infra_apps/runtime.py` & `resotocore-3.6.0/resotocore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.6.0/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1037.51967a2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1037.51967a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1079.cdbaf67.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1079.cdbaf67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1084.4cd1c89.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1084.4cd1c89.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1113.23c9417.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1113.23c9417.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1125.129d070.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1125.129d070.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1163.ac28297.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1163.ac28297.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1221.c51249a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1221.c51249a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1245.be46619.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1245.be46619.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1261.199fc1d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1261.199fc1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1272.f334098.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1272.f334098.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1278.0524a4a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt` & `resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1290.3981211.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1290.3981211.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1295.46e72b8.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1295.46e72b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1310.23bbe67.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1310.23bbe67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1320.21effe3.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1320.21effe3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1325.f76267c.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1325.f76267c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1408.7461890.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1408.7461890.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1440.a9e7ea1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1440.a9e7ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1483.616d9ab.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1483.616d9ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1489.e50b6d4.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1489.e50b6d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1507.5705605.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1507.5705605.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/152.525d460.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/152.525d460.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1520.4e2eb21.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1520.4e2eb21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1555.e188f3f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1555.e188f3f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1559.7c89925.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1559.7c89925.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/160.5f28731.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/160.5f28731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1603.370a2a6.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1603.370a2a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1644.0e49167.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1644.0e49167.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1667.f0afb2b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1667.f0afb2b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1687.27f1ad6.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1687.27f1ad6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1725.f151c33.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1725.f151c33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1767.c8c2f26.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1767.c8c2f26.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1806.1aaf66b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1806.1aaf66b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1838.1202b16.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1838.1202b16.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1909.28a2def.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1909.28a2def.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/1989.88d258f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/1989.88d258f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2030.1562cc6.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2030.1562cc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2047.baed97b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2047.baed97b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2099.f4b6fcd.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2099.f4b6fcd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2118.5b65f70.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2118.5b65f70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/213.5769e57.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/213.5769e57.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2161.dcb27b8.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2161.dcb27b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2169.635c88e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2169.635c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/217.90d10e2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/217.90d10e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2212.72be094.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2212.72be094.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2287.997c38e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt` & `resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2303.9ff8710.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2303.9ff8710.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2319.6b4cbb7.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2319.6b4cbb7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2329.4c5ca6d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2329.4c5ca6d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2351.fbd96d8.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2351.fbd96d8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2358.d5cf7c8.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2358.d5cf7c8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2359.6451c3e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2359.6451c3e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/237.f765e77.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/237.f765e77.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2384.71782be.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2384.71782be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/240.cddc46b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/240.cddc46b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2431.648d237.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2431.648d237.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2546.1f48267.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2546.1f48267.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2557.75e9da2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2557.75e9da2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/261.5f53c0e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/261.5f53c0e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2629.c0e1cd6.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2629.c0e1cd6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2788.46acc8a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2788.46acc8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2834.942acc6.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2834.942acc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2887.47ba752.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2887.47ba752.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2956.8880209.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2956.8880209.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/2973.2a51dc4.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/2973.2a51dc4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3004.255e79c.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3004.255e79c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/302.8bcc38f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/302.8bcc38f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3037.70ee38d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3037.70ee38d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3042.7cfad84.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3042.7cfad84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3051.34fac68.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3051.34fac68.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3122.2289fca.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3122.2289fca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3151.10ef4de.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3151.10ef4de.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/316.c850a76.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/316.c850a76.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3196.4e35a17.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3196.4e35a17.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3265.a80440a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3265.a80440a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3277.9c04e75.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3277.9c04e75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/330.126fa98.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/330.126fa98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3392.29fe6b9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3392.29fe6b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3413.480a49d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3413.480a49d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3444.47d5ea1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3444.47d5ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3469.7d14d0b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3469.7d14d0b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3546.fee1bd7.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3546.fee1bd7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/362.6716970.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/362.6716970.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3708.410d087.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3708.410d087.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3850.903abc2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt` & `resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3880.bd39dce.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3880.bd39dce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3970.236586f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3970.236586f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3976.58893b9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt` & `resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/3979.385527e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/3979.385527e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/400.d72234b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/400.d72234b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4018.1a35967.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4018.1a35967.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/406.9b7af92.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/406.9b7af92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4117.a8107fd.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4117.a8107fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4182.e2430f9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4182.e2430f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4191.02bbea8.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4191.02bbea8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4197.53ab10b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4197.53ab10b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4206.a5f8bb0.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4206.a5f8bb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4207.0d0580b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4207.0d0580b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4262.bb73457.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4262.bb73457.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4298.5ee510c.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4298.5ee510c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/44.0cfa785.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt` & `resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4410.e4a25d3.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4410.e4a25d3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4466.64d23d1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4466.64d23d1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/451.d9683ad.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/451.d9683ad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4535.34b060a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4535.34b060a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4565.43bdb91.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4565.43bdb91.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4569.f374f9d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4569.f374f9d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4615.eb5d40a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4615.eb5d40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4658.090d4a9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4658.090d4a9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4690.3dd4096.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4690.3dd4096.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4715.e7690b9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4715.e7690b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4749.46ebbb2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4749.46ebbb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4750.56c06ab.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4750.56c06ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4856.2d7415f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4856.2d7415f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4875.375150e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4875.375150e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/489.b981dea.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/489.b981dea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/490.c2624d4.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/490.c2624d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4905.667bf33.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4905.667bf33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4931.430433b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4931.430433b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/4942.b96c164.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/4942.b96c164.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5016.dd2fe83.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5016.dd2fe83.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5072.733a1b5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5072.733a1b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/509.6448878.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/509.6448878.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5096.8ed0d8e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5096.8ed0d8e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5126.eecad7a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5126.eecad7a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5129.1ba4763.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5129.1ba4763.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5153.763d8fa.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5153.763d8fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5155.06b4ea9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5155.06b4ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5193.e9f6866.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5193.e9f6866.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5213.3e1a360.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5213.3e1a360.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5227.8c8acd8.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5227.8c8acd8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5238.1751cc3.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5238.1751cc3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/528.2262cb0.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/528.2262cb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5292.79d4aba.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5292.79d4aba.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5437.31236f7.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5437.31236f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5489.848a8cf.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5489.848a8cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5508.317fca3.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5508.317fca3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/554.ac98303.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/554.ac98303.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/555.2cd31dd.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/555.2cd31dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5573.ebcdb93.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5573.ebcdb93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5666.c5e5324.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5666.c5e5324.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5710.70d0b1d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5710.70d0b1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5747.94ad626.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5747.94ad626.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/582.21b8e7d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/582.21b8e7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5823.5045bdb.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5823.5045bdb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5851.30b7b2a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5851.30b7b2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5878.32d92fa.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5878.32d92fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5880.68f975b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5880.68f975b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5955.88508f7.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5955.88508f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/5971.88c5642.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/5971.88c5642.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6080.aa0ff24.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6080.aa0ff24.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/61.2808a0d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/61.2808a0d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6136.b8ba2b2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6136.b8ba2b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6141.9831d58.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6141.9831d58.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6475.6037fbb.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6475.6037fbb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6493.d796aa5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6493.d796aa5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6556.b3d9293.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6556.b3d9293.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6571.2c8884e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6571.2c8884e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6576.3ea568e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6576.3ea568e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6591.94ed352.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6591.94ed352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6612.1632879.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6612.1632879.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6623.ae3b3cc.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6623.ae3b3cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6664.2160109.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6664.2160109.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6747.47be7f5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6747.47be7f5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6748.be68f5f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6748.be68f5f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6870.7940288.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6870.7940288.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6879.c8367a5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6879.c8367a5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6898.9bbc12a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6898.9bbc12a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6952.f68b818.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6952.f68b818.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6985.321ad92.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6985.321ad92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6993.32cf9a6.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6993.32cf9a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/6997.b06fe71.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/6997.b06fe71.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7041.d4f561e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7041.d4f561e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7058.805c88e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7058.805c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7174.6c45206.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7174.6c45206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7334.8859b1b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7334.8859b1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7359.6ee65ec.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7359.6ee65ec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7364.195178b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7364.195178b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7380.58a4413.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7380.58a4413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7427.f9c2017.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7427.f9c2017.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7463.18fd278.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7463.18fd278.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7509.1e0189e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7509.1e0189e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7526.1a303e5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7526.1a303e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7537.1323a15.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7537.1323a15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7692.33d5169.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7692.33d5169.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7746.5908d29.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7746.5908d29.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7808.1d582a2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7808.1d582a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/783.c156751.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/783.c156751.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7858.2386e4d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7858.2386e4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/7941.01ea680.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/7941.01ea680.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8005.c5ad7b2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8005.c5ad7b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8028.39e2fa1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8028.39e2fa1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8061.cc62561.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8061.cc62561.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8101.cf46d02.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8101.cf46d02.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/812.9b0e86e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/812.9b0e86e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/816.c8050f2.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/816.c8050f2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8165.b2c3285.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8165.b2c3285.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8232.a578bf9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8232.a578bf9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/824.8678196.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/824.8678196.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8270.89fe7e1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8270.89fe7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/833.9cc6653.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/833.9cc6653.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8370.8f855e5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8370.8f855e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8373.96b0b3a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8373.96b0b3a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8389.ffe031f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8389.ffe031f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8412.1528057.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8412.1528057.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8427.4923f43.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8427.4923f43.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8542.027afdc.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8542.027afdc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8594.0112f03.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8594.0112f03.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8656.d5b8e92.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8656.d5b8e92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8685.d78bdab.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8685.d78bdab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8698.9817d75.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8698.9817d75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8732.9320f73.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8732.9320f73.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8785.cf4fe95.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8785.cf4fe95.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8828.77c71d0.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8828.77c71d0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8883.80c7b63.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8883.80c7b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8976.3816942.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8976.3816942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/8990.2a453cf.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/8990.2a453cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9035.1e45c1b.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9035.1e45c1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9053.45b77fc.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9053.45b77fc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9077.fefb6ca.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9077.fefb6ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9128.b8fa6f0.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9128.b8fa6f0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9156.0cefbd3.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9156.0cefbd3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9170.0023587.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9170.0023587.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9196.315f9f9.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9196.315f9f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9198.9971d70.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9198.9971d70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/920.d15c177.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/920.d15c177.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9253.0b31caa.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9253.0b31caa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9266.bacd0dd.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9266.bacd0dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9307.c3a00ed.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9307.c3a00ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9321.869e413.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9321.869e413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9344.ba0abcf.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9344.ba0abcf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9382.9014799.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9382.9014799.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9440.1b10b8f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9440.1b10b8f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9464.79e6ac5.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9464.79e6ac5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9502.9a24831.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9502.9a24831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9507.1e6cc5d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9507.1e6cc5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9602.62bf0f1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9602.62bf0f1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9621.e2e8b5d.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9621.e2e8b5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9622.ccab065.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9622.ccab065.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9626.a178bd0.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9626.a178bd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9647.ed91993.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9647.ed91993.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9657.bc5c60e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9657.bc5c60e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/97.ad126b0.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/97.ad126b0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9712.796a0a1.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9712.796a0a1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9737.7dc8f98.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9737.7dc8f98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9777.0b8a504.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9777.0b8a504.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9793.6d63a85.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9793.6d63a85.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9806.652c162.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9806.652c162.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9865.2e3db6f.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9865.2e3db6f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/989.bcca86a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/989.bcca86a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9943.f3f35c7.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9943.f3f35c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9958.25c8c06.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9958.25c8c06.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/9960.64cd61e.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/9960.64cd61e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/build.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/close.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/json.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/python.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/react.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/service-worker-b2fb40a.js` & `resotocore-3.6.0/resotocore/jupyterlite/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.6.0/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.6.0/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/config-utils.js` & `resotocore-3.6.0/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.6.0/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.6.0/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.6.0/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/index.html` & `resotocore-3.6.0/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.6.0/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.6.0/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.6.0/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/lab/index.html` & `resotocore-3.6.0/resotocore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.6.0/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/lab/package.json` & `resotocore-3.6.0/resotocore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.6.0/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/package.json` & `resotocore-3.6.0/resotocore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/jupyterlite/service-worker-b2fb40a.js` & `resotocore-3.6.0/resotocore/jupyterlite/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/message_bus.py` & `resotocore-3.6.0/resotocore/message_bus.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/metrics.py` & `resotocore-3.6.0/resotocore/metrics.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/model/adjust_node.py` & `resotocore-3.6.0/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/model/db_updater.py` & `resotocore-3.6.0/resotocore/model/db_updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from resotocore.db.graphdb import GraphDB
 from resotocore.db.model import GraphUpdate
 from resotocore.db.deferred_edge_db import PendingDeferredEdges
 from resotocore.dependencies import db_access, setup_process, reset_process_start_method
 from resotocore.error import ImportAborted
 from resotocore.model.graph_access import GraphBuilder
 from resotocore.model.model import Model
+from resotocore.model.model_handler import ModelHandlerDB, ModelHandler
 from resotocore.types import Json
 from resotocore.ids import TaskId, GraphName
 from resotocore.util import utc, uuid_str, shutdown_process
 
 log = logging.getLogger(__name__)
 
 
@@ -143,14 +144,17 @@
             shutdown_process(0)
         elif isinstance(nxt, MergeGraph):
             log.debug("Graph read into memory")
             builder.check_complete()
             graphdb = db.get_graph_db(nxt.graph)
             outer_edge_db = db.pending_deferred_edge_db
             _, result = await graphdb.merge_graph(builder.graph, model, nxt.change_id, nxt.is_batch)
+            # sizes of model entries have been adjusted during the merge. Update the model in the db.
+            model_handler = ModelHandlerDB(db, "")
+            await model_handler.update_model(graphdb.name, list(model.kinds.values()))
             if nxt.task_id and builder.deferred_edges:
                 await outer_edge_db.update(PendingDeferredEdges(nxt.task_id, utc(), nxt.graph, builder.deferred_edges))
                 log.debug(f"Updated {len(builder.deferred_edges)} pending outer edges for collect task {nxt.task_id}")
             return result
 
     async def setup_and_merge(self) -> GraphUpdate:
         sender = InMemoryEventSender()
@@ -175,14 +179,15 @@
             self.write_queue.put(Result(repr(ex)))
             log.error(f"Update process interrupted. Preemptive Exit. {ex}", exc_info=ex)
             shutdown_process(1)
 
 
 async def merge_graph_process(
     db: GraphDB,
+    model_handler: ModelHandler,
     event_sender: AnalyticsEventSender,
     config: CoreConfig,
     content: AsyncGenerator[Union[bytes, Json], None],
     max_wait: timedelta,
     maybe_batch: Optional[str],
     task_id: Optional[TaskId],
 ) -> GraphUpdate:
@@ -233,14 +238,15 @@
         async with chunked.stream() as streamer:
             async for lines in streamer:
                 if not await send_to_child(ReadElement(lines, task_id)):
                     # in case the child is dead, we should stop
                     break
         await send_to_child(MergeGraph(db.name, change_id, maybe_batch is not None, task_id))
         result = await task  # wait for final result
+        await model_handler.load_model(db.name, force=True)  # reload model to get the latest changes
         return result
     finally:
         if task is not None and not task.done():
             task.cancel()
         if not result:
             # make sure the change is aborted in case of transaction
             log.info(f"Abort update manually: {change_id}")
```

### Comparing `resotocore-3.5.3/resotocore/model/graph_access.py` & `resotocore-3.6.0/resotocore/model/graph_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,37 @@
 import hashlib
 import json
 import logging
 import re
 from collections import namedtuple, defaultdict
 from functools import reduce
 from typing import Optional, Generator, Any, Dict, List, Set, Tuple, Union
-from attrs import define
 
+from attrs import define
 from networkx import DiGraph, MultiDiGraph, all_shortest_paths, is_directed_acyclic_graph
 
-from resotocore.model.model import Model, Kind, AnyKind, ComplexKind, ArrayKind, DateTimeKind, DictionaryKind
-from resotocore.model.resolve_in_graph import GraphResolver, NodePath, ResolveProp
-from resotocore.types import Json, EdgeType
 from resotocore.ids import NodeId
-from resotocore.util import utc, utc_str, value_in_path, set_value_in_path, value_in_path_get
+from resotocore.model.model import (
+    Model,
+    Kind,
+    AnyKind,
+    ComplexKind,
+    ArrayKind,
+    DateTimeKind,
+    DictionaryKind,
+    StringKind,
+    Property,
+    SimpleKind,
+    DateKind,
+    DurationKind,
+)
+from resotocore.model.resolve_in_graph import GraphResolver, NodePath, ResolveProp
 from resotocore.model.typed_model import from_js
-
+from resotocore.types import Json, EdgeType, JsonElement
+from resotocore.util import utc, utc_str, value_in_path, set_value_in_path, value_in_path_get
 
 log = logging.getLogger(__name__)
 
 # This version is used when the content hash of a node is computed.
 # All computed hashes will be invalidated, by incrementing the version.
 # This can be used, if computed values should be recomputed for all imported data.
 ContentHashVersion = 3
@@ -158,14 +170,46 @@
                 parse_selector(js["from_selector"]),
                 parse_selector(js["to_selector"]),
                 js.get("edge_type", EdgeTypes.default),
             )
         else:
             raise AttributeError(f"Format not understood! Got {json.dumps(js)} which is neither vertex nor edge.")
 
+    def __update_property_size(self, kind: Kind, element: JsonElement) -> None:
+        def prop_size(prop: Property, pk: Kind, part: JsonElement) -> None:
+            if part is None:
+                pass
+            elif isinstance(pk, (StringKind, DateTimeKind, DateKind, DurationKind)) and isinstance(part, str):
+                str_len = len(part)
+                if prop.metadata is None:
+                    prop.metadata = {}
+                size = prop.metadata.get("len", 0)
+                prop.metadata["len"] = max(size, str_len)
+            elif isinstance(pk, SimpleKind):
+                pass
+            elif isinstance(pk, ArrayKind) and isinstance(part, list) and isinstance(pk.inner, StringKind):
+                for elem in part:
+                    prop_size(prop, pk.inner, elem)
+            elif isinstance(pk, ArrayKind) and isinstance(part, list):
+                for elem in part:
+                    self.__update_property_size(pk.inner, elem)
+            elif isinstance(pk, DictionaryKind) and isinstance(part, dict) and isinstance(pk.value_kind, StringKind):
+                for elem in part.values():
+                    prop_size(prop, pk.value_kind, elem)
+            elif isinstance(pk, DictionaryKind) and isinstance(part, dict):
+                for k, v in part.items():
+                    self.__update_property_size(pk.key_kind, k)
+                    self.__update_property_size(pk.value_kind, v)
+            elif isinstance(pk, ComplexKind) and isinstance(part, dict):
+                for cp, cpk in pk.all_props_with_kind():
+                    prop_size(cp, cpk, part.get(cp.name, None))
+
+        if isinstance(kind, ComplexKind) and isinstance(element, dict):
+            prop_size(Property("root", kind.fqn), kind, element)
+
     def add_node(
         self,
         node_id: NodeId,
         reported: Json,
         desired: Optional[Json] = None,
         metadata: Optional[Json] = None,
         search: Optional[str] = None,
@@ -189,14 +233,16 @@
             hash=sha,
             kind=kind,
             kinds=list(kind.kind_hierarchy()),
             kinds_set=kind.kind_hierarchy(),
             flat=flat,
             replace=replace | metadata.get("replace", False) is True if metadata else False,
         )
+        # update property sizes
+        self.__update_property_size(kind, reported)
 
     def add_edge(self, from_node: str, to_node: str, edge_type: EdgeType) -> None:
         self.edges += 1
         key = GraphAccess.edge_key(from_node, to_node, edge_type)
         self.graph.add_edge(from_node, to_node, key, edge_type=edge_type)
 
     def store_deferred_connection(self, from_selector: NodeSelector, to_selector: NodeSelector, edge_type: str) -> None:
```

### Comparing `resotocore-3.5.3/resotocore/model/json_schema.py` & `resotocore-3.6.0/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/model/model.py` & `resotocore-3.6.0/resotocore/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import json
 import re
 import sys
 import textwrap
 from abc import ABC, abstractmethod
-from functools import lru_cache
-
-from attrs import define
 from datetime import datetime, timezone, date
+from functools import lru_cache
 from json import JSONDecodeError
-from typing import Union, Any, Optional, Callable, Type, Sequence, Dict, List, Set, cast, Tuple, Iterable
+from typing import Union, Any, Optional, Callable, Type, Sequence, Dict, List, Set, cast, Tuple, Iterable, TypeVar
 
 import yaml
+from attrs import define
 from dateutil.parser import parse
 from jsons import set_deserializer, set_serializer
 from networkx import MultiDiGraph
 from parsy import regex, string, Parser
 
-from resotolib.core.model_check import check_overlap_for
-from resotolib.durations import duration_parser, DurationRe
-from resotolib.parse_util import make_parser, variable_dp_backtick, dot_dp
-from resotolib.utils import is_env_var_string
+from resotocore.compat import remove_suffix
 from resotocore.model.transform_kind_convert import converters
 from resotocore.model.typed_model import from_js, to_js
 from resotocore.types import Json, JsonElement, ValidationResult, ValidationFn, EdgeType
 from resotocore.util import if_set, utc, duration, first
-from resotocore.compat import remove_suffix
+from resotolib.core.model_check import check_overlap_for
+from resotolib.durations import duration_parser, DurationRe
+from resotolib.parse_util import make_parser, variable_dp_backtick, dot_dp
+from resotolib.utils import is_env_var_string
+
+T = TypeVar("T")
 
 
 def check_type_fn(t: type, type_name: str) -> ValidationFn:
     def check_type(x: Any) -> ValidationResult:
         if isinstance(x, t):
             return None
         else:
@@ -72,29 +73,36 @@
     A synthetic property does not exist in the underlying data model.
     It is defined by a function on an existing other property.
     Example: age is a duration defined on ctime which is a datetime.
              the function is age=now-ctime.
     """
 
 
-@define(order=True, hash=True, frozen=True)
+@define(order=True, hash=True, eq=True)
 class Property:
     name: str
     kind: str
     required: bool = False
     synthetic: Optional[SyntheticProperty] = None
     description: Optional[str] = None
     metadata: Optional[Json] = None
 
     def __attrs_post_init__(self) -> None:
         assert self.synthetic is None or not self.required, "Synthetic properties can not be required!"
 
     def resolve(self, model: Dict[str, Kind]) -> Kind:
         return Property.parse_kind(self.kind, model)
 
+    def meta(self, name: str, clazz: Type[T]) -> Optional[T]:
+        meta = self.metadata
+        return v if meta is not None and (v := meta.get(name)) is not None and isinstance(v, clazz) else None
+
+    def meta_get(self, name: str, clazz: Type[T], default: T) -> T:
+        return self.meta(name, clazz) or default
+
     @staticmethod
     def parse_kind(name: str, model: Dict[str, Kind]) -> Kind:
         def kind_by_name(kind_name: str) -> Kind:
             if kind_name not in model:
                 raise AttributeError(f"Property kind is not known: {kind_name}. Have you registered it?")
             return model[kind_name]
 
@@ -103,15 +111,15 @@
         dict_string_parser = string("dictionary[")
         comma_parser = regex("\\s*,\\s*")
         bracket_r = string("]")
 
         @make_parser
         def array_parser() -> Parser:
             inner = yield dictionary_parser | simple_kind_parser
-            brackets = yield bracket_parser.times(1, float("inf"))
+            brackets = yield bracket_parser.times(1, cast(int, float("inf")))
             return ArrayKind.mk_array(inner, len(brackets))
 
         @make_parser
         def dictionary_parser() -> Parser:
             yield dict_string_parser
             key_kind = cast(Kind, (yield simple_kind_parser))
             yield comma_parser
@@ -202,14 +210,17 @@
 class Kind(ABC):
     def __init__(self, fqn: str):
         self.fqn = fqn
 
     def __eq__(self, other: object) -> bool:
         return self.__dict__ == other.__dict__ if isinstance(other, Kind) else False
 
+    def __hash__(self) -> int:
+        return hash(self.fqn)
+
     def coerce(self, value: JsonElement, **kwargs: bool) -> JsonElement:
         coerced = self.coerce_if_required(value, **kwargs)
         return coerced or value
 
     @abstractmethod
     def coerce_if_required(self, value: JsonElement, **kwargs: bool) -> Optional[JsonElement]:
         """
@@ -822,14 +833,15 @@
         self.allow_unknown_props = allow_unknown_props
         self.successor_kinds = successor_kinds or {}
         self.aggregate_root = aggregate_root
         self.metadata = metadata or {}
         self.__prop_by_name = {prop.name: prop for prop in properties}
         self.__resolved = False
         self.__resolved_kinds: Dict[str, Tuple[Property, Kind]] = {}
+        self.__resolved_bases: Dict[str, ComplexKind] = {}
         self.__all_props: List[Property] = list(self.properties)
         self.__resolved_hierarchy: Set[str] = {fqn}
         self.__property_by_path: List[ResolvedProperty] = []
         self.__synthetic_props: List[ResolvedProperty] = []
 
     def resolve(self, model: Dict[str, Kind]) -> None:
         if not self.__resolved:
@@ -848,14 +860,15 @@
 
             # resolve the hierarchy
             if not self.is_root():
                 for base_name in self.bases:
                     base: Kind = model[base_name]
                     base.resolve(model)
                     if isinstance(base, ComplexKind):
+                        self.__resolved_bases[base_name] = base
                         self.__resolved_kinds.update(base.__resolved_kinds)
                         self.__all_props = base.__all_props + self.__all_props
                         self.__prop_by_name = {prop.name: prop for prop in self.__all_props}
                         self.__resolved_hierarchy.update(base.__resolved_hierarchy)
 
             # property path -> kind
             self.__property_by_path = ComplexKind.resolve_properties(self, model)
@@ -866,14 +879,16 @@
         if isinstance(other, ComplexKind):
             return (
                 self.fqn == other.fqn
                 and self.properties == other.properties
                 and self.bases == other.bases
                 and self.allow_unknown_props == other.allow_unknown_props
                 and self.successor_kinds == other.successor_kinds
+                and self.aggregate_root == other.aggregate_root
+                and self.metadata == other.metadata
             )
         else:
             return False
 
     def __contains__(self, name: str) -> bool:
         return name in self.__prop_by_name
 
@@ -895,20 +910,56 @@
 
     def kind_hierarchy(self) -> Set[str]:
         return self.__resolved_hierarchy
 
     def resolved_properties(self) -> List[ResolvedProperty]:
         return self.__property_by_path
 
+    def resolved_bases(self) -> Dict[str, ComplexKind]:
+        return self.__resolved_bases
+
     def all_props(self) -> List[Property]:
         return self.__all_props
 
+    def all_props_with_kind(self) -> List[Tuple[Property, Kind]]:
+        return [(a, self.property_kind_of(a.name, any_kind)) for a in self.__all_props]
+
     def synthetic_props(self) -> List[ResolvedProperty]:
         return self.__synthetic_props
 
+    def transitive_complex_types(self, with_bases: bool = True, with_properties: bool = True) -> List[ComplexKind]:
+        result: Dict[str, ComplexKind] = {}
+        visited: Set[str] = set()
+
+        def add_bases(ck: ComplexKind) -> None:
+            for fqn, base in ck.resolved_bases().items():
+                result[fqn] = base
+
+        def add_props(ck: ComplexKind) -> None:
+            for prop in ck.resolved_properties():
+                if isinstance(prop.kind, ComplexKind):
+                    result[prop.kind.fqn] = prop.kind
+                    in_hierarchy(prop.kind)
+
+        def in_hierarchy(ck: ComplexKind) -> None:
+            if ck.fqn in visited:
+                return
+            visited.add(ck.fqn)
+            result[ck.fqn] = ck
+            if with_bases:
+                add_bases(ck)
+            if with_properties:
+                add_props(ck)
+            for base in ck.resolved_bases().values():
+                if not base.is_root():
+                    in_hierarchy(base)
+
+        in_hierarchy(self)
+        return list(result.values())
+
     def check_valid(self, obj: JsonElement, **kwargs: bool) -> ValidationResult:
         if isinstance(obj, dict):
             coerced = self.coerce_if_required(obj, **kwargs)
             for name, value in (coerced or obj).items():
                 known = self.__resolved_kinds.get(name, None)
                 if known:
                     prop, kind = known
@@ -1035,15 +1086,15 @@
                 return remove_suffix(result, "\n")
             elif isinstance(e, list):
                 return "[]"
             elif is_env_var_string(e):
                 return str(e)
             elif isinstance(e, str):
                 # if the string contains a newline, try a literal block, else a quoted string
-                return safe_string(e, indent, "|" if "\n" in e else "'")
+                return safe_string(e, indent, "|" if ("\n" in e and len(e) > 1) else "'")
             elif e is None:
                 return "null"
             elif e is True:
                 return "true"
             elif e is False:
                 return "false"
             else:
@@ -1292,17 +1343,35 @@
                 handle_complex(kind.value_kind)
 
         return graph
 
     def update_kinds(self, kinds: List[Kind], check_overlap: bool = True) -> Model:
         # Create a list of kinds that have changed to the existing model
         to_update = []
+
+        def merge_metadata(update: ComplexKind, existing: ComplexKind) -> None:
+            """
+            Merge metadata of complex kinds and their properties.
+            ATM: we only merge the len property of string kinds.
+            """
+            existing_props: Dict[str, Property] = {prop.name: prop for prop in existing.properties}
+            for prop in update.properties:
+                existing_prop = existing_props.get(prop.name)
+                meta = prop.metadata or {}
+                # take the maximum of all lengths ever seen
+                if existing_prop is not None and existing_prop.meta("len", int) is not None:
+                    meta["len"] = max(prop.meta_get("len", int, 0), existing_prop.meta_get("len", int, 0))
+                    prop.metadata = meta
+
         for elem in kinds:
-            existing_props = self.kinds.get(elem.fqn)
-            if elem.fqn not in predefined_kinds_by_name and (not existing_props or existing_props != elem):
+            existing_elem = self.kinds.get(elem.fqn)
+            # merge old and new metadata for complex kinds and their properties
+            if isinstance(elem, ComplexKind) and isinstance(existing_elem, ComplexKind):
+                merge_metadata(elem, existing_elem)
+            if elem.fqn not in predefined_kinds_by_name and (not existing_elem or existing_elem != elem):
                 to_update.append(elem)
 
         # Short circuit, if there are no changes
         if not to_update:
             return self
 
         def update_is_valid(from_kind: Kind, to_kind: Kind) -> None:
```

### Comparing `resotocore-3.5.3/resotocore/model/model_handler.py` & `resotocore-3.6.0/resotocore/model/model_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from functools import reduce
 from typing import Optional, List, Set, Callable, Dict, Iterator
 
 from plantuml import PlantUML
 
 from resotocore.async_extensions import run_async
 from resotocore.db.db_access import DbAccess
-from resotocore.types import EdgeType
 from resotocore.ids import GraphName
 from resotocore.model.model import Model, Kind, ComplexKind, Property
+from resotocore.types import EdgeType
 from resotocore.util import exist
 
 log = logging.getLogger(__name__)
 
 
 class ModelHandler(ABC):
     @abstractmethod
-    async def load_model(self, graph_name: GraphName) -> Model:
+    async def load_model(self, graph_name: GraphName, *, force: bool = False) -> Model:
         pass
 
     @abstractmethod
     async def uml_image(
         self,
         graph_name: GraphName,
         output: str = "svg",
@@ -93,16 +93,16 @@
 class ModelHandlerDB(ModelHandler):
     def __init__(self, db_access: DbAccess, plantuml_server: str):
         self.db_access = db_access
         self.plantuml_server = plantuml_server
         self.__loaded_model: Dict[GraphName, Model] = {}
         self.default_legacy_graph_name = GraphName("resoto")
 
-    async def load_model(self, graph_name: GraphName) -> Model:
-        if model := self.__loaded_model.get(graph_name):
+    async def load_model(self, graph_name: GraphName, *, force: bool = False) -> Model:
+        if not force and (model := self.__loaded_model.get(graph_name)) is not None:
             return model
         else:
             graph_model_db = await self.db_access.get_graph_model_db(graph_name)
             model_db = self.db_access.get_model_db()
             # check the new implementation for the kinds
             model_kinds = [kind async for kind in graph_model_db.all()]
             # if nothing found and the graph is the legacy default one, look in the legacy implementation
```

### Comparing `resotocore-3.5.3/resotocore/model/resolve_in_graph.py` & `resotocore-3.6.0/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/model/transform_kind_convert.py` & `resotocore-3.6.0/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/model/typed_model.py` & `resotocore-3.6.0/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/query/__init__.py` & `resotocore-3.6.0/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/query/model.py` & `resotocore-3.6.0/resotocore/query/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/query/query_parser.py` & `resotocore-3.6.0/resotocore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/query/template_expander.py` & `resotocore-3.6.0/resotocore/query/template_expander.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import json
 from abc import abstractmethod
-from typing import Any, ByteString, Union, Iterable, Tuple, List, Optional, cast
+from typing import Any, Union, Iterable, Tuple, List, Optional, cast
 
 from parsy import string, Parser, regex, any_char
 from ustache import default_getter, default_virtuals, render, PropertyGetter, TagsTuple, default_tags
 
 from resotocore.error import NoSuchTemplateError
 from resotocore.query import query_parser, QueryParser
 from resotocore.query.model import Query, Expandable, Template, PathRoot
@@ -206,16 +206,16 @@
     :param template: the template string.
     :param props: the properties to populate.
     :param more_props: additional property maps
     :param tags: the tags to identify the template
     :return: the rendered template string.
     """
 
-    def json_stringify(data: Any, text: bool = False) -> Union[bytes, ByteString]:
-        if isinstance(data, ByteString) and not text:
+    def json_stringify(data: Any, text: bool = False) -> Union[bytes, bytearray]:
+        if isinstance(data, (bytes, bytearray)) and not text:
             return data
         elif isinstance(data, str):
             return data.encode()
         elif isinstance(data, (list, dict)):
             return json.dumps(data).encode()
         else:
             return f"{data}".encode()
```

### Comparing `resotocore-3.5.3/resotocore/query/template_expander_service.py` & `resotocore-3.6.0/resotocore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/report/__init__.py` & `resotocore-3.6.0/resotocore/report/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     categories: List[str]
     severity: ReportSeverity
     risk: str
     detect: Dict[str, str]
     remediation: Remediation
     default_values: Optional[Json] = None
     url: Optional[str] = None
-    related: List[str] = field(factory=list)
+    related: Optional[List[str]] = None
 
     def environment(self, values: Json) -> Json:
         return {**self.default_values, **values} if self.default_values else values
 
     def to_node(self) -> Json:
         reported = to_js(self)
         return dict(id=self.id, kind="report_check", type="node", reported=reported)
```

### Comparing `resotocore-3.5.3/resotocore/report/benchmark_renderer.py` & `resotocore-3.6.0/resotocore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/report/inspector_service.py` & `resotocore-3.6.0/resotocore/report/inspector_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/report/report_config.py` & `resotocore-3.6.0/resotocore/report/report_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     )
     remediation: Remediation = field(metadata={"description": "Remediation action for the check."})
     default_values: Optional[Json] = field(
         default=None,
         metadata={"description": "Default values for the check. Will be merged with the values from the config."},
     )
     url: Optional[str] = field(default=None, metadata={"description": "URL that documents the check."})
-    related: List[str] = field(factory=list, metadata={"description": "List of related checks."})
+    related: Optional[List[str]] = field(default=None, metadata={"description": "List of related checks."})
     internal_notes: Optional[str] = field(default=None, metadata={"description": "Internal notes for the check."})
 
 
 @define
 class ReportCheckCollectionConfig:
     kind: ClassVar[str] = CheckConfigRoot
     provider: str = field(metadata={"description": "Cloud provider of all checks."})
```

### Comparing `resotocore-3.5.3/resotocore/static/api-doc.yaml` & `resotocore-3.6.0/resotocore/static/api-doc.yaml`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.6.0/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.6.0/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/check_template.json` & `resotocore-3.6.0/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/static/resoto_logo_and_text.svg` & `resotocore-3.6.0/resotocore/static/resoto_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/__init__.py` & `resotocore-3.6.0/resotocore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/model.py` & `resotocore-3.6.0/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/scheduler.py` & `resotocore-3.6.0/resotocore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.6.0/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/subscribers.py` & `resotocore-3.6.0/resotocore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/task_description.py` & `resotocore-3.6.0/resotocore/task/task_description.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/task/task_handler.py` & `resotocore-3.6.0/resotocore/task/task_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/templates/base.html` & `resotocore-3.6.0/resotocore/templates/base.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/templates/create_first_user.html` & `resotocore-3.6.0/resotocore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/templates/login.html` & `resotocore-3.6.0/resotocore/templates/login.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/types.py` & `resotocore-3.6.0/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/user/__init__.py` & `resotocore-3.6.0/resotocore/user/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/user/user_management.py` & `resotocore-3.6.0/resotocore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/util.py` & `resotocore-3.6.0/resotocore/util.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/validator.py` & `resotocore-3.6.0/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/web/api.py` & `resotocore-3.6.0/resotocore/web/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     CLIContext,
     CLICommand,
     InternalPart,
     WorkerCustomCommand,
     CLI,
     AliasTemplate,
     InfraAppAlias,
+    FilePath,
 )
 from resotocore.config import ConfigHandler, ConfigValidation, ConfigEntity
 from resotocore.console_renderer import ConsoleColorSystem, ConsoleRenderer
 from resotocore.core_config import CoreConfig
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import GraphDB, HistoryChange
 from resotocore.db.model import QueryModel
@@ -916,32 +917,32 @@
         log.info("Received merge_graph request")
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         task_id: Optional[TaskId] = None
         if tid := request.headers.get("Resoto-Worker-Task-Id"):
             task_id = TaskId(tid)
         db = self.db.get_graph_db(graph_id)
         it = self.to_line_generator(request)
-        info = await merge_graph_process(
-            db, self.event_sender, self.config, it, self.config.graph_update.merge_max_wait_time(), None, task_id
-        )
+        mh = self.model_handler
+        max_wait = self.config.graph_update.merge_max_wait_time()
+        info = await merge_graph_process(db, mh, self.event_sender, self.config, it, max_wait, None, task_id)
         return web.json_response(to_js(info))
 
     async def update_merge_graph_batch(self, request: Request) -> StreamResponse:
         log.info("Received put_sub_graph_batch request")
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         task_id: Optional[TaskId] = None
         if tid := request.headers.get("Resoto-Worker-Task-Id"):
             task_id = TaskId(tid)
         db = self.db.get_graph_db(graph_id)
         rnd = "".join(SystemRandom().choice(string.ascii_letters) for _ in range(12))
         batch_id = request.query.get("batch_id", rnd)
         it = self.to_line_generator(request)
-        info = await merge_graph_process(
-            db, self.event_sender, self.config, it, self.config.graph_update.merge_max_wait_time(), batch_id, task_id
-        )
+        mh = self.model_handler
+        max_wait = self.config.graph_update.merge_max_wait_time()
+        info = await merge_graph_process(db, mh, self.event_sender, self.config, it, max_wait, batch_id, task_id)
         return web.json_response(to_json(info), headers={"BatchId": batch_id})
 
     async def list_batches(self, request: Request) -> StreamResponse:
         graph_db = self.db.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
         batch_updates = await graph_db.list_in_progress_updates()
         return web.json_response([b for b in batch_updates if b.get("is_batch")])
 
@@ -1281,24 +1282,31 @@
         async for data in result_gen:
             await writer.write(data + cr)
         await response.write_eof()
         return response
 
     @staticmethod
     async def multi_file_response(
-        cmd_line: ParsedCommandLine, results: AsyncIterator[str], boundary: str, response: StreamResponse
+        cmd_line: ParsedCommandLine, results: AsyncIterator[JsonElement], boundary: str, response: StreamResponse
     ) -> None:
         async for file_path in results:
-            path = Path(file_path)
-            if not (path.exists() and path.is_file()):
+            path = FilePath.from_path(file_path)
+            if not (path.local.is_file()):
                 raise HTTPNotFound(text=f"No file with this path: {file_path}")
-            with open(path.absolute(), "rb") as content:
+            with open(path.local, "rb") as content:
+                headers = cmd_line.envelope
+                # only add path header if the user path is more than a file name
+                if path.user.name != str(path.user):
+                    headers = {**headers, "file-path": str(path.user)}
                 with MultipartWriter(boundary=boundary) as mp:
                     pl = BufferedReaderPayload(
-                        content, content_type="application/octet-stream", filename=path.name, headers=cmd_line.envelope
+                        content,
+                        content_type="application/octet-stream",
+                        filename=path.user.name,
+                        headers=headers,
                     )
                     mp.append_payload(pl)
                     await mp.write(response, close_boundary=False)
 
     @staticmethod
     async def close_multi_part_response(response: StreamResponse, boundary: str) -> None:
         with MultipartWriter(boundary=boundary) as mp:
```

### Comparing `resotocore-3.5.3/resotocore/web/auth.py` & `resotocore-3.6.0/resotocore/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/web/certificate_handler.py` & `resotocore-3.6.0/resotocore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/web/content_renderer.py` & `resotocore-3.6.0/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/web/directives.py` & `resotocore-3.6.0/resotocore/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/web/tsdb.py` & `resotocore-3.6.0/resotocore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore/worker_task_queue.py` & `resotocore-3.6.0/resotocore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/resotocore.egg-info/PKG-INFO` & `resotocore-3.6.0/resotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.5.3
+Version: 3.6.0
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,15 +205,15 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://resoto.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: extra
 Provides-Extra: test
 License-File: LICENSE
 
 # `resotocore`
 Resoto core graph platform
```

### Comparing `resotocore-3.5.3/resotocore.egg-info/SOURCES.txt` & `resotocore-3.6.0/resotocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/__init__.py` & `resotocore-3.6.0/tests/resotocore/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/analytics/posthog_test.py` & `resotocore-3.6.0/tests/resotocore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/analytics/recurrent_events_test.py` & `resotocore-3.6.0/tests/resotocore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/cli/cli_test.py` & `resotocore-3.6.0/tests/resotocore/cli/cli_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,23 @@
     FlattenCommand,
     UniqCommand,
     EchoCommand,
     AggregateToCountCommand,
     PredecessorsPart,
     DumpCommand,
 )
-from resotocore.cli.model import ParsedCommands, ParsedCommand, CLIContext, CLI, InfraAppAlias
+from resotocore.cli.model import (
+    ParsedCommands,
+    ParsedCommand,
+    CLIContext,
+    CLI,
+    InfraAppAlias,
+    CLICommand,
+    ExecutableCommand,
+)
 from resotocore.error import CLIParseError
 from resotocore.model.graph_access import EdgeTypes
 from resotocore.util import utc
 
 
 def test_strip() -> None:
     assert strip_quotes("'test'") == "test"
@@ -246,7 +254,16 @@
 
     assert_command("echo 'f\\boo'", "echo", "'f\boo'")  # <bs>b --> \b
     assert_command("echo 'f\\noo'", "echo", "'f\noo'")  # <bs>n --> \n
     assert_command("echo 'f\\\\oo'", "echo", "'f\\\\oo'")  # <bs><bs> --> <bs><bs>
     assert_command("echo 'f\\u00a7oo'", "echo", "'f§oo'")  # <bs>unicode_number --> character
     assert_command("echo 'f\\\"oo'", "echo", "'f\\\"oo'")  # <bs>" --> <bs>"
     assert_command("echo 'f\\'oo'", "echo", "'f\\'oo'")  # <bs>' --> <bs>'
+
+
+def test_get_kwargs() -> None:
+    ec = ExecutableCommand(None, None, None, None)  # type: ignore
+    d = {"a": 1, "b": "str", "previous_command": ec}
+    assert CLICommand.get_previous_command(d) == ec
+    assert CLICommand.get_from("a", int, d) == 1
+    assert CLICommand.get_from("a", str, d) is None
+    assert CLICommand.get_from("c", str, d) is None
```

### Comparing `resotocore-3.5.3/tests/resotocore/cli/command_test.py` & `resotocore-3.6.0/tests/resotocore/cli/command_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
+import asyncio
 import json
 import logging
 import os
+import sqlite3
 from datetime import timedelta
 from functools import partial
-from pathlib import Path
-from typing import List, Dict, Optional, Any, Tuple, Type, TypeVar, cast
+from typing import List, Dict, Optional, Any, Tuple, Type, TypeVar, cast, Callable, Set
 
 import pytest
 import yaml
 from _pytest.logging import LogCaptureFixture
 from aiohttp import ClientTimeout
 from aiohttp.web import Request
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import evolve
 from pytest import fixture
-import asyncio
 
 from resotocore import version
 from resotocore.cli import is_node
 from resotocore.cli.cli import CLIService
 from resotocore.cli.command import HttpCommand, JqCommand, AggregateCommand, all_commands
 from resotocore.cli.dependencies import CLIDependencies
-from resotocore.cli.model import CLIContext, WorkerCustomCommand, CLI
+from resotocore.cli.model import CLIContext, WorkerCustomCommand, CLI, FilePath
 from resotocore.cli.tip_of_the_day import generic_tips
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.db.graphdb import ArangoGraphDB
 from resotocore.db.jobdb import JobDb
 from resotocore.error import CLIParseError
 from resotocore.graph_manager.graph_manager import GraphManager
 from resotocore.ids import InfraAppName, GraphName
@@ -479,15 +479,15 @@
         awaitable, info = await cli.dependencies.forked_tasks.get()
         assert (await awaitable)["id"] in ["root", "collector"]  # type:ignore
 
 
 @pytest.mark.asyncio
 async def test_kinds_command(cli: CLI, foo_model: Model) -> None:
     result = await cli.execute_cli_command("kind", stream.list)
-    for kind in ["account", "bla", "child", "cloud", "inner", "parent", "region", "some_complex"]:
+    for kind in ["account", "bla", "child", "cloud", "parent", "region", "some_complex"]:
         assert kind in result[0]
     result = await cli.execute_cli_command("kind foo", stream.list)
     assert result[0][0] == {
         "name": "foo",
         "bases": ["base"],
         "properties": {
             "age": "duration",
@@ -651,18 +651,18 @@
 @pytest.mark.skipif(not_in_path("arangodump"), reason="requires arangodump to be in path")
 @pytest.mark.asyncio
 async def test_system_backup_command(cli: CLI) -> None:
     async def check_backup(res: Stream) -> None:
         async with res.stream() as streamer:
             only_one = True
             async for s in streamer:
-                assert isinstance(s, str)
-                assert os.path.exists(s)
-                # backup should have size between 30k and 500k (adjust size if necessary)
-                assert 30000 < os.path.getsize(s) < 500000
+                path = FilePath.from_path(s)
+                assert path.local.exists()
+                # backup should have size between 30k and 1500k (adjust size if necessary)
+                assert 30000 < path.local.stat().st_size < 1500000
                 assert only_one
                 only_one = False
 
     await cli.execute_cli_command("system backup create", check_backup)
 
 
 @pytest.mark.asyncio
@@ -677,15 +677,16 @@
 @pytest.mark.asyncio
 async def test_system_restore_command(cli: CLI, tmp_directory: str) -> None:
     backup = os.path.join(tmp_directory, "backup")
 
     async def move_backup(res: Stream) -> None:
         async with res.stream() as streamer:
             async for s in streamer:
-                os.rename(s, backup)
+                path = FilePath.from_path(s)
+                os.rename(path.local, backup)
 
     await cli.execute_cli_command("system backup create", move_backup)
     ctx = CLIContext(uploaded_files={"backup": backup})
     restore = await cli.execute_cli_command(f"BACKUP_NO_SYS_EXIT=true system backup restore {backup}", stream.list, ctx)
     assert restore == [
         [
             "Database has been restored successfully!",
@@ -760,30 +761,32 @@
 
 @pytest.mark.asyncio
 async def test_write_command(cli: CLI) -> None:
     async def check_file(res: Stream, check_content: Optional[str] = None) -> None:
         async with res.stream() as streamer:
             only_one = True
             async for s in streamer:
-                assert isinstance(s, str)
-                p = Path(s)
-                assert p.exists() and p.is_file()
-                assert 1 < p.stat().st_size < 100000
-                assert p.name.startswith("write_test")
+                fp = FilePath.from_path(s)
+                assert fp.local.exists() and fp.local.is_file()
+                assert 1 < fp.local.stat().st_size < 100000
+                assert fp.user.name.startswith("write_test")
                 assert only_one
                 only_one = False
                 if check_content:
-                    with open(s, "r") as file:
+                    with open(fp.local, "r") as file:
                         data = file.read()
                         assert data == check_content
 
     # result can be read as json
     await cli.execute_cli_command("search all limit 3 | format --json | write write_test.json ", check_file)
     # result can be read as yaml
     await cli.execute_cli_command("search all limit 3 | format --yaml | write write_test.yaml ", check_file)
+    # throw an exception
+    with pytest.raises(Exception):
+        await cli.execute_cli_command("echo hello | write", stream.list)  # missing filename
     # write enforces unescaped output.
     env = {"now": utc_str()}  # fix the time, so that replacements will stay equal
     truecolor = CLIContext(console_renderer=ConsoleRenderer(80, 25, ConsoleColorSystem.truecolor, True), env=env)
     monochrome = CLIContext(console_renderer=ConsoleRenderer.default_renderer(), env=env)
     # Make sure, that the truecolor output is different from monochrome output
     mono_out = await cli.execute_cli_command("help", stream.list, monochrome)
     assert await cli.execute_cli_command("help", stream.list, truecolor) != mono_out
@@ -846,59 +849,14 @@
     requests.clear()
     await cli.execute_cli_command(f"search is(bla) limit 1 | http --backoff-base 0.001 :{port}/fail", stream.list)
     # 1 request + 3 retries => 4 requests
     assert len(requests) == 4
 
 
 @pytest.mark.asyncio
-async def test_discord_alias(cli: CLI, echo_http_server: Tuple[int, List[Tuple[Request, Json]]]) -> None:
-    port, requests = echo_http_server
-    result = await cli.execute_cli_command(
-        f'search is(bla) | discord --webhook "http://localhost:{port}/success" --title test --message "test message"',
-        stream.list,
-    )
-    # 100 times bla, discord allows 25 fields -> 4 requests
-    assert result == [["4 requests with status 200 sent."]]
-    assert len(requests) == 4
-    print(requests[0][1])
-    assert requests[0][1] == {
-        "embeds": [
-            {
-                "type": "rich",
-                "title": "test",
-                "description": "test message",
-                "fields": [{"name": "bla", "value": "yes or no"} for _ in range(0, 25)],
-                "footer": {"text": "Message created by Resoto"},
-            }
-        ],
-    }
-
-
-@pytest.mark.asyncio
-async def test_slack_alias(cli: CLI, echo_http_server: Tuple[int, List[Tuple[Request, Json]]]) -> None:
-    port, requests = echo_http_server
-    result = await cli.execute_cli_command(
-        f'search is(bla) | slack --webhook "http://localhost:{port}/success" --title test --message "test message"',
-        stream.list,
-    )
-    # 100 times bla, discord allows 25 fields -> 4 requests
-    assert result == [["4 requests with status 200 sent."]]
-    assert len(requests) == 4
-    print(requests[0][1])
-    assert requests[0][1] == {
-        "blocks": [
-            {"type": "header", "text": {"type": "plain_text", "text": "test"}},
-            {"type": "section", "text": {"type": "mrkdwn", "text": "test message"}},
-            {"type": "section", "fields": [{"type": "mrkdwn", "text": "*bla*: yes or no"} for _ in range(0, 25)]},
-            {"type": "context", "elements": [{"type": "mrkdwn", "text": "Message created by Resoto"}]},
-        ],
-    }
-
-
-@pytest.mark.asyncio
 async def test_jira_alias(cli: CLI, echo_http_server: Tuple[int, List[Tuple[Request, Json]]]) -> None:
     port, requests = echo_http_server
     result = await cli.execute_cli_command(
         f'search is(bla) | jira --url "http://localhost:{port}/success" --title test --message "test message" --username test --token test --project_id 10000 --reporter_id test',
         stream.list,
     )
     assert result == [["1 requests with status 200 sent."]]
@@ -1100,32 +1058,32 @@
 
     # install a package
     assert "installed successfully" in (await execute("apps install cleanup-untagged", str))[0]
     manifest = await package_manager.get_manifest(InfraAppName("cleanup-untagged"))
     assert manifest is not None
     assert manifest.name == "cleanup-untagged"
     # install discord app
-    assert "installed successfully" in (await execute("apps install discordapp", str))[0]
+    assert "installed successfully" in (await execute("apps install discord", str))[0]
 
     # info about the app
     info_json = (await execute("apps info cleanup-untagged", Json))[0]
     assert info_json["name"] == "cleanup-untagged"
 
     # run the app
     result = await execute("apps run cleanup-untagged --dry-run", str)
     assert result[0].startswith("search /metadata.protected == false and /metadata.phantom")
 
     # run the app with stdin
     result = await execute("echo foo | apps run cleanup-untagged --dry-run", str)
     assert result[0].startswith("search /metadata.protected == false and /metadata.phantom")
 
     # run discord app with stdin
-    result = await execute("search is(graph_root) | apps run discordapp --title foo --dry-run", str)
+    result = await execute("search is(graph_root) | apps run discord --title foo --dry-run", str)
     assert "http POST https://discordapp.com" in result[0]
-    await execute("apps uninstall discordapp", str)
+    await execute("apps uninstall discord", str)
 
     # update the app
     assert (
         "App cleanup-untagged updated sucessfully to the latest version"
         in (await execute("apps update cleanup-untagged", str))[0]
     )
 
@@ -1284,21 +1242,103 @@
     assert set(graph_names) == {"ns", "graphtest", "graphtest3"}
 
     dump = os.path.join(tmp_directory, "dump")
 
     async def move_dump(res: Stream) -> None:
         async with res.stream() as streamer:
             async for s in streamer:
-                os.rename(s, dump)
+                fp = FilePath.from_path(s)
+                os.rename(fp.local, dump)
 
     # graph export works
     await cli.execute_cli_command("graph export graphtest dump", move_dump)
 
     ctx = CLIContext(uploaded_files={"dump": dump})
 
     # graph import works too
     await cli.execute_cli_command("graph import graphtest_import graphtest.backup", stream.list, ctx)
     assert await graph_manager.list(GraphName("graphtest_import")) == [GraphName("graphtest_import")]
 
     # clean up
     await graph_manager.delete(GraphName("graphtest3"))
     await graph_manager.delete(GraphName("graphtest_import"))
+
+
+@pytest.mark.asyncio
+async def test_db(cli: CLI) -> None:
+    db_file = "test_db"
+
+    async def sync_and_check(
+        cmd: str,
+        *,
+        expected_table: Optional[Callable[[str, int], bool]] = None,
+        expected_tables: Optional[Set[str]] = None,
+        expected_table_count: Optional[int] = None,
+    ) -> str:
+        result: List[str] = []
+
+        async def check(in_: Stream) -> None:
+            async with in_.stream() as streamer:
+                async for s in streamer:
+                    path = FilePath.from_path(s)
+                    # open sqlite database
+                    conn = sqlite3.connect(path.local)
+                    c = conn.cursor()
+                    tables = {
+                        row[0] for row in c.execute("SELECT tbl_name FROM sqlite_master WHERE type='table'").fetchall()
+                    }
+                    if expected_tables is not None:
+                        assert tables == expected_tables
+                    if expected_table_count is not None:
+                        assert len(tables) == expected_table_count
+                    if expected_table is not None:
+                        for table in tables:
+                            count = c.execute(f"SELECT COUNT(*) FROM {table}").fetchone()[0]
+                            assert expected_table(table, count), f"Table {table} has {count} rows"
+                    c.close()
+                    conn.close()
+                    result.append(s)
+
+        await cli.execute_cli_command(cmd, check)
+        assert len(result) == 1
+        return result[0]
+
+    # search | db sync
+    await sync_and_check(
+        f"search --with-edges is(foo) -[0:1]-> | db sync sqlite --database {db_file}",
+        expected_table=lambda table, count: count > 0 if not table.startswith("link_") else True,
+        expected_tables={"foo", "bla", "link_bla_bla", "link_foo_bla"},
+    )
+
+    # db sync synchronizes the whole graph
+    await sync_and_check(
+        f"db sync sqlite --database {db_file}",
+        expected_table=lambda table, count: count > 0 if not table.startswith("link_") else True,
+        expected_tables={"foo", "bla", "link_bla_bla", "link_foo_bla"},
+    )
+
+    # db sync with complete schema synchronizes the whole graph and created tables for all kinds even if they are empty
+    await sync_and_check(f"db sync sqlite --complete-schema --database {db_file}", expected_table_count=11)
+
+    # support write after db sync (not required for simple files, but we want to support s3 etc. in the future)
+    path_result = await sync_and_check(f"db sync sqlite --database {db_file} | write out.db")
+    assert FilePath.from_path(path_result).user.name == "out.db"
+
+    # search with aggregation does not export anything
+    with pytest.raises(Exception):
+        await sync_and_check(f"search all | aggregate kind:sum(1) | db sync sqlite --database foo")
+
+    # define all parameters and check the connection string
+    with pytest.raises(Exception) as ex:
+        await sync_and_check(
+            f"db sync sqlite --database db --host bla --port 1234 --user test --password check --arg foo=bla foo2=bla2",
+            expected_table_count=11,
+        )
+    assert "sqlite://test:check@bla:1234" in str(ex.value)
+    assert "?foo=bla&foo2=bla2" in str(ex.value)
+
+    # calling db without command will print the help
+    db_res = await cli.execute_cli_command("db", stream.list)
+    assert "Synchronizes data to an SQL database." in db_res[0][0]
+
+    # make sure argsinfo is available
+    assert "sync" in cli.direct_commands["db"].args_info()
```

### Comparing `resotocore-3.5.3/tests/resotocore/cli/model_test.py` & `resotocore-3.6.0/tests/resotocore/cli/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/config/config_handler_service_test.py` & `resotocore-3.6.0/tests/resotocore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/config/config_override_service_test.py` & `resotocore-3.6.0/tests/resotocore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/config/core_config_handler_test.py` & `resotocore-3.6.0/tests/resotocore/config/core_config_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/conftest.py` & `resotocore-3.6.0/tests/resotocore/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,46 +216,47 @@
         "base",
         [],
         [
             Property("identifier", "string", required=True),
             Property("kind", "string", required=True),
             Property("ctime", "datetime"),
         ],
+        aggregate_root=False,
     )
     foo = ComplexKind(
         "foo",
         ["base"],
         [
             Property("name", "string"),
             Property("some_int", "int32"),
             Property("some_string", "string"),
             Property("now_is", "datetime"),
             Property("ctime", "datetime"),
             Property("age", "trafo.duration_to_datetime", False, SyntheticProperty(["ctime"])),
         ],
         successor_kinds={EdgeTypes.default: ["bla"]},
     )
-    inner = ComplexKind("inner", [], [Property("name", "string"), Property("inner", "inner[]")])
+    inner = ComplexKind("inner", [], [Property("name", "string"), Property("inner", "inner[]")], aggregate_root=False)
     bla = ComplexKind(
         "bla",
         ["base"],
         [
             Property("name", "string"),
             Property("now", "date"),
             Property("f", "int32"),
             Property("g", "int32[]"),
             Property("h", "inner"),
         ],
         successor_kinds={EdgeTypes.default: ["bla"]},
     )
-    cloud = ComplexKind("cloud", ["foo"], [])
-    account = ComplexKind("account", ["foo"], [])
-    region = ComplexKind("region", ["foo"], [])
-    parent = ComplexKind("parent", ["foo"], [])
-    child = ComplexKind("child", ["foo"], [])
+    cloud = ComplexKind("cloud", ["foo"], [Property("nick", "string")])
+    account = ComplexKind("account", ["foo"], [Property("nick", "string")])
+    region = ComplexKind("region", ["foo"], [Property("nick", "string")])
+    parent = ComplexKind("parent", ["foo"], [Property("nick", "string")])
+    child = ComplexKind("child", ["foo"], [Property("nick", "string")])
     some_complex = ComplexKind(
         "some_complex",
         ["base"],
         [
             Property("cloud", "cloud"),
             Property("account", "account"),
             Property("parents", "parent[]"),
```

### Comparing `resotocore-3.5.3/tests/resotocore/console_renderer_test.py` & `resotocore-3.6.0/tests/resotocore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/core_config_test.py` & `resotocore-3.6.0/tests/resotocore/core_config_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/arango_query_test.py` & `resotocore-3.6.0/tests/resotocore/db/arango_query_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,19 @@
     # make sure, there is no limit in the filter statement
     assert "LET filter0 = (FOR m0 in `ns` FILTER @b0 IN m0.kinds  RETURN m0)" in query_str
     # make sure the limit is applied to the with statement
     assert "FILTER counter1==1  LIMIT 0, 2 RETURN l0_l0_res" in query_str
 
 
 def test_context(foo_model: Model, graph_db: GraphDB) -> None:
-    query = 'is(foo) and inner[*].{name=true and inner[*].{name=true}} and parents[*].{some_int="23"}'
+    query = 'is(foo) and nested[*].{name=true and inner[*].{name=true}} and parents[*].{some_int="23"}'
     aql, bind_vars = to_query(graph_db, QueryModel(parse_query(query).on_section("reported"), foo_model))
     # query unfolds all nested loops
     assert aql == (
-        "LET filter0 = (LET nested_distinct0 = (FOR m0 in `ns`  FOR pre0 IN TO_ARRAY(m0.reported.inner) "
+        "LET filter0 = (LET nested_distinct0 = (FOR m0 in `ns`  FOR pre0 IN TO_ARRAY(m0.reported.nested) "
         "FOR pre1 IN TO_ARRAY(pre0.inner)  "
         "FOR pre2 IN TO_ARRAY(m0.reported.parents) "
         "FILTER ((@b0 IN m0.kinds) and ((pre0.name == @b1) and (pre1.name == @b2))) and (pre2.some_int == @b3) "
         "RETURN DISTINCT m0) FOR m1 in nested_distinct0  "
         'RETURN m1) FOR result in filter0 RETURN UNSET(result, ["flat"])'
     )
     # coercing works correctly for context terms
```

### Comparing `resotocore-3.5.3/tests/resotocore/db/arangodb_functions_test.py` & `resotocore-3.6.0/tests/resotocore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/async_arangodb_test.py` & `resotocore-3.6.0/tests/resotocore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/configdb_test.py` & `resotocore-3.6.0/tests/resotocore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/db_access_test.py` & `resotocore-3.6.0/tests/resotocore/db/db_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/entitydb.py` & `resotocore-3.6.0/tests/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/graphdb_test.py` & `resotocore-3.6.0/tests/resotocore/db/graphdb_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,28 +600,37 @@
     # make sure the copy graph does not exist
     await db_access.delete_graph(copy_db_name)
 
     # copy the graph
     copy_db = await graph_db.copy_graph(copy_db_name)
     assert copy_db.name == copy_db_name
 
-    # validate the vertices
-    existing_vertex_ids = {a["_key"] for a in await db.all(graph_db.name)}
-    copy_vertex_ids = {a["_key"] for a in await db.all(copy_db_name)}
-    assert existing_vertex_ids == copy_vertex_ids
-
-    # validate the default edges
-    existing_default_edge_ids = {a["_key"] for a in await db.all(f"{graph_db.name}_default")}
-    copy_default_edge_ids = {a["_key"] for a in await db.all(f"{copy_db_name}_default")}
-    assert existing_default_edge_ids == copy_default_edge_ids
-
-    # validate the delete edges
-    existing_delete_edge_ids = {a["_key"] for a in await db.all(f"{graph_db.name}_delete")}
-    copy_delete_edge_ids = {a["_key"] for a in await db.all(f"{copy_db_name}_delete")}
-    assert existing_delete_edge_ids == copy_delete_edge_ids
+    async def validate(original_db_name: GraphName, copy_db_name: str) -> None:
+        # validate the vertices
+        existing_vertex_ids = {a["_key"] for a in await db.all(original_db_name)}
+        copy_vertex_ids = {a["_key"] for a in await db.all(copy_db_name)}
+        assert existing_vertex_ids == copy_vertex_ids
+
+        # validate the default edges
+        existing_default_edge_ids = {a["_key"] for a in await db.all(f"{original_db_name}_default")}
+        copy_default_edge_ids = {a["_key"] for a in await db.all(f"{copy_db_name}_default")}
+        assert existing_default_edge_ids == copy_default_edge_ids
+
+        # validate the delete edges
+        existing_delete_edge_ids = {a["_key"] for a in await db.all(f"{original_db_name}_delete")}
+        copy_delete_edge_ids = {a["_key"] for a in await db.all(f"{copy_db_name}_delete")}
+        assert existing_delete_edge_ids == copy_delete_edge_ids
+
+    await validate(graph_db.name, copy_db.name)
+
+    # check snapshots
+    snapshot_db_name = GraphName("snapshot_" + graph_db.name)
+    snapshot_db = await graph_db.copy_graph(snapshot_db_name, to_snapshot=True)
+    assert snapshot_db.name == snapshot_db_name
+    await validate(graph_db.name, snapshot_db.name)
 
 
 def test_render_metadata_section(foo_model: Model) -> None:
     printer = ArangoGraphDB.document_to_instance_fn(foo_model)
     out = printer({"_key": "1", "reported": {"kind": "foo"}, "metadata": {"exported_at": "2023-03-06T19:37:51Z"}})
     assert "exported_age" in out["metadata"]  # exported_age is not part of the document, but should be added
```

### Comparing `resotocore-3.5.3/tests/resotocore/db/jobdb_test.py` & `resotocore-3.6.0/tests/resotocore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/modeldb_test.py` & `resotocore-3.6.0/tests/resotocore/db/modeldb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/runningtaskdb_test.py` & `resotocore-3.6.0/tests/resotocore/db/runningtaskdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/subscriberdb_test.py` & `resotocore-3.6.0/tests/resotocore/db/subscriberdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/system_data_db_test.py` & `resotocore-3.6.0/tests/resotocore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/db/templatedb_test.py` & `resotocore-3.6.0/tests/resotocore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/dependencies_test.py` & `resotocore-3.6.0/tests/resotocore/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/graph_manager/graph_manager_test.py` & `resotocore-3.6.0/tests/resotocore/graph_manager/graph_manager_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 vertex.pop("_id")
                 vertex.pop("_rev")
                 vertex.pop("hash", None)
                 vertex.pop("_from", None)
                 vertex.pop("_to", None)
                 vertices.append(vertex)
 
-        return sorted(vertices, key=lambda doc: doc["_key"])  # type: ignore
+        return sorted(vertices, key=lambda doc: doc["_key"])
 
     # check vertices content after import
     original_vertices = await collect_docs("test_graph")
     imported_vertices = await collect_docs("test_graph_import")
     assert original_vertices == imported_vertices
 
     # check default edges after import
```

### Comparing `resotocore-3.5.3/tests/resotocore/hypothesis_extension.py` & `resotocore-3.6.0/tests/resotocore/hypothesis_extension.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/infra_apps/local_runtime_test.py` & `resotocore-3.6.0/tests/resotocore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/infra_apps/package_manager_test.py` & `resotocore-3.6.0/tests/resotocore/infra_apps/package_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/message_bus_test.py` & `resotocore-3.6.0/tests/resotocore/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/model/__init__.py` & `resotocore-3.6.0/tests/resotocore/model/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Optional, List, Set
+from typing import Optional, List, Set, Any
 
 from resotocore.model.model import Model, Kind
 from resotocore.model.model_handler import ModelHandler
 from resotocore.types import EdgeType
 from resotocore.ids import GraphName
 
 
 class ModelHandlerStatic(ModelHandler):
     def __init__(self, model: Model):
         self.model = model
 
-    async def load_model(self, graph_name: GraphName) -> Model:
+    async def load_model(self, graph_name: GraphName, **kwargs: Any) -> Model:
         return self.model
 
     async def uml_image(
         self,
         graph_name: GraphName,
         output: str = "svg",
         *,
```

### Comparing `resotocore-3.5.3/tests/resotocore/model/adjust_node_test.py` & `resotocore-3.6.0/tests/resotocore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/model/db_updater_test.py` & `resotocore-3.6.0/tests/resotocore/model/db_updater_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from resotocore.analytics import AnalyticsEventSender
 from resotocore.db.deferred_edge_db import pending_deferred_edge_db
 from resotocore.db.graphdb import ArangoGraphDB
 from resotocore.db.model import GraphUpdate
 from resotocore.dependencies import empty_config
 from resotocore.ids import TaskId
 from resotocore.model.db_updater import merge_graph_process
-from resotocore.model.model import Kind
+from resotocore.model.model import Kind, Model
 from resotocore.model.typed_model import to_js
 from resotocore.types import Json
 from tests.resotocore.db.graphdb_test import create_graph
+from tests.resotocore.model import ModelHandlerStatic
 
 
 @pytest.mark.asyncio
 async def test_merge_process(
     event_sender: AnalyticsEventSender, graph_db: ArangoGraphDB, foo_kinds: List[Kind]
 ) -> None:
     # set explicitly (is done in main explicitly as well)
@@ -44,15 +45,16 @@
         yield bytes(
             json.dumps(
                 {"from_selector": {"node_id": "id_123"}, "to_selector": {"node_id": "id_456"}, "edge_type": "delete"}
             ),
             "utf-8",
         )
 
+    model_handler = ModelHandlerStatic(Model.from_kinds(foo_kinds))
     result = await merge_graph_process(
-        graph_db, event_sender, config, iterator(), timedelta(seconds=30), None, TaskId("test_task_123")
+        graph_db, model_handler, event_sender, config, iterator(), timedelta(seconds=30), None, TaskId("test_task_123")
     )
     assert result == GraphUpdate(112, 1, 0, 212, 0, 0)
     elem: Json = graph_db.db.collection("deferred_outer_edges").get("test_task_123")  # type: ignore
     assert elem["_key"] == "test_task_123"
     assert elem["task_id"] == "test_task_123"
     assert elem["edges"][0] == {"from_node": {"value": "id_123"}, "to_node": {"value": "id_456"}, "edge_type": "delete"}
```

### Comparing `resotocore-3.5.3/tests/resotocore/model/graph_access_test.py` & `resotocore-3.6.0/tests/resotocore/model/graph_access_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import collections
 import re
 from datetime import date
-from typing import Optional
+from typing import Optional, cast, Dict
 
 import jsons
 import pytest
 from deepdiff import DeepDiff
 from networkx import MultiDiGraph
 from pytest import fixture
 
 from resotocore.ids import NodeId
 from resotocore.model.graph_access import GraphAccess, GraphBuilder, EdgeTypes, EdgeKey
-from resotocore.model.model import Model, AnyKind
+from resotocore.model.model import Model, AnyKind, ComplexKind
 from resotocore.model.typed_model import to_json
 from resotocore.types import Json, EdgeType
 from resotocore.util import AccessJson, AccessNone
 from tests.resotocore.db.graphdb_test import Foo
 
 FooTuple = collections.namedtuple(
     "FooTuple",
@@ -354,7 +354,25 @@
     assert r1.metadata.descendant_count == 9
     r2 = AccessJson(graph.node("account_cloud_gcp_1"))  # type: ignore
     assert r2.metadata.descendant_summary == {"child": 54, "region": 6}
     assert r2.metadata.descendant_count == 60
     r3 = AccessJson(graph.node("cloud_gcp"))  # type: ignore
     assert r3.metadata.descendant_summary == {"child": 162, "region": 18, "account": 3}
     assert r3.metadata.descendant_count == 183
+
+
+def test_model_size(person_model: Model) -> None:
+    builder = GraphBuilder(person_model)
+    tags1 = {"foo": "bar", "bla": "blub" * 22}
+    a1 = {"kind": "Address", "id": "a1", "zip": "s1", "city": "c1", "list": ["ccc"]}
+    a2 = {"kind": "Address", "id": "aa2", "zip": "s2", "city": "gotham", "tags": tags1}
+    p1 = dict(kind="Person", id="pp1", name="pp1", address=a1, list=["a", "bb"], tags=tags1)
+    p2 = dict(kind="Person", id="p2", name="ppp2", addresses=[a1, a2], other_addresses=dict(home=a1, work=a2))
+    builder.add_node(NodeId("p1"), p1)
+    builder.add_node(NodeId("p2"), p2)
+
+    def kind_props(p: ComplexKind) -> Dict[str, int]:
+        return {p.name: p.meta_get("len", int, 0) for p in p.all_props() if p.meta("len", int)}
+
+    base = {"id": 3, "kind": 7, "list": 3, "tags": 88}  # base properties shared by person and address
+    assert kind_props(cast(ComplexKind, person_model["Person"])) == base | {"name": 4}
+    assert kind_props(cast(ComplexKind, person_model["Address"])) == base | {"city": 6, "zip": 2}
```

### Comparing `resotocore-3.5.3/tests/resotocore/model/json_schema_test.py` & `resotocore-3.6.0/tests/resotocore/model/json_schema_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from resotocore.model.json_schema import json_schema
 from resotocore.model.model import Model
 
 
 def test_schema(foo_model: Model) -> None:
     schema = json_schema(foo_model)
-    # The resource is one of the possible 9 types
-    assert len(schema["oneOf"]) == 9
+    # The resource is one of the possible 8 types
+    assert len(schema["oneOf"]) == 8
 
     # base type - all properties are defined, additional properties are allowed
     assert schema["$defs"]["base"]["required"] == ["identifier", "kind"]
     assert schema["$defs"]["base"]["properties"].keys() == {"identifier", "kind", "ctime"}
     assert schema["$defs"]["base"]["additionalProperties"] is True
 
     # final resource type - all properties are defined, additional properties are not allowed
```

### Comparing `resotocore-3.5.3/tests/resotocore/model/model_handler_test.py` & `resotocore-3.6.0/tests/resotocore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/model/model_test.py` & `resotocore-3.6.0/tests/resotocore/model/model_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
+from copy import deepcopy
 from datetime import datetime, timedelta
 from textwrap import dedent
-from typing import Type, Any, Union, cast, List
+from typing import Type, Any, Union, cast, List, Dict
 
 import pytest
 import yaml
 from attr import evolve
 from deepdiff import DeepDiff
 from hypothesis import HealthCheck, settings, given
 from networkx import DiGraph
@@ -331,14 +332,39 @@
     assert person_model.kind_by_path("other_addresses") == DictionaryKind(string_kind, person_model["Address"])
     assert person_model.kind_by_path("other_addresses.test") == person_model["Address"]
 
     # properties in hierarchy (tags is defined in base) works as well
     assert person_model.kind_by_path("tags.owner") == person_model["string"]
 
 
+def test_metadata_on_update(person_model: Model) -> None:
+    person = cast(ComplexKind, person_model["Person"])
+    person_23 = deepcopy(person)
+    person_23.properties = [evolve(prop, metadata={"len": 23}) for prop in person_23.properties]
+    person_42 = deepcopy(person)
+    person_42.properties = [evolve(prop, metadata={"size": 23, "len": 42}) for prop in person_42.properties]
+
+    def check_person(model: Model, expect_prop: Dict[str, int]) -> None:
+        for pp in cast(ComplexKind, model["Person"]).properties:
+            assert pp.metadata == expect_prop
+
+    # we update the model and expect the metadata to be set
+    updated = person_model.update_kinds([person_23])
+    check_person(updated, {"len": 23})
+    # when we update the updated model with the original person, we expect the metadata to be unchanged (not removed)
+    updated = updated.update_kinds([person])
+    check_person(updated, {"len": 23})
+    # when we update the updated model with the person_with_bla, we expect the metadata to be updated
+    updated = updated.update_kinds([person_42])
+    check_person(updated, {"len": 42, "size": 23})
+    # when we update the updated model with the person_with_foo, we expect the len property to keep as is
+    updated = updated.update_kinds([person_23])
+    check_person(updated, {"len": 42})
+
+
 def test_update(person_model: Model) -> None:
     updated = person_model.update_kinds([StringKind("Foo")])
     assert updated["Foo"].fqn == "Foo"
     # update simple type Foo as Complex is forbidden
     with pytest.raises(AttributeError) as simple:
         updated.update_kinds([ComplexKind("Foo", [], [])])
     assert str(simple.value) == "Update Foo changes an existing property type Foo"
@@ -544,11 +570,11 @@
           """.rstrip()
     )
 
     assert person == yaml.safe_load(person_kind.create_yaml(person))
 
 
 @given(json_object_gen)
-@settings(max_examples=200, suppress_health_check=HealthCheck.all())
+@settings(max_examples=200, suppress_health_check=list(HealthCheck))
 def test_yaml_generation(js: Json) -> None:
     kind = ComplexKind("test", [], [])
     assert js == yaml.safe_load(kind.create_yaml(js))
```

### Comparing `resotocore-3.5.3/tests/resotocore/model/typed_model_test.py` & `resotocore-3.6.0/tests/resotocore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/query/__init__.py` & `resotocore-3.6.0/tests/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/query/model_test.py` & `resotocore-3.6.0/tests/resotocore/query/model_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,10 +313,10 @@
     assert str(mq1 | sq1) == '(is("foo") or age > "23h") {bla: all -default-> is("bla")} bla.test == 2'
     assert str(sq1 | mq1) == '(is("foo") or age > "23h") {bla: all -default-> is("bla")} bla.test == 2'
     assert str(mq1 & sq1) == '(is("foo") and age > "23h") {bla: all -default-> is("bla")} bla.test == 2'
     assert str(sq1 & mq1) == '(is("foo") and age > "23h") {bla: all -default-> is("bla")} bla.test == 2'
 
 
 @given(query)
-@settings(max_examples=200, suppress_health_check=HealthCheck.all())
+@settings(max_examples=200, suppress_health_check=list(HealthCheck))
 def test_generated_query(q: Query) -> None:
     assert q.structure()
```

### Comparing `resotocore-3.5.3/tests/resotocore/query/query_parser_test.py` & `resotocore-3.6.0/tests/resotocore/query/query_parser_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 
     # parser read the reversed option as separate part, so following query became 3 parts
     q = parse_query("all sort kind desc limit 1 reversed -default-> all sort kind asc")
     assert len(q.parts) == 2
 
 
 @given(query)
-@settings(max_examples=200, suppress_health_check=HealthCheck.all())
+@settings(max_examples=200, suppress_health_check=list(HealthCheck))
 def test_generated_query(q: Query) -> None:
     assert str(q) == str(parse_query(str(q)))
 
 
 def assert_round_trip(parser: Parser, obj: object, after_parsed: Optional[Callable[[Any], Any]] = None) -> None:
     str_rep = str(obj)
     parsed = parser.parse(str_rep)
```

### Comparing `resotocore-3.5.3/tests/resotocore/query/template_expander_test.py` & `resotocore-3.6.0/tests/resotocore/query/template_expander_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/report/benchnmark_renderer_test.py` & `resotocore-3.6.0/tests/resotocore/report/benchnmark_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/report/inspector_service_test.py` & `resotocore-3.6.0/tests/resotocore/report/inspector_service_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     assert len(failing) == 0
 
 
 async def test_benchmark_node_result(inspector_service_with_test_benchmark: InspectorService) -> None:
     inspector = inspector_service_with_test_benchmark
     result = await inspector.perform_benchmark(inspector.cli.env["graph"], "test")
     node_edge_list = result.to_graph()
-    nodes, edges = partition_by(lambda x: x["type"] == "node", node_edge_list)  # type: ignore
+    nodes, edges = partition_by(lambda x: x["type"] == "node", node_edge_list)
     assert len(node_edge_list) == 5  # 3 nodes + 2 edges
     assert len(nodes) == 3
     assert len(edges) == 2
     for edge in edges:
         assert edge["from"] == result.node_id
```

### Comparing `resotocore-3.5.3/tests/resotocore/task/job_handler_test.py` & `resotocore-3.6.0/tests/resotocore/task/job_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/task/start_workflow_on_first_subscriber_test.py` & `resotocore-3.6.0/tests/resotocore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/task/subscribers_test.py` & `resotocore-3.6.0/tests/resotocore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/task/task_description_test.py` & `resotocore-3.6.0/tests/resotocore/task/task_description_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/task/task_handler_test.py` & `resotocore-3.6.0/tests/resotocore/task/task_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/user/user_management_service_test.py` & `resotocore-3.6.0/tests/resotocore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/util_test.py` & `resotocore-3.6.0/tests/resotocore/util_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/validator_test.py` & `resotocore-3.6.0/tests/resotocore/validator_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/web/api_client.py` & `resotocore-3.6.0/tests/resotocore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/web/api_test.py` & `resotocore-3.6.0/tests/resotocore/web/api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,21 +157,22 @@
     assert len((await core_client.model()).kinds) >= len(predefined_kinds)
 
     # PATCH /model
     string_kind: rc.Kind = rc.Kind(fqn="only_three", runtime_kind="string", properties=None, bases=None)
     setattr(string_kind, "min_length", 3)
     setattr(string_kind, "max_length", 3)
 
-    prop = rc.Property(name="ot", kind="only_three", required=False)
-    complex_kind: rc.Kind = rc.Kind(fqn="test_cpl", runtime_kind=None, properties=[prop], bases=None)
+    prop = rc.Property(name="ot", kind="only_three", required=False, metadata={"len": 3})
+    complex_kind: rc.Kind = rc.Kind(fqn="test_cpl", runtime_kind=None, properties=[prop], bases=None, metadata={"a": 1})
     setattr(complex_kind, "allow_unknown_props", False)
 
     update = await core_client.update_model([string_kind, complex_kind])
-    none_kind = rc.Kind(fqn="none", runtime_kind=None, properties=None, bases=None)
-    assert (update.kinds.get("only_three") or none_kind).runtime_kind == "string"
+    assert update.kinds["only_three"].runtime_kind == "string"
+    assert update.kinds["test_cpl"].metadata["a"] == 1
+    assert update.kinds["test_cpl"].properties[0].metadata["len"] == 3
 
     # GET /model/uml
     async with client_session.get(core_client.resotocore_url + "/model/uml", params={"output": "puml"}) as r:
         assert r.status == 200
         assert r.headers["content-type"] == "text/plain"
         puml = await r.text()
         assert puml.startswith("@startuml")
@@ -382,15 +383,15 @@
     # execute multiple commands
     response = await core_client.cli_execute_raw("echo foo; echo bar; echo bla")
     reader: MultipartReader = MultipartReader.from_response(response.undrelying)  # type: ignore
     assert [await p.text() async for p in reader] == ['"foo"', '"bar"', '"bla"']
 
     # list all cli commands
     info = AccessJson(await core_client.cli_info())
-    assert len(info.commands) == 43
+    assert len(info.commands) == 44
 
 
 @pytest.mark.asyncio
 async def test_config(core_client: ResotoClient, foo_kinds: List[rc.Kind]) -> None:
     # make sure we have a clean slate
     async for config in core_client.configs():
         await core_client.delete_config(config)
```

### Comparing `resotocore-3.5.3/tests/resotocore/web/certificate_handler_test.py` & `resotocore-3.6.0/tests/resotocore/web/certificate_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.3/tests/resotocore/web/content_renderer_test.py` & `resotocore-3.6.0/tests/resotocore/web/content_renderer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,84 +23,84 @@
     json_simple_element_gen,
     node_gen,
     graph_stream,
 )
 
 
 @given(json_array_gen)
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_json(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
         result = ""
         async for elem in respond_json(streamer):
             result += elem
         assert json.loads(result) == elements
 
 
 @given(json_array_gen)
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_ndjson(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
         result = []
         async for elem in respond_ndjson(streamer):
             result.append(json.loads(elem.strip()))
         assert result == elements
 
 
 @given(json_array_gen)
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_yaml(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
         result = ""
         async for elem in respond_yaml(streamer):
             result += elem + "\n"
         assert [a for a in yaml.full_load_all(result)] == elements
 
 
 @given(lists(json_simple_element_gen, min_size=1, max_size=10))
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_text_simple_elements(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
         result = ""
         async for elem in respond_text(streamer):
             result += elem + "\n"
         # every element is rendered as one or more line (string with \n is rendered as multiple lines)
         assert len(elements) + 1 <= len(result.split("\n"))
 
 
 @given(lists(node_gen(), min_size=1, max_size=10))
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_text_complex_elements(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
         result = ""
         async for elem in respond_text(streamer):
             result += elem
         # every element is rendered as yaml with --- as object deliminator
         assert len(elements) == len(result.split("---"))
 
 
 @given(lists(node_gen(), min_size=1, max_size=10))
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_cytoscape(elements: List[Json]) -> None:
     async with graph_stream(elements).stream() as streamer:
         result = ""
         async for elem in respond_cytoscape(streamer):
             result += elem
         # The resulting string can be parsed as json
         assert json.loads(result)
 
 
 @given(lists(node_gen(), min_size=1, max_size=10))
-@settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
+@settings(max_examples=20, suppress_health_check=list(HealthCheck), deadline=1000)
 @pytest.mark.asyncio
 async def test_graphml(elements: List[Json]) -> None:
     async with graph_stream(elements).stream() as streamer:
         result = ""
         async for elem in respond_graphml(streamer):
             result += elem
     # The resulting string can be parsed as xml
```

### Comparing `resotocore-3.5.3/tests/resotocore/worker_task_queue_test.py` & `resotocore-3.6.0/tests/resotocore/worker_task_queue_test.py`

 * *Files identical despite different names*

