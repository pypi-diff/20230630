# Comparing `tmp/fullctl-1.2.0.tar.gz` & `tmp/fullctl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullctl-1.2.0.tar", max compression
+gzip compressed data, was "fullctl-1.4.0.tar", max compression
```

## Comparing `fullctl-1.2.0.tar` & `fullctl-1.4.0.tar`

### file list

```diff
@@ -1,292 +1,311 @@
--rw-r--r--   0        0        0    11357 2021-04-22 13:27:52.952758 fullctl-1.2.0/LICENSE
--rw-r--r--   0        0        0     1203 2023-04-15 17:47:54.744256 fullctl-1.2.0/README.md
--rw-r--r--   0        0        0     2223 2023-04-15 17:47:45.806100 fullctl-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.2.0/src/fullctl/__init__.py
--rwxr-xr-x   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.2.0/src/fullctl/django/__init__.py
--rw-r--r--   0        0        0     5587 2023-04-15 16:24:16.029446 fullctl-1.2.0/src/fullctl/django/admin.py
--rw-r--r--   0        0        0      259 2021-10-21 03:49:59.920722 fullctl-1.2.0/src/fullctl/django/apps.py
--rw-r--r--   0        0        0     7188 2023-02-27 05:27:02.246818 fullctl-1.2.0/src/fullctl/django/auditlog.py
--rw-r--r--   0        0        0     4863 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/auth.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.2.0/src/fullctl/django/autocomplete/__init__.py
--rw-r--r--   0        0        0      954 2023-02-27 05:27:02.247818 fullctl-1.2.0/src/fullctl/django/autocomplete/pdb.py
--rw-r--r--   0        0        0     2518 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/context.py
--rw-r--r--   0        0        0     3402 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/context_processors.py
--rw-r--r--   0        0        0     3102 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/decorators.py
--rw-r--r--   0        0        0      233 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/enum.py
--rw-r--r--   0        0        0      283 2022-10-14 13:57:25.205745 fullctl-1.2.0/src/fullctl/django/exceptions.py
--rw-r--r--   0        0        0      650 2022-10-14 13:57:25.205745 fullctl-1.2.0/src/fullctl/django/fields/__init__.py
--rw-r--r--   0        0        0     4351 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/fields/service_bridge/__init__.py
--rw-r--r--   0        0        0      317 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/fields/service_bridge/prefixctl.py
--rw-r--r--   0        0        0       79 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/forms.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.2.0/src/fullctl/django/inet/__init__.py
--rw-r--r--   0        0        0      325 2021-04-22 13:27:52.954758 fullctl-1.2.0/src/fullctl/django/inet/const.py
--rw-r--r--   0        0        0      186 2021-04-22 13:27:52.955758 fullctl-1.2.0/src/fullctl/django/inet/exceptions.py
--rw-r--r--   0        0        0      761 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/inet/fields.py
--rw-r--r--   0        0        0      519 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/inet/util.py
--rw-r--r--   0        0        0     3738 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/inet/validators.py
--rw-r--r--   0        0        0      307 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/mail.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.2.0/src/fullctl/django/management/__init__.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.2.0/src/fullctl/django/management/commands/__init__.py
--rw-r--r--   0        0        0     4128 2021-10-29 12:45:46.921418 fullctl-1.2.0/src/fullctl/django/management/commands/base.py
--rw-r--r--   0        0        0     1867 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
--rw-r--r--   0        0        0     4750 2023-02-27 05:27:02.249818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py
--rw-r--r--   0        0        0      620 2023-02-27 05:27:02.249818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_promote_user.py
--rw-r--r--   0        0        0      763 2023-02-27 05:27:02.249818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_work_task.py
--rw-r--r--   0        0        0     3040 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/middleware.py
--rw-r--r--   0        0        0     8661 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0001_initial.py
--rw-r--r--   0        0        0      291 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0002_delete_apikey.py
--rw-r--r--   0        0        0     2216 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0003_auditlog.py
--rw-r--r--   0        0        0     1081 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py
--rw-r--r--   0        0        0      625 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py
--rw-r--r--   0        0        0     1374 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py
--rw-r--r--   0        0        0      485 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0007_auditlog_ip_address.py
--rw-r--r--   0        0        0     4435 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0008_managementtask.py
--rw-r--r--   0        0        0     2341 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0009_taskclaim.py
--rw-r--r--   0        0        0      557 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
--rw-r--r--   0        0        0      749 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py
--rw-r--r--   0        0        0     5399 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py
--rw-r--r--   0        0        0      723 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py
--rw-r--r--   0        0        0      516 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
--rw-r--r--   0        0        0      625 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0015_alter_task_parent.py
--rw-r--r--   0        0        0      414 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0016_task_limit_id.py
--rw-r--r--   0        0        0      463 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
--rw-r--r--   0        0        0     4271 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0018_task_schedule.py
--rw-r--r--   0        0        0      402 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0019_default_org.py
--rw-r--r--   0        0        0      389 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0020_auditlog_action_length.py
--rw-r--r--   0        0        0     3330 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0021_servicebridgeaction.py
--rw-r--r--   0        0        0     1077 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py
--rw-r--r--   0        0        0     1050 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py
--rw-r--r--   0        0        0     2539 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py
--rw-r--r--   0        0        0      900 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py
--rw-r--r--   0        0        0      837 2023-02-27 05:27:02.255818 fullctl-1.2.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py
--rw-r--r--   0        0        0     4518 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0027_request_response.py
--rw-r--r--   0        0        0      457 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0028_request_identifier.py
--rw-r--r--   0        0        0      427 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0029_response_content.py
--rw-r--r--   0        0        0      550 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0030_alter_response_content.py
--rw-r--r--   0        0        0     2496 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.2.0/src/fullctl/django/migrations/__init__.py
--rw-r--r--   0        0        0      218 2021-10-21 03:49:59.989723 fullctl-1.2.0/src/fullctl/django/models/__init__.py
--rw-r--r--   0        0        0      150 2022-10-14 13:57:25.208745 fullctl-1.2.0/src/fullctl/django/models/abstract/__init__.py
--rw-r--r--   0        0        0     3282 2022-06-14 21:13:57.268730 fullctl-1.2.0/src/fullctl/django/models/abstract/alert.py
--rw-r--r--   0        0        0     3337 2022-10-14 13:57:25.209745 fullctl-1.2.0/src/fullctl/django/models/abstract/base.py
--rw-r--r--   0        0        0    13540 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/models/abstract/meta.py
--rw-r--r--   0        0        0     7822 2023-02-27 05:27:02.255818 fullctl-1.2.0/src/fullctl/django/models/abstract/service_bridge.py
--rw-r--r--   0        0        0     2682 2023-02-27 05:27:02.256818 fullctl-1.2.0/src/fullctl/django/models/abstract/template.py
--rw-r--r--   0        0        0      288 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/models/concrete/__init__.py
--rw-r--r--   0        0        0     7437 2023-02-27 05:27:02.256818 fullctl-1.2.0/src/fullctl/django/models/concrete/account.py
--rw-r--r--   0        0        0     1884 2023-02-27 05:27:02.256818 fullctl-1.2.0/src/fullctl/django/models/concrete/auditlog.py
--rw-r--r--   0        0        0     1808 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/models/concrete/meta.py
--rw-r--r--   0        0        0     7811 2023-02-27 05:27:02.257818 fullctl-1.2.0/src/fullctl/django/models/concrete/service_bridge.py
--rw-r--r--   0        0        0    16238 2023-04-15 16:24:16.031446 fullctl-1.2.0/src/fullctl/django/models/concrete/tasks.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.2.0/src/fullctl/django/rest/__init__.py
--rw-r--r--   0        0        0     8217 2023-02-27 05:27:02.257818 fullctl-1.2.0/src/fullctl/django/rest/api_schema.py
--rw-r--r--   0        0        0     1143 2021-10-29 12:45:46.966419 fullctl-1.2.0/src/fullctl/django/rest/authentication.py
--rw-r--r--   0        0        0     1831 2021-06-15 13:03:05.250145 fullctl-1.2.0/src/fullctl/django/rest/core.py
--rw-r--r--   0        0        0     8517 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/decorators.py
--rw-r--r--   0        0        0      328 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/fields.py
--rw-r--r--   0        0        0     1074 2021-10-21 03:50:00.023724 fullctl-1.2.0/src/fullctl/django/rest/filters.py
--rw-r--r--   0        0        0     1486 2022-10-14 13:57:25.257745 fullctl-1.2.0/src/fullctl/django/rest/mixins.py
--rw-r--r--   0        0        0     2148 2021-10-29 12:45:46.983419 fullctl-1.2.0/src/fullctl/django/rest/renderers.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.957758 fullctl-1.2.0/src/fullctl/django/rest/route/__init__.py
--rw-r--r--   0        0        0      352 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/route/aaactl_sync.py
--rw-r--r--   0        0        0      298 2021-10-21 03:50:00.070725 fullctl-1.2.0/src/fullctl/django/rest/route/account.py
--rw-r--r--   0        0        0      426 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/route/service_bridge.py
--rw-r--r--   0        0        0      342 2023-02-27 05:27:02.259818 fullctl-1.2.0/src/fullctl/django/rest/route/usage.py
--rw-r--r--   0        0        0     1558 2023-02-27 05:27:02.259818 fullctl-1.2.0/src/fullctl/django/rest/serializers/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-15 16:24:16.031446 fullctl-1.2.0/src/fullctl/django/rest/serializers/aaactl_sync.py
--rw-r--r--   0        0        0     2523 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/serializers/account.py
--rw-r--r--   0        0        0      518 2023-04-15 16:24:16.032446 fullctl-1.2.0/src/fullctl/django/rest/serializers/meta.py
--rw-r--r--   0        0        0      807 2022-10-14 13:57:25.258745 fullctl-1.2.0/src/fullctl/django/rest/serializers/org.py
--rw-r--r--   0        0        0      233 2023-02-27 05:27:02.260818 fullctl-1.2.0/src/fullctl/django/rest/serializers/service_bridge.py
--rw-r--r--   0        0        0      688 2022-10-14 13:57:25.258745 fullctl-1.2.0/src/fullctl/django/rest/serializers/template.py
--rw-r--r--   0        0        0      440 2023-02-27 05:27:02.260818 fullctl-1.2.0/src/fullctl/django/rest/serializers/usage.py
--rw-r--r--   0        0        0      395 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/throttle.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0/src/fullctl/django/rest/urls/__init__.py
--rw-r--r--   0        0        0      222 2021-10-21 03:50:00.135727 fullctl-1.2.0/src/fullctl/django/rest/urls/aaactl_sync.py
--rw-r--r--   0        0        0      210 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/urls/account.py
--rw-r--r--   0        0        0      491 2021-10-29 12:45:46.983419 fullctl-1.2.0/src/fullctl/django/rest/urls/service_bridge.py
--rw-r--r--   0        0        0     2084 2023-02-27 05:27:02.260818 fullctl-1.2.0/src/fullctl/django/rest/urls/service_bridge_proxy.py
--rw-r--r--   0        0        0      204 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/urls/usage.py
--rw-r--r--   0        0        0      419 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/usage.py
--rw-r--r--   0        0        0        0 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/views/__init__.py
--rw-r--r--   0        0        0     3258 2022-10-14 13:57:25.258745 fullctl-1.2.0/src/fullctl/django/rest/views/aaactl_sync.py
--rw-r--r--   0        0        0     2576 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/views/account.py
--rw-r--r--   0        0        0     7159 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/views/service_bridge.py
--rw-r--r--   0        0        0      994 2023-02-27 05:27:02.261818 fullctl-1.2.0/src/fullctl/django/rest/views/template.py
--rw-r--r--   0        0        0     1410 2023-02-27 05:27:02.261818 fullctl-1.2.0/src/fullctl/django/rest/views/usage.py
--rw-r--r--   0        0        0    16282 2023-04-15 17:32:55.631524 fullctl-1.2.0/src/fullctl/django/settings/__init__.py
--rw-r--r--   0        0        0     2655 2023-02-27 05:27:02.262818 fullctl-1.2.0/src/fullctl/django/settings/default.py
--rw-r--r--   0        0        0     1215 2023-02-27 05:27:02.262818 fullctl-1.2.0/src/fullctl/django/signals.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0/src/fullctl/django/social/__init__.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0/src/fullctl/django/social/backends/__init__.py
--rw-r--r--   0        0        0     1206 2021-06-15 13:03:05.252145 fullctl-1.2.0/src/fullctl/django/social/backends/peeringdb.py
--rw-r--r--   0        0        0     1589 2021-10-21 03:50:00.137727 fullctl-1.2.0/src/fullctl/django/social/backends/twentyc.py
--rw-r--r--   0        0        0      388 2021-06-15 13:03:05.252145 fullctl-1.2.0/src/fullctl/django/social/pipelines/__init__.py
--rw-r--r--   0        0        0     4237 2021-04-22 13:27:52.959758 fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
--rw-r--r--   0        0        0    56503 2023-04-15 17:32:55.631524 fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.rest.js
--rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.959758 fullctl-1.2.0/src/fullctl/django/static/common/20c-logo-filled.svg
--rw-r--r--   0        0        0    21299 2023-02-27 05:27:02.264818 fullctl-1.2.0/src/fullctl/django/static/common/app.css
--rw-r--r--   0        0        0    19449 2023-02-27 05:27:02.265818 fullctl-1.2.0/src/fullctl/django/static/common/app.js
--rwxr-xr-x   0        0        0   372526 2021-10-29 12:45:47.007420 fullctl-1.2.0/src/fullctl/django/static/common/favicon.ico
--rw-r--r--   0        0        0     3380 2021-04-22 13:27:52.960758 fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
--rw-r--r--   0        0        0     3657 2021-04-22 13:27:52.960758 fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
--rw-r--r--   0        0        0     3430 2021-04-22 13:27:52.960758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/add.svg
--rw-r--r--   0        0        0     3819 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/alerts.svg
--rw-r--r--   0        0        0     2838 2022-06-14 21:13:57.362731 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/api.svg
--rw-r--r--   0        0        0     1303 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
--rw-r--r--   0        0        0     2681 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/delete.svg
--rw-r--r--   0        0        0     5490 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/edit.svg
--rwxr-xr-x   0        0        0     1172 2021-10-29 12:45:47.024420 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/launch.svg
--rw-r--r--   0        0        0     1601 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
--rw-r--r--   0        0        0     3357 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/list.svg
--rwxr-xr-x   0        0        0     1721 2022-06-14 21:13:57.362731 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/location.svg
--rw-r--r--   0        0        0     2617 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/logout.svg
--rwxr-xr-x   0        0        0      726 2021-10-29 12:45:47.026420 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/mail.svg
--rw-r--r--   0        0        0     2761 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/org.svg
--rw-r--r--   0        0        0     1597 2022-06-14 21:13:57.599734 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/refresh.svg
--rw-r--r--   0        0        0     1515 2022-06-14 21:13:57.623735 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/report.svg
--rw-r--r--   0        0        0     8263 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/settings.svg
--rw-r--r--   0        0        0     4138 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/user.svg
--rwxr-xr-x   0        0        0     2782 2021-10-29 12:45:47.035421 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/view.svg
--rw-r--r--   0        0        0     3689 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      169 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-add.svg
--rw-r--r--   0        0        0      275 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-create.svg
--rw-r--r--   0        0        0      272 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-list-box.svg
--rw-r--r--   0        0        0      240 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-trash.svg
--rw-r--r--   0        0        0     5957 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      954 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
--rw-r--r--   0        0        0      818 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-close.svg
--rwxr-xr-x   0        0        0     2427 2023-02-27 05:27:02.266818 fullctl-1.2.0/src/fullctl/django/static/common/logos/aclctl-dark.svg
--rwxr-xr-x   0        0        0    36084 2023-04-15 16:24:16.033446 fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png
--rwxr-xr-x   0        0        0    36307 2023-04-15 16:24:16.033446 fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-light.png
--rwxr-xr-x   0        0        0     4680 2022-10-14 13:57:25.295745 fullctl-1.2.0/src/fullctl/django/static/common/logos/devicectl-dark.svg
--rwxr-xr-x   0        0        0     2579 2021-10-29 12:45:47.035421 fullctl-1.2.0/src/fullctl/django/static/common/logos/ixctl-dark.svg
--rwxr-xr-x   0        0        0     3857 2021-10-29 12:45:47.035421 fullctl-1.2.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg
--rwxr-xr-x   0        0        0     4166 2021-10-29 12:45:47.036420 fullctl-1.2.0/src/fullctl/django/static/common/logos/peerctl-dark.svg
--rwxr-xr-x   0        0        0     4336 2022-06-14 21:13:57.623735 fullctl-1.2.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg
--rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/oauth/20c.svg
--rw-r--r--   0        0        0      689 2021-04-22 13:27:52.963758 fullctl-1.2.0/src/fullctl/django/static/common/oauth/google.svg
--rw-r--r--   0        0        0     5222 2023-04-15 16:24:16.033446 fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png
--rw-r--r--   0        0        0     9186 2021-04-22 13:27:52.963758 fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb.png
--rw-r--r--   0        0        0     4323 2021-10-21 03:50:00.180728 fullctl-1.2.0/src/fullctl/django/static/common/service_bridge.js
--rw-r--r--   0        0        0    11545 2023-02-27 05:27:02.266818 fullctl-1.2.0/src/fullctl/django/static/common/themes/dark.css
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.963758 fullctl-1.2.0/src/fullctl/django/static/common/themes/light.css
--rw-r--r--   0        0        0    25412 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/static/common/v2/app.css
--rw-r--r--   0        0        0    32037 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/static/common/v2/app.js
--rw-r--r--   0        0        0      644 2023-02-27 05:27:02.268818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/add.svg
--rw-r--r--   0        0        0     4812 2023-02-27 05:27:02.268818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/api.svg
--rw-r--r--   0        0        0      352 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
--rw-r--r--   0        0        0      232 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/arrow.svg
--rw-r--r--   0        0        0      532 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
--rw-r--r--   0        0        0      423 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/cancel.svg
--rw-r--r--   0        0        0      274 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/close.svg
--rw-r--r--   0        0        0     1229 2023-04-15 16:24:16.034446 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/database.svg
--rw-r--r--   0        0        0      427 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/download.svg
--rw-r--r--   0        0        0      438 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/envelope.svg
--rw-r--r--   0        0        0      569 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/eye.svg
--rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
--rw-r--r--   0        0        0     1530 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/gear.svg
--rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/geo-alt.svg
--rw-r--r--   0        0        0     1975 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/help.svg
--rw-r--r--   0        0        0      582 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/delete.svg
--rw-r--r--   0        0        0      438 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/edit.svg
--rw-r--r--   0        0        0      818 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/options.svg
--rw-r--r--   0        0        0      447 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list-ul.svg
--rw-r--r--   0        0        0      553 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/logout.svg
--rw-r--r--   0        0        0      749 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/org.svg
--rw-r--r--   0        0        0      331 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/search.svg
--rw-r--r--   0        0        0     1465 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
--rw-r--r--   0        0        0      465 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
--rw-r--r--   0        0        0      190 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
--rw-r--r--   0        0        0     4138 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/user.svg
--rw-r--r--   0        0        0     3986 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/view-settings.svg
--rw-r--r--   0        0        0    61189 2023-02-27 05:27:02.273818 fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/help.png
--rw-r--r--   0        0        0   426086 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png
--rw-r--r--   0        0        0    14637 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/static/common/v2/themes/dark.css
--rw-r--r--   0        0        0        0 2023-02-27 05:27:02.273818 fullctl-1.2.0/src/fullctl/django/static/common/v2/themes/light.css
--rw-r--r--   0        0        0      921 2023-02-27 05:27:02.274818 fullctl-1.2.0/src/fullctl/django/tasks/__init__.py
--rw-r--r--   0        0        0      740 2021-10-21 03:50:00.186728 fullctl-1.2.0/src/fullctl/django/tasks/celery.py
--rw-r--r--   0        0        0     2351 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/tasks/orm.py
--rw-r--r--   0        0        0     2220 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/tasks/qualifiers.py
--rw-r--r--   0        0        0      374 2023-02-27 05:27:02.274818 fullctl-1.2.0/src/fullctl/django/tasks/util.py
--rw-r--r--   0        0        0      658 2022-10-14 13:57:25.296744 fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/redoc.html
--rw-r--r--   0        0        0      856 2022-10-14 13:57:25.296744 fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/swagger.html
--rw-r--r--   0        0        0     8871 2022-10-14 13:57:25.296744 fullctl-1.2.0/src/fullctl/django/templates/common/app/base.html
--rw-r--r--   0        0        0      211 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/checkbox.html
--rw-r--r--   0        0        0     1935 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      726 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/invite.html
--rw-r--r--   0        0        0      792 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
--rw-r--r--   0        0        0      355 2021-06-15 13:03:05.254145 fullctl-1.2.0/src/fullctl/django/templates/common/app/index.html
--rw-r--r--   0        0        0     1974 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/manage/permissions.html
--rw-r--r--   0        0        0     4752 2022-10-14 13:57:25.297744 fullctl-1.2.0/src/fullctl/django/templates/common/app/modal.html
--rw-r--r--   0        0        0     2668 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/app/navbar.html
--rw-r--r--   0        0        0      371 2023-02-27 05:27:02.275818 fullctl-1.2.0/src/fullctl/django/templates/common/app/templates.html
--rw-r--r--   0        0        0     3101 2022-10-14 13:57:25.297744 fullctl-1.2.0/src/fullctl/django/templates/common/auth/login.html
--rw-r--r--   0        0        0      880 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth-badge.html
--rw-r--r--   0        0        0     1110 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth.html
--rw-r--r--   0        0        0     1996 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/base.html
--rw-r--r--   0        0        0      333 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/400.html
--rw-r--r--   0        0        0      367 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/401.html
--rw-r--r--   0        0        0      375 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/403.html
--rw-r--r--   0        0        0      377 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/404.html
--rw-r--r--   0        0        0      456 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/500.html
--rw-r--r--   0        0        0      565 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/base.html
--rw-r--r--   0        0        0      351 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/details.html
--rw-r--r--   0        0        0     1229 2022-06-14 21:13:57.992740 fullctl-1.2.0/src/fullctl/django/templates/common/snippets.html
--rw-r--r--   0        0        0      234 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/tool_base.html
--rw-r--r--   0        0        0      658 2023-02-27 05:27:02.276818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html
--rw-r--r--   0        0        0      856 2023-02-27 05:27:02.276818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html
--rw-r--r--   0        0        0    12217 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/base.html
--rw-r--r--   0        0        0      211 2023-02-27 05:27:02.277818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/checkbox.html
--rw-r--r--   0        0        0     2092 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
--rw-r--r--   0        0        0      357 2023-02-27 05:27:02.277818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/delete_selected.html
--rw-r--r--   0        0        0     1775 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/footer.html
--rw-r--r--   0        0        0     1935 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      430 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
--rw-r--r--   0        0        0      726 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/invite.html
--rw-r--r--   0        0        0      792 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
--rw-r--r--   0        0        0      358 2023-02-27 05:27:02.279818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/index.html
--rw-r--r--   0        0        0     1974 2023-02-27 05:27:02.279818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html
--rw-r--r--   0        0        0     6317 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/modal.html
--rw-r--r--   0        0        0     2668 2023-02-27 05:27:02.280818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/navbar.html
--rw-r--r--   0        0        0      413 2023-02-27 05:27:02.280818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/templates.html
--rw-r--r--   0        0        0     3048 2023-02-27 05:27:02.280818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/login.html
--rw-r--r--   0        0        0     1109 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
--rw-r--r--   0        0        0     1339 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth.html
--rw-r--r--   0        0        0     1977 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/base.html
--rw-r--r--   0        0        0      339 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/400.html
--rw-r--r--   0        0        0      373 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/401.html
--rw-r--r--   0        0        0      381 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/403.html
--rw-r--r--   0        0        0      383 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/404.html
--rw-r--r--   0        0        0      462 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/500.html
--rw-r--r--   0        0        0      568 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/base.html
--rw-r--r--   0        0        0      351 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/details.html
--rw-r--r--   0        0        0     1661 2023-04-15 16:24:16.039446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/snippets.html
--rw-r--r--   0        0        0      234 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/tool_base.html
--rw-r--r--   0        0        0      249 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
--rw-r--r--   0        0        0        0 2022-06-14 21:13:57.992740 fullctl-1.2.0/src/fullctl/django/templatetags/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-15 16:24:16.039446 fullctl-1.2.0/src/fullctl/django/templatetags/fullctl_util.py
--rw-r--r--   0        0        0     3152 2023-02-27 05:27:02.283818 fullctl-1.2.0/src/fullctl/django/testutil.py
--rw-r--r--   0        0        0     3266 2023-04-15 17:32:55.633525 fullctl-1.2.0/src/fullctl/django/urls.py
--rw-r--r--   0        0        0     1171 2023-02-27 05:27:02.283818 fullctl-1.2.0/src/fullctl/django/util.py
--rw-r--r--   0        0        0     1193 2022-10-14 13:57:25.299744 fullctl-1.2.0/src/fullctl/django/validators.py
--rw-r--r--   0        0        0     2304 2023-02-27 05:27:02.284818 fullctl-1.2.0/src/fullctl/django/views/__init__.py
--rw-r--r--   0        0        0      199 2022-10-14 13:57:25.300744 fullctl-1.2.0/src/fullctl/django/views/api_schema.py
--rw-r--r--   0        0        0      927 2023-04-15 17:32:55.633525 fullctl-1.2.0/src/fullctl/django/views/template.py
--rw-r--r--   0        0        0        0 2021-06-15 13:03:05.256145 fullctl-1.2.0/src/fullctl/service_bridge/__init__.py
--rw-r--r--   0        0        0     2604 2023-04-15 17:32:55.633525 fullctl-1.2.0/src/fullctl/service_bridge/aaactl.py
--rw-r--r--   0        0        0     8510 2023-04-15 16:24:16.052446 fullctl-1.2.0/src/fullctl/service_bridge/client.py
--rw-r--r--   0        0        0     3419 2023-02-27 05:27:02.285818 fullctl-1.2.0/src/fullctl/service_bridge/data.py
--rw-r--r--   0        0        0     2180 2023-04-15 16:24:16.053446 fullctl-1.2.0/src/fullctl/service_bridge/devicectl.py
--rw-r--r--   0        0        0     2577 2023-04-15 16:24:16.053446 fullctl-1.2.0/src/fullctl/service_bridge/ixctl.py
--rw-r--r--   0        0        0     2651 2023-02-27 05:27:02.286818 fullctl-1.2.0/src/fullctl/service_bridge/nautobot.py
--rw-r--r--   0        0        0     1699 2023-04-15 16:24:16.054446 fullctl-1.2.0/src/fullctl/service_bridge/pdbctl.py
--rw-r--r--   0        0        0     1037 2023-04-15 16:24:16.063447 fullctl-1.2.0/src/fullctl/service_bridge/peerctl.py
--rw-r--r--   0        0        0     1076 2023-04-15 16:24:16.097447 fullctl-1.2.0/src/fullctl/service_bridge/prefixctl.py
--rw-r--r--   0        0        0     6952 2023-04-15 16:24:16.097447 fullctl-1.2.0/src/fullctl/service_bridge/sot.py
--rw-r--r--   0        0        0      323 2022-10-14 13:57:25.408743 fullctl-1.2.0/src/fullctl/utils/__init__.py
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 fullctl-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-04-22 13:27:52.952758 fullctl-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1203 2023-04-18 23:41:07.569197 fullctl-1.4.0/README.md
+-rw-r--r--   0        0        0     2213 2023-06-30 20:48:24.070788 fullctl-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.4.0/src/fullctl/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.4.0/src/fullctl/django/__init__.py
+-rw-r--r--   0        0        0     5719 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/admin.py
+-rw-r--r--   0        0        0      259 2021-10-21 03:49:59.920722 fullctl-1.4.0/src/fullctl/django/apps.py
+-rw-r--r--   0        0        0     7188 2023-02-27 05:27:02.246818 fullctl-1.4.0/src/fullctl/django/auditlog.py
+-rw-r--r--   0        0        0     4966 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/auth.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.4.0/src/fullctl/django/autocomplete/__init__.py
+-rw-r--r--   0        0        0     1231 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/autocomplete/devicectl.py
+-rw-r--r--   0        0        0      954 2023-02-27 05:27:02.247818 fullctl-1.4.0/src/fullctl/django/autocomplete/pdb.py
+-rw-r--r--   0        0        0     2518 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/context.py
+-rw-r--r--   0        0        0     3389 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/context_processors.py
+-rw-r--r--   0        0        0     3102 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/decorators.py
+-rw-r--r--   0        0        0      233 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/enum.py
+-rw-r--r--   0        0        0      283 2022-10-14 13:57:25.205745 fullctl-1.4.0/src/fullctl/django/exceptions.py
+-rw-r--r--   0        0        0      650 2022-10-14 13:57:25.205745 fullctl-1.4.0/src/fullctl/django/fields/__init__.py
+-rw-r--r--   0        0        0     4351 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/fields/service_bridge/__init__.py
+-rw-r--r--   0        0        0      317 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/fields/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0       79 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/forms.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.4.0/src/fullctl/django/inet/__init__.py
+-rw-r--r--   0        0        0      325 2021-04-22 13:27:52.954758 fullctl-1.4.0/src/fullctl/django/inet/const.py
+-rw-r--r--   0        0        0      186 2021-04-22 13:27:52.955758 fullctl-1.4.0/src/fullctl/django/inet/exceptions.py
+-rw-r--r--   0        0        0      761 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/inet/fields.py
+-rw-r--r--   0        0        0      519 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/inet/util.py
+-rw-r--r--   0        0        0     3738 2021-06-15 13:03:05.246145 fullctl-1.4.0/src/fullctl/django/inet/validators.py
+-rw-r--r--   0        0        0      307 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/mail.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.4.0/src/fullctl/django/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.4.0/src/fullctl/django/management/commands/__init__.py
+-rw-r--r--   0        0        0     4128 2021-10-29 12:45:46.921418 fullctl-1.4.0/src/fullctl/django/management/commands/base.py
+-rw-r--r--   0        0        0     1867 2023-02-27 05:27:02.248818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
+-rw-r--r--   0        0        0     4750 2023-02-27 05:27:02.249818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py
+-rw-r--r--   0        0        0      620 2023-02-27 05:27:02.249818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_promote_user.py
+-rw-r--r--   0        0        0      763 2023-02-27 05:27:02.249818 fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_work_task.py
+-rw-r--r--   0        0        0     4373 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/middleware.py
+-rw-r--r--   0        0        0     8661 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0      291 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0002_delete_apikey.py
+-rw-r--r--   0        0        0     2216 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0003_auditlog.py
+-rw-r--r--   0        0        0     1081 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py
+-rw-r--r--   0        0        0      625 2023-02-27 05:27:02.250818 fullctl-1.4.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py
+-rw-r--r--   0        0        0     1374 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py
+-rw-r--r--   0        0        0      485 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0007_auditlog_ip_address.py
+-rw-r--r--   0        0        0     4435 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0008_managementtask.py
+-rw-r--r--   0        0        0     2341 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0009_taskclaim.py
+-rw-r--r--   0        0        0      557 2023-02-27 05:27:02.251818 fullctl-1.4.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
+-rw-r--r--   0        0        0      749 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py
+-rw-r--r--   0        0        0     5399 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py
+-rw-r--r--   0        0        0      723 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py
+-rw-r--r--   0        0        0      516 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
+-rw-r--r--   0        0        0      625 2023-02-27 05:27:02.252818 fullctl-1.4.0/src/fullctl/django/migrations/0015_alter_task_parent.py
+-rw-r--r--   0        0        0      414 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0016_task_limit_id.py
+-rw-r--r--   0        0        0      463 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
+-rw-r--r--   0        0        0     4271 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0018_task_schedule.py
+-rw-r--r--   0        0        0      402 2023-02-27 05:27:02.253818 fullctl-1.4.0/src/fullctl/django/migrations/0019_default_org.py
+-rw-r--r--   0        0        0      389 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0020_auditlog_action_length.py
+-rw-r--r--   0        0        0     3330 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0021_servicebridgeaction.py
+-rw-r--r--   0        0        0     1077 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py
+-rw-r--r--   0        0        0     1050 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py
+-rw-r--r--   0        0        0     2539 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py
+-rw-r--r--   0        0        0      900 2023-02-27 05:27:02.254818 fullctl-1.4.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py
+-rw-r--r--   0        0        0      837 2023-02-27 05:27:02.255818 fullctl-1.4.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py
+-rw-r--r--   0        0        0     4518 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0027_request_response.py
+-rw-r--r--   0        0        0      457 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0028_request_identifier.py
+-rw-r--r--   0        0        0      427 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0029_response_content.py
+-rw-r--r--   0        0        0      550 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0030_alter_response_content.py
+-rw-r--r--   0        0        0     2496 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.4.0/src/fullctl/django/migrations/__init__.py
+-rw-r--r--   0        0        0      218 2021-10-21 03:49:59.989723 fullctl-1.4.0/src/fullctl/django/models/__init__.py
+-rw-r--r--   0        0        0      150 2022-10-14 13:57:25.208745 fullctl-1.4.0/src/fullctl/django/models/abstract/__init__.py
+-rw-r--r--   0        0        0     3282 2022-06-14 21:13:57.268730 fullctl-1.4.0/src/fullctl/django/models/abstract/alert.py
+-rw-r--r--   0        0        0     3337 2022-10-14 13:57:25.209745 fullctl-1.4.0/src/fullctl/django/models/abstract/base.py
+-rw-r--r--   0        0        0    14848 2023-06-30 20:48:24.070788 fullctl-1.4.0/src/fullctl/django/models/abstract/meta.py
+-rw-r--r--   0        0        0     7822 2023-02-27 05:27:02.255818 fullctl-1.4.0/src/fullctl/django/models/abstract/service_bridge.py
+-rw-r--r--   0        0        0     2682 2023-02-27 05:27:02.256818 fullctl-1.4.0/src/fullctl/django/models/abstract/template.py
+-rw-r--r--   0        0        0      288 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/models/concrete/__init__.py
+-rw-r--r--   0        0        0     7437 2023-02-27 05:27:02.256818 fullctl-1.4.0/src/fullctl/django/models/concrete/account.py
+-rw-r--r--   0        0        0     1884 2023-02-27 05:27:02.256818 fullctl-1.4.0/src/fullctl/django/models/concrete/auditlog.py
+-rw-r--r--   0        0        0     1808 2023-04-15 16:24:16.030446 fullctl-1.4.0/src/fullctl/django/models/concrete/meta.py
+-rw-r--r--   0        0        0     7811 2023-02-27 05:27:02.257818 fullctl-1.4.0/src/fullctl/django/models/concrete/service_bridge.py
+-rw-r--r--   0        0        0    16238 2023-04-15 16:24:16.031446 fullctl-1.4.0/src/fullctl/django/models/concrete/tasks.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.4.0/src/fullctl/django/rest/__init__.py
+-rw-r--r--   0        0        0     8217 2023-02-27 05:27:02.257818 fullctl-1.4.0/src/fullctl/django/rest/api_schema.py
+-rw-r--r--   0        0        0     1143 2021-10-29 12:45:46.966419 fullctl-1.4.0/src/fullctl/django/rest/authentication.py
+-rw-r--r--   0        0        0     1831 2021-06-15 13:03:05.250145 fullctl-1.4.0/src/fullctl/django/rest/core.py
+-rw-r--r--   0        0        0     8517 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/decorators.py
+-rw-r--r--   0        0        0      328 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/fields.py
+-rw-r--r--   0        0        0     1074 2021-10-21 03:50:00.023724 fullctl-1.4.0/src/fullctl/django/rest/filters.py
+-rw-r--r--   0        0        0     1486 2022-10-14 13:57:25.257745 fullctl-1.4.0/src/fullctl/django/rest/mixins.py
+-rw-r--r--   0        0        0     2148 2021-10-29 12:45:46.983419 fullctl-1.4.0/src/fullctl/django/rest/renderers.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.957758 fullctl-1.4.0/src/fullctl/django/rest/route/__init__.py
+-rw-r--r--   0        0        0      352 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/route/aaactl_sync.py
+-rw-r--r--   0        0        0      298 2021-10-21 03:50:00.070725 fullctl-1.4.0/src/fullctl/django/rest/route/account.py
+-rw-r--r--   0        0        0      426 2023-02-27 05:27:02.258818 fullctl-1.4.0/src/fullctl/django/rest/route/service_bridge.py
+-rw-r--r--   0        0        0      342 2023-02-27 05:27:02.259818 fullctl-1.4.0/src/fullctl/django/rest/route/usage.py
+-rw-r--r--   0        0        0     1558 2023-02-27 05:27:02.259818 fullctl-1.4.0/src/fullctl/django/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-15 16:24:16.031446 fullctl-1.4.0/src/fullctl/django/rest/serializers/aaactl_sync.py
+-rw-r--r--   0        0        0     2523 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/serializers/account.py
+-rw-r--r--   0        0        0      518 2023-04-15 16:24:16.032446 fullctl-1.4.0/src/fullctl/django/rest/serializers/meta.py
+-rw-r--r--   0        0        0      807 2022-10-14 13:57:25.258745 fullctl-1.4.0/src/fullctl/django/rest/serializers/org.py
+-rw-r--r--   0        0        0      233 2023-02-27 05:27:02.260818 fullctl-1.4.0/src/fullctl/django/rest/serializers/service_bridge.py
+-rw-r--r--   0        0        0      688 2022-10-14 13:57:25.258745 fullctl-1.4.0/src/fullctl/django/rest/serializers/template.py
+-rw-r--r--   0        0        0      440 2023-02-27 05:27:02.260818 fullctl-1.4.0/src/fullctl/django/rest/serializers/usage.py
+-rw-r--r--   0        0        0      395 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/throttle.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.4.0/src/fullctl/django/rest/urls/__init__.py
+-rw-r--r--   0        0        0      222 2021-10-21 03:50:00.135727 fullctl-1.4.0/src/fullctl/django/rest/urls/aaactl_sync.py
+-rw-r--r--   0        0        0      210 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/urls/account.py
+-rw-r--r--   0        0        0      491 2021-10-29 12:45:46.983419 fullctl-1.4.0/src/fullctl/django/rest/urls/service_bridge.py
+-rw-r--r--   0        0        0     2161 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/rest/urls/service_bridge_proxy.py
+-rw-r--r--   0        0        0      204 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/urls/usage.py
+-rw-r--r--   0        0        0      419 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/usage.py
+-rw-r--r--   0        0        0        0 2021-06-15 13:03:05.251145 fullctl-1.4.0/src/fullctl/django/rest/views/__init__.py
+-rw-r--r--   0        0        0     3258 2022-10-14 13:57:25.258745 fullctl-1.4.0/src/fullctl/django/rest/views/aaactl_sync.py
+-rw-r--r--   0        0        0     2576 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/views/account.py
+-rw-r--r--   0        0        0     7159 2023-04-15 17:32:55.630524 fullctl-1.4.0/src/fullctl/django/rest/views/service_bridge.py
+-rw-r--r--   0        0        0      994 2023-02-27 05:27:02.261818 fullctl-1.4.0/src/fullctl/django/rest/views/template.py
+-rw-r--r--   0        0        0     1410 2023-02-27 05:27:02.261818 fullctl-1.4.0/src/fullctl/django/rest/views/usage.py
+-rw-r--r--   0        0        0    16540 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/settings/__init__.py
+-rw-r--r--   0        0        0     2655 2023-02-27 05:27:02.262818 fullctl-1.4.0/src/fullctl/django/settings/default.py
+-rw-r--r--   0        0        0     1215 2023-02-27 05:27:02.262818 fullctl-1.4.0/src/fullctl/django/signals.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.4.0/src/fullctl/django/social/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.4.0/src/fullctl/django/social/backends/__init__.py
+-rw-r--r--   0        0        0     1206 2021-06-15 13:03:05.252145 fullctl-1.4.0/src/fullctl/django/social/backends/peeringdb.py
+-rw-r--r--   0        0        0     1589 2021-10-21 03:50:00.137727 fullctl-1.4.0/src/fullctl/django/social/backends/twentyc.py
+-rw-r--r--   0        0        0      388 2021-06-15 13:03:05.252145 fullctl-1.4.0/src/fullctl/django/social/pipelines/__init__.py
+-rw-r--r--   0        0        0     4237 2021-04-22 13:27:52.959758 fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
+-rw-r--r--   0        0        0    59951 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.rest.js
+-rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.959758 fullctl-1.4.0/src/fullctl/django/static/common/20c-logo-filled.svg
+-rw-r--r--   0        0        0    21299 2023-02-27 05:27:02.264818 fullctl-1.4.0/src/fullctl/django/static/common/app.css
+-rw-r--r--   0        0        0    19449 2023-02-27 05:27:02.265818 fullctl-1.4.0/src/fullctl/django/static/common/app.js
+-rwxr-xr-x   0        0        0   372526 2021-10-29 12:45:47.007420 fullctl-1.4.0/src/fullctl/django/static/common/favicon.ico
+-rw-r--r--   0        0        0     3380 2021-04-22 13:27:52.960758 fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
+-rw-r--r--   0        0        0     3657 2021-04-22 13:27:52.960758 fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
+-rw-r--r--   0        0        0     3430 2021-04-22 13:27:52.960758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/add.svg
+-rw-r--r--   0        0        0     3819 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/alerts.svg
+-rw-r--r--   0        0        0     2838 2022-06-14 21:13:57.362731 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/api.svg
+-rw-r--r--   0        0        0     1303 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
+-rw-r--r--   0        0        0     2681 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/delete.svg
+-rw-r--r--   0        0        0     5490 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/edit.svg
+-rwxr-xr-x   0        0        0     1172 2021-10-29 12:45:47.024420 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/launch.svg
+-rw-r--r--   0        0        0     1601 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
+-rw-r--r--   0        0        0     3357 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/list.svg
+-rwxr-xr-x   0        0        0     1721 2022-06-14 21:13:57.362731 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/location.svg
+-rw-r--r--   0        0        0     2617 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/logout.svg
+-rwxr-xr-x   0        0        0      726 2021-10-29 12:45:47.026420 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/mail.svg
+-rw-r--r--   0        0        0     2761 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/org.svg
+-rw-r--r--   0        0        0     1597 2022-06-14 21:13:57.599734 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/refresh.svg
+-rw-r--r--   0        0        0     1515 2022-06-14 21:13:57.623735 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/report.svg
+-rw-r--r--   0        0        0     8263 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/settings.svg
+-rw-r--r--   0        0        0     4138 2021-04-22 13:27:52.961758 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/user.svg
+-rwxr-xr-x   0        0        0     2782 2021-10-29 12:45:47.035421 fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/view.svg
+-rw-r--r--   0        0        0     3689 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      169 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-add.svg
+-rw-r--r--   0        0        0      275 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-create.svg
+-rw-r--r--   0        0        0      272 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-list-box.svg
+-rw-r--r--   0        0        0      240 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/md-trash.svg
+-rw-r--r--   0        0        0     5957 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      954 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
+-rw-r--r--   0        0        0      818 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-close.svg
+-rw-r--r--   0        0        0     4482 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/logos/aaactl-dark.svg
+-rw-r--r--   0        0        0     4484 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/logos/aaactl-light.svg
+-rw-r--r--   0        0        0     4512 2023-06-30 20:48:24.071788 fullctl-1.4.0/src/fullctl/django/static/common/logos/aclctl-dark.svg
+-rw-r--r--   0        0        0     2625 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/aclctl-light.svg
+-rwxr-xr-x   0        0        0     3333 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/auditctl-dark.svg
+-rwxr-xr-x   0        0        0     3333 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/auditctl-light.svg
+-rwxr-xr-x   0        0        0    36084 2023-04-15 16:24:16.033446 fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png
+-rwxr-xr-x   0        0        0    36307 2023-04-15 16:24:16.033446 fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-light.png
+-rwxr-xr-x   0        0        0     4680 2022-10-14 13:57:25.295745 fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-dark.svg
+-rw-r--r--   0        0        0     4682 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-light.svg
+-rwxr-xr-x   0        0        0     2579 2021-10-29 12:45:47.035421 fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-dark.svg
+-rw-r--r--   0        0        0     2581 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-light.svg
+-rwxr-xr-x   0        0        0     3857 2021-10-29 12:45:47.035421 fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg
+-rw-r--r--   0        0        0     3859 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-light.svg
+-rwxr-xr-x   0        0        0     4166 2021-10-29 12:45:47.036420 fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-dark.svg
+-rw-r--r--   0        0        0     4168 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-light.svg
+-rwxr-xr-x   0        0        0     4336 2022-06-14 21:13:57.623735 fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg
+-rw-r--r--   0        0        0     4338 2023-04-22 03:42:18.732445 fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-light.svg
+-rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.962758 fullctl-1.4.0/src/fullctl/django/static/common/oauth/20c.svg
+-rw-r--r--   0        0        0      689 2021-04-22 13:27:52.963758 fullctl-1.4.0/src/fullctl/django/static/common/oauth/google.svg
+-rw-r--r--   0        0        0     5222 2023-04-15 16:24:16.033446 fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png
+-rw-r--r--   0        0        0     9186 2021-04-22 13:27:52.963758 fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb.png
+-rw-r--r--   0        0        0     4323 2021-10-21 03:50:00.180728 fullctl-1.4.0/src/fullctl/django/static/common/service_bridge.js
+-rw-r--r--   0        0        0    11545 2023-02-27 05:27:02.266818 fullctl-1.4.0/src/fullctl/django/static/common/themes/dark.css
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.963758 fullctl-1.4.0/src/fullctl/django/static/common/themes/light.css
+-rw-r--r--   0        0        0    31266 2023-06-30 20:48:24.072788 fullctl-1.4.0/src/fullctl/django/static/common/v2/app.css
+-rw-r--r--   0        0        0    50966 2023-06-30 20:48:24.072788 fullctl-1.4.0/src/fullctl/django/static/common/v2/app.js
+-rw-r--r--   0        0        0     9584 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/graph.js
+-rw-r--r--   0        0        0      644 2023-02-27 05:27:02.268818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/add.svg
+-rw-r--r--   0        0        0     4812 2023-02-27 05:27:02.268818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/api.svg
+-rw-r--r--   0        0        0      352 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
+-rw-r--r--   0        0        0      232 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/arrow.svg
+-rw-r--r--   0        0        0      532 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
+-rw-r--r--   0        0        0      423 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/cancel.svg
+-rw-r--r--   0        0        0      274 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/close.svg
+-rw-r--r--   0        0        0     1229 2023-04-15 16:24:16.034446 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/database.svg
+-rw-r--r--   0        0        0      427 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/download.svg
+-rw-r--r--   0        0        0      438 2023-02-27 05:27:02.269818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/envelope.svg
+-rw-r--r--   0        0        0      569 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/eye.svg
+-rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
+-rw-r--r--   0        0        0      404 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/funnel.svg
+-rw-r--r--   0        0        0     1530 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/gear.svg
+-rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/geo-alt.svg
+-rw-r--r--   0        0        0     1975 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/help.svg
+-rw-r--r--   0        0        0      582 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/delete.svg
+-rw-r--r--   0        0        0      438 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/edit.svg
+-rw-r--r--   0        0        0      818 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/options.svg
+-rw-r--r--   0        0        0      447 2023-02-27 05:27:02.270818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list-ul.svg
+-rw-r--r--   0        0        0      553 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/logout.svg
+-rw-r--r--   0        0        0      749 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/org.svg
+-rw-r--r--   0        0        0      331 2023-02-27 05:27:02.271818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/search.svg
+-rw-r--r--   0        0        0     1465 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
+-rw-r--r--   0        0        0      298 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/triangle-fill.svg
+-rw-r--r--   0        0        0      465 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
+-rw-r--r--   0        0        0      190 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
+-rw-r--r--   0        0        0     4138 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/user.svg
+-rw-r--r--   0        0        0     3986 2023-02-27 05:27:02.272818 fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/view-settings.svg
+-rw-r--r--   0        0        0    61189 2023-02-27 05:27:02.273818 fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/help.png
+-rw-r--r--   0        0        0   426086 2023-04-15 16:24:16.037446 fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png
+-rw-r--r--   0        0        0    18080 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/static/common/v2/themes/dark.css
+-rw-r--r--   0        0        0        0 2023-02-27 05:27:02.273818 fullctl-1.4.0/src/fullctl/django/static/common/v2/themes/light.css
+-rw-r--r--   0        0        0      921 2023-02-27 05:27:02.274818 fullctl-1.4.0/src/fullctl/django/tasks/__init__.py
+-rw-r--r--   0        0        0      740 2021-10-21 03:50:00.186728 fullctl-1.4.0/src/fullctl/django/tasks/celery.py
+-rw-r--r--   0        0        0     2385 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/tasks/orm.py
+-rw-r--r--   0        0        0     2232 2023-04-22 03:42:18.733445 fullctl-1.4.0/src/fullctl/django/tasks/qualifiers.py
+-rw-r--r--   0        0        0      374 2023-02-27 05:27:02.274818 fullctl-1.4.0/src/fullctl/django/tasks/util.py
+-rw-r--r--   0        0        0      658 2022-10-14 13:57:25.296744 fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2022-10-14 13:57:25.296744 fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/swagger.html
+-rw-r--r--   0        0        0     8871 2022-10-14 13:57:25.296744 fullctl-1.4.0/src/fullctl/django/templates/common/app/base.html
+-rw-r--r--   0        0        0      211 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/checkbox.html
+-rw-r--r--   0        0        0     1935 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      726 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      355 2021-06-15 13:03:05.254145 fullctl-1.4.0/src/fullctl/django/templates/common/app/index.html
+-rw-r--r--   0        0        0     1974 2021-04-22 13:27:52.964758 fullctl-1.4.0/src/fullctl/django/templates/common/app/manage/permissions.html
+-rw-r--r--   0        0        0     4752 2022-10-14 13:57:25.297744 fullctl-1.4.0/src/fullctl/django/templates/common/app/modal.html
+-rw-r--r--   0        0        0     2668 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/app/navbar.html
+-rw-r--r--   0        0        0      371 2023-02-27 05:27:02.275818 fullctl-1.4.0/src/fullctl/django/templates/common/app/templates.html
+-rw-r--r--   0        0        0     3101 2022-10-14 13:57:25.297744 fullctl-1.4.0/src/fullctl/django/templates/common/auth/login.html
+-rw-r--r--   0        0        0      880 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1110 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth.html
+-rw-r--r--   0        0        0     1996 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/base.html
+-rw-r--r--   0        0        0      333 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/400.html
+-rw-r--r--   0        0        0      367 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/401.html
+-rw-r--r--   0        0        0      375 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/403.html
+-rw-r--r--   0        0        0      377 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/404.html
+-rw-r--r--   0        0        0      456 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/500.html
+-rw-r--r--   0        0        0      597 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/templates/common/errors/base.html
+-rw-r--r--   0        0        0      351 2021-06-15 13:03:05.255145 fullctl-1.4.0/src/fullctl/django/templates/common/errors/details.html
+-rw-r--r--   0        0        0     1229 2022-06-14 21:13:57.992740 fullctl-1.4.0/src/fullctl/django/templates/common/snippets.html
+-rw-r--r--   0        0        0      234 2021-04-22 13:27:52.965758 fullctl-1.4.0/src/fullctl/django/templates/common/tool_base.html
+-rw-r--r--   0        0        0      658 2023-02-27 05:27:02.276818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2023-02-27 05:27:02.276818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html
+-rw-r--r--   0        0        0    12350 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/base.html
+-rw-r--r--   0        0        0      211 2023-02-27 05:27:02.277818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/checkbox.html
+-rw-r--r--   0        0        0     2092 2023-04-15 17:32:55.632524 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
+-rw-r--r--   0        0        0      357 2023-02-27 05:27:02.277818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/delete_selected.html
+-rw-r--r--   0        0        0     1945 2023-04-22 03:42:18.733445 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/footer.html
+-rw-r--r--   0        0        0     1935 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      430 2023-04-15 17:32:55.632524 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
+-rw-r--r--   0        0        0      726 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2023-02-27 05:27:02.278818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      358 2023-02-27 05:27:02.279818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/index.html
+-rw-r--r--   0        0        0     1974 2023-02-27 05:27:02.279818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html
+-rw-r--r--   0        0        0     6317 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/modal.html
+-rw-r--r--   0        0        0     2668 2023-02-27 05:27:02.280818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/navbar.html
+-rw-r--r--   0        0        0      413 2023-02-27 05:27:02.280818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/templates.html
+-rw-r--r--   0        0        0     3048 2023-02-27 05:27:02.280818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/login.html
+-rw-r--r--   0        0        0     1109 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1339 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth.html
+-rw-r--r--   0        0        0     1977 2023-04-15 16:24:16.038446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/base.html
+-rw-r--r--   0        0        0      339 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/400.html
+-rw-r--r--   0        0        0      373 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/401.html
+-rw-r--r--   0        0        0      381 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/403.html
+-rw-r--r--   0        0        0      383 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/404.html
+-rw-r--r--   0        0        0      462 2023-02-27 05:27:02.281818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/500.html
+-rw-r--r--   0        0        0      568 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/base.html
+-rw-r--r--   0        0        0      351 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/details.html
+-rw-r--r--   0        0        0     1661 2023-04-15 16:24:16.039446 fullctl-1.4.0/src/fullctl/django/templates/common/v2/snippets.html
+-rw-r--r--   0        0        0      234 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/tool_base.html
+-rw-r--r--   0        0        0      249 2023-02-27 05:27:02.282818 fullctl-1.4.0/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
+-rw-r--r--   0        0        0        0 2022-06-14 21:13:57.992740 fullctl-1.4.0/src/fullctl/django/templatetags/__init__.py
+-rw-r--r--   0        0        0     3398 2023-04-15 16:24:16.039446 fullctl-1.4.0/src/fullctl/django/templatetags/fullctl_util.py
+-rw-r--r--   0        0        0     3152 2023-02-27 05:27:02.283818 fullctl-1.4.0/src/fullctl/django/testutil.py
+-rw-r--r--   0        0        0     3690 2023-06-30 20:48:24.073788 fullctl-1.4.0/src/fullctl/django/urls.py
+-rw-r--r--   0        0        0     1171 2023-02-27 05:27:02.283818 fullctl-1.4.0/src/fullctl/django/util.py
+-rw-r--r--   0        0        0     1193 2022-10-14 13:57:25.299744 fullctl-1.4.0/src/fullctl/django/validators.py
+-rw-r--r--   0        0        0     2885 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/django/views/__init__.py
+-rw-r--r--   0        0        0      199 2022-10-14 13:57:25.300744 fullctl-1.4.0/src/fullctl/django/views/api_schema.py
+-rw-r--r--   0        0        0      927 2023-04-15 17:32:55.633525 fullctl-1.4.0/src/fullctl/django/views/template.py
+-rw-r--r--   0        0        0        0 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/mrtg/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/mrtg/mock.py
+-rw-r--r--   0        0        0     7664 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/graph/mrtg/rrd.py
+-rw-r--r--   0        0        0        0 2021-06-15 13:03:05.256145 fullctl-1.4.0/src/fullctl/service_bridge/__init__.py
+-rw-r--r--   0        0        0     2706 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/service_bridge/aaactl.py
+-rw-r--r--   0        0        0      940 2023-04-22 03:42:18.733445 fullctl-1.4.0/src/fullctl/service_bridge/auditctl.py
+-rw-r--r--   0        0        0     8510 2023-04-15 16:24:16.052446 fullctl-1.4.0/src/fullctl/service_bridge/client.py
+-rw-r--r--   0        0        0     3419 2023-02-27 05:27:02.285818 fullctl-1.4.0/src/fullctl/service_bridge/data.py
+-rw-r--r--   0        0        0     3239 2023-06-30 20:48:24.074788 fullctl-1.4.0/src/fullctl/service_bridge/devicectl.py
+-rw-r--r--   0        0        0     2577 2023-04-15 16:24:16.053446 fullctl-1.4.0/src/fullctl/service_bridge/ixctl.py
+-rw-r--r--   0        0        0     2651 2023-02-27 05:27:02.286818 fullctl-1.4.0/src/fullctl/service_bridge/nautobot.py
+-rw-r--r--   0        0        0     1699 2023-04-15 16:24:16.054446 fullctl-1.4.0/src/fullctl/service_bridge/pdbctl.py
+-rw-r--r--   0        0        0     1037 2023-04-15 16:24:16.063447 fullctl-1.4.0/src/fullctl/service_bridge/peerctl.py
+-rw-r--r--   0        0        0     1076 2023-04-15 16:24:16.097447 fullctl-1.4.0/src/fullctl/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0     6952 2023-04-15 16:24:16.097447 fullctl-1.4.0/src/fullctl/service_bridge/sot.py
+-rw-r--r--   0        0        0      323 2022-10-14 13:57:25.408743 fullctl-1.4.0/src/fullctl/utils/__init__.py
+-rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 fullctl-1.4.0/PKG-INFO
```

### Comparing `fullctl-1.2.0/LICENSE` & `fullctl-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/README.md` & `fullctl-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/pyproject.toml` & `fullctl-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [tool.poetry]
 name = "fullctl"
 repository = "https://github.com/fullctl/fullctl"
-version = "1.2.0"
+version = "1.4.0"
 description = "Core classes and functions for service applications"
 authors = ["FullCtl <code@fullctl.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Topic :: Software Development",
   "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 #packages = [
 #    { include = "fullctl", from = "src" },
 #]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 # django deps
 Django = "~3.2"
 # >3.5.1 is not backwards compatible
 django-autocomplete-light = "3.5.1"
 django-crispy-forms = "^1.8"
 django-grainy = "^1.9"
@@ -55,15 +54,17 @@
 whitenoise = "^6"
 pyuwsgi = "^2.0.19"
 
 confu = "^1.5"
 grainy = "^1.8.1"
 psycopg2-binary = "^2.8"
 # psycopg = {extras = ["binary"], version = "^3.0.14"}
+# force update
 pyyaml = ">=5"
+munge = ">=1.3.0"
 
 [tool.poetry.dev-dependencies]
 # tests
 coverage = ">=5"
 pytest = ">=6"
 pytest-django = ">=3.8"
 pytest-cov = "*"
```

### Comparing `fullctl-1.2.0/src/fullctl/django/admin.py` & `fullctl-1.4.0/src/fullctl/django/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         "id",
         "source",
         "queue_id",
         "parent",
         "status",
         "op",
         "limit_id",
-        "param",
+        # Params can ge quite large at this point, maybe we
+        # hide it by default? Could do display up to a certain length
+        # "param",
         "time",
         "user",
         "org",
         "created",
         "updated",
     )
     list_filter = ("status", "op")
```

### Comparing `fullctl-1.2.0/src/fullctl/django/auditlog.py` & `fullctl-1.4.0/src/fullctl/django/auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/auth.py` & `fullctl-1.4.0/src/fullctl/django/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,18 @@
         # aaactl will send the X-User header if user personation
         # is currently active - it will hold the aaactl-side ID
         # of the user.
 
         user_id = response.headers.get("X-User")
 
         with current_request() as request:
+            # no request in context, nothing to do
+            if not request:
+                return
+
             if not user_id:
                 # if no X-User header is present, impersonation is stopped
 
                 if (
                     "impersonating" in request.session
                     and request.session["impersonating"] != request.user.id
                 ):
```

### Comparing `fullctl-1.2.0/src/fullctl/django/autocomplete/pdb.py` & `fullctl-1.4.0/src/fullctl/django/autocomplete/pdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/context.py` & `fullctl-1.4.0/src/fullctl/django/context.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/context_processors.py` & `fullctl-1.4.0/src/fullctl/django/context_processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     # TODO abstract so other auth services can be
     # defined
     context.update(
         account_service={
             "urls": {
                 "billing_setup": f"{settings.OAUTH_TWENTYC_URL}/billing/setup?org={org_slug}",
-                "manage_account": f"{settings.OAUTH_TWENTYC_URL}/account/?edit=account",
+                "manage_account": f"{settings.OAUTH_TWENTYC_URL}/account/",
                 # TODO: flesh out to redirect to org/create
                 "create_org": f"{settings.OAUTH_TWENTYC_URL}/account/",
                 "manage_org": f"{settings.OAUTH_TWENTYC_URL}/account/?org={org_slug}",
             },
         },
         # TODO: deprecated
         oauth_manages_org=True,
```

### Comparing `fullctl-1.2.0/src/fullctl/django/decorators.py` & `fullctl-1.4.0/src/fullctl/django/decorators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/fields/__init__.py` & `fullctl-1.4.0/src/fullctl/django/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/fields/service_bridge/__init__.py` & `fullctl-1.4.0/src/fullctl/django/fields/service_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/inet/fields.py` & `fullctl-1.4.0/src/fullctl/django/inet/fields.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/inet/util.py` & `fullctl-1.4.0/src/fullctl/django/inet/util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/inet/validators.py` & `fullctl-1.4.0/src/fullctl/django/inet/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/base.py` & `fullctl-1.4.0/src/fullctl/django/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py` & `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py` & `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_promote_user.py` & `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_promote_user.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_work_task.py` & `fullctl-1.4.0/src/fullctl/django/management/commands/fullctl_work_task.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0001_initial.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0003_auditlog.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0003_auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0008_managementtask.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0008_managementtask.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0009_taskclaim.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0009_taskclaim.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0015_alter_task_parent.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0015_alter_task_parent.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0018_task_schedule.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0018_task_schedule.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0021_servicebridgeaction.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0021_servicebridgeaction.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0027_request_response.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0027_request_response.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0030_alter_response_content.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0030_alter_response_content.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py` & `fullctl-1.4.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/alert.py` & `fullctl-1.4.0/src/fullctl/django/models/abstract/alert.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/base.py` & `fullctl-1.4.0/src/fullctl/django/models/abstract/base.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/meta.py` & `fullctl-1.4.0/src/fullctl/django/models/abstract/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Abstract classes to facilitate the fetching, caching and retrieving of meta data
 sourced from third party sources.
 """
 import json
 import re
+import time
 from datetime import timedelta
 
 import confu.schema
 import requests
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db import models
@@ -97,14 +98,24 @@
     source = models.CharField(max_length=255)
     type = models.CharField(max_length=255, null=True, blank=True)
     url = models.URLField()
     http_status = models.PositiveIntegerField()
     payload = models.JSONField(null=True, blank=True)
     count = models.PositiveIntegerField(default=1)
 
+    valid_http_status = [200]
+
+    # what to do on too many requests
+
+    # how long to wait before retrying
+    retry_429_interval = 1
+
+    # how many times to try before giving up
+    retry_429_tries = 2
+
     processing_error = models.CharField(
         max_length=255,
         help_text="will hold error information if the request came back as a success but reading its data resulted in an error on our end.",
         null=True,
         blank=True,
     )
 
@@ -218,16 +229,32 @@
 
         In this impementation a GET request is sent off using the `requests`
         module and expecting a json response.
         """
 
         url = cls.target_to_url(target)
 
-        print("seding request to", url, " - target - ", target)
-        _resp = cls.send_request(url)
+        _resp = None
+
+        tries = 0
+        while not _resp or _resp.status_code == 429:
+            print("seding request to", url, " - target - ", target)
+            tries += 1
+            _resp = cls.send_request(url)
+
+            # if we get a 429, sleep for a bit and try again
+            if _resp.status_code == 429 and cls.retry_429_tries > tries:
+                print(
+                    cls,
+                    target,
+                    f"got 429, sleeping for {cls.retry_429_interval} seconds",
+                )
+                time.sleep(cls.retry_429_interval)
+            else:
+                break
 
         return cls.process(target, url, _resp.status_code, lambda: _resp.json())
 
     @classmethod
     def send_request(cls, url):
         return requests.get(url)
 
@@ -318,20 +345,28 @@
             raise ValueError(f"`{cls}.Config.{config_name}` property not specified")
 
         return value
 
     @classmethod
     def get_cache(cls, target):
         qset = cls.get_cache_queryset(target)
-        qset = qset.filter(updated__gte=cls.valid_cache_datetime(target))
+        cached = qset.filter(updated__gte=cls.valid_cache_datetime(target)).first()
+
+        if not cached:
+            return None
 
-        if qset.exists():
-            return qset.first()
+        tdiff = time.time() - cached.updated.timestamp()
 
-        return None
+        if cached.http_status == 429:
+            if tdiff > 300:
+                # if the cached request is a 429 and it's older than 5 minutes
+                # we will ignore it and send a new request
+                return None
+
+        return cached
 
     @classmethod
     def get_cache_queryset(cls, target):
         target_field = cls.config("target_field")
         typ = cls.target_to_type(target)
         filters = {target_field: target, "source": cls.config("source_name")}
 
@@ -357,14 +392,15 @@
     @classmethod
     def cache_expiry(cls, target):
         # try to get the expiry from the settings
         try:
             expiry = cls.cache_expiry_from_settings(target)
         except AttributeError:
             expiry = cls.config("cache_expiry")
+
         return expiry
 
     @classmethod
     def valid_cache_datetime(cls, target):
         expiry = cls.cache_expiry(target)
         if expiry is None:
             # no cache expiry, return a date far in the past (100 years)
@@ -419,19 +455,28 @@
             raise NoMetaClassDefined()
 
     def write_meta_data(self, req):
         target_field = self.config("target_field", req.config("target_field"))
         source_name = req.config("source_name")
         target = getattr(req, target_field)
 
+        had_entries = False
+
         for date, _target, data in req.process_response(self, target, timezone.now()):
+            had_entries = True
             self._write_meta_data(
                 req, date, req.prepare_data(data), _target, target_field, source_name
             )
 
+        if not had_entries:
+            # no entries were written, write an empty entry
+            self._write_meta_data(
+                req, timezone.now(), {}, target, target_field, source_name
+            )
+
     def _write_meta_data(self, request, date, data, target, target_field, source_name):
         meta_data_cls = self.meta_data_cls
 
         meta_data_type = meta_data_cls.config("type")
         period = meta_data_cls.config("period")
         start = date - timedelta(seconds=period)
         end = date + timedelta(seconds=period)
```

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/service_bridge.py` & `fullctl-1.4.0/src/fullctl/django/models/abstract/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/template.py` & `fullctl-1.4.0/src/fullctl/django/models/abstract/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/account.py` & `fullctl-1.4.0/src/fullctl/django/models/concrete/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/auditlog.py` & `fullctl-1.4.0/src/fullctl/django/models/concrete/auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/meta.py` & `fullctl-1.4.0/src/fullctl/django/models/concrete/meta.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/service_bridge.py` & `fullctl-1.4.0/src/fullctl/django/models/concrete/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/tasks.py` & `fullctl-1.4.0/src/fullctl/django/models/concrete/tasks.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/api_schema.py` & `fullctl-1.4.0/src/fullctl/django/rest/api_schema.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/authentication.py` & `fullctl-1.4.0/src/fullctl/django/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/core.py` & `fullctl-1.4.0/src/fullctl/django/rest/core.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/decorators.py` & `fullctl-1.4.0/src/fullctl/django/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/filters.py` & `fullctl-1.4.0/src/fullctl/django/rest/filters.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/mixins.py` & `fullctl-1.4.0/src/fullctl/django/rest/mixins.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/renderers.py` & `fullctl-1.4.0/src/fullctl/django/rest/renderers.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/__init__.py` & `fullctl-1.4.0/src/fullctl/django/rest/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/aaactl_sync.py` & `fullctl-1.4.0/src/fullctl/django/rest/serializers/aaactl_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/account.py` & `fullctl-1.4.0/src/fullctl/django/rest/serializers/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/meta.py` & `fullctl-1.4.0/src/fullctl/django/rest/serializers/meta.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/org.py` & `fullctl-1.4.0/src/fullctl/django/rest/serializers/org.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/template.py` & `fullctl-1.4.0/src/fullctl/django/rest/serializers/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/urls/service_bridge_proxy.py` & `fullctl-1.4.0/src/fullctl/django/rest/urls/service_bridge_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         request_fn = getattr(requests, method)
 
         # drf_request = Request(request, parsers=[JSONParser])
         _kwargs = {}
 
         if method in ["post", "put", "patch"]:
             _kwargs.update(json=json.loads(request.body))
+        elif method == "get":
+            _kwargs.update(params=request.GET)
 
         endpoint_remote = endpoint["remote"].format(org_tag=org_tag, **kwargs)
 
         url = f"{host}/api/{endpoint_remote}"
 
         headers = {
             "Authorization": f"Bearer {api_key}",
```

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/aaactl_sync.py` & `fullctl-1.4.0/src/fullctl/django/rest/views/aaactl_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/account.py` & `fullctl-1.4.0/src/fullctl/django/rest/views/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/service_bridge.py` & `fullctl-1.4.0/src/fullctl/django/rest/views/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/template.py` & `fullctl-1.4.0/src/fullctl/django/rest/views/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/usage.py` & `fullctl-1.4.0/src/fullctl/django/rest/views/usage.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/settings/__init__.py` & `fullctl-1.4.0/src/fullctl/django/settings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         # TODO EMAIL_SUBJECT_PREFIX = "[{}] ".format(RELEASE_ENV)
 
         self.set_from_env("EMAIL_HOST")
         self.set_from_env("EMAIL_PORT")
         self.set_from_env("EMAIL_HOST_USER")
         self.set_from_env("EMAIL_HOST_PASSWORD")
         self.set_bool("EMAIL_USE_TLS", True)
+        self.set_option("EMAIL_BACKEND", "django.core.mail.backends.smtp.EmailBackend")
 
         # Application definition
 
         INSTALLED_APPS = [
             "django.contrib.admin",
             "django.contrib.auth",
             "django.contrib.contenttypes",
@@ -311,14 +312,15 @@
         # no default so we error sooner
         self.set_option("AAACTL_URL", "")
         self.set_option("PDBCTL_URL", "")
         self.set_option("PEERCTL_URL", "")
         self.set_option("PREFIXCTL_URL", "")
         self.set_option("IXCTL_URL", "")
         self.set_option("DEVICECTL_URL", "")
+        self.set_option("AUDITCTL_URL", "")
 
     def set_twentyc_social_oauth(self, AAACTL_URL=None):
         """
         This function sets the variables required to OAuth against aaactl using
         django-social-auth. It does not set the SOCIAL_AUTH_PIPELINE or
         AUTHENTICATION_BACKENDS.
         """
@@ -377,14 +379,17 @@
         )
         self.set_option("SOCIAL_AUTH_PIPELINE", SOCIAL_AUTH_PIPELINE)
 
         self.set_option("LOGIN_REDIRECT_URL", "/")
         self.set_option("LOGOUT_REDIRECT_URL", "/login")
         self.set_option("LOGIN_URL", "/login")
 
+        MIDDLEWARE = self.get("MIDDLEWARE")
+        MIDDLEWARE.append("fullctl.django.middleware.TokenValidationMiddleware")
+
     def set_twentyc_service(self, billing_integration=True, propagate_user_fields=True):
         """
         Sets up everything needed for a twentyc service.
 
         billing_integration
         Toggles billing integration with aaactl, if false, billing checks on api end points will be disabled
         """
```

### Comparing `fullctl-1.2.0/src/fullctl/django/settings/default.py` & `fullctl-1.4.0/src/fullctl/django/settings/default.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/signals.py` & `fullctl-1.4.0/src/fullctl/django/signals.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/social/backends/peeringdb.py` & `fullctl-1.4.0/src/fullctl/django/social/backends/peeringdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/social/backends/twentyc.py` & `fullctl-1.4.0/src/fullctl/django/social/backends/twentyc.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.core.min.js` & `fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.core.min.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.rest.js` & `fullctl-1.4.0/src/fullctl/django/static/common/20c/twentyc.rest.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -93,31 +93,31 @@
             },
 
             /**
              * Joins URL parts, removing extra slashes at the edges of the parts.
              *
              * @method url_join
              * @param {String} left - The leftmost URL part.
-             * @param {...String} args - The remaining URL parts.
+             * @param {...(String|Number)} args - The remaining URL parts.
              * @return {String} The joined URL string with removed extra slashes.
              */
             url_join: function(left, ...args) {
                 // Simplified urljoin that gets rid of extra / at the edges
                 // of parts
 
                 let right = [];
                 let trailing_slash = !twentyc.rest.no_end_slash;
 
                 // trim left
-
                 left = left.replace(/\/+$/g, "");
 
                 for (const parts of args) {
                     right = right.concat(
                         parts
+                        .toString()
                         .split("/")
                         .filter((part) => part)
                         .map((part) => this.trim_endpoint(part))
                     );
                 }
 
                 if (!right.length)
@@ -694,21 +694,24 @@
              * This will trigger the `processing` event
              *
              * @method start_processing
              */
 
             start_processing: function() {
                 this.busy = true
+                this.element.addClass("loading")
                 if (!this.loading_shim) {
                     this.loading_shim = $('<div>').addClass("loading-shim")
                     this.element.append(this.loading_shim);
                 }
                 if (!this.loading_shim_disabled)
                     this.loading_shim.show();
 
+                this.element.siblings(".loading-indicator-container").show();
+
                 $(this).trigger("processing");
             },
 
 
             /**
              * Sets the widget state to ready or done with processing
              *
@@ -717,14 +720,16 @@
              * @method done_processing
              */
 
             done_processing: function() {
                 this.busy = false
                 if (this.loading_shim && !window.debug_loading_shim)
                     this.loading_shim.hide();
+                this.element.removeClass("loading")
+                //this.element.siblings(".loading-indicator-container").hide();
                 $(this).trigger("ready");
             },
 
             /**
              * Clones a template element by name and returns it
              *
              * Templates for a widget should be stored within an element inside
@@ -840,17 +845,16 @@
              * Renders non field errors (think server errors, generic errors)
              *
              * @method render_non_field_errors
              * @param {Array} errors list of error strings
              */
 
             render_non_field_errors: function(errors) {
-                var error_node = $('<div>').addClass("alert alert-danger validation-error non-field-errors");
-                let i;
-                for (i = 0; i < errors.length; i++) {
+                error_node = $('<div>').addClass("alert alert-danger validation-error non-field-errors");
+                for (let i = 0; i < errors.length; i++) {
                     $(twentyc.rest).trigger("non-field-error", [errors[i], errors, i, error_node, this]);
                     if (errors[i])
                         error_node.append($('<div>').addClass("non-field-error").text(errors[i]));
                 }
 
                 replace_urls_with_links(error_node);
 
@@ -1053,15 +1057,15 @@
                 for (k in this.payload()) {
                     empty[k] = ""
                 }
                 this.fill(empty);
             },
 
             post_success: function(result) {
-
+                this.element.attr("data-submitted", "true")
             },
 
             post_failure: function(response) {
                 response.field_errors(this.render_error.bind(this));
                 response.non_field_errors(this.render_non_field_errors.bind(this))
             },
 
@@ -1210,38 +1214,39 @@
              * @method start_processing
              */
 
             start_processing: function() {
                 this.busy = true
                 this.element.prop("disabled", true);
                 $(this).trigger("processing");
+                this.element.siblings(".loading-indicator-container").show();
             },
 
 
             /**
              * Sets the widget state to ready or done with processing
              *
              * This will trigger the `ready` event
              *
              * @method done_processing
              */
 
             done_processing: function() {
                 this.busy = false
                 this.element.prop("disabled", false);
+                this.element.siblings(".loading-indicator-container").hide();
                 $(this).trigger("ready");
             },
 
 
             post_success: function(result) {
 
             },
 
             post_failure: function(response) {
-                console.error(response);
                 response.field_errors(this.render_error.bind(this));
                 response.non_field_errors(this.render_non_field_errors.bind(this))
             },
 
 
             bind: function(jq) {
                 this.Widget_bind(jq);
@@ -1292,14 +1297,15 @@
     twentyc.rest.Checkbox = twentyc.cls.extend(
         "Checkbox", {
             payload: function() {
                 var pl = {};
                 pl[this.element.attr('name')] = (this.element.prop("checked") ? true : false);
                 return pl;
             },
+
             bind: function(jq) {
                 this.Widget_bind(jq);
                 this.method = jq.data("api-method") || "POST";
 
                 this.element.on("change", function(ev) {
 
                     var confirm_required = this.element.data("confirm");
@@ -1313,15 +1319,23 @@
 
                     fn(action, this.payload()).then(
                         this.post_success.bind(this),
                         this.post_failure.bind(this)
                     );
                 }.bind(this));
 
-            }
+            },
+
+            post_failure: function(field, error) {
+                this.Input_post_failure(field, error);
+
+                // reset checkbox to previous state
+                this.element.prop("checked", !this.element.prop("checked"));
+            },
+
         },
         twentyc.rest.Input
     );
 
 
     /**
      * Button widget
@@ -1397,14 +1411,15 @@
      *   should be auto-selected, defaults to "selected"
      * - data-load-type: what load method to use, can be "get" or "drf-choices",
      *   with the latter being a way to load in django-rest-framework field values
      *   choices. Defaults to "get"
      * - data-drf-name: relevant if load type is "drf-choices". Specifies the
      *   serializer field name, will default to "name" attribute if not specified.
      * - data-null-option: specify to add a "empty" value option with a label
+     * - data-localstorage-key: specify where to store the selected data in localstorage
      *
      * @class Select
      * @extends twentyc.rest.Input
      * @namespace twentyc.rest
      * @constructor
      * @param {jQuery result} jq jquery result holding the select element
      */
@@ -1416,14 +1431,15 @@
                 this.name_field = jq.data("name-field") || "name"
                 this.id_field = jq.data("id-field") || "id"
                 this.selected_field = jq.data("selected-field") || "selected"
                 this.load_type = jq.data("load-type") || "get"
                 this.drf_name = jq.data("drf-name") || jq.attr("name");
                 this.null_option = jq.data("null-option")
                 this.proxy_data = jq.data("proxy-data")
+                this.localstorage_key = jq.data("localstorage-key")
                 this.Input(jq);
             },
 
             payload: function() {
                 return {
                     "id": this.element.val()
                 }
@@ -1530,16 +1546,19 @@
                         if (selected)
                             opt.attr("selected", true);
                         select.append(opt);
                     });
 
                     if (select_this) {
                         select.val(select_this);
-                        if (select_this != old_val)
-                            select.trigger("change", []);
+                        if (select_this != old_val) {
+                            // on_load_change is used to identify that this change event is
+                            // being triggered by the load method, and not by the user
+                            select.trigger("change", ["on_load_change"]);
+                        }
                     }
 
                     $(this).trigger("load:after", [select, response.content.data, this]);
                 }.bind(this));
             },
 
             /**
@@ -1598,14 +1617,93 @@
                 );
             },
 
             prepare_write_url: function(url) {
                 return url;
             },
 
+            /**
+             * if there is a localstorage_key applies values stored in localstorage on
+             * inital load and attaches change listener to update localstorage.
+             *
+             * @method init_localstorage
+             */
+
+            init_localstorage: function() {
+                if (!this.localstorage_key)
+                    return;
+
+                this.element.on("change", () => {
+                    this.localstorage_set(this.element.val());
+                });
+
+                $(this).one("load:after", () => {
+                    this.localstorage_apply();
+                });
+            },
+
+            /**
+             * if localstorage_key is set, sets localstorage of localstorage_key to
+             * data
+             *
+             * @method localstorage_set
+             * @param {String} data
+             */
+            localstorage_set: function(data) {
+                if (!this.localstorage_key)
+                    return;
+
+                if (this.localstorage_get() == data)
+                    return;
+
+                localStorage.setItem(this.localstorage_key, data);
+            },
+
+            /**
+             * if localstorage_key is set, returns localstorage of localstorage_key
+             *
+             * @method localstorage_get
+             * @returns {String}
+             */
+
+            localstorage_get: function() {
+                if (!this.localstorage_key)
+                    return;
+
+                return localStorage.getItem(this.localstorage_key);
+            },
+
+            /**
+             * if localstorage_key is set, removes localstorage_key from localstorage
+             *
+             * @method localstorage_remove
+             */
+
+            localstorage_remove: function() {
+                if (!this.localstorage_key)
+                    return;
+
+                localStorage.removeItem(this.localstorage_key);
+            },
+
+            /**
+             * if localstorage_key is set, sets the option with the same value as
+             * localstorage as the selected option if the option exists.
+             *
+             * @method localstorage_apply
+             */
+
+            localstorage_apply: function() {
+                if (!this.localstorage_key)
+                    return;
+
+                const val = this.localstorage_get();
+                if (val && this.element.find("option[value='" + val + "']").length > 0)
+                    this.element.val(val);
+            },
 
             bind: function(jq) {
                 this.Widget_bind(jq);
                 this.method = jq.data("api-method") || "POST";
 
                 if (this.load_action)
                     this.load();
@@ -1781,16 +1879,35 @@
              * @param {Mixed} id
              */
 
             reload_row: function(id) {
                 var row = this.find_row(id);
                 if (row) {
                     return this.get(id, this.payload()).then(function(response) {
+
+                        // build new row
                         var new_row = this.insert(response.first())
-                        new_row.insertAfter(row);
+
+                        // find siblings surrounding current row, which we can then
+                        // use the insert the new row at the correct location
+                        //
+                        // note, we can't use the old row itself because it introduces
+                        // weird behaviour in the DOM rendering, to investigate at a later
+                        // point if necessary
+                        var next = row.next();
+                        var prev = row.prev();
+
+                        if (next.length) {
+                            new_row.insertBefore(next);
+                        } else if (prev.length) {
+                            new_row.insertAfter(prev);
+                        } else {
+                            new_row.appendTo(this.list_body);
+                        }
+
                         row.detach();
                     }.bind(this));
                 }
             },
 
             /**
              * Builds the html elements for a row in the list
```

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/20c-logo-filled.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/20c-logo-filled.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/app.css` & `fullctl-1.4.0/src/fullctl/django/static/common/app.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/app.js` & `fullctl-1.4.0/src/fullctl/django/static/common/app.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/favicon.ico` & `fullctl-1.4.0/src/fullctl/django/static/common/favicon.ico`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/add.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/alerts.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/alerts.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/api.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/api.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/delete.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/edit.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/edit.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/launch.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/launch.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/light-mode.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/light-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/list.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/list.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/location.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/location.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/logout.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/mail.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/mail.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/org.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/refresh.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/refresh.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/report.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/report.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/settings.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/user.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/view.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/icon/view.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-close.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/icons/ui-close.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-light.png` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/ctl-mark-light.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/devicectl-dark.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/devicectl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/ixctl-dark.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/ixctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/peerctl-dark.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/peerctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/20c.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/oauth/20c.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/google.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/oauth/google.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png` & `fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb.png` & `fullctl-1.4.0/src/fullctl/django/static/common/oauth/peeringdb.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/service_bridge.js` & `fullctl-1.4.0/src/fullctl/django/static/common/service_bridge.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/themes/dark.css` & `fullctl-1.4.0/src/fullctl/django/static/common/themes/dark.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/app.css` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/app.css`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,18 @@
   height: 100%;
 }
 
 /* Set core body defaults */
 body {
   text-rendering: optimizeSpeed;
   line-height: 1.5;
+  /* always show body scroll bar so we dont get jittery widths between cotent
+   * that overflows and content that doesn't
+   */
+  overflow-y: scroll;
 }
 
 /* A elements that don't have a class get default styles */
 a:not([class]) {
   text-decoration-skip-ink: auto;
 }
 
@@ -102,14 +106,18 @@
   display: none !important;
 }
 
 main {
   flex: 1;
 }
 
+.nowrap {
+  white-space: nowrap;
+}
+
 .btn.primary,
 .btn[data-btn-type="delete"] {
   text-transform: uppercase;
   font-size: var(--fs-300);
   font-weight: var(--fw-semi-bold);
 }
 
@@ -136,14 +144,20 @@
   border-radius: 100vmax;
   display: inline-flex;
   border: 1px solid;
   padding: var(--size-100);
   border-color: var(--theme-secondary-border-color);
 }
 
+.btn.filter {
+  border-radius: 30px / 100%;
+  border: 1px solid;
+  font-size: 12px;
+}
+
 a.btn:hover {
   text-decoration: none;
 }
 
 .btn div {
   display: inline-flex;
 }
@@ -165,34 +179,53 @@
   position: relative;
 }
 
 button:focus {
   outline: none;
 }
 
+/* to make loading shim cover entire area */
+.loading {
+  position: relative;
+}
+
 .loading-shim {
   position: absolute;
   top: 0px;
   left: 0px;
   bottom: 0px;
   right: 0px;
   z-index: 10;
   display: flex;
   align-items: center;
 }
 
+.input-group-text.loading-indicator-container {
+  width: 50px;
+}
+
+.loading-indicator,
 .loading-shim:after {
   content: '';
   display: block;
   background: url("imgs/loading-shim.png") center/contain no-repeat;
   height: 84%;
   width: 100%;
   max-height: 84px;
 }
 
+.loading-indicator-container.fixed {
+  height: 24px;
+  display: inline-block;
+  width: 24px;
+  position: absolute;
+  left: 5px;
+  top: 5px;
+}
+
 .nowrap {
   white-space: nowrap;
 }
 
 .center {
   text-align: center;
 }
@@ -201,14 +234,19 @@
   text-align: right;
 }
 
 .bold {
   font-weight: bold;
 }
 
+.dotted-underline {
+  text-decoration: underline;
+  text-decoration-style: dotted;
+}
+
 .sortable-button {
   cursor: pointer;
 }
 
 .rounded-button {
   border-radius: 50px;
   padding: 12px 16px;
@@ -252,14 +290,20 @@
   text-decoration: underline;
 }
 
 button {
   cursor: pointer;
 }
 
+.label-oneline {
+  white-space: nowrap;
+  display: flex;
+  align-items: center;
+}
+
 @media (min-width: 1900px) {
   .container {
     max-width: 1400px;
   }
 }
 
 div.validation-error {
@@ -323,28 +367,78 @@
   padding-left: 20px;
 }
 
 .indent-on .indent-toggled {
   padding-left: 20px;
 }
 
+/* The switch - the box around the slider */
+.switch {
+  position: relative;
+  display: inline-block;
+  width: 60px;
+  height: 34px;
+}
+
+/* Hide default HTML checkbox */
+.switch input {
+  opacity: 0;
+  width: 0;
+  height: 0;
+}
+
+/* The slider */
+.slider {
+  position: absolute;
+  cursor: pointer;
+  top: 0;
+  left: 0;
+  right: 0;
+  bottom: 0;
+  -webkit-transition: .4s;
+  transition: .4s;
+  border-radius: 34px;
+}
+
+.slider:before {
+  position: absolute;
+  content: "";
+  height: 26px;
+  width: 26px;
+  left: 4px;
+  bottom: 4px;
+  border-radius: 50%;
+  -webkit-transition: .4s;
+  transition: .4s;
+}
+
+input:checked ~ .slider:before {
+  -webkit-transform: translateX(26px);
+  -ms-transform: translateX(26px);
+  transform: translateX(26px);
+}
+
 /**
  * bootstrap overrides
  */
 .form-select.secondary {
   display: inline-block;
   width: fit-content;
   border-radius: var(--size-100);
 }
 
 .alert-warning .btn-warning {
   border: none;
   font-weight: 800;
 }
 
+.filter-hidden {
+  display: none;
+}
+
 /**
  * page
  */
 
 body {
   font-family: 'Inter', sans-serif;
   letter-spacing: 0;
@@ -483,15 +577,15 @@
 }
 
 .list-body .secondary div.row:not(:first-child) {
   margin-top: 3px;
 }
 
 .list-body label {
-  font-size: 11px;
+  font-size: var(--fs-400);
   margin: 0px;
 }
 
 .list-body+.list-no-data {
   display: none;
 }
 
@@ -546,14 +640,21 @@
 
 div.toolbar span.toolbar-control>img.caret {
   position: absolute;
   right: 18px;
   top: 19px;
 }
 
+div.toolbar span.toolbar-control .btn {
+  padding: 8px;
+  margin-left: 5px;
+  margin-right: 5px;
+  display: inline-block;
+}
+
 div.toolbar-field {
   position: relative;
   font-size: 16px;
   letter-spacing: 0;
   line-height: 20px;
   display: inline;
   margin-left: 1px;
@@ -799,14 +900,30 @@
 }
 
 span.icon-as {
   -webkit-mask-image: url(icons/database.svg);
   mask-image: url(icons/database.svg);
 }
 
+span.icon-filter {
+  -webkit-mask-image: url(icons/funnel.svg);
+  mask-image: url(icons/funnel.svg);
+}
+
+span.icon-triangle-fill-up {
+  -webkit-mask-image: url(icons/triangle-fill.svg);
+  mask-image: url(icons/triangle-fill.svg);
+}
+
+span.icon-triangle-fill-down {
+  -webkit-mask-image: url(icons/triangle-fill.svg);
+  mask-image: url(icons/triangle-fill.svg);
+  rotate: 180deg;
+}
+
 [data-true] {
   display: none;
 }
 
 .checked [data-true],
 [data-toggle="checked"] [data-false] {
   display: inline;
@@ -829,14 +946,31 @@
   border-bottom: 2px solid transparent;
 }
 
 a.nav-link.active {
   border-bottom: 2px solid;
 }
 
+.fullctl-inner-tabs .nav .nav-item {
+  margin-right: 10px;
+}
+
+.fullctl-inner-tabs .nav {
+  border: none;
+  margin-bottom: 25px;
+}
+
+.fullctl-inner-tabs .nav .nav-link {
+  border: 0px;
+  border-bottom: 1px solid;
+  border-radius: 0px;
+}
+
+
+
 /**
  * menu
  */
 
 div.menu {
   position: relative;
 }
@@ -870,34 +1004,46 @@
 /**
   * searchbar
   */
 .input-group.searchbar {
   flex-wrap: nowrap;
 }
 
+.input-group.searchbar select.form-select,
 .input-group.searchbar input {
   padding: var(--size-200);
   border-top-left-radius: var(--size-200);
   border-bottom-left-radius: var(--size-200);
   flex: 1;
   border: 1px solid;
+  width: 100%;
 }
 
 .input-group.searchbar .btn {
   border: 1px solid;
   border-top-right-radius: var(--size-200);
   border-bottom-right-radius: var(--size-200);
   padding: var(--size-200);
 }
 
 .input-group.searchbar .btn.curved {
   border-top-right-radius: var(--size-200) !important;
   border-bottom-right-radius: var(--size-200) !important;
 }
 
+.input-group span.static-label {
+  background-color: var(--background);
+  color: var(--foreground);
+  border-color: var(--theme-secondary-border-color);
+}
+
+.input-group.searchbar select.form-select {
+  margin-left: 0px;
+}
+
 /**
   * lists
   */
 .list-table .btn {
   border-radius: 100vmax;
   display: inline-flex;
   border: 1px solid;
@@ -1116,15 +1262,14 @@
 
 div.list-body div.secondary {
   margin-left: 0px;
 }
 
 div.list-body .primary-row-name {
   font-size: 24px;
-  font-weight: bold;
   letter-spacing: 0;
   line-height: 24px;
   margin: 16px 0px;
 }
 
 tbody.list-footer {
   border-top: 1px solid transparent !important;
@@ -1304,31 +1449,14 @@
 div.controls label {
   font-size: 14px;
   line-height: 16px;
   letter-spacing: 2.4px;
   margin-bottom: 12px;
 }
 
-div.controls input[type="checkbox"] {
-  outline: none;
-  box-sizing: border-box;
-  height: 16px;
-  width: 16px;
-  -webkit-appearance: none;
-  -moz-appearance: none;
-  appearance: none;
-}
-
-div.controls input[type="checkbox"]:checked:before {
-  content: '\2713';
-  position: relative;
-  top: -5px;
-  left: 2px;
-}
-
 div.controls .form-check {
   margin-bottom: 15px;
 }
 
 div.controls input[type="checkbox"]~label {
   font-size: 20px;
   letter-spacing: 0;
@@ -1475,15 +1603,15 @@
 
 
 /**
  * footer
  */
 
 footer {
-  margin: 2rem .5rem;
+  padding: 2rem .5rem;
   text-align: center;
 }
 
 .footer-right {
   position: relative;
 }
 
@@ -1586,21 +1714,236 @@
 .cross-promotion .alert {
   padding: 3px;
   border-radius: 0px 5px 5px 0px;
   margin-top: 3px;
   padding-left: 5px;
 }
 
+.notification.bg-info,
 .cross-promotion .alert-info {
-  background-color: #2b2e39;
+  background-color: #2b2e39 !important;
   border-color: #d1ff27;
 }
 
 .cross-promotion .btn {
   padding: 3px;
   font-size: 12px;
 }
 
 .cross-promotion img.app-logo {
   height: 18px;
   display: inline;
-}
+}
+
+img.service-link {
+  height: 25px;
+  border: none;
+  display: inline;
+  vertical-align: middle;
+}
+
+img.service-link ~ span.icon {
+  margin-left: 5px;
+  vertical-align: middle;
+}
+
+/*
+ * autocomplete stylings
+ */
+
+div.autocomplete-item {
+  position: relative;
+  margin: -5px;
+  padding: 5px;
+  border-bottom: 1px solid var(--secondary-list-btn-bg);
+}
+
+div.autocomplete-item .autocomplete-secondary {
+  font-size: 12px;
+}
+
+div.autocomplete-item .autocomplete-extra {
+  font-size: 11px;
+}
+
+div.autocomplete-controls {
+  font-size: 11px;
+  text-align: right;
+}
+
+.modal-control .select2-selection.select2-selection--single {
+  height: 60px;
+  padding: 5px;
+}
+
+.modal-control .select2-selection.select2-selection--single .select2-selection__placeholder {
+  white-space: normal;
+}
+
+.modal-control .autocomplete-primary {
+  height: auto;
+  line-height: initial;
+}
+
+.modal .controls input.select2-search__field {
+  border: none;
+  border-bottom: 1px solid transparent;
+}
+
+.select2-selection.select2-selection--single {
+  height: 42px;
+  padding-left: var(--size-100);
+  display: flex;
+  align-items: center;
+  background-color: transparent;
+}
+
+.select2-container--default .select2-selection--single .select2-selection__arrow {
+  right: 4px;
+  top: initial;
+}
+
+/* table display */
+.table-disp {
+  display: table;
+}
+
+.table-row-disp {
+  display: table-row;
+}
+
+.table-cell-disp {
+  display: table-cell;
+}
+
+div.notifications {
+  position: fixed;
+  top: 75px;
+  left: 50%;
+  transform: translate(-50%);
+  padding: 5px;
+  z-index: 100;
+}
+
+div.notifications .badge.notification {
+  padding: 10px;
+  display: block;
+  margin-bottom: 10px;
+  cursor: pointer;
+  min-width: 200px;
+  max-width: 600px;
+}
+
+div.notifications .badge.notification.bg-info {
+  border-width: 1px;
+  border-style: solid;
+}
+
+/** DropdownBtn */
+
+.dropdown-btn {
+  display: inline-flex;
+  position: relative;
+}
+
+.dropdown-btn > button:not(.active) {
+  display: none;
+}
+
+.dropdown-btn > button {
+  border-top-right-radius: 0px;
+  border-bottom-right-radius: 0px;
+}
+
+.dropdown-btn details[open]::after {
+  content: '';
+  position: fixed;
+  top: 0;
+  left: 0;
+  bottom: 0;
+  right: 0;
+  z-index: 98;
+}
+
+.dropdown-btn summary {
+  height: 100%;
+  display: flex;
+  align-items: center;
+  padding-left: 0.5rem;
+  padding-right: 0.5rem;
+}
+
+.dropdown-btn summary::marker {
+  content: '';
+}
+
+.dropdown-btn summary::before {
+  content: '';
+  display: inline-block;
+  height: var(--size-425);
+  width: var(--size-425);
+  vertical-align: bottom;
+  mask-position: center;
+  -webkit-mask-position: center;
+  mask-repeat: no-repeat;
+  -webkit-mask-repeat: no-repeat;
+  -webkit-mask-image: url(icons/ui-caret/down.svg);
+  mask-image: url(icons/ui-caret/down.svg);
+}
+
+.dropdown-btn summary {
+  border-left: 1px solid;
+  border-top-right-radius: var(--bs-border-radius);
+  border-bottom-right-radius: var(--bs-border-radius);
+}
+
+.dropdown-btn .dropdown-btn-menu {
+  position: absolute;
+  top: 100%;
+  left: 0;
+  margin-top: 4px;
+  z-index: 99;
+  min-width: 100%;
+  display: flex;
+  flex-direction: column;
+  gap: 4px 0;
+}
+
+.dropdown-btn.single-option > button{
+  border-top-right-radius: var(--bs-border-radius);
+  border-bottom-right-radius: var(--bs-border-radius);
+}
+
+.dropdown-btn.single-option details {
+  display: none;
+}
+
+
+/*
+ * badges
+ */
+
+.badge-btn .label {
+  vertical-align: super;
+  text-transform: uppercase;
+}
+
+.badge-btn .icon {
+  vertical-align: baseline;
+}
+
+button.badge-btn {
+  border: none;
+}
+
+button.badge-btn:disabled {
+  opacity: 0.5;
+}
+
+/*
+ * graphs
+ */
+.graph-placeholder {
+  height: 256px;
+  display: block;
+  position: relative;
+}
```

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/app.js` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/app.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,113 @@
 
     fullctl.application = {}
     fullctl.widget = {}
     fullctl.formatters = {}
     fullctl.modals = {}
     fullctl.util = {}
     fullctl.help_box = {}
+    fullctl.auth = {};
     fullctl.static_path = "/s/0.0.0-dev/"
+    fullctl.session_expired = false;
+
+    class NotificationManager {
+        constructor() {
+            this.notifications = [];
+            this.max_notifications = 3;
+        }
+
+        /**
+         * Add a new notification
+         * @param {string} type - notification type (danger, info, success)
+         * @param {string} message - HTML message content
+         * @param {function} [click_handler] - custom click handler (optional)
+         * @param {number} [auto_close_seconds] - auto close in seconds (optional)
+         */
+        add_notification(type, message, click_handler, auto_close_seconds) {
+            // Remove old notification if needed
+            if (this.notifications.length === this.max_notifications) {
+                this.notifications.shift().remove();
+            }
+
+            // Create new notification element
+            const notification = $(`<div class="notification badge bg-${type}">${message}</div>`);
+
+            // Append the notification to the .notifications element
+            $('.notifications').append(notification);
+
+            // Add click listener for custom click handler (if provided) and removing the notification
+            notification.on('click', () => {
+                if (click_handler) {
+                    click_handler();
+                }
+                notification.remove();
+            });
+
+            // Auto close the notification after n seconds (if provided)
+            if (auto_close_seconds) {
+                setTimeout(() => {
+                    notification.remove();
+                }, auto_close_seconds * 1000);
+            }
+
+            // Add to the notifications array
+            this.notifications.push(notification);
+        }
+
+        danger(html_message, click_handler, auto_close_seconds) {
+            this.add_notification("danger", html_message, click_handler, auto_close_seconds);
+        }
+
+        info(html_message, click_handler, auto_close_seconds) {
+            this.add_notification("info", html_message, click_handler, auto_close_seconds);
+        }
+
+        success(html_message, click_handler, auto_close_seconds) {
+            this.add_notification("success", html_message, click_handler, auto_close_seconds);
+        }
+
+    }
+
+    // Create a NotificationManager instance in the window.fullctl namespace
+    fullctl.notification_manager = new NotificationManager();
+
+    /**
+     * starts periodically checking the /authcheck endpoint
+     * and will display an alert if the user is no longer
+     * authenticated
+     *
+     * interval is set to 15 seconds.
+     *
+     * @method start_check
+     */
+    fullctl.auth.start_check = function() {
+        this.auth_check_timer = setInterval(() => {
+            $.get("/authcheck/").fail(() => {
+                clearInterval(this.auth_check_timer);
+                if (!fullctl.session_expired) {
+                    $(fullctl).trigger("session-expired");
+                    fullctl.notification_manager.danger("Your session has expired. <a href=\"\">Reconnect</a>.", () => {
+                        window.location.href = "";
+                    });
+                }
+                fullctl.session_expired = true;
+
+            });
+        }, 15000);
+    }
+
+    /**
+     * stops the periodic auth check
+     *
+     * @method stop_check
+     */
+
+    fullctl.auth.stop_check = function() {
+        clearInterval(this.auth_check_timer);
+    }
 
 
     fullctl.util.slugify = (txt) => {
         return txt.toLowerCase().replace(/\s/g, "-").replace(/_/g, "-").replace(/[^a-zA-Z0-9-]/g, "").replace(/-+/g, '-');
     };
 
     /**
@@ -30,24 +128,48 @@
      * @returns {String} full path to file
      */
 
     fullctl.util.static = (path) => {
         return fullctl.static_path + path;
     };
 
+    fullctl.util.is_valid_ip4 = (ip) => {
+        // Regular expression to match IPv4 addresses with optional prefix length
+        const ipv4Regex = /^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(\/([1-9]|[1-2][0-9]|3[0-2]))?$/;
+
+        // Test the input against the regular expression
+        const isValid = ipv4Regex.test(ip);
+
+        return isValid;
+    }
+
     fullctl.formatters.pretty_speed = (value) => {
         if (value >= 1000000)
             value = parseInt(value / 1000000) + "T";
         else if (value >= 1000)
             value = parseInt(value / 1000) + "G";
         else
             value = value + "M";
         return value
     }
 
+    fullctl.formatters.pretty_speed_bits = (value) => {
+        if (value >= 1000000000000)
+            value = parseInt(value / 1000000000000) + "T";
+        else if (value >= 1000000000)
+            value = parseInt(value / 1000000000) + "G";
+        else if (value >= 1000000)
+            value = parseInt(value / 1000000) + "M";
+        else if (value >= 1000)
+            value = parseInt(value / 1000) + "K";
+        else
+            value = value + "";
+        return value
+    }
+
     fullctl.formatters.monitor_status = (value) => {
         if (value == "ok") {
             return $('<span>').addClass('active').text('Active');
         } else if (value == "deactivated") {
             return $('<span>').addClass('inactive').text('Stopped');
         }
         return value
@@ -61,14 +183,69 @@
         for (k in value) {
             node.append($('<div>').addClass("badge").text(k + ": " + value[k]));
         }
         return node;
     }
 
     /**
+     * Formats a datetime string into a human readable format
+     */
+    fullctl.formatters.datetime = (value) => {
+        const date = new Date(value);
+
+        const year = date.getFullYear();
+        const month = String(date.getMonth() + 1).padStart(2, '0');
+        const day = String(date.getDate()).padStart(2, '0');
+        const hours = String(date.getHours()).padStart(2, '0');
+        const minutes = String(date.getMinutes()).padStart(2, '0');
+        const seconds = String(date.getSeconds()).padStart(2, '0');
+
+        return `${year}-${month}-${day} ${hours}:${minutes}:${seconds}`;
+    }
+
+    /**
+     * Formats seconds as XwXd if its higher than 48 hours
+     * and hh:mm:ss otherwise
+     */
+    fullctl.formatters.seconds_to_wdhms = (seconds) => {
+        seconds = Number(seconds);
+        const w = Math.floor(seconds / (3600 * 24 * 7));
+        const d = Math.floor(seconds % (3600 * 24 * 7) / (3600 * 24));
+
+        const wDisplay = w > 0 ? w + "w" : "";
+        const dDisplay = d > 0 ? d + "d" : "";
+        if (w > 0 || d > 2) {
+            return (wDisplay + dDisplay).replace(/,\s*$/, "");
+        }
+
+        const h = Math.floor(seconds / 3600);
+        const m = Math.floor(seconds % 3600 / 60);
+        const s = Math.floor(seconds % 60);
+
+        return (`${h}:${m}:${s}`);
+    }
+
+    /**
+     * Shortens numbers by prefixing K for thousands and M for millions
+     */
+    fullctl.formatters.shorten_number = (value) => {
+        value = Number(value);
+        const millions = (value / 1000000).toPrecision(3);
+        if (millions > 1) {
+            return millions + "M";
+        }
+
+        const thousands = (value / 1000).toPrecision(3);
+        if (thousands > 1)
+            return thousands + "K";
+
+        return String(value);
+    }
+
+    /**
      * Formats `True` and `False` as checkmark and cross
      * @method pretty_bool
      * @param {String} value value of cell
      * @param {Object} data object literal of row data
      * @param {Object} cell jQuery object for container
      */
 
@@ -125,14 +302,19 @@
 
 
             spinner: function() {
                 return $('<div class="spinner loadingio-spinner-bars-k879i8bcs9"><div class="ldio-a9ruqenne8l"><div></div><div></div><div></div><div></div></div></div>');
             },
 
             load: function() {
+                // stop refreshing if the element is no longer in the DOM
+                if (!document.body.contains(this.element[0])) {
+                    this.refresh_timer.cancel();
+                    return
+                }
                 return this.get().then((response) => {
                     response.rows((row) => {
                         if (row.id == this.row_id) {
                             var value = row[this.field_name];
                             this.render(value, row);
                         }
                     })
@@ -365,33 +547,68 @@
     fullctl.application.Modal = $tc.extend(
         "Modal", {
             Modal: function(type, title, content) {
                 this.Component("modal_" + type)
                 this.set_title(title);
                 this.set_content(content);
 
-                var modal = this;
+                const modal = this;
 
                 content.find('.modal-action-note-text').each(function() {
                     $(this).appendTo(modal.jquery.find('.modal-action-note'))
                 });
 
                 this.show();
+
+                const on_modal_close = (e) => {
+                    if (modal.jquery.find('form').attr('data-submitted') == 'true') {
+                        modal.jquery.find('form').attr('data-submitted', 'false');
+                    } else if (this.changed) {
+                        const conrimation = confirm("Are you sure you want to close this modal? Any unsaved changes will be lost.");
+                        if (!conrimation) {
+                            e.preventDefault();
+                            return;
+                        }
+                    }
+                    this.jquery.off('hide.bs.modal', on_modal_close);
+                }
+                this.jquery.on('hide.bs.modal', on_modal_close);
             },
+
             show: function() {
                 this.jquery.modal('show');
             },
+
             hide: function() {
                 this.jquery.modal('hide');
             },
+
             set_title: function(title) {
                 this.jquery.find('.modal-title').text(title);
             },
+
             set_content: function(content) {
                 this.jquery.find('.modal-body').empty().append(content);
+                this.track_form_changes();
+            },
+
+            track_form_changes: function() {
+                const modal = this;
+                modal.changed = false;
+
+                const form_inputs = this.jquery.find('form :input');
+                const change_setter = function(e, info) {
+                    if (info === "on_load_change") {
+                        return
+                    }
+
+                    modal.changed = true;
+                    form_inputs.off('change', change_setter);
+                }
+                form_inputs.on('change', change_setter);
             }
         },
         fullctl.application.Component
     );
 
     fullctl.application.Tool = $tc.extend(
         "Tool", {
@@ -438,19 +655,23 @@
 
             deactivate: function() {
                 this.active = false
             },
 
             apply_ordering: function() {
                 //deprecated
+                console.warn("use of Tool.apply_ordering is deprecated")
+
                 return;
             },
 
             initialize_sortable_headers: function() {
                 //deprecated
+                console.warn("use of Tool.initialize_sortable_headers is deprecated")
+
                 return;
             },
 
             custom_dialog: function(title) {
                 this.$e.body.empty();
                 var custom_dialog = $('<div>').addClass("tool-custom")
                 custom_dialog.append($('<h4>').addClass("tool-title").text(title));
@@ -547,14 +768,15 @@
                             row.click(() => {
                                 window.location.href = "/" + data.slug + "/";
                             })
                         }
                     });
                     w.load()
 
+                    this.order_app_switcher();
                     this.wire_app_switcher();
                     this.wire_stop_impersonation();
 
                     return w;
                 });
             },
 
@@ -562,15 +784,15 @@
              * wires the service application switcher in the header
              * @method wire_app_switcher
              * @return {void}
              */
 
             wire_app_switcher: function() {
                 this.widget("app_switcher", ($e) => {
-                    var others = $e.app_switcher.find('.others')
+                    const others = $e.app_switcher.find('.others')
                     const selected = $e.app_switcher.find('.selected')
                     selected.click(() => {
                         others.show();
                         selected.addClass('app_bg muted');
                     });
                     $(document.body).click(function(e) {
                         if (
@@ -581,14 +803,31 @@
                         }
                     });
                     return {};
                 });
             },
 
             /**
+             * order elements within the service application switcher in the header
+             * @method order_app_switcher
+             */
+
+            order_app_switcher: function() {
+                const service_list_order = ["ixctl", "peerctl", "devicectl", "prefixctl", "pdbctl", "aclctl", "aaactl"];
+                const service_list = {};
+                $(this.$e.app_switcher).find(".others .list-item").each(function() {
+                    service_list[$(this).attr("data-slug")] = $(this);
+                })
+
+                service_list_order.reverse().forEach((value, index) => {
+                    $(this.$e.app_switcher).find(".others").prepend(service_list[value]);
+                });
+            },
+
+            /**
              * wires the stop impersonation button in the header
              * @method wire_stop_impersonation
              */
 
             wire_stop_impersonation: function() {
 
                 var stop_impersonation = $('[data-element="stop_impersonation"]')
@@ -698,14 +937,16 @@
                         $(button).parents(".alert").find('.msg-trial-started').show();
                     });
                 });
 
 
                 this.application_access_granted = grainy.check("service." + this.id + "." + fullctl.org.id, "r");
 
+                fullctl.auth.start_check();
+
             },
 
             autoload_page: function() {
                 var hash = window.location.hash;
                 if (hash) {
                     hash = hash.substr(1);
 
@@ -734,21 +975,19 @@
             tool: function(name, fn) {
                 fn = fn.bind(this);
                 var tool = this.$t[name] = fn()
                 return tool;
             },
 
             sync: function() {
-                var i, app = this;
-                for (i in this.$t) {
+                for (let i in this.$t) {
                     if (this.$t[i].active) {
-                        this.$t[i].sync(app);
+                        this.$t[i].sync();
                     }
                 }
-
             },
 
             /**
              * Gets the element representing the page in the pages menu.
              *
              * @method get_page
              * @param {String} page Value set for aria-controls
@@ -813,27 +1052,27 @@
                             this.permission_ui();
                         }
                     });
                     return w
                 });
 
                 $(this.$c.toolbar.$w[selector_name]).one("load:after", () => {
-
                     if (this["preselect_" + ref_tag]) {
                         this[selector_name](this["preselect_" + ref_tag])
                     } else {
                         this.sync();
                         this.sync_url(this.$c.toolbar.$e[selector_name].val());
                         this.sync_title(this.$c.toolbar.$e[selector_name].val());
                     }
                 });
 
                 $(this.$c.toolbar.$e[selector_name]).on("change", () => {
                     this.sync();
                     this.sync_url(this.$c.toolbar.$e[selector_name].val())
+                    this.sync_title(this.$c.toolbar.$e[selector_name].val())
                     if (this.$t.settings) {
                         this.$t.settings.sync();
                     }
                 });
 
                 this[ref_tag] = function() {
                     return this.container();
@@ -1186,14 +1425,94 @@
                 if (event.target.closest(".help-box")) return;
                 if (event.target.closest(".help-btn")) return;
                 box.classList.add("js-hide");
             })
         })
     });
 
+    /**
+     * Searchbar component for filtering elements
+     *
+     * @param {*} jq searchbar element
+     * @class Searchbar
+     * @namespace fullctl.application
+     * @constructor
+     * @param {(str) => undefined} filter_function function to call when filtering
+     * @param {() => undefined} clear_filter_function function to reverse what happens in the `filter_function`
+     */
+
+    fullctl.application.Searchbar = $tc.define(
+        "Searchbar", {
+            Searchbar: function(jq, filter_function, clear_filter_function) {
+                const filter_input =
+                    this.filter_input =
+                    this.element =
+                    jq.find('[data-role="filter"]') ||
+                    jq.find('[data-element="filter"]');
+
+                const search_btn =
+                    this.search_btn =
+                    jq.find('[data-role="filter_submit"]') ||
+                    jq.find('[data-element="filter_submit"]');
+
+                const clear_search_btn =
+                    this.clear_search_btn =
+                    jq.find('[data-role="filter_clear"]') ||
+                    jq.find('[data-element="filter_clear"]');
+
+                this.filter_function = filter_function;
+                this.clear_filter_function = clear_filter_function;
+
+                const searchbar = this;
+                filter_input.on("keyup", function(event) {
+                    if (event.key === "Enter") {
+                        if ($(this).val() != "") {
+                            searchbar.search($(this).val())
+                        } else {
+                            searchbar.clear_search();
+                        }
+                    }
+                });
+
+                search_btn.on("click", () => {
+                    if (filter_input.val() != "") {
+                        this.search(filter_input.val())
+                    } else {
+                        this.clear_search();
+                    }
+                });
+
+                clear_search_btn.on("click", () => {
+                    this.clear_search();
+                });
+            },
+
+            search: function(prefix) {
+                this.filter_function(prefix);
+                this.show_clear_button();
+            },
+
+            clear_search: function() {
+                this.filter_input.val("");
+                this.clear_filter_function();
+                this.hide_clear_button();
+            },
+
+            show_clear_button: function() {
+                this.search_btn.removeClass("curved");
+                this.clear_search_btn.show();
+            },
+
+            hide_clear_button: function() {
+                this.search_btn.addClass("curved");
+                this.clear_search_btn.hide();
+            }
+        }
+    );
+
     fullctl.theme_switching = document.addEventListener("DOMContentLoaded", () => {
         function toggle_theme() {
             if (detect_theme() === 'dark')
                 set_theme('light');
             else
                 set_theme('dark');
         }
@@ -1216,16 +1535,369 @@
         document.documentElement.setAttribute('data-theme', detect_theme())
 
         $(".theme-switcher").click(() => {
             toggle_theme();
         });
     });
 
+    /**
+     * Dropdown button widget for selecting options.
+     * should follow a strcuture as follows:
+     *
+     *      <div class="dropdown-btn">
+     *        <button data-option-text="Option 1 text">
+     *          Option 1
+     *        </button>
+     *
+     *        <button data-option-text="Option 2 text">
+     *          Option 1
+     *        </button>
+     *
+     *        <details>
+     *          <summary><span class="visually-hidden">Description of choice</span></summary>
+     *        </details>
+     *      </div>
+     *
+     * @class DropdownBtn
+     * @namespace fullctl.application
+     * @constructor
+     * @param {jQuery} jq - the element to use as the dropdown button
+     */
+
+    fullctl.application.DropdownBtn = $tc.define(
+        "DropdownBtn", {
+            DropdownBtn: function(jq) {
+                this.jq = jq;
+                const element = jq[0];
+                this.dropdown_expand_btn = element.querySelector('details');
+
+                this.menu = $('<div class="dropdown-btn-menu">');
+                this.dropdown_expand_btn.append(this.menu.get(0));
+                this.dropdown_buttons = this.get_dropdown_buttons();
+
+                this.render_dropdown();
+
+                // close dropdown button logic
+                const on_dropdown_btn_open = (event) => {
+                    if (event.target.closest(".dropdown-btn-menu")) return;
+                    this.close_dropdown();
+                    document.removeEventListener('click', on_dropdown_btn_open);
+                }
+                this.dropdown_expand_btn.addEventListener("toggle", (event) => {
+                    if (this.dropdown_expand_btn.open) {
+                        document.addEventListener("click", on_dropdown_btn_open);
+                    }
+                });
+            },
+
+            get_dropdown_buttons: function() {
+                return this.jq.find('> button');
+            },
+
+            close_dropdown: function() {
+                this.dropdown_expand_btn.removeAttribute("open");
+            },
+
+            render_dropdown: function() {
+                this.dropdown_buttons = this.get_dropdown_buttons();
+
+                // add class active to first option if no active
+                if (!this.dropdown_buttons.hasClass('active')) {
+                    this.dropdown_buttons.first().addClass('active');
+                }
+
+                // only show first active if multiple actives
+                this.dropdown_buttons.filter('.active:not(:first)').removeClass('active')
+
+
+                const menu = this.menu
+                menu.empty();
+
+                if (this.dropdown_buttons.length == 1) {
+                    this.jq.addClass('single-option');
+
+                    return;
+                } else {
+                    this.jq.removeClass('single-option');
+                }
+
+                this.dropdown_buttons.each(function() {
+                    menu.append(
+                        $('<button>').text($(this).data('option-text')).data("element-for", $(this))
+                    )
+                });
+
+                this.dropdown_options = menu.children();
+
+                // select option from dropdown
+                const dropdown_btn = this;
+                this.dropdown_options.click(function(event) {
+                    dropdown_btn.select_option(this);
+                });
+
+            },
+
+            select_option: function(option_element) {
+                this.jq.find('.active').removeClass('active');
+                $(option_element).data('element-for').addClass('active');
+                this.close_dropdown();
+            },
+
+            add_option: function(elem) {
+                this.jq.prepend(elem);
+                this.render_dropdown();
+            },
+
+            remove_option: function(index) {
+                this.dropdown_buttons.eq(index).remove();
+                this.dropdown_buttons = this.get_dropdown_buttons();
+                if (!this.dropdown_buttons.hasClass('active')) {
+                    this.dropdown_buttons.first().addClass('active');
+                }
+                this.render_dropdown();
+            },
+        }
+    );
+
+    /**
+     * Holds extension functions and classes that deal
+     * with third party library quality of life utilities
+     * @class fullctl.ext
+     *
+     */
+
+    fullctl.ext = {}
+
+    /**
+     * Select2 extension utilities
+     * @class fullctl.ext.select2
+     */
+
+    fullctl.ext.select2 = {
+
+
+        /**
+         * Initializes autocomplete on a select2 element using
+         * the fullctl autocomplete response schema which contains
+         * a `results` array of objects with the following structure:
+         *
+         * {
+         *   id,
+         *   primary, # primary text (name etc.)
+         *   secondary, # Secondary text (second row, description etc.)
+         *   extra, # Extra text (third row, additional info etc.)
+         * }
+         *
+         * @method init_autocomplete
+         * @param {jQuery} jq - the select2 element
+         * @param {jQuery} parent - the parent element to attach the dropdown to
+         * @param {Object} opt - options
+         * @param {Boolean} opt.controls - whether to show controls to remove the selected element
+         * @param {String} opt.url - the url to fetch the autocomplete data from
+         * @param {String} opt.placeholder - the placeholder text
+         * @param {Function} opt.process - a function to process the autocomplete data
+         * @param {Object} opt.initial - the initial value (object containing id,primary,secondary and extra)
+         * @param {Object} opt.localstorage_key - the key that is used to store the selected value in localstorage
+         */
+
+        init_autocomplete: function(jq, parent, opt) {
+
+            this.element = jq;
+
+            jq.select2({
+                dropdownParent: parent,
+                allowClear: false,
+                ajax: {
+                    url: opt.url,
+                    dataType: 'json',
+                    processResults: function(data, params) {
+                        if (opt.process)
+                            opt.process(data, params.term, params);
+                        return {
+                            results: data.results
+                        }
+                    },
+
+                },
+                width: '20em',
+                placeholder: opt.placeholder,
+
+                templateResult: function(state) {
+
+                    // overrides the template used when an item is rendered into
+                    // the results list
+
+                    if (!state.id) {
+                        return state.text;
+                    }
+
+                    return $('<div>').addClass('autocomplete-item').append(
+                        $('<div>').addClass('autocomplete-primary').text(state.text.primary)
+                    ).append(
+                        $('<div>').addClass('autocomplete-secondary').text(state.text.secondary)
+                    ).append(
+                        $('<div>').addClass('autocomplete-extra').text(state.text.extra)
+                    )
+                },
+                templateSelection: function(state) {
+
+                    // overrides the template used when an item is selected
+
+                    if (!state.id) {
+                        return state.text;
+                    }
+
+                    if (!state.selected_text)
+                        state.selected_text = $(state.element).data('selection_data')
+
+                    return $('<div>').addClass('autocomplete-item').append(
+                        $('<div>').addClass('autocomplete-primary').text(state.selected_text.primary)
+                    ).append(
+                        $('<div>').addClass('autocomplete-secondary').text(state.selected_text.secondary)
+                    ).append(
+                        $('<div>').addClass('autocomplete-extra').text(state.selected_text.extra)
+                    )
+                }
+            });
+
+            // if initial is set, select the initial value
+
+            if (opt.initial) {
+
+                // check if initial is callable
+                if (typeof opt.initial === "function") {
+                    opt.initial((initial) => {
+                        let option = $(new Option(initial.primary, initial.id, true, true))
+                        option.data("selection_data", initial)
+                        jq.append(option.get(0)).trigger("change")
+                    })
+                } else {
+                    let initial = opt.initial;
+                    let option = $(new Option(initial.primary, initial.id, true, true))
+                    option.data("selection_data", initial)
+                    jq.append(option.get(0)).trigger("change")
+                }
+
+            }
+
+            if (opt.controls !== false)
+                this.setup_controls();
+
+            if (opt.localstorage_key)
+                this.localstorage_key = opt.localstorage_key;
+
+            return this
+        },
+
+        setup_controls: function() {
+            // controls that allow removal of selected autocomplete element.
+            let controls = $('<div>').addClass('autocomplete-controls').append(
+                $('<a>').addClass('action').text('remove')
+            ).hide().on("click", () => {
+                this.element.val(null).trigger("change");
+                controls.hide();
+            });
+
+            this.element.on("change", function(e) {
+                if ($(this).val()) {
+                    controls.show();
+                } else {
+                    controls.hide();
+                }
+            });
+
+            // add autocomplete controls to bottom
+            this.element.parent().append(controls);
+        },
+
+        /**
+         *
+         * if there is a localstorage_key applies values stored in localstorage on
+         * inital load and attaches change listener to update localstorage.
+         *
+         * @method init_localstorage
+         */
+
+        init_localstorage: function() {
+            if (!this.localstorage_key)
+                return;
+
+            this.element.on("change", () => {
+                this.localstorage_set(this.element.val());
+            });
+        },
+
+        /**
+         * if localstorage_key is set, sets localstorage of localstorage_key to
+         * data
+         *
+         * @method localstorage_set
+         * @param {String} data
+         */
+        localstorage_set: function(data) {
+            if (!this.localstorage_key)
+                return;
+
+            if (this.localstorage_get() == data)
+                return;
+
+            localStorage.setItem(this.localstorage_key, data);
+        },
+
+        /**
+         * if localstorage_key is set, returns localstorage of localstorage_key
+         *
+         * @method localstorage_get
+         * @returns {String}
+         */
+
+        localstorage_get: function() {
+            if (!this.localstorage_key)
+                return;
+
+            return localStorage.getItem(this.localstorage_key);
+        },
+
+        /**
+         * if localstorage_key is set, removes localstorage_key from localstorage
+         *
+         * @method localstorage_remove
+         */
+
+        localstorage_remove: function() {
+            if (!this.localstorage_key)
+                return;
+
+            localStorage.removeItem(this.localstorage_key);
+        },
+
+        /**
+         * if localstorage_key is set, sets the option with the same value as
+         * localstorage as the selected option if the option exists.
+         *
+         * @method localstorage_apply
+         */
+
+        localstorage_apply: function() {
+            if (!this.localstorage_key)
+                return;
+
+            const val = this.localstorage_get();
+            if (val && this.element.find("option[value='" + val + "']").length > 0)
+                this.element.val(val);
+        },
+    }
+
+
     $.fn.grainy_toggle = function(namespace, level) {
         if (grainy.check(namespace, level)) {
             this.show();
         } else {
             this.hide();
         }
     };
 
+    $(document).on('select2:open', () => {
+        document.querySelector('.select2-search__field').focus();
+    });
+
 })(jQuery, twentyc.cls);
```

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/add.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/api.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/api.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/database.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/database.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/eye.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/eye.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/gear.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/gear.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/help.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/help.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/delete.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/options.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/list/options.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/logout.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/org.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/user.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/view-settings.svg` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/icons/view-settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/help.png` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/help.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/themes/dark.css` & `fullctl-1.4.0/src/fullctl/django/static/common/v2/themes/dark.css`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   --clr-primary-700: hsl(233, 4%, 43%);
   --clr-primary-800: hsl(227, 9%, 19%);
   --clr-primary-900: #191B22;
 
   --clr-accent-400: #D1FF27;
   --clr-accent-500: #FD7E14;
   --clr-accent-600: red;
+  --clr-accent-700: #1E90FF;
 
   --clr-bg-200: rgba(246, 248, 250, 1);
   --clr-bg-210: hsl(210, 14%, 95%);
   --clr-bg-300: #E5E5E5;
   --clr-bg-700: rgba(62, 70, 79, 1);
   --clr-bg-800: rgba(44, 47, 58, 0.96);
   --clr-bg-850: hsl(227, 12%, 14%);
@@ -23,20 +24,14 @@
   --clr-border-200: var(--clr-primary-500);
   --clr-border-400: var(--clr-primary-700);
 
 
   --theme-secondary-border-color: rgba(255, 255, 255, 0.15);
   --theme-toolbar-color: #fff;
 
-  --theme-alert-info-bg: #7747FF;
-  --theme-alert-info-color: #fff;
-  --theme-alert-info-border: rgba(255, 255, 255, 0.12);
-  --theme-alert-info-link-color: #d1ff27;
-
-
 
   --foreground: var(--clr-primary-100);
   --background: var(--clr-bg-900);
 
   /* need to manually find this */
   --clr-filter-black-to-foreground: invert(100%) sepia(2%) saturate(8%) hue-rotate(335deg) brightness(101%) contrast(101%);
 
@@ -51,31 +46,38 @@
   --primary-btn-bg: var(--clr-accent-400);
   --secondary-list-btn-bg: var(--clr-bg-800);
   --box-bg: var(--clr-bg-800);
   --dropdown-svg-url: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='rgb(255, 255, 255)' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");
   --codeblock-even-bg: var(--clr-bg-800);
   --modal-clr: var(--clr-primary-200);
   --modal-bg: var(--clr-bg-700);
+  --switch-bg: var(--clr-bg-850);
+  --switch-active-clr: var(--clr-accent-400);
 
   --bs-body-color: var(--foreground);
   --bs-body-color-rgb: var(--foreground);
   --bs-body-bg: var(--background);
+  --bs-link-color: var(--foreground);
+  --bs-link-hover-color: var(--foreground);
 
   --source-of-truth-icon: url("../logos/ctl-mark-dark.png");
 
+  --clr-bg-loading-indicator: #0c0e14;
+  --default-input-bg: #3b3b3b;
+
+  --graph-placeholder-bg: rgba(0,0,0,0.5);
+
   color-scheme: dark;
 }
 
 :root[data-theme="light"] {
   --theme-bg-secondary: #3E464F;
   --clr-border-400: var(--clr-primary-500);
   --theme-secondary-border-color: rgba(25, 27, 34, 0.15);
 
-
-
   --foreground: var(--clr-primary-900);
   --background: var(--clr-bg-300);
 
   /* need to manually find this */
   --clr-filter-black-to-foreground: invert(7%) sepia(12%) saturate(1104%) hue-rotate(189deg) brightness(99%) contrast(93%);
 
   --footer-clr: var(--clr-primary-700);
@@ -87,17 +89,25 @@
   --header-bg: var(--clr-bg-700);
   --secondary-list-btn-bg: var(--modal-bg);
   --box-bg: var(--clr-bg-200);
   --dropdown-svg-url: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='rgb(0, 0, 0)' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");
   --codeblock-even-bg: var(--clr-bg-200);
   --modal-bg: var(--clr-bg-200);
   --modal-clr: var(--clr-primary-800);
+  --switch-bg: var(--clr-bg-210);
 
   --source-of-truth-icon: url("../logos/ctl-mark-light.png");
 
+  --bs-link-color: rgb(13, 110, 253);
+  --bs-link-hover-color: rgb(13, 110, 253);
+
+  --clr-bg-loading-indicator: #d5d5d5;
+
+  --graph-placeholder-bg: rgba(0,0,0,0.2);
+
   color-scheme: light;
 }
 
 /**
  * Basic styles
  */
 
@@ -117,20 +127,27 @@
 .btn.primary {
   --bs-btn-color: var(--primary-btn-clr);
   --bs-btn-bg: var(--primary-btn-bg);
   --bs-btn-hover-color: var(--primary-btn-clr);
   --bs-btn-hover-bg: var(--primary-btn-bg);
   --bs-btn-active-color: var(--primary-btn-clr);
   --bs-btn-active-bg: var(--primary-btn-bg);
+  --bs-btn-active-border-color: var(--primary-btn-bg);
 }
 
+.bg-primary .icon,
 .btn.primary .icon {
   background-color: var(--primary-btn-clr);
 }
 
+.bg-primary {
+  background-color: var(--primary-btn-bg) !important;
+  color: var(--primary-btn-clr) !important;
+}
+
 .btn.secondary {
   --bs-btn-color: var(--foreground);
   --bs-btn-bg: transparent;
   --bs-btn-hover-color: var(--foreground);
   --bs-btn-hover-bg: transparent;
   --bs-btn-active-color: var(--foreground);
   --bs-btn-active-bg: transparent;
@@ -152,14 +169,25 @@
 }
 
 .modal {
   --bs-modal-bg: var(--modal-bg);
   --bs-modal-color: var(--modal-clr);
 }
 
+.btn.filter {
+  border-color: var(--clr-border-400);
+}
+
+.btn.filter.active {
+  border-color: var(--clr-accent-400);
+}
+.btn.filter.active .icon {
+  background-color: var(--clr-accent-400);
+}
+
 .modal .modal-content div.controls,
 .modal .modal-content div label {
   color : var(--modal-clr);
 }
 
 .btn-close {
   filter: var(--clr-filter-black-to-foreground);
@@ -190,31 +218,58 @@
   color: var(--foreground);
 }
 
 .no-color {
   color: inherit !important;
 }
 
+.slider {
+  border: 1px solid var(--clr-border-400);
+  background-color: var(--switch-bg);
+}
+
+.slider:before {
+  background-color: var(--clr-primary-500);
+}
+
+input:checked ~ .slider:before {
+  background-color: var(--switch-active-clr);
+}
+
+input:focus ~ .slider {
+  box-shadow: 0 0 1px var(--switch-active-clr);
+}
+
 /**
  * Bootstrap overrides
  */
 .form-select {
   color: var(--foreground);
   background-image: var(--dropdown-svg-url);
+  background-color: transparent;
+  border-color: var(--theme-secondary-border-color);
 }
 
-.alert-warning {
-  --bs-alert-color: var(--foreground);
-  --bs-alert-bg: var(--box-bg);
-  --bs-alert-border-color: var(--clr-accent-600);
+
+.toolbar-control .form-select {
+  color: var(--foreground);
+  background-image: url(../../icons/ui-caret-caret/down.svg);
+  background-color: var(--default-input-bg);
+  background-position: right 0.5rem center; /* Adjust these values for horizontal and vertical position */
+  background-repeat: no-repeat;
+  background-size:  0.5rem; /* Adjust this value for the size of the caret */
+  -webkit-appearance: none; /* Remove default caret in Webkit browsers */
+  -moz-appearance: none; /* Remove default caret in Mozilla browsers */
+  appearance: none; /* Remove default caret for other browsers */
+  padding-right: 2rem; /* Add extra padding to the right to make space for the caret */
 }
 
-.alert-warning .btn-warning {
-  background-color: var(--primary-btn-bg);
-  color: var(--primary-btn-clr);
+
+.toolbar-control .form-select:disabled {
+  opacity: 0.5;
 }
 
 /**
  * header
  */
 
 
@@ -327,14 +382,22 @@
   border-color: #760505 !important;
 }
 
 .loading-shim {
   background-color: rgba(0, 0, 0, 0.5);
 }
 
+.loading-indicator-container {
+  background-color: var(--clr-bg-loading-indicator);
+  border-color: var(--theme-secondary-border-color);
+}
+
+table td .loading-indicator-container {
+  background-color: transparent;
+}
 
 a[data-action].prefixctl,
 a[data-action].prefixctl:hover,
 a.prefixctl,
 .prefixctl {
   color: var(--foreground);
 }
@@ -409,14 +472,15 @@
 div.toolbar-field select.secondary,
 select.secondary {
   background-color: transparent;
   border-color: var(--theme-secondary-border-color);
 }
 
 div.controls input[type="text"],
+.input-group.searchbar select.form-select,
 div.controls select.form-control {
   background: transparent;
   border-color: var(--theme-secondary-border-color);
   color: inherit;
 }
 
 div.controls select.form-control option {
@@ -520,48 +584,79 @@
 }
 
 .controls .select2-container--default .select2-selection--single {
   background-color: var(--background);
   border: 1px solid var(--clr-border-400);
 }
 
+.modal-control .select2-container--default .select2-selection--single {
+  background-color: var(--modal-bg);
+  border: 1px solid var(--theme-secondary-border-color);
+}
+
+.modal-control .select2-container--default.select2-container--open .select2-selection--single .select2-selection__arrow b {
+  border-color: transparent transparent var(--foreground) transparent;
+}
+.modal-control .select2-container--default .select2-selection--single .select2-selection__arrow b {
+  border-color: var(--foreground) transparent transparent transparent;
+}
+
+.modal .controls input.select2-search__field {
+  background-color: transparent;
+  border-bottom: 1px solid var(--theme-secondary-border-color);
+  outline: 0;
+}
+
 .controls .select2-container--default .select2-selection--single .select2-selection__rendered {
   color: var(--foreground);
 }
 
 span.select2-dropdown {
   border-color: var(--clr-border-400);
   background-color: var(--background);
+  box-shadow: 5px 5px #0000004d;
+}
+
+.modal span.select2-dropdown {
+  border-color: var(--clr-border-400);
+  background-color: var(--modal-bg);
+  box-shadow: 5px 5px #0000004d;
 }
 
 div.controls label {
   color: var(--th-clr);
 }
 
 div.menu div.menu-deco-border {
   background-color: var(--clr-border-400);
 }
 
 /*
  * bootstrap alerts
  */
 
+.alert {
+  --bs-alert-color: var(--foreground);
+  --bs-alert-bg: var(--box-bg);
+}
+
+.alert-warning {
+  --bs-alert-border-color: var(--clr-accent-600);
+}
+
 .alert-info {
-  font-family: 'Space Mono';
-  font-size: 12px;
-  line-height: 16px;
-  color: var(--theme-alert-info-color);
-  background: var(--theme-alert-info-bg);
-  border-color: var(--theme-alert-info-border);
+  --bs-alert-border-color: var(--clr-accent-400);
 }
 
-.alert-info a {
-  color: var(--theme-alert-info-link-color);
+.alert-warning .btn-warning {
+  background-color: var(--primary-btn-bg);
+  color: var(--primary-btn-clr);
 }
 
+
 tbody.list-footer button {
   border-color: transparent;
 }
 
 .status-badge.issues,
 .status-badge.warning {
   background-color: #f58200 !important;
@@ -638,14 +733,19 @@
 
 .nav a.nav-link.active {
   border-color: var(--clr-accent-400);
   opacity: 1;
 }
 
 
+.fullctl-inner-tabs .nav .nav-link.active {
+  background-color: transparent;
+  color: var(--foreground);
+}
+
 /* loading spinner */
 
 
 @keyframes ldio-a9ruqenne8l {
   0% {
     opacity: 1
   }
@@ -732,7 +832,41 @@
 /**
  * sidebar
  */
 .sidebar[data-element="menu"] .button {
   color: var(--foreground);
   background: transparent;
 }
+
+
+div.autocomplete-item .autocomplete-primary {
+  color: var(--foreground);
+}
+
+
+/**
+ * syntax hl
+*/
+.syntax-highlight-transparent-bg pre {
+  background-color: transparent !important;
+}
+
+/** DropdownBtn */
+.dropdown-btn summary::before {
+  background-color: var(--primary-btn-clr);
+}
+
+.dropdown-btn summary {
+  background-color: var(--primary-btn-bg);
+  border-left-color: var(--primary-btn-clr);
+}
+
+.legend {
+  color: var(--clr-primary-300);
+}
+
+/*
+ * graphs
+ */
+.graph-placeholder {
+  background-color: var(--graph-placeholder-bg);
+}
```

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/__init__.py` & `fullctl-1.4.0/src/fullctl/django/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/celery.py` & `fullctl-1.4.0/src/fullctl/django/tasks/celery.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/orm.py` & `fullctl-1.4.0/src/fullctl/django/tasks/orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from fullctl.django.models import (
     Task,
     TaskAlreadyStarted,
     TaskClaimed,
     TaskSchedule,
     WorkerUnqualified,
 )
-from fullctl.django.models.concrete.tasks import TaskClaim
+from fullctl.django.models.concrete.tasks import TaskClaim, TaskLimitError
 from fullctl.django.tasks import specify_task
 from fullctl.django.tasks.util import worker_id
 
 
 def fetch_task(**filters):
     """
     Checks for the next available and qualifying
@@ -101,9 +101,9 @@
         .first()
     )
     if not schedule:
         return
 
     try:
         schedule.spawn_tasks()
-    except TaskAlreadyStarted:
+    except (TaskAlreadyStarted, TaskLimitError):
         schedule.reschedule()
```

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/qualifiers.py` & `fullctl-1.4.0/src/fullctl/django/tasks/qualifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,11 +95,11 @@
 
     def __str__(self):
         return f"{self.__class__.__name__} {self.limit}"
 
     def check(self, task):
         return (
             task.__class__.objects.filter(
-                status="pending", queue_id__isnull=False
+                status="pending", queue_id__isnull=False, op=task.op
             ).count()
             < self.limit
         )
```

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/redoc.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/redoc.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/swagger.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/apidocs/swagger.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/base.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/import-org.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-create.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-prefs.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/manage/permissions.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/modal.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/modal.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/navbar.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/auth/login.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/auth/login.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth-badge.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/base.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/errors/base.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/errors/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "common/app/base.html" %}
+{% extends "common/v2/app/base.html" %}
 {% block "app_content" %}{% endblock %}
 {% block "error_content" %}
 <div class="page_error">
   <h1>{% block error_title %}{% endblock %}{% block error_status %} (#{{ error.status }}){% endblock %}</h1>
   <pi class="error_descr">
   {% block error_descr %}
   {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends "common/app/base.html" %} {% block "app_content" %}{% endblock %} {%
-block "error_content" %}
+{% extends "common/v2/app/base.html" %} {% block "app_content" %}{% endblock %}
+{% block "error_content" %}
 ****** {% block error_title %}{% endblock %}{% block error_status %} (#{
 { error.status }}){% endblock %} ******
  {% block error_descr %} {% endblock %}
 {% block error_details %} {% endblock %}
 {% block return_home %} {%_block_return_home_label_%}{%_endblock_%} {% endblock
 %}
 {% endblock %}
```

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/snippets.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/snippets.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/base.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 <script src="{% static "autocomplete_light/jquery.post-setup.js" %}" type="text/javascript"></script>
 <script src="{% static "common/v2/app.js" %}" type="text/javascript"></script>
 <script src="{% static "common/service_bridge.js" %}" type="text/javascript"></script>
 {% endblock %}
 
 {% block "css" %}
 {{ block.super }}
-<link rel="stylesheet" type="text/css" href="{% static "common/v2/app.css" %}?v=041208" />
-<link rel="stylesheet" type="text/css" href="{% static "common/v2/themes/dark.css" %}?v=130801" />
 <link rel="stylesheet" type="text/css" href="{% static "admin/css/vendor/select2/select2.css" %}" />
 <link rel="stylesheet" type="text/css" href="{% static "admin/css/autocomplete.css" %}" />
 <link rel="stylesheet" type="text/css" href="{% static "autocomplete_light/select2.css" %}" />
 <link href="https://fonts.googleapis.com/css2?family=Archivo+Narrow:wght@400;500;600;700&display=swap" rel="stylesheet">
 
+<link rel="stylesheet" type="text/css" href="{% static "common/v2/app.css" %}?v=041208" />
+<link rel="stylesheet" type="text/css" href="{% static "common/v2/themes/dark.css" %}?v=130801" />
+
 {% endblock %}
 
 {% block "content" %}
 
 <script>
 fullctl.user = {
   id : {{ request.user.id }},
@@ -81,15 +82,15 @@
         <div class="selected {{ request.app_id }} d-flex align-items-center">
           <img class="app-logo" src="{% static service_logo_dark %}" alt="{{ service_tag }}">
         <span class="icon {{ request.app_id }} icon-caret-y ms-4"></span>
         <div class="others" style="display:none">
           {% for service_app in service_applications %}
           {%   if service_app.slug != service_tag %}
           {%     with "common/logos/"|add:service_app.slug|add:"-dark.svg" as other_app_logo %}
-            <a {% if not service_app.always_show_dashboard %}data-grainy-remove="{{ service_app.grainy }}.{{ request.org.remote_id}}"{% endif %} href="{{ service_app.org_redirect }}">
+            <a class="list-item" {% if not service_app.always_show_dashboard %}data-grainy-remove="{{ service_app.grainy }}.{{ request.org.remote_id}}"{% endif %} href="{{ service_app.org_redirect }}" data-slug="{{ service_app.slug }}">
               {% if not service_app.logo %}
                 <img class="app-logo" src="{% static other_app_logo %}" alt="{{ service_app.slug }}">
               {% else %}
                 <img class="app-logo" src="{{ service_app.logo }}" alt="{{ service_app.slug }}">
               {% endif %}
                 <span class="icon-arrow | icon icon-lg"></span>
             </a>
@@ -234,14 +235,19 @@
 <!-- cross promote trials -->
 
 {% include "common/v2/app/cross-promote-trials.html" %}
 
 <main>
 {% block "error_content" %}{% endblock %}
 
+{% block "notifications" %}
+<div class="notifications">
+</div>
+{% endblock %}
+
 <!-- app trial -->
 
 {% if not request|can_access:service_info.org_namespace %}
 
 <div class="row">
   <div class="col-4"></div>
   <div class="col-4">
```

#### html2text {}

```diff
@@ -6,20 +6,20 @@
 utocomplete.init.js" %}" type="text/javascript">
 orward.js" %}" type="text/javascript">
 elect2.js" %}" type="text/javascript">
 query.post-setup.js" %}" type="text/javascript">
 2/app.js" %}" type="text/javascript">
 ervice_bridge.js" %}" type="text/javascript">
 {% endblock %} {% block "css" %} {{ block.super }}
-2/app.css" %}?v=041208" />
-2/themes/dark.css" %}?v=130801" />
 ss/vendor/select2/select2.css" %}" />
 ss/autocomplete.css" %}" />
 elect2.css" %}" />
- {% endblock %} {% block "content" %}
+
+2/app.css" %}?v=041208" />
+2/themes/dark.css" %}?v=130801" /> {% endblock %} {% block "content" %}
  {% block "header" %}
  {% if request.impersonating %}
 {% blocktrans with user=request.user
 logged_in_user=request.impersonating.superuser %} You are currently
 impersonating {{ user }} - logged in as {{ logged_in_user }} {% endblocktrans
 %}
  %}" data-api-method="POST">[{% trans "Stop Impersonating" %}]
@@ -27,16 +27,17 @@
 {% block "header_left" %}
 [{{ service_tag }}]
 {% for service_app in service_applications %} {% if service_app.slug !=
 service_tag %} {% with "common/logos/"|add:service_app.slug|add:"-dark.svg" as
 other_app_logo %}
 % if not service_app.always_show_dashboard %}data-grainy-remove="{
 { service_app.grainy }}.{{ request.org.remote_id}}"{% endif %} href="{
-{ service_app.org_redirect }}"> {% if not service_app.logo %} [{
-{ service_app.slug }}] {% else %} [{{ service_app.slug }}] {% endif %}
+{ service_app.org_redirect }}" data-slug="{{ service_app.slug }}"> {% if not
+service_app.logo %} [{{ service_app.slug }}] {% else %} [{{ service_app.slug
+}}] {% endif %}
  {% endwith %} {% endif %} {% endfor %}
 {% endblock "header_left" %}
 
 {% block "header_middle" %} {% endblock "header_middle" %}
 {% block "header_right" %} {% block "header_account_panel" %}
  {{ request.org.display_name }}
 
@@ -47,16 +48,16 @@
 Organization"_%}_ {% endif %}
  {{ request.user.username }}
 *** {{ request.user.first_name }} {{ request.user.last_name }} ***
 {{ request.user.email }}
 __{%_trans_"Manage_Profile"_%}_ __{%_trans_"Logout"_%}_
 {% endblock %} {% endblock %}
  {% endblock %}  {% include "common/v2/app/cross-promote-trials.html" %}  {%
-block "error_content" %}{% endblock %}  {% if not request|can_access:
-service_info.org_namespace %}
+block "error_content" %}{% endblock %} {% block "notifications" %}
+{% endblock %}  {% if not request|can_access:service_info.org_namespace %}
 {% if service_info.org_can_trial and not service_info.org_has_access and
 permissions.billing %}
 {% blocktrans trimmed with app_id=request.app_id app_slug=service_info.slug
 app_name=service_info.name org_name=request.org.display_name_verbose %} Start
 your {{ app_name }} trial for {{ org_name }} {% endblocktrans %}
  org_tag=request.org.slug %}" class="primary btn">
 {% trans "Start trial" %}
```

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/footer.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/footer.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 {% load i18n static %}
 <div class="container-fluid">
   <div class="row align-items-center">
     <div class="col footer-left">
+      {% block footer_left %}
       <div class="row align-items-center">
         <div class="col-sm-auto theme-switcher" type="button">
           <span class="icon icon-lg icon-theme-switcher"></span>
         </div>
         <div class="col-auto">
           <a title="Contact support" data-message-type="support" {% if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else %}data-element="feature_request_btn"{% endif %}>Contact Us</a> |
           <a title="Feature request" data-message-type="feature-request" {% if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else %}data-element="feature_request_btn"{% endif %} type="button">
             Feature Request
           </a>
         </div>
       </div>
+      {% endblock %}
     </div>
     <div class="col-auto footer-center">
-      Copyright © 2014 - {{ current_year }} FullCtl, LLC
+      {% block footer_center %}
+        Copyright © 2014 - {{ current_year }} FullCtl, LLC
+      {% endblock %}
     </div>
     <div class="col footer-right">
-      <div class="row align-items-center">
-        <div class="ms-auto col-auto">{{ version }}</div>
+      {% block footer_right %}
+      <div class="row align-items-center justify-content-end">
+        <div class="col-auto">{{ version }}</div>
         <div class="help-box js-hide">
           <div class="banner-img">
             <img src="{% static "common/v2/imgs/help.png" %}" alt="">
           </div>
           <a href="{{ docs_url }}" target="_blank">Help Center</a>
           <a title="Contact support" data-message-type="support" {% if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else %}data-element="feature_request_btn"{% endif %}>Contact Support</a>
           <a href="{{ legal_url }}">Legal Notes</a>
         </div>
         <div class="col-sm-auto help-btn" type="button">
           <span class="icon icon-lg icon-help"></span>
         </div>
       </div>
+      {% endblock %}
     </div>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,13 +1,18 @@
 {% load i18n static %}
+{% block footer_left %}
 % if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else
 %}data-element="feature_request_btn"{% endif %}>Contact Us
  |
 % if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else
 %}data-element="feature_request_btn"{% endif %} type="button"> Feature Request
-Copyright Â© 2014 - {{ current_year }} FullCtl, LLC
+{% endblock %}
+{% block footer_center %} Copyright Â© 2014 - {{ current_year }} FullCtl, LLC
+{% endblock %}
+{% block footer_right %}
 {{ version }}
 2/imgs/help.png" %}" alt="">
 Help_Center
 % if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else
 %}data-element="feature_request_btn"{% endif %}>Contact Support
  Legal_Notes
+{% endblock %}
```

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/modal.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/modal.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/navbar.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/login.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/login.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/base.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/snippets.html` & `fullctl-1.4.0/src/fullctl/django/templates/common/v2/snippets.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templatetags/fullctl_util.py` & `fullctl-1.4.0/src/fullctl/django/templatetags/fullctl_util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/testutil.py` & `fullctl-1.4.0/src/fullctl/django/testutil.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/urls.py` & `fullctl-1.4.0/src/fullctl/django/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,26 +52,40 @@
         path(
             "autocomplete/pdb/org",
             fullctl.django.autocomplete.pdb.peeringdb_org.as_view(),
             name="pdb org autocomplete",
         ),
     ]
 
+if getattr(settings, "DEVICECTL_URL", None):
+    import fullctl.django.autocomplete.devicectl
+
+    urlpatterns += [
+        path(
+            "autocomplete/device/port",
+            fullctl.django.autocomplete.devicectl.devicectl_port.as_view(),
+            name="devicectl port autocomplete",
+        ),
+    ]
+
+
 if settings.DEBUG:
     # support version ignorant serving of static files
     urlpatterns += [
         re_path(r"^s/[^\/]+/(?P<path>.*)$", static_file_views.serve),
     ]
 
 
 for import_path, namespace in getattr(settings, "FULLCTL_ADDON_URLS", []):
     urlpatterns += [path("", include((import_path, namespace), namespace=namespace))]
 
 urlpatterns += [
     path("_diag", fullctl.django.views.diag),
+    path("health/", fullctl.django.views.healthcheck),
+    path("authcheck/", fullctl.django.views.authcheck),
     path("apidocs/schema.json", api_schema, name="api_schema"),
     path(
         "api/account/",
         include(
             ("fullctl.django.rest.urls.account", "fullctl_account_api"),
             namespace="fullctl_account_api",
         ),
```

### Comparing `fullctl-1.2.0/src/fullctl/django/util.py` & `fullctl-1.4.0/src/fullctl/django/util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/validators.py` & `fullctl-1.4.0/src/fullctl/django/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/views/__init__.py` & `fullctl-1.4.0/src/fullctl/django/views/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import re
 import sys
 
 from django.conf import settings
+from django.db import connection
 
 # from django.conf import settings
 from django.http import Http404, HttpResponse
 from django.shortcuts import redirect, render
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 
@@ -29,14 +30,39 @@
             continue
         # if k.startswith("HTTP"):
         txt += f"{k}: {v}\n"
 
     return HttpResponse(mark_safe(f"<div><pre>Meta:\n{escape(txt)}</pre></div>"))
 
 
+def healthcheck(request):
+    """
+    Performs a simple database version query
+    """
+
+    with connection.cursor() as cursor:
+        cursor.execute("SELECT version()")
+
+    return HttpResponse("")
+
+
+def authcheck(request):
+    """
+    Checks if the user's access token is still valid
+
+    The check itself is performed by middleware, status of the resonse
+    will be set to 401 if the token is invalid. 200 otherwise.
+    """
+
+    if not request.user.is_authenticated:
+        return HttpResponse("", status=401)
+
+    return HttpResponse("")
+
+
 @require_auth()
 def login(request):
     return redirect("/")
 
 
 def logout(request):
     response = redirect(f"{settings.AAACTL_URL}/account/auth/logout/")
```

### Comparing `fullctl-1.2.0/src/fullctl/django/views/template.py` & `fullctl-1.4.0/src/fullctl/django/views/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/aaactl.py` & `fullctl-1.4.0/src/fullctl/service_bridge/aaactl.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,7 +101,12 @@
 
         self.destroy(impersonation)
 
 
 class ContactMessage(Aaactl):
     class Meta(Aaactl.Meta):
         ref_tag = "contact_message"
+
+
+class OauthAccessToken(Aaactl):
+    class Meta(Aaactl.Meta):
+        ref_tag = "oauth_access_token"
```

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/client.py` & `fullctl-1.4.0/src/fullctl/service_bridge/client.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/data.py` & `fullctl-1.4.0/src/fullctl/service_bridge/data.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/ixctl.py` & `fullctl-1.4.0/src/fullctl/service_bridge/ixctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/nautobot.py` & `fullctl-1.4.0/src/fullctl/service_bridge/nautobot.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/pdbctl.py` & `fullctl-1.4.0/src/fullctl/service_bridge/pdbctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/peerctl.py` & `fullctl-1.4.0/src/fullctl/service_bridge/peerctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/prefixctl.py` & `fullctl-1.4.0/src/fullctl/service_bridge/prefixctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/sot.py` & `fullctl-1.4.0/src/fullctl/service_bridge/sot.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/PKG-INFO` & `fullctl-1.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 Metadata-Version: 2.1
 Name: fullctl
-Version: 1.2.0
+Version: 1.4.0
 Summary: Core classes and functions for service applications
 Home-page: https://github.com/fullctl/fullctl
 License: Apache-2.0
 Author: FullCtl
 Author-email: code@fullctl.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Dist: Django (>=3.2,<3.3)
 Requires-Dist: confu (>=1.5,<2.0)
 Requires-Dist: django-autocomplete-light (==3.5.1)
 Requires-Dist: django-crispy-forms (>=1.8,<2.0)
 Requires-Dist: django-grainy (>=1.9,<2.0)
 Requires-Dist: django-handleref (>=1,<2)
@@ -32,14 +26,15 @@
 Requires-Dist: django-netfields (<2)
 Requires-Dist: django-peeringdb (>=2.8,<3.0)
 Requires-Dist: django-recaptcha (>=2,<3)
 Requires-Dist: django-reversion (>=5,<6)
 Requires-Dist: django-structlog (>=2.1.3,<3.0.0)
 Requires-Dist: djangorestframework (>=3,<4)
 Requires-Dist: grainy (>=1.8.1,<2.0.0)
+Requires-Dist: munge (>=1.3.0)
 Requires-Dist: psycopg2-binary (>=2.8,<3.0)
 Requires-Dist: pyuwsgi (>=2.0.19,<3.0.0)
 Requires-Dist: pyyaml (>=5)
 Requires-Dist: setuptools
 Requires-Dist: social-auth-app-django (>=5.2)
 Requires-Dist: whitenoise (>=6,<7)
 Project-URL: Repository, https://github.com/fullctl/fullctl
```

